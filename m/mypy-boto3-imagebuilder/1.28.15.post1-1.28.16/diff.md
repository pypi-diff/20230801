# Comparing `tmp/mypy-boto3-imagebuilder-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-imagebuilder-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-imagebuilder-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:16 2023, max compression
+gzip compressed data, was "mypy-boto3-imagebuilder-1.28.16.tar", last modified: Tue Aug  1 11:36:56 2023, max compression
```

## Comparing `mypy-boto3-imagebuilder-1.28.15.post1.tar` & `mypy-boto3-imagebuilder-1.28.16.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:16.549174 mypy-boto3-imagebuilder-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:47:09.000000 mypy-boto3-imagebuilder-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19996 2023-07-29 10:03:16.545174 mypy-boto3-imagebuilder-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18483 2023-07-29 09:47:09.000000 mypy-boto3-imagebuilder-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:16.537174 mypy-boto3-imagebuilder-1.28.15.post1/mypy_boto3_imagebuilder/
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-29 09:47:09.000000 mypy-boto3-imagebuilder-1.28.15.post1/mypy_boto3_imagebuilder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-29 09:47:09.000000 mypy-boto3-imagebuilder-1.28.15.post1/mypy_boto3_imagebuilder/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-29 09:47:09.000000 mypy-boto3-imagebuilder-1.28.15.post1/mypy_boto3_imagebuilder/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42485 2023-07-29 09:47:09.000000 mypy-boto3-imagebuilder-1.28.15.post1/mypy_boto3_imagebuilder/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    42422 2023-07-29 09:47:09.000000 mypy-boto3-imagebuilder-1.28.15.post1/mypy_boto3_imagebuilder/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9765 2023-07-29 09:47:10.000000 mypy-boto3-imagebuilder-1.28.15.post1/mypy_boto3_imagebuilder/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9763 2023-07-29 09:47:10.000000 mypy-boto3-imagebuilder-1.28.15.post1/mypy_boto3_imagebuilder/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:47:09.000000 mypy-boto3-imagebuilder-1.28.15.post1/mypy_boto3_imagebuilder/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    70589 2023-07-29 09:47:14.000000 mypy-boto3-imagebuilder-1.28.15.post1/mypy_boto3_imagebuilder/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    70528 2023-07-29 09:47:11.000000 mypy-boto3-imagebuilder-1.28.15.post1/mypy_boto3_imagebuilder/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:47:09.000000 mypy-boto3-imagebuilder-1.28.15.post1/mypy_boto3_imagebuilder/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:16.545174 mypy-boto3-imagebuilder-1.28.15.post1/mypy_boto3_imagebuilder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19996 2023-07-29 10:03:16.000000 mypy-boto3-imagebuilder-1.28.15.post1/mypy_boto3_imagebuilder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-29 10:03:16.000000 mypy-boto3-imagebuilder-1.28.15.post1/mypy_boto3_imagebuilder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:16.000000 mypy-boto3-imagebuilder-1.28.15.post1/mypy_boto3_imagebuilder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:16.000000 mypy-boto3-imagebuilder-1.28.15.post1/mypy_boto3_imagebuilder.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:16.000000 mypy-boto3-imagebuilder-1.28.15.post1/mypy_boto3_imagebuilder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-29 10:03:16.000000 mypy-boto3-imagebuilder-1.28.15.post1/mypy_boto3_imagebuilder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:16.549174 mypy-boto3-imagebuilder-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-07-29 09:47:09.000000 mypy-boto3-imagebuilder-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:56.324873 mypy-boto3-imagebuilder-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:19:49.000000 mypy-boto3-imagebuilder-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20139 2023-08-01 11:36:56.316873 mypy-boto3-imagebuilder-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18635 2023-08-01 11:19:49.000000 mypy-boto3-imagebuilder-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:56.316873 mypy-boto3-imagebuilder-1.28.16/mypy_boto3_imagebuilder/
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-08-01 11:19:49.000000 mypy-boto3-imagebuilder-1.28.16/mypy_boto3_imagebuilder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-08-01 11:19:49.000000 mypy-boto3-imagebuilder-1.28.16/mypy_boto3_imagebuilder/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-08-01 11:19:49.000000 mypy-boto3-imagebuilder-1.28.16/mypy_boto3_imagebuilder/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41906 2023-08-01 11:19:49.000000 mypy-boto3-imagebuilder-1.28.16/mypy_boto3_imagebuilder/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41843 2023-08-01 11:19:49.000000 mypy-boto3-imagebuilder-1.28.16/mypy_boto3_imagebuilder/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9765 2023-08-01 11:19:49.000000 mypy-boto3-imagebuilder-1.28.16/mypy_boto3_imagebuilder/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9763 2023-08-01 11:19:49.000000 mypy-boto3-imagebuilder-1.28.16/mypy_boto3_imagebuilder/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:19:49.000000 mypy-boto3-imagebuilder-1.28.16/mypy_boto3_imagebuilder/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    71009 2023-08-01 11:19:53.000000 mypy-boto3-imagebuilder-1.28.16/mypy_boto3_imagebuilder/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70948 2023-08-01 11:19:52.000000 mypy-boto3-imagebuilder-1.28.16/mypy_boto3_imagebuilder/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:19:49.000000 mypy-boto3-imagebuilder-1.28.16/mypy_boto3_imagebuilder/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:56.316873 mypy-boto3-imagebuilder-1.28.16/mypy_boto3_imagebuilder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20139 2023-08-01 11:36:56.000000 mypy-boto3-imagebuilder-1.28.16/mypy_boto3_imagebuilder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-08-01 11:36:56.000000 mypy-boto3-imagebuilder-1.28.16/mypy_boto3_imagebuilder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:56.000000 mypy-boto3-imagebuilder-1.28.16/mypy_boto3_imagebuilder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:56.000000 mypy-boto3-imagebuilder-1.28.16/mypy_boto3_imagebuilder.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:56.000000 mypy-boto3-imagebuilder-1.28.16/mypy_boto3_imagebuilder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-01 11:36:56.000000 mypy-boto3-imagebuilder-1.28.16/mypy_boto3_imagebuilder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:56.324873 mypy-boto3-imagebuilder-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-08-01 11:19:48.000000 mypy-boto3-imagebuilder-1.28.16/setup.py
```

### Comparing `mypy-boto3-imagebuilder-1.28.15.post1/LICENSE` & `mypy-boto3-imagebuilder-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-imagebuilder-1.28.15.post1/PKG-INFO` & `mypy-boto3-imagebuilder-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-imagebuilder
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.imagebuilder 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.imagebuilder 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_imagebuilder/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 imagebuilder type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 imagebuilder type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-imagebuilder.svg?color=blue)](https://pypi.org/project/mypy-boto3-imagebuilder)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_imagebuilder/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-imagebuilder)](https://pepy.tech/project/mypy-boto3-imagebuilder)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.imagebuilder 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder)
+[boto3.imagebuilder 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder)
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
 [mypy-boto3-imagebuilder docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_imagebuilder/).
 
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
@@ -306,20 +306,20 @@
 )
 
 
 def check_value(value: BuildTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_imagebuilder.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_imagebuilder.type_defs import (
     SeverityCountsTypeDef,
     SystemsManagerAgentTypeDef,
     LaunchPermissionConfigurationOutputTypeDef,
     LaunchPermissionConfigurationTypeDef,
@@ -466,53 +466,57 @@
     ListWorkflowExecutionsResponseTypeDef,
     ListWorkflowStepExecutionsResponseTypeDef,
     LoggingTypeDef,
     PackageVulnerabilityDetailsTypeDef,
     RemediationTypeDef,
     ImageScanFindingAggregationTypeDef,
     OutputResourcesTypeDef,
+    ComponentConfigurationUnionTypeDef,
     ListComponentBuildVersionsResponseTypeDef,
     GetComponentResponseTypeDef,
     InspectorScoreDetailsTypeDef,
-    CreateImageRecipeRequestRequestTypeDef,
     ImageRecipeTypeDef,
     InstanceConfigurationOutputTypeDef,
     InstanceConfigurationTypeDef,
     ImagePipelineTypeDef,
     CreateImagePipelineRequestRequestTypeDef,
     CreateImageRequestRequestTypeDef,
+    ImageScanningConfigurationUnionTypeDef,
     UpdateImagePipelineRequestRequestTypeDef,
     DistributionOutputTypeDef,
     DistributionTypeDef,
     CreateInfrastructureConfigurationRequestRequestTypeDef,
     InfrastructureConfigurationTypeDef,
     UpdateInfrastructureConfigurationRequestRequestTypeDef,
     ListImageScanFindingAggregationsResponseTypeDef,
     ImageSummaryTypeDef,
+    CreateImageRecipeRequestRequestTypeDef,
     ImageScanFindingTypeDef,
     GetImageRecipeResponseTypeDef,
     ContainerRecipeTypeDef,
     CreateContainerRecipeRequestRequestTypeDef,
+    InstanceConfigurationUnionTypeDef,
     GetImagePipelineResponseTypeDef,
     ListImagePipelinesResponseTypeDef,
     DistributionConfigurationTypeDef,
-    CreateDistributionConfigurationRequestRequestTypeDef,
-    UpdateDistributionConfigurationRequestRequestTypeDef,
+    DistributionUnionTypeDef,
     GetInfrastructureConfigurationResponseTypeDef,
     ListImageBuildVersionsResponseTypeDef,
     ListImagePipelineImagesResponseTypeDef,
     ListImageScanFindingsResponseTypeDef,
     GetContainerRecipeResponseTypeDef,
     GetDistributionConfigurationResponseTypeDef,
     ImageTypeDef,
+    CreateDistributionConfigurationRequestRequestTypeDef,
+    UpdateDistributionConfigurationRequestRequestTypeDef,
     GetImageResponseTypeDef,
 )
 
 
-def get_structure() -> SeverityCountsTypeDef:
+def get_value() -> SeverityCountsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-imagebuilder-1.28.15.post1/README.md` & `mypy-boto3-imagebuilder-1.28.16/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-imagebuilder.svg?color=blue)](https://pypi.org/project/mypy-boto3-imagebuilder)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_imagebuilder/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-imagebuilder)](https://pepy.tech/project/mypy-boto3-imagebuilder)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.imagebuilder 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder)
+[boto3.imagebuilder 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder)
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
 [mypy-boto3-imagebuilder docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_imagebuilder/).
 
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
@@ -274,20 +274,20 @@
 )
 
 
 def check_value(value: BuildTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_imagebuilder.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_imagebuilder.type_defs import (
     SeverityCountsTypeDef,
     SystemsManagerAgentTypeDef,
     LaunchPermissionConfigurationOutputTypeDef,
     LaunchPermissionConfigurationTypeDef,
@@ -434,53 +434,57 @@
     ListWorkflowExecutionsResponseTypeDef,
     ListWorkflowStepExecutionsResponseTypeDef,
     LoggingTypeDef,
     PackageVulnerabilityDetailsTypeDef,
     RemediationTypeDef,
     ImageScanFindingAggregationTypeDef,
     OutputResourcesTypeDef,
+    ComponentConfigurationUnionTypeDef,
     ListComponentBuildVersionsResponseTypeDef,
     GetComponentResponseTypeDef,
     InspectorScoreDetailsTypeDef,
-    CreateImageRecipeRequestRequestTypeDef,
     ImageRecipeTypeDef,
     InstanceConfigurationOutputTypeDef,
     InstanceConfigurationTypeDef,
     ImagePipelineTypeDef,
     CreateImagePipelineRequestRequestTypeDef,
     CreateImageRequestRequestTypeDef,
+    ImageScanningConfigurationUnionTypeDef,
     UpdateImagePipelineRequestRequestTypeDef,
     DistributionOutputTypeDef,
     DistributionTypeDef,
     CreateInfrastructureConfigurationRequestRequestTypeDef,
     InfrastructureConfigurationTypeDef,
     UpdateInfrastructureConfigurationRequestRequestTypeDef,
     ListImageScanFindingAggregationsResponseTypeDef,
     ImageSummaryTypeDef,
+    CreateImageRecipeRequestRequestTypeDef,
     ImageScanFindingTypeDef,
     GetImageRecipeResponseTypeDef,
     ContainerRecipeTypeDef,
     CreateContainerRecipeRequestRequestTypeDef,
+    InstanceConfigurationUnionTypeDef,
     GetImagePipelineResponseTypeDef,
     ListImagePipelinesResponseTypeDef,
     DistributionConfigurationTypeDef,
-    CreateDistributionConfigurationRequestRequestTypeDef,
-    UpdateDistributionConfigurationRequestRequestTypeDef,
+    DistributionUnionTypeDef,
     GetInfrastructureConfigurationResponseTypeDef,
     ListImageBuildVersionsResponseTypeDef,
     ListImagePipelineImagesResponseTypeDef,
     ListImageScanFindingsResponseTypeDef,
     GetContainerRecipeResponseTypeDef,
     GetDistributionConfigurationResponseTypeDef,
     ImageTypeDef,
+    CreateDistributionConfigurationRequestRequestTypeDef,
+    UpdateDistributionConfigurationRequestRequestTypeDef,
     GetImageResponseTypeDef,
 )
 
 
-def get_structure() -> SeverityCountsTypeDef:
+def get_value() -> SeverityCountsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-imagebuilder-1.28.15.post1/mypy_boto3_imagebuilder/__main__.py` & `mypy-boto3-imagebuilder-1.28.16/mypy_boto3_imagebuilder/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.imagebuilder 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.imagebuilder 1.28.16\nVersion:         1.28.16\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_imagebuilder//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder\nOther"
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

### Comparing `mypy-boto3-imagebuilder-1.28.15.post1/mypy_boto3_imagebuilder/client.py` & `mypy-boto3-imagebuilder-1.28.16/mypy_boto3_imagebuilder/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,40 +10,38 @@
     from mypy_boto3_imagebuilder.client import imagebuilderClient
 
     session = Session()
     client: imagebuilderClient = session.client("imagebuilder")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import ComponentTypeType, OwnershipType, PipelineStatusType, PlatformType
 from .type_defs import (
     AdditionalInstanceConfigurationTypeDef,
     CancelImageCreationResponseTypeDef,
-    ComponentConfigurationOutputTypeDef,
-    ComponentConfigurationTypeDef,
+    ComponentConfigurationUnionTypeDef,
     CreateComponentResponseTypeDef,
     CreateContainerRecipeResponseTypeDef,
     CreateDistributionConfigurationResponseTypeDef,
     CreateImagePipelineResponseTypeDef,
     CreateImageRecipeResponseTypeDef,
     CreateImageResponseTypeDef,
     CreateInfrastructureConfigurationResponseTypeDef,
     DeleteComponentResponseTypeDef,
     DeleteContainerRecipeResponseTypeDef,
     DeleteDistributionConfigurationResponseTypeDef,
     DeleteImagePipelineResponseTypeDef,
     DeleteImageRecipeResponseTypeDef,
     DeleteImageResponseTypeDef,
     DeleteInfrastructureConfigurationResponseTypeDef,
-    DistributionOutputTypeDef,
-    DistributionTypeDef,
+    DistributionUnionTypeDef,
     FilterTypeDef,
     GetComponentPolicyResponseTypeDef,
     GetComponentResponseTypeDef,
     GetContainerRecipePolicyResponseTypeDef,
     GetContainerRecipeResponseTypeDef,
     GetDistributionConfigurationResponseTypeDef,
     GetImagePipelineResponseTypeDef,
@@ -51,22 +49,20 @@
     GetImageRecipePolicyResponseTypeDef,
     GetImageRecipeResponseTypeDef,
     GetImageResponseTypeDef,
     GetInfrastructureConfigurationResponseTypeDef,
     GetWorkflowExecutionResponseTypeDef,
     GetWorkflowStepExecutionResponseTypeDef,
     ImageScanFindingsFilterTypeDef,
-    ImageScanningConfigurationOutputTypeDef,
-    ImageScanningConfigurationTypeDef,
+    ImageScanningConfigurationUnionTypeDef,
     ImageTestsConfigurationTypeDef,
     ImportComponentResponseTypeDef,
     ImportVmImageResponseTypeDef,
     InstanceBlockDeviceMappingTypeDef,
-    InstanceConfigurationOutputTypeDef,
-    InstanceConfigurationTypeDef,
+    InstanceConfigurationUnionTypeDef,
     InstanceMetadataOptionsTypeDef,
     ListComponentBuildVersionsResponseTypeDef,
     ListComponentsResponseTypeDef,
     ListContainerRecipesResponseTypeDef,
     ListDistributionConfigurationsResponseTypeDef,
     ListImageBuildVersionsResponseTypeDef,
     ListImagePackagesResponseTypeDef,
@@ -199,24 +195,20 @@
 
     def create_container_recipe(
         self,
         *,
         containerType: Literal["DOCKER"],
         name: str,
         semanticVersion: str,
-        components: Sequence[
-            Union[ComponentConfigurationTypeDef, ComponentConfigurationOutputTypeDef]
-        ],
+        components: Sequence[ComponentConfigurationUnionTypeDef],
         parentImage: str,
         targetRepository: TargetContainerRepositoryTypeDef,
         clientToken: str,
         description: str = ...,
-        instanceConfiguration: Union[
-            InstanceConfigurationTypeDef, InstanceConfigurationOutputTypeDef
-        ] = ...,
+        instanceConfiguration: InstanceConfigurationUnionTypeDef = ...,
         dockerfileTemplateData: str = ...,
         dockerfileTemplateUri: str = ...,
         platformOverride: PlatformType = ...,
         imageOsVersionOverride: str = ...,
         tags: Mapping[str, str] = ...,
         workingDirectory: str = ...,
         kmsKeyId: str = ...
@@ -228,15 +220,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_imagebuilder/client/#create_container_recipe)
         """
 
     def create_distribution_configuration(
         self,
         *,
         name: str,
-        distributions: Sequence[Union[DistributionTypeDef, DistributionOutputTypeDef]],
+        distributions: Sequence[DistributionUnionTypeDef],
         clientToken: str,
         description: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateDistributionConfigurationResponseTypeDef:
         """
         Creates a new distribution configuration.
 
@@ -251,17 +243,15 @@
         clientToken: str,
         imageRecipeArn: str = ...,
         containerRecipeArn: str = ...,
         distributionConfigurationArn: str = ...,
         imageTestsConfiguration: ImageTestsConfigurationTypeDef = ...,
         enhancedImageMetadataEnabled: bool = ...,
         tags: Mapping[str, str] = ...,
-        imageScanningConfiguration: Union[
-            ImageScanningConfigurationTypeDef, ImageScanningConfigurationOutputTypeDef
-        ] = ...
+        imageScanningConfiguration: ImageScanningConfigurationUnionTypeDef = ...
     ) -> CreateImageResponseTypeDef:
         """
         Creates a new image.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder.Client.create_image)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_imagebuilder/client/#create_image)
         """
@@ -277,33 +267,29 @@
         containerRecipeArn: str = ...,
         distributionConfigurationArn: str = ...,
         imageTestsConfiguration: ImageTestsConfigurationTypeDef = ...,
         enhancedImageMetadataEnabled: bool = ...,
         schedule: ScheduleTypeDef = ...,
         status: PipelineStatusType = ...,
         tags: Mapping[str, str] = ...,
-        imageScanningConfiguration: Union[
-            ImageScanningConfigurationTypeDef, ImageScanningConfigurationOutputTypeDef
-        ] = ...
+        imageScanningConfiguration: ImageScanningConfigurationUnionTypeDef = ...
     ) -> CreateImagePipelineResponseTypeDef:
         """
         Creates a new image pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder.Client.create_image_pipeline)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_imagebuilder/client/#create_image_pipeline)
         """
 
     def create_image_recipe(
         self,
         *,
         name: str,
         semanticVersion: str,
-        components: Sequence[
-            Union[ComponentConfigurationTypeDef, ComponentConfigurationOutputTypeDef]
-        ],
+        components: Sequence[ComponentConfigurationUnionTypeDef],
         parentImage: str,
         clientToken: str,
         description: str = ...,
         blockDeviceMappings: Sequence[InstanceBlockDeviceMappingTypeDef] = ...,
         tags: Mapping[str, str] = ...,
         workingDirectory: str = ...,
         additionalInstanceConfiguration: AdditionalInstanceConfigurationTypeDef = ...
@@ -841,15 +827,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_imagebuilder/client/#untag_resource)
         """
 
     def update_distribution_configuration(
         self,
         *,
         distributionConfigurationArn: str,
-        distributions: Sequence[Union[DistributionTypeDef, DistributionOutputTypeDef]],
+        distributions: Sequence[DistributionUnionTypeDef],
         clientToken: str,
         description: str = ...
     ) -> UpdateDistributionConfigurationResponseTypeDef:
         """
         Updates a new distribution configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder.Client.update_distribution_configuration)
@@ -866,17 +852,15 @@
         imageRecipeArn: str = ...,
         containerRecipeArn: str = ...,
         distributionConfigurationArn: str = ...,
         imageTestsConfiguration: ImageTestsConfigurationTypeDef = ...,
         enhancedImageMetadataEnabled: bool = ...,
         schedule: ScheduleTypeDef = ...,
         status: PipelineStatusType = ...,
-        imageScanningConfiguration: Union[
-            ImageScanningConfigurationTypeDef, ImageScanningConfigurationOutputTypeDef
-        ] = ...
+        imageScanningConfiguration: ImageScanningConfigurationUnionTypeDef = ...
     ) -> UpdateImagePipelineResponseTypeDef:
         """
         Updates an image pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder.Client.update_image_pipeline)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_imagebuilder/client/#update_image_pipeline)
         """
```

### Comparing `mypy-boto3-imagebuilder-1.28.15.post1/mypy_boto3_imagebuilder/client.pyi` & `mypy-boto3-imagebuilder-1.28.16/mypy_boto3_imagebuilder/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -10,40 +10,38 @@
     from mypy_boto3_imagebuilder.client import imagebuilderClient
 
     session = Session()
     client: imagebuilderClient = session.client("imagebuilder")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import ComponentTypeType, OwnershipType, PipelineStatusType, PlatformType
 from .type_defs import (
     AdditionalInstanceConfigurationTypeDef,
     CancelImageCreationResponseTypeDef,
-    ComponentConfigurationOutputTypeDef,
-    ComponentConfigurationTypeDef,
+    ComponentConfigurationUnionTypeDef,
     CreateComponentResponseTypeDef,
     CreateContainerRecipeResponseTypeDef,
     CreateDistributionConfigurationResponseTypeDef,
     CreateImagePipelineResponseTypeDef,
     CreateImageRecipeResponseTypeDef,
     CreateImageResponseTypeDef,
     CreateInfrastructureConfigurationResponseTypeDef,
     DeleteComponentResponseTypeDef,
     DeleteContainerRecipeResponseTypeDef,
     DeleteDistributionConfigurationResponseTypeDef,
     DeleteImagePipelineResponseTypeDef,
     DeleteImageRecipeResponseTypeDef,
     DeleteImageResponseTypeDef,
     DeleteInfrastructureConfigurationResponseTypeDef,
-    DistributionOutputTypeDef,
-    DistributionTypeDef,
+    DistributionUnionTypeDef,
     FilterTypeDef,
     GetComponentPolicyResponseTypeDef,
     GetComponentResponseTypeDef,
     GetContainerRecipePolicyResponseTypeDef,
     GetContainerRecipeResponseTypeDef,
     GetDistributionConfigurationResponseTypeDef,
     GetImagePipelineResponseTypeDef,
@@ -51,22 +49,20 @@
     GetImageRecipePolicyResponseTypeDef,
     GetImageRecipeResponseTypeDef,
     GetImageResponseTypeDef,
     GetInfrastructureConfigurationResponseTypeDef,
     GetWorkflowExecutionResponseTypeDef,
     GetWorkflowStepExecutionResponseTypeDef,
     ImageScanFindingsFilterTypeDef,
-    ImageScanningConfigurationOutputTypeDef,
-    ImageScanningConfigurationTypeDef,
+    ImageScanningConfigurationUnionTypeDef,
     ImageTestsConfigurationTypeDef,
     ImportComponentResponseTypeDef,
     ImportVmImageResponseTypeDef,
     InstanceBlockDeviceMappingTypeDef,
-    InstanceConfigurationOutputTypeDef,
-    InstanceConfigurationTypeDef,
+    InstanceConfigurationUnionTypeDef,
     InstanceMetadataOptionsTypeDef,
     ListComponentBuildVersionsResponseTypeDef,
     ListComponentsResponseTypeDef,
     ListContainerRecipesResponseTypeDef,
     ListDistributionConfigurationsResponseTypeDef,
     ListImageBuildVersionsResponseTypeDef,
     ListImagePackagesResponseTypeDef,
@@ -190,24 +186,20 @@
         """
     def create_container_recipe(
         self,
         *,
         containerType: Literal["DOCKER"],
         name: str,
         semanticVersion: str,
-        components: Sequence[
-            Union[ComponentConfigurationTypeDef, ComponentConfigurationOutputTypeDef]
-        ],
+        components: Sequence[ComponentConfigurationUnionTypeDef],
         parentImage: str,
         targetRepository: TargetContainerRepositoryTypeDef,
         clientToken: str,
         description: str = ...,
-        instanceConfiguration: Union[
-            InstanceConfigurationTypeDef, InstanceConfigurationOutputTypeDef
-        ] = ...,
+        instanceConfiguration: InstanceConfigurationUnionTypeDef = ...,
         dockerfileTemplateData: str = ...,
         dockerfileTemplateUri: str = ...,
         platformOverride: PlatformType = ...,
         imageOsVersionOverride: str = ...,
         tags: Mapping[str, str] = ...,
         workingDirectory: str = ...,
         kmsKeyId: str = ...
@@ -218,15 +210,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder.Client.create_container_recipe)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_imagebuilder/client/#create_container_recipe)
         """
     def create_distribution_configuration(
         self,
         *,
         name: str,
-        distributions: Sequence[Union[DistributionTypeDef, DistributionOutputTypeDef]],
+        distributions: Sequence[DistributionUnionTypeDef],
         clientToken: str,
         description: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateDistributionConfigurationResponseTypeDef:
         """
         Creates a new distribution configuration.
 
@@ -240,17 +232,15 @@
         clientToken: str,
         imageRecipeArn: str = ...,
         containerRecipeArn: str = ...,
         distributionConfigurationArn: str = ...,
         imageTestsConfiguration: ImageTestsConfigurationTypeDef = ...,
         enhancedImageMetadataEnabled: bool = ...,
         tags: Mapping[str, str] = ...,
-        imageScanningConfiguration: Union[
-            ImageScanningConfigurationTypeDef, ImageScanningConfigurationOutputTypeDef
-        ] = ...
+        imageScanningConfiguration: ImageScanningConfigurationUnionTypeDef = ...
     ) -> CreateImageResponseTypeDef:
         """
         Creates a new image.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder.Client.create_image)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_imagebuilder/client/#create_image)
         """
@@ -265,32 +255,28 @@
         containerRecipeArn: str = ...,
         distributionConfigurationArn: str = ...,
         imageTestsConfiguration: ImageTestsConfigurationTypeDef = ...,
         enhancedImageMetadataEnabled: bool = ...,
         schedule: ScheduleTypeDef = ...,
         status: PipelineStatusType = ...,
         tags: Mapping[str, str] = ...,
-        imageScanningConfiguration: Union[
-            ImageScanningConfigurationTypeDef, ImageScanningConfigurationOutputTypeDef
-        ] = ...
+        imageScanningConfiguration: ImageScanningConfigurationUnionTypeDef = ...
     ) -> CreateImagePipelineResponseTypeDef:
         """
         Creates a new image pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder.Client.create_image_pipeline)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_imagebuilder/client/#create_image_pipeline)
         """
     def create_image_recipe(
         self,
         *,
         name: str,
         semanticVersion: str,
-        components: Sequence[
-            Union[ComponentConfigurationTypeDef, ComponentConfigurationOutputTypeDef]
-        ],
+        components: Sequence[ComponentConfigurationUnionTypeDef],
         parentImage: str,
         clientToken: str,
         description: str = ...,
         blockDeviceMappings: Sequence[InstanceBlockDeviceMappingTypeDef] = ...,
         tags: Mapping[str, str] = ...,
         workingDirectory: str = ...,
         additionalInstanceConfiguration: AdditionalInstanceConfigurationTypeDef = ...
@@ -780,15 +766,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_imagebuilder/client/#untag_resource)
         """
     def update_distribution_configuration(
         self,
         *,
         distributionConfigurationArn: str,
-        distributions: Sequence[Union[DistributionTypeDef, DistributionOutputTypeDef]],
+        distributions: Sequence[DistributionUnionTypeDef],
         clientToken: str,
         description: str = ...
     ) -> UpdateDistributionConfigurationResponseTypeDef:
         """
         Updates a new distribution configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder.Client.update_distribution_configuration)
@@ -804,17 +790,15 @@
         imageRecipeArn: str = ...,
         containerRecipeArn: str = ...,
         distributionConfigurationArn: str = ...,
         imageTestsConfiguration: ImageTestsConfigurationTypeDef = ...,
         enhancedImageMetadataEnabled: bool = ...,
         schedule: ScheduleTypeDef = ...,
         status: PipelineStatusType = ...,
-        imageScanningConfiguration: Union[
-            ImageScanningConfigurationTypeDef, ImageScanningConfigurationOutputTypeDef
-        ] = ...
+        imageScanningConfiguration: ImageScanningConfigurationUnionTypeDef = ...
     ) -> UpdateImagePipelineResponseTypeDef:
         """
         Updates an image pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder.Client.update_image_pipeline)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_imagebuilder/client/#update_image_pipeline)
         """
```

### Comparing `mypy-boto3-imagebuilder-1.28.15.post1/mypy_boto3_imagebuilder/literals.py` & `mypy-boto3-imagebuilder-1.28.16/mypy_boto3_imagebuilder/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-imagebuilder-1.28.15.post1/mypy_boto3_imagebuilder/literals.pyi` & `mypy-boto3-imagebuilder-1.28.16/mypy_boto3_imagebuilder/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-imagebuilder-1.28.15.post1/mypy_boto3_imagebuilder/type_defs.py` & `mypy-boto3-imagebuilder-1.28.16/mypy_boto3_imagebuilder/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_imagebuilder/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_imagebuilder.type_defs import SeverityCountsTypeDef
 
-    data: SeverityCountsTypeDef = {...}
+    data: SeverityCountsTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -192,48 +192,52 @@
     "ListWorkflowExecutionsResponseTypeDef",
     "ListWorkflowStepExecutionsResponseTypeDef",
     "LoggingTypeDef",
     "PackageVulnerabilityDetailsTypeDef",
     "RemediationTypeDef",
     "ImageScanFindingAggregationTypeDef",
     "OutputResourcesTypeDef",
+    "ComponentConfigurationUnionTypeDef",
     "ListComponentBuildVersionsResponseTypeDef",
     "GetComponentResponseTypeDef",
     "InspectorScoreDetailsTypeDef",
-    "CreateImageRecipeRequestRequestTypeDef",
     "ImageRecipeTypeDef",
     "InstanceConfigurationOutputTypeDef",
     "InstanceConfigurationTypeDef",
     "ImagePipelineTypeDef",
     "CreateImagePipelineRequestRequestTypeDef",
     "CreateImageRequestRequestTypeDef",
+    "ImageScanningConfigurationUnionTypeDef",
     "UpdateImagePipelineRequestRequestTypeDef",
     "DistributionOutputTypeDef",
     "DistributionTypeDef",
     "CreateInfrastructureConfigurationRequestRequestTypeDef",
     "InfrastructureConfigurationTypeDef",
     "UpdateInfrastructureConfigurationRequestRequestTypeDef",
     "ListImageScanFindingAggregationsResponseTypeDef",
     "ImageSummaryTypeDef",
+    "CreateImageRecipeRequestRequestTypeDef",
     "ImageScanFindingTypeDef",
     "GetImageRecipeResponseTypeDef",
     "ContainerRecipeTypeDef",
     "CreateContainerRecipeRequestRequestTypeDef",
+    "InstanceConfigurationUnionTypeDef",
     "GetImagePipelineResponseTypeDef",
     "ListImagePipelinesResponseTypeDef",
     "DistributionConfigurationTypeDef",
-    "CreateDistributionConfigurationRequestRequestTypeDef",
-    "UpdateDistributionConfigurationRequestRequestTypeDef",
+    "DistributionUnionTypeDef",
     "GetInfrastructureConfigurationResponseTypeDef",
     "ListImageBuildVersionsResponseTypeDef",
     "ListImagePipelineImagesResponseTypeDef",
     "ListImageScanFindingsResponseTypeDef",
     "GetContainerRecipeResponseTypeDef",
     "GetDistributionConfigurationResponseTypeDef",
     "ImageTypeDef",
+    "CreateDistributionConfigurationRequestRequestTypeDef",
+    "UpdateDistributionConfigurationRequestRequestTypeDef",
     "GetImageResponseTypeDef",
 )
 
 SeverityCountsTypeDef = TypedDict(
     "SeverityCountsTypeDef",
     {
         "all": int,
@@ -2004,14 +2008,17 @@
     {
         "amis": List[AmiTypeDef],
         "containers": List[ContainerTypeDef],
     },
     total=False,
 )
 
+ComponentConfigurationUnionTypeDef = Union[
+    ComponentConfigurationTypeDef, ComponentConfigurationOutputTypeDef
+]
 ListComponentBuildVersionsResponseTypeDef = TypedDict(
     "ListComponentBuildVersionsResponseTypeDef",
     {
         "requestId": str,
         "componentSummaryList": List[ComponentSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -2031,45 +2038,14 @@
     "InspectorScoreDetailsTypeDef",
     {
         "adjustedCvss": CvssScoreDetailsTypeDef,
     },
     total=False,
 )
 
-_RequiredCreateImageRecipeRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateImageRecipeRequestRequestTypeDef",
-    {
-        "name": str,
-        "semanticVersion": str,
-        "components": Sequence[
-            Union[ComponentConfigurationTypeDef, ComponentConfigurationOutputTypeDef]
-        ],
-        "parentImage": str,
-        "clientToken": str,
-    },
-)
-_OptionalCreateImageRecipeRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateImageRecipeRequestRequestTypeDef",
-    {
-        "description": str,
-        "blockDeviceMappings": Sequence[InstanceBlockDeviceMappingTypeDef],
-        "tags": Mapping[str, str],
-        "workingDirectory": str,
-        "additionalInstanceConfiguration": AdditionalInstanceConfigurationTypeDef,
-    },
-    total=False,
-)
-
-
-class CreateImageRecipeRequestRequestTypeDef(
-    _RequiredCreateImageRecipeRequestRequestTypeDef, _OptionalCreateImageRecipeRequestRequestTypeDef
-):
-    pass
-
-
 ImageRecipeTypeDef = TypedDict(
     "ImageRecipeTypeDef",
     {
         "arn": str,
         "type": ImageTypeType,
         "name": str,
         "description": str,
@@ -2187,14 +2163,17 @@
 
 class CreateImageRequestRequestTypeDef(
     _RequiredCreateImageRequestRequestTypeDef, _OptionalCreateImageRequestRequestTypeDef
 ):
     pass
 
 
+ImageScanningConfigurationUnionTypeDef = Union[
+    ImageScanningConfigurationTypeDef, ImageScanningConfigurationOutputTypeDef
+]
 _RequiredUpdateImagePipelineRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateImagePipelineRequestRequestTypeDef",
     {
         "imagePipelineArn": str,
         "infrastructureConfigurationArn": str,
         "clientToken": str,
     },
@@ -2390,14 +2369,43 @@
         "tags": Dict[str, str],
         "buildType": BuildTypeType,
         "imageSource": ImageSourceType,
     },
     total=False,
 )
 
+_RequiredCreateImageRecipeRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateImageRecipeRequestRequestTypeDef",
+    {
+        "name": str,
+        "semanticVersion": str,
+        "components": Sequence[ComponentConfigurationUnionTypeDef],
+        "parentImage": str,
+        "clientToken": str,
+    },
+)
+_OptionalCreateImageRecipeRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateImageRecipeRequestRequestTypeDef",
+    {
+        "description": str,
+        "blockDeviceMappings": Sequence[InstanceBlockDeviceMappingTypeDef],
+        "tags": Mapping[str, str],
+        "workingDirectory": str,
+        "additionalInstanceConfiguration": AdditionalInstanceConfigurationTypeDef,
+    },
+    total=False,
+)
+
+
+class CreateImageRecipeRequestRequestTypeDef(
+    _RequiredCreateImageRecipeRequestRequestTypeDef, _OptionalCreateImageRecipeRequestRequestTypeDef
+):
+    pass
+
+
 ImageScanFindingTypeDef = TypedDict(
     "ImageScanFindingTypeDef",
     {
         "awsAccountId": str,
         "imageBuildVersionArn": str,
         "imagePipelineArn": str,
         "type": str,
@@ -2450,17 +2458,15 @@
 
 _RequiredCreateContainerRecipeRequestRequestTypeDef = TypedDict(
     "_RequiredCreateContainerRecipeRequestRequestTypeDef",
     {
         "containerType": Literal["DOCKER"],
         "name": str,
         "semanticVersion": str,
-        "components": Sequence[
-            Union[ComponentConfigurationTypeDef, ComponentConfigurationOutputTypeDef]
-        ],
+        "components": Sequence[ComponentConfigurationUnionTypeDef],
         "parentImage": str,
         "targetRepository": TargetContainerRepositoryTypeDef,
         "clientToken": str,
     },
 )
 _OptionalCreateContainerRecipeRequestRequestTypeDef = TypedDict(
     "_OptionalCreateContainerRecipeRequestRequestTypeDef",
@@ -2482,14 +2488,17 @@
 class CreateContainerRecipeRequestRequestTypeDef(
     _RequiredCreateContainerRecipeRequestRequestTypeDef,
     _OptionalCreateContainerRecipeRequestRequestTypeDef,
 ):
     pass
 
 
+InstanceConfigurationUnionTypeDef = Union[
+    InstanceConfigurationTypeDef, InstanceConfigurationOutputTypeDef
+]
 GetImagePipelineResponseTypeDef = TypedDict(
     "GetImagePipelineResponseTypeDef",
     {
         "requestId": str,
         "imagePipeline": ImagePipelineTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2528,63 +2537,15 @@
 
 class DistributionConfigurationTypeDef(
     _RequiredDistributionConfigurationTypeDef, _OptionalDistributionConfigurationTypeDef
 ):
     pass
 
 
-_RequiredCreateDistributionConfigurationRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateDistributionConfigurationRequestRequestTypeDef",
-    {
-        "name": str,
-        "distributions": Sequence[Union[DistributionTypeDef, DistributionOutputTypeDef]],
-        "clientToken": str,
-    },
-)
-_OptionalCreateDistributionConfigurationRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateDistributionConfigurationRequestRequestTypeDef",
-    {
-        "description": str,
-        "tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-
-class CreateDistributionConfigurationRequestRequestTypeDef(
-    _RequiredCreateDistributionConfigurationRequestRequestTypeDef,
-    _OptionalCreateDistributionConfigurationRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredUpdateDistributionConfigurationRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateDistributionConfigurationRequestRequestTypeDef",
-    {
-        "distributionConfigurationArn": str,
-        "distributions": Sequence[Union[DistributionTypeDef, DistributionOutputTypeDef]],
-        "clientToken": str,
-    },
-)
-_OptionalUpdateDistributionConfigurationRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateDistributionConfigurationRequestRequestTypeDef",
-    {
-        "description": str,
-    },
-    total=False,
-)
-
-
-class UpdateDistributionConfigurationRequestRequestTypeDef(
-    _RequiredUpdateDistributionConfigurationRequestRequestTypeDef,
-    _OptionalUpdateDistributionConfigurationRequestRequestTypeDef,
-):
-    pass
-
-
+DistributionUnionTypeDef = Union[DistributionTypeDef, DistributionOutputTypeDef]
 GetInfrastructureConfigurationResponseTypeDef = TypedDict(
     "GetInfrastructureConfigurationResponseTypeDef",
     {
         "requestId": str,
         "infrastructureConfiguration": InfrastructureConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2663,14 +2624,63 @@
         "imageSource": ImageSourceType,
         "scanState": ImageScanStateTypeDef,
         "imageScanningConfiguration": ImageScanningConfigurationOutputTypeDef,
     },
     total=False,
 )
 
+_RequiredCreateDistributionConfigurationRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateDistributionConfigurationRequestRequestTypeDef",
+    {
+        "name": str,
+        "distributions": Sequence[DistributionUnionTypeDef],
+        "clientToken": str,
+    },
+)
+_OptionalCreateDistributionConfigurationRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateDistributionConfigurationRequestRequestTypeDef",
+    {
+        "description": str,
+        "tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+
+class CreateDistributionConfigurationRequestRequestTypeDef(
+    _RequiredCreateDistributionConfigurationRequestRequestTypeDef,
+    _OptionalCreateDistributionConfigurationRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredUpdateDistributionConfigurationRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateDistributionConfigurationRequestRequestTypeDef",
+    {
+        "distributionConfigurationArn": str,
+        "distributions": Sequence[DistributionUnionTypeDef],
+        "clientToken": str,
+    },
+)
+_OptionalUpdateDistributionConfigurationRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateDistributionConfigurationRequestRequestTypeDef",
+    {
+        "description": str,
+    },
+    total=False,
+)
+
+
+class UpdateDistributionConfigurationRequestRequestTypeDef(
+    _RequiredUpdateDistributionConfigurationRequestRequestTypeDef,
+    _OptionalUpdateDistributionConfigurationRequestRequestTypeDef,
+):
+    pass
+
+
 GetImageResponseTypeDef = TypedDict(
     "GetImageResponseTypeDef",
     {
         "requestId": str,
         "image": ImageTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-imagebuilder-1.28.15.post1/mypy_boto3_imagebuilder/type_defs.pyi` & `mypy-boto3-imagebuilder-1.28.16/mypy_boto3_imagebuilder/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_imagebuilder/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_imagebuilder.type_defs import SeverityCountsTypeDef
 
-    data: SeverityCountsTypeDef = {...}
+    data: SeverityCountsTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -191,48 +191,52 @@
     "ListWorkflowExecutionsResponseTypeDef",
     "ListWorkflowStepExecutionsResponseTypeDef",
     "LoggingTypeDef",
     "PackageVulnerabilityDetailsTypeDef",
     "RemediationTypeDef",
     "ImageScanFindingAggregationTypeDef",
     "OutputResourcesTypeDef",
+    "ComponentConfigurationUnionTypeDef",
     "ListComponentBuildVersionsResponseTypeDef",
     "GetComponentResponseTypeDef",
     "InspectorScoreDetailsTypeDef",
-    "CreateImageRecipeRequestRequestTypeDef",
     "ImageRecipeTypeDef",
     "InstanceConfigurationOutputTypeDef",
     "InstanceConfigurationTypeDef",
     "ImagePipelineTypeDef",
     "CreateImagePipelineRequestRequestTypeDef",
     "CreateImageRequestRequestTypeDef",
+    "ImageScanningConfigurationUnionTypeDef",
     "UpdateImagePipelineRequestRequestTypeDef",
     "DistributionOutputTypeDef",
     "DistributionTypeDef",
     "CreateInfrastructureConfigurationRequestRequestTypeDef",
     "InfrastructureConfigurationTypeDef",
     "UpdateInfrastructureConfigurationRequestRequestTypeDef",
     "ListImageScanFindingAggregationsResponseTypeDef",
     "ImageSummaryTypeDef",
+    "CreateImageRecipeRequestRequestTypeDef",
     "ImageScanFindingTypeDef",
     "GetImageRecipeResponseTypeDef",
     "ContainerRecipeTypeDef",
     "CreateContainerRecipeRequestRequestTypeDef",
+    "InstanceConfigurationUnionTypeDef",
     "GetImagePipelineResponseTypeDef",
     "ListImagePipelinesResponseTypeDef",
     "DistributionConfigurationTypeDef",
-    "CreateDistributionConfigurationRequestRequestTypeDef",
-    "UpdateDistributionConfigurationRequestRequestTypeDef",
+    "DistributionUnionTypeDef",
     "GetInfrastructureConfigurationResponseTypeDef",
     "ListImageBuildVersionsResponseTypeDef",
     "ListImagePipelineImagesResponseTypeDef",
     "ListImageScanFindingsResponseTypeDef",
     "GetContainerRecipeResponseTypeDef",
     "GetDistributionConfigurationResponseTypeDef",
     "ImageTypeDef",
+    "CreateDistributionConfigurationRequestRequestTypeDef",
+    "UpdateDistributionConfigurationRequestRequestTypeDef",
     "GetImageResponseTypeDef",
 )
 
 SeverityCountsTypeDef = TypedDict(
     "SeverityCountsTypeDef",
     {
         "all": int,
@@ -1967,14 +1971,17 @@
     {
         "amis": List[AmiTypeDef],
         "containers": List[ContainerTypeDef],
     },
     total=False,
 )
 
+ComponentConfigurationUnionTypeDef = Union[
+    ComponentConfigurationTypeDef, ComponentConfigurationOutputTypeDef
+]
 ListComponentBuildVersionsResponseTypeDef = TypedDict(
     "ListComponentBuildVersionsResponseTypeDef",
     {
         "requestId": str,
         "componentSummaryList": List[ComponentSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1994,43 +2001,14 @@
     "InspectorScoreDetailsTypeDef",
     {
         "adjustedCvss": CvssScoreDetailsTypeDef,
     },
     total=False,
 )
 
-_RequiredCreateImageRecipeRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateImageRecipeRequestRequestTypeDef",
-    {
-        "name": str,
-        "semanticVersion": str,
-        "components": Sequence[
-            Union[ComponentConfigurationTypeDef, ComponentConfigurationOutputTypeDef]
-        ],
-        "parentImage": str,
-        "clientToken": str,
-    },
-)
-_OptionalCreateImageRecipeRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateImageRecipeRequestRequestTypeDef",
-    {
-        "description": str,
-        "blockDeviceMappings": Sequence[InstanceBlockDeviceMappingTypeDef],
-        "tags": Mapping[str, str],
-        "workingDirectory": str,
-        "additionalInstanceConfiguration": AdditionalInstanceConfigurationTypeDef,
-    },
-    total=False,
-)
-
-class CreateImageRecipeRequestRequestTypeDef(
-    _RequiredCreateImageRecipeRequestRequestTypeDef, _OptionalCreateImageRecipeRequestRequestTypeDef
-):
-    pass
-
 ImageRecipeTypeDef = TypedDict(
     "ImageRecipeTypeDef",
     {
         "arn": str,
         "type": ImageTypeType,
         "name": str,
         "description": str,
@@ -2144,14 +2122,17 @@
 )
 
 class CreateImageRequestRequestTypeDef(
     _RequiredCreateImageRequestRequestTypeDef, _OptionalCreateImageRequestRequestTypeDef
 ):
     pass
 
+ImageScanningConfigurationUnionTypeDef = Union[
+    ImageScanningConfigurationTypeDef, ImageScanningConfigurationOutputTypeDef
+]
 _RequiredUpdateImagePipelineRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateImagePipelineRequestRequestTypeDef",
     {
         "imagePipelineArn": str,
         "infrastructureConfigurationArn": str,
         "clientToken": str,
     },
@@ -2337,14 +2318,41 @@
         "tags": Dict[str, str],
         "buildType": BuildTypeType,
         "imageSource": ImageSourceType,
     },
     total=False,
 )
 
+_RequiredCreateImageRecipeRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateImageRecipeRequestRequestTypeDef",
+    {
+        "name": str,
+        "semanticVersion": str,
+        "components": Sequence[ComponentConfigurationUnionTypeDef],
+        "parentImage": str,
+        "clientToken": str,
+    },
+)
+_OptionalCreateImageRecipeRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateImageRecipeRequestRequestTypeDef",
+    {
+        "description": str,
+        "blockDeviceMappings": Sequence[InstanceBlockDeviceMappingTypeDef],
+        "tags": Mapping[str, str],
+        "workingDirectory": str,
+        "additionalInstanceConfiguration": AdditionalInstanceConfigurationTypeDef,
+    },
+    total=False,
+)
+
+class CreateImageRecipeRequestRequestTypeDef(
+    _RequiredCreateImageRecipeRequestRequestTypeDef, _OptionalCreateImageRecipeRequestRequestTypeDef
+):
+    pass
+
 ImageScanFindingTypeDef = TypedDict(
     "ImageScanFindingTypeDef",
     {
         "awsAccountId": str,
         "imageBuildVersionArn": str,
         "imagePipelineArn": str,
         "type": str,
@@ -2397,17 +2405,15 @@
 
 _RequiredCreateContainerRecipeRequestRequestTypeDef = TypedDict(
     "_RequiredCreateContainerRecipeRequestRequestTypeDef",
     {
         "containerType": Literal["DOCKER"],
         "name": str,
         "semanticVersion": str,
-        "components": Sequence[
-            Union[ComponentConfigurationTypeDef, ComponentConfigurationOutputTypeDef]
-        ],
+        "components": Sequence[ComponentConfigurationUnionTypeDef],
         "parentImage": str,
         "targetRepository": TargetContainerRepositoryTypeDef,
         "clientToken": str,
     },
 )
 _OptionalCreateContainerRecipeRequestRequestTypeDef = TypedDict(
     "_OptionalCreateContainerRecipeRequestRequestTypeDef",
@@ -2427,14 +2433,17 @@
 
 class CreateContainerRecipeRequestRequestTypeDef(
     _RequiredCreateContainerRecipeRequestRequestTypeDef,
     _OptionalCreateContainerRecipeRequestRequestTypeDef,
 ):
     pass
 
+InstanceConfigurationUnionTypeDef = Union[
+    InstanceConfigurationTypeDef, InstanceConfigurationOutputTypeDef
+]
 GetImagePipelineResponseTypeDef = TypedDict(
     "GetImagePipelineResponseTypeDef",
     {
         "requestId": str,
         "imagePipeline": ImagePipelineTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2471,59 +2480,15 @@
 )
 
 class DistributionConfigurationTypeDef(
     _RequiredDistributionConfigurationTypeDef, _OptionalDistributionConfigurationTypeDef
 ):
     pass
 
-_RequiredCreateDistributionConfigurationRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateDistributionConfigurationRequestRequestTypeDef",
-    {
-        "name": str,
-        "distributions": Sequence[Union[DistributionTypeDef, DistributionOutputTypeDef]],
-        "clientToken": str,
-    },
-)
-_OptionalCreateDistributionConfigurationRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateDistributionConfigurationRequestRequestTypeDef",
-    {
-        "description": str,
-        "tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-class CreateDistributionConfigurationRequestRequestTypeDef(
-    _RequiredCreateDistributionConfigurationRequestRequestTypeDef,
-    _OptionalCreateDistributionConfigurationRequestRequestTypeDef,
-):
-    pass
-
-_RequiredUpdateDistributionConfigurationRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateDistributionConfigurationRequestRequestTypeDef",
-    {
-        "distributionConfigurationArn": str,
-        "distributions": Sequence[Union[DistributionTypeDef, DistributionOutputTypeDef]],
-        "clientToken": str,
-    },
-)
-_OptionalUpdateDistributionConfigurationRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateDistributionConfigurationRequestRequestTypeDef",
-    {
-        "description": str,
-    },
-    total=False,
-)
-
-class UpdateDistributionConfigurationRequestRequestTypeDef(
-    _RequiredUpdateDistributionConfigurationRequestRequestTypeDef,
-    _OptionalUpdateDistributionConfigurationRequestRequestTypeDef,
-):
-    pass
-
+DistributionUnionTypeDef = Union[DistributionTypeDef, DistributionOutputTypeDef]
 GetInfrastructureConfigurationResponseTypeDef = TypedDict(
     "GetInfrastructureConfigurationResponseTypeDef",
     {
         "requestId": str,
         "infrastructureConfiguration": InfrastructureConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2602,14 +2567,59 @@
         "imageSource": ImageSourceType,
         "scanState": ImageScanStateTypeDef,
         "imageScanningConfiguration": ImageScanningConfigurationOutputTypeDef,
     },
     total=False,
 )
 
+_RequiredCreateDistributionConfigurationRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateDistributionConfigurationRequestRequestTypeDef",
+    {
+        "name": str,
+        "distributions": Sequence[DistributionUnionTypeDef],
+        "clientToken": str,
+    },
+)
+_OptionalCreateDistributionConfigurationRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateDistributionConfigurationRequestRequestTypeDef",
+    {
+        "description": str,
+        "tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+class CreateDistributionConfigurationRequestRequestTypeDef(
+    _RequiredCreateDistributionConfigurationRequestRequestTypeDef,
+    _OptionalCreateDistributionConfigurationRequestRequestTypeDef,
+):
+    pass
+
+_RequiredUpdateDistributionConfigurationRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateDistributionConfigurationRequestRequestTypeDef",
+    {
+        "distributionConfigurationArn": str,
+        "distributions": Sequence[DistributionUnionTypeDef],
+        "clientToken": str,
+    },
+)
+_OptionalUpdateDistributionConfigurationRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateDistributionConfigurationRequestRequestTypeDef",
+    {
+        "description": str,
+    },
+    total=False,
+)
+
+class UpdateDistributionConfigurationRequestRequestTypeDef(
+    _RequiredUpdateDistributionConfigurationRequestRequestTypeDef,
+    _OptionalUpdateDistributionConfigurationRequestRequestTypeDef,
+):
+    pass
+
 GetImageResponseTypeDef = TypedDict(
     "GetImageResponseTypeDef",
     {
         "requestId": str,
         "image": ImageTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-imagebuilder-1.28.15.post1/mypy_boto3_imagebuilder.egg-info/PKG-INFO` & `mypy-boto3-imagebuilder-1.28.16/mypy_boto3_imagebuilder.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-imagebuilder
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.imagebuilder 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.imagebuilder 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_imagebuilder/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 imagebuilder type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 imagebuilder type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-imagebuilder.svg?color=blue)](https://pypi.org/project/mypy-boto3-imagebuilder)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_imagebuilder/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-imagebuilder)](https://pepy.tech/project/mypy-boto3-imagebuilder)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.imagebuilder 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder)
+[boto3.imagebuilder 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder)
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
 [mypy-boto3-imagebuilder docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_imagebuilder/).
 
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
@@ -306,20 +306,20 @@
 )
 
 
 def check_value(value: BuildTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_imagebuilder.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_imagebuilder.type_defs import (
     SeverityCountsTypeDef,
     SystemsManagerAgentTypeDef,
     LaunchPermissionConfigurationOutputTypeDef,
     LaunchPermissionConfigurationTypeDef,
@@ -466,53 +466,57 @@
     ListWorkflowExecutionsResponseTypeDef,
     ListWorkflowStepExecutionsResponseTypeDef,
     LoggingTypeDef,
     PackageVulnerabilityDetailsTypeDef,
     RemediationTypeDef,
     ImageScanFindingAggregationTypeDef,
     OutputResourcesTypeDef,
+    ComponentConfigurationUnionTypeDef,
     ListComponentBuildVersionsResponseTypeDef,
     GetComponentResponseTypeDef,
     InspectorScoreDetailsTypeDef,
-    CreateImageRecipeRequestRequestTypeDef,
     ImageRecipeTypeDef,
     InstanceConfigurationOutputTypeDef,
     InstanceConfigurationTypeDef,
     ImagePipelineTypeDef,
     CreateImagePipelineRequestRequestTypeDef,
     CreateImageRequestRequestTypeDef,
+    ImageScanningConfigurationUnionTypeDef,
     UpdateImagePipelineRequestRequestTypeDef,
     DistributionOutputTypeDef,
     DistributionTypeDef,
     CreateInfrastructureConfigurationRequestRequestTypeDef,
     InfrastructureConfigurationTypeDef,
     UpdateInfrastructureConfigurationRequestRequestTypeDef,
     ListImageScanFindingAggregationsResponseTypeDef,
     ImageSummaryTypeDef,
+    CreateImageRecipeRequestRequestTypeDef,
     ImageScanFindingTypeDef,
     GetImageRecipeResponseTypeDef,
     ContainerRecipeTypeDef,
     CreateContainerRecipeRequestRequestTypeDef,
+    InstanceConfigurationUnionTypeDef,
     GetImagePipelineResponseTypeDef,
     ListImagePipelinesResponseTypeDef,
     DistributionConfigurationTypeDef,
-    CreateDistributionConfigurationRequestRequestTypeDef,
-    UpdateDistributionConfigurationRequestRequestTypeDef,
+    DistributionUnionTypeDef,
     GetInfrastructureConfigurationResponseTypeDef,
     ListImageBuildVersionsResponseTypeDef,
     ListImagePipelineImagesResponseTypeDef,
     ListImageScanFindingsResponseTypeDef,
     GetContainerRecipeResponseTypeDef,
     GetDistributionConfigurationResponseTypeDef,
     ImageTypeDef,
+    CreateDistributionConfigurationRequestRequestTypeDef,
+    UpdateDistributionConfigurationRequestRequestTypeDef,
     GetImageResponseTypeDef,
 )
 
 
-def get_structure() -> SeverityCountsTypeDef:
+def get_value() -> SeverityCountsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-imagebuilder-1.28.15.post1/mypy_boto3_imagebuilder.egg-info/SOURCES.txt` & `mypy-boto3-imagebuilder-1.28.16/mypy_boto3_imagebuilder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-imagebuilder-1.28.15.post1/setup.py` & `mypy-boto3-imagebuilder-1.28.16/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-imagebuilder",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_imagebuilder"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.imagebuilder 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.2"
+        "Type annotations for boto3.imagebuilder 1.28.16 service generated with mypy-boto3-builder"
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
-    keywords="boto3 imagebuilder type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 imagebuilder type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_imagebuilder": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_imagebuilder/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

