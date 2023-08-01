# Comparing `tmp/mypy-boto3-lookoutmetrics-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-lookoutmetrics-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-lookoutmetrics-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:34 2023, max compression
+gzip compressed data, was "mypy-boto3-lookoutmetrics-1.28.16.tar", last modified: Tue Aug  1 11:37:14 2023, max compression
```

## Comparing `mypy-boto3-lookoutmetrics-1.28.15.post1.tar` & `mypy-boto3-lookoutmetrics-1.28.16.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:34.025253 mypy-boto3-lookoutmetrics-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:50:12.000000 mypy-boto3-lookoutmetrics-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16902 2023-07-29 10:03:34.017253 mypy-boto3-lookoutmetrics-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15381 2023-07-29 09:50:12.000000 mypy-boto3-lookoutmetrics-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:34.009253 mypy-boto3-lookoutmetrics-1.28.15.post1/mypy_boto3_lookoutmetrics/
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-29 09:50:12.000000 mypy-boto3-lookoutmetrics-1.28.15.post1/mypy_boto3_lookoutmetrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-29 09:50:12.000000 mypy-boto3-lookoutmetrics-1.28.15.post1/mypy_boto3_lookoutmetrics/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-29 09:50:12.000000 mypy-boto3-lookoutmetrics-1.28.15.post1/mypy_boto3_lookoutmetrics/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22942 2023-07-29 09:50:12.000000 mypy-boto3-lookoutmetrics-1.28.15.post1/mypy_boto3_lookoutmetrics/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    22906 2023-07-29 09:50:12.000000 mypy-boto3-lookoutmetrics-1.28.15.post1/mypy_boto3_lookoutmetrics/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9691 2023-07-29 09:50:13.000000 mypy-boto3-lookoutmetrics-1.28.15.post1/mypy_boto3_lookoutmetrics/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-07-29 09:50:12.000000 mypy-boto3-lookoutmetrics-1.28.15.post1/mypy_boto3_lookoutmetrics/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:50:12.000000 mypy-boto3-lookoutmetrics-1.28.15.post1/mypy_boto3_lookoutmetrics/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    39841 2023-07-29 09:50:14.000000 mypy-boto3-lookoutmetrics-1.28.15.post1/mypy_boto3_lookoutmetrics/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    39808 2023-07-29 09:50:13.000000 mypy-boto3-lookoutmetrics-1.28.15.post1/mypy_boto3_lookoutmetrics/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:50:12.000000 mypy-boto3-lookoutmetrics-1.28.15.post1/mypy_boto3_lookoutmetrics/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:34.017253 mypy-boto3-lookoutmetrics-1.28.15.post1/mypy_boto3_lookoutmetrics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16902 2023-07-29 10:03:33.000000 mypy-boto3-lookoutmetrics-1.28.15.post1/mypy_boto3_lookoutmetrics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-29 10:03:33.000000 mypy-boto3-lookoutmetrics-1.28.15.post1/mypy_boto3_lookoutmetrics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:33.000000 mypy-boto3-lookoutmetrics-1.28.15.post1/mypy_boto3_lookoutmetrics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:33.000000 mypy-boto3-lookoutmetrics-1.28.15.post1/mypy_boto3_lookoutmetrics.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:33.000000 mypy-boto3-lookoutmetrics-1.28.15.post1/mypy_boto3_lookoutmetrics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-29 10:03:33.000000 mypy-boto3-lookoutmetrics-1.28.15.post1/mypy_boto3_lookoutmetrics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:34.025253 mypy-boto3-lookoutmetrics-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-07-29 09:50:12.000000 mypy-boto3-lookoutmetrics-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:13.988836 mypy-boto3-lookoutmetrics-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:23:03.000000 mypy-boto3-lookoutmetrics-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16994 2023-08-01 11:37:13.980836 mypy-boto3-lookoutmetrics-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15482 2023-08-01 11:23:03.000000 mypy-boto3-lookoutmetrics-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:13.976836 mypy-boto3-lookoutmetrics-1.28.16/mypy_boto3_lookoutmetrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-08-01 11:23:03.000000 mypy-boto3-lookoutmetrics-1.28.16/mypy_boto3_lookoutmetrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-08-01 11:23:03.000000 mypy-boto3-lookoutmetrics-1.28.16/mypy_boto3_lookoutmetrics/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-08-01 11:23:03.000000 mypy-boto3-lookoutmetrics-1.28.16/mypy_boto3_lookoutmetrics/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22603 2023-08-01 11:23:04.000000 mypy-boto3-lookoutmetrics-1.28.16/mypy_boto3_lookoutmetrics/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22567 2023-08-01 11:23:04.000000 mypy-boto3-lookoutmetrics-1.28.16/mypy_boto3_lookoutmetrics/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9691 2023-08-01 11:23:04.000000 mypy-boto3-lookoutmetrics-1.28.16/mypy_boto3_lookoutmetrics/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-08-01 11:23:04.000000 mypy-boto3-lookoutmetrics-1.28.16/mypy_boto3_lookoutmetrics/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:23:03.000000 mypy-boto3-lookoutmetrics-1.28.16/mypy_boto3_lookoutmetrics/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    40106 2023-08-01 11:23:05.000000 mypy-boto3-lookoutmetrics-1.28.16/mypy_boto3_lookoutmetrics/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40073 2023-08-01 11:23:04.000000 mypy-boto3-lookoutmetrics-1.28.16/mypy_boto3_lookoutmetrics/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:23:03.000000 mypy-boto3-lookoutmetrics-1.28.16/mypy_boto3_lookoutmetrics/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:13.980836 mypy-boto3-lookoutmetrics-1.28.16/mypy_boto3_lookoutmetrics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16994 2023-08-01 11:37:13.000000 mypy-boto3-lookoutmetrics-1.28.16/mypy_boto3_lookoutmetrics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-08-01 11:37:13.000000 mypy-boto3-lookoutmetrics-1.28.16/mypy_boto3_lookoutmetrics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:13.000000 mypy-boto3-lookoutmetrics-1.28.16/mypy_boto3_lookoutmetrics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:13.000000 mypy-boto3-lookoutmetrics-1.28.16/mypy_boto3_lookoutmetrics.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:13.000000 mypy-boto3-lookoutmetrics-1.28.16/mypy_boto3_lookoutmetrics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-01 11:37:13.000000 mypy-boto3-lookoutmetrics-1.28.16/mypy_boto3_lookoutmetrics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:13.988836 mypy-boto3-lookoutmetrics-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-08-01 11:23:03.000000 mypy-boto3-lookoutmetrics-1.28.16/setup.py
```

### Comparing `mypy-boto3-lookoutmetrics-1.28.15.post1/LICENSE` & `mypy-boto3-lookoutmetrics-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lookoutmetrics-1.28.15.post1/PKG-INFO` & `mypy-boto3-lookoutmetrics-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-lookoutmetrics
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.LookoutMetrics 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.LookoutMetrics 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutmetrics/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 lookoutmetrics type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 lookoutmetrics type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lookoutmetrics.svg?color=blue)](https://pypi.org/project/mypy-boto3-lookoutmetrics)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutmetrics/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-lookoutmetrics)](https://pepy.tech/project/mypy-boto3-lookoutmetrics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LookoutMetrics 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics)
+[boto3.LookoutMetrics 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics)
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
 [mypy-boto3-lookoutmetrics docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutmetrics/).
 
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
@@ -302,20 +302,20 @@
 )
 
 
 def check_value(value: AggregationFunctionType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_lookoutmetrics.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_lookoutmetrics.type_defs import (
     LambdaConfigurationTypeDef,
     SNSConfigurationTypeDef,
     ActivateAnomalyDetectorRequestRequestTypeDef,
     DimensionFilterOutputTypeDef,
@@ -402,46 +402,49 @@
     ListAnomalyGroupRelatedMetricsResponseTypeDef,
     ListMetricSetsResponseTypeDef,
     RDSSourceConfigOutputTypeDef,
     RedshiftSourceConfigOutputTypeDef,
     RDSSourceConfigTypeDef,
     RedshiftSourceConfigTypeDef,
     AlertTypeDef,
+    AlertFiltersUnionTypeDef,
     CreateAlertRequestRequestTypeDef,
     UpdateAlertRequestRequestTypeDef,
     ListAnomalyGroupSummariesResponseTypeDef,
     DetectedCsvFormatDescriptorTypeDef,
     DetectedJsonFormatDescriptorTypeDef,
     DetectMetricSetConfigRequestRequestTypeDef,
     AnomalyDetectorDataQualityMetricTypeDef,
     ContributionMatrixTypeDef,
     ListAnomalyGroupTimeSeriesResponseTypeDef,
     S3SourceConfigOutputTypeDef,
     S3SourceConfigTypeDef,
     SampleDataS3SourceConfigTypeDef,
+    MetricSetDimensionFilterUnionTypeDef,
     DescribeAlertResponseTypeDef,
     DetectedFileFormatDescriptorTypeDef,
     GetDataQualityMetricsResponseTypeDef,
     MetricLevelImpactTypeDef,
     MetricSourceOutputTypeDef,
     MetricSourceTypeDef,
     GetSampleDataRequestRequestTypeDef,
     DetectedS3SourceConfigTypeDef,
     AnomalyGroupTypeDef,
     DescribeMetricSetResponseTypeDef,
     CreateMetricSetRequestRequestTypeDef,
+    MetricSourceUnionTypeDef,
     UpdateMetricSetRequestRequestTypeDef,
     DetectedMetricSourceTypeDef,
     GetAnomalyGroupResponseTypeDef,
     DetectedMetricSetConfigTypeDef,
     DetectMetricSetConfigResponseTypeDef,
 )
 
 
-def get_structure() -> LambdaConfigurationTypeDef:
+def get_value() -> LambdaConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-lookoutmetrics-1.28.15.post1/README.md` & `mypy-boto3-lookoutmetrics-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lookoutmetrics.svg?color=blue)](https://pypi.org/project/mypy-boto3-lookoutmetrics)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutmetrics/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-lookoutmetrics)](https://pepy.tech/project/mypy-boto3-lookoutmetrics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LookoutMetrics 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics)
+[boto3.LookoutMetrics 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics)
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
 [mypy-boto3-lookoutmetrics docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutmetrics/).
 
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
@@ -270,20 +270,20 @@
 )
 
 
 def check_value(value: AggregationFunctionType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_lookoutmetrics.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_lookoutmetrics.type_defs import (
     LambdaConfigurationTypeDef,
     SNSConfigurationTypeDef,
     ActivateAnomalyDetectorRequestRequestTypeDef,
     DimensionFilterOutputTypeDef,
@@ -370,46 +370,49 @@
     ListAnomalyGroupRelatedMetricsResponseTypeDef,
     ListMetricSetsResponseTypeDef,
     RDSSourceConfigOutputTypeDef,
     RedshiftSourceConfigOutputTypeDef,
     RDSSourceConfigTypeDef,
     RedshiftSourceConfigTypeDef,
     AlertTypeDef,
+    AlertFiltersUnionTypeDef,
     CreateAlertRequestRequestTypeDef,
     UpdateAlertRequestRequestTypeDef,
     ListAnomalyGroupSummariesResponseTypeDef,
     DetectedCsvFormatDescriptorTypeDef,
     DetectedJsonFormatDescriptorTypeDef,
     DetectMetricSetConfigRequestRequestTypeDef,
     AnomalyDetectorDataQualityMetricTypeDef,
     ContributionMatrixTypeDef,
     ListAnomalyGroupTimeSeriesResponseTypeDef,
     S3SourceConfigOutputTypeDef,
     S3SourceConfigTypeDef,
     SampleDataS3SourceConfigTypeDef,
+    MetricSetDimensionFilterUnionTypeDef,
     DescribeAlertResponseTypeDef,
     DetectedFileFormatDescriptorTypeDef,
     GetDataQualityMetricsResponseTypeDef,
     MetricLevelImpactTypeDef,
     MetricSourceOutputTypeDef,
     MetricSourceTypeDef,
     GetSampleDataRequestRequestTypeDef,
     DetectedS3SourceConfigTypeDef,
     AnomalyGroupTypeDef,
     DescribeMetricSetResponseTypeDef,
     CreateMetricSetRequestRequestTypeDef,
+    MetricSourceUnionTypeDef,
     UpdateMetricSetRequestRequestTypeDef,
     DetectedMetricSourceTypeDef,
     GetAnomalyGroupResponseTypeDef,
     DetectedMetricSetConfigTypeDef,
     DetectMetricSetConfigResponseTypeDef,
 )
 
 
-def get_structure() -> LambdaConfigurationTypeDef:
+def get_value() -> LambdaConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-lookoutmetrics-1.28.15.post1/mypy_boto3_lookoutmetrics/__main__.py` & `mypy-boto3-lookoutmetrics-1.28.16/mypy_boto3_lookoutmetrics/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.LookoutMetrics 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.LookoutMetrics 1.28.16\nVersion:         1.28.16\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutmetrics//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics\nOther"
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

### Comparing `mypy-boto3-lookoutmetrics-1.28.15.post1/mypy_boto3_lookoutmetrics/client.py` & `mypy-boto3-lookoutmetrics-1.28.16/mypy_boto3_lookoutmetrics/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,23 +9,22 @@
     from boto3.session import Session
     from mypy_boto3_lookoutmetrics.client import LookoutMetricsClient
 
     session = Session()
     client: LookoutMetricsClient = session.client("lookoutmetrics")
     ```
 """
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import FrequencyType, RelationshipTypeType
 from .type_defs import (
     ActionTypeDef,
-    AlertFiltersOutputTypeDef,
-    AlertFiltersTypeDef,
+    AlertFiltersUnionTypeDef,
     AnomalyDetectorConfigTypeDef,
     AnomalyGroupTimeSeriesFeedbackTypeDef,
     AnomalyGroupTimeSeriesTypeDef,
     AutoDetectionMetricSourceTypeDef,
     CreateAlertResponseTypeDef,
     CreateAnomalyDetectorResponseTypeDef,
     CreateMetricSetResponseTypeDef,
@@ -41,18 +40,16 @@
     ListAlertsResponseTypeDef,
     ListAnomalyDetectorsResponseTypeDef,
     ListAnomalyGroupRelatedMetricsResponseTypeDef,
     ListAnomalyGroupSummariesResponseTypeDef,
     ListAnomalyGroupTimeSeriesResponseTypeDef,
     ListMetricSetsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    MetricSetDimensionFilterOutputTypeDef,
-    MetricSetDimensionFilterTypeDef,
-    MetricSourceOutputTypeDef,
-    MetricSourceTypeDef,
+    MetricSetDimensionFilterUnionTypeDef,
+    MetricSourceUnionTypeDef,
     MetricTypeDef,
     SampleDataS3SourceConfigTypeDef,
     TimestampColumnTypeDef,
     UpdateAlertResponseTypeDef,
     UpdateAnomalyDetectorResponseTypeDef,
     UpdateMetricSetResponseTypeDef,
 )
@@ -133,15 +130,15 @@
         *,
         AlertName: str,
         AnomalyDetectorArn: str,
         Action: ActionTypeDef,
         AlertSensitivityThreshold: int = ...,
         AlertDescription: str = ...,
         Tags: Mapping[str, str] = ...,
-        AlertFilters: Union[AlertFiltersTypeDef, AlertFiltersOutputTypeDef] = ...
+        AlertFilters: AlertFiltersUnionTypeDef = ...
     ) -> CreateAlertResponseTypeDef:
         """
         Creates an alert for an anomaly detector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics.Client.create_alert)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutmetrics/client/#create_alert)
         """
@@ -164,25 +161,23 @@
 
     def create_metric_set(
         self,
         *,
         AnomalyDetectorArn: str,
         MetricSetName: str,
         MetricList: Sequence[MetricTypeDef],
-        MetricSource: Union[MetricSourceTypeDef, MetricSourceOutputTypeDef],
+        MetricSource: MetricSourceUnionTypeDef,
         MetricSetDescription: str = ...,
         Offset: int = ...,
         TimestampColumn: TimestampColumnTypeDef = ...,
         DimensionList: Sequence[str] = ...,
         MetricSetFrequency: FrequencyType = ...,
         Timezone: str = ...,
         Tags: Mapping[str, str] = ...,
-        DimensionFilterList: Sequence[
-            Union[MetricSetDimensionFilterTypeDef, MetricSetDimensionFilterOutputTypeDef]
-        ] = ...
+        DimensionFilterList: Sequence[MetricSetDimensionFilterUnionTypeDef] = ...
     ) -> CreateMetricSetResponseTypeDef:
         """
         Creates a dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics.Client.create_metric_set)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutmetrics/client/#create_metric_set)
         """
@@ -446,15 +441,15 @@
     def update_alert(
         self,
         *,
         AlertArn: str,
         AlertDescription: str = ...,
         AlertSensitivityThreshold: int = ...,
         Action: ActionTypeDef = ...,
-        AlertFilters: Union[AlertFiltersTypeDef, AlertFiltersOutputTypeDef] = ...
+        AlertFilters: AlertFiltersUnionTypeDef = ...
     ) -> UpdateAlertResponseTypeDef:
         """
         Make changes to an existing alert.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics.Client.update_alert)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutmetrics/client/#update_alert)
         """
@@ -480,18 +475,16 @@
         MetricSetArn: str,
         MetricSetDescription: str = ...,
         MetricList: Sequence[MetricTypeDef] = ...,
         Offset: int = ...,
         TimestampColumn: TimestampColumnTypeDef = ...,
         DimensionList: Sequence[str] = ...,
         MetricSetFrequency: FrequencyType = ...,
-        MetricSource: Union[MetricSourceTypeDef, MetricSourceOutputTypeDef] = ...,
-        DimensionFilterList: Sequence[
-            Union[MetricSetDimensionFilterTypeDef, MetricSetDimensionFilterOutputTypeDef]
-        ] = ...
+        MetricSource: MetricSourceUnionTypeDef = ...,
+        DimensionFilterList: Sequence[MetricSetDimensionFilterUnionTypeDef] = ...
     ) -> UpdateMetricSetResponseTypeDef:
         """
         Updates a dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics.Client.update_metric_set)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutmetrics/client/#update_metric_set)
         """
```

### Comparing `mypy-boto3-lookoutmetrics-1.28.15.post1/mypy_boto3_lookoutmetrics/client.pyi` & `mypy-boto3-lookoutmetrics-1.28.16/mypy_boto3_lookoutmetrics/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -9,23 +9,22 @@
     from boto3.session import Session
     from mypy_boto3_lookoutmetrics.client import LookoutMetricsClient
 
     session = Session()
     client: LookoutMetricsClient = session.client("lookoutmetrics")
     ```
 """
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import FrequencyType, RelationshipTypeType
 from .type_defs import (
     ActionTypeDef,
-    AlertFiltersOutputTypeDef,
-    AlertFiltersTypeDef,
+    AlertFiltersUnionTypeDef,
     AnomalyDetectorConfigTypeDef,
     AnomalyGroupTimeSeriesFeedbackTypeDef,
     AnomalyGroupTimeSeriesTypeDef,
     AutoDetectionMetricSourceTypeDef,
     CreateAlertResponseTypeDef,
     CreateAnomalyDetectorResponseTypeDef,
     CreateMetricSetResponseTypeDef,
@@ -41,18 +40,16 @@
     ListAlertsResponseTypeDef,
     ListAnomalyDetectorsResponseTypeDef,
     ListAnomalyGroupRelatedMetricsResponseTypeDef,
     ListAnomalyGroupSummariesResponseTypeDef,
     ListAnomalyGroupTimeSeriesResponseTypeDef,
     ListMetricSetsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    MetricSetDimensionFilterOutputTypeDef,
-    MetricSetDimensionFilterTypeDef,
-    MetricSourceOutputTypeDef,
-    MetricSourceTypeDef,
+    MetricSetDimensionFilterUnionTypeDef,
+    MetricSourceUnionTypeDef,
     MetricTypeDef,
     SampleDataS3SourceConfigTypeDef,
     TimestampColumnTypeDef,
     UpdateAlertResponseTypeDef,
     UpdateAnomalyDetectorResponseTypeDef,
     UpdateMetricSetResponseTypeDef,
 )
@@ -125,15 +122,15 @@
         *,
         AlertName: str,
         AnomalyDetectorArn: str,
         Action: ActionTypeDef,
         AlertSensitivityThreshold: int = ...,
         AlertDescription: str = ...,
         Tags: Mapping[str, str] = ...,
-        AlertFilters: Union[AlertFiltersTypeDef, AlertFiltersOutputTypeDef] = ...
+        AlertFilters: AlertFiltersUnionTypeDef = ...
     ) -> CreateAlertResponseTypeDef:
         """
         Creates an alert for an anomaly detector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics.Client.create_alert)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutmetrics/client/#create_alert)
         """
@@ -154,25 +151,23 @@
         """
     def create_metric_set(
         self,
         *,
         AnomalyDetectorArn: str,
         MetricSetName: str,
         MetricList: Sequence[MetricTypeDef],
-        MetricSource: Union[MetricSourceTypeDef, MetricSourceOutputTypeDef],
+        MetricSource: MetricSourceUnionTypeDef,
         MetricSetDescription: str = ...,
         Offset: int = ...,
         TimestampColumn: TimestampColumnTypeDef = ...,
         DimensionList: Sequence[str] = ...,
         MetricSetFrequency: FrequencyType = ...,
         Timezone: str = ...,
         Tags: Mapping[str, str] = ...,
-        DimensionFilterList: Sequence[
-            Union[MetricSetDimensionFilterTypeDef, MetricSetDimensionFilterOutputTypeDef]
-        ] = ...
+        DimensionFilterList: Sequence[MetricSetDimensionFilterUnionTypeDef] = ...
     ) -> CreateMetricSetResponseTypeDef:
         """
         Creates a dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics.Client.create_metric_set)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutmetrics/client/#create_metric_set)
         """
@@ -412,15 +407,15 @@
     def update_alert(
         self,
         *,
         AlertArn: str,
         AlertDescription: str = ...,
         AlertSensitivityThreshold: int = ...,
         Action: ActionTypeDef = ...,
-        AlertFilters: Union[AlertFiltersTypeDef, AlertFiltersOutputTypeDef] = ...
+        AlertFilters: AlertFiltersUnionTypeDef = ...
     ) -> UpdateAlertResponseTypeDef:
         """
         Make changes to an existing alert.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics.Client.update_alert)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutmetrics/client/#update_alert)
         """
@@ -444,18 +439,16 @@
         MetricSetArn: str,
         MetricSetDescription: str = ...,
         MetricList: Sequence[MetricTypeDef] = ...,
         Offset: int = ...,
         TimestampColumn: TimestampColumnTypeDef = ...,
         DimensionList: Sequence[str] = ...,
         MetricSetFrequency: FrequencyType = ...,
-        MetricSource: Union[MetricSourceTypeDef, MetricSourceOutputTypeDef] = ...,
-        DimensionFilterList: Sequence[
-            Union[MetricSetDimensionFilterTypeDef, MetricSetDimensionFilterOutputTypeDef]
-        ] = ...
+        MetricSource: MetricSourceUnionTypeDef = ...,
+        DimensionFilterList: Sequence[MetricSetDimensionFilterUnionTypeDef] = ...
     ) -> UpdateMetricSetResponseTypeDef:
         """
         Updates a dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics.Client.update_metric_set)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutmetrics/client/#update_metric_set)
         """
```

### Comparing `mypy-boto3-lookoutmetrics-1.28.15.post1/mypy_boto3_lookoutmetrics/literals.py` & `mypy-boto3-lookoutmetrics-1.28.16/mypy_boto3_lookoutmetrics/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lookoutmetrics-1.28.15.post1/mypy_boto3_lookoutmetrics/literals.pyi` & `mypy-boto3-lookoutmetrics-1.28.16/mypy_boto3_lookoutmetrics/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lookoutmetrics-1.28.15.post1/mypy_boto3_lookoutmetrics/type_defs.py` & `mypy-boto3-lookoutmetrics-1.28.16/mypy_boto3_lookoutmetrics/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutmetrics/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_lookoutmetrics.type_defs import LambdaConfigurationTypeDef
 
-    data: LambdaConfigurationTypeDef = {...}
+    data: LambdaConfigurationTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -129,37 +129,40 @@
     "ListAnomalyGroupRelatedMetricsResponseTypeDef",
     "ListMetricSetsResponseTypeDef",
     "RDSSourceConfigOutputTypeDef",
     "RedshiftSourceConfigOutputTypeDef",
     "RDSSourceConfigTypeDef",
     "RedshiftSourceConfigTypeDef",
     "AlertTypeDef",
+    "AlertFiltersUnionTypeDef",
     "CreateAlertRequestRequestTypeDef",
     "UpdateAlertRequestRequestTypeDef",
     "ListAnomalyGroupSummariesResponseTypeDef",
     "DetectedCsvFormatDescriptorTypeDef",
     "DetectedJsonFormatDescriptorTypeDef",
     "DetectMetricSetConfigRequestRequestTypeDef",
     "AnomalyDetectorDataQualityMetricTypeDef",
     "ContributionMatrixTypeDef",
     "ListAnomalyGroupTimeSeriesResponseTypeDef",
     "S3SourceConfigOutputTypeDef",
     "S3SourceConfigTypeDef",
     "SampleDataS3SourceConfigTypeDef",
+    "MetricSetDimensionFilterUnionTypeDef",
     "DescribeAlertResponseTypeDef",
     "DetectedFileFormatDescriptorTypeDef",
     "GetDataQualityMetricsResponseTypeDef",
     "MetricLevelImpactTypeDef",
     "MetricSourceOutputTypeDef",
     "MetricSourceTypeDef",
     "GetSampleDataRequestRequestTypeDef",
     "DetectedS3SourceConfigTypeDef",
     "AnomalyGroupTypeDef",
     "DescribeMetricSetResponseTypeDef",
     "CreateMetricSetRequestRequestTypeDef",
+    "MetricSourceUnionTypeDef",
     "UpdateMetricSetRequestRequestTypeDef",
     "DetectedMetricSourceTypeDef",
     "GetAnomalyGroupResponseTypeDef",
     "DetectedMetricSetConfigTypeDef",
     "DetectMetricSetConfigResponseTypeDef",
 )
 
@@ -1183,14 +1186,15 @@
         "LastModificationTime": datetime,
         "CreationTime": datetime,
         "AlertFilters": AlertFiltersOutputTypeDef,
     },
     total=False,
 )
 
+AlertFiltersUnionTypeDef = Union[AlertFiltersTypeDef, AlertFiltersOutputTypeDef]
 _RequiredCreateAlertRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAlertRequestRequestTypeDef",
     {
         "AlertName": str,
         "AnomalyDetectorArn": str,
         "Action": ActionTypeDef,
     },
@@ -1347,14 +1351,17 @@
 
 class SampleDataS3SourceConfigTypeDef(
     _RequiredSampleDataS3SourceConfigTypeDef, _OptionalSampleDataS3SourceConfigTypeDef
 ):
     pass
 
 
+MetricSetDimensionFilterUnionTypeDef = Union[
+    MetricSetDimensionFilterTypeDef, MetricSetDimensionFilterOutputTypeDef
+]
 DescribeAlertResponseTypeDef = TypedDict(
     "DescribeAlertResponseTypeDef",
     {
         "Alert": AlertTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1477,28 +1484,27 @@
         "MetricSetDescription": str,
         "Offset": int,
         "TimestampColumn": TimestampColumnTypeDef,
         "DimensionList": Sequence[str],
         "MetricSetFrequency": FrequencyType,
         "Timezone": str,
         "Tags": Mapping[str, str],
-        "DimensionFilterList": Sequence[
-            Union[MetricSetDimensionFilterTypeDef, MetricSetDimensionFilterOutputTypeDef]
-        ],
+        "DimensionFilterList": Sequence[MetricSetDimensionFilterUnionTypeDef],
     },
     total=False,
 )
 
 
 class CreateMetricSetRequestRequestTypeDef(
     _RequiredCreateMetricSetRequestRequestTypeDef, _OptionalCreateMetricSetRequestRequestTypeDef
 ):
     pass
 
 
+MetricSourceUnionTypeDef = Union[MetricSourceTypeDef, MetricSourceOutputTypeDef]
 _RequiredUpdateMetricSetRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateMetricSetRequestRequestTypeDef",
     {
         "MetricSetArn": str,
     },
 )
 _OptionalUpdateMetricSetRequestRequestTypeDef = TypedDict(
@@ -1507,17 +1513,15 @@
         "MetricSetDescription": str,
         "MetricList": Sequence[MetricTypeDef],
         "Offset": int,
         "TimestampColumn": TimestampColumnTypeDef,
         "DimensionList": Sequence[str],
         "MetricSetFrequency": FrequencyType,
         "MetricSource": MetricSourceTypeDef,
-        "DimensionFilterList": Sequence[
-            Union[MetricSetDimensionFilterTypeDef, MetricSetDimensionFilterOutputTypeDef]
-        ],
+        "DimensionFilterList": Sequence[MetricSetDimensionFilterUnionTypeDef],
     },
     total=False,
 )
 
 
 class UpdateMetricSetRequestRequestTypeDef(
     _RequiredUpdateMetricSetRequestRequestTypeDef, _OptionalUpdateMetricSetRequestRequestTypeDef
```

### Comparing `mypy-boto3-lookoutmetrics-1.28.15.post1/mypy_boto3_lookoutmetrics/type_defs.pyi` & `mypy-boto3-lookoutmetrics-1.28.16/mypy_boto3_lookoutmetrics/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutmetrics/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_lookoutmetrics.type_defs import LambdaConfigurationTypeDef
 
-    data: LambdaConfigurationTypeDef = {...}
+    data: LambdaConfigurationTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -128,37 +128,40 @@
     "ListAnomalyGroupRelatedMetricsResponseTypeDef",
     "ListMetricSetsResponseTypeDef",
     "RDSSourceConfigOutputTypeDef",
     "RedshiftSourceConfigOutputTypeDef",
     "RDSSourceConfigTypeDef",
     "RedshiftSourceConfigTypeDef",
     "AlertTypeDef",
+    "AlertFiltersUnionTypeDef",
     "CreateAlertRequestRequestTypeDef",
     "UpdateAlertRequestRequestTypeDef",
     "ListAnomalyGroupSummariesResponseTypeDef",
     "DetectedCsvFormatDescriptorTypeDef",
     "DetectedJsonFormatDescriptorTypeDef",
     "DetectMetricSetConfigRequestRequestTypeDef",
     "AnomalyDetectorDataQualityMetricTypeDef",
     "ContributionMatrixTypeDef",
     "ListAnomalyGroupTimeSeriesResponseTypeDef",
     "S3SourceConfigOutputTypeDef",
     "S3SourceConfigTypeDef",
     "SampleDataS3SourceConfigTypeDef",
+    "MetricSetDimensionFilterUnionTypeDef",
     "DescribeAlertResponseTypeDef",
     "DetectedFileFormatDescriptorTypeDef",
     "GetDataQualityMetricsResponseTypeDef",
     "MetricLevelImpactTypeDef",
     "MetricSourceOutputTypeDef",
     "MetricSourceTypeDef",
     "GetSampleDataRequestRequestTypeDef",
     "DetectedS3SourceConfigTypeDef",
     "AnomalyGroupTypeDef",
     "DescribeMetricSetResponseTypeDef",
     "CreateMetricSetRequestRequestTypeDef",
+    "MetricSourceUnionTypeDef",
     "UpdateMetricSetRequestRequestTypeDef",
     "DetectedMetricSourceTypeDef",
     "GetAnomalyGroupResponseTypeDef",
     "DetectedMetricSetConfigTypeDef",
     "DetectMetricSetConfigResponseTypeDef",
 )
 
@@ -1160,14 +1163,15 @@
         "LastModificationTime": datetime,
         "CreationTime": datetime,
         "AlertFilters": AlertFiltersOutputTypeDef,
     },
     total=False,
 )
 
+AlertFiltersUnionTypeDef = Union[AlertFiltersTypeDef, AlertFiltersOutputTypeDef]
 _RequiredCreateAlertRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAlertRequestRequestTypeDef",
     {
         "AlertName": str,
         "AnomalyDetectorArn": str,
         "Action": ActionTypeDef,
     },
@@ -1318,14 +1322,17 @@
 )
 
 class SampleDataS3SourceConfigTypeDef(
     _RequiredSampleDataS3SourceConfigTypeDef, _OptionalSampleDataS3SourceConfigTypeDef
 ):
     pass
 
+MetricSetDimensionFilterUnionTypeDef = Union[
+    MetricSetDimensionFilterTypeDef, MetricSetDimensionFilterOutputTypeDef
+]
 DescribeAlertResponseTypeDef = TypedDict(
     "DescribeAlertResponseTypeDef",
     {
         "Alert": AlertTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1448,26 +1455,25 @@
         "MetricSetDescription": str,
         "Offset": int,
         "TimestampColumn": TimestampColumnTypeDef,
         "DimensionList": Sequence[str],
         "MetricSetFrequency": FrequencyType,
         "Timezone": str,
         "Tags": Mapping[str, str],
-        "DimensionFilterList": Sequence[
-            Union[MetricSetDimensionFilterTypeDef, MetricSetDimensionFilterOutputTypeDef]
-        ],
+        "DimensionFilterList": Sequence[MetricSetDimensionFilterUnionTypeDef],
     },
     total=False,
 )
 
 class CreateMetricSetRequestRequestTypeDef(
     _RequiredCreateMetricSetRequestRequestTypeDef, _OptionalCreateMetricSetRequestRequestTypeDef
 ):
     pass
 
+MetricSourceUnionTypeDef = Union[MetricSourceTypeDef, MetricSourceOutputTypeDef]
 _RequiredUpdateMetricSetRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateMetricSetRequestRequestTypeDef",
     {
         "MetricSetArn": str,
     },
 )
 _OptionalUpdateMetricSetRequestRequestTypeDef = TypedDict(
@@ -1476,17 +1482,15 @@
         "MetricSetDescription": str,
         "MetricList": Sequence[MetricTypeDef],
         "Offset": int,
         "TimestampColumn": TimestampColumnTypeDef,
         "DimensionList": Sequence[str],
         "MetricSetFrequency": FrequencyType,
         "MetricSource": MetricSourceTypeDef,
-        "DimensionFilterList": Sequence[
-            Union[MetricSetDimensionFilterTypeDef, MetricSetDimensionFilterOutputTypeDef]
-        ],
+        "DimensionFilterList": Sequence[MetricSetDimensionFilterUnionTypeDef],
     },
     total=False,
 )
 
 class UpdateMetricSetRequestRequestTypeDef(
     _RequiredUpdateMetricSetRequestRequestTypeDef, _OptionalUpdateMetricSetRequestRequestTypeDef
 ):
```

### Comparing `mypy-boto3-lookoutmetrics-1.28.15.post1/mypy_boto3_lookoutmetrics.egg-info/PKG-INFO` & `mypy-boto3-lookoutmetrics-1.28.16/mypy_boto3_lookoutmetrics.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-lookoutmetrics
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.LookoutMetrics 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.LookoutMetrics 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutmetrics/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 lookoutmetrics type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 lookoutmetrics type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lookoutmetrics.svg?color=blue)](https://pypi.org/project/mypy-boto3-lookoutmetrics)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutmetrics/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-lookoutmetrics)](https://pepy.tech/project/mypy-boto3-lookoutmetrics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LookoutMetrics 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics)
+[boto3.LookoutMetrics 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics)
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
 [mypy-boto3-lookoutmetrics docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutmetrics/).
 
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
@@ -302,20 +302,20 @@
 )
 
 
 def check_value(value: AggregationFunctionType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_lookoutmetrics.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_lookoutmetrics.type_defs import (
     LambdaConfigurationTypeDef,
     SNSConfigurationTypeDef,
     ActivateAnomalyDetectorRequestRequestTypeDef,
     DimensionFilterOutputTypeDef,
@@ -402,46 +402,49 @@
     ListAnomalyGroupRelatedMetricsResponseTypeDef,
     ListMetricSetsResponseTypeDef,
     RDSSourceConfigOutputTypeDef,
     RedshiftSourceConfigOutputTypeDef,
     RDSSourceConfigTypeDef,
     RedshiftSourceConfigTypeDef,
     AlertTypeDef,
+    AlertFiltersUnionTypeDef,
     CreateAlertRequestRequestTypeDef,
     UpdateAlertRequestRequestTypeDef,
     ListAnomalyGroupSummariesResponseTypeDef,
     DetectedCsvFormatDescriptorTypeDef,
     DetectedJsonFormatDescriptorTypeDef,
     DetectMetricSetConfigRequestRequestTypeDef,
     AnomalyDetectorDataQualityMetricTypeDef,
     ContributionMatrixTypeDef,
     ListAnomalyGroupTimeSeriesResponseTypeDef,
     S3SourceConfigOutputTypeDef,
     S3SourceConfigTypeDef,
     SampleDataS3SourceConfigTypeDef,
+    MetricSetDimensionFilterUnionTypeDef,
     DescribeAlertResponseTypeDef,
     DetectedFileFormatDescriptorTypeDef,
     GetDataQualityMetricsResponseTypeDef,
     MetricLevelImpactTypeDef,
     MetricSourceOutputTypeDef,
     MetricSourceTypeDef,
     GetSampleDataRequestRequestTypeDef,
     DetectedS3SourceConfigTypeDef,
     AnomalyGroupTypeDef,
     DescribeMetricSetResponseTypeDef,
     CreateMetricSetRequestRequestTypeDef,
+    MetricSourceUnionTypeDef,
     UpdateMetricSetRequestRequestTypeDef,
     DetectedMetricSourceTypeDef,
     GetAnomalyGroupResponseTypeDef,
     DetectedMetricSetConfigTypeDef,
     DetectMetricSetConfigResponseTypeDef,
 )
 
 
-def get_structure() -> LambdaConfigurationTypeDef:
+def get_value() -> LambdaConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-lookoutmetrics-1.28.15.post1/mypy_boto3_lookoutmetrics.egg-info/SOURCES.txt` & `mypy-boto3-lookoutmetrics-1.28.16/mypy_boto3_lookoutmetrics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lookoutmetrics-1.28.15.post1/setup.py` & `mypy-boto3-lookoutmetrics-1.28.16/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-lookoutmetrics",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_lookoutmetrics"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.LookoutMetrics 1.28.15 service generated with"
-        " mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.LookoutMetrics 1.28.16 service generated with"
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
-    keywords="boto3 lookoutmetrics type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 lookoutmetrics type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_lookoutmetrics": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutmetrics/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

