# Comparing `tmp/mypy-boto3-forecast-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-forecast-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-forecast-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:09 2023, max compression
+gzip compressed data, was "mypy-boto3-forecast-1.28.16.tar", last modified: Tue Aug  1 11:36:49 2023, max compression
```

## Comparing `mypy-boto3-forecast-1.28.15.post1.tar` & `mypy-boto3-forecast-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:09.669155 mypy-boto3-forecast-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:45:34.000000 mypy-boto3-forecast-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    23733 2023-07-29 10:03:09.669155 mypy-boto3-forecast-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22229 2023-07-29 09:45:34.000000 mypy-boto3-forecast-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:09.665155 mypy-boto3-forecast-1.28.15.post1/mypy_boto3_forecast/
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-07-29 09:45:34.000000 mypy-boto3-forecast-1.28.15.post1/mypy_boto3_forecast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-07-29 09:45:34.000000 mypy-boto3-forecast-1.28.15.post1/mypy_boto3_forecast/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-29 09:45:34.000000 mypy-boto3-forecast-1.28.15.post1/mypy_boto3_forecast/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    52340 2023-07-29 09:45:35.000000 mypy-boto3-forecast-1.28.15.post1/mypy_boto3_forecast/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    52256 2023-07-29 09:45:35.000000 mypy-boto3-forecast-1.28.15.post1/mypy_boto3_forecast/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11618 2023-07-29 09:45:35.000000 mypy-boto3-forecast-1.28.15.post1/mypy_boto3_forecast/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11616 2023-07-29 09:45:35.000000 mypy-boto3-forecast-1.28.15.post1/mypy_boto3_forecast/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    17059 2023-07-29 09:45:35.000000 mypy-boto3-forecast-1.28.15.post1/mypy_boto3_forecast/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    17043 2023-07-29 09:45:35.000000 mypy-boto3-forecast-1.28.15.post1/mypy_boto3_forecast/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:45:34.000000 mypy-boto3-forecast-1.28.15.post1/mypy_boto3_forecast/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    71276 2023-07-29 09:45:37.000000 mypy-boto3-forecast-1.28.15.post1/mypy_boto3_forecast/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    71210 2023-07-29 09:45:36.000000 mypy-boto3-forecast-1.28.15.post1/mypy_boto3_forecast/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:45:34.000000 mypy-boto3-forecast-1.28.15.post1/mypy_boto3_forecast/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:09.669155 mypy-boto3-forecast-1.28.15.post1/mypy_boto3_forecast.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    23733 2023-07-29 10:03:09.000000 mypy-boto3-forecast-1.28.15.post1/mypy_boto3_forecast.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-29 10:03:09.000000 mypy-boto3-forecast-1.28.15.post1/mypy_boto3_forecast.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:09.000000 mypy-boto3-forecast-1.28.15.post1/mypy_boto3_forecast.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:09.000000 mypy-boto3-forecast-1.28.15.post1/mypy_boto3_forecast.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:09.000000 mypy-boto3-forecast-1.28.15.post1/mypy_boto3_forecast.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-29 10:03:09.000000 mypy-boto3-forecast-1.28.15.post1/mypy_boto3_forecast.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:09.669155 mypy-boto3-forecast-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-07-29 09:45:34.000000 mypy-boto3-forecast-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:49.288888 mypy-boto3-forecast-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:18:11.000000 mypy-boto3-forecast-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    24020 2023-08-01 11:36:49.288888 mypy-boto3-forecast-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22525 2023-08-01 11:18:11.000000 mypy-boto3-forecast-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:49.268888 mypy-boto3-forecast-1.28.16/mypy_boto3_forecast/
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-08-01 11:18:11.000000 mypy-boto3-forecast-1.28.16/mypy_boto3_forecast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-08-01 11:18:11.000000 mypy-boto3-forecast-1.28.16/mypy_boto3_forecast/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-08-01 11:18:11.000000 mypy-boto3-forecast-1.28.16/mypy_boto3_forecast/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51655 2023-08-01 11:18:12.000000 mypy-boto3-forecast-1.28.16/mypy_boto3_forecast/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51571 2023-08-01 11:18:11.000000 mypy-boto3-forecast-1.28.16/mypy_boto3_forecast/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11618 2023-08-01 11:18:12.000000 mypy-boto3-forecast-1.28.16/mypy_boto3_forecast/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11616 2023-08-01 11:18:12.000000 mypy-boto3-forecast-1.28.16/mypy_boto3_forecast/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    17059 2023-08-01 11:18:12.000000 mypy-boto3-forecast-1.28.16/mypy_boto3_forecast/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17043 2023-08-01 11:18:12.000000 mypy-boto3-forecast-1.28.16/mypy_boto3_forecast/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:18:11.000000 mypy-boto3-forecast-1.28.16/mypy_boto3_forecast/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    72369 2023-08-01 11:18:14.000000 mypy-boto3-forecast-1.28.16/mypy_boto3_forecast/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72302 2023-08-01 11:18:13.000000 mypy-boto3-forecast-1.28.16/mypy_boto3_forecast/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:18:11.000000 mypy-boto3-forecast-1.28.16/mypy_boto3_forecast/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:49.288888 mypy-boto3-forecast-1.28.16/mypy_boto3_forecast.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    24020 2023-08-01 11:36:49.000000 mypy-boto3-forecast-1.28.16/mypy_boto3_forecast.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-08-01 11:36:49.000000 mypy-boto3-forecast-1.28.16/mypy_boto3_forecast.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:49.000000 mypy-boto3-forecast-1.28.16/mypy_boto3_forecast.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:49.000000 mypy-boto3-forecast-1.28.16/mypy_boto3_forecast.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:49.000000 mypy-boto3-forecast-1.28.16/mypy_boto3_forecast.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-01 11:36:49.000000 mypy-boto3-forecast-1.28.16/mypy_boto3_forecast.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:49.288888 mypy-boto3-forecast-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-08-01 11:18:11.000000 mypy-boto3-forecast-1.28.16/setup.py
```

### Comparing `mypy-boto3-forecast-1.28.15.post1/LICENSE` & `mypy-boto3-forecast-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-forecast-1.28.15.post1/PKG-INFO` & `mypy-boto3-forecast-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-forecast
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.ForecastService 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.ForecastService 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 forecast type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 forecast type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-forecast.svg?color=blue)](https://pypi.org/project/mypy-boto3-forecast)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-forecast)](https://pepy.tech/project/mypy-boto3-forecast)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ForecastService 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService)
+[boto3.ForecastService 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService)
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
 [mypy-boto3-forecast docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/).
 
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
@@ -387,20 +387,20 @@
 )
 
 
 def check_value(value: AttributeTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_forecast.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_forecast.type_defs import (
     ActionTypeDef,
     AdditionalDatasetOutputTypeDef,
     AdditionalDatasetTypeDef,
     AttributeConfigOutputTypeDef,
@@ -547,14 +547,15 @@
     PredictorExecutionTypeDef,
     SchemaOutputTypeDef,
     SchemaTypeDef,
     TimeSeriesTransformationOutputTypeDef,
     TimeSeriesTransformationTypeDef,
     DescribeAutoPredictorResponseTypeDef,
     CreateAutoPredictorRequestRequestTypeDef,
+    DataConfigUnionTypeDef,
     BaselineTypeDef,
     ListExplainabilitiesResponseTypeDef,
     CreateExplainabilityExportRequestRequestTypeDef,
     CreateForecastExportJobRequestRequestTypeDef,
     CreatePredictorBacktestExportJobRequestRequestTypeDef,
     CreateWhatIfForecastExportRequestRequestTypeDef,
     DescribeExplainabilityExportResponseTypeDef,
@@ -567,49 +568,56 @@
     WhatIfForecastExportSummaryTypeDef,
     CreateDatasetImportJobRequestRequestTypeDef,
     DatasetImportJobSummaryTypeDef,
     DescribeDatasetImportJobResponseTypeDef,
     ListPredictorsResponseTypeDef,
     FeaturizationConfigOutputTypeDef,
     FeaturizationConfigTypeDef,
+    InputDataConfigUnionTypeDef,
     HyperParameterTuningJobConfigOutputTypeDef,
     HyperParameterTuningJobConfigTypeDef,
     WindowSummaryTypeDef,
     ListMonitorEvaluationsResponseTypeDef,
     PredictorExecutionDetailsTypeDef,
     DescribeDatasetResponseTypeDef,
     DescribeExplainabilityResponseTypeDef,
     TimeSeriesIdentifiersOutputTypeDef,
     TimeSeriesReplacementsDataSourceOutputTypeDef,
     CreateDatasetRequestRequestTypeDef,
     CreateExplainabilityRequestRequestTypeDef,
+    SchemaUnionTypeDef,
     TimeSeriesIdentifiersTypeDef,
     TimeSeriesReplacementsDataSourceTypeDef,
+    TimeSeriesTransformationUnionTypeDef,
     DescribeMonitorResponseTypeDef,
     ListExplainabilityExportsResponseTypeDef,
     ListForecastExportJobsResponseTypeDef,
     ListPredictorBacktestExportJobsResponseTypeDef,
     ListWhatIfForecastExportsResponseTypeDef,
     ListDatasetImportJobsResponseTypeDef,
+    FeaturizationConfigUnionTypeDef,
     CreatePredictorRequestRequestTypeDef,
+    HyperParameterTuningJobConfigUnionTypeDef,
     EvaluationResultTypeDef,
     DescribePredictorResponseTypeDef,
     TimeSeriesSelectorOutputTypeDef,
     DescribeWhatIfForecastResponseTypeDef,
     TimeSeriesSelectorTypeDef,
+    TimeSeriesReplacementsDataSourceUnionTypeDef,
     CreateWhatIfForecastRequestRequestTypeDef,
     GetAccuracyMetricsResponseTypeDef,
     DescribeForecastResponseTypeDef,
     DescribeWhatIfAnalysisResponseTypeDef,
     CreateForecastRequestRequestTypeDef,
     CreateWhatIfAnalysisRequestRequestTypeDef,
+    TimeSeriesSelectorUnionTypeDef,
 )
 
 
-def get_structure() -> ActionTypeDef:
+def get_value() -> ActionTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-forecast-1.28.15.post1/README.md` & `mypy-boto3-forecast-1.28.16/mypy_boto3_forecast.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-forecast
+Version: 1.28.16
+Summary: Type annotations for boto3.ForecastService 1.28.16 service generated with mypy-boto3-builder 7.17.1
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 forecast type-annotations botocore mypy typeshed autocomplete
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Typing :: Typed
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <a id="mypy-boto3-forecast"></a>
 
 # mypy-boto3-forecast
 
 [![PyPI - mypy-boto3-forecast](https://img.shields.io/pypi/v/mypy-boto3-forecast.svg?color=blue)](https://pypi.org/project/mypy-boto3-forecast)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-forecast.svg?color=blue)](https://pypi.org/project/mypy-boto3-forecast)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-forecast)](https://pepy.tech/project/mypy-boto3-forecast)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ForecastService 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService)
+[boto3.ForecastService 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService)
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
 [mypy-boto3-forecast docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/).
 
 See how it helps to find and fix potential bugs:
 
@@ -42,15 +74,15 @@
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
@@ -355,20 +387,20 @@
 )
 
 
 def check_value(value: AttributeTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_forecast.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_forecast.type_defs import (
     ActionTypeDef,
     AdditionalDatasetOutputTypeDef,
     AdditionalDatasetTypeDef,
     AttributeConfigOutputTypeDef,
@@ -515,14 +547,15 @@
     PredictorExecutionTypeDef,
     SchemaOutputTypeDef,
     SchemaTypeDef,
     TimeSeriesTransformationOutputTypeDef,
     TimeSeriesTransformationTypeDef,
     DescribeAutoPredictorResponseTypeDef,
     CreateAutoPredictorRequestRequestTypeDef,
+    DataConfigUnionTypeDef,
     BaselineTypeDef,
     ListExplainabilitiesResponseTypeDef,
     CreateExplainabilityExportRequestRequestTypeDef,
     CreateForecastExportJobRequestRequestTypeDef,
     CreatePredictorBacktestExportJobRequestRequestTypeDef,
     CreateWhatIfForecastExportRequestRequestTypeDef,
     DescribeExplainabilityExportResponseTypeDef,
@@ -535,49 +568,56 @@
     WhatIfForecastExportSummaryTypeDef,
     CreateDatasetImportJobRequestRequestTypeDef,
     DatasetImportJobSummaryTypeDef,
     DescribeDatasetImportJobResponseTypeDef,
     ListPredictorsResponseTypeDef,
     FeaturizationConfigOutputTypeDef,
     FeaturizationConfigTypeDef,
+    InputDataConfigUnionTypeDef,
     HyperParameterTuningJobConfigOutputTypeDef,
     HyperParameterTuningJobConfigTypeDef,
     WindowSummaryTypeDef,
     ListMonitorEvaluationsResponseTypeDef,
     PredictorExecutionDetailsTypeDef,
     DescribeDatasetResponseTypeDef,
     DescribeExplainabilityResponseTypeDef,
     TimeSeriesIdentifiersOutputTypeDef,
     TimeSeriesReplacementsDataSourceOutputTypeDef,
     CreateDatasetRequestRequestTypeDef,
     CreateExplainabilityRequestRequestTypeDef,
+    SchemaUnionTypeDef,
     TimeSeriesIdentifiersTypeDef,
     TimeSeriesReplacementsDataSourceTypeDef,
+    TimeSeriesTransformationUnionTypeDef,
     DescribeMonitorResponseTypeDef,
     ListExplainabilityExportsResponseTypeDef,
     ListForecastExportJobsResponseTypeDef,
     ListPredictorBacktestExportJobsResponseTypeDef,
     ListWhatIfForecastExportsResponseTypeDef,
     ListDatasetImportJobsResponseTypeDef,
+    FeaturizationConfigUnionTypeDef,
     CreatePredictorRequestRequestTypeDef,
+    HyperParameterTuningJobConfigUnionTypeDef,
     EvaluationResultTypeDef,
     DescribePredictorResponseTypeDef,
     TimeSeriesSelectorOutputTypeDef,
     DescribeWhatIfForecastResponseTypeDef,
     TimeSeriesSelectorTypeDef,
+    TimeSeriesReplacementsDataSourceUnionTypeDef,
     CreateWhatIfForecastRequestRequestTypeDef,
     GetAccuracyMetricsResponseTypeDef,
     DescribeForecastResponseTypeDef,
     DescribeWhatIfAnalysisResponseTypeDef,
     CreateForecastRequestRequestTypeDef,
     CreateWhatIfAnalysisRequestRequestTypeDef,
+    TimeSeriesSelectorUnionTypeDef,
 )
 
 
-def get_structure() -> ActionTypeDef:
+def get_value() -> ActionTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-forecast-1.28.15.post1/mypy_boto3_forecast/__init__.py` & `mypy-boto3-forecast-1.28.16/mypy_boto3_forecast/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-forecast-1.28.15.post1/mypy_boto3_forecast/__init__.pyi` & `mypy-boto3-forecast-1.28.16/mypy_boto3_forecast/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-forecast-1.28.15.post1/mypy_boto3_forecast/__main__.py` & `mypy-boto3-forecast-1.28.16/mypy_boto3_forecast/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ForecastService 1.28.15\nVersion:        "
-        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.ForecastService 1.28.16\nVersion:         1.28.16\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService\nOther"
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

### Comparing `mypy-boto3-forecast-1.28.15.post1/mypy_boto3_forecast/client.py` & `mypy-boto3-forecast-1.28.16/mypy_boto3_forecast/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_forecast.client import ForecastServiceClient
 
     session = Session()
     client: ForecastServiceClient = session.client("forecast")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AutoMLOverrideStrategyType,
     DatasetTypeType,
     DomainType,
@@ -52,16 +52,15 @@
     CreateForecastResponseTypeDef,
     CreateMonitorResponseTypeDef,
     CreatePredictorBacktestExportJobResponseTypeDef,
     CreatePredictorResponseTypeDef,
     CreateWhatIfAnalysisResponseTypeDef,
     CreateWhatIfForecastExportResponseTypeDef,
     CreateWhatIfForecastResponseTypeDef,
-    DataConfigOutputTypeDef,
-    DataConfigTypeDef,
+    DataConfigUnionTypeDef,
     DataDestinationTypeDef,
     DataSourceTypeDef,
     DescribeAutoPredictorResponseTypeDef,
     DescribeDatasetGroupResponseTypeDef,
     DescribeDatasetImportJobResponseTypeDef,
     DescribeDatasetResponseTypeDef,
     DescribeExplainabilityExportResponseTypeDef,
@@ -74,22 +73,19 @@
     DescribeWhatIfAnalysisResponseTypeDef,
     DescribeWhatIfForecastExportResponseTypeDef,
     DescribeWhatIfForecastResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     EncryptionConfigTypeDef,
     EvaluationParametersTypeDef,
     ExplainabilityConfigTypeDef,
-    FeaturizationConfigOutputTypeDef,
-    FeaturizationConfigTypeDef,
+    FeaturizationConfigUnionTypeDef,
     FilterTypeDef,
     GetAccuracyMetricsResponseTypeDef,
-    HyperParameterTuningJobConfigOutputTypeDef,
-    HyperParameterTuningJobConfigTypeDef,
-    InputDataConfigOutputTypeDef,
-    InputDataConfigTypeDef,
+    HyperParameterTuningJobConfigUnionTypeDef,
+    InputDataConfigUnionTypeDef,
     ListDatasetGroupsResponseTypeDef,
     ListDatasetImportJobsResponseTypeDef,
     ListDatasetsResponseTypeDef,
     ListExplainabilitiesResponseTypeDef,
     ListExplainabilityExportsResponseTypeDef,
     ListForecastExportJobsResponseTypeDef,
     ListForecastsResponseTypeDef,
@@ -98,24 +94,20 @@
     ListPredictorBacktestExportJobsResponseTypeDef,
     ListPredictorsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListWhatIfAnalysesResponseTypeDef,
     ListWhatIfForecastExportsResponseTypeDef,
     ListWhatIfForecastsResponseTypeDef,
     MonitorConfigTypeDef,
-    SchemaOutputTypeDef,
-    SchemaTypeDef,
+    SchemaUnionTypeDef,
     TagTypeDef,
     TimeAlignmentBoundaryTypeDef,
-    TimeSeriesReplacementsDataSourceOutputTypeDef,
-    TimeSeriesReplacementsDataSourceTypeDef,
-    TimeSeriesSelectorOutputTypeDef,
-    TimeSeriesSelectorTypeDef,
-    TimeSeriesTransformationOutputTypeDef,
-    TimeSeriesTransformationTypeDef,
+    TimeSeriesReplacementsDataSourceUnionTypeDef,
+    TimeSeriesSelectorUnionTypeDef,
+    TimeSeriesTransformationUnionTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -178,15 +170,15 @@
         self,
         *,
         PredictorName: str,
         ForecastHorizon: int = ...,
         ForecastTypes: Sequence[str] = ...,
         ForecastDimensions: Sequence[str] = ...,
         ForecastFrequency: str = ...,
-        DataConfig: Union[DataConfigTypeDef, DataConfigOutputTypeDef] = ...,
+        DataConfig: DataConfigUnionTypeDef = ...,
         EncryptionConfig: EncryptionConfigTypeDef = ...,
         ReferencePredictorArn: str = ...,
         OptimizationMetric: OptimizationMetricType = ...,
         ExplainPredictor: bool = ...,
         Tags: Sequence[TagTypeDef] = ...,
         MonitorConfig: MonitorConfigTypeDef = ...,
         TimeAlignmentBoundary: TimeAlignmentBoundaryTypeDef = ...
@@ -200,15 +192,15 @@
 
     def create_dataset(
         self,
         *,
         DatasetName: str,
         Domain: DomainType,
         DatasetType: DatasetTypeType,
-        Schema: Union[SchemaTypeDef, SchemaOutputTypeDef],
+        Schema: SchemaUnionTypeDef,
         DataFrequency: str = ...,
         EncryptionConfig: EncryptionConfigTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateDatasetResponseTypeDef:
         """
         Creates an Amazon Forecast dataset.
 
@@ -255,15 +247,15 @@
     def create_explainability(
         self,
         *,
         ExplainabilityName: str,
         ResourceArn: str,
         ExplainabilityConfig: ExplainabilityConfigTypeDef,
         DataSource: DataSourceTypeDef = ...,
-        Schema: Union[SchemaTypeDef, SchemaOutputTypeDef] = ...,
+        Schema: SchemaUnionTypeDef = ...,
         EnableVisualization: bool = ...,
         StartDateTime: str = ...,
         EndDateTime: str = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateExplainabilityResponseTypeDef:
         """
         .
@@ -292,15 +284,15 @@
     def create_forecast(
         self,
         *,
         ForecastName: str,
         PredictorArn: str,
         ForecastTypes: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        TimeSeriesSelector: Union[TimeSeriesSelectorTypeDef, TimeSeriesSelectorOutputTypeDef] = ...
+        TimeSeriesSelector: TimeSeriesSelectorUnionTypeDef = ...
     ) -> CreateForecastResponseTypeDef:
         """
         Creates a forecast for each item in the `TARGET_TIME_SERIES` dataset that was
         used to train the predictor.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Client.create_forecast)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/client/#create_forecast)
@@ -334,26 +326,24 @@
         """
 
     def create_predictor(
         self,
         *,
         PredictorName: str,
         ForecastHorizon: int,
-        InputDataConfig: Union[InputDataConfigTypeDef, InputDataConfigOutputTypeDef],
-        FeaturizationConfig: Union[FeaturizationConfigTypeDef, FeaturizationConfigOutputTypeDef],
+        InputDataConfig: InputDataConfigUnionTypeDef,
+        FeaturizationConfig: FeaturizationConfigUnionTypeDef,
         AlgorithmArn: str = ...,
         ForecastTypes: Sequence[str] = ...,
         PerformAutoML: bool = ...,
         AutoMLOverrideStrategy: AutoMLOverrideStrategyType = ...,
         PerformHPO: bool = ...,
         TrainingParameters: Mapping[str, str] = ...,
         EvaluationParameters: EvaluationParametersTypeDef = ...,
-        HPOConfig: Union[
-            HyperParameterTuningJobConfigTypeDef, HyperParameterTuningJobConfigOutputTypeDef
-        ] = ...,
+        HPOConfig: HyperParameterTuningJobConfigUnionTypeDef = ...,
         EncryptionConfig: EncryptionConfigTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         OptimizationMetric: OptimizationMetricType = ...
     ) -> CreatePredictorResponseTypeDef:
         """
         .
 
@@ -379,15 +369,15 @@
         """
 
     def create_what_if_analysis(
         self,
         *,
         WhatIfAnalysisName: str,
         ForecastArn: str,
-        TimeSeriesSelector: Union[TimeSeriesSelectorTypeDef, TimeSeriesSelectorOutputTypeDef] = ...,
+        TimeSeriesSelector: TimeSeriesSelectorUnionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateWhatIfAnalysisResponseTypeDef:
         """
         What-if analysis is a scenario modeling technique where you make a hypothetical
         change to a time series and compare the forecasts generated by these changes
         against the baseline, unchanged time series.
 
@@ -396,20 +386,16 @@
         """
 
     def create_what_if_forecast(
         self,
         *,
         WhatIfForecastName: str,
         WhatIfAnalysisArn: str,
-        TimeSeriesTransformations: Sequence[
-            Union[TimeSeriesTransformationTypeDef, TimeSeriesTransformationOutputTypeDef]
-        ] = ...,
-        TimeSeriesReplacementsDataSource: Union[
-            TimeSeriesReplacementsDataSourceTypeDef, TimeSeriesReplacementsDataSourceOutputTypeDef
-        ] = ...,
+        TimeSeriesTransformations: Sequence[TimeSeriesTransformationUnionTypeDef] = ...,
+        TimeSeriesReplacementsDataSource: TimeSeriesReplacementsDataSourceUnionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateWhatIfForecastResponseTypeDef:
         """
         A what-if forecast is a forecast that is created from a modified version of the
         baseline forecast.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Client.create_what_if_forecast)
```

### Comparing `mypy-boto3-forecast-1.28.15.post1/mypy_boto3_forecast/client.pyi` & `mypy-boto3-forecast-1.28.16/mypy_boto3_forecast/client.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_forecast.client import ForecastServiceClient
 
     session = Session()
     client: ForecastServiceClient = session.client("forecast")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AutoMLOverrideStrategyType,
     DatasetTypeType,
     DomainType,
@@ -52,16 +52,15 @@
     CreateForecastResponseTypeDef,
     CreateMonitorResponseTypeDef,
     CreatePredictorBacktestExportJobResponseTypeDef,
     CreatePredictorResponseTypeDef,
     CreateWhatIfAnalysisResponseTypeDef,
     CreateWhatIfForecastExportResponseTypeDef,
     CreateWhatIfForecastResponseTypeDef,
-    DataConfigOutputTypeDef,
-    DataConfigTypeDef,
+    DataConfigUnionTypeDef,
     DataDestinationTypeDef,
     DataSourceTypeDef,
     DescribeAutoPredictorResponseTypeDef,
     DescribeDatasetGroupResponseTypeDef,
     DescribeDatasetImportJobResponseTypeDef,
     DescribeDatasetResponseTypeDef,
     DescribeExplainabilityExportResponseTypeDef,
@@ -74,22 +73,19 @@
     DescribeWhatIfAnalysisResponseTypeDef,
     DescribeWhatIfForecastExportResponseTypeDef,
     DescribeWhatIfForecastResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     EncryptionConfigTypeDef,
     EvaluationParametersTypeDef,
     ExplainabilityConfigTypeDef,
-    FeaturizationConfigOutputTypeDef,
-    FeaturizationConfigTypeDef,
+    FeaturizationConfigUnionTypeDef,
     FilterTypeDef,
     GetAccuracyMetricsResponseTypeDef,
-    HyperParameterTuningJobConfigOutputTypeDef,
-    HyperParameterTuningJobConfigTypeDef,
-    InputDataConfigOutputTypeDef,
-    InputDataConfigTypeDef,
+    HyperParameterTuningJobConfigUnionTypeDef,
+    InputDataConfigUnionTypeDef,
     ListDatasetGroupsResponseTypeDef,
     ListDatasetImportJobsResponseTypeDef,
     ListDatasetsResponseTypeDef,
     ListExplainabilitiesResponseTypeDef,
     ListExplainabilityExportsResponseTypeDef,
     ListForecastExportJobsResponseTypeDef,
     ListForecastsResponseTypeDef,
@@ -98,24 +94,20 @@
     ListPredictorBacktestExportJobsResponseTypeDef,
     ListPredictorsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListWhatIfAnalysesResponseTypeDef,
     ListWhatIfForecastExportsResponseTypeDef,
     ListWhatIfForecastsResponseTypeDef,
     MonitorConfigTypeDef,
-    SchemaOutputTypeDef,
-    SchemaTypeDef,
+    SchemaUnionTypeDef,
     TagTypeDef,
     TimeAlignmentBoundaryTypeDef,
-    TimeSeriesReplacementsDataSourceOutputTypeDef,
-    TimeSeriesReplacementsDataSourceTypeDef,
-    TimeSeriesSelectorOutputTypeDef,
-    TimeSeriesSelectorTypeDef,
-    TimeSeriesTransformationOutputTypeDef,
-    TimeSeriesTransformationTypeDef,
+    TimeSeriesReplacementsDataSourceUnionTypeDef,
+    TimeSeriesSelectorUnionTypeDef,
+    TimeSeriesTransformationUnionTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -171,15 +163,15 @@
         self,
         *,
         PredictorName: str,
         ForecastHorizon: int = ...,
         ForecastTypes: Sequence[str] = ...,
         ForecastDimensions: Sequence[str] = ...,
         ForecastFrequency: str = ...,
-        DataConfig: Union[DataConfigTypeDef, DataConfigOutputTypeDef] = ...,
+        DataConfig: DataConfigUnionTypeDef = ...,
         EncryptionConfig: EncryptionConfigTypeDef = ...,
         ReferencePredictorArn: str = ...,
         OptimizationMetric: OptimizationMetricType = ...,
         ExplainPredictor: bool = ...,
         Tags: Sequence[TagTypeDef] = ...,
         MonitorConfig: MonitorConfigTypeDef = ...,
         TimeAlignmentBoundary: TimeAlignmentBoundaryTypeDef = ...
@@ -192,15 +184,15 @@
         """
     def create_dataset(
         self,
         *,
         DatasetName: str,
         Domain: DomainType,
         DatasetType: DatasetTypeType,
-        Schema: Union[SchemaTypeDef, SchemaOutputTypeDef],
+        Schema: SchemaUnionTypeDef,
         DataFrequency: str = ...,
         EncryptionConfig: EncryptionConfigTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateDatasetResponseTypeDef:
         """
         Creates an Amazon Forecast dataset.
 
@@ -244,15 +236,15 @@
     def create_explainability(
         self,
         *,
         ExplainabilityName: str,
         ResourceArn: str,
         ExplainabilityConfig: ExplainabilityConfigTypeDef,
         DataSource: DataSourceTypeDef = ...,
-        Schema: Union[SchemaTypeDef, SchemaOutputTypeDef] = ...,
+        Schema: SchemaUnionTypeDef = ...,
         EnableVisualization: bool = ...,
         StartDateTime: str = ...,
         EndDateTime: str = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateExplainabilityResponseTypeDef:
         """
         .
@@ -279,15 +271,15 @@
     def create_forecast(
         self,
         *,
         ForecastName: str,
         PredictorArn: str,
         ForecastTypes: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        TimeSeriesSelector: Union[TimeSeriesSelectorTypeDef, TimeSeriesSelectorOutputTypeDef] = ...
+        TimeSeriesSelector: TimeSeriesSelectorUnionTypeDef = ...
     ) -> CreateForecastResponseTypeDef:
         """
         Creates a forecast for each item in the `TARGET_TIME_SERIES` dataset that was
         used to train the predictor.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Client.create_forecast)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/client/#create_forecast)
@@ -318,26 +310,24 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/client/#create_monitor)
         """
     def create_predictor(
         self,
         *,
         PredictorName: str,
         ForecastHorizon: int,
-        InputDataConfig: Union[InputDataConfigTypeDef, InputDataConfigOutputTypeDef],
-        FeaturizationConfig: Union[FeaturizationConfigTypeDef, FeaturizationConfigOutputTypeDef],
+        InputDataConfig: InputDataConfigUnionTypeDef,
+        FeaturizationConfig: FeaturizationConfigUnionTypeDef,
         AlgorithmArn: str = ...,
         ForecastTypes: Sequence[str] = ...,
         PerformAutoML: bool = ...,
         AutoMLOverrideStrategy: AutoMLOverrideStrategyType = ...,
         PerformHPO: bool = ...,
         TrainingParameters: Mapping[str, str] = ...,
         EvaluationParameters: EvaluationParametersTypeDef = ...,
-        HPOConfig: Union[
-            HyperParameterTuningJobConfigTypeDef, HyperParameterTuningJobConfigOutputTypeDef
-        ] = ...,
+        HPOConfig: HyperParameterTuningJobConfigUnionTypeDef = ...,
         EncryptionConfig: EncryptionConfigTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         OptimizationMetric: OptimizationMetricType = ...
     ) -> CreatePredictorResponseTypeDef:
         """
         .
 
@@ -361,15 +351,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/client/#create_predictor_backtest_export_job)
         """
     def create_what_if_analysis(
         self,
         *,
         WhatIfAnalysisName: str,
         ForecastArn: str,
-        TimeSeriesSelector: Union[TimeSeriesSelectorTypeDef, TimeSeriesSelectorOutputTypeDef] = ...,
+        TimeSeriesSelector: TimeSeriesSelectorUnionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateWhatIfAnalysisResponseTypeDef:
         """
         What-if analysis is a scenario modeling technique where you make a hypothetical
         change to a time series and compare the forecasts generated by these changes
         against the baseline, unchanged time series.
 
@@ -377,20 +367,16 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/client/#create_what_if_analysis)
         """
     def create_what_if_forecast(
         self,
         *,
         WhatIfForecastName: str,
         WhatIfAnalysisArn: str,
-        TimeSeriesTransformations: Sequence[
-            Union[TimeSeriesTransformationTypeDef, TimeSeriesTransformationOutputTypeDef]
-        ] = ...,
-        TimeSeriesReplacementsDataSource: Union[
-            TimeSeriesReplacementsDataSourceTypeDef, TimeSeriesReplacementsDataSourceOutputTypeDef
-        ] = ...,
+        TimeSeriesTransformations: Sequence[TimeSeriesTransformationUnionTypeDef] = ...,
+        TimeSeriesReplacementsDataSource: TimeSeriesReplacementsDataSourceUnionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateWhatIfForecastResponseTypeDef:
         """
         A what-if forecast is a forecast that is created from a modified version of the
         baseline forecast.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Client.create_what_if_forecast)
```

### Comparing `mypy-boto3-forecast-1.28.15.post1/mypy_boto3_forecast/literals.py` & `mypy-boto3-forecast-1.28.16/mypy_boto3_forecast/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-forecast-1.28.15.post1/mypy_boto3_forecast/literals.pyi` & `mypy-boto3-forecast-1.28.16/mypy_boto3_forecast/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-forecast-1.28.15.post1/mypy_boto3_forecast/paginator.py` & `mypy-boto3-forecast-1.28.16/mypy_boto3_forecast/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-forecast-1.28.15.post1/mypy_boto3_forecast/paginator.pyi` & `mypy-boto3-forecast-1.28.16/mypy_boto3_forecast/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-forecast-1.28.15.post1/mypy_boto3_forecast/type_defs.py` & `mypy-boto3-forecast-1.28.16/mypy_boto3_forecast/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_forecast.type_defs import ActionTypeDef
 
-    data: ActionTypeDef = {...}
+    data: ActionTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -192,14 +192,15 @@
     "PredictorExecutionTypeDef",
     "SchemaOutputTypeDef",
     "SchemaTypeDef",
     "TimeSeriesTransformationOutputTypeDef",
     "TimeSeriesTransformationTypeDef",
     "DescribeAutoPredictorResponseTypeDef",
     "CreateAutoPredictorRequestRequestTypeDef",
+    "DataConfigUnionTypeDef",
     "BaselineTypeDef",
     "ListExplainabilitiesResponseTypeDef",
     "CreateExplainabilityExportRequestRequestTypeDef",
     "CreateForecastExportJobRequestRequestTypeDef",
     "CreatePredictorBacktestExportJobRequestRequestTypeDef",
     "CreateWhatIfForecastExportRequestRequestTypeDef",
     "DescribeExplainabilityExportResponseTypeDef",
@@ -212,45 +213,52 @@
     "WhatIfForecastExportSummaryTypeDef",
     "CreateDatasetImportJobRequestRequestTypeDef",
     "DatasetImportJobSummaryTypeDef",
     "DescribeDatasetImportJobResponseTypeDef",
     "ListPredictorsResponseTypeDef",
     "FeaturizationConfigOutputTypeDef",
     "FeaturizationConfigTypeDef",
+    "InputDataConfigUnionTypeDef",
     "HyperParameterTuningJobConfigOutputTypeDef",
     "HyperParameterTuningJobConfigTypeDef",
     "WindowSummaryTypeDef",
     "ListMonitorEvaluationsResponseTypeDef",
     "PredictorExecutionDetailsTypeDef",
     "DescribeDatasetResponseTypeDef",
     "DescribeExplainabilityResponseTypeDef",
     "TimeSeriesIdentifiersOutputTypeDef",
     "TimeSeriesReplacementsDataSourceOutputTypeDef",
     "CreateDatasetRequestRequestTypeDef",
     "CreateExplainabilityRequestRequestTypeDef",
+    "SchemaUnionTypeDef",
     "TimeSeriesIdentifiersTypeDef",
     "TimeSeriesReplacementsDataSourceTypeDef",
+    "TimeSeriesTransformationUnionTypeDef",
     "DescribeMonitorResponseTypeDef",
     "ListExplainabilityExportsResponseTypeDef",
     "ListForecastExportJobsResponseTypeDef",
     "ListPredictorBacktestExportJobsResponseTypeDef",
     "ListWhatIfForecastExportsResponseTypeDef",
     "ListDatasetImportJobsResponseTypeDef",
+    "FeaturizationConfigUnionTypeDef",
     "CreatePredictorRequestRequestTypeDef",
+    "HyperParameterTuningJobConfigUnionTypeDef",
     "EvaluationResultTypeDef",
     "DescribePredictorResponseTypeDef",
     "TimeSeriesSelectorOutputTypeDef",
     "DescribeWhatIfForecastResponseTypeDef",
     "TimeSeriesSelectorTypeDef",
+    "TimeSeriesReplacementsDataSourceUnionTypeDef",
     "CreateWhatIfForecastRequestRequestTypeDef",
     "GetAccuracyMetricsResponseTypeDef",
     "DescribeForecastResponseTypeDef",
     "DescribeWhatIfAnalysisResponseTypeDef",
     "CreateForecastRequestRequestTypeDef",
     "CreateWhatIfAnalysisRequestRequestTypeDef",
+    "TimeSeriesSelectorUnionTypeDef",
 )
 
 ActionTypeDef = TypedDict(
     "ActionTypeDef",
     {
         "AttributeName": str,
         "Operation": OperationType,
@@ -1842,14 +1850,15 @@
 class CreateAutoPredictorRequestRequestTypeDef(
     _RequiredCreateAutoPredictorRequestRequestTypeDef,
     _OptionalCreateAutoPredictorRequestRequestTypeDef,
 ):
     pass
 
 
+DataConfigUnionTypeDef = Union[DataConfigTypeDef, DataConfigOutputTypeDef]
 BaselineTypeDef = TypedDict(
     "BaselineTypeDef",
     {
         "PredictorBaseline": PredictorBaselineTypeDef,
     },
     total=False,
 )
@@ -2203,14 +2212,15 @@
 
 class FeaturizationConfigTypeDef(
     _RequiredFeaturizationConfigTypeDef, _OptionalFeaturizationConfigTypeDef
 ):
     pass
 
 
+InputDataConfigUnionTypeDef = Union[InputDataConfigTypeDef, InputDataConfigOutputTypeDef]
 HyperParameterTuningJobConfigOutputTypeDef = TypedDict(
     "HyperParameterTuningJobConfigOutputTypeDef",
     {
         "ParameterRanges": ParameterRangesOutputTypeDef,
     },
     total=False,
 )
@@ -2375,14 +2385,15 @@
 class CreateExplainabilityRequestRequestTypeDef(
     _RequiredCreateExplainabilityRequestRequestTypeDef,
     _OptionalCreateExplainabilityRequestRequestTypeDef,
 ):
     pass
 
 
+SchemaUnionTypeDef = Union[SchemaTypeDef, SchemaOutputTypeDef]
 TimeSeriesIdentifiersTypeDef = TypedDict(
     "TimeSeriesIdentifiersTypeDef",
     {
         "DataSource": DataSourceTypeDef,
         "Schema": SchemaTypeDef,
         "Format": str,
     },
@@ -2409,14 +2420,17 @@
 class TimeSeriesReplacementsDataSourceTypeDef(
     _RequiredTimeSeriesReplacementsDataSourceTypeDef,
     _OptionalTimeSeriesReplacementsDataSourceTypeDef,
 ):
     pass
 
 
+TimeSeriesTransformationUnionTypeDef = Union[
+    TimeSeriesTransformationTypeDef, TimeSeriesTransformationOutputTypeDef
+]
 DescribeMonitorResponseTypeDef = TypedDict(
     "DescribeMonitorResponseTypeDef",
     {
         "MonitorName": str,
         "MonitorArn": str,
         "ResourceArn": str,
         "Status": str,
@@ -2472,14 +2486,17 @@
     {
         "DatasetImportJobs": List[DatasetImportJobSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+FeaturizationConfigUnionTypeDef = Union[
+    FeaturizationConfigTypeDef, FeaturizationConfigOutputTypeDef
+]
 _RequiredCreatePredictorRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePredictorRequestRequestTypeDef",
     {
         "PredictorName": str,
         "ForecastHorizon": int,
         "InputDataConfig": InputDataConfigTypeDef,
         "FeaturizationConfig": FeaturizationConfigTypeDef,
@@ -2506,14 +2523,17 @@
 
 class CreatePredictorRequestRequestTypeDef(
     _RequiredCreatePredictorRequestRequestTypeDef, _OptionalCreatePredictorRequestRequestTypeDef
 ):
     pass
 
 
+HyperParameterTuningJobConfigUnionTypeDef = Union[
+    HyperParameterTuningJobConfigTypeDef, HyperParameterTuningJobConfigOutputTypeDef
+]
 EvaluationResultTypeDef = TypedDict(
     "EvaluationResultTypeDef",
     {
         "AlgorithmArn": str,
         "TestWindows": List[WindowSummaryTypeDef],
     },
     total=False,
@@ -2580,27 +2600,28 @@
     "TimeSeriesSelectorTypeDef",
     {
         "TimeSeriesIdentifiers": TimeSeriesIdentifiersTypeDef,
     },
     total=False,
 )
 
+TimeSeriesReplacementsDataSourceUnionTypeDef = Union[
+    TimeSeriesReplacementsDataSourceTypeDef, TimeSeriesReplacementsDataSourceOutputTypeDef
+]
 _RequiredCreateWhatIfForecastRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWhatIfForecastRequestRequestTypeDef",
     {
         "WhatIfForecastName": str,
         "WhatIfAnalysisArn": str,
     },
 )
 _OptionalCreateWhatIfForecastRequestRequestTypeDef = TypedDict(
     "_OptionalCreateWhatIfForecastRequestRequestTypeDef",
     {
-        "TimeSeriesTransformations": Sequence[
-            Union[TimeSeriesTransformationTypeDef, TimeSeriesTransformationOutputTypeDef]
-        ],
+        "TimeSeriesTransformations": Sequence[TimeSeriesTransformationUnionTypeDef],
         "TimeSeriesReplacementsDataSource": TimeSeriesReplacementsDataSourceTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
 
@@ -2698,7 +2719,10 @@
 
 
 class CreateWhatIfAnalysisRequestRequestTypeDef(
     _RequiredCreateWhatIfAnalysisRequestRequestTypeDef,
     _OptionalCreateWhatIfAnalysisRequestRequestTypeDef,
 ):
     pass
+
+
+TimeSeriesSelectorUnionTypeDef = Union[TimeSeriesSelectorTypeDef, TimeSeriesSelectorOutputTypeDef]
```

### Comparing `mypy-boto3-forecast-1.28.15.post1/mypy_boto3_forecast/type_defs.pyi` & `mypy-boto3-forecast-1.28.16/mypy_boto3_forecast/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_forecast.type_defs import ActionTypeDef
 
-    data: ActionTypeDef = {...}
+    data: ActionTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -191,14 +191,15 @@
     "PredictorExecutionTypeDef",
     "SchemaOutputTypeDef",
     "SchemaTypeDef",
     "TimeSeriesTransformationOutputTypeDef",
     "TimeSeriesTransformationTypeDef",
     "DescribeAutoPredictorResponseTypeDef",
     "CreateAutoPredictorRequestRequestTypeDef",
+    "DataConfigUnionTypeDef",
     "BaselineTypeDef",
     "ListExplainabilitiesResponseTypeDef",
     "CreateExplainabilityExportRequestRequestTypeDef",
     "CreateForecastExportJobRequestRequestTypeDef",
     "CreatePredictorBacktestExportJobRequestRequestTypeDef",
     "CreateWhatIfForecastExportRequestRequestTypeDef",
     "DescribeExplainabilityExportResponseTypeDef",
@@ -211,45 +212,52 @@
     "WhatIfForecastExportSummaryTypeDef",
     "CreateDatasetImportJobRequestRequestTypeDef",
     "DatasetImportJobSummaryTypeDef",
     "DescribeDatasetImportJobResponseTypeDef",
     "ListPredictorsResponseTypeDef",
     "FeaturizationConfigOutputTypeDef",
     "FeaturizationConfigTypeDef",
+    "InputDataConfigUnionTypeDef",
     "HyperParameterTuningJobConfigOutputTypeDef",
     "HyperParameterTuningJobConfigTypeDef",
     "WindowSummaryTypeDef",
     "ListMonitorEvaluationsResponseTypeDef",
     "PredictorExecutionDetailsTypeDef",
     "DescribeDatasetResponseTypeDef",
     "DescribeExplainabilityResponseTypeDef",
     "TimeSeriesIdentifiersOutputTypeDef",
     "TimeSeriesReplacementsDataSourceOutputTypeDef",
     "CreateDatasetRequestRequestTypeDef",
     "CreateExplainabilityRequestRequestTypeDef",
+    "SchemaUnionTypeDef",
     "TimeSeriesIdentifiersTypeDef",
     "TimeSeriesReplacementsDataSourceTypeDef",
+    "TimeSeriesTransformationUnionTypeDef",
     "DescribeMonitorResponseTypeDef",
     "ListExplainabilityExportsResponseTypeDef",
     "ListForecastExportJobsResponseTypeDef",
     "ListPredictorBacktestExportJobsResponseTypeDef",
     "ListWhatIfForecastExportsResponseTypeDef",
     "ListDatasetImportJobsResponseTypeDef",
+    "FeaturizationConfigUnionTypeDef",
     "CreatePredictorRequestRequestTypeDef",
+    "HyperParameterTuningJobConfigUnionTypeDef",
     "EvaluationResultTypeDef",
     "DescribePredictorResponseTypeDef",
     "TimeSeriesSelectorOutputTypeDef",
     "DescribeWhatIfForecastResponseTypeDef",
     "TimeSeriesSelectorTypeDef",
+    "TimeSeriesReplacementsDataSourceUnionTypeDef",
     "CreateWhatIfForecastRequestRequestTypeDef",
     "GetAccuracyMetricsResponseTypeDef",
     "DescribeForecastResponseTypeDef",
     "DescribeWhatIfAnalysisResponseTypeDef",
     "CreateForecastRequestRequestTypeDef",
     "CreateWhatIfAnalysisRequestRequestTypeDef",
+    "TimeSeriesSelectorUnionTypeDef",
 )
 
 ActionTypeDef = TypedDict(
     "ActionTypeDef",
     {
         "AttributeName": str,
         "Operation": OperationType,
@@ -1805,14 +1813,15 @@
 
 class CreateAutoPredictorRequestRequestTypeDef(
     _RequiredCreateAutoPredictorRequestRequestTypeDef,
     _OptionalCreateAutoPredictorRequestRequestTypeDef,
 ):
     pass
 
+DataConfigUnionTypeDef = Union[DataConfigTypeDef, DataConfigOutputTypeDef]
 BaselineTypeDef = TypedDict(
     "BaselineTypeDef",
     {
         "PredictorBaseline": PredictorBaselineTypeDef,
     },
     total=False,
 )
@@ -2152,14 +2161,15 @@
 )
 
 class FeaturizationConfigTypeDef(
     _RequiredFeaturizationConfigTypeDef, _OptionalFeaturizationConfigTypeDef
 ):
     pass
 
+InputDataConfigUnionTypeDef = Union[InputDataConfigTypeDef, InputDataConfigOutputTypeDef]
 HyperParameterTuningJobConfigOutputTypeDef = TypedDict(
     "HyperParameterTuningJobConfigOutputTypeDef",
     {
         "ParameterRanges": ParameterRangesOutputTypeDef,
     },
     total=False,
 )
@@ -2318,14 +2328,15 @@
 
 class CreateExplainabilityRequestRequestTypeDef(
     _RequiredCreateExplainabilityRequestRequestTypeDef,
     _OptionalCreateExplainabilityRequestRequestTypeDef,
 ):
     pass
 
+SchemaUnionTypeDef = Union[SchemaTypeDef, SchemaOutputTypeDef]
 TimeSeriesIdentifiersTypeDef = TypedDict(
     "TimeSeriesIdentifiersTypeDef",
     {
         "DataSource": DataSourceTypeDef,
         "Schema": SchemaTypeDef,
         "Format": str,
     },
@@ -2350,14 +2361,17 @@
 
 class TimeSeriesReplacementsDataSourceTypeDef(
     _RequiredTimeSeriesReplacementsDataSourceTypeDef,
     _OptionalTimeSeriesReplacementsDataSourceTypeDef,
 ):
     pass
 
+TimeSeriesTransformationUnionTypeDef = Union[
+    TimeSeriesTransformationTypeDef, TimeSeriesTransformationOutputTypeDef
+]
 DescribeMonitorResponseTypeDef = TypedDict(
     "DescribeMonitorResponseTypeDef",
     {
         "MonitorName": str,
         "MonitorArn": str,
         "ResourceArn": str,
         "Status": str,
@@ -2413,14 +2427,17 @@
     {
         "DatasetImportJobs": List[DatasetImportJobSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+FeaturizationConfigUnionTypeDef = Union[
+    FeaturizationConfigTypeDef, FeaturizationConfigOutputTypeDef
+]
 _RequiredCreatePredictorRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePredictorRequestRequestTypeDef",
     {
         "PredictorName": str,
         "ForecastHorizon": int,
         "InputDataConfig": InputDataConfigTypeDef,
         "FeaturizationConfig": FeaturizationConfigTypeDef,
@@ -2445,14 +2462,17 @@
 )
 
 class CreatePredictorRequestRequestTypeDef(
     _RequiredCreatePredictorRequestRequestTypeDef, _OptionalCreatePredictorRequestRequestTypeDef
 ):
     pass
 
+HyperParameterTuningJobConfigUnionTypeDef = Union[
+    HyperParameterTuningJobConfigTypeDef, HyperParameterTuningJobConfigOutputTypeDef
+]
 EvaluationResultTypeDef = TypedDict(
     "EvaluationResultTypeDef",
     {
         "AlgorithmArn": str,
         "TestWindows": List[WindowSummaryTypeDef],
     },
     total=False,
@@ -2519,27 +2539,28 @@
     "TimeSeriesSelectorTypeDef",
     {
         "TimeSeriesIdentifiers": TimeSeriesIdentifiersTypeDef,
     },
     total=False,
 )
 
+TimeSeriesReplacementsDataSourceUnionTypeDef = Union[
+    TimeSeriesReplacementsDataSourceTypeDef, TimeSeriesReplacementsDataSourceOutputTypeDef
+]
 _RequiredCreateWhatIfForecastRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWhatIfForecastRequestRequestTypeDef",
     {
         "WhatIfForecastName": str,
         "WhatIfAnalysisArn": str,
     },
 )
 _OptionalCreateWhatIfForecastRequestRequestTypeDef = TypedDict(
     "_OptionalCreateWhatIfForecastRequestRequestTypeDef",
     {
-        "TimeSeriesTransformations": Sequence[
-            Union[TimeSeriesTransformationTypeDef, TimeSeriesTransformationOutputTypeDef]
-        ],
+        "TimeSeriesTransformations": Sequence[TimeSeriesTransformationUnionTypeDef],
         "TimeSeriesReplacementsDataSource": TimeSeriesReplacementsDataSourceTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
 class CreateWhatIfForecastRequestRequestTypeDef(
@@ -2632,7 +2653,9 @@
 )
 
 class CreateWhatIfAnalysisRequestRequestTypeDef(
     _RequiredCreateWhatIfAnalysisRequestRequestTypeDef,
     _OptionalCreateWhatIfAnalysisRequestRequestTypeDef,
 ):
     pass
+
+TimeSeriesSelectorUnionTypeDef = Union[TimeSeriesSelectorTypeDef, TimeSeriesSelectorOutputTypeDef]
```

### Comparing `mypy-boto3-forecast-1.28.15.post1/mypy_boto3_forecast.egg-info/PKG-INFO` & `mypy-boto3-forecast-1.28.16/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,61 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-forecast
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.ForecastService 1.28.15 service generated with mypy-boto3-builder 7.16.2
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 forecast type-annotations boto3-stubs mypy typeshed autocomplete
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <a id="mypy-boto3-forecast"></a>
 
 # mypy-boto3-forecast
 
 [![PyPI - mypy-boto3-forecast](https://img.shields.io/pypi/v/mypy-boto3-forecast.svg?color=blue)](https://pypi.org/project/mypy-boto3-forecast)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-forecast.svg?color=blue)](https://pypi.org/project/mypy-boto3-forecast)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-forecast)](https://pepy.tech/project/mypy-boto3-forecast)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ForecastService 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService)
+[boto3.ForecastService 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService)
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
 [mypy-boto3-forecast docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/).
 
 See how it helps to find and fix potential bugs:
 
@@ -74,15 +42,15 @@
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
@@ -387,20 +355,20 @@
 )
 
 
 def check_value(value: AttributeTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_forecast.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_forecast.type_defs import (
     ActionTypeDef,
     AdditionalDatasetOutputTypeDef,
     AdditionalDatasetTypeDef,
     AttributeConfigOutputTypeDef,
@@ -547,14 +515,15 @@
     PredictorExecutionTypeDef,
     SchemaOutputTypeDef,
     SchemaTypeDef,
     TimeSeriesTransformationOutputTypeDef,
     TimeSeriesTransformationTypeDef,
     DescribeAutoPredictorResponseTypeDef,
     CreateAutoPredictorRequestRequestTypeDef,
+    DataConfigUnionTypeDef,
     BaselineTypeDef,
     ListExplainabilitiesResponseTypeDef,
     CreateExplainabilityExportRequestRequestTypeDef,
     CreateForecastExportJobRequestRequestTypeDef,
     CreatePredictorBacktestExportJobRequestRequestTypeDef,
     CreateWhatIfForecastExportRequestRequestTypeDef,
     DescribeExplainabilityExportResponseTypeDef,
@@ -567,49 +536,56 @@
     WhatIfForecastExportSummaryTypeDef,
     CreateDatasetImportJobRequestRequestTypeDef,
     DatasetImportJobSummaryTypeDef,
     DescribeDatasetImportJobResponseTypeDef,
     ListPredictorsResponseTypeDef,
     FeaturizationConfigOutputTypeDef,
     FeaturizationConfigTypeDef,
+    InputDataConfigUnionTypeDef,
     HyperParameterTuningJobConfigOutputTypeDef,
     HyperParameterTuningJobConfigTypeDef,
     WindowSummaryTypeDef,
     ListMonitorEvaluationsResponseTypeDef,
     PredictorExecutionDetailsTypeDef,
     DescribeDatasetResponseTypeDef,
     DescribeExplainabilityResponseTypeDef,
     TimeSeriesIdentifiersOutputTypeDef,
     TimeSeriesReplacementsDataSourceOutputTypeDef,
     CreateDatasetRequestRequestTypeDef,
     CreateExplainabilityRequestRequestTypeDef,
+    SchemaUnionTypeDef,
     TimeSeriesIdentifiersTypeDef,
     TimeSeriesReplacementsDataSourceTypeDef,
+    TimeSeriesTransformationUnionTypeDef,
     DescribeMonitorResponseTypeDef,
     ListExplainabilityExportsResponseTypeDef,
     ListForecastExportJobsResponseTypeDef,
     ListPredictorBacktestExportJobsResponseTypeDef,
     ListWhatIfForecastExportsResponseTypeDef,
     ListDatasetImportJobsResponseTypeDef,
+    FeaturizationConfigUnionTypeDef,
     CreatePredictorRequestRequestTypeDef,
+    HyperParameterTuningJobConfigUnionTypeDef,
     EvaluationResultTypeDef,
     DescribePredictorResponseTypeDef,
     TimeSeriesSelectorOutputTypeDef,
     DescribeWhatIfForecastResponseTypeDef,
     TimeSeriesSelectorTypeDef,
+    TimeSeriesReplacementsDataSourceUnionTypeDef,
     CreateWhatIfForecastRequestRequestTypeDef,
     GetAccuracyMetricsResponseTypeDef,
     DescribeForecastResponseTypeDef,
     DescribeWhatIfAnalysisResponseTypeDef,
     CreateForecastRequestRequestTypeDef,
     CreateWhatIfAnalysisRequestRequestTypeDef,
+    TimeSeriesSelectorUnionTypeDef,
 )
 
 
-def get_structure() -> ActionTypeDef:
+def get_value() -> ActionTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-forecast-1.28.15.post1/mypy_boto3_forecast.egg-info/SOURCES.txt` & `mypy-boto3-forecast-1.28.16/mypy_boto3_forecast.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-forecast-1.28.15.post1/setup.py` & `mypy-boto3-forecast-1.28.16/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-forecast",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_forecast"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ForecastService 1.28.15 service generated with"
-        " mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.ForecastService 1.28.16 service generated with"
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
-    keywords="boto3 forecast type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 forecast type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_forecast": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecast/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

