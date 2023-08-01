# Comparing `tmp/mypy-boto3-medical-imaging-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-medical-imaging-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-medical-imaging-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:40 2023, max compression
+gzip compressed data, was "mypy-boto3-medical-imaging-1.28.16.tar", last modified: Tue Aug  1 11:37:20 2023, max compression
```

## Comparing `mypy-boto3-medical-imaging-1.28.15.post1.tar` & `mypy-boto3-medical-imaging-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:40.921285 mypy-boto3-medical-imaging-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:51:25.000000 mypy-boto3-medical-imaging-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15858 2023-07-29 10:03:40.913285 mypy-boto3-medical-imaging-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14335 2023-07-29 09:51:25.000000 mypy-boto3-medical-imaging-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:40.897285 mypy-boto3-medical-imaging-1.28.15.post1/mypy_boto3_medical_imaging/
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-07-29 09:51:25.000000 mypy-boto3-medical-imaging-1.28.15.post1/mypy_boto3_medical_imaging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-07-29 09:51:25.000000 mypy-boto3-medical-imaging-1.28.15.post1/mypy_boto3_medical_imaging/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-29 09:51:25.000000 mypy-boto3-medical-imaging-1.28.15.post1/mypy_boto3_medical_imaging/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16223 2023-07-29 09:51:25.000000 mypy-boto3-medical-imaging-1.28.15.post1/mypy_boto3_medical_imaging/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    16194 2023-07-29 09:51:25.000000 mypy-boto3-medical-imaging-1.28.15.post1/mypy_boto3_medical_imaging/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8812 2023-07-29 09:51:25.000000 mypy-boto3-medical-imaging-1.28.15.post1/mypy_boto3_medical_imaging/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8810 2023-07-29 09:51:25.000000 mypy-boto3-medical-imaging-1.28.15.post1/mypy_boto3_medical_imaging/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5618 2023-07-29 09:51:25.000000 mypy-boto3-medical-imaging-1.28.15.post1/mypy_boto3_medical_imaging/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5612 2023-07-29 09:51:25.000000 mypy-boto3-medical-imaging-1.28.15.post1/mypy_boto3_medical_imaging/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:51:25.000000 mypy-boto3-medical-imaging-1.28.15.post1/mypy_boto3_medical_imaging/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    24194 2023-07-29 09:51:26.000000 mypy-boto3-medical-imaging-1.28.15.post1/mypy_boto3_medical_imaging/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    24154 2023-07-29 09:51:26.000000 mypy-boto3-medical-imaging-1.28.15.post1/mypy_boto3_medical_imaging/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:51:25.000000 mypy-boto3-medical-imaging-1.28.15.post1/mypy_boto3_medical_imaging/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:40.913285 mypy-boto3-medical-imaging-1.28.15.post1/mypy_boto3_medical_imaging.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15858 2023-07-29 10:03:40.000000 mypy-boto3-medical-imaging-1.28.15.post1/mypy_boto3_medical_imaging.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-29 10:03:40.000000 mypy-boto3-medical-imaging-1.28.15.post1/mypy_boto3_medical_imaging.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:40.000000 mypy-boto3-medical-imaging-1.28.15.post1/mypy_boto3_medical_imaging.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:40.000000 mypy-boto3-medical-imaging-1.28.15.post1/mypy_boto3_medical_imaging.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:40.000000 mypy-boto3-medical-imaging-1.28.15.post1/mypy_boto3_medical_imaging.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-29 10:03:40.000000 mypy-boto3-medical-imaging-1.28.15.post1/mypy_boto3_medical_imaging.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:40.921285 mypy-boto3-medical-imaging-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-07-29 09:51:25.000000 mypy-boto3-medical-imaging-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:20.696821 mypy-boto3-medical-imaging-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:24:21.000000 mypy-boto3-medical-imaging-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15858 2023-08-01 11:37:20.688821 mypy-boto3-medical-imaging-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14344 2023-08-01 11:24:21.000000 mypy-boto3-medical-imaging-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:20.688821 mypy-boto3-medical-imaging-1.28.16/mypy_boto3_medical_imaging/
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-08-01 11:24:21.000000 mypy-boto3-medical-imaging-1.28.16/mypy_boto3_medical_imaging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-08-01 11:24:21.000000 mypy-boto3-medical-imaging-1.28.16/mypy_boto3_medical_imaging/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-08-01 11:24:21.000000 mypy-boto3-medical-imaging-1.28.16/mypy_boto3_medical_imaging/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16223 2023-08-01 11:24:21.000000 mypy-boto3-medical-imaging-1.28.16/mypy_boto3_medical_imaging/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16194 2023-08-01 11:24:21.000000 mypy-boto3-medical-imaging-1.28.16/mypy_boto3_medical_imaging/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8812 2023-08-01 11:24:22.000000 mypy-boto3-medical-imaging-1.28.16/mypy_boto3_medical_imaging/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8810 2023-08-01 11:24:21.000000 mypy-boto3-medical-imaging-1.28.16/mypy_boto3_medical_imaging/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5618 2023-08-01 11:24:21.000000 mypy-boto3-medical-imaging-1.28.16/mypy_boto3_medical_imaging/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5612 2023-08-01 11:24:21.000000 mypy-boto3-medical-imaging-1.28.16/mypy_boto3_medical_imaging/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:24:21.000000 mypy-boto3-medical-imaging-1.28.16/mypy_boto3_medical_imaging/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    24209 2023-08-01 11:24:22.000000 mypy-boto3-medical-imaging-1.28.16/mypy_boto3_medical_imaging/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24169 2023-08-01 11:24:22.000000 mypy-boto3-medical-imaging-1.28.16/mypy_boto3_medical_imaging/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:24:21.000000 mypy-boto3-medical-imaging-1.28.16/mypy_boto3_medical_imaging/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:20.688821 mypy-boto3-medical-imaging-1.28.16/mypy_boto3_medical_imaging.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15858 2023-08-01 11:37:20.000000 mypy-boto3-medical-imaging-1.28.16/mypy_boto3_medical_imaging.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-08-01 11:37:20.000000 mypy-boto3-medical-imaging-1.28.16/mypy_boto3_medical_imaging.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:20.000000 mypy-boto3-medical-imaging-1.28.16/mypy_boto3_medical_imaging.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:20.000000 mypy-boto3-medical-imaging-1.28.16/mypy_boto3_medical_imaging.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:20.000000 mypy-boto3-medical-imaging-1.28.16/mypy_boto3_medical_imaging.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-01 11:37:20.000000 mypy-boto3-medical-imaging-1.28.16/mypy_boto3_medical_imaging.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:20.696821 mypy-boto3-medical-imaging-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-08-01 11:24:21.000000 mypy-boto3-medical-imaging-1.28.16/setup.py
```

### Comparing `mypy-boto3-medical-imaging-1.28.15.post1/LICENSE` & `mypy-boto3-medical-imaging-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-medical-imaging-1.28.15.post1/PKG-INFO` & `mypy-boto3-medical-imaging-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-medical-imaging
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.HealthImaging 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.HealthImaging 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medical_imaging/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 medical-imaging type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 medical-imaging type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-medical-imaging.svg?color=blue)](https://pypi.org/project/mypy-boto3-medical-imaging)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medical_imaging/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-medical-imaging)](https://pepy.tech/project/mypy-boto3-medical-imaging)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.HealthImaging 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging)
+[boto3.HealthImaging 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging)
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
 [mypy-boto3-medical-imaging docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medical_imaging/).
 
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
@@ -330,34 +330,34 @@
 )
 
 
 def check_value(value: DatastoreStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_medical_imaging.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_medical_imaging.type_defs import (
+    BlobTypeDef,
     CopyDestinationImageSetPropertiesTypeDef,
     CopyDestinationImageSetTypeDef,
     CopySourceImageSetInformationTypeDef,
     CopySourceImageSetPropertiesTypeDef,
     ResponseMetadataTypeDef,
     CreateDatastoreRequestRequestTypeDef,
     DICOMImportJobPropertiesTypeDef,
     DICOMImportJobSummaryTypeDef,
     DICOMStudyDateAndTimeTypeDef,
     DICOMTagsTypeDef,
-    DICOMUpdatesTypeDef,
     DatastorePropertiesTypeDef,
     DatastoreSummaryTypeDef,
     DeleteDatastoreRequestRequestTypeDef,
     DeleteImageSetRequestRequestTypeDef,
     GetDICOMImportJobRequestRequestTypeDef,
     GetDatastoreRequestRequestTypeDef,
     ImageFrameInformationTypeDef,
@@ -365,51 +365,53 @@
     GetImageSetRequestRequestTypeDef,
     ImageSetPropertiesTypeDef,
     PaginatorConfigTypeDef,
     ListDICOMImportJobsRequestRequestTypeDef,
     ListDatastoresRequestRequestTypeDef,
     ListImageSetVersionsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TimestampTypeDef,
     StartDICOMImportJobRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    DICOMUpdatesTypeDef,
     CopyImageSetInformationTypeDef,
     CopyImageSetResponseTypeDef,
     CreateDatastoreResponseTypeDef,
     DeleteDatastoreResponseTypeDef,
     DeleteImageSetResponseTypeDef,
     GetImageFrameResponseTypeDef,
     GetImageSetMetadataResponseTypeDef,
     GetImageSetResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     StartDICOMImportJobResponseTypeDef,
     UpdateImageSetMetadataResponseTypeDef,
     GetDICOMImportJobResponseTypeDef,
     ListDICOMImportJobsResponseTypeDef,
-    SearchByAttributeValueTypeDef,
     ImageSetsMetadataSummaryTypeDef,
-    MetadataUpdatesTypeDef,
     GetDatastoreResponseTypeDef,
     ListDatastoresResponseTypeDef,
     GetImageFrameRequestRequestTypeDef,
     ListImageSetVersionsResponseTypeDef,
     ListDICOMImportJobsRequestListDICOMImportJobsPaginateTypeDef,
     ListDatastoresRequestListDatastoresPaginateTypeDef,
     ListImageSetVersionsRequestListImageSetVersionsPaginateTypeDef,
+    SearchByAttributeValueTypeDef,
+    MetadataUpdatesTypeDef,
     CopyImageSetRequestRequestTypeDef,
-    SearchFilterTypeDef,
     SearchImageSetsResponseTypeDef,
+    SearchFilterTypeDef,
     UpdateImageSetMetadataRequestRequestTypeDef,
     SearchCriteriaTypeDef,
     SearchImageSetsRequestRequestTypeDef,
     SearchImageSetsRequestSearchImageSetsPaginateTypeDef,
 )
 
 
-def get_structure() -> CopyDestinationImageSetPropertiesTypeDef:
+def get_value() -> BlobTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-medical-imaging-1.28.15.post1/README.md` & `mypy-boto3-medical-imaging-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-medical-imaging.svg?color=blue)](https://pypi.org/project/mypy-boto3-medical-imaging)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medical_imaging/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-medical-imaging)](https://pepy.tech/project/mypy-boto3-medical-imaging)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.HealthImaging 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging)
+[boto3.HealthImaging 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging)
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
 [mypy-boto3-medical-imaging docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medical_imaging/).
 
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
@@ -298,34 +298,34 @@
 )
 
 
 def check_value(value: DatastoreStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_medical_imaging.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_medical_imaging.type_defs import (
+    BlobTypeDef,
     CopyDestinationImageSetPropertiesTypeDef,
     CopyDestinationImageSetTypeDef,
     CopySourceImageSetInformationTypeDef,
     CopySourceImageSetPropertiesTypeDef,
     ResponseMetadataTypeDef,
     CreateDatastoreRequestRequestTypeDef,
     DICOMImportJobPropertiesTypeDef,
     DICOMImportJobSummaryTypeDef,
     DICOMStudyDateAndTimeTypeDef,
     DICOMTagsTypeDef,
-    DICOMUpdatesTypeDef,
     DatastorePropertiesTypeDef,
     DatastoreSummaryTypeDef,
     DeleteDatastoreRequestRequestTypeDef,
     DeleteImageSetRequestRequestTypeDef,
     GetDICOMImportJobRequestRequestTypeDef,
     GetDatastoreRequestRequestTypeDef,
     ImageFrameInformationTypeDef,
@@ -333,51 +333,53 @@
     GetImageSetRequestRequestTypeDef,
     ImageSetPropertiesTypeDef,
     PaginatorConfigTypeDef,
     ListDICOMImportJobsRequestRequestTypeDef,
     ListDatastoresRequestRequestTypeDef,
     ListImageSetVersionsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TimestampTypeDef,
     StartDICOMImportJobRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    DICOMUpdatesTypeDef,
     CopyImageSetInformationTypeDef,
     CopyImageSetResponseTypeDef,
     CreateDatastoreResponseTypeDef,
     DeleteDatastoreResponseTypeDef,
     DeleteImageSetResponseTypeDef,
     GetImageFrameResponseTypeDef,
     GetImageSetMetadataResponseTypeDef,
     GetImageSetResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     StartDICOMImportJobResponseTypeDef,
     UpdateImageSetMetadataResponseTypeDef,
     GetDICOMImportJobResponseTypeDef,
     ListDICOMImportJobsResponseTypeDef,
-    SearchByAttributeValueTypeDef,
     ImageSetsMetadataSummaryTypeDef,
-    MetadataUpdatesTypeDef,
     GetDatastoreResponseTypeDef,
     ListDatastoresResponseTypeDef,
     GetImageFrameRequestRequestTypeDef,
     ListImageSetVersionsResponseTypeDef,
     ListDICOMImportJobsRequestListDICOMImportJobsPaginateTypeDef,
     ListDatastoresRequestListDatastoresPaginateTypeDef,
     ListImageSetVersionsRequestListImageSetVersionsPaginateTypeDef,
+    SearchByAttributeValueTypeDef,
+    MetadataUpdatesTypeDef,
     CopyImageSetRequestRequestTypeDef,
-    SearchFilterTypeDef,
     SearchImageSetsResponseTypeDef,
+    SearchFilterTypeDef,
     UpdateImageSetMetadataRequestRequestTypeDef,
     SearchCriteriaTypeDef,
     SearchImageSetsRequestRequestTypeDef,
     SearchImageSetsRequestSearchImageSetsPaginateTypeDef,
 )
 
 
-def get_structure() -> CopyDestinationImageSetPropertiesTypeDef:
+def get_value() -> BlobTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-medical-imaging-1.28.15.post1/mypy_boto3_medical_imaging/__init__.py` & `mypy-boto3-medical-imaging-1.28.16/mypy_boto3_medical_imaging/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-medical-imaging-1.28.15.post1/mypy_boto3_medical_imaging/__init__.pyi` & `mypy-boto3-medical-imaging-1.28.16/mypy_boto3_medical_imaging/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-medical-imaging-1.28.15.post1/mypy_boto3_medical_imaging/__main__.py` & `mypy-boto3-medical-imaging-1.28.16/mypy_boto3_medical_imaging/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.HealthImaging 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.HealthImaging 1.28.16\nVersion:         1.28.16\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medical_imaging//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging\nOther"
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

### Comparing `mypy-boto3-medical-imaging-1.28.15.post1/mypy_boto3_medical_imaging/client.py` & `mypy-boto3-medical-imaging-1.28.16/mypy_boto3_medical_imaging/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-medical-imaging-1.28.15.post1/mypy_boto3_medical_imaging/client.pyi` & `mypy-boto3-medical-imaging-1.28.16/mypy_boto3_medical_imaging/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-medical-imaging-1.28.15.post1/mypy_boto3_medical_imaging/literals.py` & `mypy-boto3-medical-imaging-1.28.16/mypy_boto3_medical_imaging/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-medical-imaging-1.28.15.post1/mypy_boto3_medical_imaging/literals.pyi` & `mypy-boto3-medical-imaging-1.28.16/mypy_boto3_medical_imaging/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-medical-imaging-1.28.15.post1/mypy_boto3_medical_imaging/paginator.py` & `mypy-boto3-medical-imaging-1.28.16/mypy_boto3_medical_imaging/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-medical-imaging-1.28.15.post1/mypy_boto3_medical_imaging/paginator.pyi` & `mypy-boto3-medical-imaging-1.28.16/mypy_boto3_medical_imaging/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-medical-imaging-1.28.15.post1/mypy_boto3_medical_imaging/type_defs.py` & `mypy-boto3-medical-imaging-1.28.16/mypy_boto3_medical_imaging/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for medical-imaging service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medical_imaging/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_medical_imaging.type_defs import CopyDestinationImageSetPropertiesTypeDef
+    from mypy_boto3_medical_imaging.type_defs import BlobTypeDef
 
-    data: CopyDestinationImageSetPropertiesTypeDef = {...}
+    data: BlobTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -28,25 +28,25 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
+    "BlobTypeDef",
     "CopyDestinationImageSetPropertiesTypeDef",
     "CopyDestinationImageSetTypeDef",
     "CopySourceImageSetInformationTypeDef",
     "CopySourceImageSetPropertiesTypeDef",
     "ResponseMetadataTypeDef",
     "CreateDatastoreRequestRequestTypeDef",
     "DICOMImportJobPropertiesTypeDef",
     "DICOMImportJobSummaryTypeDef",
     "DICOMStudyDateAndTimeTypeDef",
     "DICOMTagsTypeDef",
-    "DICOMUpdatesTypeDef",
     "DatastorePropertiesTypeDef",
     "DatastoreSummaryTypeDef",
     "DeleteDatastoreRequestRequestTypeDef",
     "DeleteImageSetRequestRequestTypeDef",
     "GetDICOMImportJobRequestRequestTypeDef",
     "GetDatastoreRequestRequestTypeDef",
     "ImageFrameInformationTypeDef",
@@ -54,49 +54,52 @@
     "GetImageSetRequestRequestTypeDef",
     "ImageSetPropertiesTypeDef",
     "PaginatorConfigTypeDef",
     "ListDICOMImportJobsRequestRequestTypeDef",
     "ListDatastoresRequestRequestTypeDef",
     "ListImageSetVersionsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "TimestampTypeDef",
     "StartDICOMImportJobRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "DICOMUpdatesTypeDef",
     "CopyImageSetInformationTypeDef",
     "CopyImageSetResponseTypeDef",
     "CreateDatastoreResponseTypeDef",
     "DeleteDatastoreResponseTypeDef",
     "DeleteImageSetResponseTypeDef",
     "GetImageFrameResponseTypeDef",
     "GetImageSetMetadataResponseTypeDef",
     "GetImageSetResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "StartDICOMImportJobResponseTypeDef",
     "UpdateImageSetMetadataResponseTypeDef",
     "GetDICOMImportJobResponseTypeDef",
     "ListDICOMImportJobsResponseTypeDef",
-    "SearchByAttributeValueTypeDef",
     "ImageSetsMetadataSummaryTypeDef",
-    "MetadataUpdatesTypeDef",
     "GetDatastoreResponseTypeDef",
     "ListDatastoresResponseTypeDef",
     "GetImageFrameRequestRequestTypeDef",
     "ListImageSetVersionsResponseTypeDef",
     "ListDICOMImportJobsRequestListDICOMImportJobsPaginateTypeDef",
     "ListDatastoresRequestListDatastoresPaginateTypeDef",
     "ListImageSetVersionsRequestListImageSetVersionsPaginateTypeDef",
+    "SearchByAttributeValueTypeDef",
+    "MetadataUpdatesTypeDef",
     "CopyImageSetRequestRequestTypeDef",
-    "SearchFilterTypeDef",
     "SearchImageSetsResponseTypeDef",
+    "SearchFilterTypeDef",
     "UpdateImageSetMetadataRequestRequestTypeDef",
     "SearchCriteriaTypeDef",
     "SearchImageSetsRequestRequestTypeDef",
     "SearchImageSetsRequestSearchImageSetsPaginateTypeDef",
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 _RequiredCopyDestinationImageSetPropertiesTypeDef = TypedDict(
     "_RequiredCopyDestinationImageSetPropertiesTypeDef",
     {
         "imageSetId": str,
         "latestVersionId": str,
     },
 )
@@ -287,23 +290,14 @@
         "DICOMAccessionNumber": str,
         "DICOMStudyDate": str,
         "DICOMStudyTime": str,
     },
     total=False,
 )
 
-DICOMUpdatesTypeDef = TypedDict(
-    "DICOMUpdatesTypeDef",
-    {
-        "removableAttributes": Union[str, bytes, IO[Any], StreamingBody],
-        "updatableAttributes": Union[str, bytes, IO[Any], StreamingBody],
-    },
-    total=False,
-)
-
 _RequiredDatastorePropertiesTypeDef = TypedDict(
     "_RequiredDatastorePropertiesTypeDef",
     {
         "datastoreId": str,
         "datastoreName": str,
         "datastoreStatus": DatastoreStatusType,
     },
@@ -529,14 +523,15 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
+TimestampTypeDef = Union[datetime, str]
 _RequiredStartDICOMImportJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartDICOMImportJobRequestRequestTypeDef",
     {
         "dataAccessRoleArn": str,
         "clientToken": str,
         "datastoreId": str,
         "inputS3Uri": str,
@@ -571,14 +566,23 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
+DICOMUpdatesTypeDef = TypedDict(
+    "DICOMUpdatesTypeDef",
+    {
+        "removableAttributes": BlobTypeDef,
+        "updatableAttributes": BlobTypeDef,
+    },
+    total=False,
+)
+
 _RequiredCopyImageSetInformationTypeDef = TypedDict(
     "_RequiredCopyImageSetInformationTypeDef",
     {
         "sourceImageSet": CopySourceImageSetInformationTypeDef,
     },
 )
 _OptionalCopyImageSetInformationTypeDef = TypedDict(
@@ -718,27 +722,14 @@
     {
         "jobSummaries": List[DICOMImportJobSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-SearchByAttributeValueTypeDef = TypedDict(
-    "SearchByAttributeValueTypeDef",
-    {
-        "DICOMPatientId": str,
-        "DICOMAccessionNumber": str,
-        "DICOMStudyId": str,
-        "DICOMStudyInstanceUID": str,
-        "createdAt": Union[datetime, str],
-        "DICOMStudyDateAndTime": DICOMStudyDateAndTimeTypeDef,
-    },
-    total=False,
-)
-
 _RequiredImageSetsMetadataSummaryTypeDef = TypedDict(
     "_RequiredImageSetsMetadataSummaryTypeDef",
     {
         "imageSetId": str,
     },
 )
 _OptionalImageSetsMetadataSummaryTypeDef = TypedDict(
@@ -755,22 +746,14 @@
 
 class ImageSetsMetadataSummaryTypeDef(
     _RequiredImageSetsMetadataSummaryTypeDef, _OptionalImageSetsMetadataSummaryTypeDef
 ):
     pass
 
 
-MetadataUpdatesTypeDef = TypedDict(
-    "MetadataUpdatesTypeDef",
-    {
-        "DICOMUpdates": DICOMUpdatesTypeDef,
-    },
-    total=False,
-)
-
 GetDatastoreResponseTypeDef = TypedDict(
     "GetDatastoreResponseTypeDef",
     {
         "datastoreProperties": DatastorePropertiesTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -853,40 +836,61 @@
 class ListImageSetVersionsRequestListImageSetVersionsPaginateTypeDef(
     _RequiredListImageSetVersionsRequestListImageSetVersionsPaginateTypeDef,
     _OptionalListImageSetVersionsRequestListImageSetVersionsPaginateTypeDef,
 ):
     pass
 
 
+SearchByAttributeValueTypeDef = TypedDict(
+    "SearchByAttributeValueTypeDef",
+    {
+        "DICOMPatientId": str,
+        "DICOMAccessionNumber": str,
+        "DICOMStudyId": str,
+        "DICOMStudyInstanceUID": str,
+        "createdAt": TimestampTypeDef,
+        "DICOMStudyDateAndTime": DICOMStudyDateAndTimeTypeDef,
+    },
+    total=False,
+)
+
+MetadataUpdatesTypeDef = TypedDict(
+    "MetadataUpdatesTypeDef",
+    {
+        "DICOMUpdates": DICOMUpdatesTypeDef,
+    },
+    total=False,
+)
+
 CopyImageSetRequestRequestTypeDef = TypedDict(
     "CopyImageSetRequestRequestTypeDef",
     {
         "datastoreId": str,
         "sourceImageSetId": str,
         "copyImageSetInformation": CopyImageSetInformationTypeDef,
     },
 )
 
-SearchFilterTypeDef = TypedDict(
-    "SearchFilterTypeDef",
-    {
-        "values": Sequence[SearchByAttributeValueTypeDef],
-        "operator": OperatorType,
-    },
-)
-
 SearchImageSetsResponseTypeDef = TypedDict(
     "SearchImageSetsResponseTypeDef",
     {
         "imageSetsMetadataSummaries": List[ImageSetsMetadataSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+SearchFilterTypeDef = TypedDict(
+    "SearchFilterTypeDef",
+    {
+        "values": Sequence[SearchByAttributeValueTypeDef],
+        "operator": OperatorType,
+    },
+)
+
 UpdateImageSetMetadataRequestRequestTypeDef = TypedDict(
     "UpdateImageSetMetadataRequestRequestTypeDef",
     {
         "datastoreId": str,
         "imageSetId": str,
         "latestVersionId": str,
         "updateImageSetMetadataUpdates": MetadataUpdatesTypeDef,
```

### Comparing `mypy-boto3-medical-imaging-1.28.15.post1/mypy_boto3_medical_imaging/type_defs.pyi` & `mypy-boto3-medical-imaging-1.28.16/mypy_boto3_medical_imaging/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for medical-imaging service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medical_imaging/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_medical_imaging.type_defs import CopyDestinationImageSetPropertiesTypeDef
+    from mypy_boto3_medical_imaging.type_defs import BlobTypeDef
 
-    data: CopyDestinationImageSetPropertiesTypeDef = {...}
+    data: BlobTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -27,25 +27,25 @@
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
+    "BlobTypeDef",
     "CopyDestinationImageSetPropertiesTypeDef",
     "CopyDestinationImageSetTypeDef",
     "CopySourceImageSetInformationTypeDef",
     "CopySourceImageSetPropertiesTypeDef",
     "ResponseMetadataTypeDef",
     "CreateDatastoreRequestRequestTypeDef",
     "DICOMImportJobPropertiesTypeDef",
     "DICOMImportJobSummaryTypeDef",
     "DICOMStudyDateAndTimeTypeDef",
     "DICOMTagsTypeDef",
-    "DICOMUpdatesTypeDef",
     "DatastorePropertiesTypeDef",
     "DatastoreSummaryTypeDef",
     "DeleteDatastoreRequestRequestTypeDef",
     "DeleteImageSetRequestRequestTypeDef",
     "GetDICOMImportJobRequestRequestTypeDef",
     "GetDatastoreRequestRequestTypeDef",
     "ImageFrameInformationTypeDef",
@@ -53,49 +53,52 @@
     "GetImageSetRequestRequestTypeDef",
     "ImageSetPropertiesTypeDef",
     "PaginatorConfigTypeDef",
     "ListDICOMImportJobsRequestRequestTypeDef",
     "ListDatastoresRequestRequestTypeDef",
     "ListImageSetVersionsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "TimestampTypeDef",
     "StartDICOMImportJobRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "DICOMUpdatesTypeDef",
     "CopyImageSetInformationTypeDef",
     "CopyImageSetResponseTypeDef",
     "CreateDatastoreResponseTypeDef",
     "DeleteDatastoreResponseTypeDef",
     "DeleteImageSetResponseTypeDef",
     "GetImageFrameResponseTypeDef",
     "GetImageSetMetadataResponseTypeDef",
     "GetImageSetResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "StartDICOMImportJobResponseTypeDef",
     "UpdateImageSetMetadataResponseTypeDef",
     "GetDICOMImportJobResponseTypeDef",
     "ListDICOMImportJobsResponseTypeDef",
-    "SearchByAttributeValueTypeDef",
     "ImageSetsMetadataSummaryTypeDef",
-    "MetadataUpdatesTypeDef",
     "GetDatastoreResponseTypeDef",
     "ListDatastoresResponseTypeDef",
     "GetImageFrameRequestRequestTypeDef",
     "ListImageSetVersionsResponseTypeDef",
     "ListDICOMImportJobsRequestListDICOMImportJobsPaginateTypeDef",
     "ListDatastoresRequestListDatastoresPaginateTypeDef",
     "ListImageSetVersionsRequestListImageSetVersionsPaginateTypeDef",
+    "SearchByAttributeValueTypeDef",
+    "MetadataUpdatesTypeDef",
     "CopyImageSetRequestRequestTypeDef",
-    "SearchFilterTypeDef",
     "SearchImageSetsResponseTypeDef",
+    "SearchFilterTypeDef",
     "UpdateImageSetMetadataRequestRequestTypeDef",
     "SearchCriteriaTypeDef",
     "SearchImageSetsRequestRequestTypeDef",
     "SearchImageSetsRequestSearchImageSetsPaginateTypeDef",
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 _RequiredCopyDestinationImageSetPropertiesTypeDef = TypedDict(
     "_RequiredCopyDestinationImageSetPropertiesTypeDef",
     {
         "imageSetId": str,
         "latestVersionId": str,
     },
 )
@@ -274,23 +277,14 @@
         "DICOMAccessionNumber": str,
         "DICOMStudyDate": str,
         "DICOMStudyTime": str,
     },
     total=False,
 )
 
-DICOMUpdatesTypeDef = TypedDict(
-    "DICOMUpdatesTypeDef",
-    {
-        "removableAttributes": Union[str, bytes, IO[Any], StreamingBody],
-        "updatableAttributes": Union[str, bytes, IO[Any], StreamingBody],
-    },
-    total=False,
-)
-
 _RequiredDatastorePropertiesTypeDef = TypedDict(
     "_RequiredDatastorePropertiesTypeDef",
     {
         "datastoreId": str,
         "datastoreName": str,
         "datastoreStatus": DatastoreStatusType,
     },
@@ -502,14 +496,15 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
+TimestampTypeDef = Union[datetime, str]
 _RequiredStartDICOMImportJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartDICOMImportJobRequestRequestTypeDef",
     {
         "dataAccessRoleArn": str,
         "clientToken": str,
         "datastoreId": str,
         "inputS3Uri": str,
@@ -542,14 +537,23 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
+DICOMUpdatesTypeDef = TypedDict(
+    "DICOMUpdatesTypeDef",
+    {
+        "removableAttributes": BlobTypeDef,
+        "updatableAttributes": BlobTypeDef,
+    },
+    total=False,
+)
+
 _RequiredCopyImageSetInformationTypeDef = TypedDict(
     "_RequiredCopyImageSetInformationTypeDef",
     {
         "sourceImageSet": CopySourceImageSetInformationTypeDef,
     },
 )
 _OptionalCopyImageSetInformationTypeDef = TypedDict(
@@ -687,27 +691,14 @@
     {
         "jobSummaries": List[DICOMImportJobSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-SearchByAttributeValueTypeDef = TypedDict(
-    "SearchByAttributeValueTypeDef",
-    {
-        "DICOMPatientId": str,
-        "DICOMAccessionNumber": str,
-        "DICOMStudyId": str,
-        "DICOMStudyInstanceUID": str,
-        "createdAt": Union[datetime, str],
-        "DICOMStudyDateAndTime": DICOMStudyDateAndTimeTypeDef,
-    },
-    total=False,
-)
-
 _RequiredImageSetsMetadataSummaryTypeDef = TypedDict(
     "_RequiredImageSetsMetadataSummaryTypeDef",
     {
         "imageSetId": str,
     },
 )
 _OptionalImageSetsMetadataSummaryTypeDef = TypedDict(
@@ -722,22 +713,14 @@
 )
 
 class ImageSetsMetadataSummaryTypeDef(
     _RequiredImageSetsMetadataSummaryTypeDef, _OptionalImageSetsMetadataSummaryTypeDef
 ):
     pass
 
-MetadataUpdatesTypeDef = TypedDict(
-    "MetadataUpdatesTypeDef",
-    {
-        "DICOMUpdates": DICOMUpdatesTypeDef,
-    },
-    total=False,
-)
-
 GetDatastoreResponseTypeDef = TypedDict(
     "GetDatastoreResponseTypeDef",
     {
         "datastoreProperties": DatastorePropertiesTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -816,40 +799,61 @@
 
 class ListImageSetVersionsRequestListImageSetVersionsPaginateTypeDef(
     _RequiredListImageSetVersionsRequestListImageSetVersionsPaginateTypeDef,
     _OptionalListImageSetVersionsRequestListImageSetVersionsPaginateTypeDef,
 ):
     pass
 
+SearchByAttributeValueTypeDef = TypedDict(
+    "SearchByAttributeValueTypeDef",
+    {
+        "DICOMPatientId": str,
+        "DICOMAccessionNumber": str,
+        "DICOMStudyId": str,
+        "DICOMStudyInstanceUID": str,
+        "createdAt": TimestampTypeDef,
+        "DICOMStudyDateAndTime": DICOMStudyDateAndTimeTypeDef,
+    },
+    total=False,
+)
+
+MetadataUpdatesTypeDef = TypedDict(
+    "MetadataUpdatesTypeDef",
+    {
+        "DICOMUpdates": DICOMUpdatesTypeDef,
+    },
+    total=False,
+)
+
 CopyImageSetRequestRequestTypeDef = TypedDict(
     "CopyImageSetRequestRequestTypeDef",
     {
         "datastoreId": str,
         "sourceImageSetId": str,
         "copyImageSetInformation": CopyImageSetInformationTypeDef,
     },
 )
 
-SearchFilterTypeDef = TypedDict(
-    "SearchFilterTypeDef",
-    {
-        "values": Sequence[SearchByAttributeValueTypeDef],
-        "operator": OperatorType,
-    },
-)
-
 SearchImageSetsResponseTypeDef = TypedDict(
     "SearchImageSetsResponseTypeDef",
     {
         "imageSetsMetadataSummaries": List[ImageSetsMetadataSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+SearchFilterTypeDef = TypedDict(
+    "SearchFilterTypeDef",
+    {
+        "values": Sequence[SearchByAttributeValueTypeDef],
+        "operator": OperatorType,
+    },
+)
+
 UpdateImageSetMetadataRequestRequestTypeDef = TypedDict(
     "UpdateImageSetMetadataRequestRequestTypeDef",
     {
         "datastoreId": str,
         "imageSetId": str,
         "latestVersionId": str,
         "updateImageSetMetadataUpdates": MetadataUpdatesTypeDef,
```

### Comparing `mypy-boto3-medical-imaging-1.28.15.post1/mypy_boto3_medical_imaging.egg-info/PKG-INFO` & `mypy-boto3-medical-imaging-1.28.16/mypy_boto3_medical_imaging.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-medical-imaging
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.HealthImaging 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.HealthImaging 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medical_imaging/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 medical-imaging type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 medical-imaging type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-medical-imaging.svg?color=blue)](https://pypi.org/project/mypy-boto3-medical-imaging)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medical_imaging/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-medical-imaging)](https://pepy.tech/project/mypy-boto3-medical-imaging)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.HealthImaging 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging)
+[boto3.HealthImaging 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging)
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
 [mypy-boto3-medical-imaging docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medical_imaging/).
 
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
@@ -330,34 +330,34 @@
 )
 
 
 def check_value(value: DatastoreStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_medical_imaging.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_medical_imaging.type_defs import (
+    BlobTypeDef,
     CopyDestinationImageSetPropertiesTypeDef,
     CopyDestinationImageSetTypeDef,
     CopySourceImageSetInformationTypeDef,
     CopySourceImageSetPropertiesTypeDef,
     ResponseMetadataTypeDef,
     CreateDatastoreRequestRequestTypeDef,
     DICOMImportJobPropertiesTypeDef,
     DICOMImportJobSummaryTypeDef,
     DICOMStudyDateAndTimeTypeDef,
     DICOMTagsTypeDef,
-    DICOMUpdatesTypeDef,
     DatastorePropertiesTypeDef,
     DatastoreSummaryTypeDef,
     DeleteDatastoreRequestRequestTypeDef,
     DeleteImageSetRequestRequestTypeDef,
     GetDICOMImportJobRequestRequestTypeDef,
     GetDatastoreRequestRequestTypeDef,
     ImageFrameInformationTypeDef,
@@ -365,51 +365,53 @@
     GetImageSetRequestRequestTypeDef,
     ImageSetPropertiesTypeDef,
     PaginatorConfigTypeDef,
     ListDICOMImportJobsRequestRequestTypeDef,
     ListDatastoresRequestRequestTypeDef,
     ListImageSetVersionsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TimestampTypeDef,
     StartDICOMImportJobRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    DICOMUpdatesTypeDef,
     CopyImageSetInformationTypeDef,
     CopyImageSetResponseTypeDef,
     CreateDatastoreResponseTypeDef,
     DeleteDatastoreResponseTypeDef,
     DeleteImageSetResponseTypeDef,
     GetImageFrameResponseTypeDef,
     GetImageSetMetadataResponseTypeDef,
     GetImageSetResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     StartDICOMImportJobResponseTypeDef,
     UpdateImageSetMetadataResponseTypeDef,
     GetDICOMImportJobResponseTypeDef,
     ListDICOMImportJobsResponseTypeDef,
-    SearchByAttributeValueTypeDef,
     ImageSetsMetadataSummaryTypeDef,
-    MetadataUpdatesTypeDef,
     GetDatastoreResponseTypeDef,
     ListDatastoresResponseTypeDef,
     GetImageFrameRequestRequestTypeDef,
     ListImageSetVersionsResponseTypeDef,
     ListDICOMImportJobsRequestListDICOMImportJobsPaginateTypeDef,
     ListDatastoresRequestListDatastoresPaginateTypeDef,
     ListImageSetVersionsRequestListImageSetVersionsPaginateTypeDef,
+    SearchByAttributeValueTypeDef,
+    MetadataUpdatesTypeDef,
     CopyImageSetRequestRequestTypeDef,
-    SearchFilterTypeDef,
     SearchImageSetsResponseTypeDef,
+    SearchFilterTypeDef,
     UpdateImageSetMetadataRequestRequestTypeDef,
     SearchCriteriaTypeDef,
     SearchImageSetsRequestRequestTypeDef,
     SearchImageSetsRequestSearchImageSetsPaginateTypeDef,
 )
 
 
-def get_structure() -> CopyDestinationImageSetPropertiesTypeDef:
+def get_value() -> BlobTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-medical-imaging-1.28.15.post1/mypy_boto3_medical_imaging.egg-info/SOURCES.txt` & `mypy-boto3-medical-imaging-1.28.16/mypy_boto3_medical_imaging.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-medical-imaging-1.28.15.post1/setup.py` & `mypy-boto3-medical-imaging-1.28.16/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-medical-imaging",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_medical_imaging"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.HealthImaging 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.2"
+        "Type annotations for boto3.HealthImaging 1.28.16 service generated with mypy-boto3-builder"
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
-    keywords="boto3 medical-imaging type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 medical-imaging type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_medical_imaging": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medical_imaging/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

