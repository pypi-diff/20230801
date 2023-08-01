# Comparing `tmp/mypy-boto3-comprehendmedical-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-comprehendmedical-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-comprehendmedical-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:50 2023, max compression
+gzip compressed data, was "mypy-boto3-comprehendmedical-1.28.16.tar", last modified: Tue Aug  1 11:36:31 2023, max compression
```

## Comparing `mypy-boto3-comprehendmedical-1.28.15.post1.tar` & `mypy-boto3-comprehendmedical-1.28.16.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:50.825085 mypy-boto3-comprehendmedical-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:41:14.000000 mypy-boto3-comprehendmedical-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15837 2023-07-29 10:02:50.813085 mypy-boto3-comprehendmedical-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14304 2023-07-29 09:41:14.000000 mypy-boto3-comprehendmedical-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:50.813085 mypy-boto3-comprehendmedical-1.28.15.post1/mypy_boto3_comprehendmedical/
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-29 09:41:14.000000 mypy-boto3-comprehendmedical-1.28.15.post1/mypy_boto3_comprehendmedical/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-29 09:41:14.000000 mypy-boto3-comprehendmedical-1.28.15.post1/mypy_boto3_comprehendmedical/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-29 09:41:14.000000 mypy-boto3-comprehendmedical-1.28.15.post1/mypy_boto3_comprehendmedical/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21575 2023-07-29 09:41:15.000000 mypy-boto3-comprehendmedical-1.28.15.post1/mypy_boto3_comprehendmedical/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    21542 2023-07-29 09:41:15.000000 mypy-boto3-comprehendmedical-1.28.15.post1/mypy_boto3_comprehendmedical/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11715 2023-07-29 09:41:15.000000 mypy-boto3-comprehendmedical-1.28.15.post1/mypy_boto3_comprehendmedical/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11713 2023-07-29 09:41:15.000000 mypy-boto3-comprehendmedical-1.28.15.post1/mypy_boto3_comprehendmedical/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:41:14.000000 mypy-boto3-comprehendmedical-1.28.15.post1/mypy_boto3_comprehendmedical/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    24890 2023-07-29 09:41:16.000000 mypy-boto3-comprehendmedical-1.28.15.post1/mypy_boto3_comprehendmedical/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    24875 2023-07-29 09:41:15.000000 mypy-boto3-comprehendmedical-1.28.15.post1/mypy_boto3_comprehendmedical/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:41:14.000000 mypy-boto3-comprehendmedical-1.28.15.post1/mypy_boto3_comprehendmedical/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:50.813085 mypy-boto3-comprehendmedical-1.28.15.post1/mypy_boto3_comprehendmedical.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15837 2023-07-29 10:02:50.000000 mypy-boto3-comprehendmedical-1.28.15.post1/mypy_boto3_comprehendmedical.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-29 10:02:50.000000 mypy-boto3-comprehendmedical-1.28.15.post1/mypy_boto3_comprehendmedical.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:50.000000 mypy-boto3-comprehendmedical-1.28.15.post1/mypy_boto3_comprehendmedical.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:50.000000 mypy-boto3-comprehendmedical-1.28.15.post1/mypy_boto3_comprehendmedical.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:50.000000 mypy-boto3-comprehendmedical-1.28.15.post1/mypy_boto3_comprehendmedical.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-29 10:02:50.000000 mypy-boto3-comprehendmedical-1.28.15.post1/mypy_boto3_comprehendmedical.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:50.825085 mypy-boto3-comprehendmedical-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-07-29 09:41:14.000000 mypy-boto3-comprehendmedical-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:31.956919 mypy-boto3-comprehendmedical-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:13:46.000000 mypy-boto3-comprehendmedical-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15849 2023-08-01 11:36:31.948918 mypy-boto3-comprehendmedical-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14325 2023-08-01 11:13:46.000000 mypy-boto3-comprehendmedical-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:31.940919 mypy-boto3-comprehendmedical-1.28.16/mypy_boto3_comprehendmedical/
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-08-01 11:13:46.000000 mypy-boto3-comprehendmedical-1.28.16/mypy_boto3_comprehendmedical/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-08-01 11:13:46.000000 mypy-boto3-comprehendmedical-1.28.16/mypy_boto3_comprehendmedical/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-08-01 11:13:46.000000 mypy-boto3-comprehendmedical-1.28.16/mypy_boto3_comprehendmedical/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21575 2023-08-01 11:13:47.000000 mypy-boto3-comprehendmedical-1.28.16/mypy_boto3_comprehendmedical/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21542 2023-08-01 11:13:46.000000 mypy-boto3-comprehendmedical-1.28.16/mypy_boto3_comprehendmedical/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11715 2023-08-01 11:13:47.000000 mypy-boto3-comprehendmedical-1.28.16/mypy_boto3_comprehendmedical/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11713 2023-08-01 11:13:47.000000 mypy-boto3-comprehendmedical-1.28.16/mypy_boto3_comprehendmedical/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:13:46.000000 mypy-boto3-comprehendmedical-1.28.16/mypy_boto3_comprehendmedical/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    24944 2023-08-01 11:13:48.000000 mypy-boto3-comprehendmedical-1.28.16/mypy_boto3_comprehendmedical/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24929 2023-08-01 11:13:47.000000 mypy-boto3-comprehendmedical-1.28.16/mypy_boto3_comprehendmedical/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:13:46.000000 mypy-boto3-comprehendmedical-1.28.16/mypy_boto3_comprehendmedical/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:31.948918 mypy-boto3-comprehendmedical-1.28.16/mypy_boto3_comprehendmedical.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15849 2023-08-01 11:36:31.000000 mypy-boto3-comprehendmedical-1.28.16/mypy_boto3_comprehendmedical.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-08-01 11:36:31.000000 mypy-boto3-comprehendmedical-1.28.16/mypy_boto3_comprehendmedical.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:31.000000 mypy-boto3-comprehendmedical-1.28.16/mypy_boto3_comprehendmedical.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:31.000000 mypy-boto3-comprehendmedical-1.28.16/mypy_boto3_comprehendmedical.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:31.000000 mypy-boto3-comprehendmedical-1.28.16/mypy_boto3_comprehendmedical.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-01 11:36:31.000000 mypy-boto3-comprehendmedical-1.28.16/mypy_boto3_comprehendmedical.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:31.956919 mypy-boto3-comprehendmedical-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-08-01 11:13:46.000000 mypy-boto3-comprehendmedical-1.28.16/setup.py
```

### Comparing `mypy-boto3-comprehendmedical-1.28.15.post1/LICENSE` & `mypy-boto3-comprehendmedical-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-comprehendmedical-1.28.15.post1/PKG-INFO` & `mypy-boto3-comprehendmedical-1.28.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-comprehendmedical
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.ComprehendMedical 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.ComprehendMedical 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehendmedical/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 comprehendmedical type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 comprehendmedical type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-comprehendmedical.svg?color=blue)](https://pypi.org/project/mypy-boto3-comprehendmedical)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehendmedical/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-comprehendmedical)](https://pepy.tech/project/mypy-boto3-comprehendmedical)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ComprehendMedical 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehendmedical.html#ComprehendMedical)
+[boto3.ComprehendMedical 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehendmedical.html#ComprehendMedical)
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
 [mypy-boto3-comprehendmedical docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehendmedical/).
 
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
@@ -308,26 +308,26 @@
 )
 
 
 def check_value(value: AttributeNameType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_comprehendmedical.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_comprehendmedical.type_defs import (
     TraitTypeDef,
     CharactersTypeDef,
-    ComprehendMedicalAsyncJobFilterTypeDef,
+    TimestampTypeDef,
     InputDataConfigTypeDef,
     OutputDataConfigTypeDef,
     DescribeEntitiesDetectionV2JobRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     DescribeICD10CMInferenceJobRequestRequestTypeDef,
     DescribePHIDetectionJobRequestRequestTypeDef,
     DescribeRxNormInferenceJobRequestRequestTypeDef,
@@ -347,19 +347,15 @@
     SNOMEDCTTraitTypeDef,
     StopEntitiesDetectionV2JobRequestRequestTypeDef,
     StopICD10CMInferenceJobRequestRequestTypeDef,
     StopPHIDetectionJobRequestRequestTypeDef,
     StopRxNormInferenceJobRequestRequestTypeDef,
     StopSNOMEDCTInferenceJobRequestRequestTypeDef,
     AttributeTypeDef,
-    ListEntitiesDetectionV2JobsRequestRequestTypeDef,
-    ListICD10CMInferenceJobsRequestRequestTypeDef,
-    ListPHIDetectionJobsRequestRequestTypeDef,
-    ListRxNormInferenceJobsRequestRequestTypeDef,
-    ListSNOMEDCTInferenceJobsRequestRequestTypeDef,
+    ComprehendMedicalAsyncJobFilterTypeDef,
     ComprehendMedicalAsyncJobPropertiesTypeDef,
     StartEntitiesDetectionV2JobRequestRequestTypeDef,
     StartICD10CMInferenceJobRequestRequestTypeDef,
     StartPHIDetectionJobRequestRequestTypeDef,
     StartRxNormInferenceJobRequestRequestTypeDef,
     StartSNOMEDCTInferenceJobRequestRequestTypeDef,
     StartEntitiesDetectionV2JobResponseTypeDef,
@@ -373,14 +369,19 @@
     StopRxNormInferenceJobResponseTypeDef,
     StopSNOMEDCTInferenceJobResponseTypeDef,
     ICD10CMAttributeTypeDef,
     RxNormAttributeTypeDef,
     SNOMEDCTAttributeTypeDef,
     EntityTypeDef,
     UnmappedAttributeTypeDef,
+    ListEntitiesDetectionV2JobsRequestRequestTypeDef,
+    ListICD10CMInferenceJobsRequestRequestTypeDef,
+    ListPHIDetectionJobsRequestRequestTypeDef,
+    ListRxNormInferenceJobsRequestRequestTypeDef,
+    ListSNOMEDCTInferenceJobsRequestRequestTypeDef,
     DescribeEntitiesDetectionV2JobResponseTypeDef,
     DescribeICD10CMInferenceJobResponseTypeDef,
     DescribePHIDetectionJobResponseTypeDef,
     DescribeRxNormInferenceJobResponseTypeDef,
     DescribeSNOMEDCTInferenceJobResponseTypeDef,
     ListEntitiesDetectionV2JobsResponseTypeDef,
     ListICD10CMInferenceJobsResponseTypeDef,
@@ -395,15 +396,15 @@
     DetectEntitiesV2ResponseTypeDef,
     InferICD10CMResponseTypeDef,
     InferRxNormResponseTypeDef,
     InferSNOMEDCTResponseTypeDef,
 )
 
 
-def get_structure() -> TraitTypeDef:
+def get_value() -> TraitTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-comprehendmedical-1.28.15.post1/README.md` & `mypy-boto3-comprehendmedical-1.28.16/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-comprehendmedical.svg?color=blue)](https://pypi.org/project/mypy-boto3-comprehendmedical)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehendmedical/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-comprehendmedical)](https://pepy.tech/project/mypy-boto3-comprehendmedical)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ComprehendMedical 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehendmedical.html#ComprehendMedical)
+[boto3.ComprehendMedical 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehendmedical.html#ComprehendMedical)
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
 [mypy-boto3-comprehendmedical docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehendmedical/).
 
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
@@ -276,26 +276,26 @@
 )
 
 
 def check_value(value: AttributeNameType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_comprehendmedical.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_comprehendmedical.type_defs import (
     TraitTypeDef,
     CharactersTypeDef,
-    ComprehendMedicalAsyncJobFilterTypeDef,
+    TimestampTypeDef,
     InputDataConfigTypeDef,
     OutputDataConfigTypeDef,
     DescribeEntitiesDetectionV2JobRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     DescribeICD10CMInferenceJobRequestRequestTypeDef,
     DescribePHIDetectionJobRequestRequestTypeDef,
     DescribeRxNormInferenceJobRequestRequestTypeDef,
@@ -315,19 +315,15 @@
     SNOMEDCTTraitTypeDef,
     StopEntitiesDetectionV2JobRequestRequestTypeDef,
     StopICD10CMInferenceJobRequestRequestTypeDef,
     StopPHIDetectionJobRequestRequestTypeDef,
     StopRxNormInferenceJobRequestRequestTypeDef,
     StopSNOMEDCTInferenceJobRequestRequestTypeDef,
     AttributeTypeDef,
-    ListEntitiesDetectionV2JobsRequestRequestTypeDef,
-    ListICD10CMInferenceJobsRequestRequestTypeDef,
-    ListPHIDetectionJobsRequestRequestTypeDef,
-    ListRxNormInferenceJobsRequestRequestTypeDef,
-    ListSNOMEDCTInferenceJobsRequestRequestTypeDef,
+    ComprehendMedicalAsyncJobFilterTypeDef,
     ComprehendMedicalAsyncJobPropertiesTypeDef,
     StartEntitiesDetectionV2JobRequestRequestTypeDef,
     StartICD10CMInferenceJobRequestRequestTypeDef,
     StartPHIDetectionJobRequestRequestTypeDef,
     StartRxNormInferenceJobRequestRequestTypeDef,
     StartSNOMEDCTInferenceJobRequestRequestTypeDef,
     StartEntitiesDetectionV2JobResponseTypeDef,
@@ -341,14 +337,19 @@
     StopRxNormInferenceJobResponseTypeDef,
     StopSNOMEDCTInferenceJobResponseTypeDef,
     ICD10CMAttributeTypeDef,
     RxNormAttributeTypeDef,
     SNOMEDCTAttributeTypeDef,
     EntityTypeDef,
     UnmappedAttributeTypeDef,
+    ListEntitiesDetectionV2JobsRequestRequestTypeDef,
+    ListICD10CMInferenceJobsRequestRequestTypeDef,
+    ListPHIDetectionJobsRequestRequestTypeDef,
+    ListRxNormInferenceJobsRequestRequestTypeDef,
+    ListSNOMEDCTInferenceJobsRequestRequestTypeDef,
     DescribeEntitiesDetectionV2JobResponseTypeDef,
     DescribeICD10CMInferenceJobResponseTypeDef,
     DescribePHIDetectionJobResponseTypeDef,
     DescribeRxNormInferenceJobResponseTypeDef,
     DescribeSNOMEDCTInferenceJobResponseTypeDef,
     ListEntitiesDetectionV2JobsResponseTypeDef,
     ListICD10CMInferenceJobsResponseTypeDef,
@@ -363,15 +364,15 @@
     DetectEntitiesV2ResponseTypeDef,
     InferICD10CMResponseTypeDef,
     InferRxNormResponseTypeDef,
     InferSNOMEDCTResponseTypeDef,
 )
 
 
-def get_structure() -> TraitTypeDef:
+def get_value() -> TraitTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-comprehendmedical-1.28.15.post1/mypy_boto3_comprehendmedical/__main__.py` & `mypy-boto3-comprehendmedical-1.28.16/mypy_boto3_comprehendmedical/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ComprehendMedical 1.28.15\nVersion:        "
-        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.ComprehendMedical 1.28.16\nVersion:         1.28.16\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehendmedical//\nBoto3 docs:   "
         "   https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehendmedical.html#ComprehendMedical\nOther"
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

### Comparing `mypy-boto3-comprehendmedical-1.28.15.post1/mypy_boto3_comprehendmedical/client.py` & `mypy-boto3-comprehendmedical-1.28.16/mypy_boto3_comprehendmedical/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-comprehendmedical-1.28.15.post1/mypy_boto3_comprehendmedical/client.pyi` & `mypy-boto3-comprehendmedical-1.28.16/mypy_boto3_comprehendmedical/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-comprehendmedical-1.28.15.post1/mypy_boto3_comprehendmedical/literals.py` & `mypy-boto3-comprehendmedical-1.28.16/mypy_boto3_comprehendmedical/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-comprehendmedical-1.28.15.post1/mypy_boto3_comprehendmedical/literals.pyi` & `mypy-boto3-comprehendmedical-1.28.16/mypy_boto3_comprehendmedical/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-comprehendmedical-1.28.15.post1/mypy_boto3_comprehendmedical/type_defs.py` & `mypy-boto3-comprehendmedical-1.28.16/mypy_boto3_comprehendmedical/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehendmedical/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_comprehendmedical.type_defs import TraitTypeDef
 
-    data: TraitTypeDef = {...}
+    data: TraitTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Union
 
 from .literals import (
@@ -44,15 +44,15 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "TraitTypeDef",
     "CharactersTypeDef",
-    "ComprehendMedicalAsyncJobFilterTypeDef",
+    "TimestampTypeDef",
     "InputDataConfigTypeDef",
     "OutputDataConfigTypeDef",
     "DescribeEntitiesDetectionV2JobRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "DescribeICD10CMInferenceJobRequestRequestTypeDef",
     "DescribePHIDetectionJobRequestRequestTypeDef",
     "DescribeRxNormInferenceJobRequestRequestTypeDef",
@@ -72,19 +72,15 @@
     "SNOMEDCTTraitTypeDef",
     "StopEntitiesDetectionV2JobRequestRequestTypeDef",
     "StopICD10CMInferenceJobRequestRequestTypeDef",
     "StopPHIDetectionJobRequestRequestTypeDef",
     "StopRxNormInferenceJobRequestRequestTypeDef",
     "StopSNOMEDCTInferenceJobRequestRequestTypeDef",
     "AttributeTypeDef",
-    "ListEntitiesDetectionV2JobsRequestRequestTypeDef",
-    "ListICD10CMInferenceJobsRequestRequestTypeDef",
-    "ListPHIDetectionJobsRequestRequestTypeDef",
-    "ListRxNormInferenceJobsRequestRequestTypeDef",
-    "ListSNOMEDCTInferenceJobsRequestRequestTypeDef",
+    "ComprehendMedicalAsyncJobFilterTypeDef",
     "ComprehendMedicalAsyncJobPropertiesTypeDef",
     "StartEntitiesDetectionV2JobRequestRequestTypeDef",
     "StartICD10CMInferenceJobRequestRequestTypeDef",
     "StartPHIDetectionJobRequestRequestTypeDef",
     "StartRxNormInferenceJobRequestRequestTypeDef",
     "StartSNOMEDCTInferenceJobRequestRequestTypeDef",
     "StartEntitiesDetectionV2JobResponseTypeDef",
@@ -98,14 +94,19 @@
     "StopRxNormInferenceJobResponseTypeDef",
     "StopSNOMEDCTInferenceJobResponseTypeDef",
     "ICD10CMAttributeTypeDef",
     "RxNormAttributeTypeDef",
     "SNOMEDCTAttributeTypeDef",
     "EntityTypeDef",
     "UnmappedAttributeTypeDef",
+    "ListEntitiesDetectionV2JobsRequestRequestTypeDef",
+    "ListICD10CMInferenceJobsRequestRequestTypeDef",
+    "ListPHIDetectionJobsRequestRequestTypeDef",
+    "ListRxNormInferenceJobsRequestRequestTypeDef",
+    "ListSNOMEDCTInferenceJobsRequestRequestTypeDef",
     "DescribeEntitiesDetectionV2JobResponseTypeDef",
     "DescribeICD10CMInferenceJobResponseTypeDef",
     "DescribePHIDetectionJobResponseTypeDef",
     "DescribeRxNormInferenceJobResponseTypeDef",
     "DescribeSNOMEDCTInferenceJobResponseTypeDef",
     "ListEntitiesDetectionV2JobsResponseTypeDef",
     "ListICD10CMInferenceJobsResponseTypeDef",
@@ -136,25 +137,15 @@
     "CharactersTypeDef",
     {
         "OriginalTextCharacters": int,
     },
     total=False,
 )
 
-ComprehendMedicalAsyncJobFilterTypeDef = TypedDict(
-    "ComprehendMedicalAsyncJobFilterTypeDef",
-    {
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "SubmitTimeBefore": Union[datetime, str],
-        "SubmitTimeAfter": Union[datetime, str],
-    },
-    total=False,
-)
-
+TimestampTypeDef = Union[datetime, str]
 _RequiredInputDataConfigTypeDef = TypedDict(
     "_RequiredInputDataConfigTypeDef",
     {
         "S3Bucket": str,
     },
 )
 _OptionalInputDataConfigTypeDef = TypedDict(
@@ -392,60 +383,21 @@
         "Text": str,
         "Category": EntityTypeType,
         "Traits": List[TraitTypeDef],
     },
     total=False,
 )
 
-ListEntitiesDetectionV2JobsRequestRequestTypeDef = TypedDict(
-    "ListEntitiesDetectionV2JobsRequestRequestTypeDef",
-    {
-        "Filter": ComprehendMedicalAsyncJobFilterTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
-ListICD10CMInferenceJobsRequestRequestTypeDef = TypedDict(
-    "ListICD10CMInferenceJobsRequestRequestTypeDef",
-    {
-        "Filter": ComprehendMedicalAsyncJobFilterTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
-ListPHIDetectionJobsRequestRequestTypeDef = TypedDict(
-    "ListPHIDetectionJobsRequestRequestTypeDef",
-    {
-        "Filter": ComprehendMedicalAsyncJobFilterTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
-ListRxNormInferenceJobsRequestRequestTypeDef = TypedDict(
-    "ListRxNormInferenceJobsRequestRequestTypeDef",
-    {
-        "Filter": ComprehendMedicalAsyncJobFilterTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
-ListSNOMEDCTInferenceJobsRequestRequestTypeDef = TypedDict(
-    "ListSNOMEDCTInferenceJobsRequestRequestTypeDef",
+ComprehendMedicalAsyncJobFilterTypeDef = TypedDict(
+    "ComprehendMedicalAsyncJobFilterTypeDef",
     {
-        "Filter": ComprehendMedicalAsyncJobFilterTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "SubmitTimeBefore": TimestampTypeDef,
+        "SubmitTimeAfter": TimestampTypeDef,
     },
     total=False,
 )
 
 ComprehendMedicalAsyncJobPropertiesTypeDef = TypedDict(
     "ComprehendMedicalAsyncJobPropertiesTypeDef",
     {
@@ -753,14 +705,64 @@
     {
         "Type": EntityTypeType,
         "Attribute": AttributeTypeDef,
     },
     total=False,
 )
 
+ListEntitiesDetectionV2JobsRequestRequestTypeDef = TypedDict(
+    "ListEntitiesDetectionV2JobsRequestRequestTypeDef",
+    {
+        "Filter": ComprehendMedicalAsyncJobFilterTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+ListICD10CMInferenceJobsRequestRequestTypeDef = TypedDict(
+    "ListICD10CMInferenceJobsRequestRequestTypeDef",
+    {
+        "Filter": ComprehendMedicalAsyncJobFilterTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+ListPHIDetectionJobsRequestRequestTypeDef = TypedDict(
+    "ListPHIDetectionJobsRequestRequestTypeDef",
+    {
+        "Filter": ComprehendMedicalAsyncJobFilterTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+ListRxNormInferenceJobsRequestRequestTypeDef = TypedDict(
+    "ListRxNormInferenceJobsRequestRequestTypeDef",
+    {
+        "Filter": ComprehendMedicalAsyncJobFilterTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+ListSNOMEDCTInferenceJobsRequestRequestTypeDef = TypedDict(
+    "ListSNOMEDCTInferenceJobsRequestRequestTypeDef",
+    {
+        "Filter": ComprehendMedicalAsyncJobFilterTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
 DescribeEntitiesDetectionV2JobResponseTypeDef = TypedDict(
     "DescribeEntitiesDetectionV2JobResponseTypeDef",
     {
         "ComprehendMedicalAsyncJobProperties": ComprehendMedicalAsyncJobPropertiesTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-comprehendmedical-1.28.15.post1/mypy_boto3_comprehendmedical/type_defs.pyi` & `mypy-boto3-comprehendmedical-1.28.16/mypy_boto3_comprehendmedical/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehendmedical/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_comprehendmedical.type_defs import TraitTypeDef
 
-    data: TraitTypeDef = {...}
+    data: TraitTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Union
 
 from .literals import (
@@ -43,15 +43,15 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "TraitTypeDef",
     "CharactersTypeDef",
-    "ComprehendMedicalAsyncJobFilterTypeDef",
+    "TimestampTypeDef",
     "InputDataConfigTypeDef",
     "OutputDataConfigTypeDef",
     "DescribeEntitiesDetectionV2JobRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "DescribeICD10CMInferenceJobRequestRequestTypeDef",
     "DescribePHIDetectionJobRequestRequestTypeDef",
     "DescribeRxNormInferenceJobRequestRequestTypeDef",
@@ -71,19 +71,15 @@
     "SNOMEDCTTraitTypeDef",
     "StopEntitiesDetectionV2JobRequestRequestTypeDef",
     "StopICD10CMInferenceJobRequestRequestTypeDef",
     "StopPHIDetectionJobRequestRequestTypeDef",
     "StopRxNormInferenceJobRequestRequestTypeDef",
     "StopSNOMEDCTInferenceJobRequestRequestTypeDef",
     "AttributeTypeDef",
-    "ListEntitiesDetectionV2JobsRequestRequestTypeDef",
-    "ListICD10CMInferenceJobsRequestRequestTypeDef",
-    "ListPHIDetectionJobsRequestRequestTypeDef",
-    "ListRxNormInferenceJobsRequestRequestTypeDef",
-    "ListSNOMEDCTInferenceJobsRequestRequestTypeDef",
+    "ComprehendMedicalAsyncJobFilterTypeDef",
     "ComprehendMedicalAsyncJobPropertiesTypeDef",
     "StartEntitiesDetectionV2JobRequestRequestTypeDef",
     "StartICD10CMInferenceJobRequestRequestTypeDef",
     "StartPHIDetectionJobRequestRequestTypeDef",
     "StartRxNormInferenceJobRequestRequestTypeDef",
     "StartSNOMEDCTInferenceJobRequestRequestTypeDef",
     "StartEntitiesDetectionV2JobResponseTypeDef",
@@ -97,14 +93,19 @@
     "StopRxNormInferenceJobResponseTypeDef",
     "StopSNOMEDCTInferenceJobResponseTypeDef",
     "ICD10CMAttributeTypeDef",
     "RxNormAttributeTypeDef",
     "SNOMEDCTAttributeTypeDef",
     "EntityTypeDef",
     "UnmappedAttributeTypeDef",
+    "ListEntitiesDetectionV2JobsRequestRequestTypeDef",
+    "ListICD10CMInferenceJobsRequestRequestTypeDef",
+    "ListPHIDetectionJobsRequestRequestTypeDef",
+    "ListRxNormInferenceJobsRequestRequestTypeDef",
+    "ListSNOMEDCTInferenceJobsRequestRequestTypeDef",
     "DescribeEntitiesDetectionV2JobResponseTypeDef",
     "DescribeICD10CMInferenceJobResponseTypeDef",
     "DescribePHIDetectionJobResponseTypeDef",
     "DescribeRxNormInferenceJobResponseTypeDef",
     "DescribeSNOMEDCTInferenceJobResponseTypeDef",
     "ListEntitiesDetectionV2JobsResponseTypeDef",
     "ListICD10CMInferenceJobsResponseTypeDef",
@@ -135,25 +136,15 @@
     "CharactersTypeDef",
     {
         "OriginalTextCharacters": int,
     },
     total=False,
 )
 
-ComprehendMedicalAsyncJobFilterTypeDef = TypedDict(
-    "ComprehendMedicalAsyncJobFilterTypeDef",
-    {
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "SubmitTimeBefore": Union[datetime, str],
-        "SubmitTimeAfter": Union[datetime, str],
-    },
-    total=False,
-)
-
+TimestampTypeDef = Union[datetime, str]
 _RequiredInputDataConfigTypeDef = TypedDict(
     "_RequiredInputDataConfigTypeDef",
     {
         "S3Bucket": str,
     },
 )
 _OptionalInputDataConfigTypeDef = TypedDict(
@@ -387,60 +378,21 @@
         "Text": str,
         "Category": EntityTypeType,
         "Traits": List[TraitTypeDef],
     },
     total=False,
 )
 
-ListEntitiesDetectionV2JobsRequestRequestTypeDef = TypedDict(
-    "ListEntitiesDetectionV2JobsRequestRequestTypeDef",
-    {
-        "Filter": ComprehendMedicalAsyncJobFilterTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
-ListICD10CMInferenceJobsRequestRequestTypeDef = TypedDict(
-    "ListICD10CMInferenceJobsRequestRequestTypeDef",
-    {
-        "Filter": ComprehendMedicalAsyncJobFilterTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
-ListPHIDetectionJobsRequestRequestTypeDef = TypedDict(
-    "ListPHIDetectionJobsRequestRequestTypeDef",
-    {
-        "Filter": ComprehendMedicalAsyncJobFilterTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
-ListRxNormInferenceJobsRequestRequestTypeDef = TypedDict(
-    "ListRxNormInferenceJobsRequestRequestTypeDef",
-    {
-        "Filter": ComprehendMedicalAsyncJobFilterTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
-ListSNOMEDCTInferenceJobsRequestRequestTypeDef = TypedDict(
-    "ListSNOMEDCTInferenceJobsRequestRequestTypeDef",
+ComprehendMedicalAsyncJobFilterTypeDef = TypedDict(
+    "ComprehendMedicalAsyncJobFilterTypeDef",
     {
-        "Filter": ComprehendMedicalAsyncJobFilterTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "SubmitTimeBefore": TimestampTypeDef,
+        "SubmitTimeAfter": TimestampTypeDef,
     },
     total=False,
 )
 
 ComprehendMedicalAsyncJobPropertiesTypeDef = TypedDict(
     "ComprehendMedicalAsyncJobPropertiesTypeDef",
     {
@@ -738,14 +690,64 @@
     {
         "Type": EntityTypeType,
         "Attribute": AttributeTypeDef,
     },
     total=False,
 )
 
+ListEntitiesDetectionV2JobsRequestRequestTypeDef = TypedDict(
+    "ListEntitiesDetectionV2JobsRequestRequestTypeDef",
+    {
+        "Filter": ComprehendMedicalAsyncJobFilterTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+ListICD10CMInferenceJobsRequestRequestTypeDef = TypedDict(
+    "ListICD10CMInferenceJobsRequestRequestTypeDef",
+    {
+        "Filter": ComprehendMedicalAsyncJobFilterTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+ListPHIDetectionJobsRequestRequestTypeDef = TypedDict(
+    "ListPHIDetectionJobsRequestRequestTypeDef",
+    {
+        "Filter": ComprehendMedicalAsyncJobFilterTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+ListRxNormInferenceJobsRequestRequestTypeDef = TypedDict(
+    "ListRxNormInferenceJobsRequestRequestTypeDef",
+    {
+        "Filter": ComprehendMedicalAsyncJobFilterTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+ListSNOMEDCTInferenceJobsRequestRequestTypeDef = TypedDict(
+    "ListSNOMEDCTInferenceJobsRequestRequestTypeDef",
+    {
+        "Filter": ComprehendMedicalAsyncJobFilterTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
 DescribeEntitiesDetectionV2JobResponseTypeDef = TypedDict(
     "DescribeEntitiesDetectionV2JobResponseTypeDef",
     {
         "ComprehendMedicalAsyncJobProperties": ComprehendMedicalAsyncJobPropertiesTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-comprehendmedical-1.28.15.post1/mypy_boto3_comprehendmedical.egg-info/PKG-INFO` & `mypy-boto3-comprehendmedical-1.28.16/mypy_boto3_comprehendmedical.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-comprehendmedical
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.ComprehendMedical 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.ComprehendMedical 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehendmedical/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 comprehendmedical type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 comprehendmedical type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-comprehendmedical.svg?color=blue)](https://pypi.org/project/mypy-boto3-comprehendmedical)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehendmedical/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-comprehendmedical)](https://pepy.tech/project/mypy-boto3-comprehendmedical)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ComprehendMedical 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehendmedical.html#ComprehendMedical)
+[boto3.ComprehendMedical 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehendmedical.html#ComprehendMedical)
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
 [mypy-boto3-comprehendmedical docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehendmedical/).
 
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
@@ -308,26 +308,26 @@
 )
 
 
 def check_value(value: AttributeNameType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_comprehendmedical.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_comprehendmedical.type_defs import (
     TraitTypeDef,
     CharactersTypeDef,
-    ComprehendMedicalAsyncJobFilterTypeDef,
+    TimestampTypeDef,
     InputDataConfigTypeDef,
     OutputDataConfigTypeDef,
     DescribeEntitiesDetectionV2JobRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     DescribeICD10CMInferenceJobRequestRequestTypeDef,
     DescribePHIDetectionJobRequestRequestTypeDef,
     DescribeRxNormInferenceJobRequestRequestTypeDef,
@@ -347,19 +347,15 @@
     SNOMEDCTTraitTypeDef,
     StopEntitiesDetectionV2JobRequestRequestTypeDef,
     StopICD10CMInferenceJobRequestRequestTypeDef,
     StopPHIDetectionJobRequestRequestTypeDef,
     StopRxNormInferenceJobRequestRequestTypeDef,
     StopSNOMEDCTInferenceJobRequestRequestTypeDef,
     AttributeTypeDef,
-    ListEntitiesDetectionV2JobsRequestRequestTypeDef,
-    ListICD10CMInferenceJobsRequestRequestTypeDef,
-    ListPHIDetectionJobsRequestRequestTypeDef,
-    ListRxNormInferenceJobsRequestRequestTypeDef,
-    ListSNOMEDCTInferenceJobsRequestRequestTypeDef,
+    ComprehendMedicalAsyncJobFilterTypeDef,
     ComprehendMedicalAsyncJobPropertiesTypeDef,
     StartEntitiesDetectionV2JobRequestRequestTypeDef,
     StartICD10CMInferenceJobRequestRequestTypeDef,
     StartPHIDetectionJobRequestRequestTypeDef,
     StartRxNormInferenceJobRequestRequestTypeDef,
     StartSNOMEDCTInferenceJobRequestRequestTypeDef,
     StartEntitiesDetectionV2JobResponseTypeDef,
@@ -373,14 +369,19 @@
     StopRxNormInferenceJobResponseTypeDef,
     StopSNOMEDCTInferenceJobResponseTypeDef,
     ICD10CMAttributeTypeDef,
     RxNormAttributeTypeDef,
     SNOMEDCTAttributeTypeDef,
     EntityTypeDef,
     UnmappedAttributeTypeDef,
+    ListEntitiesDetectionV2JobsRequestRequestTypeDef,
+    ListICD10CMInferenceJobsRequestRequestTypeDef,
+    ListPHIDetectionJobsRequestRequestTypeDef,
+    ListRxNormInferenceJobsRequestRequestTypeDef,
+    ListSNOMEDCTInferenceJobsRequestRequestTypeDef,
     DescribeEntitiesDetectionV2JobResponseTypeDef,
     DescribeICD10CMInferenceJobResponseTypeDef,
     DescribePHIDetectionJobResponseTypeDef,
     DescribeRxNormInferenceJobResponseTypeDef,
     DescribeSNOMEDCTInferenceJobResponseTypeDef,
     ListEntitiesDetectionV2JobsResponseTypeDef,
     ListICD10CMInferenceJobsResponseTypeDef,
@@ -395,15 +396,15 @@
     DetectEntitiesV2ResponseTypeDef,
     InferICD10CMResponseTypeDef,
     InferRxNormResponseTypeDef,
     InferSNOMEDCTResponseTypeDef,
 )
 
 
-def get_structure() -> TraitTypeDef:
+def get_value() -> TraitTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-comprehendmedical-1.28.15.post1/mypy_boto3_comprehendmedical.egg-info/SOURCES.txt` & `mypy-boto3-comprehendmedical-1.28.16/mypy_boto3_comprehendmedical.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-comprehendmedical-1.28.15.post1/setup.py` & `mypy-boto3-comprehendmedical-1.28.16/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-comprehendmedical",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_comprehendmedical"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ComprehendMedical 1.28.15 service generated with"
-        " mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.ComprehendMedical 1.28.16 service generated with"
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
-    keywords="boto3 comprehendmedical type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 comprehendmedical type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_comprehendmedical": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehendmedical/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

