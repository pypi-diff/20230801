# Comparing `tmp/mypy-boto3-cloudwatch-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-cloudwatch-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-cloudwatch-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:44 2023, max compression
+gzip compressed data, was "mypy-boto3-cloudwatch-1.28.16.tar", last modified: Tue Aug  1 11:36:25 2023, max compression
```

## Comparing `mypy-boto3-cloudwatch-1.28.15.post1.tar` & `mypy-boto3-cloudwatch-1.28.16.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:44.845063 mypy-boto3-cloudwatch-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:40:19.000000 mypy-boto3-cloudwatch-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21131 2023-07-29 10:02:44.845063 mypy-boto3-cloudwatch-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19626 2023-07-29 09:40:19.000000 mypy-boto3-cloudwatch-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:44.845063 mypy-boto3-cloudwatch-1.28.15.post1/mypy_boto3_cloudwatch/
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-07-29 09:40:19.000000 mypy-boto3-cloudwatch-1.28.15.post1/mypy_boto3_cloudwatch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-07-29 09:40:19.000000 mypy-boto3-cloudwatch-1.28.15.post1/mypy_boto3_cloudwatch/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-29 09:40:19.000000 mypy-boto3-cloudwatch-1.28.15.post1/mypy_boto3_cloudwatch/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33764 2023-07-29 09:40:19.000000 mypy-boto3-cloudwatch-1.28.15.post1/mypy_boto3_cloudwatch/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    33711 2023-07-29 09:40:19.000000 mypy-boto3-cloudwatch-1.28.15.post1/mypy_boto3_cloudwatch/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11219 2023-07-29 09:40:20.000000 mypy-boto3-cloudwatch-1.28.15.post1/mypy_boto3_cloudwatch/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11217 2023-07-29 09:40:20.000000 mypy-boto3-cloudwatch-1.28.15.post1/mypy_boto3_cloudwatch/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8940 2023-07-29 09:40:20.000000 mypy-boto3-cloudwatch-1.28.15.post1/mypy_boto3_cloudwatch/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8931 2023-07-29 09:40:19.000000 mypy-boto3-cloudwatch-1.28.15.post1/mypy_boto3_cloudwatch/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:40:19.000000 mypy-boto3-cloudwatch-1.28.15.post1/mypy_boto3_cloudwatch/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    23164 2023-07-29 09:40:19.000000 mypy-boto3-cloudwatch-1.28.15.post1/mypy_boto3_cloudwatch/service_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    23119 2023-07-29 09:40:19.000000 mypy-boto3-cloudwatch-1.28.15.post1/mypy_boto3_cloudwatch/service_resource.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    45680 2023-07-29 09:40:22.000000 mypy-boto3-cloudwatch-1.28.15.post1/mypy_boto3_cloudwatch/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    45631 2023-07-29 09:40:22.000000 mypy-boto3-cloudwatch-1.28.15.post1/mypy_boto3_cloudwatch/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:40:19.000000 mypy-boto3-cloudwatch-1.28.15.post1/mypy_boto3_cloudwatch/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-07-29 09:40:20.000000 mypy-boto3-cloudwatch-1.28.15.post1/mypy_boto3_cloudwatch/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-07-29 09:40:20.000000 mypy-boto3-cloudwatch-1.28.15.post1/mypy_boto3_cloudwatch/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:44.845063 mypy-boto3-cloudwatch-1.28.15.post1/mypy_boto3_cloudwatch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21131 2023-07-29 10:02:44.000000 mypy-boto3-cloudwatch-1.28.15.post1/mypy_boto3_cloudwatch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-29 10:02:44.000000 mypy-boto3-cloudwatch-1.28.15.post1/mypy_boto3_cloudwatch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:44.000000 mypy-boto3-cloudwatch-1.28.15.post1/mypy_boto3_cloudwatch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:44.000000 mypy-boto3-cloudwatch-1.28.15.post1/mypy_boto3_cloudwatch.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:44.000000 mypy-boto3-cloudwatch-1.28.15.post1/mypy_boto3_cloudwatch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-29 10:02:44.000000 mypy-boto3-cloudwatch-1.28.15.post1/mypy_boto3_cloudwatch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:44.869063 mypy-boto3-cloudwatch-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-07-29 09:40:19.000000 mypy-boto3-cloudwatch-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:25.540928 mypy-boto3-cloudwatch-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:12:51.000000 mypy-boto3-cloudwatch-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21399 2023-08-01 11:36:25.532928 mypy-boto3-cloudwatch-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19903 2023-08-01 11:12:51.000000 mypy-boto3-cloudwatch-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:25.532928 mypy-boto3-cloudwatch-1.28.16/mypy_boto3_cloudwatch/
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-08-01 11:12:51.000000 mypy-boto3-cloudwatch-1.28.16/mypy_boto3_cloudwatch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-08-01 11:12:51.000000 mypy-boto3-cloudwatch-1.28.16/mypy_boto3_cloudwatch/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-08-01 11:12:51.000000 mypy-boto3-cloudwatch-1.28.16/mypy_boto3_cloudwatch/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32859 2023-08-01 11:12:53.000000 mypy-boto3-cloudwatch-1.28.16/mypy_boto3_cloudwatch/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32806 2023-08-01 11:12:51.000000 mypy-boto3-cloudwatch-1.28.16/mypy_boto3_cloudwatch/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11219 2023-08-01 11:12:53.000000 mypy-boto3-cloudwatch-1.28.16/mypy_boto3_cloudwatch/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11217 2023-08-01 11:12:53.000000 mypy-boto3-cloudwatch-1.28.16/mypy_boto3_cloudwatch/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8848 2023-08-01 11:12:53.000000 mypy-boto3-cloudwatch-1.28.16/mypy_boto3_cloudwatch/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8839 2023-08-01 11:12:53.000000 mypy-boto3-cloudwatch-1.28.16/mypy_boto3_cloudwatch/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:12:51.000000 mypy-boto3-cloudwatch-1.28.16/mypy_boto3_cloudwatch/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    23163 2023-08-01 11:12:53.000000 mypy-boto3-cloudwatch-1.28.16/mypy_boto3_cloudwatch/service_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23118 2023-08-01 11:12:53.000000 mypy-boto3-cloudwatch-1.28.16/mypy_boto3_cloudwatch/service_resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    46341 2023-08-01 11:12:54.000000 mypy-boto3-cloudwatch-1.28.16/mypy_boto3_cloudwatch/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46292 2023-08-01 11:12:54.000000 mypy-boto3-cloudwatch-1.28.16/mypy_boto3_cloudwatch/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:12:51.000000 mypy-boto3-cloudwatch-1.28.16/mypy_boto3_cloudwatch/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-08-01 11:12:53.000000 mypy-boto3-cloudwatch-1.28.16/mypy_boto3_cloudwatch/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-08-01 11:12:53.000000 mypy-boto3-cloudwatch-1.28.16/mypy_boto3_cloudwatch/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:25.532928 mypy-boto3-cloudwatch-1.28.16/mypy_boto3_cloudwatch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21399 2023-08-01 11:36:25.000000 mypy-boto3-cloudwatch-1.28.16/mypy_boto3_cloudwatch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-08-01 11:36:25.000000 mypy-boto3-cloudwatch-1.28.16/mypy_boto3_cloudwatch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:25.000000 mypy-boto3-cloudwatch-1.28.16/mypy_boto3_cloudwatch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:25.000000 mypy-boto3-cloudwatch-1.28.16/mypy_boto3_cloudwatch.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:25.000000 mypy-boto3-cloudwatch-1.28.16/mypy_boto3_cloudwatch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-01 11:36:25.000000 mypy-boto3-cloudwatch-1.28.16/mypy_boto3_cloudwatch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:25.540928 mypy-boto3-cloudwatch-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-08-01 11:12:51.000000 mypy-boto3-cloudwatch-1.28.16/setup.py
```

### Comparing `mypy-boto3-cloudwatch-1.28.15.post1/LICENSE` & `mypy-boto3-cloudwatch-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudwatch-1.28.15.post1/PKG-INFO` & `mypy-boto3-cloudwatch-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cloudwatch
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.CloudWatch 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.CloudWatch 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 cloudwatch type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 cloudwatch type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudwatch.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudwatch)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cloudwatch)](https://pepy.tech/project/mypy-boto3-cloudwatch)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudWatch 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch)
+[boto3.CloudWatch 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch)
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
 [mypy-boto3-cloudwatch docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch/).
 
 See how it helps to find and fix potential bugs:
 
@@ -78,15 +78,15 @@
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Waiters annotations](#waiters-annotations)
     - [Service Resource annotations](#service-resource-annotations)
     - [Other resources annotations](#other-resources-annotations)
     - [Collections annotations](#collections-annotations)
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
@@ -436,51 +436,48 @@
 )
 
 
 def check_value(value: ActionsSuppressedByType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_cloudwatch.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_cloudwatch.type_defs import (
     AlarmHistoryItemTypeDef,
     RangeOutputTypeDef,
-    RangeTypeDef,
     DimensionTypeDef,
     CompositeAlarmTypeDef,
     DashboardEntryTypeDef,
     DashboardValidationMessageTypeDef,
     DatapointTypeDef,
     DeleteAlarmsInputRequestTypeDef,
     DeleteDashboardsInputRequestTypeDef,
     DeleteInsightRulesInputRequestTypeDef,
     PartialFailureTypeDef,
     ResponseMetadataTypeDef,
     DeleteMetricStreamInputRequestTypeDef,
-    DescribeAlarmHistoryInputAlarmDescribeHistoryTypeDef,
+    TimestampTypeDef,
     PaginatorConfigTypeDef,
-    DescribeAlarmHistoryInputRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeAlarmsInputRequestTypeDef,
     DescribeInsightRulesInputRequestTypeDef,
     InsightRuleTypeDef,
     DimensionFilterTypeDef,
     DisableAlarmActionsInputRequestTypeDef,
     DisableInsightRulesInputRequestTypeDef,
     EnableAlarmActionsInputRequestTypeDef,
     EnableInsightRulesInputRequestTypeDef,
     GetDashboardInputRequestTypeDef,
-    GetInsightRuleReportInputRequestTypeDef,
     InsightRuleMetricDatapointTypeDef,
     LabelOptionsTypeDef,
     MessageDataTypeDef,
     GetMetricStreamInputRequestTypeDef,
     MetricStreamFilterOutputTypeDef,
     GetMetricWidgetImageInputRequestTypeDef,
     InsightRuleContributorDatapointTypeDef,
@@ -497,19 +494,16 @@
     PutDashboardInputRequestTypeDef,
     SetAlarmStateInputAlarmSetStateTypeDef,
     SetAlarmStateInputRequestTypeDef,
     StartMetricStreamsInputRequestTypeDef,
     StopMetricStreamsInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     AnomalyDetectorConfigurationOutputTypeDef,
-    AnomalyDetectorConfigurationTypeDef,
     DescribeAlarmsForMetricInputRequestTypeDef,
     DescribeAnomalyDetectorsInputRequestTypeDef,
-    GetMetricStatisticsInputMetricGetStatisticsTypeDef,
-    GetMetricStatisticsInputRequestTypeDef,
     MetricOutputTypeDef,
     MetricTypeDef,
     SingleMetricAnomalyDetectorOutputTypeDef,
     SingleMetricAnomalyDetectorTypeDef,
     DeleteInsightRulesOutputTypeDef,
     DescribeAlarmHistoryOutputTypeDef,
     DisableInsightRulesOutputTypeDef,
@@ -518,14 +512,20 @@
     GetDashboardOutputTypeDef,
     GetMetricStatisticsOutputTypeDef,
     GetMetricWidgetImageOutputTypeDef,
     ListDashboardsOutputTypeDef,
     PutDashboardOutputTypeDef,
     PutManagedInsightRulesOutputTypeDef,
     PutMetricStreamOutputTypeDef,
+    DescribeAlarmHistoryInputAlarmDescribeHistoryTypeDef,
+    DescribeAlarmHistoryInputRequestTypeDef,
+    GetInsightRuleReportInputRequestTypeDef,
+    GetMetricStatisticsInputMetricGetStatisticsTypeDef,
+    GetMetricStatisticsInputRequestTypeDef,
+    RangeTypeDef,
     DescribeAlarmHistoryInputDescribeAlarmHistoryPaginateTypeDef,
     DescribeAlarmsInputDescribeAlarmsPaginateTypeDef,
     DescribeAnomalyDetectorsInputDescribeAnomalyDetectorsPaginateTypeDef,
     ListDashboardsInputListDashboardsPaginateTypeDef,
     DescribeAlarmsInputAlarmExistsWaitTypeDef,
     DescribeAlarmsInputCompositeAlarmExistsWaitTypeDef,
     DescribeInsightRulesOutputTypeDef,
@@ -537,45 +537,52 @@
     ListTagsForResourceOutputTypeDef,
     ManagedRuleTypeDef,
     PutCompositeAlarmInputRequestTypeDef,
     PutInsightRuleInputRequestTypeDef,
     TagResourceInputRequestTypeDef,
     ManagedRuleDescriptionTypeDef,
     MetricDatumTypeDef,
+    MetricStreamFilterUnionTypeDef,
     MetricStreamStatisticsConfigurationOutputTypeDef,
     MetricStreamStatisticsConfigurationTypeDef,
     ListMetricsOutputTypeDef,
     MetricStatOutputTypeDef,
     MetricStatTypeDef,
+    SingleMetricAnomalyDetectorUnionTypeDef,
+    AnomalyDetectorConfigurationTypeDef,
     GetMetricDataOutputTypeDef,
     GetInsightRuleReportOutputTypeDef,
     PutManagedInsightRulesInputRequestTypeDef,
     ListManagedInsightRulesOutputTypeDef,
     PutMetricDataInputRequestTypeDef,
     GetMetricStreamOutputTypeDef,
-    PutMetricStreamInputRequestTypeDef,
+    MetricStreamStatisticsConfigurationUnionTypeDef,
     MetricDataQueryOutputTypeDef,
     MetricDataQueryTypeDef,
+    AnomalyDetectorConfigurationUnionTypeDef,
+    PutMetricStreamInputRequestTypeDef,
     MetricAlarmTypeDef,
     MetricMathAnomalyDetectorOutputTypeDef,
-    GetMetricDataInputGetMetricDataPaginateTypeDef,
-    GetMetricDataInputRequestTypeDef,
+    MetricDataQueryUnionTypeDef,
     MetricMathAnomalyDetectorTypeDef,
     PutMetricAlarmInputMetricPutAlarmTypeDef,
-    PutMetricAlarmInputRequestTypeDef,
     DescribeAlarmsForMetricOutputTypeDef,
     DescribeAlarmsOutputTypeDef,
     AnomalyDetectorTypeDef,
+    GetMetricDataInputGetMetricDataPaginateTypeDef,
+    GetMetricDataInputRequestTypeDef,
+    PutMetricAlarmInputRequestTypeDef,
     DeleteAnomalyDetectorInputRequestTypeDef,
+    MetricMathAnomalyDetectorUnionTypeDef,
     PutAnomalyDetectorInputRequestTypeDef,
     DescribeAnomalyDetectorsOutputTypeDef,
 )
 
 
-def get_structure() -> AlarmHistoryItemTypeDef:
+def get_value() -> AlarmHistoryItemTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-cloudwatch-1.28.15.post1/README.md` & `mypy-boto3-cloudwatch-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudwatch.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudwatch)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cloudwatch)](https://pepy.tech/project/mypy-boto3-cloudwatch)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudWatch 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch)
+[boto3.CloudWatch 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch)
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
 [mypy-boto3-cloudwatch docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch/).
 
 See how it helps to find and fix potential bugs:
 
@@ -46,15 +46,15 @@
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Waiters annotations](#waiters-annotations)
     - [Service Resource annotations](#service-resource-annotations)
     - [Other resources annotations](#other-resources-annotations)
     - [Collections annotations](#collections-annotations)
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
@@ -404,51 +404,48 @@
 )
 
 
 def check_value(value: ActionsSuppressedByType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_cloudwatch.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_cloudwatch.type_defs import (
     AlarmHistoryItemTypeDef,
     RangeOutputTypeDef,
-    RangeTypeDef,
     DimensionTypeDef,
     CompositeAlarmTypeDef,
     DashboardEntryTypeDef,
     DashboardValidationMessageTypeDef,
     DatapointTypeDef,
     DeleteAlarmsInputRequestTypeDef,
     DeleteDashboardsInputRequestTypeDef,
     DeleteInsightRulesInputRequestTypeDef,
     PartialFailureTypeDef,
     ResponseMetadataTypeDef,
     DeleteMetricStreamInputRequestTypeDef,
-    DescribeAlarmHistoryInputAlarmDescribeHistoryTypeDef,
+    TimestampTypeDef,
     PaginatorConfigTypeDef,
-    DescribeAlarmHistoryInputRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeAlarmsInputRequestTypeDef,
     DescribeInsightRulesInputRequestTypeDef,
     InsightRuleTypeDef,
     DimensionFilterTypeDef,
     DisableAlarmActionsInputRequestTypeDef,
     DisableInsightRulesInputRequestTypeDef,
     EnableAlarmActionsInputRequestTypeDef,
     EnableInsightRulesInputRequestTypeDef,
     GetDashboardInputRequestTypeDef,
-    GetInsightRuleReportInputRequestTypeDef,
     InsightRuleMetricDatapointTypeDef,
     LabelOptionsTypeDef,
     MessageDataTypeDef,
     GetMetricStreamInputRequestTypeDef,
     MetricStreamFilterOutputTypeDef,
     GetMetricWidgetImageInputRequestTypeDef,
     InsightRuleContributorDatapointTypeDef,
@@ -465,19 +462,16 @@
     PutDashboardInputRequestTypeDef,
     SetAlarmStateInputAlarmSetStateTypeDef,
     SetAlarmStateInputRequestTypeDef,
     StartMetricStreamsInputRequestTypeDef,
     StopMetricStreamsInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     AnomalyDetectorConfigurationOutputTypeDef,
-    AnomalyDetectorConfigurationTypeDef,
     DescribeAlarmsForMetricInputRequestTypeDef,
     DescribeAnomalyDetectorsInputRequestTypeDef,
-    GetMetricStatisticsInputMetricGetStatisticsTypeDef,
-    GetMetricStatisticsInputRequestTypeDef,
     MetricOutputTypeDef,
     MetricTypeDef,
     SingleMetricAnomalyDetectorOutputTypeDef,
     SingleMetricAnomalyDetectorTypeDef,
     DeleteInsightRulesOutputTypeDef,
     DescribeAlarmHistoryOutputTypeDef,
     DisableInsightRulesOutputTypeDef,
@@ -486,14 +480,20 @@
     GetDashboardOutputTypeDef,
     GetMetricStatisticsOutputTypeDef,
     GetMetricWidgetImageOutputTypeDef,
     ListDashboardsOutputTypeDef,
     PutDashboardOutputTypeDef,
     PutManagedInsightRulesOutputTypeDef,
     PutMetricStreamOutputTypeDef,
+    DescribeAlarmHistoryInputAlarmDescribeHistoryTypeDef,
+    DescribeAlarmHistoryInputRequestTypeDef,
+    GetInsightRuleReportInputRequestTypeDef,
+    GetMetricStatisticsInputMetricGetStatisticsTypeDef,
+    GetMetricStatisticsInputRequestTypeDef,
+    RangeTypeDef,
     DescribeAlarmHistoryInputDescribeAlarmHistoryPaginateTypeDef,
     DescribeAlarmsInputDescribeAlarmsPaginateTypeDef,
     DescribeAnomalyDetectorsInputDescribeAnomalyDetectorsPaginateTypeDef,
     ListDashboardsInputListDashboardsPaginateTypeDef,
     DescribeAlarmsInputAlarmExistsWaitTypeDef,
     DescribeAlarmsInputCompositeAlarmExistsWaitTypeDef,
     DescribeInsightRulesOutputTypeDef,
@@ -505,45 +505,52 @@
     ListTagsForResourceOutputTypeDef,
     ManagedRuleTypeDef,
     PutCompositeAlarmInputRequestTypeDef,
     PutInsightRuleInputRequestTypeDef,
     TagResourceInputRequestTypeDef,
     ManagedRuleDescriptionTypeDef,
     MetricDatumTypeDef,
+    MetricStreamFilterUnionTypeDef,
     MetricStreamStatisticsConfigurationOutputTypeDef,
     MetricStreamStatisticsConfigurationTypeDef,
     ListMetricsOutputTypeDef,
     MetricStatOutputTypeDef,
     MetricStatTypeDef,
+    SingleMetricAnomalyDetectorUnionTypeDef,
+    AnomalyDetectorConfigurationTypeDef,
     GetMetricDataOutputTypeDef,
     GetInsightRuleReportOutputTypeDef,
     PutManagedInsightRulesInputRequestTypeDef,
     ListManagedInsightRulesOutputTypeDef,
     PutMetricDataInputRequestTypeDef,
     GetMetricStreamOutputTypeDef,
-    PutMetricStreamInputRequestTypeDef,
+    MetricStreamStatisticsConfigurationUnionTypeDef,
     MetricDataQueryOutputTypeDef,
     MetricDataQueryTypeDef,
+    AnomalyDetectorConfigurationUnionTypeDef,
+    PutMetricStreamInputRequestTypeDef,
     MetricAlarmTypeDef,
     MetricMathAnomalyDetectorOutputTypeDef,
-    GetMetricDataInputGetMetricDataPaginateTypeDef,
-    GetMetricDataInputRequestTypeDef,
+    MetricDataQueryUnionTypeDef,
     MetricMathAnomalyDetectorTypeDef,
     PutMetricAlarmInputMetricPutAlarmTypeDef,
-    PutMetricAlarmInputRequestTypeDef,
     DescribeAlarmsForMetricOutputTypeDef,
     DescribeAlarmsOutputTypeDef,
     AnomalyDetectorTypeDef,
+    GetMetricDataInputGetMetricDataPaginateTypeDef,
+    GetMetricDataInputRequestTypeDef,
+    PutMetricAlarmInputRequestTypeDef,
     DeleteAnomalyDetectorInputRequestTypeDef,
+    MetricMathAnomalyDetectorUnionTypeDef,
     PutAnomalyDetectorInputRequestTypeDef,
     DescribeAnomalyDetectorsOutputTypeDef,
 )
 
 
-def get_structure() -> AlarmHistoryItemTypeDef:
+def get_value() -> AlarmHistoryItemTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-cloudwatch-1.28.15.post1/mypy_boto3_cloudwatch/__init__.py` & `mypy-boto3-cloudwatch-1.28.16/mypy_boto3_cloudwatch/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudwatch-1.28.15.post1/mypy_boto3_cloudwatch/__init__.pyi` & `mypy-boto3-cloudwatch-1.28.16/mypy_boto3_cloudwatch/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudwatch-1.28.15.post1/mypy_boto3_cloudwatch/__main__.py` & `mypy-boto3-cloudwatch-1.28.16/mypy_boto3_cloudwatch/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CloudWatch 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.CloudWatch 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch\nOther"
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

### Comparing `mypy-boto3-cloudwatch-1.28.15.post1/mypy_boto3_cloudwatch/client.py` & `mypy-boto3-cloudwatch-1.28.16/mypy_boto3_cloudwatch/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from mypy_boto3_cloudwatch.client import CloudWatchClient
 
     session = Session()
     client: CloudWatchClient = session.client("cloudwatch")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AlarmTypeType,
     AnomalyDetectorTypeType,
     ComparisonOperatorType,
@@ -35,16 +34,15 @@
     DescribeAlarmsPaginator,
     DescribeAnomalyDetectorsPaginator,
     GetMetricDataPaginator,
     ListDashboardsPaginator,
     ListMetricsPaginator,
 )
 from .type_defs import (
-    AnomalyDetectorConfigurationOutputTypeDef,
-    AnomalyDetectorConfigurationTypeDef,
+    AnomalyDetectorConfigurationUnionTypeDef,
     DeleteInsightRulesOutputTypeDef,
     DescribeAlarmHistoryOutputTypeDef,
     DescribeAlarmsForMetricOutputTypeDef,
     DescribeAlarmsOutputTypeDef,
     DescribeAnomalyDetectorsOutputTypeDef,
     DescribeInsightRulesOutputTypeDef,
     DimensionFilterTypeDef,
@@ -61,29 +59,25 @@
     LabelOptionsTypeDef,
     ListDashboardsOutputTypeDef,
     ListManagedInsightRulesOutputTypeDef,
     ListMetricsOutputTypeDef,
     ListMetricStreamsOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     ManagedRuleTypeDef,
-    MetricDataQueryOutputTypeDef,
-    MetricDataQueryTypeDef,
+    MetricDataQueryUnionTypeDef,
     MetricDatumTypeDef,
-    MetricMathAnomalyDetectorOutputTypeDef,
-    MetricMathAnomalyDetectorTypeDef,
-    MetricStreamFilterOutputTypeDef,
-    MetricStreamFilterTypeDef,
-    MetricStreamStatisticsConfigurationOutputTypeDef,
-    MetricStreamStatisticsConfigurationTypeDef,
+    MetricMathAnomalyDetectorUnionTypeDef,
+    MetricStreamFilterUnionTypeDef,
+    MetricStreamStatisticsConfigurationUnionTypeDef,
     PutDashboardOutputTypeDef,
     PutManagedInsightRulesOutputTypeDef,
     PutMetricStreamOutputTypeDef,
-    SingleMetricAnomalyDetectorOutputTypeDef,
-    SingleMetricAnomalyDetectorTypeDef,
+    SingleMetricAnomalyDetectorUnionTypeDef,
     TagTypeDef,
+    TimestampTypeDef,
 )
 from .waiter import AlarmExistsWaiter, CompositeAlarmExistsWaiter
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -161,20 +155,16 @@
     def delete_anomaly_detector(
         self,
         *,
         Namespace: str = ...,
         MetricName: str = ...,
         Dimensions: Sequence[DimensionTypeDef] = ...,
         Stat: str = ...,
-        SingleMetricAnomalyDetector: Union[
-            SingleMetricAnomalyDetectorTypeDef, SingleMetricAnomalyDetectorOutputTypeDef
-        ] = ...,
-        MetricMathAnomalyDetector: Union[
-            MetricMathAnomalyDetectorTypeDef, MetricMathAnomalyDetectorOutputTypeDef
-        ] = ...
+        SingleMetricAnomalyDetector: SingleMetricAnomalyDetectorUnionTypeDef = ...,
+        MetricMathAnomalyDetector: MetricMathAnomalyDetectorUnionTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Deletes the specified anomaly detection model from your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Client.delete_anomaly_detector)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch/client/#delete_anomaly_detector)
         """
@@ -205,16 +195,16 @@
 
     def describe_alarm_history(
         self,
         *,
         AlarmName: str = ...,
         AlarmTypes: Sequence[AlarmTypeType] = ...,
         HistoryItemType: HistoryItemTypeType = ...,
-        StartDate: Union[datetime, str] = ...,
-        EndDate: Union[datetime, str] = ...,
+        StartDate: TimestampTypeDef = ...,
+        EndDate: TimestampTypeDef = ...,
         MaxRecords: int = ...,
         NextToken: str = ...,
         ScanBy: ScanByType = ...
     ) -> DescribeAlarmHistoryOutputTypeDef:
         """
         Retrieves the history for the specified alarm.
 
@@ -343,16 +333,16 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch/client/#get_dashboard)
         """
 
     def get_insight_rule_report(
         self,
         *,
         RuleName: str,
-        StartTime: Union[datetime, str],
-        EndTime: Union[datetime, str],
+        StartTime: TimestampTypeDef,
+        EndTime: TimestampTypeDef,
         Period: int,
         MaxContributorCount: int = ...,
         Metrics: Sequence[str] = ...,
         OrderBy: str = ...
     ) -> GetInsightRuleReportOutputTypeDef:
         """
         This operation returns the time series data collected by a Contributor Insights
@@ -361,17 +351,17 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Client.get_insight_rule_report)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch/client/#get_insight_rule_report)
         """
 
     def get_metric_data(
         self,
         *,
-        MetricDataQueries: Sequence[Union[MetricDataQueryTypeDef, MetricDataQueryOutputTypeDef]],
-        StartTime: Union[datetime, str],
-        EndTime: Union[datetime, str],
+        MetricDataQueries: Sequence[MetricDataQueryUnionTypeDef],
+        StartTime: TimestampTypeDef,
+        EndTime: TimestampTypeDef,
         NextToken: str = ...,
         ScanBy: ScanByType = ...,
         MaxDatapoints: int = ...,
         LabelOptions: LabelOptionsTypeDef = ...
     ) -> GetMetricDataOutputTypeDef:
         """
         You can use the `GetMetricData` API to retrieve CloudWatch metric values.
@@ -381,16 +371,16 @@
         """
 
     def get_metric_statistics(
         self,
         *,
         Namespace: str,
         MetricName: str,
-        StartTime: Union[datetime, str],
-        EndTime: Union[datetime, str],
+        StartTime: TimestampTypeDef,
+        EndTime: TimestampTypeDef,
         Period: int,
         Dimensions: Sequence[DimensionTypeDef] = ...,
         Statistics: Sequence[StatisticType] = ...,
         ExtendedStatistics: Sequence[str] = ...,
         Unit: StandardUnitType = ...
     ) -> GetMetricStatisticsOutputTypeDef:
         """
@@ -479,23 +469,17 @@
     def put_anomaly_detector(
         self,
         *,
         Namespace: str = ...,
         MetricName: str = ...,
         Dimensions: Sequence[DimensionTypeDef] = ...,
         Stat: str = ...,
-        Configuration: Union[
-            AnomalyDetectorConfigurationTypeDef, AnomalyDetectorConfigurationOutputTypeDef
-        ] = ...,
-        SingleMetricAnomalyDetector: Union[
-            SingleMetricAnomalyDetectorTypeDef, SingleMetricAnomalyDetectorOutputTypeDef
-        ] = ...,
-        MetricMathAnomalyDetector: Union[
-            MetricMathAnomalyDetectorTypeDef, MetricMathAnomalyDetectorOutputTypeDef
-        ] = ...
+        Configuration: AnomalyDetectorConfigurationUnionTypeDef = ...,
+        SingleMetricAnomalyDetector: SingleMetricAnomalyDetectorUnionTypeDef = ...,
+        MetricMathAnomalyDetector: MetricMathAnomalyDetectorUnionTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Creates an anomaly detection model for a CloudWatch metric.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Client.put_anomaly_detector)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch/client/#put_anomaly_detector)
         """
@@ -575,15 +559,15 @@
         Dimensions: Sequence[DimensionTypeDef] = ...,
         Period: int = ...,
         Unit: StandardUnitType = ...,
         DatapointsToAlarm: int = ...,
         Threshold: float = ...,
         TreatMissingData: str = ...,
         EvaluateLowSampleCountPercentile: str = ...,
-        Metrics: Sequence[Union[MetricDataQueryTypeDef, MetricDataQueryOutputTypeDef]] = ...,
+        Metrics: Sequence[MetricDataQueryUnionTypeDef] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ThresholdMetricId: str = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Creates or updates an alarm and associates it with the specified metric, metric
         math expression, anomaly detection model, or Metrics Insights query.
 
@@ -604,27 +588,18 @@
     def put_metric_stream(
         self,
         *,
         Name: str,
         FirehoseArn: str,
         RoleArn: str,
         OutputFormat: MetricStreamOutputFormatType,
-        IncludeFilters: Sequence[
-            Union[MetricStreamFilterTypeDef, MetricStreamFilterOutputTypeDef]
-        ] = ...,
-        ExcludeFilters: Sequence[
-            Union[MetricStreamFilterTypeDef, MetricStreamFilterOutputTypeDef]
-        ] = ...,
+        IncludeFilters: Sequence[MetricStreamFilterUnionTypeDef] = ...,
+        ExcludeFilters: Sequence[MetricStreamFilterUnionTypeDef] = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        StatisticsConfigurations: Sequence[
-            Union[
-                MetricStreamStatisticsConfigurationTypeDef,
-                MetricStreamStatisticsConfigurationOutputTypeDef,
-            ]
-        ] = ...,
+        StatisticsConfigurations: Sequence[MetricStreamStatisticsConfigurationUnionTypeDef] = ...,
         IncludeLinkedAccountsMetrics: bool = ...
     ) -> PutMetricStreamOutputTypeDef:
         """
         Creates or updates a metric stream.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Client.put_metric_stream)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch/client/#put_metric_stream)
```

### Comparing `mypy-boto3-cloudwatch-1.28.15.post1/mypy_boto3_cloudwatch/client.pyi` & `mypy-boto3-cloudwatch-1.28.16/mypy_boto3_cloudwatch/client.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from mypy_boto3_cloudwatch.client import CloudWatchClient
 
     session = Session()
     client: CloudWatchClient = session.client("cloudwatch")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AlarmTypeType,
     AnomalyDetectorTypeType,
     ComparisonOperatorType,
@@ -35,16 +34,15 @@
     DescribeAlarmsPaginator,
     DescribeAnomalyDetectorsPaginator,
     GetMetricDataPaginator,
     ListDashboardsPaginator,
     ListMetricsPaginator,
 )
 from .type_defs import (
-    AnomalyDetectorConfigurationOutputTypeDef,
-    AnomalyDetectorConfigurationTypeDef,
+    AnomalyDetectorConfigurationUnionTypeDef,
     DeleteInsightRulesOutputTypeDef,
     DescribeAlarmHistoryOutputTypeDef,
     DescribeAlarmsForMetricOutputTypeDef,
     DescribeAlarmsOutputTypeDef,
     DescribeAnomalyDetectorsOutputTypeDef,
     DescribeInsightRulesOutputTypeDef,
     DimensionFilterTypeDef,
@@ -61,29 +59,25 @@
     LabelOptionsTypeDef,
     ListDashboardsOutputTypeDef,
     ListManagedInsightRulesOutputTypeDef,
     ListMetricsOutputTypeDef,
     ListMetricStreamsOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     ManagedRuleTypeDef,
-    MetricDataQueryOutputTypeDef,
-    MetricDataQueryTypeDef,
+    MetricDataQueryUnionTypeDef,
     MetricDatumTypeDef,
-    MetricMathAnomalyDetectorOutputTypeDef,
-    MetricMathAnomalyDetectorTypeDef,
-    MetricStreamFilterOutputTypeDef,
-    MetricStreamFilterTypeDef,
-    MetricStreamStatisticsConfigurationOutputTypeDef,
-    MetricStreamStatisticsConfigurationTypeDef,
+    MetricMathAnomalyDetectorUnionTypeDef,
+    MetricStreamFilterUnionTypeDef,
+    MetricStreamStatisticsConfigurationUnionTypeDef,
     PutDashboardOutputTypeDef,
     PutManagedInsightRulesOutputTypeDef,
     PutMetricStreamOutputTypeDef,
-    SingleMetricAnomalyDetectorOutputTypeDef,
-    SingleMetricAnomalyDetectorTypeDef,
+    SingleMetricAnomalyDetectorUnionTypeDef,
     TagTypeDef,
+    TimestampTypeDef,
 )
 from .waiter import AlarmExistsWaiter, CompositeAlarmExistsWaiter
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -153,20 +147,16 @@
     def delete_anomaly_detector(
         self,
         *,
         Namespace: str = ...,
         MetricName: str = ...,
         Dimensions: Sequence[DimensionTypeDef] = ...,
         Stat: str = ...,
-        SingleMetricAnomalyDetector: Union[
-            SingleMetricAnomalyDetectorTypeDef, SingleMetricAnomalyDetectorOutputTypeDef
-        ] = ...,
-        MetricMathAnomalyDetector: Union[
-            MetricMathAnomalyDetectorTypeDef, MetricMathAnomalyDetectorOutputTypeDef
-        ] = ...
+        SingleMetricAnomalyDetector: SingleMetricAnomalyDetectorUnionTypeDef = ...,
+        MetricMathAnomalyDetector: MetricMathAnomalyDetectorUnionTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Deletes the specified anomaly detection model from your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Client.delete_anomaly_detector)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch/client/#delete_anomaly_detector)
         """
@@ -193,16 +183,16 @@
         """
     def describe_alarm_history(
         self,
         *,
         AlarmName: str = ...,
         AlarmTypes: Sequence[AlarmTypeType] = ...,
         HistoryItemType: HistoryItemTypeType = ...,
-        StartDate: Union[datetime, str] = ...,
-        EndDate: Union[datetime, str] = ...,
+        StartDate: TimestampTypeDef = ...,
+        EndDate: TimestampTypeDef = ...,
         MaxRecords: int = ...,
         NextToken: str = ...,
         ScanBy: ScanByType = ...
     ) -> DescribeAlarmHistoryOutputTypeDef:
         """
         Retrieves the history for the specified alarm.
 
@@ -320,16 +310,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Client.get_dashboard)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch/client/#get_dashboard)
         """
     def get_insight_rule_report(
         self,
         *,
         RuleName: str,
-        StartTime: Union[datetime, str],
-        EndTime: Union[datetime, str],
+        StartTime: TimestampTypeDef,
+        EndTime: TimestampTypeDef,
         Period: int,
         MaxContributorCount: int = ...,
         Metrics: Sequence[str] = ...,
         OrderBy: str = ...
     ) -> GetInsightRuleReportOutputTypeDef:
         """
         This operation returns the time series data collected by a Contributor Insights
@@ -337,17 +327,17 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Client.get_insight_rule_report)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch/client/#get_insight_rule_report)
         """
     def get_metric_data(
         self,
         *,
-        MetricDataQueries: Sequence[Union[MetricDataQueryTypeDef, MetricDataQueryOutputTypeDef]],
-        StartTime: Union[datetime, str],
-        EndTime: Union[datetime, str],
+        MetricDataQueries: Sequence[MetricDataQueryUnionTypeDef],
+        StartTime: TimestampTypeDef,
+        EndTime: TimestampTypeDef,
         NextToken: str = ...,
         ScanBy: ScanByType = ...,
         MaxDatapoints: int = ...,
         LabelOptions: LabelOptionsTypeDef = ...
     ) -> GetMetricDataOutputTypeDef:
         """
         You can use the `GetMetricData` API to retrieve CloudWatch metric values.
@@ -356,16 +346,16 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch/client/#get_metric_data)
         """
     def get_metric_statistics(
         self,
         *,
         Namespace: str,
         MetricName: str,
-        StartTime: Union[datetime, str],
-        EndTime: Union[datetime, str],
+        StartTime: TimestampTypeDef,
+        EndTime: TimestampTypeDef,
         Period: int,
         Dimensions: Sequence[DimensionTypeDef] = ...,
         Statistics: Sequence[StatisticType] = ...,
         ExtendedStatistics: Sequence[str] = ...,
         Unit: StandardUnitType = ...
     ) -> GetMetricStatisticsOutputTypeDef:
         """
@@ -446,23 +436,17 @@
     def put_anomaly_detector(
         self,
         *,
         Namespace: str = ...,
         MetricName: str = ...,
         Dimensions: Sequence[DimensionTypeDef] = ...,
         Stat: str = ...,
-        Configuration: Union[
-            AnomalyDetectorConfigurationTypeDef, AnomalyDetectorConfigurationOutputTypeDef
-        ] = ...,
-        SingleMetricAnomalyDetector: Union[
-            SingleMetricAnomalyDetectorTypeDef, SingleMetricAnomalyDetectorOutputTypeDef
-        ] = ...,
-        MetricMathAnomalyDetector: Union[
-            MetricMathAnomalyDetectorTypeDef, MetricMathAnomalyDetectorOutputTypeDef
-        ] = ...
+        Configuration: AnomalyDetectorConfigurationUnionTypeDef = ...,
+        SingleMetricAnomalyDetector: SingleMetricAnomalyDetectorUnionTypeDef = ...,
+        MetricMathAnomalyDetector: MetricMathAnomalyDetectorUnionTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Creates an anomaly detection model for a CloudWatch metric.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Client.put_anomaly_detector)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch/client/#put_anomaly_detector)
         """
@@ -537,15 +521,15 @@
         Dimensions: Sequence[DimensionTypeDef] = ...,
         Period: int = ...,
         Unit: StandardUnitType = ...,
         DatapointsToAlarm: int = ...,
         Threshold: float = ...,
         TreatMissingData: str = ...,
         EvaluateLowSampleCountPercentile: str = ...,
-        Metrics: Sequence[Union[MetricDataQueryTypeDef, MetricDataQueryOutputTypeDef]] = ...,
+        Metrics: Sequence[MetricDataQueryUnionTypeDef] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ThresholdMetricId: str = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Creates or updates an alarm and associates it with the specified metric, metric
         math expression, anomaly detection model, or Metrics Insights query.
 
@@ -564,27 +548,18 @@
     def put_metric_stream(
         self,
         *,
         Name: str,
         FirehoseArn: str,
         RoleArn: str,
         OutputFormat: MetricStreamOutputFormatType,
-        IncludeFilters: Sequence[
-            Union[MetricStreamFilterTypeDef, MetricStreamFilterOutputTypeDef]
-        ] = ...,
-        ExcludeFilters: Sequence[
-            Union[MetricStreamFilterTypeDef, MetricStreamFilterOutputTypeDef]
-        ] = ...,
+        IncludeFilters: Sequence[MetricStreamFilterUnionTypeDef] = ...,
+        ExcludeFilters: Sequence[MetricStreamFilterUnionTypeDef] = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        StatisticsConfigurations: Sequence[
-            Union[
-                MetricStreamStatisticsConfigurationTypeDef,
-                MetricStreamStatisticsConfigurationOutputTypeDef,
-            ]
-        ] = ...,
+        StatisticsConfigurations: Sequence[MetricStreamStatisticsConfigurationUnionTypeDef] = ...,
         IncludeLinkedAccountsMetrics: bool = ...
     ) -> PutMetricStreamOutputTypeDef:
         """
         Creates or updates a metric stream.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Client.put_metric_stream)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch/client/#put_metric_stream)
```

### Comparing `mypy-boto3-cloudwatch-1.28.15.post1/mypy_boto3_cloudwatch/literals.py` & `mypy-boto3-cloudwatch-1.28.16/mypy_boto3_cloudwatch/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudwatch-1.28.15.post1/mypy_boto3_cloudwatch/literals.pyi` & `mypy-boto3-cloudwatch-1.28.16/mypy_boto3_cloudwatch/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudwatch-1.28.15.post1/mypy_boto3_cloudwatch/paginator.py` & `mypy-boto3-cloudwatch-1.28.16/mypy_boto3_cloudwatch/paginator.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,16 +26,15 @@
     describe_anomaly_detectors_paginator: DescribeAnomalyDetectorsPaginator = client.get_paginator("describe_anomaly_detectors")
     get_metric_data_paginator: GetMetricDataPaginator = client.get_paginator("get_metric_data")
     list_dashboards_paginator: ListDashboardsPaginator = client.get_paginator("list_dashboards")
     list_metrics_paginator: ListMetricsPaginator = client.get_paginator("list_metrics")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Generic, Iterator, Sequence, TypeVar, Union
+from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import (
     AlarmTypeType,
     AnomalyDetectorTypeType,
     HistoryItemTypeType,
@@ -48,17 +47,17 @@
     DescribeAnomalyDetectorsOutputTypeDef,
     DimensionFilterTypeDef,
     DimensionTypeDef,
     GetMetricDataOutputTypeDef,
     LabelOptionsTypeDef,
     ListDashboardsOutputTypeDef,
     ListMetricsOutputTypeDef,
-    MetricDataQueryOutputTypeDef,
-    MetricDataQueryTypeDef,
+    MetricDataQueryUnionTypeDef,
     PaginatorConfigTypeDef,
+    TimestampTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -91,16 +90,16 @@
 
     def paginate(
         self,
         *,
         AlarmName: str = ...,
         AlarmTypes: Sequence[AlarmTypeType] = ...,
         HistoryItemType: HistoryItemTypeType = ...,
-        StartDate: Union[datetime, str] = ...,
-        EndDate: Union[datetime, str] = ...,
+        StartDate: TimestampTypeDef = ...,
+        EndDate: TimestampTypeDef = ...,
         ScanBy: ScanByType = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeAlarmHistoryOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Paginator.DescribeAlarmHistory.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch/paginators/#describealarmhistorypaginator)
         """
@@ -156,17 +155,17 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Paginator.GetMetricData)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch/paginators/#getmetricdatapaginator)
     """
 
     def paginate(
         self,
         *,
-        MetricDataQueries: Sequence[Union[MetricDataQueryTypeDef, MetricDataQueryOutputTypeDef]],
-        StartTime: Union[datetime, str],
-        EndTime: Union[datetime, str],
+        MetricDataQueries: Sequence[MetricDataQueryUnionTypeDef],
+        StartTime: TimestampTypeDef,
+        EndTime: TimestampTypeDef,
         ScanBy: ScanByType = ...,
         LabelOptions: LabelOptionsTypeDef = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetMetricDataOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Paginator.GetMetricData.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch/paginators/#getmetricdatapaginator)
```

### Comparing `mypy-boto3-cloudwatch-1.28.15.post1/mypy_boto3_cloudwatch/paginator.pyi` & `mypy-boto3-cloudwatch-1.28.16/mypy_boto3_cloudwatch/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -26,16 +26,15 @@
     describe_anomaly_detectors_paginator: DescribeAnomalyDetectorsPaginator = client.get_paginator("describe_anomaly_detectors")
     get_metric_data_paginator: GetMetricDataPaginator = client.get_paginator("get_metric_data")
     list_dashboards_paginator: ListDashboardsPaginator = client.get_paginator("list_dashboards")
     list_metrics_paginator: ListMetricsPaginator = client.get_paginator("list_metrics")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Generic, Iterator, Sequence, TypeVar, Union
+from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import (
     AlarmTypeType,
     AnomalyDetectorTypeType,
     HistoryItemTypeType,
@@ -48,17 +47,17 @@
     DescribeAnomalyDetectorsOutputTypeDef,
     DimensionFilterTypeDef,
     DimensionTypeDef,
     GetMetricDataOutputTypeDef,
     LabelOptionsTypeDef,
     ListDashboardsOutputTypeDef,
     ListMetricsOutputTypeDef,
-    MetricDataQueryOutputTypeDef,
-    MetricDataQueryTypeDef,
+    MetricDataQueryUnionTypeDef,
     PaginatorConfigTypeDef,
+    TimestampTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -87,16 +86,16 @@
 
     def paginate(
         self,
         *,
         AlarmName: str = ...,
         AlarmTypes: Sequence[AlarmTypeType] = ...,
         HistoryItemType: HistoryItemTypeType = ...,
-        StartDate: Union[datetime, str] = ...,
-        EndDate: Union[datetime, str] = ...,
+        StartDate: TimestampTypeDef = ...,
+        EndDate: TimestampTypeDef = ...,
         ScanBy: ScanByType = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeAlarmHistoryOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Paginator.DescribeAlarmHistory.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch/paginators/#describealarmhistorypaginator)
         """
@@ -149,17 +148,17 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Paginator.GetMetricData)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch/paginators/#getmetricdatapaginator)
     """
 
     def paginate(
         self,
         *,
-        MetricDataQueries: Sequence[Union[MetricDataQueryTypeDef, MetricDataQueryOutputTypeDef]],
-        StartTime: Union[datetime, str],
-        EndTime: Union[datetime, str],
+        MetricDataQueries: Sequence[MetricDataQueryUnionTypeDef],
+        StartTime: TimestampTypeDef,
+        EndTime: TimestampTypeDef,
         ScanBy: ScanByType = ...,
         LabelOptions: LabelOptionsTypeDef = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetMetricDataOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Paginator.GetMetricData.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch/paginators/#getmetricdatapaginator)
```

### Comparing `mypy-boto3-cloudwatch-1.28.15.post1/mypy_boto3_cloudwatch/service_resource.py` & `mypy-boto3-cloudwatch-1.28.16/mypy_boto3_cloudwatch/service_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
     my_alarm: cloudwatch_resources.Alarm = resource.Alarm(...)
     my_metric: cloudwatch_resources.Metric = resource.Metric(...)
 ```
 """
 import sys
 from datetime import datetime
-from typing import Iterator, List, Sequence, Union
+from typing import Iterator, List, Sequence
 
 from boto3.resources.base import ResourceMeta, ServiceResource
 from boto3.resources.collection import ResourceCollection
 
 from .client import CloudWatchClient
 from .literals import (
     AlarmTypeType,
@@ -39,14 +39,15 @@
     DescribeAlarmHistoryOutputTypeDef,
     DimensionFilterTypeDef,
     DimensionTypeDef,
     GetMetricStatisticsOutputTypeDef,
     MetricDataQueryOutputTypeDef,
     MetricDataQueryTypeDef,
     TagTypeDef,
+    TimestampTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -319,16 +320,16 @@
         """
 
     def describe_history(
         self,
         *,
         AlarmTypes: Sequence[AlarmTypeType] = ...,
         HistoryItemType: HistoryItemTypeType = ...,
-        StartDate: Union[datetime, str] = ...,
-        EndDate: Union[datetime, str] = ...,
+        StartDate: TimestampTypeDef = ...,
+        EndDate: TimestampTypeDef = ...,
         MaxRecords: int = ...,
         NextToken: str = ...,
         ScanBy: ScanByType = ...
     ) -> DescribeAlarmHistoryOutputTypeDef:
         """
         Retrieves the history for the specified alarm.
 
@@ -411,16 +412,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Metric.get_available_subresources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch/service_resource/#metricget_available_subresources-method)
         """
 
     def get_statistics(
         self,
         *,
-        StartTime: Union[datetime, str],
-        EndTime: Union[datetime, str],
+        StartTime: TimestampTypeDef,
+        EndTime: TimestampTypeDef,
         Period: int,
         Dimensions: Sequence[DimensionTypeDef] = ...,
         Statistics: Sequence[StatisticType] = ...,
         ExtendedStatistics: Sequence[str] = ...,
         Unit: StandardUnitType = ...
     ) -> GetMetricStatisticsOutputTypeDef:
         """
```

### Comparing `mypy-boto3-cloudwatch-1.28.15.post1/mypy_boto3_cloudwatch/service_resource.pyi` & `mypy-boto3-cloudwatch-1.28.16/mypy_boto3_cloudwatch/service_resource.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
     my_alarm: cloudwatch_resources.Alarm = resource.Alarm(...)
     my_metric: cloudwatch_resources.Metric = resource.Metric(...)
 ```
 """
 import sys
 from datetime import datetime
-from typing import Iterator, List, Sequence, Union
+from typing import Iterator, List, Sequence
 
 from boto3.resources.base import ResourceMeta, ServiceResource
 from boto3.resources.collection import ResourceCollection
 
 from .client import CloudWatchClient
 from .literals import (
     AlarmTypeType,
@@ -39,14 +39,15 @@
     DescribeAlarmHistoryOutputTypeDef,
     DimensionFilterTypeDef,
     DimensionTypeDef,
     GetMetricStatisticsOutputTypeDef,
     MetricDataQueryOutputTypeDef,
     MetricDataQueryTypeDef,
     TagTypeDef,
+    TimestampTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -292,16 +293,16 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch/service_resource/#alarmdelete-method)
         """
     def describe_history(
         self,
         *,
         AlarmTypes: Sequence[AlarmTypeType] = ...,
         HistoryItemType: HistoryItemTypeType = ...,
-        StartDate: Union[datetime, str] = ...,
-        EndDate: Union[datetime, str] = ...,
+        StartDate: TimestampTypeDef = ...,
+        EndDate: TimestampTypeDef = ...,
         MaxRecords: int = ...,
         NextToken: str = ...,
         ScanBy: ScanByType = ...
     ) -> DescribeAlarmHistoryOutputTypeDef:
         """
         Retrieves the history for the specified alarm.
 
@@ -375,16 +376,16 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Metric.get_available_subresources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch/service_resource/#metricget_available_subresources-method)
         """
     def get_statistics(
         self,
         *,
-        StartTime: Union[datetime, str],
-        EndTime: Union[datetime, str],
+        StartTime: TimestampTypeDef,
+        EndTime: TimestampTypeDef,
         Period: int,
         Dimensions: Sequence[DimensionTypeDef] = ...,
         Statistics: Sequence[StatisticType] = ...,
         ExtendedStatistics: Sequence[str] = ...,
         Unit: StandardUnitType = ...
     ) -> GetMetricStatisticsOutputTypeDef:
         """
```

### Comparing `mypy-boto3-cloudwatch-1.28.15.post1/mypy_boto3_cloudwatch/type_defs.py` & `mypy-boto3-cloudwatch-1.28.16/mypy_boto3_cloudwatch/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_cloudwatch.type_defs import AlarmHistoryItemTypeDef
 
-    data: AlarmHistoryItemTypeDef = {...}
+    data: AlarmHistoryItemTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -39,40 +39,37 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AlarmHistoryItemTypeDef",
     "RangeOutputTypeDef",
-    "RangeTypeDef",
     "DimensionTypeDef",
     "CompositeAlarmTypeDef",
     "DashboardEntryTypeDef",
     "DashboardValidationMessageTypeDef",
     "DatapointTypeDef",
     "DeleteAlarmsInputRequestTypeDef",
     "DeleteDashboardsInputRequestTypeDef",
     "DeleteInsightRulesInputRequestTypeDef",
     "PartialFailureTypeDef",
     "ResponseMetadataTypeDef",
     "DeleteMetricStreamInputRequestTypeDef",
-    "DescribeAlarmHistoryInputAlarmDescribeHistoryTypeDef",
+    "TimestampTypeDef",
     "PaginatorConfigTypeDef",
-    "DescribeAlarmHistoryInputRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeAlarmsInputRequestTypeDef",
     "DescribeInsightRulesInputRequestTypeDef",
     "InsightRuleTypeDef",
     "DimensionFilterTypeDef",
     "DisableAlarmActionsInputRequestTypeDef",
     "DisableInsightRulesInputRequestTypeDef",
     "EnableAlarmActionsInputRequestTypeDef",
     "EnableInsightRulesInputRequestTypeDef",
     "GetDashboardInputRequestTypeDef",
-    "GetInsightRuleReportInputRequestTypeDef",
     "InsightRuleMetricDatapointTypeDef",
     "LabelOptionsTypeDef",
     "MessageDataTypeDef",
     "GetMetricStreamInputRequestTypeDef",
     "MetricStreamFilterOutputTypeDef",
     "GetMetricWidgetImageInputRequestTypeDef",
     "InsightRuleContributorDatapointTypeDef",
@@ -89,19 +86,16 @@
     "PutDashboardInputRequestTypeDef",
     "SetAlarmStateInputAlarmSetStateTypeDef",
     "SetAlarmStateInputRequestTypeDef",
     "StartMetricStreamsInputRequestTypeDef",
     "StopMetricStreamsInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "AnomalyDetectorConfigurationOutputTypeDef",
-    "AnomalyDetectorConfigurationTypeDef",
     "DescribeAlarmsForMetricInputRequestTypeDef",
     "DescribeAnomalyDetectorsInputRequestTypeDef",
-    "GetMetricStatisticsInputMetricGetStatisticsTypeDef",
-    "GetMetricStatisticsInputRequestTypeDef",
     "MetricOutputTypeDef",
     "MetricTypeDef",
     "SingleMetricAnomalyDetectorOutputTypeDef",
     "SingleMetricAnomalyDetectorTypeDef",
     "DeleteInsightRulesOutputTypeDef",
     "DescribeAlarmHistoryOutputTypeDef",
     "DisableInsightRulesOutputTypeDef",
@@ -110,14 +104,20 @@
     "GetDashboardOutputTypeDef",
     "GetMetricStatisticsOutputTypeDef",
     "GetMetricWidgetImageOutputTypeDef",
     "ListDashboardsOutputTypeDef",
     "PutDashboardOutputTypeDef",
     "PutManagedInsightRulesOutputTypeDef",
     "PutMetricStreamOutputTypeDef",
+    "DescribeAlarmHistoryInputAlarmDescribeHistoryTypeDef",
+    "DescribeAlarmHistoryInputRequestTypeDef",
+    "GetInsightRuleReportInputRequestTypeDef",
+    "GetMetricStatisticsInputMetricGetStatisticsTypeDef",
+    "GetMetricStatisticsInputRequestTypeDef",
+    "RangeTypeDef",
     "DescribeAlarmHistoryInputDescribeAlarmHistoryPaginateTypeDef",
     "DescribeAlarmsInputDescribeAlarmsPaginateTypeDef",
     "DescribeAnomalyDetectorsInputDescribeAnomalyDetectorsPaginateTypeDef",
     "ListDashboardsInputListDashboardsPaginateTypeDef",
     "DescribeAlarmsInputAlarmExistsWaitTypeDef",
     "DescribeAlarmsInputCompositeAlarmExistsWaitTypeDef",
     "DescribeInsightRulesOutputTypeDef",
@@ -129,39 +129,46 @@
     "ListTagsForResourceOutputTypeDef",
     "ManagedRuleTypeDef",
     "PutCompositeAlarmInputRequestTypeDef",
     "PutInsightRuleInputRequestTypeDef",
     "TagResourceInputRequestTypeDef",
     "ManagedRuleDescriptionTypeDef",
     "MetricDatumTypeDef",
+    "MetricStreamFilterUnionTypeDef",
     "MetricStreamStatisticsConfigurationOutputTypeDef",
     "MetricStreamStatisticsConfigurationTypeDef",
     "ListMetricsOutputTypeDef",
     "MetricStatOutputTypeDef",
     "MetricStatTypeDef",
+    "SingleMetricAnomalyDetectorUnionTypeDef",
+    "AnomalyDetectorConfigurationTypeDef",
     "GetMetricDataOutputTypeDef",
     "GetInsightRuleReportOutputTypeDef",
     "PutManagedInsightRulesInputRequestTypeDef",
     "ListManagedInsightRulesOutputTypeDef",
     "PutMetricDataInputRequestTypeDef",
     "GetMetricStreamOutputTypeDef",
-    "PutMetricStreamInputRequestTypeDef",
+    "MetricStreamStatisticsConfigurationUnionTypeDef",
     "MetricDataQueryOutputTypeDef",
     "MetricDataQueryTypeDef",
+    "AnomalyDetectorConfigurationUnionTypeDef",
+    "PutMetricStreamInputRequestTypeDef",
     "MetricAlarmTypeDef",
     "MetricMathAnomalyDetectorOutputTypeDef",
-    "GetMetricDataInputGetMetricDataPaginateTypeDef",
-    "GetMetricDataInputRequestTypeDef",
+    "MetricDataQueryUnionTypeDef",
     "MetricMathAnomalyDetectorTypeDef",
     "PutMetricAlarmInputMetricPutAlarmTypeDef",
-    "PutMetricAlarmInputRequestTypeDef",
     "DescribeAlarmsForMetricOutputTypeDef",
     "DescribeAlarmsOutputTypeDef",
     "AnomalyDetectorTypeDef",
+    "GetMetricDataInputGetMetricDataPaginateTypeDef",
+    "GetMetricDataInputRequestTypeDef",
+    "PutMetricAlarmInputRequestTypeDef",
     "DeleteAnomalyDetectorInputRequestTypeDef",
+    "MetricMathAnomalyDetectorUnionTypeDef",
     "PutAnomalyDetectorInputRequestTypeDef",
     "DescribeAnomalyDetectorsOutputTypeDef",
 )
 
 AlarmHistoryItemTypeDef = TypedDict(
     "AlarmHistoryItemTypeDef",
     {
@@ -179,22 +186,14 @@
     "RangeOutputTypeDef",
     {
         "StartTime": datetime,
         "EndTime": datetime,
     },
 )
 
-RangeTypeDef = TypedDict(
-    "RangeTypeDef",
-    {
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-    },
-)
-
 DimensionTypeDef = TypedDict(
     "DimensionTypeDef",
     {
         "Name": str,
         "Value": str,
     },
 )
@@ -306,53 +305,25 @@
 DeleteMetricStreamInputRequestTypeDef = TypedDict(
     "DeleteMetricStreamInputRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-DescribeAlarmHistoryInputAlarmDescribeHistoryTypeDef = TypedDict(
-    "DescribeAlarmHistoryInputAlarmDescribeHistoryTypeDef",
-    {
-        "AlarmTypes": Sequence[AlarmTypeType],
-        "HistoryItemType": HistoryItemTypeType,
-        "StartDate": Union[datetime, str],
-        "EndDate": Union[datetime, str],
-        "MaxRecords": int,
-        "NextToken": str,
-        "ScanBy": ScanByType,
-    },
-    total=False,
-)
-
+TimestampTypeDef = Union[datetime, str]
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
-DescribeAlarmHistoryInputRequestTypeDef = TypedDict(
-    "DescribeAlarmHistoryInputRequestTypeDef",
-    {
-        "AlarmName": str,
-        "AlarmTypes": Sequence[AlarmTypeType],
-        "HistoryItemType": HistoryItemTypeType,
-        "StartDate": Union[datetime, str],
-        "EndDate": Union[datetime, str],
-        "MaxRecords": int,
-        "NextToken": str,
-        "ScanBy": ScanByType,
-    },
-    total=False,
-)
-
 WaiterConfigTypeDef = TypedDict(
     "WaiterConfigTypeDef",
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
@@ -455,41 +426,14 @@
 GetDashboardInputRequestTypeDef = TypedDict(
     "GetDashboardInputRequestTypeDef",
     {
         "DashboardName": str,
     },
 )
 
-_RequiredGetInsightRuleReportInputRequestTypeDef = TypedDict(
-    "_RequiredGetInsightRuleReportInputRequestTypeDef",
-    {
-        "RuleName": str,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "Period": int,
-    },
-)
-_OptionalGetInsightRuleReportInputRequestTypeDef = TypedDict(
-    "_OptionalGetInsightRuleReportInputRequestTypeDef",
-    {
-        "MaxContributorCount": int,
-        "Metrics": Sequence[str],
-        "OrderBy": str,
-    },
-    total=False,
-)
-
-
-class GetInsightRuleReportInputRequestTypeDef(
-    _RequiredGetInsightRuleReportInputRequestTypeDef,
-    _OptionalGetInsightRuleReportInputRequestTypeDef,
-):
-    pass
-
-
 _RequiredInsightRuleMetricDatapointTypeDef = TypedDict(
     "_RequiredInsightRuleMetricDatapointTypeDef",
     {
         "Timestamp": datetime,
     },
 )
 _OptionalInsightRuleMetricDatapointTypeDef = TypedDict(
@@ -761,23 +705,14 @@
     {
         "ExcludedTimeRanges": List[RangeOutputTypeDef],
         "MetricTimezone": str,
     },
     total=False,
 )
 
-AnomalyDetectorConfigurationTypeDef = TypedDict(
-    "AnomalyDetectorConfigurationTypeDef",
-    {
-        "ExcludedTimeRanges": Sequence[RangeTypeDef],
-        "MetricTimezone": str,
-    },
-    total=False,
-)
-
 _RequiredDescribeAlarmsForMetricInputRequestTypeDef = TypedDict(
     "_RequiredDescribeAlarmsForMetricInputRequestTypeDef",
     {
         "MetricName": str,
         "Namespace": str,
     },
 )
@@ -810,69 +745,14 @@
         "MetricName": str,
         "Dimensions": Sequence[DimensionTypeDef],
         "AnomalyDetectorTypes": Sequence[AnomalyDetectorTypeType],
     },
     total=False,
 )
 
-_RequiredGetMetricStatisticsInputMetricGetStatisticsTypeDef = TypedDict(
-    "_RequiredGetMetricStatisticsInputMetricGetStatisticsTypeDef",
-    {
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "Period": int,
-    },
-)
-_OptionalGetMetricStatisticsInputMetricGetStatisticsTypeDef = TypedDict(
-    "_OptionalGetMetricStatisticsInputMetricGetStatisticsTypeDef",
-    {
-        "Dimensions": Sequence[DimensionTypeDef],
-        "Statistics": Sequence[StatisticType],
-        "ExtendedStatistics": Sequence[str],
-        "Unit": StandardUnitType,
-    },
-    total=False,
-)
-
-
-class GetMetricStatisticsInputMetricGetStatisticsTypeDef(
-    _RequiredGetMetricStatisticsInputMetricGetStatisticsTypeDef,
-    _OptionalGetMetricStatisticsInputMetricGetStatisticsTypeDef,
-):
-    pass
-
-
-_RequiredGetMetricStatisticsInputRequestTypeDef = TypedDict(
-    "_RequiredGetMetricStatisticsInputRequestTypeDef",
-    {
-        "Namespace": str,
-        "MetricName": str,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "Period": int,
-    },
-)
-_OptionalGetMetricStatisticsInputRequestTypeDef = TypedDict(
-    "_OptionalGetMetricStatisticsInputRequestTypeDef",
-    {
-        "Dimensions": Sequence[DimensionTypeDef],
-        "Statistics": Sequence[StatisticType],
-        "ExtendedStatistics": Sequence[str],
-        "Unit": StandardUnitType,
-    },
-    total=False,
-)
-
-
-class GetMetricStatisticsInputRequestTypeDef(
-    _RequiredGetMetricStatisticsInputRequestTypeDef, _OptionalGetMetricStatisticsInputRequestTypeDef
-):
-    pass
-
-
 MetricOutputTypeDef = TypedDict(
     "MetricOutputTypeDef",
     {
         "Namespace": str,
         "MetricName": str,
         "Dimensions": List[DimensionTypeDef],
     },
@@ -1007,22 +887,141 @@
     "PutMetricStreamOutputTypeDef",
     {
         "Arn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DescribeAlarmHistoryInputAlarmDescribeHistoryTypeDef = TypedDict(
+    "DescribeAlarmHistoryInputAlarmDescribeHistoryTypeDef",
+    {
+        "AlarmTypes": Sequence[AlarmTypeType],
+        "HistoryItemType": HistoryItemTypeType,
+        "StartDate": TimestampTypeDef,
+        "EndDate": TimestampTypeDef,
+        "MaxRecords": int,
+        "NextToken": str,
+        "ScanBy": ScanByType,
+    },
+    total=False,
+)
+
+DescribeAlarmHistoryInputRequestTypeDef = TypedDict(
+    "DescribeAlarmHistoryInputRequestTypeDef",
+    {
+        "AlarmName": str,
+        "AlarmTypes": Sequence[AlarmTypeType],
+        "HistoryItemType": HistoryItemTypeType,
+        "StartDate": TimestampTypeDef,
+        "EndDate": TimestampTypeDef,
+        "MaxRecords": int,
+        "NextToken": str,
+        "ScanBy": ScanByType,
+    },
+    total=False,
+)
+
+_RequiredGetInsightRuleReportInputRequestTypeDef = TypedDict(
+    "_RequiredGetInsightRuleReportInputRequestTypeDef",
+    {
+        "RuleName": str,
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "Period": int,
+    },
+)
+_OptionalGetInsightRuleReportInputRequestTypeDef = TypedDict(
+    "_OptionalGetInsightRuleReportInputRequestTypeDef",
+    {
+        "MaxContributorCount": int,
+        "Metrics": Sequence[str],
+        "OrderBy": str,
+    },
+    total=False,
+)
+
+
+class GetInsightRuleReportInputRequestTypeDef(
+    _RequiredGetInsightRuleReportInputRequestTypeDef,
+    _OptionalGetInsightRuleReportInputRequestTypeDef,
+):
+    pass
+
+
+_RequiredGetMetricStatisticsInputMetricGetStatisticsTypeDef = TypedDict(
+    "_RequiredGetMetricStatisticsInputMetricGetStatisticsTypeDef",
+    {
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "Period": int,
+    },
+)
+_OptionalGetMetricStatisticsInputMetricGetStatisticsTypeDef = TypedDict(
+    "_OptionalGetMetricStatisticsInputMetricGetStatisticsTypeDef",
+    {
+        "Dimensions": Sequence[DimensionTypeDef],
+        "Statistics": Sequence[StatisticType],
+        "ExtendedStatistics": Sequence[str],
+        "Unit": StandardUnitType,
+    },
+    total=False,
+)
+
+
+class GetMetricStatisticsInputMetricGetStatisticsTypeDef(
+    _RequiredGetMetricStatisticsInputMetricGetStatisticsTypeDef,
+    _OptionalGetMetricStatisticsInputMetricGetStatisticsTypeDef,
+):
+    pass
+
+
+_RequiredGetMetricStatisticsInputRequestTypeDef = TypedDict(
+    "_RequiredGetMetricStatisticsInputRequestTypeDef",
+    {
+        "Namespace": str,
+        "MetricName": str,
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "Period": int,
+    },
+)
+_OptionalGetMetricStatisticsInputRequestTypeDef = TypedDict(
+    "_OptionalGetMetricStatisticsInputRequestTypeDef",
+    {
+        "Dimensions": Sequence[DimensionTypeDef],
+        "Statistics": Sequence[StatisticType],
+        "ExtendedStatistics": Sequence[str],
+        "Unit": StandardUnitType,
+    },
+    total=False,
+)
+
+
+class GetMetricStatisticsInputRequestTypeDef(
+    _RequiredGetMetricStatisticsInputRequestTypeDef, _OptionalGetMetricStatisticsInputRequestTypeDef
+):
+    pass
+
+
+RangeTypeDef = TypedDict(
+    "RangeTypeDef",
+    {
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+    },
+)
+
 DescribeAlarmHistoryInputDescribeAlarmHistoryPaginateTypeDef = TypedDict(
     "DescribeAlarmHistoryInputDescribeAlarmHistoryPaginateTypeDef",
     {
         "AlarmName": str,
         "AlarmTypes": Sequence[AlarmTypeType],
         "HistoryItemType": HistoryItemTypeType,
-        "StartDate": Union[datetime, str],
-        "EndDate": Union[datetime, str],
+        "StartDate": TimestampTypeDef,
+        "EndDate": TimestampTypeDef,
         "ScanBy": ScanByType,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeAlarmsInputDescribeAlarmsPaginateTypeDef = TypedDict(
@@ -1268,15 +1267,15 @@
         "MetricName": str,
     },
 )
 _OptionalMetricDatumTypeDef = TypedDict(
     "_OptionalMetricDatumTypeDef",
     {
         "Dimensions": Sequence[DimensionTypeDef],
-        "Timestamp": Union[datetime, str],
+        "Timestamp": TimestampTypeDef,
         "Value": float,
         "StatisticValues": StatisticSetTypeDef,
         "Values": Sequence[float],
         "Counts": Sequence[float],
         "Unit": StandardUnitType,
         "StorageResolution": int,
     },
@@ -1284,14 +1283,15 @@
 )
 
 
 class MetricDatumTypeDef(_RequiredMetricDatumTypeDef, _OptionalMetricDatumTypeDef):
     pass
 
 
+MetricStreamFilterUnionTypeDef = Union[MetricStreamFilterTypeDef, MetricStreamFilterOutputTypeDef]
 MetricStreamStatisticsConfigurationOutputTypeDef = TypedDict(
     "MetricStreamStatisticsConfigurationOutputTypeDef",
     {
         "IncludeMetrics": List[MetricStreamStatisticsMetricTypeDef],
         "AdditionalStatistics": List[str],
     },
 )
@@ -1352,14 +1352,26 @@
 )
 
 
 class MetricStatTypeDef(_RequiredMetricStatTypeDef, _OptionalMetricStatTypeDef):
     pass
 
 
+SingleMetricAnomalyDetectorUnionTypeDef = Union[
+    SingleMetricAnomalyDetectorTypeDef, SingleMetricAnomalyDetectorOutputTypeDef
+]
+AnomalyDetectorConfigurationTypeDef = TypedDict(
+    "AnomalyDetectorConfigurationTypeDef",
+    {
+        "ExcludedTimeRanges": Sequence[RangeTypeDef],
+        "MetricTimezone": str,
+    },
+    total=False,
+)
+
 GetMetricDataOutputTypeDef = TypedDict(
     "GetMetricDataOutputTypeDef",
     {
         "MetricDataResults": List[MetricDataResultTypeDef],
         "NextToken": str,
         "Messages": List[MessageDataTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1418,51 +1430,17 @@
         "OutputFormat": MetricStreamOutputFormatType,
         "StatisticsConfigurations": List[MetricStreamStatisticsConfigurationOutputTypeDef],
         "IncludeLinkedAccountsMetrics": bool,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredPutMetricStreamInputRequestTypeDef = TypedDict(
-    "_RequiredPutMetricStreamInputRequestTypeDef",
-    {
-        "Name": str,
-        "FirehoseArn": str,
-        "RoleArn": str,
-        "OutputFormat": MetricStreamOutputFormatType,
-    },
-)
-_OptionalPutMetricStreamInputRequestTypeDef = TypedDict(
-    "_OptionalPutMetricStreamInputRequestTypeDef",
-    {
-        "IncludeFilters": Sequence[
-            Union[MetricStreamFilterTypeDef, MetricStreamFilterOutputTypeDef]
-        ],
-        "ExcludeFilters": Sequence[
-            Union[MetricStreamFilterTypeDef, MetricStreamFilterOutputTypeDef]
-        ],
-        "Tags": Sequence[TagTypeDef],
-        "StatisticsConfigurations": Sequence[
-            Union[
-                MetricStreamStatisticsConfigurationTypeDef,
-                MetricStreamStatisticsConfigurationOutputTypeDef,
-            ]
-        ],
-        "IncludeLinkedAccountsMetrics": bool,
-    },
-    total=False,
-)
-
-
-class PutMetricStreamInputRequestTypeDef(
-    _RequiredPutMetricStreamInputRequestTypeDef, _OptionalPutMetricStreamInputRequestTypeDef
-):
-    pass
-
-
+MetricStreamStatisticsConfigurationUnionTypeDef = Union[
+    MetricStreamStatisticsConfigurationTypeDef, MetricStreamStatisticsConfigurationOutputTypeDef
+]
 _RequiredMetricDataQueryOutputTypeDef = TypedDict(
     "_RequiredMetricDataQueryOutputTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalMetricDataQueryOutputTypeDef = TypedDict(
@@ -1505,14 +1483,45 @@
 )
 
 
 class MetricDataQueryTypeDef(_RequiredMetricDataQueryTypeDef, _OptionalMetricDataQueryTypeDef):
     pass
 
 
+AnomalyDetectorConfigurationUnionTypeDef = Union[
+    AnomalyDetectorConfigurationTypeDef, AnomalyDetectorConfigurationOutputTypeDef
+]
+_RequiredPutMetricStreamInputRequestTypeDef = TypedDict(
+    "_RequiredPutMetricStreamInputRequestTypeDef",
+    {
+        "Name": str,
+        "FirehoseArn": str,
+        "RoleArn": str,
+        "OutputFormat": MetricStreamOutputFormatType,
+    },
+)
+_OptionalPutMetricStreamInputRequestTypeDef = TypedDict(
+    "_OptionalPutMetricStreamInputRequestTypeDef",
+    {
+        "IncludeFilters": Sequence[MetricStreamFilterUnionTypeDef],
+        "ExcludeFilters": Sequence[MetricStreamFilterUnionTypeDef],
+        "Tags": Sequence[TagTypeDef],
+        "StatisticsConfigurations": Sequence[MetricStreamStatisticsConfigurationUnionTypeDef],
+        "IncludeLinkedAccountsMetrics": bool,
+    },
+    total=False,
+)
+
+
+class PutMetricStreamInputRequestTypeDef(
+    _RequiredPutMetricStreamInputRequestTypeDef, _OptionalPutMetricStreamInputRequestTypeDef
+):
+    pass
+
+
 MetricAlarmTypeDef = TypedDict(
     "MetricAlarmTypeDef",
     {
         "AlarmName": str,
         "AlarmArn": str,
         "AlarmDescription": str,
         "AlarmConfigurationUpdatedTimestamp": datetime,
@@ -1549,66 +1558,15 @@
     "MetricMathAnomalyDetectorOutputTypeDef",
     {
         "MetricDataQueries": List[MetricDataQueryOutputTypeDef],
     },
     total=False,
 )
 
-_RequiredGetMetricDataInputGetMetricDataPaginateTypeDef = TypedDict(
-    "_RequiredGetMetricDataInputGetMetricDataPaginateTypeDef",
-    {
-        "MetricDataQueries": Sequence[Union[MetricDataQueryTypeDef, MetricDataQueryOutputTypeDef]],
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-    },
-)
-_OptionalGetMetricDataInputGetMetricDataPaginateTypeDef = TypedDict(
-    "_OptionalGetMetricDataInputGetMetricDataPaginateTypeDef",
-    {
-        "ScanBy": ScanByType,
-        "LabelOptions": LabelOptionsTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class GetMetricDataInputGetMetricDataPaginateTypeDef(
-    _RequiredGetMetricDataInputGetMetricDataPaginateTypeDef,
-    _OptionalGetMetricDataInputGetMetricDataPaginateTypeDef,
-):
-    pass
-
-
-_RequiredGetMetricDataInputRequestTypeDef = TypedDict(
-    "_RequiredGetMetricDataInputRequestTypeDef",
-    {
-        "MetricDataQueries": Sequence[Union[MetricDataQueryTypeDef, MetricDataQueryOutputTypeDef]],
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-    },
-)
-_OptionalGetMetricDataInputRequestTypeDef = TypedDict(
-    "_OptionalGetMetricDataInputRequestTypeDef",
-    {
-        "NextToken": str,
-        "ScanBy": ScanByType,
-        "MaxDatapoints": int,
-        "LabelOptions": LabelOptionsTypeDef,
-    },
-    total=False,
-)
-
-
-class GetMetricDataInputRequestTypeDef(
-    _RequiredGetMetricDataInputRequestTypeDef, _OptionalGetMetricDataInputRequestTypeDef
-):
-    pass
-
-
+MetricDataQueryUnionTypeDef = Union[MetricDataQueryTypeDef, MetricDataQueryOutputTypeDef]
 MetricMathAnomalyDetectorTypeDef = TypedDict(
     "MetricMathAnomalyDetectorTypeDef",
     {
         "MetricDataQueries": Sequence[MetricDataQueryTypeDef],
     },
     total=False,
 )
@@ -1649,14 +1607,99 @@
 class PutMetricAlarmInputMetricPutAlarmTypeDef(
     _RequiredPutMetricAlarmInputMetricPutAlarmTypeDef,
     _OptionalPutMetricAlarmInputMetricPutAlarmTypeDef,
 ):
     pass
 
 
+DescribeAlarmsForMetricOutputTypeDef = TypedDict(
+    "DescribeAlarmsForMetricOutputTypeDef",
+    {
+        "MetricAlarms": List[MetricAlarmTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeAlarmsOutputTypeDef = TypedDict(
+    "DescribeAlarmsOutputTypeDef",
+    {
+        "CompositeAlarms": List[CompositeAlarmTypeDef],
+        "MetricAlarms": List[MetricAlarmTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AnomalyDetectorTypeDef = TypedDict(
+    "AnomalyDetectorTypeDef",
+    {
+        "Namespace": str,
+        "MetricName": str,
+        "Dimensions": List[DimensionTypeDef],
+        "Stat": str,
+        "Configuration": AnomalyDetectorConfigurationOutputTypeDef,
+        "StateValue": AnomalyDetectorStateValueType,
+        "SingleMetricAnomalyDetector": SingleMetricAnomalyDetectorOutputTypeDef,
+        "MetricMathAnomalyDetector": MetricMathAnomalyDetectorOutputTypeDef,
+    },
+    total=False,
+)
+
+_RequiredGetMetricDataInputGetMetricDataPaginateTypeDef = TypedDict(
+    "_RequiredGetMetricDataInputGetMetricDataPaginateTypeDef",
+    {
+        "MetricDataQueries": Sequence[MetricDataQueryUnionTypeDef],
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+    },
+)
+_OptionalGetMetricDataInputGetMetricDataPaginateTypeDef = TypedDict(
+    "_OptionalGetMetricDataInputGetMetricDataPaginateTypeDef",
+    {
+        "ScanBy": ScanByType,
+        "LabelOptions": LabelOptionsTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetMetricDataInputGetMetricDataPaginateTypeDef(
+    _RequiredGetMetricDataInputGetMetricDataPaginateTypeDef,
+    _OptionalGetMetricDataInputGetMetricDataPaginateTypeDef,
+):
+    pass
+
+
+_RequiredGetMetricDataInputRequestTypeDef = TypedDict(
+    "_RequiredGetMetricDataInputRequestTypeDef",
+    {
+        "MetricDataQueries": Sequence[MetricDataQueryUnionTypeDef],
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+    },
+)
+_OptionalGetMetricDataInputRequestTypeDef = TypedDict(
+    "_OptionalGetMetricDataInputRequestTypeDef",
+    {
+        "NextToken": str,
+        "ScanBy": ScanByType,
+        "MaxDatapoints": int,
+        "LabelOptions": LabelOptionsTypeDef,
+    },
+    total=False,
+)
+
+
+class GetMetricDataInputRequestTypeDef(
+    _RequiredGetMetricDataInputRequestTypeDef, _OptionalGetMetricDataInputRequestTypeDef
+):
+    pass
+
+
 _RequiredPutMetricAlarmInputRequestTypeDef = TypedDict(
     "_RequiredPutMetricAlarmInputRequestTypeDef",
     {
         "AlarmName": str,
         "EvaluationPeriods": int,
         "ComparisonOperator": ComparisonOperatorType,
     },
@@ -1676,74 +1719,44 @@
         "Dimensions": Sequence[DimensionTypeDef],
         "Period": int,
         "Unit": StandardUnitType,
         "DatapointsToAlarm": int,
         "Threshold": float,
         "TreatMissingData": str,
         "EvaluateLowSampleCountPercentile": str,
-        "Metrics": Sequence[Union[MetricDataQueryTypeDef, MetricDataQueryOutputTypeDef]],
+        "Metrics": Sequence[MetricDataQueryUnionTypeDef],
         "Tags": Sequence[TagTypeDef],
         "ThresholdMetricId": str,
     },
     total=False,
 )
 
 
 class PutMetricAlarmInputRequestTypeDef(
     _RequiredPutMetricAlarmInputRequestTypeDef, _OptionalPutMetricAlarmInputRequestTypeDef
 ):
     pass
 
 
-DescribeAlarmsForMetricOutputTypeDef = TypedDict(
-    "DescribeAlarmsForMetricOutputTypeDef",
-    {
-        "MetricAlarms": List[MetricAlarmTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeAlarmsOutputTypeDef = TypedDict(
-    "DescribeAlarmsOutputTypeDef",
-    {
-        "CompositeAlarms": List[CompositeAlarmTypeDef],
-        "MetricAlarms": List[MetricAlarmTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-AnomalyDetectorTypeDef = TypedDict(
-    "AnomalyDetectorTypeDef",
-    {
-        "Namespace": str,
-        "MetricName": str,
-        "Dimensions": List[DimensionTypeDef],
-        "Stat": str,
-        "Configuration": AnomalyDetectorConfigurationOutputTypeDef,
-        "StateValue": AnomalyDetectorStateValueType,
-        "SingleMetricAnomalyDetector": SingleMetricAnomalyDetectorOutputTypeDef,
-        "MetricMathAnomalyDetector": MetricMathAnomalyDetectorOutputTypeDef,
-    },
-    total=False,
-)
-
 DeleteAnomalyDetectorInputRequestTypeDef = TypedDict(
     "DeleteAnomalyDetectorInputRequestTypeDef",
     {
         "Namespace": str,
         "MetricName": str,
         "Dimensions": Sequence[DimensionTypeDef],
         "Stat": str,
         "SingleMetricAnomalyDetector": SingleMetricAnomalyDetectorTypeDef,
         "MetricMathAnomalyDetector": MetricMathAnomalyDetectorTypeDef,
     },
     total=False,
 )
 
+MetricMathAnomalyDetectorUnionTypeDef = Union[
+    MetricMathAnomalyDetectorTypeDef, MetricMathAnomalyDetectorOutputTypeDef
+]
 PutAnomalyDetectorInputRequestTypeDef = TypedDict(
     "PutAnomalyDetectorInputRequestTypeDef",
     {
         "Namespace": str,
         "MetricName": str,
         "Dimensions": Sequence[DimensionTypeDef],
         "Stat": str,
```

### Comparing `mypy-boto3-cloudwatch-1.28.15.post1/mypy_boto3_cloudwatch/type_defs.pyi` & `mypy-boto3-cloudwatch-1.28.16/mypy_boto3_cloudwatch/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_cloudwatch.type_defs import AlarmHistoryItemTypeDef
 
-    data: AlarmHistoryItemTypeDef = {...}
+    data: AlarmHistoryItemTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -38,40 +38,37 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AlarmHistoryItemTypeDef",
     "RangeOutputTypeDef",
-    "RangeTypeDef",
     "DimensionTypeDef",
     "CompositeAlarmTypeDef",
     "DashboardEntryTypeDef",
     "DashboardValidationMessageTypeDef",
     "DatapointTypeDef",
     "DeleteAlarmsInputRequestTypeDef",
     "DeleteDashboardsInputRequestTypeDef",
     "DeleteInsightRulesInputRequestTypeDef",
     "PartialFailureTypeDef",
     "ResponseMetadataTypeDef",
     "DeleteMetricStreamInputRequestTypeDef",
-    "DescribeAlarmHistoryInputAlarmDescribeHistoryTypeDef",
+    "TimestampTypeDef",
     "PaginatorConfigTypeDef",
-    "DescribeAlarmHistoryInputRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeAlarmsInputRequestTypeDef",
     "DescribeInsightRulesInputRequestTypeDef",
     "InsightRuleTypeDef",
     "DimensionFilterTypeDef",
     "DisableAlarmActionsInputRequestTypeDef",
     "DisableInsightRulesInputRequestTypeDef",
     "EnableAlarmActionsInputRequestTypeDef",
     "EnableInsightRulesInputRequestTypeDef",
     "GetDashboardInputRequestTypeDef",
-    "GetInsightRuleReportInputRequestTypeDef",
     "InsightRuleMetricDatapointTypeDef",
     "LabelOptionsTypeDef",
     "MessageDataTypeDef",
     "GetMetricStreamInputRequestTypeDef",
     "MetricStreamFilterOutputTypeDef",
     "GetMetricWidgetImageInputRequestTypeDef",
     "InsightRuleContributorDatapointTypeDef",
@@ -88,19 +85,16 @@
     "PutDashboardInputRequestTypeDef",
     "SetAlarmStateInputAlarmSetStateTypeDef",
     "SetAlarmStateInputRequestTypeDef",
     "StartMetricStreamsInputRequestTypeDef",
     "StopMetricStreamsInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "AnomalyDetectorConfigurationOutputTypeDef",
-    "AnomalyDetectorConfigurationTypeDef",
     "DescribeAlarmsForMetricInputRequestTypeDef",
     "DescribeAnomalyDetectorsInputRequestTypeDef",
-    "GetMetricStatisticsInputMetricGetStatisticsTypeDef",
-    "GetMetricStatisticsInputRequestTypeDef",
     "MetricOutputTypeDef",
     "MetricTypeDef",
     "SingleMetricAnomalyDetectorOutputTypeDef",
     "SingleMetricAnomalyDetectorTypeDef",
     "DeleteInsightRulesOutputTypeDef",
     "DescribeAlarmHistoryOutputTypeDef",
     "DisableInsightRulesOutputTypeDef",
@@ -109,14 +103,20 @@
     "GetDashboardOutputTypeDef",
     "GetMetricStatisticsOutputTypeDef",
     "GetMetricWidgetImageOutputTypeDef",
     "ListDashboardsOutputTypeDef",
     "PutDashboardOutputTypeDef",
     "PutManagedInsightRulesOutputTypeDef",
     "PutMetricStreamOutputTypeDef",
+    "DescribeAlarmHistoryInputAlarmDescribeHistoryTypeDef",
+    "DescribeAlarmHistoryInputRequestTypeDef",
+    "GetInsightRuleReportInputRequestTypeDef",
+    "GetMetricStatisticsInputMetricGetStatisticsTypeDef",
+    "GetMetricStatisticsInputRequestTypeDef",
+    "RangeTypeDef",
     "DescribeAlarmHistoryInputDescribeAlarmHistoryPaginateTypeDef",
     "DescribeAlarmsInputDescribeAlarmsPaginateTypeDef",
     "DescribeAnomalyDetectorsInputDescribeAnomalyDetectorsPaginateTypeDef",
     "ListDashboardsInputListDashboardsPaginateTypeDef",
     "DescribeAlarmsInputAlarmExistsWaitTypeDef",
     "DescribeAlarmsInputCompositeAlarmExistsWaitTypeDef",
     "DescribeInsightRulesOutputTypeDef",
@@ -128,39 +128,46 @@
     "ListTagsForResourceOutputTypeDef",
     "ManagedRuleTypeDef",
     "PutCompositeAlarmInputRequestTypeDef",
     "PutInsightRuleInputRequestTypeDef",
     "TagResourceInputRequestTypeDef",
     "ManagedRuleDescriptionTypeDef",
     "MetricDatumTypeDef",
+    "MetricStreamFilterUnionTypeDef",
     "MetricStreamStatisticsConfigurationOutputTypeDef",
     "MetricStreamStatisticsConfigurationTypeDef",
     "ListMetricsOutputTypeDef",
     "MetricStatOutputTypeDef",
     "MetricStatTypeDef",
+    "SingleMetricAnomalyDetectorUnionTypeDef",
+    "AnomalyDetectorConfigurationTypeDef",
     "GetMetricDataOutputTypeDef",
     "GetInsightRuleReportOutputTypeDef",
     "PutManagedInsightRulesInputRequestTypeDef",
     "ListManagedInsightRulesOutputTypeDef",
     "PutMetricDataInputRequestTypeDef",
     "GetMetricStreamOutputTypeDef",
-    "PutMetricStreamInputRequestTypeDef",
+    "MetricStreamStatisticsConfigurationUnionTypeDef",
     "MetricDataQueryOutputTypeDef",
     "MetricDataQueryTypeDef",
+    "AnomalyDetectorConfigurationUnionTypeDef",
+    "PutMetricStreamInputRequestTypeDef",
     "MetricAlarmTypeDef",
     "MetricMathAnomalyDetectorOutputTypeDef",
-    "GetMetricDataInputGetMetricDataPaginateTypeDef",
-    "GetMetricDataInputRequestTypeDef",
+    "MetricDataQueryUnionTypeDef",
     "MetricMathAnomalyDetectorTypeDef",
     "PutMetricAlarmInputMetricPutAlarmTypeDef",
-    "PutMetricAlarmInputRequestTypeDef",
     "DescribeAlarmsForMetricOutputTypeDef",
     "DescribeAlarmsOutputTypeDef",
     "AnomalyDetectorTypeDef",
+    "GetMetricDataInputGetMetricDataPaginateTypeDef",
+    "GetMetricDataInputRequestTypeDef",
+    "PutMetricAlarmInputRequestTypeDef",
     "DeleteAnomalyDetectorInputRequestTypeDef",
+    "MetricMathAnomalyDetectorUnionTypeDef",
     "PutAnomalyDetectorInputRequestTypeDef",
     "DescribeAnomalyDetectorsOutputTypeDef",
 )
 
 AlarmHistoryItemTypeDef = TypedDict(
     "AlarmHistoryItemTypeDef",
     {
@@ -178,22 +185,14 @@
     "RangeOutputTypeDef",
     {
         "StartTime": datetime,
         "EndTime": datetime,
     },
 )
 
-RangeTypeDef = TypedDict(
-    "RangeTypeDef",
-    {
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-    },
-)
-
 DimensionTypeDef = TypedDict(
     "DimensionTypeDef",
     {
         "Name": str,
         "Value": str,
     },
 )
@@ -305,53 +304,25 @@
 DeleteMetricStreamInputRequestTypeDef = TypedDict(
     "DeleteMetricStreamInputRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-DescribeAlarmHistoryInputAlarmDescribeHistoryTypeDef = TypedDict(
-    "DescribeAlarmHistoryInputAlarmDescribeHistoryTypeDef",
-    {
-        "AlarmTypes": Sequence[AlarmTypeType],
-        "HistoryItemType": HistoryItemTypeType,
-        "StartDate": Union[datetime, str],
-        "EndDate": Union[datetime, str],
-        "MaxRecords": int,
-        "NextToken": str,
-        "ScanBy": ScanByType,
-    },
-    total=False,
-)
-
+TimestampTypeDef = Union[datetime, str]
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
-DescribeAlarmHistoryInputRequestTypeDef = TypedDict(
-    "DescribeAlarmHistoryInputRequestTypeDef",
-    {
-        "AlarmName": str,
-        "AlarmTypes": Sequence[AlarmTypeType],
-        "HistoryItemType": HistoryItemTypeType,
-        "StartDate": Union[datetime, str],
-        "EndDate": Union[datetime, str],
-        "MaxRecords": int,
-        "NextToken": str,
-        "ScanBy": ScanByType,
-    },
-    total=False,
-)
-
 WaiterConfigTypeDef = TypedDict(
     "WaiterConfigTypeDef",
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
@@ -450,39 +421,14 @@
 GetDashboardInputRequestTypeDef = TypedDict(
     "GetDashboardInputRequestTypeDef",
     {
         "DashboardName": str,
     },
 )
 
-_RequiredGetInsightRuleReportInputRequestTypeDef = TypedDict(
-    "_RequiredGetInsightRuleReportInputRequestTypeDef",
-    {
-        "RuleName": str,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "Period": int,
-    },
-)
-_OptionalGetInsightRuleReportInputRequestTypeDef = TypedDict(
-    "_OptionalGetInsightRuleReportInputRequestTypeDef",
-    {
-        "MaxContributorCount": int,
-        "Metrics": Sequence[str],
-        "OrderBy": str,
-    },
-    total=False,
-)
-
-class GetInsightRuleReportInputRequestTypeDef(
-    _RequiredGetInsightRuleReportInputRequestTypeDef,
-    _OptionalGetInsightRuleReportInputRequestTypeDef,
-):
-    pass
-
 _RequiredInsightRuleMetricDatapointTypeDef = TypedDict(
     "_RequiredInsightRuleMetricDatapointTypeDef",
     {
         "Timestamp": datetime,
     },
 )
 _OptionalInsightRuleMetricDatapointTypeDef = TypedDict(
@@ -744,23 +690,14 @@
     {
         "ExcludedTimeRanges": List[RangeOutputTypeDef],
         "MetricTimezone": str,
     },
     total=False,
 )
 
-AnomalyDetectorConfigurationTypeDef = TypedDict(
-    "AnomalyDetectorConfigurationTypeDef",
-    {
-        "ExcludedTimeRanges": Sequence[RangeTypeDef],
-        "MetricTimezone": str,
-    },
-    total=False,
-)
-
 _RequiredDescribeAlarmsForMetricInputRequestTypeDef = TypedDict(
     "_RequiredDescribeAlarmsForMetricInputRequestTypeDef",
     {
         "MetricName": str,
         "Namespace": str,
     },
 )
@@ -791,65 +728,14 @@
         "MetricName": str,
         "Dimensions": Sequence[DimensionTypeDef],
         "AnomalyDetectorTypes": Sequence[AnomalyDetectorTypeType],
     },
     total=False,
 )
 
-_RequiredGetMetricStatisticsInputMetricGetStatisticsTypeDef = TypedDict(
-    "_RequiredGetMetricStatisticsInputMetricGetStatisticsTypeDef",
-    {
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "Period": int,
-    },
-)
-_OptionalGetMetricStatisticsInputMetricGetStatisticsTypeDef = TypedDict(
-    "_OptionalGetMetricStatisticsInputMetricGetStatisticsTypeDef",
-    {
-        "Dimensions": Sequence[DimensionTypeDef],
-        "Statistics": Sequence[StatisticType],
-        "ExtendedStatistics": Sequence[str],
-        "Unit": StandardUnitType,
-    },
-    total=False,
-)
-
-class GetMetricStatisticsInputMetricGetStatisticsTypeDef(
-    _RequiredGetMetricStatisticsInputMetricGetStatisticsTypeDef,
-    _OptionalGetMetricStatisticsInputMetricGetStatisticsTypeDef,
-):
-    pass
-
-_RequiredGetMetricStatisticsInputRequestTypeDef = TypedDict(
-    "_RequiredGetMetricStatisticsInputRequestTypeDef",
-    {
-        "Namespace": str,
-        "MetricName": str,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "Period": int,
-    },
-)
-_OptionalGetMetricStatisticsInputRequestTypeDef = TypedDict(
-    "_OptionalGetMetricStatisticsInputRequestTypeDef",
-    {
-        "Dimensions": Sequence[DimensionTypeDef],
-        "Statistics": Sequence[StatisticType],
-        "ExtendedStatistics": Sequence[str],
-        "Unit": StandardUnitType,
-    },
-    total=False,
-)
-
-class GetMetricStatisticsInputRequestTypeDef(
-    _RequiredGetMetricStatisticsInputRequestTypeDef, _OptionalGetMetricStatisticsInputRequestTypeDef
-):
-    pass
-
 MetricOutputTypeDef = TypedDict(
     "MetricOutputTypeDef",
     {
         "Namespace": str,
         "MetricName": str,
         "Dimensions": List[DimensionTypeDef],
     },
@@ -984,22 +870,135 @@
     "PutMetricStreamOutputTypeDef",
     {
         "Arn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DescribeAlarmHistoryInputAlarmDescribeHistoryTypeDef = TypedDict(
+    "DescribeAlarmHistoryInputAlarmDescribeHistoryTypeDef",
+    {
+        "AlarmTypes": Sequence[AlarmTypeType],
+        "HistoryItemType": HistoryItemTypeType,
+        "StartDate": TimestampTypeDef,
+        "EndDate": TimestampTypeDef,
+        "MaxRecords": int,
+        "NextToken": str,
+        "ScanBy": ScanByType,
+    },
+    total=False,
+)
+
+DescribeAlarmHistoryInputRequestTypeDef = TypedDict(
+    "DescribeAlarmHistoryInputRequestTypeDef",
+    {
+        "AlarmName": str,
+        "AlarmTypes": Sequence[AlarmTypeType],
+        "HistoryItemType": HistoryItemTypeType,
+        "StartDate": TimestampTypeDef,
+        "EndDate": TimestampTypeDef,
+        "MaxRecords": int,
+        "NextToken": str,
+        "ScanBy": ScanByType,
+    },
+    total=False,
+)
+
+_RequiredGetInsightRuleReportInputRequestTypeDef = TypedDict(
+    "_RequiredGetInsightRuleReportInputRequestTypeDef",
+    {
+        "RuleName": str,
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "Period": int,
+    },
+)
+_OptionalGetInsightRuleReportInputRequestTypeDef = TypedDict(
+    "_OptionalGetInsightRuleReportInputRequestTypeDef",
+    {
+        "MaxContributorCount": int,
+        "Metrics": Sequence[str],
+        "OrderBy": str,
+    },
+    total=False,
+)
+
+class GetInsightRuleReportInputRequestTypeDef(
+    _RequiredGetInsightRuleReportInputRequestTypeDef,
+    _OptionalGetInsightRuleReportInputRequestTypeDef,
+):
+    pass
+
+_RequiredGetMetricStatisticsInputMetricGetStatisticsTypeDef = TypedDict(
+    "_RequiredGetMetricStatisticsInputMetricGetStatisticsTypeDef",
+    {
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "Period": int,
+    },
+)
+_OptionalGetMetricStatisticsInputMetricGetStatisticsTypeDef = TypedDict(
+    "_OptionalGetMetricStatisticsInputMetricGetStatisticsTypeDef",
+    {
+        "Dimensions": Sequence[DimensionTypeDef],
+        "Statistics": Sequence[StatisticType],
+        "ExtendedStatistics": Sequence[str],
+        "Unit": StandardUnitType,
+    },
+    total=False,
+)
+
+class GetMetricStatisticsInputMetricGetStatisticsTypeDef(
+    _RequiredGetMetricStatisticsInputMetricGetStatisticsTypeDef,
+    _OptionalGetMetricStatisticsInputMetricGetStatisticsTypeDef,
+):
+    pass
+
+_RequiredGetMetricStatisticsInputRequestTypeDef = TypedDict(
+    "_RequiredGetMetricStatisticsInputRequestTypeDef",
+    {
+        "Namespace": str,
+        "MetricName": str,
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "Period": int,
+    },
+)
+_OptionalGetMetricStatisticsInputRequestTypeDef = TypedDict(
+    "_OptionalGetMetricStatisticsInputRequestTypeDef",
+    {
+        "Dimensions": Sequence[DimensionTypeDef],
+        "Statistics": Sequence[StatisticType],
+        "ExtendedStatistics": Sequence[str],
+        "Unit": StandardUnitType,
+    },
+    total=False,
+)
+
+class GetMetricStatisticsInputRequestTypeDef(
+    _RequiredGetMetricStatisticsInputRequestTypeDef, _OptionalGetMetricStatisticsInputRequestTypeDef
+):
+    pass
+
+RangeTypeDef = TypedDict(
+    "RangeTypeDef",
+    {
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+    },
+)
+
 DescribeAlarmHistoryInputDescribeAlarmHistoryPaginateTypeDef = TypedDict(
     "DescribeAlarmHistoryInputDescribeAlarmHistoryPaginateTypeDef",
     {
         "AlarmName": str,
         "AlarmTypes": Sequence[AlarmTypeType],
         "HistoryItemType": HistoryItemTypeType,
-        "StartDate": Union[datetime, str],
-        "EndDate": Union[datetime, str],
+        "StartDate": TimestampTypeDef,
+        "EndDate": TimestampTypeDef,
         "ScanBy": ScanByType,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeAlarmsInputDescribeAlarmsPaginateTypeDef = TypedDict(
@@ -1239,28 +1238,29 @@
         "MetricName": str,
     },
 )
 _OptionalMetricDatumTypeDef = TypedDict(
     "_OptionalMetricDatumTypeDef",
     {
         "Dimensions": Sequence[DimensionTypeDef],
-        "Timestamp": Union[datetime, str],
+        "Timestamp": TimestampTypeDef,
         "Value": float,
         "StatisticValues": StatisticSetTypeDef,
         "Values": Sequence[float],
         "Counts": Sequence[float],
         "Unit": StandardUnitType,
         "StorageResolution": int,
     },
     total=False,
 )
 
 class MetricDatumTypeDef(_RequiredMetricDatumTypeDef, _OptionalMetricDatumTypeDef):
     pass
 
+MetricStreamFilterUnionTypeDef = Union[MetricStreamFilterTypeDef, MetricStreamFilterOutputTypeDef]
 MetricStreamStatisticsConfigurationOutputTypeDef = TypedDict(
     "MetricStreamStatisticsConfigurationOutputTypeDef",
     {
         "IncludeMetrics": List[MetricStreamStatisticsMetricTypeDef],
         "AdditionalStatistics": List[str],
     },
 )
@@ -1317,14 +1317,26 @@
     },
     total=False,
 )
 
 class MetricStatTypeDef(_RequiredMetricStatTypeDef, _OptionalMetricStatTypeDef):
     pass
 
+SingleMetricAnomalyDetectorUnionTypeDef = Union[
+    SingleMetricAnomalyDetectorTypeDef, SingleMetricAnomalyDetectorOutputTypeDef
+]
+AnomalyDetectorConfigurationTypeDef = TypedDict(
+    "AnomalyDetectorConfigurationTypeDef",
+    {
+        "ExcludedTimeRanges": Sequence[RangeTypeDef],
+        "MetricTimezone": str,
+    },
+    total=False,
+)
+
 GetMetricDataOutputTypeDef = TypedDict(
     "GetMetricDataOutputTypeDef",
     {
         "MetricDataResults": List[MetricDataResultTypeDef],
         "NextToken": str,
         "Messages": List[MessageDataTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1383,49 +1395,17 @@
         "OutputFormat": MetricStreamOutputFormatType,
         "StatisticsConfigurations": List[MetricStreamStatisticsConfigurationOutputTypeDef],
         "IncludeLinkedAccountsMetrics": bool,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredPutMetricStreamInputRequestTypeDef = TypedDict(
-    "_RequiredPutMetricStreamInputRequestTypeDef",
-    {
-        "Name": str,
-        "FirehoseArn": str,
-        "RoleArn": str,
-        "OutputFormat": MetricStreamOutputFormatType,
-    },
-)
-_OptionalPutMetricStreamInputRequestTypeDef = TypedDict(
-    "_OptionalPutMetricStreamInputRequestTypeDef",
-    {
-        "IncludeFilters": Sequence[
-            Union[MetricStreamFilterTypeDef, MetricStreamFilterOutputTypeDef]
-        ],
-        "ExcludeFilters": Sequence[
-            Union[MetricStreamFilterTypeDef, MetricStreamFilterOutputTypeDef]
-        ],
-        "Tags": Sequence[TagTypeDef],
-        "StatisticsConfigurations": Sequence[
-            Union[
-                MetricStreamStatisticsConfigurationTypeDef,
-                MetricStreamStatisticsConfigurationOutputTypeDef,
-            ]
-        ],
-        "IncludeLinkedAccountsMetrics": bool,
-    },
-    total=False,
-)
-
-class PutMetricStreamInputRequestTypeDef(
-    _RequiredPutMetricStreamInputRequestTypeDef, _OptionalPutMetricStreamInputRequestTypeDef
-):
-    pass
-
+MetricStreamStatisticsConfigurationUnionTypeDef = Union[
+    MetricStreamStatisticsConfigurationTypeDef, MetricStreamStatisticsConfigurationOutputTypeDef
+]
 _RequiredMetricDataQueryOutputTypeDef = TypedDict(
     "_RequiredMetricDataQueryOutputTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalMetricDataQueryOutputTypeDef = TypedDict(
@@ -1464,14 +1444,43 @@
     },
     total=False,
 )
 
 class MetricDataQueryTypeDef(_RequiredMetricDataQueryTypeDef, _OptionalMetricDataQueryTypeDef):
     pass
 
+AnomalyDetectorConfigurationUnionTypeDef = Union[
+    AnomalyDetectorConfigurationTypeDef, AnomalyDetectorConfigurationOutputTypeDef
+]
+_RequiredPutMetricStreamInputRequestTypeDef = TypedDict(
+    "_RequiredPutMetricStreamInputRequestTypeDef",
+    {
+        "Name": str,
+        "FirehoseArn": str,
+        "RoleArn": str,
+        "OutputFormat": MetricStreamOutputFormatType,
+    },
+)
+_OptionalPutMetricStreamInputRequestTypeDef = TypedDict(
+    "_OptionalPutMetricStreamInputRequestTypeDef",
+    {
+        "IncludeFilters": Sequence[MetricStreamFilterUnionTypeDef],
+        "ExcludeFilters": Sequence[MetricStreamFilterUnionTypeDef],
+        "Tags": Sequence[TagTypeDef],
+        "StatisticsConfigurations": Sequence[MetricStreamStatisticsConfigurationUnionTypeDef],
+        "IncludeLinkedAccountsMetrics": bool,
+    },
+    total=False,
+)
+
+class PutMetricStreamInputRequestTypeDef(
+    _RequiredPutMetricStreamInputRequestTypeDef, _OptionalPutMetricStreamInputRequestTypeDef
+):
+    pass
+
 MetricAlarmTypeDef = TypedDict(
     "MetricAlarmTypeDef",
     {
         "AlarmName": str,
         "AlarmArn": str,
         "AlarmDescription": str,
         "AlarmConfigurationUpdatedTimestamp": datetime,
@@ -1508,62 +1517,15 @@
     "MetricMathAnomalyDetectorOutputTypeDef",
     {
         "MetricDataQueries": List[MetricDataQueryOutputTypeDef],
     },
     total=False,
 )
 
-_RequiredGetMetricDataInputGetMetricDataPaginateTypeDef = TypedDict(
-    "_RequiredGetMetricDataInputGetMetricDataPaginateTypeDef",
-    {
-        "MetricDataQueries": Sequence[Union[MetricDataQueryTypeDef, MetricDataQueryOutputTypeDef]],
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-    },
-)
-_OptionalGetMetricDataInputGetMetricDataPaginateTypeDef = TypedDict(
-    "_OptionalGetMetricDataInputGetMetricDataPaginateTypeDef",
-    {
-        "ScanBy": ScanByType,
-        "LabelOptions": LabelOptionsTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class GetMetricDataInputGetMetricDataPaginateTypeDef(
-    _RequiredGetMetricDataInputGetMetricDataPaginateTypeDef,
-    _OptionalGetMetricDataInputGetMetricDataPaginateTypeDef,
-):
-    pass
-
-_RequiredGetMetricDataInputRequestTypeDef = TypedDict(
-    "_RequiredGetMetricDataInputRequestTypeDef",
-    {
-        "MetricDataQueries": Sequence[Union[MetricDataQueryTypeDef, MetricDataQueryOutputTypeDef]],
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-    },
-)
-_OptionalGetMetricDataInputRequestTypeDef = TypedDict(
-    "_OptionalGetMetricDataInputRequestTypeDef",
-    {
-        "NextToken": str,
-        "ScanBy": ScanByType,
-        "MaxDatapoints": int,
-        "LabelOptions": LabelOptionsTypeDef,
-    },
-    total=False,
-)
-
-class GetMetricDataInputRequestTypeDef(
-    _RequiredGetMetricDataInputRequestTypeDef, _OptionalGetMetricDataInputRequestTypeDef
-):
-    pass
-
+MetricDataQueryUnionTypeDef = Union[MetricDataQueryTypeDef, MetricDataQueryOutputTypeDef]
 MetricMathAnomalyDetectorTypeDef = TypedDict(
     "MetricMathAnomalyDetectorTypeDef",
     {
         "MetricDataQueries": Sequence[MetricDataQueryTypeDef],
     },
     total=False,
 )
@@ -1602,14 +1564,95 @@
 
 class PutMetricAlarmInputMetricPutAlarmTypeDef(
     _RequiredPutMetricAlarmInputMetricPutAlarmTypeDef,
     _OptionalPutMetricAlarmInputMetricPutAlarmTypeDef,
 ):
     pass
 
+DescribeAlarmsForMetricOutputTypeDef = TypedDict(
+    "DescribeAlarmsForMetricOutputTypeDef",
+    {
+        "MetricAlarms": List[MetricAlarmTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeAlarmsOutputTypeDef = TypedDict(
+    "DescribeAlarmsOutputTypeDef",
+    {
+        "CompositeAlarms": List[CompositeAlarmTypeDef],
+        "MetricAlarms": List[MetricAlarmTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AnomalyDetectorTypeDef = TypedDict(
+    "AnomalyDetectorTypeDef",
+    {
+        "Namespace": str,
+        "MetricName": str,
+        "Dimensions": List[DimensionTypeDef],
+        "Stat": str,
+        "Configuration": AnomalyDetectorConfigurationOutputTypeDef,
+        "StateValue": AnomalyDetectorStateValueType,
+        "SingleMetricAnomalyDetector": SingleMetricAnomalyDetectorOutputTypeDef,
+        "MetricMathAnomalyDetector": MetricMathAnomalyDetectorOutputTypeDef,
+    },
+    total=False,
+)
+
+_RequiredGetMetricDataInputGetMetricDataPaginateTypeDef = TypedDict(
+    "_RequiredGetMetricDataInputGetMetricDataPaginateTypeDef",
+    {
+        "MetricDataQueries": Sequence[MetricDataQueryUnionTypeDef],
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+    },
+)
+_OptionalGetMetricDataInputGetMetricDataPaginateTypeDef = TypedDict(
+    "_OptionalGetMetricDataInputGetMetricDataPaginateTypeDef",
+    {
+        "ScanBy": ScanByType,
+        "LabelOptions": LabelOptionsTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetMetricDataInputGetMetricDataPaginateTypeDef(
+    _RequiredGetMetricDataInputGetMetricDataPaginateTypeDef,
+    _OptionalGetMetricDataInputGetMetricDataPaginateTypeDef,
+):
+    pass
+
+_RequiredGetMetricDataInputRequestTypeDef = TypedDict(
+    "_RequiredGetMetricDataInputRequestTypeDef",
+    {
+        "MetricDataQueries": Sequence[MetricDataQueryUnionTypeDef],
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+    },
+)
+_OptionalGetMetricDataInputRequestTypeDef = TypedDict(
+    "_OptionalGetMetricDataInputRequestTypeDef",
+    {
+        "NextToken": str,
+        "ScanBy": ScanByType,
+        "MaxDatapoints": int,
+        "LabelOptions": LabelOptionsTypeDef,
+    },
+    total=False,
+)
+
+class GetMetricDataInputRequestTypeDef(
+    _RequiredGetMetricDataInputRequestTypeDef, _OptionalGetMetricDataInputRequestTypeDef
+):
+    pass
+
 _RequiredPutMetricAlarmInputRequestTypeDef = TypedDict(
     "_RequiredPutMetricAlarmInputRequestTypeDef",
     {
         "AlarmName": str,
         "EvaluationPeriods": int,
         "ComparisonOperator": ComparisonOperatorType,
     },
@@ -1629,72 +1672,42 @@
         "Dimensions": Sequence[DimensionTypeDef],
         "Period": int,
         "Unit": StandardUnitType,
         "DatapointsToAlarm": int,
         "Threshold": float,
         "TreatMissingData": str,
         "EvaluateLowSampleCountPercentile": str,
-        "Metrics": Sequence[Union[MetricDataQueryTypeDef, MetricDataQueryOutputTypeDef]],
+        "Metrics": Sequence[MetricDataQueryUnionTypeDef],
         "Tags": Sequence[TagTypeDef],
         "ThresholdMetricId": str,
     },
     total=False,
 )
 
 class PutMetricAlarmInputRequestTypeDef(
     _RequiredPutMetricAlarmInputRequestTypeDef, _OptionalPutMetricAlarmInputRequestTypeDef
 ):
     pass
 
-DescribeAlarmsForMetricOutputTypeDef = TypedDict(
-    "DescribeAlarmsForMetricOutputTypeDef",
-    {
-        "MetricAlarms": List[MetricAlarmTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeAlarmsOutputTypeDef = TypedDict(
-    "DescribeAlarmsOutputTypeDef",
-    {
-        "CompositeAlarms": List[CompositeAlarmTypeDef],
-        "MetricAlarms": List[MetricAlarmTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-AnomalyDetectorTypeDef = TypedDict(
-    "AnomalyDetectorTypeDef",
-    {
-        "Namespace": str,
-        "MetricName": str,
-        "Dimensions": List[DimensionTypeDef],
-        "Stat": str,
-        "Configuration": AnomalyDetectorConfigurationOutputTypeDef,
-        "StateValue": AnomalyDetectorStateValueType,
-        "SingleMetricAnomalyDetector": SingleMetricAnomalyDetectorOutputTypeDef,
-        "MetricMathAnomalyDetector": MetricMathAnomalyDetectorOutputTypeDef,
-    },
-    total=False,
-)
-
 DeleteAnomalyDetectorInputRequestTypeDef = TypedDict(
     "DeleteAnomalyDetectorInputRequestTypeDef",
     {
         "Namespace": str,
         "MetricName": str,
         "Dimensions": Sequence[DimensionTypeDef],
         "Stat": str,
         "SingleMetricAnomalyDetector": SingleMetricAnomalyDetectorTypeDef,
         "MetricMathAnomalyDetector": MetricMathAnomalyDetectorTypeDef,
     },
     total=False,
 )
 
+MetricMathAnomalyDetectorUnionTypeDef = Union[
+    MetricMathAnomalyDetectorTypeDef, MetricMathAnomalyDetectorOutputTypeDef
+]
 PutAnomalyDetectorInputRequestTypeDef = TypedDict(
     "PutAnomalyDetectorInputRequestTypeDef",
     {
         "Namespace": str,
         "MetricName": str,
         "Dimensions": Sequence[DimensionTypeDef],
         "Stat": str,
```

### Comparing `mypy-boto3-cloudwatch-1.28.15.post1/mypy_boto3_cloudwatch/waiter.py` & `mypy-boto3-cloudwatch-1.28.16/mypy_boto3_cloudwatch/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudwatch-1.28.15.post1/mypy_boto3_cloudwatch/waiter.pyi` & `mypy-boto3-cloudwatch-1.28.16/mypy_boto3_cloudwatch/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudwatch-1.28.15.post1/mypy_boto3_cloudwatch.egg-info/PKG-INFO` & `mypy-boto3-cloudwatch-1.28.16/mypy_boto3_cloudwatch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cloudwatch
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.CloudWatch 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.CloudWatch 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 cloudwatch type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 cloudwatch type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudwatch.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudwatch)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cloudwatch)](https://pepy.tech/project/mypy-boto3-cloudwatch)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudWatch 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch)
+[boto3.CloudWatch 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch)
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
 [mypy-boto3-cloudwatch docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch/).
 
 See how it helps to find and fix potential bugs:
 
@@ -78,15 +78,15 @@
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Waiters annotations](#waiters-annotations)
     - [Service Resource annotations](#service-resource-annotations)
     - [Other resources annotations](#other-resources-annotations)
     - [Collections annotations](#collections-annotations)
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
@@ -436,51 +436,48 @@
 )
 
 
 def check_value(value: ActionsSuppressedByType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_cloudwatch.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_cloudwatch.type_defs import (
     AlarmHistoryItemTypeDef,
     RangeOutputTypeDef,
-    RangeTypeDef,
     DimensionTypeDef,
     CompositeAlarmTypeDef,
     DashboardEntryTypeDef,
     DashboardValidationMessageTypeDef,
     DatapointTypeDef,
     DeleteAlarmsInputRequestTypeDef,
     DeleteDashboardsInputRequestTypeDef,
     DeleteInsightRulesInputRequestTypeDef,
     PartialFailureTypeDef,
     ResponseMetadataTypeDef,
     DeleteMetricStreamInputRequestTypeDef,
-    DescribeAlarmHistoryInputAlarmDescribeHistoryTypeDef,
+    TimestampTypeDef,
     PaginatorConfigTypeDef,
-    DescribeAlarmHistoryInputRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeAlarmsInputRequestTypeDef,
     DescribeInsightRulesInputRequestTypeDef,
     InsightRuleTypeDef,
     DimensionFilterTypeDef,
     DisableAlarmActionsInputRequestTypeDef,
     DisableInsightRulesInputRequestTypeDef,
     EnableAlarmActionsInputRequestTypeDef,
     EnableInsightRulesInputRequestTypeDef,
     GetDashboardInputRequestTypeDef,
-    GetInsightRuleReportInputRequestTypeDef,
     InsightRuleMetricDatapointTypeDef,
     LabelOptionsTypeDef,
     MessageDataTypeDef,
     GetMetricStreamInputRequestTypeDef,
     MetricStreamFilterOutputTypeDef,
     GetMetricWidgetImageInputRequestTypeDef,
     InsightRuleContributorDatapointTypeDef,
@@ -497,19 +494,16 @@
     PutDashboardInputRequestTypeDef,
     SetAlarmStateInputAlarmSetStateTypeDef,
     SetAlarmStateInputRequestTypeDef,
     StartMetricStreamsInputRequestTypeDef,
     StopMetricStreamsInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     AnomalyDetectorConfigurationOutputTypeDef,
-    AnomalyDetectorConfigurationTypeDef,
     DescribeAlarmsForMetricInputRequestTypeDef,
     DescribeAnomalyDetectorsInputRequestTypeDef,
-    GetMetricStatisticsInputMetricGetStatisticsTypeDef,
-    GetMetricStatisticsInputRequestTypeDef,
     MetricOutputTypeDef,
     MetricTypeDef,
     SingleMetricAnomalyDetectorOutputTypeDef,
     SingleMetricAnomalyDetectorTypeDef,
     DeleteInsightRulesOutputTypeDef,
     DescribeAlarmHistoryOutputTypeDef,
     DisableInsightRulesOutputTypeDef,
@@ -518,14 +512,20 @@
     GetDashboardOutputTypeDef,
     GetMetricStatisticsOutputTypeDef,
     GetMetricWidgetImageOutputTypeDef,
     ListDashboardsOutputTypeDef,
     PutDashboardOutputTypeDef,
     PutManagedInsightRulesOutputTypeDef,
     PutMetricStreamOutputTypeDef,
+    DescribeAlarmHistoryInputAlarmDescribeHistoryTypeDef,
+    DescribeAlarmHistoryInputRequestTypeDef,
+    GetInsightRuleReportInputRequestTypeDef,
+    GetMetricStatisticsInputMetricGetStatisticsTypeDef,
+    GetMetricStatisticsInputRequestTypeDef,
+    RangeTypeDef,
     DescribeAlarmHistoryInputDescribeAlarmHistoryPaginateTypeDef,
     DescribeAlarmsInputDescribeAlarmsPaginateTypeDef,
     DescribeAnomalyDetectorsInputDescribeAnomalyDetectorsPaginateTypeDef,
     ListDashboardsInputListDashboardsPaginateTypeDef,
     DescribeAlarmsInputAlarmExistsWaitTypeDef,
     DescribeAlarmsInputCompositeAlarmExistsWaitTypeDef,
     DescribeInsightRulesOutputTypeDef,
@@ -537,45 +537,52 @@
     ListTagsForResourceOutputTypeDef,
     ManagedRuleTypeDef,
     PutCompositeAlarmInputRequestTypeDef,
     PutInsightRuleInputRequestTypeDef,
     TagResourceInputRequestTypeDef,
     ManagedRuleDescriptionTypeDef,
     MetricDatumTypeDef,
+    MetricStreamFilterUnionTypeDef,
     MetricStreamStatisticsConfigurationOutputTypeDef,
     MetricStreamStatisticsConfigurationTypeDef,
     ListMetricsOutputTypeDef,
     MetricStatOutputTypeDef,
     MetricStatTypeDef,
+    SingleMetricAnomalyDetectorUnionTypeDef,
+    AnomalyDetectorConfigurationTypeDef,
     GetMetricDataOutputTypeDef,
     GetInsightRuleReportOutputTypeDef,
     PutManagedInsightRulesInputRequestTypeDef,
     ListManagedInsightRulesOutputTypeDef,
     PutMetricDataInputRequestTypeDef,
     GetMetricStreamOutputTypeDef,
-    PutMetricStreamInputRequestTypeDef,
+    MetricStreamStatisticsConfigurationUnionTypeDef,
     MetricDataQueryOutputTypeDef,
     MetricDataQueryTypeDef,
+    AnomalyDetectorConfigurationUnionTypeDef,
+    PutMetricStreamInputRequestTypeDef,
     MetricAlarmTypeDef,
     MetricMathAnomalyDetectorOutputTypeDef,
-    GetMetricDataInputGetMetricDataPaginateTypeDef,
-    GetMetricDataInputRequestTypeDef,
+    MetricDataQueryUnionTypeDef,
     MetricMathAnomalyDetectorTypeDef,
     PutMetricAlarmInputMetricPutAlarmTypeDef,
-    PutMetricAlarmInputRequestTypeDef,
     DescribeAlarmsForMetricOutputTypeDef,
     DescribeAlarmsOutputTypeDef,
     AnomalyDetectorTypeDef,
+    GetMetricDataInputGetMetricDataPaginateTypeDef,
+    GetMetricDataInputRequestTypeDef,
+    PutMetricAlarmInputRequestTypeDef,
     DeleteAnomalyDetectorInputRequestTypeDef,
+    MetricMathAnomalyDetectorUnionTypeDef,
     PutAnomalyDetectorInputRequestTypeDef,
     DescribeAnomalyDetectorsOutputTypeDef,
 )
 
 
-def get_structure() -> AlarmHistoryItemTypeDef:
+def get_value() -> AlarmHistoryItemTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-cloudwatch-1.28.15.post1/mypy_boto3_cloudwatch.egg-info/SOURCES.txt` & `mypy-boto3-cloudwatch-1.28.16/mypy_boto3_cloudwatch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudwatch-1.28.15.post1/setup.py` & `mypy-boto3-cloudwatch-1.28.16/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-cloudwatch",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_cloudwatch"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CloudWatch 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.2"
+        "Type annotations for boto3.CloudWatch 1.28.16 service generated with mypy-boto3-builder"
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
-    keywords="boto3 cloudwatch type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 cloudwatch type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_cloudwatch": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

