# Comparing `tmp/mypy-boto3-location-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-location-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-location-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:33 2023, max compression
+gzip compressed data, was "mypy-boto3-location-1.28.16.tar", last modified: Tue Aug  1 11:37:13 2023, max compression
```

## Comparing `mypy-boto3-location-1.28.15.post1.tar` & `mypy-boto3-location-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:33.761251 mypy-boto3-location-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:50:00.000000 mypy-boto3-location-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21143 2023-07-29 10:03:33.757251 mypy-boto3-location-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19639 2023-07-29 09:50:00.000000 mypy-boto3-location-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:33.757251 mypy-boto3-location-1.28.15.post1/mypy_boto3_location/
--rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-07-29 09:50:00.000000 mypy-boto3-location-1.28.15.post1/mypy_boto3_location/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-07-29 09:50:00.000000 mypy-boto3-location-1.28.15.post1/mypy_boto3_location/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-29 09:50:00.000000 mypy-boto3-location-1.28.15.post1/mypy_boto3_location/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    45733 2023-07-29 09:50:03.000000 mypy-boto3-location-1.28.15.post1/mypy_boto3_location/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    45658 2023-07-29 09:50:00.000000 mypy-boto3-location-1.28.15.post1/mypy_boto3_location/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10356 2023-07-29 09:50:03.000000 mypy-boto3-location-1.28.15.post1/mypy_boto3_location/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10354 2023-07-29 09:50:03.000000 mypy-boto3-location-1.28.15.post1/mypy_boto3_location/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11790 2023-07-29 09:50:03.000000 mypy-boto3-location-1.28.15.post1/mypy_boto3_location/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11778 2023-07-29 09:50:03.000000 mypy-boto3-location-1.28.15.post1/mypy_boto3_location/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:50:00.000000 mypy-boto3-location-1.28.15.post1/mypy_boto3_location/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    65922 2023-07-29 09:50:05.000000 mypy-boto3-location-1.28.15.post1/mypy_boto3_location/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    65809 2023-07-29 09:50:04.000000 mypy-boto3-location-1.28.15.post1/mypy_boto3_location/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:50:00.000000 mypy-boto3-location-1.28.15.post1/mypy_boto3_location/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:33.757251 mypy-boto3-location-1.28.15.post1/mypy_boto3_location.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21143 2023-07-29 10:03:33.000000 mypy-boto3-location-1.28.15.post1/mypy_boto3_location.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-29 10:03:33.000000 mypy-boto3-location-1.28.15.post1/mypy_boto3_location.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:33.000000 mypy-boto3-location-1.28.15.post1/mypy_boto3_location.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:33.000000 mypy-boto3-location-1.28.15.post1/mypy_boto3_location.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:33.000000 mypy-boto3-location-1.28.15.post1/mypy_boto3_location.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-29 10:03:33.000000 mypy-boto3-location-1.28.15.post1/mypy_boto3_location.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:33.761251 mypy-boto3-location-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-07-29 09:50:00.000000 mypy-boto3-location-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:13.624837 mypy-boto3-location-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:22:53.000000 mypy-boto3-location-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21225 2023-08-01 11:37:13.616837 mypy-boto3-location-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19730 2023-08-01 11:22:53.000000 mypy-boto3-location-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:13.604837 mypy-boto3-location-1.28.16/mypy_boto3_location/
+-rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-08-01 11:22:53.000000 mypy-boto3-location-1.28.16/mypy_boto3_location/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-08-01 11:22:53.000000 mypy-boto3-location-1.28.16/mypy_boto3_location/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-08-01 11:22:53.000000 mypy-boto3-location-1.28.16/mypy_boto3_location/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45529 2023-08-01 11:22:53.000000 mypy-boto3-location-1.28.16/mypy_boto3_location/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45454 2023-08-01 11:22:53.000000 mypy-boto3-location-1.28.16/mypy_boto3_location/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10356 2023-08-01 11:22:53.000000 mypy-boto3-location-1.28.16/mypy_boto3_location/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10354 2023-08-01 11:22:53.000000 mypy-boto3-location-1.28.16/mypy_boto3_location/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11767 2023-08-01 11:22:53.000000 mypy-boto3-location-1.28.16/mypy_boto3_location/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11755 2023-08-01 11:22:53.000000 mypy-boto3-location-1.28.16/mypy_boto3_location/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:22:53.000000 mypy-boto3-location-1.28.16/mypy_boto3_location/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    66214 2023-08-01 11:22:55.000000 mypy-boto3-location-1.28.16/mypy_boto3_location/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66101 2023-08-01 11:22:54.000000 mypy-boto3-location-1.28.16/mypy_boto3_location/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:22:53.000000 mypy-boto3-location-1.28.16/mypy_boto3_location/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:13.616837 mypy-boto3-location-1.28.16/mypy_boto3_location.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21225 2023-08-01 11:37:13.000000 mypy-boto3-location-1.28.16/mypy_boto3_location.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-08-01 11:37:13.000000 mypy-boto3-location-1.28.16/mypy_boto3_location.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:13.000000 mypy-boto3-location-1.28.16/mypy_boto3_location.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:13.000000 mypy-boto3-location-1.28.16/mypy_boto3_location.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:13.000000 mypy-boto3-location-1.28.16/mypy_boto3_location.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-01 11:37:13.000000 mypy-boto3-location-1.28.16/mypy_boto3_location.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:13.624837 mypy-boto3-location-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-08-01 11:22:52.000000 mypy-boto3-location-1.28.16/setup.py
```

### Comparing `mypy-boto3-location-1.28.15.post1/LICENSE` & `mypy-boto3-location-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-location-1.28.15.post1/PKG-INFO` & `mypy-boto3-location-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-location
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.LocationService 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.LocationService 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 location type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 location type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-location.svg?color=blue)](https://pypi.org/project/mypy-boto3-location)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-location)](https://pepy.tech/project/mypy-boto3-location)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LocationService 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService)
+[boto3.LocationService 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService)
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
 [mypy-boto3-location docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/).
 
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
@@ -358,34 +358,35 @@
 )
 
 
 def check_value(value: BatchItemErrorCodeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_location.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_location.type_defs import (
     ApiKeyFilterTypeDef,
     ApiKeyRestrictionsOutputTypeDef,
     ApiKeyRestrictionsTypeDef,
     AssociateTrackerConsumerRequestRequestTypeDef,
     BatchItemErrorTypeDef,
     BatchDeleteDevicePositionHistoryRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     BatchDeleteGeofenceRequestRequestTypeDef,
     BatchGetDevicePositionRequestRequestTypeDef,
     BatchPutGeofenceSuccessTypeDef,
     CalculateRouteCarModeOptionsTypeDef,
+    TimestampTypeDef,
     CalculateRouteMatrixSummaryTypeDef,
     CalculateRouteSummaryTypeDef,
     TruckDimensionsTypeDef,
     TruckWeightTypeDef,
     CircleOutputTypeDef,
     CircleTypeDef,
     CreateGeofenceCollectionRequestRequestTypeDef,
@@ -404,15 +405,14 @@
     DescribeMapRequestRequestTypeDef,
     DescribePlaceIndexRequestRequestTypeDef,
     DescribeRouteCalculatorRequestRequestTypeDef,
     DescribeTrackerRequestRequestTypeDef,
     PositionalAccuracyTypeDef,
     DisassociateTrackerConsumerRequestRequestTypeDef,
     PaginatorConfigTypeDef,
-    GetDevicePositionHistoryRequestRequestTypeDef,
     GetDevicePositionRequestRequestTypeDef,
     GetGeofenceRequestRequestTypeDef,
     GetMapGlyphsRequestRequestTypeDef,
     GetMapSpritesRequestRequestTypeDef,
     GetMapStyleDescriptorRequestRequestTypeDef,
     GetMapTileRequestRequestTypeDef,
     GetPlaceRequestRequestTypeDef,
@@ -446,16 +446,15 @@
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateGeofenceCollectionRequestRequestTypeDef,
     UpdateRouteCalculatorRequestRequestTypeDef,
     UpdateTrackerRequestRequestTypeDef,
     ListKeysRequestRequestTypeDef,
     ListKeysResponseEntryTypeDef,
-    CreateKeyRequestRequestTypeDef,
-    UpdateKeyRequestRequestTypeDef,
+    ApiKeyRestrictionsUnionTypeDef,
     BatchDeleteDevicePositionHistoryErrorTypeDef,
     BatchDeleteGeofenceErrorTypeDef,
     BatchEvaluateGeofencesErrorTypeDef,
     BatchGetDevicePositionErrorTypeDef,
     BatchPutGeofenceErrorTypeDef,
     BatchUpdateDevicePositionErrorTypeDef,
     CreateGeofenceCollectionResponseTypeDef,
@@ -477,14 +476,17 @@
     PutGeofenceResponseTypeDef,
     UpdateGeofenceCollectionResponseTypeDef,
     UpdateKeyResponseTypeDef,
     UpdateMapResponseTypeDef,
     UpdatePlaceIndexResponseTypeDef,
     UpdateRouteCalculatorResponseTypeDef,
     UpdateTrackerResponseTypeDef,
+    CreateKeyRequestRequestTypeDef,
+    GetDevicePositionHistoryRequestRequestTypeDef,
+    UpdateKeyRequestRequestTypeDef,
     CalculateRouteTruckModeOptionsTypeDef,
     GeofenceGeometryOutputTypeDef,
     GeofenceGeometryTypeDef,
     CreateMapRequestRequestTypeDef,
     DescribeMapResponseTypeDef,
     CreatePlaceIndexRequestRequestTypeDef,
     DescribePlaceIndexResponseTypeDef,
@@ -520,14 +522,15 @@
     BatchPutGeofenceResponseTypeDef,
     BatchUpdateDevicePositionResponseTypeDef,
     CalculateRouteMatrixRequestRequestTypeDef,
     CalculateRouteRequestRequestTypeDef,
     GetGeofenceResponseTypeDef,
     ListGeofenceResponseEntryTypeDef,
     BatchPutGeofenceRequestEntryTypeDef,
+    GeofenceGeometryUnionTypeDef,
     PutGeofenceRequestRequestTypeDef,
     BatchGetDevicePositionResponseTypeDef,
     GetDevicePositionHistoryResponseTypeDef,
     BatchEvaluateGeofencesRequestRequestTypeDef,
     BatchUpdateDevicePositionRequestRequestTypeDef,
     ListDevicePositionsResponseTypeDef,
     CalculateRouteResponseTypeDef,
@@ -538,15 +541,15 @@
     ListGeofencesResponseTypeDef,
     BatchPutGeofenceRequestRequestTypeDef,
     SearchPlaceIndexForPositionResponseTypeDef,
     SearchPlaceIndexForTextResponseTypeDef,
 )
 
 
-def get_structure() -> ApiKeyFilterTypeDef:
+def get_value() -> ApiKeyFilterTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-location-1.28.15.post1/README.md` & `mypy-boto3-location-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-location.svg?color=blue)](https://pypi.org/project/mypy-boto3-location)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-location)](https://pepy.tech/project/mypy-boto3-location)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LocationService 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService)
+[boto3.LocationService 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService)
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
 [mypy-boto3-location docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/).
 
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
@@ -326,34 +326,35 @@
 )
 
 
 def check_value(value: BatchItemErrorCodeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_location.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_location.type_defs import (
     ApiKeyFilterTypeDef,
     ApiKeyRestrictionsOutputTypeDef,
     ApiKeyRestrictionsTypeDef,
     AssociateTrackerConsumerRequestRequestTypeDef,
     BatchItemErrorTypeDef,
     BatchDeleteDevicePositionHistoryRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     BatchDeleteGeofenceRequestRequestTypeDef,
     BatchGetDevicePositionRequestRequestTypeDef,
     BatchPutGeofenceSuccessTypeDef,
     CalculateRouteCarModeOptionsTypeDef,
+    TimestampTypeDef,
     CalculateRouteMatrixSummaryTypeDef,
     CalculateRouteSummaryTypeDef,
     TruckDimensionsTypeDef,
     TruckWeightTypeDef,
     CircleOutputTypeDef,
     CircleTypeDef,
     CreateGeofenceCollectionRequestRequestTypeDef,
@@ -372,15 +373,14 @@
     DescribeMapRequestRequestTypeDef,
     DescribePlaceIndexRequestRequestTypeDef,
     DescribeRouteCalculatorRequestRequestTypeDef,
     DescribeTrackerRequestRequestTypeDef,
     PositionalAccuracyTypeDef,
     DisassociateTrackerConsumerRequestRequestTypeDef,
     PaginatorConfigTypeDef,
-    GetDevicePositionHistoryRequestRequestTypeDef,
     GetDevicePositionRequestRequestTypeDef,
     GetGeofenceRequestRequestTypeDef,
     GetMapGlyphsRequestRequestTypeDef,
     GetMapSpritesRequestRequestTypeDef,
     GetMapStyleDescriptorRequestRequestTypeDef,
     GetMapTileRequestRequestTypeDef,
     GetPlaceRequestRequestTypeDef,
@@ -414,16 +414,15 @@
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateGeofenceCollectionRequestRequestTypeDef,
     UpdateRouteCalculatorRequestRequestTypeDef,
     UpdateTrackerRequestRequestTypeDef,
     ListKeysRequestRequestTypeDef,
     ListKeysResponseEntryTypeDef,
-    CreateKeyRequestRequestTypeDef,
-    UpdateKeyRequestRequestTypeDef,
+    ApiKeyRestrictionsUnionTypeDef,
     BatchDeleteDevicePositionHistoryErrorTypeDef,
     BatchDeleteGeofenceErrorTypeDef,
     BatchEvaluateGeofencesErrorTypeDef,
     BatchGetDevicePositionErrorTypeDef,
     BatchPutGeofenceErrorTypeDef,
     BatchUpdateDevicePositionErrorTypeDef,
     CreateGeofenceCollectionResponseTypeDef,
@@ -445,14 +444,17 @@
     PutGeofenceResponseTypeDef,
     UpdateGeofenceCollectionResponseTypeDef,
     UpdateKeyResponseTypeDef,
     UpdateMapResponseTypeDef,
     UpdatePlaceIndexResponseTypeDef,
     UpdateRouteCalculatorResponseTypeDef,
     UpdateTrackerResponseTypeDef,
+    CreateKeyRequestRequestTypeDef,
+    GetDevicePositionHistoryRequestRequestTypeDef,
+    UpdateKeyRequestRequestTypeDef,
     CalculateRouteTruckModeOptionsTypeDef,
     GeofenceGeometryOutputTypeDef,
     GeofenceGeometryTypeDef,
     CreateMapRequestRequestTypeDef,
     DescribeMapResponseTypeDef,
     CreatePlaceIndexRequestRequestTypeDef,
     DescribePlaceIndexResponseTypeDef,
@@ -488,14 +490,15 @@
     BatchPutGeofenceResponseTypeDef,
     BatchUpdateDevicePositionResponseTypeDef,
     CalculateRouteMatrixRequestRequestTypeDef,
     CalculateRouteRequestRequestTypeDef,
     GetGeofenceResponseTypeDef,
     ListGeofenceResponseEntryTypeDef,
     BatchPutGeofenceRequestEntryTypeDef,
+    GeofenceGeometryUnionTypeDef,
     PutGeofenceRequestRequestTypeDef,
     BatchGetDevicePositionResponseTypeDef,
     GetDevicePositionHistoryResponseTypeDef,
     BatchEvaluateGeofencesRequestRequestTypeDef,
     BatchUpdateDevicePositionRequestRequestTypeDef,
     ListDevicePositionsResponseTypeDef,
     CalculateRouteResponseTypeDef,
@@ -506,15 +509,15 @@
     ListGeofencesResponseTypeDef,
     BatchPutGeofenceRequestRequestTypeDef,
     SearchPlaceIndexForPositionResponseTypeDef,
     SearchPlaceIndexForTextResponseTypeDef,
 )
 
 
-def get_structure() -> ApiKeyFilterTypeDef:
+def get_value() -> ApiKeyFilterTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-location-1.28.15.post1/mypy_boto3_location/__init__.py` & `mypy-boto3-location-1.28.16/mypy_boto3_location/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-location-1.28.15.post1/mypy_boto3_location/__init__.pyi` & `mypy-boto3-location-1.28.16/mypy_boto3_location/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-location-1.28.15.post1/mypy_boto3_location/__main__.py` & `mypy-boto3-location-1.28.16/mypy_boto3_location/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.LocationService 1.28.15\nVersion:        "
-        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.LocationService 1.28.16\nVersion:         1.28.16\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService\nOther"
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

### Comparing `mypy-boto3-location-1.28.15.post1/mypy_boto3_location/client.py` & `mypy-boto3-location-1.28.16/mypy_boto3_location/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from mypy_boto3_location.client import LocationServiceClient
 
     session = Session()
     client: LocationServiceClient = session.client("location")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import DistanceUnitType, PositionFilteringType, PricingPlanType, TravelModeType
 from .paginator import (
     GetDevicePositionHistoryPaginator,
     ListDevicePositionsPaginator,
@@ -30,16 +29,15 @@
     ListPlaceIndexesPaginator,
     ListRouteCalculatorsPaginator,
     ListTrackerConsumersPaginator,
     ListTrackersPaginator,
 )
 from .type_defs import (
     ApiKeyFilterTypeDef,
-    ApiKeyRestrictionsOutputTypeDef,
-    ApiKeyRestrictionsTypeDef,
+    ApiKeyRestrictionsUnionTypeDef,
     BatchDeleteDevicePositionHistoryResponseTypeDef,
     BatchDeleteGeofenceResponseTypeDef,
     BatchEvaluateGeofencesResponseTypeDef,
     BatchGetDevicePositionResponseTypeDef,
     BatchPutGeofenceRequestEntryTypeDef,
     BatchPutGeofenceResponseTypeDef,
     BatchUpdateDevicePositionResponseTypeDef,
@@ -57,16 +55,15 @@
     DescribeGeofenceCollectionResponseTypeDef,
     DescribeKeyResponseTypeDef,
     DescribeMapResponseTypeDef,
     DescribePlaceIndexResponseTypeDef,
     DescribeRouteCalculatorResponseTypeDef,
     DescribeTrackerResponseTypeDef,
     DevicePositionUpdateTypeDef,
-    GeofenceGeometryOutputTypeDef,
-    GeofenceGeometryTypeDef,
+    GeofenceGeometryUnionTypeDef,
     GetDevicePositionHistoryResponseTypeDef,
     GetDevicePositionResponseTypeDef,
     GetGeofenceResponseTypeDef,
     GetMapGlyphsResponseTypeDef,
     GetMapSpritesResponseTypeDef,
     GetMapStyleDescriptorResponseTypeDef,
     GetMapTileResponseTypeDef,
@@ -83,14 +80,15 @@
     ListTrackersResponseTypeDef,
     MapConfigurationTypeDef,
     MapConfigurationUpdateTypeDef,
     PutGeofenceResponseTypeDef,
     SearchPlaceIndexForPositionResponseTypeDef,
     SearchPlaceIndexForSuggestionsResponseTypeDef,
     SearchPlaceIndexForTextResponseTypeDef,
+    TimestampTypeDef,
     UpdateGeofenceCollectionResponseTypeDef,
     UpdateKeyResponseTypeDef,
     UpdateMapResponseTypeDef,
     UpdatePlaceIndexResponseTypeDef,
     UpdateRouteCalculatorResponseTypeDef,
     UpdateTrackerResponseTypeDef,
 )
@@ -216,15 +214,15 @@
         self,
         *,
         CalculatorName: str,
         DeparturePosition: Sequence[float],
         DestinationPosition: Sequence[float],
         CarModeOptions: CalculateRouteCarModeOptionsTypeDef = ...,
         DepartNow: bool = ...,
-        DepartureTime: Union[datetime, str] = ...,
+        DepartureTime: TimestampTypeDef = ...,
         DistanceUnit: DistanceUnitType = ...,
         IncludeLegGeometry: bool = ...,
         Key: str = ...,
         TravelMode: TravelModeType = ...,
         TruckModeOptions: CalculateRouteTruckModeOptionsTypeDef = ...,
         WaypointPositions: Sequence[Sequence[float]] = ...
     ) -> CalculateRouteResponseTypeDef:
@@ -242,15 +240,15 @@
         self,
         *,
         CalculatorName: str,
         DeparturePositions: Sequence[Sequence[float]],
         DestinationPositions: Sequence[Sequence[float]],
         CarModeOptions: CalculateRouteCarModeOptionsTypeDef = ...,
         DepartNow: bool = ...,
-        DepartureTime: Union[datetime, str] = ...,
+        DepartureTime: TimestampTypeDef = ...,
         DistanceUnit: DistanceUnitType = ...,
         Key: str = ...,
         TravelMode: TravelModeType = ...,
         TruckModeOptions: CalculateRouteTruckModeOptionsTypeDef = ...
     ) -> CalculateRouteMatrixResponseTypeDef:
         """
         [Calculates a route
@@ -295,17 +293,17 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/client/#create_geofence_collection)
         """
 
     def create_key(
         self,
         *,
         KeyName: str,
-        Restrictions: Union[ApiKeyRestrictionsTypeDef, ApiKeyRestrictionsOutputTypeDef],
+        Restrictions: ApiKeyRestrictionsUnionTypeDef,
         Description: str = ...,
-        ExpireTime: Union[datetime, str] = ...,
+        ExpireTime: TimestampTypeDef = ...,
         NoExpiry: bool = ...,
         Tags: Mapping[str, str] = ...
     ) -> CreateKeyResponseTypeDef:
         """
         Creates an API key resource in your Amazon Web Services account, which lets you
         grant actions for Amazon Location resources to the API key bearer.
 
@@ -518,18 +516,18 @@
         """
 
     def get_device_position_history(
         self,
         *,
         DeviceId: str,
         TrackerName: str,
-        EndTimeExclusive: Union[datetime, str] = ...,
+        EndTimeExclusive: TimestampTypeDef = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
-        StartTimeInclusive: Union[datetime, str] = ...
+        StartTimeInclusive: TimestampTypeDef = ...
     ) -> GetDevicePositionHistoryResponseTypeDef:
         """
         Retrieves the device position history from a tracker resource within a specified
         range of time.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.get_device_position_history)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/client/#get_device_position_history)
@@ -691,15 +689,15 @@
         """
 
     def put_geofence(
         self,
         *,
         CollectionName: str,
         GeofenceId: str,
-        Geometry: Union[GeofenceGeometryTypeDef, GeofenceGeometryOutputTypeDef],
+        Geometry: GeofenceGeometryUnionTypeDef,
         GeofenceProperties: Mapping[str, str] = ...
     ) -> PutGeofenceResponseTypeDef:
         """
         Stores a geofence geometry in a given geofence collection, or updates the
         geometry of an existing geofence if a geofence ID is included in the request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.put_geofence)
@@ -797,18 +795,18 @@
         """
 
     def update_key(
         self,
         *,
         KeyName: str,
         Description: str = ...,
-        ExpireTime: Union[datetime, str] = ...,
+        ExpireTime: TimestampTypeDef = ...,
         ForceUpdate: bool = ...,
         NoExpiry: bool = ...,
-        Restrictions: Union[ApiKeyRestrictionsTypeDef, ApiKeyRestrictionsOutputTypeDef] = ...
+        Restrictions: ApiKeyRestrictionsUnionTypeDef = ...
     ) -> UpdateKeyResponseTypeDef:
         """
         Updates the specified properties of a given API key resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.update_key)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/client/#update_key)
         """
```

### Comparing `mypy-boto3-location-1.28.15.post1/mypy_boto3_location/client.pyi` & `mypy-boto3-location-1.28.16/mypy_boto3_location/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from mypy_boto3_location.client import LocationServiceClient
 
     session = Session()
     client: LocationServiceClient = session.client("location")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import DistanceUnitType, PositionFilteringType, PricingPlanType, TravelModeType
 from .paginator import (
     GetDevicePositionHistoryPaginator,
     ListDevicePositionsPaginator,
@@ -30,16 +29,15 @@
     ListPlaceIndexesPaginator,
     ListRouteCalculatorsPaginator,
     ListTrackerConsumersPaginator,
     ListTrackersPaginator,
 )
 from .type_defs import (
     ApiKeyFilterTypeDef,
-    ApiKeyRestrictionsOutputTypeDef,
-    ApiKeyRestrictionsTypeDef,
+    ApiKeyRestrictionsUnionTypeDef,
     BatchDeleteDevicePositionHistoryResponseTypeDef,
     BatchDeleteGeofenceResponseTypeDef,
     BatchEvaluateGeofencesResponseTypeDef,
     BatchGetDevicePositionResponseTypeDef,
     BatchPutGeofenceRequestEntryTypeDef,
     BatchPutGeofenceResponseTypeDef,
     BatchUpdateDevicePositionResponseTypeDef,
@@ -57,16 +55,15 @@
     DescribeGeofenceCollectionResponseTypeDef,
     DescribeKeyResponseTypeDef,
     DescribeMapResponseTypeDef,
     DescribePlaceIndexResponseTypeDef,
     DescribeRouteCalculatorResponseTypeDef,
     DescribeTrackerResponseTypeDef,
     DevicePositionUpdateTypeDef,
-    GeofenceGeometryOutputTypeDef,
-    GeofenceGeometryTypeDef,
+    GeofenceGeometryUnionTypeDef,
     GetDevicePositionHistoryResponseTypeDef,
     GetDevicePositionResponseTypeDef,
     GetGeofenceResponseTypeDef,
     GetMapGlyphsResponseTypeDef,
     GetMapSpritesResponseTypeDef,
     GetMapStyleDescriptorResponseTypeDef,
     GetMapTileResponseTypeDef,
@@ -83,14 +80,15 @@
     ListTrackersResponseTypeDef,
     MapConfigurationTypeDef,
     MapConfigurationUpdateTypeDef,
     PutGeofenceResponseTypeDef,
     SearchPlaceIndexForPositionResponseTypeDef,
     SearchPlaceIndexForSuggestionsResponseTypeDef,
     SearchPlaceIndexForTextResponseTypeDef,
+    TimestampTypeDef,
     UpdateGeofenceCollectionResponseTypeDef,
     UpdateKeyResponseTypeDef,
     UpdateMapResponseTypeDef,
     UpdatePlaceIndexResponseTypeDef,
     UpdateRouteCalculatorResponseTypeDef,
     UpdateTrackerResponseTypeDef,
 )
@@ -204,15 +202,15 @@
         self,
         *,
         CalculatorName: str,
         DeparturePosition: Sequence[float],
         DestinationPosition: Sequence[float],
         CarModeOptions: CalculateRouteCarModeOptionsTypeDef = ...,
         DepartNow: bool = ...,
-        DepartureTime: Union[datetime, str] = ...,
+        DepartureTime: TimestampTypeDef = ...,
         DistanceUnit: DistanceUnitType = ...,
         IncludeLegGeometry: bool = ...,
         Key: str = ...,
         TravelMode: TravelModeType = ...,
         TruckModeOptions: CalculateRouteTruckModeOptionsTypeDef = ...,
         WaypointPositions: Sequence[Sequence[float]] = ...
     ) -> CalculateRouteResponseTypeDef:
@@ -229,15 +227,15 @@
         self,
         *,
         CalculatorName: str,
         DeparturePositions: Sequence[Sequence[float]],
         DestinationPositions: Sequence[Sequence[float]],
         CarModeOptions: CalculateRouteCarModeOptionsTypeDef = ...,
         DepartNow: bool = ...,
-        DepartureTime: Union[datetime, str] = ...,
+        DepartureTime: TimestampTypeDef = ...,
         DistanceUnit: DistanceUnitType = ...,
         Key: str = ...,
         TravelMode: TravelModeType = ...,
         TruckModeOptions: CalculateRouteTruckModeOptionsTypeDef = ...
     ) -> CalculateRouteMatrixResponseTypeDef:
         """
         [Calculates a route
@@ -278,17 +276,17 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.create_geofence_collection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/client/#create_geofence_collection)
         """
     def create_key(
         self,
         *,
         KeyName: str,
-        Restrictions: Union[ApiKeyRestrictionsTypeDef, ApiKeyRestrictionsOutputTypeDef],
+        Restrictions: ApiKeyRestrictionsUnionTypeDef,
         Description: str = ...,
-        ExpireTime: Union[datetime, str] = ...,
+        ExpireTime: TimestampTypeDef = ...,
         NoExpiry: bool = ...,
         Tags: Mapping[str, str] = ...
     ) -> CreateKeyResponseTypeDef:
         """
         Creates an API key resource in your Amazon Web Services account, which lets you
         grant actions for Amazon Location resources to the API key bearer.
 
@@ -481,18 +479,18 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/client/#get_device_position)
         """
     def get_device_position_history(
         self,
         *,
         DeviceId: str,
         TrackerName: str,
-        EndTimeExclusive: Union[datetime, str] = ...,
+        EndTimeExclusive: TimestampTypeDef = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
-        StartTimeInclusive: Union[datetime, str] = ...
+        StartTimeInclusive: TimestampTypeDef = ...
     ) -> GetDevicePositionHistoryResponseTypeDef:
         """
         Retrieves the device position history from a tracker resource within a specified
         range of time.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.get_device_position_history)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/client/#get_device_position_history)
@@ -637,15 +635,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/client/#list_trackers)
         """
     def put_geofence(
         self,
         *,
         CollectionName: str,
         GeofenceId: str,
-        Geometry: Union[GeofenceGeometryTypeDef, GeofenceGeometryOutputTypeDef],
+        Geometry: GeofenceGeometryUnionTypeDef,
         GeofenceProperties: Mapping[str, str] = ...
     ) -> PutGeofenceResponseTypeDef:
         """
         Stores a geofence geometry in a given geofence collection, or updates the
         geometry of an existing geofence if a geofence ID is included in the request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.put_geofence)
@@ -736,18 +734,18 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/client/#update_geofence_collection)
         """
     def update_key(
         self,
         *,
         KeyName: str,
         Description: str = ...,
-        ExpireTime: Union[datetime, str] = ...,
+        ExpireTime: TimestampTypeDef = ...,
         ForceUpdate: bool = ...,
         NoExpiry: bool = ...,
-        Restrictions: Union[ApiKeyRestrictionsTypeDef, ApiKeyRestrictionsOutputTypeDef] = ...
+        Restrictions: ApiKeyRestrictionsUnionTypeDef = ...
     ) -> UpdateKeyResponseTypeDef:
         """
         Updates the specified properties of a given API key resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.update_key)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/client/#update_key)
         """
```

### Comparing `mypy-boto3-location-1.28.15.post1/mypy_boto3_location/literals.py` & `mypy-boto3-location-1.28.16/mypy_boto3_location/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-location-1.28.15.post1/mypy_boto3_location/literals.pyi` & `mypy-boto3-location-1.28.16/mypy_boto3_location/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-location-1.28.15.post1/mypy_boto3_location/paginator.py` & `mypy-boto3-location-1.28.16/mypy_boto3_location/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,16 +33,15 @@
     list_maps_paginator: ListMapsPaginator = client.get_paginator("list_maps")
     list_place_indexes_paginator: ListPlaceIndexesPaginator = client.get_paginator("list_place_indexes")
     list_route_calculators_paginator: ListRouteCalculatorsPaginator = client.get_paginator("list_route_calculators")
     list_tracker_consumers_paginator: ListTrackerConsumersPaginator = client.get_paginator("list_tracker_consumers")
     list_trackers_paginator: ListTrackersPaginator = client.get_paginator("list_trackers")
     ```
 """
-from datetime import datetime
-from typing import Generic, Iterator, TypeVar, Union
+from typing import Generic, Iterator, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import (
     ApiKeyFilterTypeDef,
     GetDevicePositionHistoryResponseTypeDef,
     ListDevicePositionsResponseTypeDef,
@@ -51,14 +50,15 @@
     ListKeysResponseTypeDef,
     ListMapsResponseTypeDef,
     ListPlaceIndexesResponseTypeDef,
     ListRouteCalculatorsResponseTypeDef,
     ListTrackerConsumersResponseTypeDef,
     ListTrackersResponseTypeDef,
     PaginatorConfigTypeDef,
+    TimestampTypeDef,
 )
 
 __all__ = (
     "GetDevicePositionHistoryPaginator",
     "ListDevicePositionsPaginator",
     "ListGeofenceCollectionsPaginator",
     "ListGeofencesPaginator",
@@ -88,16 +88,16 @@
     """
 
     def paginate(
         self,
         *,
         DeviceId: str,
         TrackerName: str,
-        EndTimeExclusive: Union[datetime, str] = ...,
-        StartTimeInclusive: Union[datetime, str] = ...,
+        EndTimeExclusive: TimestampTypeDef = ...,
+        StartTimeInclusive: TimestampTypeDef = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetDevicePositionHistoryResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.GetDevicePositionHistory.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/paginators/#getdevicepositionhistorypaginator)
         """
```

### Comparing `mypy-boto3-location-1.28.15.post1/mypy_boto3_location/paginator.pyi` & `mypy-boto3-location-1.28.16/mypy_boto3_location/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -33,16 +33,15 @@
     list_maps_paginator: ListMapsPaginator = client.get_paginator("list_maps")
     list_place_indexes_paginator: ListPlaceIndexesPaginator = client.get_paginator("list_place_indexes")
     list_route_calculators_paginator: ListRouteCalculatorsPaginator = client.get_paginator("list_route_calculators")
     list_tracker_consumers_paginator: ListTrackerConsumersPaginator = client.get_paginator("list_tracker_consumers")
     list_trackers_paginator: ListTrackersPaginator = client.get_paginator("list_trackers")
     ```
 """
-from datetime import datetime
-from typing import Generic, Iterator, TypeVar, Union
+from typing import Generic, Iterator, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import (
     ApiKeyFilterTypeDef,
     GetDevicePositionHistoryResponseTypeDef,
     ListDevicePositionsResponseTypeDef,
@@ -51,14 +50,15 @@
     ListKeysResponseTypeDef,
     ListMapsResponseTypeDef,
     ListPlaceIndexesResponseTypeDef,
     ListRouteCalculatorsResponseTypeDef,
     ListTrackerConsumersResponseTypeDef,
     ListTrackersResponseTypeDef,
     PaginatorConfigTypeDef,
+    TimestampTypeDef,
 )
 
 __all__ = (
     "GetDevicePositionHistoryPaginator",
     "ListDevicePositionsPaginator",
     "ListGeofenceCollectionsPaginator",
     "ListGeofencesPaginator",
@@ -85,16 +85,16 @@
     """
 
     def paginate(
         self,
         *,
         DeviceId: str,
         TrackerName: str,
-        EndTimeExclusive: Union[datetime, str] = ...,
-        StartTimeInclusive: Union[datetime, str] = ...,
+        EndTimeExclusive: TimestampTypeDef = ...,
+        StartTimeInclusive: TimestampTypeDef = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetDevicePositionHistoryResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.GetDevicePositionHistory.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/paginators/#getdevicepositionhistorypaginator)
         """
```

### Comparing `mypy-boto3-location-1.28.15.post1/mypy_boto3_location/type_defs.py` & `mypy-boto3-location-1.28.16/mypy_boto3_location/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_location.type_defs import ApiKeyFilterTypeDef
 
-    data: ApiKeyFilterTypeDef = {...}
+    data: ApiKeyFilterTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -44,14 +44,15 @@
     "BatchItemErrorTypeDef",
     "BatchDeleteDevicePositionHistoryRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "BatchDeleteGeofenceRequestRequestTypeDef",
     "BatchGetDevicePositionRequestRequestTypeDef",
     "BatchPutGeofenceSuccessTypeDef",
     "CalculateRouteCarModeOptionsTypeDef",
+    "TimestampTypeDef",
     "CalculateRouteMatrixSummaryTypeDef",
     "CalculateRouteSummaryTypeDef",
     "TruckDimensionsTypeDef",
     "TruckWeightTypeDef",
     "CircleOutputTypeDef",
     "CircleTypeDef",
     "CreateGeofenceCollectionRequestRequestTypeDef",
@@ -70,15 +71,14 @@
     "DescribeMapRequestRequestTypeDef",
     "DescribePlaceIndexRequestRequestTypeDef",
     "DescribeRouteCalculatorRequestRequestTypeDef",
     "DescribeTrackerRequestRequestTypeDef",
     "PositionalAccuracyTypeDef",
     "DisassociateTrackerConsumerRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
-    "GetDevicePositionHistoryRequestRequestTypeDef",
     "GetDevicePositionRequestRequestTypeDef",
     "GetGeofenceRequestRequestTypeDef",
     "GetMapGlyphsRequestRequestTypeDef",
     "GetMapSpritesRequestRequestTypeDef",
     "GetMapStyleDescriptorRequestRequestTypeDef",
     "GetMapTileRequestRequestTypeDef",
     "GetPlaceRequestRequestTypeDef",
@@ -112,16 +112,15 @@
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateGeofenceCollectionRequestRequestTypeDef",
     "UpdateRouteCalculatorRequestRequestTypeDef",
     "UpdateTrackerRequestRequestTypeDef",
     "ListKeysRequestRequestTypeDef",
     "ListKeysResponseEntryTypeDef",
-    "CreateKeyRequestRequestTypeDef",
-    "UpdateKeyRequestRequestTypeDef",
+    "ApiKeyRestrictionsUnionTypeDef",
     "BatchDeleteDevicePositionHistoryErrorTypeDef",
     "BatchDeleteGeofenceErrorTypeDef",
     "BatchEvaluateGeofencesErrorTypeDef",
     "BatchGetDevicePositionErrorTypeDef",
     "BatchPutGeofenceErrorTypeDef",
     "BatchUpdateDevicePositionErrorTypeDef",
     "CreateGeofenceCollectionResponseTypeDef",
@@ -143,14 +142,17 @@
     "PutGeofenceResponseTypeDef",
     "UpdateGeofenceCollectionResponseTypeDef",
     "UpdateKeyResponseTypeDef",
     "UpdateMapResponseTypeDef",
     "UpdatePlaceIndexResponseTypeDef",
     "UpdateRouteCalculatorResponseTypeDef",
     "UpdateTrackerResponseTypeDef",
+    "CreateKeyRequestRequestTypeDef",
+    "GetDevicePositionHistoryRequestRequestTypeDef",
+    "UpdateKeyRequestRequestTypeDef",
     "CalculateRouteTruckModeOptionsTypeDef",
     "GeofenceGeometryOutputTypeDef",
     "GeofenceGeometryTypeDef",
     "CreateMapRequestRequestTypeDef",
     "DescribeMapResponseTypeDef",
     "CreatePlaceIndexRequestRequestTypeDef",
     "DescribePlaceIndexResponseTypeDef",
@@ -186,14 +188,15 @@
     "BatchPutGeofenceResponseTypeDef",
     "BatchUpdateDevicePositionResponseTypeDef",
     "CalculateRouteMatrixRequestRequestTypeDef",
     "CalculateRouteRequestRequestTypeDef",
     "GetGeofenceResponseTypeDef",
     "ListGeofenceResponseEntryTypeDef",
     "BatchPutGeofenceRequestEntryTypeDef",
+    "GeofenceGeometryUnionTypeDef",
     "PutGeofenceRequestRequestTypeDef",
     "BatchGetDevicePositionResponseTypeDef",
     "GetDevicePositionHistoryResponseTypeDef",
     "BatchEvaluateGeofencesRequestRequestTypeDef",
     "BatchUpdateDevicePositionRequestRequestTypeDef",
     "ListDevicePositionsResponseTypeDef",
     "CalculateRouteResponseTypeDef",
@@ -325,14 +328,15 @@
     {
         "AvoidFerries": bool,
         "AvoidTolls": bool,
     },
     total=False,
 )
 
+TimestampTypeDef = Union[datetime, str]
 CalculateRouteMatrixSummaryTypeDef = TypedDict(
     "CalculateRouteMatrixSummaryTypeDef",
     {
         "DataSource": str,
         "DistanceUnit": DistanceUnitType,
         "ErrorCount": int,
         "RouteCount": int,
@@ -596,40 +600,14 @@
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
-_RequiredGetDevicePositionHistoryRequestRequestTypeDef = TypedDict(
-    "_RequiredGetDevicePositionHistoryRequestRequestTypeDef",
-    {
-        "DeviceId": str,
-        "TrackerName": str,
-    },
-)
-_OptionalGetDevicePositionHistoryRequestRequestTypeDef = TypedDict(
-    "_OptionalGetDevicePositionHistoryRequestRequestTypeDef",
-    {
-        "EndTimeExclusive": Union[datetime, str],
-        "MaxResults": int,
-        "NextToken": str,
-        "StartTimeInclusive": Union[datetime, str],
-    },
-    total=False,
-)
-
-
-class GetDevicePositionHistoryRequestRequestTypeDef(
-    _RequiredGetDevicePositionHistoryRequestRequestTypeDef,
-    _OptionalGetDevicePositionHistoryRequestRequestTypeDef,
-):
-    pass
-
-
 GetDevicePositionRequestRequestTypeDef = TypedDict(
     "GetDevicePositionRequestRequestTypeDef",
     {
         "DeviceId": str,
         "TrackerName": str,
     },
 )
@@ -1394,64 +1372,15 @@
 
 class ListKeysResponseEntryTypeDef(
     _RequiredListKeysResponseEntryTypeDef, _OptionalListKeysResponseEntryTypeDef
 ):
     pass
 
 
-_RequiredCreateKeyRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateKeyRequestRequestTypeDef",
-    {
-        "KeyName": str,
-        "Restrictions": ApiKeyRestrictionsTypeDef,
-    },
-)
-_OptionalCreateKeyRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateKeyRequestRequestTypeDef",
-    {
-        "Description": str,
-        "ExpireTime": Union[datetime, str],
-        "NoExpiry": bool,
-        "Tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-
-class CreateKeyRequestRequestTypeDef(
-    _RequiredCreateKeyRequestRequestTypeDef, _OptionalCreateKeyRequestRequestTypeDef
-):
-    pass
-
-
-_RequiredUpdateKeyRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateKeyRequestRequestTypeDef",
-    {
-        "KeyName": str,
-    },
-)
-_OptionalUpdateKeyRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateKeyRequestRequestTypeDef",
-    {
-        "Description": str,
-        "ExpireTime": Union[datetime, str],
-        "ForceUpdate": bool,
-        "NoExpiry": bool,
-        "Restrictions": ApiKeyRestrictionsTypeDef,
-    },
-    total=False,
-)
-
-
-class UpdateKeyRequestRequestTypeDef(
-    _RequiredUpdateKeyRequestRequestTypeDef, _OptionalUpdateKeyRequestRequestTypeDef
-):
-    pass
-
-
+ApiKeyRestrictionsUnionTypeDef = Union[ApiKeyRestrictionsTypeDef, ApiKeyRestrictionsOutputTypeDef]
 BatchDeleteDevicePositionHistoryErrorTypeDef = TypedDict(
     "BatchDeleteDevicePositionHistoryErrorTypeDef",
     {
         "DeviceId": str,
         "Error": BatchItemErrorTypeDef,
     },
 )
@@ -1747,14 +1676,90 @@
         "TrackerArn": str,
         "TrackerName": str,
         "UpdateTime": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredCreateKeyRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateKeyRequestRequestTypeDef",
+    {
+        "KeyName": str,
+        "Restrictions": ApiKeyRestrictionsTypeDef,
+    },
+)
+_OptionalCreateKeyRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateKeyRequestRequestTypeDef",
+    {
+        "Description": str,
+        "ExpireTime": TimestampTypeDef,
+        "NoExpiry": bool,
+        "Tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+
+class CreateKeyRequestRequestTypeDef(
+    _RequiredCreateKeyRequestRequestTypeDef, _OptionalCreateKeyRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredGetDevicePositionHistoryRequestRequestTypeDef = TypedDict(
+    "_RequiredGetDevicePositionHistoryRequestRequestTypeDef",
+    {
+        "DeviceId": str,
+        "TrackerName": str,
+    },
+)
+_OptionalGetDevicePositionHistoryRequestRequestTypeDef = TypedDict(
+    "_OptionalGetDevicePositionHistoryRequestRequestTypeDef",
+    {
+        "EndTimeExclusive": TimestampTypeDef,
+        "MaxResults": int,
+        "NextToken": str,
+        "StartTimeInclusive": TimestampTypeDef,
+    },
+    total=False,
+)
+
+
+class GetDevicePositionHistoryRequestRequestTypeDef(
+    _RequiredGetDevicePositionHistoryRequestRequestTypeDef,
+    _OptionalGetDevicePositionHistoryRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredUpdateKeyRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateKeyRequestRequestTypeDef",
+    {
+        "KeyName": str,
+    },
+)
+_OptionalUpdateKeyRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateKeyRequestRequestTypeDef",
+    {
+        "Description": str,
+        "ExpireTime": TimestampTypeDef,
+        "ForceUpdate": bool,
+        "NoExpiry": bool,
+        "Restrictions": ApiKeyRestrictionsTypeDef,
+    },
+    total=False,
+)
+
+
+class UpdateKeyRequestRequestTypeDef(
+    _RequiredUpdateKeyRequestRequestTypeDef, _OptionalUpdateKeyRequestRequestTypeDef
+):
+    pass
+
+
 CalculateRouteTruckModeOptionsTypeDef = TypedDict(
     "CalculateRouteTruckModeOptionsTypeDef",
     {
         "AvoidFerries": bool,
         "AvoidTolls": bool,
         "Dimensions": TruckDimensionsTypeDef,
         "Weight": TruckWeightTypeDef,
@@ -1908,15 +1913,15 @@
 
 
 _RequiredDevicePositionUpdateTypeDef = TypedDict(
     "_RequiredDevicePositionUpdateTypeDef",
     {
         "DeviceId": str,
         "Position": Sequence[float],
-        "SampleTime": Union[datetime, str],
+        "SampleTime": TimestampTypeDef,
     },
 )
 _OptionalDevicePositionUpdateTypeDef = TypedDict(
     "_OptionalDevicePositionUpdateTypeDef",
     {
         "Accuracy": PositionalAccuracyTypeDef,
         "PositionProperties": Mapping[str, str],
@@ -1975,16 +1980,16 @@
         "DeviceId": str,
         "TrackerName": str,
     },
 )
 _OptionalGetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef = TypedDict(
     "_OptionalGetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef",
     {
-        "EndTimeExclusive": Union[datetime, str],
-        "StartTimeInclusive": Union[datetime, str],
+        "EndTimeExclusive": TimestampTypeDef,
+        "StartTimeInclusive": TimestampTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class GetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef(
@@ -2311,15 +2316,15 @@
     },
 )
 _OptionalCalculateRouteMatrixRequestRequestTypeDef = TypedDict(
     "_OptionalCalculateRouteMatrixRequestRequestTypeDef",
     {
         "CarModeOptions": CalculateRouteCarModeOptionsTypeDef,
         "DepartNow": bool,
-        "DepartureTime": Union[datetime, str],
+        "DepartureTime": TimestampTypeDef,
         "DistanceUnit": DistanceUnitType,
         "Key": str,
         "TravelMode": TravelModeType,
         "TruckModeOptions": CalculateRouteTruckModeOptionsTypeDef,
     },
     total=False,
 )
@@ -2341,15 +2346,15 @@
     },
 )
 _OptionalCalculateRouteRequestRequestTypeDef = TypedDict(
     "_OptionalCalculateRouteRequestRequestTypeDef",
     {
         "CarModeOptions": CalculateRouteCarModeOptionsTypeDef,
         "DepartNow": bool,
-        "DepartureTime": Union[datetime, str],
+        "DepartureTime": TimestampTypeDef,
         "DistanceUnit": DistanceUnitType,
         "IncludeLegGeometry": bool,
         "Key": str,
         "TravelMode": TravelModeType,
         "TruckModeOptions": CalculateRouteTruckModeOptionsTypeDef,
         "WaypointPositions": Sequence[Sequence[float]],
     },
@@ -2419,14 +2424,15 @@
 
 class BatchPutGeofenceRequestEntryTypeDef(
     _RequiredBatchPutGeofenceRequestEntryTypeDef, _OptionalBatchPutGeofenceRequestEntryTypeDef
 ):
     pass
 
 
+GeofenceGeometryUnionTypeDef = Union[GeofenceGeometryTypeDef, GeofenceGeometryOutputTypeDef]
 _RequiredPutGeofenceRequestRequestTypeDef = TypedDict(
     "_RequiredPutGeofenceRequestRequestTypeDef",
     {
         "CollectionName": str,
         "GeofenceId": str,
         "Geometry": GeofenceGeometryTypeDef,
     },
```

### Comparing `mypy-boto3-location-1.28.15.post1/mypy_boto3_location/type_defs.pyi` & `mypy-boto3-location-1.28.16/mypy_boto3_location/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_location.type_defs import ApiKeyFilterTypeDef
 
-    data: ApiKeyFilterTypeDef = {...}
+    data: ApiKeyFilterTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -43,14 +43,15 @@
     "BatchItemErrorTypeDef",
     "BatchDeleteDevicePositionHistoryRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "BatchDeleteGeofenceRequestRequestTypeDef",
     "BatchGetDevicePositionRequestRequestTypeDef",
     "BatchPutGeofenceSuccessTypeDef",
     "CalculateRouteCarModeOptionsTypeDef",
+    "TimestampTypeDef",
     "CalculateRouteMatrixSummaryTypeDef",
     "CalculateRouteSummaryTypeDef",
     "TruckDimensionsTypeDef",
     "TruckWeightTypeDef",
     "CircleOutputTypeDef",
     "CircleTypeDef",
     "CreateGeofenceCollectionRequestRequestTypeDef",
@@ -69,15 +70,14 @@
     "DescribeMapRequestRequestTypeDef",
     "DescribePlaceIndexRequestRequestTypeDef",
     "DescribeRouteCalculatorRequestRequestTypeDef",
     "DescribeTrackerRequestRequestTypeDef",
     "PositionalAccuracyTypeDef",
     "DisassociateTrackerConsumerRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
-    "GetDevicePositionHistoryRequestRequestTypeDef",
     "GetDevicePositionRequestRequestTypeDef",
     "GetGeofenceRequestRequestTypeDef",
     "GetMapGlyphsRequestRequestTypeDef",
     "GetMapSpritesRequestRequestTypeDef",
     "GetMapStyleDescriptorRequestRequestTypeDef",
     "GetMapTileRequestRequestTypeDef",
     "GetPlaceRequestRequestTypeDef",
@@ -111,16 +111,15 @@
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateGeofenceCollectionRequestRequestTypeDef",
     "UpdateRouteCalculatorRequestRequestTypeDef",
     "UpdateTrackerRequestRequestTypeDef",
     "ListKeysRequestRequestTypeDef",
     "ListKeysResponseEntryTypeDef",
-    "CreateKeyRequestRequestTypeDef",
-    "UpdateKeyRequestRequestTypeDef",
+    "ApiKeyRestrictionsUnionTypeDef",
     "BatchDeleteDevicePositionHistoryErrorTypeDef",
     "BatchDeleteGeofenceErrorTypeDef",
     "BatchEvaluateGeofencesErrorTypeDef",
     "BatchGetDevicePositionErrorTypeDef",
     "BatchPutGeofenceErrorTypeDef",
     "BatchUpdateDevicePositionErrorTypeDef",
     "CreateGeofenceCollectionResponseTypeDef",
@@ -142,14 +141,17 @@
     "PutGeofenceResponseTypeDef",
     "UpdateGeofenceCollectionResponseTypeDef",
     "UpdateKeyResponseTypeDef",
     "UpdateMapResponseTypeDef",
     "UpdatePlaceIndexResponseTypeDef",
     "UpdateRouteCalculatorResponseTypeDef",
     "UpdateTrackerResponseTypeDef",
+    "CreateKeyRequestRequestTypeDef",
+    "GetDevicePositionHistoryRequestRequestTypeDef",
+    "UpdateKeyRequestRequestTypeDef",
     "CalculateRouteTruckModeOptionsTypeDef",
     "GeofenceGeometryOutputTypeDef",
     "GeofenceGeometryTypeDef",
     "CreateMapRequestRequestTypeDef",
     "DescribeMapResponseTypeDef",
     "CreatePlaceIndexRequestRequestTypeDef",
     "DescribePlaceIndexResponseTypeDef",
@@ -185,14 +187,15 @@
     "BatchPutGeofenceResponseTypeDef",
     "BatchUpdateDevicePositionResponseTypeDef",
     "CalculateRouteMatrixRequestRequestTypeDef",
     "CalculateRouteRequestRequestTypeDef",
     "GetGeofenceResponseTypeDef",
     "ListGeofenceResponseEntryTypeDef",
     "BatchPutGeofenceRequestEntryTypeDef",
+    "GeofenceGeometryUnionTypeDef",
     "PutGeofenceRequestRequestTypeDef",
     "BatchGetDevicePositionResponseTypeDef",
     "GetDevicePositionHistoryResponseTypeDef",
     "BatchEvaluateGeofencesRequestRequestTypeDef",
     "BatchUpdateDevicePositionRequestRequestTypeDef",
     "ListDevicePositionsResponseTypeDef",
     "CalculateRouteResponseTypeDef",
@@ -320,14 +323,15 @@
     {
         "AvoidFerries": bool,
         "AvoidTolls": bool,
     },
     total=False,
 )
 
+TimestampTypeDef = Union[datetime, str]
 CalculateRouteMatrixSummaryTypeDef = TypedDict(
     "CalculateRouteMatrixSummaryTypeDef",
     {
         "DataSource": str,
         "DistanceUnit": DistanceUnitType,
         "ErrorCount": int,
         "RouteCount": int,
@@ -583,38 +587,14 @@
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
-_RequiredGetDevicePositionHistoryRequestRequestTypeDef = TypedDict(
-    "_RequiredGetDevicePositionHistoryRequestRequestTypeDef",
-    {
-        "DeviceId": str,
-        "TrackerName": str,
-    },
-)
-_OptionalGetDevicePositionHistoryRequestRequestTypeDef = TypedDict(
-    "_OptionalGetDevicePositionHistoryRequestRequestTypeDef",
-    {
-        "EndTimeExclusive": Union[datetime, str],
-        "MaxResults": int,
-        "NextToken": str,
-        "StartTimeInclusive": Union[datetime, str],
-    },
-    total=False,
-)
-
-class GetDevicePositionHistoryRequestRequestTypeDef(
-    _RequiredGetDevicePositionHistoryRequestRequestTypeDef,
-    _OptionalGetDevicePositionHistoryRequestRequestTypeDef,
-):
-    pass
-
 GetDevicePositionRequestRequestTypeDef = TypedDict(
     "GetDevicePositionRequestRequestTypeDef",
     {
         "DeviceId": str,
         "TrackerName": str,
     },
 )
@@ -1325,60 +1305,15 @@
 )
 
 class ListKeysResponseEntryTypeDef(
     _RequiredListKeysResponseEntryTypeDef, _OptionalListKeysResponseEntryTypeDef
 ):
     pass
 
-_RequiredCreateKeyRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateKeyRequestRequestTypeDef",
-    {
-        "KeyName": str,
-        "Restrictions": ApiKeyRestrictionsTypeDef,
-    },
-)
-_OptionalCreateKeyRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateKeyRequestRequestTypeDef",
-    {
-        "Description": str,
-        "ExpireTime": Union[datetime, str],
-        "NoExpiry": bool,
-        "Tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-class CreateKeyRequestRequestTypeDef(
-    _RequiredCreateKeyRequestRequestTypeDef, _OptionalCreateKeyRequestRequestTypeDef
-):
-    pass
-
-_RequiredUpdateKeyRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateKeyRequestRequestTypeDef",
-    {
-        "KeyName": str,
-    },
-)
-_OptionalUpdateKeyRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateKeyRequestRequestTypeDef",
-    {
-        "Description": str,
-        "ExpireTime": Union[datetime, str],
-        "ForceUpdate": bool,
-        "NoExpiry": bool,
-        "Restrictions": ApiKeyRestrictionsTypeDef,
-    },
-    total=False,
-)
-
-class UpdateKeyRequestRequestTypeDef(
-    _RequiredUpdateKeyRequestRequestTypeDef, _OptionalUpdateKeyRequestRequestTypeDef
-):
-    pass
-
+ApiKeyRestrictionsUnionTypeDef = Union[ApiKeyRestrictionsTypeDef, ApiKeyRestrictionsOutputTypeDef]
 BatchDeleteDevicePositionHistoryErrorTypeDef = TypedDict(
     "BatchDeleteDevicePositionHistoryErrorTypeDef",
     {
         "DeviceId": str,
         "Error": BatchItemErrorTypeDef,
     },
 )
@@ -1674,14 +1609,84 @@
         "TrackerArn": str,
         "TrackerName": str,
         "UpdateTime": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredCreateKeyRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateKeyRequestRequestTypeDef",
+    {
+        "KeyName": str,
+        "Restrictions": ApiKeyRestrictionsTypeDef,
+    },
+)
+_OptionalCreateKeyRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateKeyRequestRequestTypeDef",
+    {
+        "Description": str,
+        "ExpireTime": TimestampTypeDef,
+        "NoExpiry": bool,
+        "Tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+class CreateKeyRequestRequestTypeDef(
+    _RequiredCreateKeyRequestRequestTypeDef, _OptionalCreateKeyRequestRequestTypeDef
+):
+    pass
+
+_RequiredGetDevicePositionHistoryRequestRequestTypeDef = TypedDict(
+    "_RequiredGetDevicePositionHistoryRequestRequestTypeDef",
+    {
+        "DeviceId": str,
+        "TrackerName": str,
+    },
+)
+_OptionalGetDevicePositionHistoryRequestRequestTypeDef = TypedDict(
+    "_OptionalGetDevicePositionHistoryRequestRequestTypeDef",
+    {
+        "EndTimeExclusive": TimestampTypeDef,
+        "MaxResults": int,
+        "NextToken": str,
+        "StartTimeInclusive": TimestampTypeDef,
+    },
+    total=False,
+)
+
+class GetDevicePositionHistoryRequestRequestTypeDef(
+    _RequiredGetDevicePositionHistoryRequestRequestTypeDef,
+    _OptionalGetDevicePositionHistoryRequestRequestTypeDef,
+):
+    pass
+
+_RequiredUpdateKeyRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateKeyRequestRequestTypeDef",
+    {
+        "KeyName": str,
+    },
+)
+_OptionalUpdateKeyRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateKeyRequestRequestTypeDef",
+    {
+        "Description": str,
+        "ExpireTime": TimestampTypeDef,
+        "ForceUpdate": bool,
+        "NoExpiry": bool,
+        "Restrictions": ApiKeyRestrictionsTypeDef,
+    },
+    total=False,
+)
+
+class UpdateKeyRequestRequestTypeDef(
+    _RequiredUpdateKeyRequestRequestTypeDef, _OptionalUpdateKeyRequestRequestTypeDef
+):
+    pass
+
 CalculateRouteTruckModeOptionsTypeDef = TypedDict(
     "CalculateRouteTruckModeOptionsTypeDef",
     {
         "AvoidFerries": bool,
         "AvoidTolls": bool,
         "Dimensions": TruckDimensionsTypeDef,
         "Weight": TruckWeightTypeDef,
@@ -1827,15 +1832,15 @@
     pass
 
 _RequiredDevicePositionUpdateTypeDef = TypedDict(
     "_RequiredDevicePositionUpdateTypeDef",
     {
         "DeviceId": str,
         "Position": Sequence[float],
-        "SampleTime": Union[datetime, str],
+        "SampleTime": TimestampTypeDef,
     },
 )
 _OptionalDevicePositionUpdateTypeDef = TypedDict(
     "_OptionalDevicePositionUpdateTypeDef",
     {
         "Accuracy": PositionalAccuracyTypeDef,
         "PositionProperties": Mapping[str, str],
@@ -1890,16 +1895,16 @@
         "DeviceId": str,
         "TrackerName": str,
     },
 )
 _OptionalGetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef = TypedDict(
     "_OptionalGetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef",
     {
-        "EndTimeExclusive": Union[datetime, str],
-        "StartTimeInclusive": Union[datetime, str],
+        "EndTimeExclusive": TimestampTypeDef,
+        "StartTimeInclusive": TimestampTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class GetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef(
     _RequiredGetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef,
@@ -2212,15 +2217,15 @@
     },
 )
 _OptionalCalculateRouteMatrixRequestRequestTypeDef = TypedDict(
     "_OptionalCalculateRouteMatrixRequestRequestTypeDef",
     {
         "CarModeOptions": CalculateRouteCarModeOptionsTypeDef,
         "DepartNow": bool,
-        "DepartureTime": Union[datetime, str],
+        "DepartureTime": TimestampTypeDef,
         "DistanceUnit": DistanceUnitType,
         "Key": str,
         "TravelMode": TravelModeType,
         "TruckModeOptions": CalculateRouteTruckModeOptionsTypeDef,
     },
     total=False,
 )
@@ -2240,15 +2245,15 @@
     },
 )
 _OptionalCalculateRouteRequestRequestTypeDef = TypedDict(
     "_OptionalCalculateRouteRequestRequestTypeDef",
     {
         "CarModeOptions": CalculateRouteCarModeOptionsTypeDef,
         "DepartNow": bool,
-        "DepartureTime": Union[datetime, str],
+        "DepartureTime": TimestampTypeDef,
         "DistanceUnit": DistanceUnitType,
         "IncludeLegGeometry": bool,
         "Key": str,
         "TravelMode": TravelModeType,
         "TruckModeOptions": CalculateRouteTruckModeOptionsTypeDef,
         "WaypointPositions": Sequence[Sequence[float]],
     },
@@ -2312,14 +2317,15 @@
 )
 
 class BatchPutGeofenceRequestEntryTypeDef(
     _RequiredBatchPutGeofenceRequestEntryTypeDef, _OptionalBatchPutGeofenceRequestEntryTypeDef
 ):
     pass
 
+GeofenceGeometryUnionTypeDef = Union[GeofenceGeometryTypeDef, GeofenceGeometryOutputTypeDef]
 _RequiredPutGeofenceRequestRequestTypeDef = TypedDict(
     "_RequiredPutGeofenceRequestRequestTypeDef",
     {
         "CollectionName": str,
         "GeofenceId": str,
         "Geometry": GeofenceGeometryTypeDef,
     },
```

### Comparing `mypy-boto3-location-1.28.15.post1/mypy_boto3_location.egg-info/PKG-INFO` & `mypy-boto3-location-1.28.16/mypy_boto3_location.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-location
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.LocationService 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.LocationService 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 location type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 location type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-location.svg?color=blue)](https://pypi.org/project/mypy-boto3-location)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-location)](https://pepy.tech/project/mypy-boto3-location)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LocationService 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService)
+[boto3.LocationService 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService)
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
 [mypy-boto3-location docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/).
 
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
@@ -358,34 +358,35 @@
 )
 
 
 def check_value(value: BatchItemErrorCodeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_location.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_location.type_defs import (
     ApiKeyFilterTypeDef,
     ApiKeyRestrictionsOutputTypeDef,
     ApiKeyRestrictionsTypeDef,
     AssociateTrackerConsumerRequestRequestTypeDef,
     BatchItemErrorTypeDef,
     BatchDeleteDevicePositionHistoryRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     BatchDeleteGeofenceRequestRequestTypeDef,
     BatchGetDevicePositionRequestRequestTypeDef,
     BatchPutGeofenceSuccessTypeDef,
     CalculateRouteCarModeOptionsTypeDef,
+    TimestampTypeDef,
     CalculateRouteMatrixSummaryTypeDef,
     CalculateRouteSummaryTypeDef,
     TruckDimensionsTypeDef,
     TruckWeightTypeDef,
     CircleOutputTypeDef,
     CircleTypeDef,
     CreateGeofenceCollectionRequestRequestTypeDef,
@@ -404,15 +405,14 @@
     DescribeMapRequestRequestTypeDef,
     DescribePlaceIndexRequestRequestTypeDef,
     DescribeRouteCalculatorRequestRequestTypeDef,
     DescribeTrackerRequestRequestTypeDef,
     PositionalAccuracyTypeDef,
     DisassociateTrackerConsumerRequestRequestTypeDef,
     PaginatorConfigTypeDef,
-    GetDevicePositionHistoryRequestRequestTypeDef,
     GetDevicePositionRequestRequestTypeDef,
     GetGeofenceRequestRequestTypeDef,
     GetMapGlyphsRequestRequestTypeDef,
     GetMapSpritesRequestRequestTypeDef,
     GetMapStyleDescriptorRequestRequestTypeDef,
     GetMapTileRequestRequestTypeDef,
     GetPlaceRequestRequestTypeDef,
@@ -446,16 +446,15 @@
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateGeofenceCollectionRequestRequestTypeDef,
     UpdateRouteCalculatorRequestRequestTypeDef,
     UpdateTrackerRequestRequestTypeDef,
     ListKeysRequestRequestTypeDef,
     ListKeysResponseEntryTypeDef,
-    CreateKeyRequestRequestTypeDef,
-    UpdateKeyRequestRequestTypeDef,
+    ApiKeyRestrictionsUnionTypeDef,
     BatchDeleteDevicePositionHistoryErrorTypeDef,
     BatchDeleteGeofenceErrorTypeDef,
     BatchEvaluateGeofencesErrorTypeDef,
     BatchGetDevicePositionErrorTypeDef,
     BatchPutGeofenceErrorTypeDef,
     BatchUpdateDevicePositionErrorTypeDef,
     CreateGeofenceCollectionResponseTypeDef,
@@ -477,14 +476,17 @@
     PutGeofenceResponseTypeDef,
     UpdateGeofenceCollectionResponseTypeDef,
     UpdateKeyResponseTypeDef,
     UpdateMapResponseTypeDef,
     UpdatePlaceIndexResponseTypeDef,
     UpdateRouteCalculatorResponseTypeDef,
     UpdateTrackerResponseTypeDef,
+    CreateKeyRequestRequestTypeDef,
+    GetDevicePositionHistoryRequestRequestTypeDef,
+    UpdateKeyRequestRequestTypeDef,
     CalculateRouteTruckModeOptionsTypeDef,
     GeofenceGeometryOutputTypeDef,
     GeofenceGeometryTypeDef,
     CreateMapRequestRequestTypeDef,
     DescribeMapResponseTypeDef,
     CreatePlaceIndexRequestRequestTypeDef,
     DescribePlaceIndexResponseTypeDef,
@@ -520,14 +522,15 @@
     BatchPutGeofenceResponseTypeDef,
     BatchUpdateDevicePositionResponseTypeDef,
     CalculateRouteMatrixRequestRequestTypeDef,
     CalculateRouteRequestRequestTypeDef,
     GetGeofenceResponseTypeDef,
     ListGeofenceResponseEntryTypeDef,
     BatchPutGeofenceRequestEntryTypeDef,
+    GeofenceGeometryUnionTypeDef,
     PutGeofenceRequestRequestTypeDef,
     BatchGetDevicePositionResponseTypeDef,
     GetDevicePositionHistoryResponseTypeDef,
     BatchEvaluateGeofencesRequestRequestTypeDef,
     BatchUpdateDevicePositionRequestRequestTypeDef,
     ListDevicePositionsResponseTypeDef,
     CalculateRouteResponseTypeDef,
@@ -538,15 +541,15 @@
     ListGeofencesResponseTypeDef,
     BatchPutGeofenceRequestRequestTypeDef,
     SearchPlaceIndexForPositionResponseTypeDef,
     SearchPlaceIndexForTextResponseTypeDef,
 )
 
 
-def get_structure() -> ApiKeyFilterTypeDef:
+def get_value() -> ApiKeyFilterTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-location-1.28.15.post1/mypy_boto3_location.egg-info/SOURCES.txt` & `mypy-boto3-location-1.28.16/mypy_boto3_location.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-location-1.28.15.post1/setup.py` & `mypy-boto3-location-1.28.16/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-location",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_location"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.LocationService 1.28.15 service generated with"
-        " mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.LocationService 1.28.16 service generated with"
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
-    keywords="boto3 location type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 location type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_location": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

