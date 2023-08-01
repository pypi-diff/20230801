# Comparing `tmp/mypy-boto3-sagemaker-geospatial-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-sagemaker-geospatial-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-sagemaker-geospatial-1.28.15.post1.tar", last modified: Sat Jul 29 10:04:06 2023, max compression
+gzip compressed data, was "mypy-boto3-sagemaker-geospatial-1.28.16.tar", last modified: Tue Aug  1 11:37:46 2023, max compression
```

## Comparing `mypy-boto3-sagemaker-geospatial-1.28.15.post1.tar` & `mypy-boto3-sagemaker-geospatial-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:06.217382 mypy-boto3-sagemaker-geospatial-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:58:34.000000 mypy-boto3-sagemaker-geospatial-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18752 2023-07-29 10:04:06.217382 mypy-boto3-sagemaker-geospatial-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17196 2023-07-29 09:58:34.000000 mypy-boto3-sagemaker-geospatial-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:06.205382 mypy-boto3-sagemaker-geospatial-1.28.15.post1/mypy_boto3_sagemaker_geospatial/
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-07-29 09:58:34.000000 mypy-boto3-sagemaker-geospatial-1.28.15.post1/mypy_boto3_sagemaker_geospatial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-29 09:58:34.000000 mypy-boto3-sagemaker-geospatial-1.28.15.post1/mypy_boto3_sagemaker_geospatial/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-07-29 09:58:34.000000 mypy-boto3-sagemaker-geospatial-1.28.15.post1/mypy_boto3_sagemaker_geospatial/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18656 2023-07-29 09:58:34.000000 mypy-boto3-sagemaker-geospatial-1.28.15.post1/mypy_boto3_sagemaker_geospatial/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    18627 2023-07-29 09:58:34.000000 mypy-boto3-sagemaker-geospatial-1.28.15.post1/mypy_boto3_sagemaker_geospatial/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11145 2023-07-29 09:58:34.000000 mypy-boto3-sagemaker-geospatial-1.28.15.post1/mypy_boto3_sagemaker_geospatial/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11143 2023-07-29 09:58:34.000000 mypy-boto3-sagemaker-geospatial-1.28.15.post1/mypy_boto3_sagemaker_geospatial/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4965 2023-07-29 09:58:34.000000 mypy-boto3-sagemaker-geospatial-1.28.15.post1/mypy_boto3_sagemaker_geospatial/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-07-29 09:58:34.000000 mypy-boto3-sagemaker-geospatial-1.28.15.post1/mypy_boto3_sagemaker_geospatial/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:58:34.000000 mypy-boto3-sagemaker-geospatial-1.28.15.post1/mypy_boto3_sagemaker_geospatial/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    39531 2023-07-29 09:58:35.000000 mypy-boto3-sagemaker-geospatial-1.28.15.post1/mypy_boto3_sagemaker_geospatial/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    39483 2023-07-29 09:58:35.000000 mypy-boto3-sagemaker-geospatial-1.28.15.post1/mypy_boto3_sagemaker_geospatial/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:58:34.000000 mypy-boto3-sagemaker-geospatial-1.28.15.post1/mypy_boto3_sagemaker_geospatial/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:06.217382 mypy-boto3-sagemaker-geospatial-1.28.15.post1/mypy_boto3_sagemaker_geospatial.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18752 2023-07-29 10:04:05.000000 mypy-boto3-sagemaker-geospatial-1.28.15.post1/mypy_boto3_sagemaker_geospatial.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-29 10:04:05.000000 mypy-boto3-sagemaker-geospatial-1.28.15.post1/mypy_boto3_sagemaker_geospatial.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:05.000000 mypy-boto3-sagemaker-geospatial-1.28.15.post1/mypy_boto3_sagemaker_geospatial.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:05.000000 mypy-boto3-sagemaker-geospatial-1.28.15.post1/mypy_boto3_sagemaker_geospatial.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:04:05.000000 mypy-boto3-sagemaker-geospatial-1.28.15.post1/mypy_boto3_sagemaker_geospatial.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-29 10:04:05.000000 mypy-boto3-sagemaker-geospatial-1.28.15.post1/mypy_boto3_sagemaker_geospatial.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:04:06.217382 mypy-boto3-sagemaker-geospatial-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-07-29 09:58:34.000000 mypy-boto3-sagemaker-geospatial-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:45.984751 mypy-boto3-sagemaker-geospatial-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:32:01.000000 mypy-boto3-sagemaker-geospatial-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18796 2023-08-01 11:37:45.984751 mypy-boto3-sagemaker-geospatial-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17249 2023-08-01 11:32:01.000000 mypy-boto3-sagemaker-geospatial-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:45.984751 mypy-boto3-sagemaker-geospatial-1.28.16/mypy_boto3_sagemaker_geospatial/
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-08-01 11:32:01.000000 mypy-boto3-sagemaker-geospatial-1.28.16/mypy_boto3_sagemaker_geospatial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-08-01 11:32:01.000000 mypy-boto3-sagemaker-geospatial-1.28.16/mypy_boto3_sagemaker_geospatial/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-08-01 11:32:01.000000 mypy-boto3-sagemaker-geospatial-1.28.16/mypy_boto3_sagemaker_geospatial/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18590 2023-08-01 11:32:06.000000 mypy-boto3-sagemaker-geospatial-1.28.16/mypy_boto3_sagemaker_geospatial/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18561 2023-08-01 11:32:01.000000 mypy-boto3-sagemaker-geospatial-1.28.16/mypy_boto3_sagemaker_geospatial/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11145 2023-08-01 11:32:06.000000 mypy-boto3-sagemaker-geospatial-1.28.16/mypy_boto3_sagemaker_geospatial/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11143 2023-08-01 11:32:06.000000 mypy-boto3-sagemaker-geospatial-1.28.16/mypy_boto3_sagemaker_geospatial/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4965 2023-08-01 11:32:06.000000 mypy-boto3-sagemaker-geospatial-1.28.16/mypy_boto3_sagemaker_geospatial/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-08-01 11:32:06.000000 mypy-boto3-sagemaker-geospatial-1.28.16/mypy_boto3_sagemaker_geospatial/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:32:01.000000 mypy-boto3-sagemaker-geospatial-1.28.16/mypy_boto3_sagemaker_geospatial/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    39706 2023-08-01 11:32:07.000000 mypy-boto3-sagemaker-geospatial-1.28.16/mypy_boto3_sagemaker_geospatial/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39658 2023-08-01 11:32:06.000000 mypy-boto3-sagemaker-geospatial-1.28.16/mypy_boto3_sagemaker_geospatial/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:32:01.000000 mypy-boto3-sagemaker-geospatial-1.28.16/mypy_boto3_sagemaker_geospatial/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:45.984751 mypy-boto3-sagemaker-geospatial-1.28.16/mypy_boto3_sagemaker_geospatial.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18796 2023-08-01 11:37:45.000000 mypy-boto3-sagemaker-geospatial-1.28.16/mypy_boto3_sagemaker_geospatial.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-08-01 11:37:45.000000 mypy-boto3-sagemaker-geospatial-1.28.16/mypy_boto3_sagemaker_geospatial.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:45.000000 mypy-boto3-sagemaker-geospatial-1.28.16/mypy_boto3_sagemaker_geospatial.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:45.000000 mypy-boto3-sagemaker-geospatial-1.28.16/mypy_boto3_sagemaker_geospatial.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:45.000000 mypy-boto3-sagemaker-geospatial-1.28.16/mypy_boto3_sagemaker_geospatial.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-01 11:37:45.000000 mypy-boto3-sagemaker-geospatial-1.28.16/mypy_boto3_sagemaker_geospatial.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:45.984751 mypy-boto3-sagemaker-geospatial-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-08-01 11:32:01.000000 mypy-boto3-sagemaker-geospatial-1.28.16/setup.py
```

### Comparing `mypy-boto3-sagemaker-geospatial-1.28.15.post1/LICENSE` & `mypy-boto3-sagemaker-geospatial-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-geospatial-1.28.15.post1/PKG-INFO` & `mypy-boto3-sagemaker-geospatial-1.28.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sagemaker-geospatial
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.SageMakergeospatialcapabilities 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.SageMakergeospatialcapabilities 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_geospatial/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 sagemaker-geospatial type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 sagemaker-geospatial type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sagemaker-geospatial.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker-geospatial)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_geospatial/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sagemaker-geospatial)](https://pepy.tech/project/mypy-boto3-sagemaker-geospatial)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SageMakergeospatialcapabilities 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities)
+[boto3.SageMakergeospatialcapabilities 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities)
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
 [mypy-boto3-sagemaker-geospatial docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_geospatial/).
 
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
@@ -349,20 +349,20 @@
 )
 
 
 def check_value(value: AlgorithmNameCloudRemovalType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_sagemaker_geospatial.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_sagemaker_geospatial.type_defs import (
     MultiPolygonGeometryInputOutputTypeDef,
     PolygonGeometryInputOutputTypeDef,
     MultiPolygonGeometryInputTypeDef,
     PolygonGeometryInputTypeDef,
@@ -404,20 +404,20 @@
     ListVectorEnrichmentJobOutputConfigTypeDef,
     MapMatchingConfigTypeDef,
     UserDefinedTypeDef,
     PlatformInputTypeDef,
     ViewOffNadirInputTypeDef,
     ViewSunAzimuthInputTypeDef,
     ViewSunElevationInputTypeDef,
-    TimeRangeFilterInputTypeDef,
     TimeRangeFilterOutputTypeDef,
     ReverseGeocodingConfigTypeDef,
     StopEarthObservationJobInputRequestTypeDef,
     StopVectorEnrichmentJobInputRequestTypeDef,
     TagResourceRequestRequestTypeDef,
+    TimestampTypeDef,
     UntagResourceRequestRequestTypeDef,
     AreaOfInterestGeometryOutputTypeDef,
     AreaOfInterestGeometryTypeDef,
     CustomIndicesInputOutputTypeDef,
     CustomIndicesInputTypeDef,
     GetTileOutputTypeDef,
     ListTagsForResourceResponseTypeDef,
@@ -433,14 +433,15 @@
     ListVectorEnrichmentJobInputListVectorEnrichmentJobsPaginateTypeDef,
     ListEarthObservationJobOutputTypeDef,
     ListVectorEnrichmentJobOutputTypeDef,
     OutputResolutionResamplingInputTypeDef,
     OutputResolutionStackInputTypeDef,
     PropertyTypeDef,
     VectorEnrichmentJobConfigTypeDef,
+    TimeRangeFilterInputTypeDef,
     AreaOfInterestOutputTypeDef,
     AreaOfInterestTypeDef,
     BandMathConfigInputOutputTypeDef,
     BandMathConfigInputTypeDef,
     ExportEarthObservationJobInputRequestTypeDef,
     ExportEarthObservationJobOutputTypeDef,
     ExportVectorEnrichmentJobInputRequestTypeDef,
@@ -456,27 +457,28 @@
     GetVectorEnrichmentJobOutputTypeDef,
     StartVectorEnrichmentJobInputRequestTypeDef,
     StartVectorEnrichmentJobOutputTypeDef,
     JobConfigInputOutputTypeDef,
     JobConfigInputTypeDef,
     PropertyFiltersOutputTypeDef,
     PropertyFiltersTypeDef,
+    JobConfigInputUnionTypeDef,
     RasterDataCollectionQueryOutputTypeDef,
     RasterDataCollectionQueryInputTypeDef,
     RasterDataCollectionQueryWithBandFilterInputTypeDef,
     InputConfigOutputTypeDef,
     InputConfigInputTypeDef,
     SearchRasterDataCollectionInputRequestTypeDef,
     GetEarthObservationJobOutputTypeDef,
     StartEarthObservationJobOutputTypeDef,
     StartEarthObservationJobInputRequestTypeDef,
 )
 
 
-def get_structure() -> MultiPolygonGeometryInputOutputTypeDef:
+def get_value() -> MultiPolygonGeometryInputOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-sagemaker-geospatial-1.28.15.post1/README.md` & `mypy-boto3-sagemaker-geospatial-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sagemaker-geospatial.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker-geospatial)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_geospatial/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sagemaker-geospatial)](https://pepy.tech/project/mypy-boto3-sagemaker-geospatial)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SageMakergeospatialcapabilities 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities)
+[boto3.SageMakergeospatialcapabilities 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities)
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
 [mypy-boto3-sagemaker-geospatial docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_geospatial/).
 
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
@@ -317,20 +317,20 @@
 )
 
 
 def check_value(value: AlgorithmNameCloudRemovalType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_sagemaker_geospatial.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_sagemaker_geospatial.type_defs import (
     MultiPolygonGeometryInputOutputTypeDef,
     PolygonGeometryInputOutputTypeDef,
     MultiPolygonGeometryInputTypeDef,
     PolygonGeometryInputTypeDef,
@@ -372,20 +372,20 @@
     ListVectorEnrichmentJobOutputConfigTypeDef,
     MapMatchingConfigTypeDef,
     UserDefinedTypeDef,
     PlatformInputTypeDef,
     ViewOffNadirInputTypeDef,
     ViewSunAzimuthInputTypeDef,
     ViewSunElevationInputTypeDef,
-    TimeRangeFilterInputTypeDef,
     TimeRangeFilterOutputTypeDef,
     ReverseGeocodingConfigTypeDef,
     StopEarthObservationJobInputRequestTypeDef,
     StopVectorEnrichmentJobInputRequestTypeDef,
     TagResourceRequestRequestTypeDef,
+    TimestampTypeDef,
     UntagResourceRequestRequestTypeDef,
     AreaOfInterestGeometryOutputTypeDef,
     AreaOfInterestGeometryTypeDef,
     CustomIndicesInputOutputTypeDef,
     CustomIndicesInputTypeDef,
     GetTileOutputTypeDef,
     ListTagsForResourceResponseTypeDef,
@@ -401,14 +401,15 @@
     ListVectorEnrichmentJobInputListVectorEnrichmentJobsPaginateTypeDef,
     ListEarthObservationJobOutputTypeDef,
     ListVectorEnrichmentJobOutputTypeDef,
     OutputResolutionResamplingInputTypeDef,
     OutputResolutionStackInputTypeDef,
     PropertyTypeDef,
     VectorEnrichmentJobConfigTypeDef,
+    TimeRangeFilterInputTypeDef,
     AreaOfInterestOutputTypeDef,
     AreaOfInterestTypeDef,
     BandMathConfigInputOutputTypeDef,
     BandMathConfigInputTypeDef,
     ExportEarthObservationJobInputRequestTypeDef,
     ExportEarthObservationJobOutputTypeDef,
     ExportVectorEnrichmentJobInputRequestTypeDef,
@@ -424,27 +425,28 @@
     GetVectorEnrichmentJobOutputTypeDef,
     StartVectorEnrichmentJobInputRequestTypeDef,
     StartVectorEnrichmentJobOutputTypeDef,
     JobConfigInputOutputTypeDef,
     JobConfigInputTypeDef,
     PropertyFiltersOutputTypeDef,
     PropertyFiltersTypeDef,
+    JobConfigInputUnionTypeDef,
     RasterDataCollectionQueryOutputTypeDef,
     RasterDataCollectionQueryInputTypeDef,
     RasterDataCollectionQueryWithBandFilterInputTypeDef,
     InputConfigOutputTypeDef,
     InputConfigInputTypeDef,
     SearchRasterDataCollectionInputRequestTypeDef,
     GetEarthObservationJobOutputTypeDef,
     StartEarthObservationJobOutputTypeDef,
     StartEarthObservationJobInputRequestTypeDef,
 )
 
 
-def get_structure() -> MultiPolygonGeometryInputOutputTypeDef:
+def get_value() -> MultiPolygonGeometryInputOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-sagemaker-geospatial-1.28.15.post1/mypy_boto3_sagemaker_geospatial/__init__.py` & `mypy-boto3-sagemaker-geospatial-1.28.16/mypy_boto3_sagemaker_geospatial/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-geospatial-1.28.15.post1/mypy_boto3_sagemaker_geospatial/__init__.pyi` & `mypy-boto3-sagemaker-geospatial-1.28.16/mypy_boto3_sagemaker_geospatial/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-geospatial-1.28.15.post1/mypy_boto3_sagemaker_geospatial/__main__.py` & `mypy-boto3-sagemaker-geospatial-1.28.16/mypy_boto3_sagemaker_geospatial/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SageMakergeospatialcapabilities 1.28.15\nVersion:        "
-        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.SageMakergeospatialcapabilities 1.28.16\nVersion:        "
+        " 1.28.16\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_geospatial//\nBoto3 docs:"
         "     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities\nOther"
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

### Comparing `mypy-boto3-sagemaker-geospatial-1.28.15.post1/mypy_boto3_sagemaker_geospatial/client.py` & `mypy-boto3-sagemaker-geospatial-1.28.16/mypy_boto3_sagemaker_geospatial/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_sagemaker_geospatial.client import SageMakergeospatialcapabilitiesClient
 
     session = Session()
     client: SageMakergeospatialcapabilitiesClient = session.client("sagemaker-geospatial")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     EarthObservationJobStatusType,
     OutputTypeType,
     SortOrderType,
@@ -34,16 +34,15 @@
     ExportVectorEnrichmentJobOutputConfigTypeDef,
     ExportVectorEnrichmentJobOutputTypeDef,
     GetEarthObservationJobOutputTypeDef,
     GetRasterDataCollectionOutputTypeDef,
     GetTileOutputTypeDef,
     GetVectorEnrichmentJobOutputTypeDef,
     InputConfigInputTypeDef,
-    JobConfigInputOutputTypeDef,
-    JobConfigInputTypeDef,
+    JobConfigInputUnionTypeDef,
     ListEarthObservationJobOutputTypeDef,
     ListRasterDataCollectionsOutputTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListVectorEnrichmentJobOutputTypeDef,
     OutputConfigInputTypeDef,
     RasterDataCollectionQueryWithBandFilterInputTypeDef,
     SearchRasterDataCollectionOutputTypeDef,
@@ -292,15 +291,15 @@
         """
 
     def start_earth_observation_job(
         self,
         *,
         ExecutionRoleArn: str,
         InputConfig: InputConfigInputTypeDef,
-        JobConfig: Union[JobConfigInputTypeDef, JobConfigInputOutputTypeDef],
+        JobConfig: JobConfigInputUnionTypeDef,
         Name: str,
         ClientToken: str = ...,
         KmsKeyId: str = ...,
         Tags: Mapping[str, str] = ...
     ) -> StartEarthObservationJobOutputTypeDef:
         """
         Use this operation to create an Earth observation job.
```

### Comparing `mypy-boto3-sagemaker-geospatial-1.28.15.post1/mypy_boto3_sagemaker_geospatial/client.pyi` & `mypy-boto3-sagemaker-geospatial-1.28.16/mypy_boto3_sagemaker_geospatial/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_sagemaker_geospatial.client import SageMakergeospatialcapabilitiesClient
 
     session = Session()
     client: SageMakergeospatialcapabilitiesClient = session.client("sagemaker-geospatial")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     EarthObservationJobStatusType,
     OutputTypeType,
     SortOrderType,
@@ -34,16 +34,15 @@
     ExportVectorEnrichmentJobOutputConfigTypeDef,
     ExportVectorEnrichmentJobOutputTypeDef,
     GetEarthObservationJobOutputTypeDef,
     GetRasterDataCollectionOutputTypeDef,
     GetTileOutputTypeDef,
     GetVectorEnrichmentJobOutputTypeDef,
     InputConfigInputTypeDef,
-    JobConfigInputOutputTypeDef,
-    JobConfigInputTypeDef,
+    JobConfigInputUnionTypeDef,
     ListEarthObservationJobOutputTypeDef,
     ListRasterDataCollectionsOutputTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListVectorEnrichmentJobOutputTypeDef,
     OutputConfigInputTypeDef,
     RasterDataCollectionQueryWithBandFilterInputTypeDef,
     SearchRasterDataCollectionOutputTypeDef,
@@ -271,15 +270,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_geospatial/client/#search_raster_data_collection)
         """
     def start_earth_observation_job(
         self,
         *,
         ExecutionRoleArn: str,
         InputConfig: InputConfigInputTypeDef,
-        JobConfig: Union[JobConfigInputTypeDef, JobConfigInputOutputTypeDef],
+        JobConfig: JobConfigInputUnionTypeDef,
         Name: str,
         ClientToken: str = ...,
         KmsKeyId: str = ...,
         Tags: Mapping[str, str] = ...
     ) -> StartEarthObservationJobOutputTypeDef:
         """
         Use this operation to create an Earth observation job.
```

### Comparing `mypy-boto3-sagemaker-geospatial-1.28.15.post1/mypy_boto3_sagemaker_geospatial/literals.py` & `mypy-boto3-sagemaker-geospatial-1.28.16/mypy_boto3_sagemaker_geospatial/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-geospatial-1.28.15.post1/mypy_boto3_sagemaker_geospatial/literals.pyi` & `mypy-boto3-sagemaker-geospatial-1.28.16/mypy_boto3_sagemaker_geospatial/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-geospatial-1.28.15.post1/mypy_boto3_sagemaker_geospatial/paginator.py` & `mypy-boto3-sagemaker-geospatial-1.28.16/mypy_boto3_sagemaker_geospatial/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-geospatial-1.28.15.post1/mypy_boto3_sagemaker_geospatial/paginator.pyi` & `mypy-boto3-sagemaker-geospatial-1.28.16/mypy_boto3_sagemaker_geospatial/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-geospatial-1.28.15.post1/mypy_boto3_sagemaker_geospatial/type_defs.py` & `mypy-boto3-sagemaker-geospatial-1.28.16/mypy_boto3_sagemaker_geospatial/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_geospatial/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_sagemaker_geospatial.type_defs import MultiPolygonGeometryInputOutputTypeDef
 
-    data: MultiPolygonGeometryInputOutputTypeDef = {...}
+    data: MultiPolygonGeometryInputOutputTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -93,20 +93,20 @@
     "ListVectorEnrichmentJobOutputConfigTypeDef",
     "MapMatchingConfigTypeDef",
     "UserDefinedTypeDef",
     "PlatformInputTypeDef",
     "ViewOffNadirInputTypeDef",
     "ViewSunAzimuthInputTypeDef",
     "ViewSunElevationInputTypeDef",
-    "TimeRangeFilterInputTypeDef",
     "TimeRangeFilterOutputTypeDef",
     "ReverseGeocodingConfigTypeDef",
     "StopEarthObservationJobInputRequestTypeDef",
     "StopVectorEnrichmentJobInputRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "TimestampTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "AreaOfInterestGeometryOutputTypeDef",
     "AreaOfInterestGeometryTypeDef",
     "CustomIndicesInputOutputTypeDef",
     "CustomIndicesInputTypeDef",
     "GetTileOutputTypeDef",
     "ListTagsForResourceResponseTypeDef",
@@ -122,14 +122,15 @@
     "ListVectorEnrichmentJobInputListVectorEnrichmentJobsPaginateTypeDef",
     "ListEarthObservationJobOutputTypeDef",
     "ListVectorEnrichmentJobOutputTypeDef",
     "OutputResolutionResamplingInputTypeDef",
     "OutputResolutionStackInputTypeDef",
     "PropertyTypeDef",
     "VectorEnrichmentJobConfigTypeDef",
+    "TimeRangeFilterInputTypeDef",
     "AreaOfInterestOutputTypeDef",
     "AreaOfInterestTypeDef",
     "BandMathConfigInputOutputTypeDef",
     "BandMathConfigInputTypeDef",
     "ExportEarthObservationJobInputRequestTypeDef",
     "ExportEarthObservationJobOutputTypeDef",
     "ExportVectorEnrichmentJobInputRequestTypeDef",
@@ -145,14 +146,15 @@
     "GetVectorEnrichmentJobOutputTypeDef",
     "StartVectorEnrichmentJobInputRequestTypeDef",
     "StartVectorEnrichmentJobOutputTypeDef",
     "JobConfigInputOutputTypeDef",
     "JobConfigInputTypeDef",
     "PropertyFiltersOutputTypeDef",
     "PropertyFiltersTypeDef",
+    "JobConfigInputUnionTypeDef",
     "RasterDataCollectionQueryOutputTypeDef",
     "RasterDataCollectionQueryInputTypeDef",
     "RasterDataCollectionQueryWithBandFilterInputTypeDef",
     "InputConfigOutputTypeDef",
     "InputConfigInputTypeDef",
     "SearchRasterDataCollectionInputRequestTypeDef",
     "GetEarthObservationJobOutputTypeDef",
@@ -728,22 +730,14 @@
     "ViewSunElevationInputTypeDef",
     {
         "LowerBound": float,
         "UpperBound": float,
     },
 )
 
-TimeRangeFilterInputTypeDef = TypedDict(
-    "TimeRangeFilterInputTypeDef",
-    {
-        "EndTime": Union[datetime, str],
-        "StartTime": Union[datetime, str],
-    },
-)
-
 TimeRangeFilterOutputTypeDef = TypedDict(
     "TimeRangeFilterOutputTypeDef",
     {
         "EndTime": datetime,
         "StartTime": datetime,
     },
 )
@@ -774,14 +768,15 @@
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
 
+TimestampTypeDef = Union[datetime, str]
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -1012,14 +1007,22 @@
     {
         "MapMatchingConfig": MapMatchingConfigTypeDef,
         "ReverseGeocodingConfig": ReverseGeocodingConfigTypeDef,
     },
     total=False,
 )
 
+TimeRangeFilterInputTypeDef = TypedDict(
+    "TimeRangeFilterInputTypeDef",
+    {
+        "EndTime": TimestampTypeDef,
+        "StartTime": TimestampTypeDef,
+    },
+)
+
 AreaOfInterestOutputTypeDef = TypedDict(
     "AreaOfInterestOutputTypeDef",
     {
         "AreaOfInterestGeometry": AreaOfInterestGeometryOutputTypeDef,
     },
     total=False,
 )
@@ -1332,14 +1335,15 @@
     {
         "LogicalOperator": Literal["AND"],
         "Properties": Sequence[PropertyFilterTypeDef],
     },
     total=False,
 )
 
+JobConfigInputUnionTypeDef = Union[JobConfigInputTypeDef, JobConfigInputOutputTypeDef]
 _RequiredRasterDataCollectionQueryOutputTypeDef = TypedDict(
     "_RequiredRasterDataCollectionQueryOutputTypeDef",
     {
         "RasterDataCollectionArn": str,
         "RasterDataCollectionName": str,
         "TimeRangeFilter": TimeRangeFilterOutputTypeDef,
     },
```

### Comparing `mypy-boto3-sagemaker-geospatial-1.28.15.post1/mypy_boto3_sagemaker_geospatial/type_defs.pyi` & `mypy-boto3-sagemaker-geospatial-1.28.16/mypy_boto3_sagemaker_geospatial/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_geospatial/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_sagemaker_geospatial.type_defs import MultiPolygonGeometryInputOutputTypeDef
 
-    data: MultiPolygonGeometryInputOutputTypeDef = {...}
+    data: MultiPolygonGeometryInputOutputTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -92,20 +92,20 @@
     "ListVectorEnrichmentJobOutputConfigTypeDef",
     "MapMatchingConfigTypeDef",
     "UserDefinedTypeDef",
     "PlatformInputTypeDef",
     "ViewOffNadirInputTypeDef",
     "ViewSunAzimuthInputTypeDef",
     "ViewSunElevationInputTypeDef",
-    "TimeRangeFilterInputTypeDef",
     "TimeRangeFilterOutputTypeDef",
     "ReverseGeocodingConfigTypeDef",
     "StopEarthObservationJobInputRequestTypeDef",
     "StopVectorEnrichmentJobInputRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "TimestampTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "AreaOfInterestGeometryOutputTypeDef",
     "AreaOfInterestGeometryTypeDef",
     "CustomIndicesInputOutputTypeDef",
     "CustomIndicesInputTypeDef",
     "GetTileOutputTypeDef",
     "ListTagsForResourceResponseTypeDef",
@@ -121,14 +121,15 @@
     "ListVectorEnrichmentJobInputListVectorEnrichmentJobsPaginateTypeDef",
     "ListEarthObservationJobOutputTypeDef",
     "ListVectorEnrichmentJobOutputTypeDef",
     "OutputResolutionResamplingInputTypeDef",
     "OutputResolutionStackInputTypeDef",
     "PropertyTypeDef",
     "VectorEnrichmentJobConfigTypeDef",
+    "TimeRangeFilterInputTypeDef",
     "AreaOfInterestOutputTypeDef",
     "AreaOfInterestTypeDef",
     "BandMathConfigInputOutputTypeDef",
     "BandMathConfigInputTypeDef",
     "ExportEarthObservationJobInputRequestTypeDef",
     "ExportEarthObservationJobOutputTypeDef",
     "ExportVectorEnrichmentJobInputRequestTypeDef",
@@ -144,14 +145,15 @@
     "GetVectorEnrichmentJobOutputTypeDef",
     "StartVectorEnrichmentJobInputRequestTypeDef",
     "StartVectorEnrichmentJobOutputTypeDef",
     "JobConfigInputOutputTypeDef",
     "JobConfigInputTypeDef",
     "PropertyFiltersOutputTypeDef",
     "PropertyFiltersTypeDef",
+    "JobConfigInputUnionTypeDef",
     "RasterDataCollectionQueryOutputTypeDef",
     "RasterDataCollectionQueryInputTypeDef",
     "RasterDataCollectionQueryWithBandFilterInputTypeDef",
     "InputConfigOutputTypeDef",
     "InputConfigInputTypeDef",
     "SearchRasterDataCollectionInputRequestTypeDef",
     "GetEarthObservationJobOutputTypeDef",
@@ -703,22 +705,14 @@
     "ViewSunElevationInputTypeDef",
     {
         "LowerBound": float,
         "UpperBound": float,
     },
 )
 
-TimeRangeFilterInputTypeDef = TypedDict(
-    "TimeRangeFilterInputTypeDef",
-    {
-        "EndTime": Union[datetime, str],
-        "StartTime": Union[datetime, str],
-    },
-)
-
 TimeRangeFilterOutputTypeDef = TypedDict(
     "TimeRangeFilterOutputTypeDef",
     {
         "EndTime": datetime,
         "StartTime": datetime,
     },
 )
@@ -749,14 +743,15 @@
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
 
+TimestampTypeDef = Union[datetime, str]
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -983,14 +978,22 @@
     {
         "MapMatchingConfig": MapMatchingConfigTypeDef,
         "ReverseGeocodingConfig": ReverseGeocodingConfigTypeDef,
     },
     total=False,
 )
 
+TimeRangeFilterInputTypeDef = TypedDict(
+    "TimeRangeFilterInputTypeDef",
+    {
+        "EndTime": TimestampTypeDef,
+        "StartTime": TimestampTypeDef,
+    },
+)
+
 AreaOfInterestOutputTypeDef = TypedDict(
     "AreaOfInterestOutputTypeDef",
     {
         "AreaOfInterestGeometry": AreaOfInterestGeometryOutputTypeDef,
     },
     total=False,
 )
@@ -1293,14 +1296,15 @@
     {
         "LogicalOperator": Literal["AND"],
         "Properties": Sequence[PropertyFilterTypeDef],
     },
     total=False,
 )
 
+JobConfigInputUnionTypeDef = Union[JobConfigInputTypeDef, JobConfigInputOutputTypeDef]
 _RequiredRasterDataCollectionQueryOutputTypeDef = TypedDict(
     "_RequiredRasterDataCollectionQueryOutputTypeDef",
     {
         "RasterDataCollectionArn": str,
         "RasterDataCollectionName": str,
         "TimeRangeFilter": TimeRangeFilterOutputTypeDef,
     },
```

### Comparing `mypy-boto3-sagemaker-geospatial-1.28.15.post1/mypy_boto3_sagemaker_geospatial.egg-info/PKG-INFO` & `mypy-boto3-sagemaker-geospatial-1.28.16/mypy_boto3_sagemaker_geospatial.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sagemaker-geospatial
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.SageMakergeospatialcapabilities 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.SageMakergeospatialcapabilities 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_geospatial/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 sagemaker-geospatial type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 sagemaker-geospatial type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sagemaker-geospatial.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker-geospatial)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_geospatial/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sagemaker-geospatial)](https://pepy.tech/project/mypy-boto3-sagemaker-geospatial)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SageMakergeospatialcapabilities 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities)
+[boto3.SageMakergeospatialcapabilities 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities)
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
 [mypy-boto3-sagemaker-geospatial docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_geospatial/).
 
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
@@ -349,20 +349,20 @@
 )
 
 
 def check_value(value: AlgorithmNameCloudRemovalType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_sagemaker_geospatial.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_sagemaker_geospatial.type_defs import (
     MultiPolygonGeometryInputOutputTypeDef,
     PolygonGeometryInputOutputTypeDef,
     MultiPolygonGeometryInputTypeDef,
     PolygonGeometryInputTypeDef,
@@ -404,20 +404,20 @@
     ListVectorEnrichmentJobOutputConfigTypeDef,
     MapMatchingConfigTypeDef,
     UserDefinedTypeDef,
     PlatformInputTypeDef,
     ViewOffNadirInputTypeDef,
     ViewSunAzimuthInputTypeDef,
     ViewSunElevationInputTypeDef,
-    TimeRangeFilterInputTypeDef,
     TimeRangeFilterOutputTypeDef,
     ReverseGeocodingConfigTypeDef,
     StopEarthObservationJobInputRequestTypeDef,
     StopVectorEnrichmentJobInputRequestTypeDef,
     TagResourceRequestRequestTypeDef,
+    TimestampTypeDef,
     UntagResourceRequestRequestTypeDef,
     AreaOfInterestGeometryOutputTypeDef,
     AreaOfInterestGeometryTypeDef,
     CustomIndicesInputOutputTypeDef,
     CustomIndicesInputTypeDef,
     GetTileOutputTypeDef,
     ListTagsForResourceResponseTypeDef,
@@ -433,14 +433,15 @@
     ListVectorEnrichmentJobInputListVectorEnrichmentJobsPaginateTypeDef,
     ListEarthObservationJobOutputTypeDef,
     ListVectorEnrichmentJobOutputTypeDef,
     OutputResolutionResamplingInputTypeDef,
     OutputResolutionStackInputTypeDef,
     PropertyTypeDef,
     VectorEnrichmentJobConfigTypeDef,
+    TimeRangeFilterInputTypeDef,
     AreaOfInterestOutputTypeDef,
     AreaOfInterestTypeDef,
     BandMathConfigInputOutputTypeDef,
     BandMathConfigInputTypeDef,
     ExportEarthObservationJobInputRequestTypeDef,
     ExportEarthObservationJobOutputTypeDef,
     ExportVectorEnrichmentJobInputRequestTypeDef,
@@ -456,27 +457,28 @@
     GetVectorEnrichmentJobOutputTypeDef,
     StartVectorEnrichmentJobInputRequestTypeDef,
     StartVectorEnrichmentJobOutputTypeDef,
     JobConfigInputOutputTypeDef,
     JobConfigInputTypeDef,
     PropertyFiltersOutputTypeDef,
     PropertyFiltersTypeDef,
+    JobConfigInputUnionTypeDef,
     RasterDataCollectionQueryOutputTypeDef,
     RasterDataCollectionQueryInputTypeDef,
     RasterDataCollectionQueryWithBandFilterInputTypeDef,
     InputConfigOutputTypeDef,
     InputConfigInputTypeDef,
     SearchRasterDataCollectionInputRequestTypeDef,
     GetEarthObservationJobOutputTypeDef,
     StartEarthObservationJobOutputTypeDef,
     StartEarthObservationJobInputRequestTypeDef,
 )
 
 
-def get_structure() -> MultiPolygonGeometryInputOutputTypeDef:
+def get_value() -> MultiPolygonGeometryInputOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-sagemaker-geospatial-1.28.15.post1/mypy_boto3_sagemaker_geospatial.egg-info/SOURCES.txt` & `mypy-boto3-sagemaker-geospatial-1.28.16/mypy_boto3_sagemaker_geospatial.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-geospatial-1.28.15.post1/setup.py` & `mypy-boto3-sagemaker-geospatial-1.28.16/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-sagemaker-geospatial",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_sagemaker_geospatial"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.SageMakergeospatialcapabilities 1.28.15 service generated with"
-        " mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.SageMakergeospatialcapabilities 1.28.16 service generated with"
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
-    keywords="boto3 sagemaker-geospatial type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 sagemaker-geospatial type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_sagemaker_geospatial": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_geospatial/"
```

