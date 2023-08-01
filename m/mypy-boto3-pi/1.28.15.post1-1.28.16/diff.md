# Comparing `tmp/mypy-boto3-pi-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-pi-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-pi-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:52 2023, max compression
+gzip compressed data, was "mypy-boto3-pi-1.28.16.tar", last modified: Tue Aug  1 11:37:32 2023, max compression
```

## Comparing `mypy-boto3-pi-1.28.15.post1.tar` & `mypy-boto3-pi-1.28.16.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:52.217334 mypy-boto3-pi-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:53:02.000000 mypy-boto3-pi-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12609 2023-07-29 10:03:52.205334 mypy-boto3-pi-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11136 2023-07-29 09:53:02.000000 mypy-boto3-pi-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:52.205334 mypy-boto3-pi-1.28.15.post1/mypy_boto3_pi/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-29 09:53:02.000000 mypy-boto3-pi-1.28.15.post1/mypy_boto3_pi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-29 09:53:02.000000 mypy-boto3-pi-1.28.15.post1/mypy_boto3_pi/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-29 09:53:02.000000 mypy-boto3-pi-1.28.15.post1/mypy_boto3_pi/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7738 2023-07-29 09:53:02.000000 mypy-boto3-pi-1.28.15.post1/mypy_boto3_pi/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-07-29 09:53:02.000000 mypy-boto3-pi-1.28.15.post1/mypy_boto3_pi/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8541 2023-07-29 09:53:02.000000 mypy-boto3-pi-1.28.15.post1/mypy_boto3_pi/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8539 2023-07-29 09:53:02.000000 mypy-boto3-pi-1.28.15.post1/mypy_boto3_pi/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:53:02.000000 mypy-boto3-pi-1.28.15.post1/mypy_boto3_pi/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    10480 2023-07-29 09:53:02.000000 mypy-boto3-pi-1.28.15.post1/mypy_boto3_pi/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    10463 2023-07-29 09:53:02.000000 mypy-boto3-pi-1.28.15.post1/mypy_boto3_pi/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:53:02.000000 mypy-boto3-pi-1.28.15.post1/mypy_boto3_pi/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:52.205334 mypy-boto3-pi-1.28.15.post1/mypy_boto3_pi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12609 2023-07-29 10:03:51.000000 mypy-boto3-pi-1.28.15.post1/mypy_boto3_pi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-29 10:03:51.000000 mypy-boto3-pi-1.28.15.post1/mypy_boto3_pi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:51.000000 mypy-boto3-pi-1.28.15.post1/mypy_boto3_pi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:51.000000 mypy-boto3-pi-1.28.15.post1/mypy_boto3_pi.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:51.000000 mypy-boto3-pi-1.28.15.post1/mypy_boto3_pi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-29 10:03:51.000000 mypy-boto3-pi-1.28.15.post1/mypy_boto3_pi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:52.217334 mypy-boto3-pi-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-07-29 09:53:02.000000 mypy-boto3-pi-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:32.344792 mypy-boto3-pi-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:26:04.000000 mypy-boto3-pi-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12621 2023-08-01 11:37:32.336791 mypy-boto3-pi-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11157 2023-08-01 11:26:04.000000 mypy-boto3-pi-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:32.336791 mypy-boto3-pi-1.28.16/mypy_boto3_pi/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-08-01 11:26:04.000000 mypy-boto3-pi-1.28.16/mypy_boto3_pi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-08-01 11:26:04.000000 mypy-boto3-pi-1.28.16/mypy_boto3_pi/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-08-01 11:26:04.000000 mypy-boto3-pi-1.28.16/mypy_boto3_pi/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7707 2023-08-01 11:26:04.000000 mypy-boto3-pi-1.28.16/mypy_boto3_pi/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7695 2023-08-01 11:26:04.000000 mypy-boto3-pi-1.28.16/mypy_boto3_pi/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8541 2023-08-01 11:26:04.000000 mypy-boto3-pi-1.28.16/mypy_boto3_pi/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8539 2023-08-01 11:26:04.000000 mypy-boto3-pi-1.28.16/mypy_boto3_pi/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:26:04.000000 mypy-boto3-pi-1.28.16/mypy_boto3_pi/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    10526 2023-08-01 11:26:05.000000 mypy-boto3-pi-1.28.16/mypy_boto3_pi/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10509 2023-08-01 11:26:05.000000 mypy-boto3-pi-1.28.16/mypy_boto3_pi/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:26:04.000000 mypy-boto3-pi-1.28.16/mypy_boto3_pi/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:32.336791 mypy-boto3-pi-1.28.16/mypy_boto3_pi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12621 2023-08-01 11:37:32.000000 mypy-boto3-pi-1.28.16/mypy_boto3_pi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-08-01 11:37:32.000000 mypy-boto3-pi-1.28.16/mypy_boto3_pi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:32.000000 mypy-boto3-pi-1.28.16/mypy_boto3_pi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:32.000000 mypy-boto3-pi-1.28.16/mypy_boto3_pi.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:32.000000 mypy-boto3-pi-1.28.16/mypy_boto3_pi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-01 11:37:32.000000 mypy-boto3-pi-1.28.16/mypy_boto3_pi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:32.344792 mypy-boto3-pi-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-08-01 11:26:04.000000 mypy-boto3-pi-1.28.16/setup.py
```

### Comparing `mypy-boto3-pi-1.28.15.post1/LICENSE` & `mypy-boto3-pi-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pi-1.28.15.post1/PKG-INFO` & `mypy-boto3-pi-1.28.16/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-pi
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.PI 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.PI 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pi/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 pi type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 pi type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-pi.svg?color=blue)](https://pypi.org/project/mypy-boto3-pi)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pi/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-pi)](https://pepy.tech/project/mypy-boto3-pi)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.PI 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI)
+[boto3.PI 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI)
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
 [mypy-boto3-pi docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pi/).
 
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
@@ -290,53 +290,54 @@
 )
 
 
 def check_value(value: DetailStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_pi.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_pi.type_defs import (
     DataPointTypeDef,
     DimensionGroupTypeDef,
+    TimestampTypeDef,
     DimensionKeyDescriptionTypeDef,
     ResponseMetadataTypeDef,
     ResponsePartitionKeyTypeDef,
     DimensionDetailTypeDef,
     DimensionKeyDetailTypeDef,
     FeatureMetadataTypeDef,
     GetDimensionKeyDetailsRequestRequestTypeDef,
     GetResourceMetadataRequestRequestTypeDef,
     ListAvailableResourceDimensionsRequestRequestTypeDef,
     ListAvailableResourceMetricsRequestRequestTypeDef,
     ResponseResourceMetricTypeDef,
     ResponseResourceMetricKeyTypeDef,
-    DescribeDimensionKeysRequestRequestTypeDef,
     MetricQueryTypeDef,
+    DescribeDimensionKeysRequestRequestTypeDef,
     DescribeDimensionKeysResponseTypeDef,
     DimensionGroupDetailTypeDef,
     GetDimensionKeyDetailsResponseTypeDef,
     GetResourceMetadataResponseTypeDef,
     ListAvailableResourceMetricsResponseTypeDef,
     MetricKeyDataPointsTypeDef,
     GetResourceMetricsRequestRequestTypeDef,
     MetricDimensionGroupsTypeDef,
     GetResourceMetricsResponseTypeDef,
     ListAvailableResourceDimensionsResponseTypeDef,
 )
 
 
-def get_structure() -> DataPointTypeDef:
+def get_value() -> DataPointTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-pi-1.28.15.post1/README.md` & `mypy-boto3-pi-1.28.16/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-pi.svg?color=blue)](https://pypi.org/project/mypy-boto3-pi)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pi/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-pi)](https://pepy.tech/project/mypy-boto3-pi)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.PI 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI)
+[boto3.PI 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI)
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
 [mypy-boto3-pi docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pi/).
 
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
@@ -258,53 +258,54 @@
 )
 
 
 def check_value(value: DetailStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_pi.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_pi.type_defs import (
     DataPointTypeDef,
     DimensionGroupTypeDef,
+    TimestampTypeDef,
     DimensionKeyDescriptionTypeDef,
     ResponseMetadataTypeDef,
     ResponsePartitionKeyTypeDef,
     DimensionDetailTypeDef,
     DimensionKeyDetailTypeDef,
     FeatureMetadataTypeDef,
     GetDimensionKeyDetailsRequestRequestTypeDef,
     GetResourceMetadataRequestRequestTypeDef,
     ListAvailableResourceDimensionsRequestRequestTypeDef,
     ListAvailableResourceMetricsRequestRequestTypeDef,
     ResponseResourceMetricTypeDef,
     ResponseResourceMetricKeyTypeDef,
-    DescribeDimensionKeysRequestRequestTypeDef,
     MetricQueryTypeDef,
+    DescribeDimensionKeysRequestRequestTypeDef,
     DescribeDimensionKeysResponseTypeDef,
     DimensionGroupDetailTypeDef,
     GetDimensionKeyDetailsResponseTypeDef,
     GetResourceMetadataResponseTypeDef,
     ListAvailableResourceMetricsResponseTypeDef,
     MetricKeyDataPointsTypeDef,
     GetResourceMetricsRequestRequestTypeDef,
     MetricDimensionGroupsTypeDef,
     GetResourceMetricsResponseTypeDef,
     ListAvailableResourceDimensionsResponseTypeDef,
 )
 
 
-def get_structure() -> DataPointTypeDef:
+def get_value() -> DataPointTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-pi-1.28.15.post1/mypy_boto3_pi/__main__.py` & `mypy-boto3-pi-1.28.16/mypy_boto3_pi/__main__.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.PI 1.28.15\nVersion:         1.28.15.post1\nBuilder version:"
-        " 7.16.2\nDocs:           "
+        "Type annotations for boto3.PI 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pi//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI\nOther"
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

### Comparing `mypy-boto3-pi-1.28.15.post1/mypy_boto3_pi/client.py` & `mypy-boto3-pi-1.28.16/mypy_boto3_pi/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,29 +9,29 @@
     from boto3.session import Session
     from mypy_boto3_pi.client import PIClient
 
     session = Session()
     client: PIClient = session.client("pi")
     ```
 """
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import PeriodAlignmentType, ServiceTypeType
 from .type_defs import (
     DescribeDimensionKeysResponseTypeDef,
     DimensionGroupTypeDef,
     GetDimensionKeyDetailsResponseTypeDef,
     GetResourceMetadataResponseTypeDef,
     GetResourceMetricsResponseTypeDef,
     ListAvailableResourceDimensionsResponseTypeDef,
     ListAvailableResourceMetricsResponseTypeDef,
     MetricQueryTypeDef,
+    TimestampTypeDef,
 )
 
 __all__ = ("PIClient",)
 
 
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
@@ -82,16 +82,16 @@
         """
 
     def describe_dimension_keys(
         self,
         *,
         ServiceType: ServiceTypeType,
         Identifier: str,
-        StartTime: Union[datetime, str],
-        EndTime: Union[datetime, str],
+        StartTime: TimestampTypeDef,
+        EndTime: TimestampTypeDef,
         Metric: str,
         GroupBy: DimensionGroupTypeDef,
         PeriodInSeconds: int = ...,
         AdditionalMetrics: Sequence[str] = ...,
         PartitionBy: DimensionGroupTypeDef = ...,
         Filter: Mapping[str, str] = ...,
         MaxResults: int = ...,
@@ -147,16 +147,16 @@
 
     def get_resource_metrics(
         self,
         *,
         ServiceType: ServiceTypeType,
         Identifier: str,
         MetricQueries: Sequence[MetricQueryTypeDef],
-        StartTime: Union[datetime, str],
-        EndTime: Union[datetime, str],
+        StartTime: TimestampTypeDef,
+        EndTime: TimestampTypeDef,
         PeriodInSeconds: int = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
         PeriodAlignment: PeriodAlignmentType = ...
     ) -> GetResourceMetricsResponseTypeDef:
         """
         Retrieve Performance Insights metrics for a set of data sources over a time
```

### Comparing `mypy-boto3-pi-1.28.15.post1/mypy_boto3_pi/client.pyi` & `mypy-boto3-pi-1.28.16/mypy_boto3_pi/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -9,29 +9,29 @@
     from boto3.session import Session
     from mypy_boto3_pi.client import PIClient
 
     session = Session()
     client: PIClient = session.client("pi")
     ```
 """
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import PeriodAlignmentType, ServiceTypeType
 from .type_defs import (
     DescribeDimensionKeysResponseTypeDef,
     DimensionGroupTypeDef,
     GetDimensionKeyDetailsResponseTypeDef,
     GetResourceMetadataResponseTypeDef,
     GetResourceMetricsResponseTypeDef,
     ListAvailableResourceDimensionsResponseTypeDef,
     ListAvailableResourceMetricsResponseTypeDef,
     MetricQueryTypeDef,
+    TimestampTypeDef,
 )
 
 __all__ = ("PIClient",)
 
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
@@ -76,16 +76,16 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pi/client/#close)
         """
     def describe_dimension_keys(
         self,
         *,
         ServiceType: ServiceTypeType,
         Identifier: str,
-        StartTime: Union[datetime, str],
-        EndTime: Union[datetime, str],
+        StartTime: TimestampTypeDef,
+        EndTime: TimestampTypeDef,
         Metric: str,
         GroupBy: DimensionGroupTypeDef,
         PeriodInSeconds: int = ...,
         AdditionalMetrics: Sequence[str] = ...,
         PartitionBy: DimensionGroupTypeDef = ...,
         Filter: Mapping[str, str] = ...,
         MaxResults: int = ...,
@@ -137,16 +137,16 @@
         """
     def get_resource_metrics(
         self,
         *,
         ServiceType: ServiceTypeType,
         Identifier: str,
         MetricQueries: Sequence[MetricQueryTypeDef],
-        StartTime: Union[datetime, str],
-        EndTime: Union[datetime, str],
+        StartTime: TimestampTypeDef,
+        EndTime: TimestampTypeDef,
         PeriodInSeconds: int = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
         PeriodAlignment: PeriodAlignmentType = ...
     ) -> GetResourceMetricsResponseTypeDef:
         """
         Retrieve Performance Insights metrics for a set of data sources over a time
```

### Comparing `mypy-boto3-pi-1.28.15.post1/mypy_boto3_pi/literals.py` & `mypy-boto3-pi-1.28.16/mypy_boto3_pi/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pi-1.28.15.post1/mypy_boto3_pi/literals.pyi` & `mypy-boto3-pi-1.28.16/mypy_boto3_pi/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pi-1.28.15.post1/mypy_boto3_pi/type_defs.py` & `mypy-boto3-pi-1.28.16/mypy_boto3_pi/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,46 +4,46 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pi/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_pi.type_defs import DataPointTypeDef
 
-    data: DataPointTypeDef = {...}
+    data: DataPointTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import DetailStatusType, FeatureStatusType, PeriodAlignmentType, ServiceTypeType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "DataPointTypeDef",
     "DimensionGroupTypeDef",
+    "TimestampTypeDef",
     "DimensionKeyDescriptionTypeDef",
     "ResponseMetadataTypeDef",
     "ResponsePartitionKeyTypeDef",
     "DimensionDetailTypeDef",
     "DimensionKeyDetailTypeDef",
     "FeatureMetadataTypeDef",
     "GetDimensionKeyDetailsRequestRequestTypeDef",
     "GetResourceMetadataRequestRequestTypeDef",
     "ListAvailableResourceDimensionsRequestRequestTypeDef",
     "ListAvailableResourceMetricsRequestRequestTypeDef",
     "ResponseResourceMetricTypeDef",
     "ResponseResourceMetricKeyTypeDef",
-    "DescribeDimensionKeysRequestRequestTypeDef",
     "MetricQueryTypeDef",
+    "DescribeDimensionKeysRequestRequestTypeDef",
     "DescribeDimensionKeysResponseTypeDef",
     "DimensionGroupDetailTypeDef",
     "GetDimensionKeyDetailsResponseTypeDef",
     "GetResourceMetadataResponseTypeDef",
     "ListAvailableResourceMetricsResponseTypeDef",
     "MetricKeyDataPointsTypeDef",
     "GetResourceMetricsRequestRequestTypeDef",
@@ -71,19 +71,18 @@
     {
         "Dimensions": Sequence[str],
         "Limit": int,
     },
     total=False,
 )
 
-
 class DimensionGroupTypeDef(_RequiredDimensionGroupTypeDef, _OptionalDimensionGroupTypeDef):
     pass
 
-
+TimestampTypeDef = Union[datetime, str]
 DimensionKeyDescriptionTypeDef = TypedDict(
     "DimensionKeyDescriptionTypeDef",
     {
         "Dimensions": Dict[str, str],
         "Total": float,
         "AdditionalMetrics": Dict[str, float],
         "Partitions": List[float],
@@ -148,22 +147,20 @@
     "_OptionalGetDimensionKeyDetailsRequestRequestTypeDef",
     {
         "RequestedDimensions": Sequence[str],
     },
     total=False,
 )
 
-
 class GetDimensionKeyDetailsRequestRequestTypeDef(
     _RequiredGetDimensionKeyDetailsRequestRequestTypeDef,
     _OptionalGetDimensionKeyDetailsRequestRequestTypeDef,
 ):
     pass
 
-
 GetResourceMetadataRequestRequestTypeDef = TypedDict(
     "GetResourceMetadataRequestRequestTypeDef",
     {
         "ServiceType": ServiceTypeType,
         "Identifier": str,
     },
 )
@@ -181,22 +178,20 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListAvailableResourceDimensionsRequestRequestTypeDef(
     _RequiredListAvailableResourceDimensionsRequestRequestTypeDef,
     _OptionalListAvailableResourceDimensionsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListAvailableResourceMetricsRequestRequestTypeDef = TypedDict(
     "_RequiredListAvailableResourceMetricsRequestRequestTypeDef",
     {
         "ServiceType": ServiceTypeType,
         "Identifier": str,
         "MetricTypes": Sequence[str],
     },
@@ -206,22 +201,20 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListAvailableResourceMetricsRequestRequestTypeDef(
     _RequiredListAvailableResourceMetricsRequestRequestTypeDef,
     _OptionalListAvailableResourceMetricsRequestRequestTypeDef,
 ):
     pass
 
-
 ResponseResourceMetricTypeDef = TypedDict(
     "ResponseResourceMetricTypeDef",
     {
         "Metric": str,
         "Description": str,
         "Unit": str,
     },
@@ -238,28 +231,44 @@
     "_OptionalResponseResourceMetricKeyTypeDef",
     {
         "Dimensions": Dict[str, str],
     },
     total=False,
 )
 
-
 class ResponseResourceMetricKeyTypeDef(
     _RequiredResponseResourceMetricKeyTypeDef, _OptionalResponseResourceMetricKeyTypeDef
 ):
     pass
 
+_RequiredMetricQueryTypeDef = TypedDict(
+    "_RequiredMetricQueryTypeDef",
+    {
+        "Metric": str,
+    },
+)
+_OptionalMetricQueryTypeDef = TypedDict(
+    "_OptionalMetricQueryTypeDef",
+    {
+        "GroupBy": DimensionGroupTypeDef,
+        "Filter": Mapping[str, str],
+    },
+    total=False,
+)
+
+class MetricQueryTypeDef(_RequiredMetricQueryTypeDef, _OptionalMetricQueryTypeDef):
+    pass
 
 _RequiredDescribeDimensionKeysRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeDimensionKeysRequestRequestTypeDef",
     {
         "ServiceType": ServiceTypeType,
         "Identifier": str,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
         "Metric": str,
         "GroupBy": DimensionGroupTypeDef,
     },
 )
 _OptionalDescribeDimensionKeysRequestRequestTypeDef = TypedDict(
     "_OptionalDescribeDimensionKeysRequestRequestTypeDef",
     {
@@ -269,42 +278,20 @@
         "Filter": Mapping[str, str],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribeDimensionKeysRequestRequestTypeDef(
     _RequiredDescribeDimensionKeysRequestRequestTypeDef,
     _OptionalDescribeDimensionKeysRequestRequestTypeDef,
 ):
     pass
 
-
-_RequiredMetricQueryTypeDef = TypedDict(
-    "_RequiredMetricQueryTypeDef",
-    {
-        "Metric": str,
-    },
-)
-_OptionalMetricQueryTypeDef = TypedDict(
-    "_OptionalMetricQueryTypeDef",
-    {
-        "GroupBy": DimensionGroupTypeDef,
-        "Filter": Mapping[str, str],
-    },
-    total=False,
-)
-
-
-class MetricQueryTypeDef(_RequiredMetricQueryTypeDef, _OptionalMetricQueryTypeDef):
-    pass
-
-
 DescribeDimensionKeysResponseTypeDef = TypedDict(
     "DescribeDimensionKeysResponseTypeDef",
     {
         "AlignedStartTime": datetime,
         "AlignedEndTime": datetime,
         "PartitionKeys": List[ResponsePartitionKeyTypeDef],
         "Keys": List[DimensionKeyDescriptionTypeDef],
@@ -359,37 +346,35 @@
 
 _RequiredGetResourceMetricsRequestRequestTypeDef = TypedDict(
     "_RequiredGetResourceMetricsRequestRequestTypeDef",
     {
         "ServiceType": ServiceTypeType,
         "Identifier": str,
         "MetricQueries": Sequence[MetricQueryTypeDef],
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
     },
 )
 _OptionalGetResourceMetricsRequestRequestTypeDef = TypedDict(
     "_OptionalGetResourceMetricsRequestRequestTypeDef",
     {
         "PeriodInSeconds": int,
         "MaxResults": int,
         "NextToken": str,
         "PeriodAlignment": PeriodAlignmentType,
     },
     total=False,
 )
 
-
 class GetResourceMetricsRequestRequestTypeDef(
     _RequiredGetResourceMetricsRequestRequestTypeDef,
     _OptionalGetResourceMetricsRequestRequestTypeDef,
 ):
     pass
 
-
 MetricDimensionGroupsTypeDef = TypedDict(
     "MetricDimensionGroupsTypeDef",
     {
         "Metric": str,
         "Groups": List[DimensionGroupDetailTypeDef],
     },
     total=False,
```

### Comparing `mypy-boto3-pi-1.28.15.post1/mypy_boto3_pi/type_defs.pyi` & `mypy-boto3-pi-1.28.16/mypy_boto3_pi/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,45 +4,47 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pi/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_pi.type_defs import DataPointTypeDef
 
-    data: DataPointTypeDef = {...}
+    data: DataPointTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import DetailStatusType, FeatureStatusType, PeriodAlignmentType, ServiceTypeType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "DataPointTypeDef",
     "DimensionGroupTypeDef",
+    "TimestampTypeDef",
     "DimensionKeyDescriptionTypeDef",
     "ResponseMetadataTypeDef",
     "ResponsePartitionKeyTypeDef",
     "DimensionDetailTypeDef",
     "DimensionKeyDetailTypeDef",
     "FeatureMetadataTypeDef",
     "GetDimensionKeyDetailsRequestRequestTypeDef",
     "GetResourceMetadataRequestRequestTypeDef",
     "ListAvailableResourceDimensionsRequestRequestTypeDef",
     "ListAvailableResourceMetricsRequestRequestTypeDef",
     "ResponseResourceMetricTypeDef",
     "ResponseResourceMetricKeyTypeDef",
-    "DescribeDimensionKeysRequestRequestTypeDef",
     "MetricQueryTypeDef",
+    "DescribeDimensionKeysRequestRequestTypeDef",
     "DescribeDimensionKeysResponseTypeDef",
     "DimensionGroupDetailTypeDef",
     "GetDimensionKeyDetailsResponseTypeDef",
     "GetResourceMetadataResponseTypeDef",
     "ListAvailableResourceMetricsResponseTypeDef",
     "MetricKeyDataPointsTypeDef",
     "GetResourceMetricsRequestRequestTypeDef",
@@ -70,17 +72,20 @@
     {
         "Dimensions": Sequence[str],
         "Limit": int,
     },
     total=False,
 )
 
+
 class DimensionGroupTypeDef(_RequiredDimensionGroupTypeDef, _OptionalDimensionGroupTypeDef):
     pass
 
+
+TimestampTypeDef = Union[datetime, str]
 DimensionKeyDescriptionTypeDef = TypedDict(
     "DimensionKeyDescriptionTypeDef",
     {
         "Dimensions": Dict[str, str],
         "Total": float,
         "AdditionalMetrics": Dict[str, float],
         "Partitions": List[float],
@@ -145,20 +150,22 @@
     "_OptionalGetDimensionKeyDetailsRequestRequestTypeDef",
     {
         "RequestedDimensions": Sequence[str],
     },
     total=False,
 )
 
+
 class GetDimensionKeyDetailsRequestRequestTypeDef(
     _RequiredGetDimensionKeyDetailsRequestRequestTypeDef,
     _OptionalGetDimensionKeyDetailsRequestRequestTypeDef,
 ):
     pass
 
+
 GetResourceMetadataRequestRequestTypeDef = TypedDict(
     "GetResourceMetadataRequestRequestTypeDef",
     {
         "ServiceType": ServiceTypeType,
         "Identifier": str,
     },
 )
@@ -176,20 +183,22 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListAvailableResourceDimensionsRequestRequestTypeDef(
     _RequiredListAvailableResourceDimensionsRequestRequestTypeDef,
     _OptionalListAvailableResourceDimensionsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListAvailableResourceMetricsRequestRequestTypeDef = TypedDict(
     "_RequiredListAvailableResourceMetricsRequestRequestTypeDef",
     {
         "ServiceType": ServiceTypeType,
         "Identifier": str,
         "MetricTypes": Sequence[str],
     },
@@ -199,20 +208,22 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListAvailableResourceMetricsRequestRequestTypeDef(
     _RequiredListAvailableResourceMetricsRequestRequestTypeDef,
     _OptionalListAvailableResourceMetricsRequestRequestTypeDef,
 ):
     pass
 
+
 ResponseResourceMetricTypeDef = TypedDict(
     "ResponseResourceMetricTypeDef",
     {
         "Metric": str,
         "Description": str,
         "Unit": str,
     },
@@ -229,26 +240,48 @@
     "_OptionalResponseResourceMetricKeyTypeDef",
     {
         "Dimensions": Dict[str, str],
     },
     total=False,
 )
 
+
 class ResponseResourceMetricKeyTypeDef(
     _RequiredResponseResourceMetricKeyTypeDef, _OptionalResponseResourceMetricKeyTypeDef
 ):
     pass
 
+
+_RequiredMetricQueryTypeDef = TypedDict(
+    "_RequiredMetricQueryTypeDef",
+    {
+        "Metric": str,
+    },
+)
+_OptionalMetricQueryTypeDef = TypedDict(
+    "_OptionalMetricQueryTypeDef",
+    {
+        "GroupBy": DimensionGroupTypeDef,
+        "Filter": Mapping[str, str],
+    },
+    total=False,
+)
+
+
+class MetricQueryTypeDef(_RequiredMetricQueryTypeDef, _OptionalMetricQueryTypeDef):
+    pass
+
+
 _RequiredDescribeDimensionKeysRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeDimensionKeysRequestRequestTypeDef",
     {
         "ServiceType": ServiceTypeType,
         "Identifier": str,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
         "Metric": str,
         "GroupBy": DimensionGroupTypeDef,
     },
 )
 _OptionalDescribeDimensionKeysRequestRequestTypeDef = TypedDict(
     "_OptionalDescribeDimensionKeysRequestRequestTypeDef",
     {
@@ -258,37 +291,21 @@
         "Filter": Mapping[str, str],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribeDimensionKeysRequestRequestTypeDef(
     _RequiredDescribeDimensionKeysRequestRequestTypeDef,
     _OptionalDescribeDimensionKeysRequestRequestTypeDef,
 ):
     pass
 
-_RequiredMetricQueryTypeDef = TypedDict(
-    "_RequiredMetricQueryTypeDef",
-    {
-        "Metric": str,
-    },
-)
-_OptionalMetricQueryTypeDef = TypedDict(
-    "_OptionalMetricQueryTypeDef",
-    {
-        "GroupBy": DimensionGroupTypeDef,
-        "Filter": Mapping[str, str],
-    },
-    total=False,
-)
-
-class MetricQueryTypeDef(_RequiredMetricQueryTypeDef, _OptionalMetricQueryTypeDef):
-    pass
 
 DescribeDimensionKeysResponseTypeDef = TypedDict(
     "DescribeDimensionKeysResponseTypeDef",
     {
         "AlignedStartTime": datetime,
         "AlignedEndTime": datetime,
         "PartitionKeys": List[ResponsePartitionKeyTypeDef],
@@ -344,35 +361,37 @@
 
 _RequiredGetResourceMetricsRequestRequestTypeDef = TypedDict(
     "_RequiredGetResourceMetricsRequestRequestTypeDef",
     {
         "ServiceType": ServiceTypeType,
         "Identifier": str,
         "MetricQueries": Sequence[MetricQueryTypeDef],
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
     },
 )
 _OptionalGetResourceMetricsRequestRequestTypeDef = TypedDict(
     "_OptionalGetResourceMetricsRequestRequestTypeDef",
     {
         "PeriodInSeconds": int,
         "MaxResults": int,
         "NextToken": str,
         "PeriodAlignment": PeriodAlignmentType,
     },
     total=False,
 )
 
+
 class GetResourceMetricsRequestRequestTypeDef(
     _RequiredGetResourceMetricsRequestRequestTypeDef,
     _OptionalGetResourceMetricsRequestRequestTypeDef,
 ):
     pass
 
+
 MetricDimensionGroupsTypeDef = TypedDict(
     "MetricDimensionGroupsTypeDef",
     {
         "Metric": str,
         "Groups": List[DimensionGroupDetailTypeDef],
     },
     total=False,
```

### Comparing `mypy-boto3-pi-1.28.15.post1/mypy_boto3_pi.egg-info/PKG-INFO` & `mypy-boto3-pi-1.28.16/mypy_boto3_pi.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-pi
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.PI 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.PI 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pi/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 pi type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 pi type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-pi.svg?color=blue)](https://pypi.org/project/mypy-boto3-pi)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pi/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-pi)](https://pepy.tech/project/mypy-boto3-pi)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.PI 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI)
+[boto3.PI 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI)
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
 [mypy-boto3-pi docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pi/).
 
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
@@ -290,53 +290,54 @@
 )
 
 
 def check_value(value: DetailStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_pi.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_pi.type_defs import (
     DataPointTypeDef,
     DimensionGroupTypeDef,
+    TimestampTypeDef,
     DimensionKeyDescriptionTypeDef,
     ResponseMetadataTypeDef,
     ResponsePartitionKeyTypeDef,
     DimensionDetailTypeDef,
     DimensionKeyDetailTypeDef,
     FeatureMetadataTypeDef,
     GetDimensionKeyDetailsRequestRequestTypeDef,
     GetResourceMetadataRequestRequestTypeDef,
     ListAvailableResourceDimensionsRequestRequestTypeDef,
     ListAvailableResourceMetricsRequestRequestTypeDef,
     ResponseResourceMetricTypeDef,
     ResponseResourceMetricKeyTypeDef,
-    DescribeDimensionKeysRequestRequestTypeDef,
     MetricQueryTypeDef,
+    DescribeDimensionKeysRequestRequestTypeDef,
     DescribeDimensionKeysResponseTypeDef,
     DimensionGroupDetailTypeDef,
     GetDimensionKeyDetailsResponseTypeDef,
     GetResourceMetadataResponseTypeDef,
     ListAvailableResourceMetricsResponseTypeDef,
     MetricKeyDataPointsTypeDef,
     GetResourceMetricsRequestRequestTypeDef,
     MetricDimensionGroupsTypeDef,
     GetResourceMetricsResponseTypeDef,
     ListAvailableResourceDimensionsResponseTypeDef,
 )
 
 
-def get_structure() -> DataPointTypeDef:
+def get_value() -> DataPointTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-pi-1.28.15.post1/mypy_boto3_pi.egg-info/SOURCES.txt` & `mypy-boto3-pi-1.28.16/mypy_boto3_pi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pi-1.28.15.post1/setup.py` & `mypy-boto3-pi-1.28.16/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-pi",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_pi"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.PI 1.28.15 service generated with mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.PI 1.28.16 service generated with mypy-boto3-builder 7.17.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
@@ -33,15 +33,15 @@
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
         "Typing :: Typed",
     ],
-    keywords="boto3 pi type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 pi type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_pi": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pi/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

