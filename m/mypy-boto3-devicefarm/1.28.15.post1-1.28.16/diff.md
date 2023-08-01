# Comparing `tmp/mypy-boto3-devicefarm-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-devicefarm-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-devicefarm-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:55 2023, max compression
+gzip compressed data, was "mypy-boto3-devicefarm-1.28.16.tar", last modified: Tue Aug  1 11:36:35 2023, max compression
```

## Comparing `mypy-boto3-devicefarm-1.28.15.post1.tar` & `mypy-boto3-devicefarm-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:55.797101 mypy-boto3-devicefarm-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:42:13.000000 mypy-boto3-devicefarm-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    24832 2023-07-29 10:02:55.797101 mypy-boto3-devicefarm-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    23327 2023-07-29 09:42:13.000000 mypy-boto3-devicefarm-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:55.789101 mypy-boto3-devicefarm-1.28.15.post1/mypy_boto3_devicefarm/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-07-29 09:42:13.000000 mypy-boto3-devicefarm-1.28.15.post1/mypy_boto3_devicefarm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-07-29 09:42:13.000000 mypy-boto3-devicefarm-1.28.15.post1/mypy_boto3_devicefarm/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-29 09:42:13.000000 mypy-boto3-devicefarm-1.28.15.post1/mypy_boto3_devicefarm/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    58062 2023-07-29 09:42:15.000000 mypy-boto3-devicefarm-1.28.15.post1/mypy_boto3_devicefarm/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    57958 2023-07-29 09:42:15.000000 mypy-boto3-devicefarm-1.28.15.post1/mypy_boto3_devicefarm/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15794 2023-07-29 09:42:15.000000 mypy-boto3-devicefarm-1.28.15.post1/mypy_boto3_devicefarm/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    15792 2023-07-29 09:42:15.000000 mypy-boto3-devicefarm-1.28.15.post1/mypy_boto3_devicefarm/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    22418 2023-07-29 09:42:15.000000 mypy-boto3-devicefarm-1.28.15.post1/mypy_boto3_devicefarm/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    22396 2023-07-29 09:42:15.000000 mypy-boto3-devicefarm-1.28.15.post1/mypy_boto3_devicefarm/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:42:13.000000 mypy-boto3-devicefarm-1.28.15.post1/mypy_boto3_devicefarm/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    74125 2023-07-29 09:42:17.000000 mypy-boto3-devicefarm-1.28.15.post1/mypy_boto3_devicefarm/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    74034 2023-07-29 09:42:16.000000 mypy-boto3-devicefarm-1.28.15.post1/mypy_boto3_devicefarm/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:42:13.000000 mypy-boto3-devicefarm-1.28.15.post1/mypy_boto3_devicefarm/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:55.793101 mypy-boto3-devicefarm-1.28.15.post1/mypy_boto3_devicefarm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    24832 2023-07-29 10:02:55.000000 mypy-boto3-devicefarm-1.28.15.post1/mypy_boto3_devicefarm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-29 10:02:55.000000 mypy-boto3-devicefarm-1.28.15.post1/mypy_boto3_devicefarm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:55.000000 mypy-boto3-devicefarm-1.28.15.post1/mypy_boto3_devicefarm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:55.000000 mypy-boto3-devicefarm-1.28.15.post1/mypy_boto3_devicefarm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:55.000000 mypy-boto3-devicefarm-1.28.15.post1/mypy_boto3_devicefarm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-29 10:02:55.000000 mypy-boto3-devicefarm-1.28.15.post1/mypy_boto3_devicefarm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:55.797101 mypy-boto3-devicefarm-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-07-29 09:42:13.000000 mypy-boto3-devicefarm-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:35.964912 mypy-boto3-devicefarm-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:14:47.000000 mypy-boto3-devicefarm-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    24936 2023-08-01 11:36:35.964912 mypy-boto3-devicefarm-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    23440 2023-08-01 11:14:47.000000 mypy-boto3-devicefarm-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:35.960912 mypy-boto3-devicefarm-1.28.16/mypy_boto3_devicefarm/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-08-01 11:14:47.000000 mypy-boto3-devicefarm-1.28.16/mypy_boto3_devicefarm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-08-01 11:14:47.000000 mypy-boto3-devicefarm-1.28.16/mypy_boto3_devicefarm/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-08-01 11:14:47.000000 mypy-boto3-devicefarm-1.28.16/mypy_boto3_devicefarm/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57770 2023-08-01 11:14:47.000000 mypy-boto3-devicefarm-1.28.16/mypy_boto3_devicefarm/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57666 2023-08-01 11:14:47.000000 mypy-boto3-devicefarm-1.28.16/mypy_boto3_devicefarm/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15794 2023-08-01 11:14:48.000000 mypy-boto3-devicefarm-1.28.16/mypy_boto3_devicefarm/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15792 2023-08-01 11:14:47.000000 mypy-boto3-devicefarm-1.28.16/mypy_boto3_devicefarm/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    22356 2023-08-01 11:14:47.000000 mypy-boto3-devicefarm-1.28.16/mypy_boto3_devicefarm/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22334 2023-08-01 11:14:47.000000 mypy-boto3-devicefarm-1.28.16/mypy_boto3_devicefarm/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:14:47.000000 mypy-boto3-devicefarm-1.28.16/mypy_boto3_devicefarm/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    74460 2023-08-01 11:14:50.000000 mypy-boto3-devicefarm-1.28.16/mypy_boto3_devicefarm/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74369 2023-08-01 11:14:49.000000 mypy-boto3-devicefarm-1.28.16/mypy_boto3_devicefarm/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:14:47.000000 mypy-boto3-devicefarm-1.28.16/mypy_boto3_devicefarm/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:35.964912 mypy-boto3-devicefarm-1.28.16/mypy_boto3_devicefarm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    24936 2023-08-01 11:36:35.000000 mypy-boto3-devicefarm-1.28.16/mypy_boto3_devicefarm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-08-01 11:36:35.000000 mypy-boto3-devicefarm-1.28.16/mypy_boto3_devicefarm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:35.000000 mypy-boto3-devicefarm-1.28.16/mypy_boto3_devicefarm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:35.000000 mypy-boto3-devicefarm-1.28.16/mypy_boto3_devicefarm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:35.000000 mypy-boto3-devicefarm-1.28.16/mypy_boto3_devicefarm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-01 11:36:35.000000 mypy-boto3-devicefarm-1.28.16/mypy_boto3_devicefarm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:35.964912 mypy-boto3-devicefarm-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-08-01 11:14:46.000000 mypy-boto3-devicefarm-1.28.16/setup.py
```

### Comparing `mypy-boto3-devicefarm-1.28.15.post1/LICENSE` & `mypy-boto3-devicefarm-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-devicefarm-1.28.15.post1/PKG-INFO` & `mypy-boto3-devicefarm-1.28.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-devicefarm
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.DeviceFarm 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.DeviceFarm 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 devicefarm type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 devicefarm type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-devicefarm.svg?color=blue)](https://pypi.org/project/mypy-boto3-devicefarm)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-devicefarm)](https://pepy.tech/project/mypy-boto3-devicefarm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DeviceFarm 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm)
+[boto3.DeviceFarm 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm)
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
 [mypy-boto3-devicefarm docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/).
 
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
@@ -414,20 +414,20 @@
 )
 
 
 def check_value(value: ArtifactCategoryType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_devicefarm.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_devicefarm.type_defs import (
     TrialMinutesTypeDef,
     ArtifactTypeDef,
     CPUTypeDef,
     CountersTypeDef,
@@ -501,15 +501,15 @@
     ListTagsForResourceRequestRequestTypeDef,
     TagTypeDef,
     ListTestGridProjectsRequestRequestTypeDef,
     ListTestGridSessionActionsRequestRequestTypeDef,
     TestGridSessionActionTypeDef,
     ListTestGridSessionArtifactsRequestRequestTypeDef,
     TestGridSessionArtifactTypeDef,
-    ListTestGridSessionsRequestRequestTypeDef,
+    TimestampTypeDef,
     ListTestsRequestRequestTypeDef,
     ListUniqueProblemsRequestRequestTypeDef,
     ListUploadsRequestRequestTypeDef,
     ListVPCEConfigurationsRequestRequestTypeDef,
     LocationTypeDef,
     MonetaryAmountTypeDef,
     ProblemDetailTypeDef,
@@ -553,23 +553,22 @@
     ListUploadsResultTypeDef,
     UpdateUploadResultTypeDef,
     CreateVPCEConfigurationResultTypeDef,
     GetVPCEConfigurationResultTypeDef,
     ListVPCEConfigurationsResultTypeDef,
     UpdateVPCEConfigurationResultTypeDef,
     DeviceSelectionResultTypeDef,
+    DeviceFilterUnionTypeDef,
     DeviceSelectionConfigurationTypeDef,
-    ListDevicesRequestRequestTypeDef,
     SuiteTypeDef,
     TestTypeDef,
     GetOfferingStatusRequestGetOfferingStatusPaginateTypeDef,
     ListArtifactsRequestListArtifactsPaginateTypeDef,
     ListDeviceInstancesRequestListDeviceInstancesPaginateTypeDef,
     ListDevicePoolsRequestListDevicePoolsPaginateTypeDef,
-    ListDevicesRequestListDevicesPaginateTypeDef,
     ListInstanceProfilesRequestListInstanceProfilesPaginateTypeDef,
     ListJobsRequestListJobsPaginateTypeDef,
     ListNetworkProfilesRequestListNetworkProfilesPaginateTypeDef,
     ListOfferingPromotionsRequestListOfferingPromotionsPaginateTypeDef,
     ListOfferingTransactionsRequestListOfferingTransactionsPaginateTypeDef,
     ListOfferingsRequestListOfferingsPaginateTypeDef,
     ListProjectsRequestListProjectsPaginateTypeDef,
@@ -585,28 +584,33 @@
     ListTestGridSessionsResultTypeDef,
     ListOfferingPromotionsResultTypeDef,
     ListSamplesResultTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     ListTestGridSessionActionsResultTypeDef,
     ListTestGridSessionArtifactsResultTypeDef,
+    ListTestGridSessionsRequestRequestTypeDef,
     RecurringChargeTypeDef,
     ProjectTypeDef,
+    VpcConfigUnionTypeDef,
     ScheduleRunConfigurationTypeDef,
     TestGridProjectTypeDef,
+    TestGridVpcConfigUnionTypeDef,
     GetAccountSettingsResultTypeDef,
     CreateDevicePoolResultTypeDef,
     GetDevicePoolResultTypeDef,
     ListDevicePoolsResultTypeDef,
     UpdateDevicePoolResultTypeDef,
     DeviceTypeDef,
     GetDeviceInstanceResultTypeDef,
     ListDeviceInstancesResultTypeDef,
     UpdateDeviceInstanceResultTypeDef,
     RunTypeDef,
+    ListDevicesRequestListDevicesPaginateTypeDef,
+    ListDevicesRequestRequestTypeDef,
     GetSuiteResultTypeDef,
     ListSuitesResultTypeDef,
     GetTestResultTypeDef,
     ListTestsResultTypeDef,
     OfferingTypeDef,
     CreateProjectResultTypeDef,
     GetProjectResultTypeDef,
@@ -644,15 +648,15 @@
     ListUniqueProblemsResultTypeDef,
     ListOfferingTransactionsResultTypeDef,
     PurchaseOfferingResultTypeDef,
     RenewOfferingResultTypeDef,
 )
 
 
-def get_structure() -> TrialMinutesTypeDef:
+def get_value() -> TrialMinutesTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-devicefarm-1.28.15.post1/README.md` & `mypy-boto3-devicefarm-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-devicefarm.svg?color=blue)](https://pypi.org/project/mypy-boto3-devicefarm)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-devicefarm)](https://pepy.tech/project/mypy-boto3-devicefarm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DeviceFarm 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm)
+[boto3.DeviceFarm 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm)
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
 [mypy-boto3-devicefarm docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/).
 
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
@@ -382,20 +382,20 @@
 )
 
 
 def check_value(value: ArtifactCategoryType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_devicefarm.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_devicefarm.type_defs import (
     TrialMinutesTypeDef,
     ArtifactTypeDef,
     CPUTypeDef,
     CountersTypeDef,
@@ -469,15 +469,15 @@
     ListTagsForResourceRequestRequestTypeDef,
     TagTypeDef,
     ListTestGridProjectsRequestRequestTypeDef,
     ListTestGridSessionActionsRequestRequestTypeDef,
     TestGridSessionActionTypeDef,
     ListTestGridSessionArtifactsRequestRequestTypeDef,
     TestGridSessionArtifactTypeDef,
-    ListTestGridSessionsRequestRequestTypeDef,
+    TimestampTypeDef,
     ListTestsRequestRequestTypeDef,
     ListUniqueProblemsRequestRequestTypeDef,
     ListUploadsRequestRequestTypeDef,
     ListVPCEConfigurationsRequestRequestTypeDef,
     LocationTypeDef,
     MonetaryAmountTypeDef,
     ProblemDetailTypeDef,
@@ -521,23 +521,22 @@
     ListUploadsResultTypeDef,
     UpdateUploadResultTypeDef,
     CreateVPCEConfigurationResultTypeDef,
     GetVPCEConfigurationResultTypeDef,
     ListVPCEConfigurationsResultTypeDef,
     UpdateVPCEConfigurationResultTypeDef,
     DeviceSelectionResultTypeDef,
+    DeviceFilterUnionTypeDef,
     DeviceSelectionConfigurationTypeDef,
-    ListDevicesRequestRequestTypeDef,
     SuiteTypeDef,
     TestTypeDef,
     GetOfferingStatusRequestGetOfferingStatusPaginateTypeDef,
     ListArtifactsRequestListArtifactsPaginateTypeDef,
     ListDeviceInstancesRequestListDeviceInstancesPaginateTypeDef,
     ListDevicePoolsRequestListDevicePoolsPaginateTypeDef,
-    ListDevicesRequestListDevicesPaginateTypeDef,
     ListInstanceProfilesRequestListInstanceProfilesPaginateTypeDef,
     ListJobsRequestListJobsPaginateTypeDef,
     ListNetworkProfilesRequestListNetworkProfilesPaginateTypeDef,
     ListOfferingPromotionsRequestListOfferingPromotionsPaginateTypeDef,
     ListOfferingTransactionsRequestListOfferingTransactionsPaginateTypeDef,
     ListOfferingsRequestListOfferingsPaginateTypeDef,
     ListProjectsRequestListProjectsPaginateTypeDef,
@@ -553,28 +552,33 @@
     ListTestGridSessionsResultTypeDef,
     ListOfferingPromotionsResultTypeDef,
     ListSamplesResultTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     ListTestGridSessionActionsResultTypeDef,
     ListTestGridSessionArtifactsResultTypeDef,
+    ListTestGridSessionsRequestRequestTypeDef,
     RecurringChargeTypeDef,
     ProjectTypeDef,
+    VpcConfigUnionTypeDef,
     ScheduleRunConfigurationTypeDef,
     TestGridProjectTypeDef,
+    TestGridVpcConfigUnionTypeDef,
     GetAccountSettingsResultTypeDef,
     CreateDevicePoolResultTypeDef,
     GetDevicePoolResultTypeDef,
     ListDevicePoolsResultTypeDef,
     UpdateDevicePoolResultTypeDef,
     DeviceTypeDef,
     GetDeviceInstanceResultTypeDef,
     ListDeviceInstancesResultTypeDef,
     UpdateDeviceInstanceResultTypeDef,
     RunTypeDef,
+    ListDevicesRequestListDevicesPaginateTypeDef,
+    ListDevicesRequestRequestTypeDef,
     GetSuiteResultTypeDef,
     ListSuitesResultTypeDef,
     GetTestResultTypeDef,
     ListTestsResultTypeDef,
     OfferingTypeDef,
     CreateProjectResultTypeDef,
     GetProjectResultTypeDef,
@@ -612,15 +616,15 @@
     ListUniqueProblemsResultTypeDef,
     ListOfferingTransactionsResultTypeDef,
     PurchaseOfferingResultTypeDef,
     RenewOfferingResultTypeDef,
 )
 
 
-def get_structure() -> TrialMinutesTypeDef:
+def get_value() -> TrialMinutesTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-devicefarm-1.28.15.post1/mypy_boto3_devicefarm/__init__.py` & `mypy-boto3-devicefarm-1.28.16/mypy_boto3_devicefarm/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-devicefarm-1.28.15.post1/mypy_boto3_devicefarm/__init__.pyi` & `mypy-boto3-devicefarm-1.28.16/mypy_boto3_devicefarm/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-devicefarm-1.28.15.post1/mypy_boto3_devicefarm/__main__.py` & `mypy-boto3-devicefarm-1.28.16/mypy_boto3_devicefarm/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.DeviceFarm 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.DeviceFarm 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm\nOther"
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

### Comparing `mypy-boto3-devicefarm-1.28.15.post1/mypy_boto3_devicefarm/client.py` & `mypy-boto3-devicefarm-1.28.16/mypy_boto3_devicefarm/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from mypy_boto3_devicefarm.client import DeviceFarmClient
 
     session = Session()
     client: DeviceFarmClient = session.client("devicefarm")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     ArtifactCategoryType,
     DevicePoolTypeType,
     InteractionModeType,
@@ -58,16 +57,15 @@
     CreateProjectResultTypeDef,
     CreateRemoteAccessSessionConfigurationTypeDef,
     CreateRemoteAccessSessionResultTypeDef,
     CreateTestGridProjectResultTypeDef,
     CreateTestGridUrlResultTypeDef,
     CreateUploadResultTypeDef,
     CreateVPCEConfigurationResultTypeDef,
-    DeviceFilterOutputTypeDef,
-    DeviceFilterTypeDef,
+    DeviceFilterUnionTypeDef,
     DeviceSelectionConfigurationTypeDef,
     ExecutionConfigurationTypeDef,
     GetAccountSettingsResultTypeDef,
     GetDeviceInstanceResultTypeDef,
     GetDevicePoolCompatibilityResultTypeDef,
     GetDevicePoolResultTypeDef,
     GetDeviceResultTypeDef,
@@ -115,26 +113,25 @@
     ScheduleRunConfigurationTypeDef,
     ScheduleRunResultTypeDef,
     ScheduleRunTestTypeDef,
     StopJobResultTypeDef,
     StopRemoteAccessSessionResultTypeDef,
     StopRunResultTypeDef,
     TagTypeDef,
-    TestGridVpcConfigOutputTypeDef,
-    TestGridVpcConfigTypeDef,
+    TestGridVpcConfigUnionTypeDef,
+    TimestampTypeDef,
     UpdateDeviceInstanceResultTypeDef,
     UpdateDevicePoolResultTypeDef,
     UpdateInstanceProfileResultTypeDef,
     UpdateNetworkProfileResultTypeDef,
     UpdateProjectResultTypeDef,
     UpdateTestGridProjectResultTypeDef,
     UpdateUploadResultTypeDef,
     UpdateVPCEConfigurationResultTypeDef,
-    VpcConfigOutputTypeDef,
-    VpcConfigTypeDef,
+    VpcConfigUnionTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -256,15 +253,15 @@
         """
 
     def create_project(
         self,
         *,
         name: str,
         defaultJobTimeoutMinutes: int = ...,
-        vpcConfig: Union[VpcConfigTypeDef, VpcConfigOutputTypeDef] = ...
+        vpcConfig: VpcConfigUnionTypeDef = ...
     ) -> CreateProjectResultTypeDef:
         """
         Creates a project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Client.create_project)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/client/#create_project)
         """
@@ -289,19 +286,15 @@
         Specifies and starts a remote access session.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Client.create_remote_access_session)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/client/#create_remote_access_session)
         """
 
     def create_test_grid_project(
-        self,
-        *,
-        name: str,
-        description: str = ...,
-        vpcConfig: Union[TestGridVpcConfigTypeDef, TestGridVpcConfigOutputTypeDef] = ...
+        self, *, name: str, description: str = ..., vpcConfig: TestGridVpcConfigUnionTypeDef = ...
     ) -> CreateTestGridProjectResultTypeDef:
         """
         Creates a Selenium testing project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Client.create_test_grid_project)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/client/#create_test_grid_project)
         """
@@ -630,15 +623,15 @@
         """
 
     def list_devices(
         self,
         *,
         arn: str = ...,
         nextToken: str = ...,
-        filters: Sequence[Union[DeviceFilterTypeDef, DeviceFilterOutputTypeDef]] = ...
+        filters: Sequence[DeviceFilterUnionTypeDef] = ...
     ) -> ListDevicesResultTypeDef:
         """
         Gets information about unique device types.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Client.list_devices)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/client/#list_devices)
         """
@@ -787,18 +780,18 @@
         """
 
     def list_test_grid_sessions(
         self,
         *,
         projectArn: str,
         status: TestGridSessionStatusType = ...,
-        creationTimeAfter: Union[datetime, str] = ...,
-        creationTimeBefore: Union[datetime, str] = ...,
-        endTimeAfter: Union[datetime, str] = ...,
-        endTimeBefore: Union[datetime, str] = ...,
+        creationTimeAfter: TimestampTypeDef = ...,
+        creationTimeBefore: TimestampTypeDef = ...,
+        endTimeAfter: TimestampTypeDef = ...,
+        endTimeBefore: TimestampTypeDef = ...,
         maxResult: int = ...,
         nextToken: str = ...
     ) -> ListTestGridSessionsResultTypeDef:
         """
         Retrieves a list of sessions for a  TestGridProject.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Client.list_test_grid_sessions)
@@ -992,30 +985,30 @@
 
     def update_project(
         self,
         *,
         arn: str,
         name: str = ...,
         defaultJobTimeoutMinutes: int = ...,
-        vpcConfig: Union[VpcConfigTypeDef, VpcConfigOutputTypeDef] = ...
+        vpcConfig: VpcConfigUnionTypeDef = ...
     ) -> UpdateProjectResultTypeDef:
         """
         Modifies the specified project name, given the project ARN and a new name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Client.update_project)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/client/#update_project)
         """
 
     def update_test_grid_project(
         self,
         *,
         projectArn: str,
         name: str = ...,
         description: str = ...,
-        vpcConfig: Union[TestGridVpcConfigTypeDef, TestGridVpcConfigOutputTypeDef] = ...
+        vpcConfig: TestGridVpcConfigUnionTypeDef = ...
     ) -> UpdateTestGridProjectResultTypeDef:
         """
         Change details of a project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Client.update_test_grid_project)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/client/#update_test_grid_project)
         """
```

### Comparing `mypy-boto3-devicefarm-1.28.15.post1/mypy_boto3_devicefarm/client.pyi` & `mypy-boto3-devicefarm-1.28.16/mypy_boto3_devicefarm/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from mypy_boto3_devicefarm.client import DeviceFarmClient
 
     session = Session()
     client: DeviceFarmClient = session.client("devicefarm")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     ArtifactCategoryType,
     DevicePoolTypeType,
     InteractionModeType,
@@ -58,16 +57,15 @@
     CreateProjectResultTypeDef,
     CreateRemoteAccessSessionConfigurationTypeDef,
     CreateRemoteAccessSessionResultTypeDef,
     CreateTestGridProjectResultTypeDef,
     CreateTestGridUrlResultTypeDef,
     CreateUploadResultTypeDef,
     CreateVPCEConfigurationResultTypeDef,
-    DeviceFilterOutputTypeDef,
-    DeviceFilterTypeDef,
+    DeviceFilterUnionTypeDef,
     DeviceSelectionConfigurationTypeDef,
     ExecutionConfigurationTypeDef,
     GetAccountSettingsResultTypeDef,
     GetDeviceInstanceResultTypeDef,
     GetDevicePoolCompatibilityResultTypeDef,
     GetDevicePoolResultTypeDef,
     GetDeviceResultTypeDef,
@@ -115,26 +113,25 @@
     ScheduleRunConfigurationTypeDef,
     ScheduleRunResultTypeDef,
     ScheduleRunTestTypeDef,
     StopJobResultTypeDef,
     StopRemoteAccessSessionResultTypeDef,
     StopRunResultTypeDef,
     TagTypeDef,
-    TestGridVpcConfigOutputTypeDef,
-    TestGridVpcConfigTypeDef,
+    TestGridVpcConfigUnionTypeDef,
+    TimestampTypeDef,
     UpdateDeviceInstanceResultTypeDef,
     UpdateDevicePoolResultTypeDef,
     UpdateInstanceProfileResultTypeDef,
     UpdateNetworkProfileResultTypeDef,
     UpdateProjectResultTypeDef,
     UpdateTestGridProjectResultTypeDef,
     UpdateUploadResultTypeDef,
     UpdateVPCEConfigurationResultTypeDef,
-    VpcConfigOutputTypeDef,
-    VpcConfigTypeDef,
+    VpcConfigUnionTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -246,15 +243,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/client/#create_network_profile)
         """
     def create_project(
         self,
         *,
         name: str,
         defaultJobTimeoutMinutes: int = ...,
-        vpcConfig: Union[VpcConfigTypeDef, VpcConfigOutputTypeDef] = ...
+        vpcConfig: VpcConfigUnionTypeDef = ...
     ) -> CreateProjectResultTypeDef:
         """
         Creates a project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Client.create_project)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/client/#create_project)
         """
@@ -277,19 +274,15 @@
         """
         Specifies and starts a remote access session.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Client.create_remote_access_session)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/client/#create_remote_access_session)
         """
     def create_test_grid_project(
-        self,
-        *,
-        name: str,
-        description: str = ...,
-        vpcConfig: Union[TestGridVpcConfigTypeDef, TestGridVpcConfigOutputTypeDef] = ...
+        self, *, name: str, description: str = ..., vpcConfig: TestGridVpcConfigUnionTypeDef = ...
     ) -> CreateTestGridProjectResultTypeDef:
         """
         Creates a Selenium testing project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Client.create_test_grid_project)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/client/#create_test_grid_project)
         """
@@ -582,15 +575,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/client/#list_device_pools)
         """
     def list_devices(
         self,
         *,
         arn: str = ...,
         nextToken: str = ...,
-        filters: Sequence[Union[DeviceFilterTypeDef, DeviceFilterOutputTypeDef]] = ...
+        filters: Sequence[DeviceFilterUnionTypeDef] = ...
     ) -> ListDevicesResultTypeDef:
         """
         Gets information about unique device types.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Client.list_devices)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/client/#list_devices)
         """
@@ -723,18 +716,18 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/client/#list_test_grid_session_artifacts)
         """
     def list_test_grid_sessions(
         self,
         *,
         projectArn: str,
         status: TestGridSessionStatusType = ...,
-        creationTimeAfter: Union[datetime, str] = ...,
-        creationTimeBefore: Union[datetime, str] = ...,
-        endTimeAfter: Union[datetime, str] = ...,
-        endTimeBefore: Union[datetime, str] = ...,
+        creationTimeAfter: TimestampTypeDef = ...,
+        creationTimeBefore: TimestampTypeDef = ...,
+        endTimeAfter: TimestampTypeDef = ...,
+        endTimeBefore: TimestampTypeDef = ...,
         maxResult: int = ...,
         nextToken: str = ...
     ) -> ListTestGridSessionsResultTypeDef:
         """
         Retrieves a list of sessions for a  TestGridProject.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Client.list_test_grid_sessions)
@@ -911,29 +904,29 @@
         """
     def update_project(
         self,
         *,
         arn: str,
         name: str = ...,
         defaultJobTimeoutMinutes: int = ...,
-        vpcConfig: Union[VpcConfigTypeDef, VpcConfigOutputTypeDef] = ...
+        vpcConfig: VpcConfigUnionTypeDef = ...
     ) -> UpdateProjectResultTypeDef:
         """
         Modifies the specified project name, given the project ARN and a new name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Client.update_project)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/client/#update_project)
         """
     def update_test_grid_project(
         self,
         *,
         projectArn: str,
         name: str = ...,
         description: str = ...,
-        vpcConfig: Union[TestGridVpcConfigTypeDef, TestGridVpcConfigOutputTypeDef] = ...
+        vpcConfig: TestGridVpcConfigUnionTypeDef = ...
     ) -> UpdateTestGridProjectResultTypeDef:
         """
         Change details of a project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Client.update_test_grid_project)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/client/#update_test_grid_project)
         """
```

### Comparing `mypy-boto3-devicefarm-1.28.15.post1/mypy_boto3_devicefarm/literals.py` & `mypy-boto3-devicefarm-1.28.16/mypy_boto3_devicefarm/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-devicefarm-1.28.15.post1/mypy_boto3_devicefarm/literals.pyi` & `mypy-boto3-devicefarm-1.28.16/mypy_boto3_devicefarm/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-devicefarm-1.28.15.post1/mypy_boto3_devicefarm/paginator.py` & `mypy-boto3-devicefarm-1.28.16/mypy_boto3_devicefarm/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,27 +53,26 @@
     list_suites_paginator: ListSuitesPaginator = client.get_paginator("list_suites")
     list_tests_paginator: ListTestsPaginator = client.get_paginator("list_tests")
     list_unique_problems_paginator: ListUniqueProblemsPaginator = client.get_paginator("list_unique_problems")
     list_uploads_paginator: ListUploadsPaginator = client.get_paginator("list_uploads")
     list_vpce_configurations_paginator: ListVPCEConfigurationsPaginator = client.get_paginator("list_vpce_configurations")
     ```
 """
-from typing import Generic, Iterator, Sequence, TypeVar, Union
+from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import (
     ArtifactCategoryType,
     DevicePoolTypeType,
     NetworkProfileTypeType,
     UploadTypeType,
 )
 from .type_defs import (
-    DeviceFilterOutputTypeDef,
-    DeviceFilterTypeDef,
+    DeviceFilterUnionTypeDef,
     GetOfferingStatusResultTypeDef,
     ListArtifactsResultTypeDef,
     ListDeviceInstancesResultTypeDef,
     ListDevicePoolsResultTypeDef,
     ListDevicesResultTypeDef,
     ListInstanceProfilesResultTypeDef,
     ListJobsResultTypeDef,
@@ -201,15 +200,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listdevicespaginator)
     """
 
     def paginate(
         self,
         *,
         arn: str = ...,
-        filters: Sequence[Union[DeviceFilterTypeDef, DeviceFilterOutputTypeDef]] = ...,
+        filters: Sequence[DeviceFilterUnionTypeDef] = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDevicesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListDevices.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listdevicespaginator)
         """
```

### Comparing `mypy-boto3-devicefarm-1.28.15.post1/mypy_boto3_devicefarm/paginator.pyi` & `mypy-boto3-devicefarm-1.28.16/mypy_boto3_devicefarm/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -53,27 +53,26 @@
     list_suites_paginator: ListSuitesPaginator = client.get_paginator("list_suites")
     list_tests_paginator: ListTestsPaginator = client.get_paginator("list_tests")
     list_unique_problems_paginator: ListUniqueProblemsPaginator = client.get_paginator("list_unique_problems")
     list_uploads_paginator: ListUploadsPaginator = client.get_paginator("list_uploads")
     list_vpce_configurations_paginator: ListVPCEConfigurationsPaginator = client.get_paginator("list_vpce_configurations")
     ```
 """
-from typing import Generic, Iterator, Sequence, TypeVar, Union
+from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import (
     ArtifactCategoryType,
     DevicePoolTypeType,
     NetworkProfileTypeType,
     UploadTypeType,
 )
 from .type_defs import (
-    DeviceFilterOutputTypeDef,
-    DeviceFilterTypeDef,
+    DeviceFilterUnionTypeDef,
     GetOfferingStatusResultTypeDef,
     ListArtifactsResultTypeDef,
     ListDeviceInstancesResultTypeDef,
     ListDevicePoolsResultTypeDef,
     ListDevicesResultTypeDef,
     ListInstanceProfilesResultTypeDef,
     ListJobsResultTypeDef,
@@ -194,15 +193,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listdevicespaginator)
     """
 
     def paginate(
         self,
         *,
         arn: str = ...,
-        filters: Sequence[Union[DeviceFilterTypeDef, DeviceFilterOutputTypeDef]] = ...,
+        filters: Sequence[DeviceFilterUnionTypeDef] = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDevicesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListDevices.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listdevicespaginator)
         """
```

### Comparing `mypy-boto3-devicefarm-1.28.15.post1/mypy_boto3_devicefarm/type_defs.py` & `mypy-boto3-devicefarm-1.28.16/mypy_boto3_devicefarm/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_devicefarm.type_defs import TrialMinutesTypeDef
 
-    data: TrialMinutesTypeDef = {...}
+    data: TrialMinutesTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -128,15 +128,15 @@
     "ListTagsForResourceRequestRequestTypeDef",
     "TagTypeDef",
     "ListTestGridProjectsRequestRequestTypeDef",
     "ListTestGridSessionActionsRequestRequestTypeDef",
     "TestGridSessionActionTypeDef",
     "ListTestGridSessionArtifactsRequestRequestTypeDef",
     "TestGridSessionArtifactTypeDef",
-    "ListTestGridSessionsRequestRequestTypeDef",
+    "TimestampTypeDef",
     "ListTestsRequestRequestTypeDef",
     "ListUniqueProblemsRequestRequestTypeDef",
     "ListUploadsRequestRequestTypeDef",
     "ListVPCEConfigurationsRequestRequestTypeDef",
     "LocationTypeDef",
     "MonetaryAmountTypeDef",
     "ProblemDetailTypeDef",
@@ -180,23 +180,22 @@
     "ListUploadsResultTypeDef",
     "UpdateUploadResultTypeDef",
     "CreateVPCEConfigurationResultTypeDef",
     "GetVPCEConfigurationResultTypeDef",
     "ListVPCEConfigurationsResultTypeDef",
     "UpdateVPCEConfigurationResultTypeDef",
     "DeviceSelectionResultTypeDef",
+    "DeviceFilterUnionTypeDef",
     "DeviceSelectionConfigurationTypeDef",
-    "ListDevicesRequestRequestTypeDef",
     "SuiteTypeDef",
     "TestTypeDef",
     "GetOfferingStatusRequestGetOfferingStatusPaginateTypeDef",
     "ListArtifactsRequestListArtifactsPaginateTypeDef",
     "ListDeviceInstancesRequestListDeviceInstancesPaginateTypeDef",
     "ListDevicePoolsRequestListDevicePoolsPaginateTypeDef",
-    "ListDevicesRequestListDevicesPaginateTypeDef",
     "ListInstanceProfilesRequestListInstanceProfilesPaginateTypeDef",
     "ListJobsRequestListJobsPaginateTypeDef",
     "ListNetworkProfilesRequestListNetworkProfilesPaginateTypeDef",
     "ListOfferingPromotionsRequestListOfferingPromotionsPaginateTypeDef",
     "ListOfferingTransactionsRequestListOfferingTransactionsPaginateTypeDef",
     "ListOfferingsRequestListOfferingsPaginateTypeDef",
     "ListProjectsRequestListProjectsPaginateTypeDef",
@@ -212,28 +211,33 @@
     "ListTestGridSessionsResultTypeDef",
     "ListOfferingPromotionsResultTypeDef",
     "ListSamplesResultTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "ListTestGridSessionActionsResultTypeDef",
     "ListTestGridSessionArtifactsResultTypeDef",
+    "ListTestGridSessionsRequestRequestTypeDef",
     "RecurringChargeTypeDef",
     "ProjectTypeDef",
+    "VpcConfigUnionTypeDef",
     "ScheduleRunConfigurationTypeDef",
     "TestGridProjectTypeDef",
+    "TestGridVpcConfigUnionTypeDef",
     "GetAccountSettingsResultTypeDef",
     "CreateDevicePoolResultTypeDef",
     "GetDevicePoolResultTypeDef",
     "ListDevicePoolsResultTypeDef",
     "UpdateDevicePoolResultTypeDef",
     "DeviceTypeDef",
     "GetDeviceInstanceResultTypeDef",
     "ListDeviceInstancesResultTypeDef",
     "UpdateDeviceInstanceResultTypeDef",
     "RunTypeDef",
+    "ListDevicesRequestListDevicesPaginateTypeDef",
+    "ListDevicesRequestRequestTypeDef",
     "GetSuiteResultTypeDef",
     "ListSuitesResultTypeDef",
     "GetTestResultTypeDef",
     "ListTestsResultTypeDef",
     "OfferingTypeDef",
     "CreateProjectResultTypeDef",
     "GetProjectResultTypeDef",
@@ -1182,42 +1186,15 @@
         "filename": str,
         "type": TestGridSessionArtifactTypeType,
         "url": str,
     },
     total=False,
 )
 
-_RequiredListTestGridSessionsRequestRequestTypeDef = TypedDict(
-    "_RequiredListTestGridSessionsRequestRequestTypeDef",
-    {
-        "projectArn": str,
-    },
-)
-_OptionalListTestGridSessionsRequestRequestTypeDef = TypedDict(
-    "_OptionalListTestGridSessionsRequestRequestTypeDef",
-    {
-        "status": TestGridSessionStatusType,
-        "creationTimeAfter": Union[datetime, str],
-        "creationTimeBefore": Union[datetime, str],
-        "endTimeAfter": Union[datetime, str],
-        "endTimeBefore": Union[datetime, str],
-        "maxResult": int,
-        "nextToken": str,
-    },
-    total=False,
-)
-
-
-class ListTestGridSessionsRequestRequestTypeDef(
-    _RequiredListTestGridSessionsRequestRequestTypeDef,
-    _OptionalListTestGridSessionsRequestRequestTypeDef,
-):
-    pass
-
-
+TimestampTypeDef = Union[datetime, str]
 _RequiredListTestsRequestRequestTypeDef = TypedDict(
     "_RequiredListTestsRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 _OptionalListTestsRequestRequestTypeDef = TypedDict(
@@ -1909,32 +1886,23 @@
         "filters": List[DeviceFilterOutputTypeDef],
         "matchedDevicesCount": int,
         "maxDevices": int,
     },
     total=False,
 )
 
+DeviceFilterUnionTypeDef = Union[DeviceFilterTypeDef, DeviceFilterOutputTypeDef]
 DeviceSelectionConfigurationTypeDef = TypedDict(
     "DeviceSelectionConfigurationTypeDef",
     {
         "filters": Sequence[DeviceFilterTypeDef],
         "maxDevices": int,
     },
 )
 
-ListDevicesRequestRequestTypeDef = TypedDict(
-    "ListDevicesRequestRequestTypeDef",
-    {
-        "arn": str,
-        "nextToken": str,
-        "filters": Sequence[Union[DeviceFilterTypeDef, DeviceFilterOutputTypeDef]],
-    },
-    total=False,
-)
-
 SuiteTypeDef = TypedDict(
     "SuiteTypeDef",
     {
         "arn": str,
         "name": str,
         "type": TestTypeType,
         "created": datetime,
@@ -2025,24 +1993,14 @@
 class ListDevicePoolsRequestListDevicePoolsPaginateTypeDef(
     _RequiredListDevicePoolsRequestListDevicePoolsPaginateTypeDef,
     _OptionalListDevicePoolsRequestListDevicePoolsPaginateTypeDef,
 ):
     pass
 
 
-ListDevicesRequestListDevicesPaginateTypeDef = TypedDict(
-    "ListDevicesRequestListDevicesPaginateTypeDef",
-    {
-        "arn": str,
-        "filters": Sequence[Union[DeviceFilterTypeDef, DeviceFilterOutputTypeDef]],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 ListInstanceProfilesRequestListInstanceProfilesPaginateTypeDef = TypedDict(
     "ListInstanceProfilesRequestListInstanceProfilesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -2351,14 +2309,42 @@
     {
         "artifacts": List[TestGridSessionArtifactTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredListTestGridSessionsRequestRequestTypeDef = TypedDict(
+    "_RequiredListTestGridSessionsRequestRequestTypeDef",
+    {
+        "projectArn": str,
+    },
+)
+_OptionalListTestGridSessionsRequestRequestTypeDef = TypedDict(
+    "_OptionalListTestGridSessionsRequestRequestTypeDef",
+    {
+        "status": TestGridSessionStatusType,
+        "creationTimeAfter": TimestampTypeDef,
+        "creationTimeBefore": TimestampTypeDef,
+        "endTimeAfter": TimestampTypeDef,
+        "endTimeBefore": TimestampTypeDef,
+        "maxResult": int,
+        "nextToken": str,
+    },
+    total=False,
+)
+
+
+class ListTestGridSessionsRequestRequestTypeDef(
+    _RequiredListTestGridSessionsRequestRequestTypeDef,
+    _OptionalListTestGridSessionsRequestRequestTypeDef,
+):
+    pass
+
+
 RecurringChargeTypeDef = TypedDict(
     "RecurringChargeTypeDef",
     {
         "cost": MonetaryAmountTypeDef,
         "frequency": Literal["MONTHLY"],
     },
     total=False,
@@ -2372,14 +2358,15 @@
         "defaultJobTimeoutMinutes": int,
         "created": datetime,
         "vpcConfig": VpcConfigOutputTypeDef,
     },
     total=False,
 )
 
+VpcConfigUnionTypeDef = Union[VpcConfigTypeDef, VpcConfigOutputTypeDef]
 ScheduleRunConfigurationTypeDef = TypedDict(
     "ScheduleRunConfigurationTypeDef",
     {
         "extraDataPackageArn": str,
         "networkProfileArn": str,
         "locale": str,
         "location": LocationTypeDef,
@@ -2400,14 +2387,15 @@
         "description": str,
         "vpcConfig": TestGridVpcConfigOutputTypeDef,
         "created": datetime,
     },
     total=False,
 )
 
+TestGridVpcConfigUnionTypeDef = Union[TestGridVpcConfigTypeDef, TestGridVpcConfigOutputTypeDef]
 GetAccountSettingsResultTypeDef = TypedDict(
     "GetAccountSettingsResultTypeDef",
     {
         "accountSettings": AccountSettingsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2533,14 +2521,34 @@
         "testSpecArn": str,
         "deviceSelectionResult": DeviceSelectionResultTypeDef,
         "vpcConfig": VpcConfigOutputTypeDef,
     },
     total=False,
 )
 
+ListDevicesRequestListDevicesPaginateTypeDef = TypedDict(
+    "ListDevicesRequestListDevicesPaginateTypeDef",
+    {
+        "arn": str,
+        "filters": Sequence[DeviceFilterUnionTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListDevicesRequestRequestTypeDef = TypedDict(
+    "ListDevicesRequestRequestTypeDef",
+    {
+        "arn": str,
+        "nextToken": str,
+        "filters": Sequence[DeviceFilterUnionTypeDef],
+    },
+    total=False,
+)
+
 GetSuiteResultTypeDef = TypedDict(
     "GetSuiteResultTypeDef",
     {
         "suite": SuiteTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-devicefarm-1.28.15.post1/mypy_boto3_devicefarm/type_defs.pyi` & `mypy-boto3-devicefarm-1.28.16/mypy_boto3_devicefarm/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_devicefarm.type_defs import TrialMinutesTypeDef
 
-    data: TrialMinutesTypeDef = {...}
+    data: TrialMinutesTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -127,15 +127,15 @@
     "ListTagsForResourceRequestRequestTypeDef",
     "TagTypeDef",
     "ListTestGridProjectsRequestRequestTypeDef",
     "ListTestGridSessionActionsRequestRequestTypeDef",
     "TestGridSessionActionTypeDef",
     "ListTestGridSessionArtifactsRequestRequestTypeDef",
     "TestGridSessionArtifactTypeDef",
-    "ListTestGridSessionsRequestRequestTypeDef",
+    "TimestampTypeDef",
     "ListTestsRequestRequestTypeDef",
     "ListUniqueProblemsRequestRequestTypeDef",
     "ListUploadsRequestRequestTypeDef",
     "ListVPCEConfigurationsRequestRequestTypeDef",
     "LocationTypeDef",
     "MonetaryAmountTypeDef",
     "ProblemDetailTypeDef",
@@ -179,23 +179,22 @@
     "ListUploadsResultTypeDef",
     "UpdateUploadResultTypeDef",
     "CreateVPCEConfigurationResultTypeDef",
     "GetVPCEConfigurationResultTypeDef",
     "ListVPCEConfigurationsResultTypeDef",
     "UpdateVPCEConfigurationResultTypeDef",
     "DeviceSelectionResultTypeDef",
+    "DeviceFilterUnionTypeDef",
     "DeviceSelectionConfigurationTypeDef",
-    "ListDevicesRequestRequestTypeDef",
     "SuiteTypeDef",
     "TestTypeDef",
     "GetOfferingStatusRequestGetOfferingStatusPaginateTypeDef",
     "ListArtifactsRequestListArtifactsPaginateTypeDef",
     "ListDeviceInstancesRequestListDeviceInstancesPaginateTypeDef",
     "ListDevicePoolsRequestListDevicePoolsPaginateTypeDef",
-    "ListDevicesRequestListDevicesPaginateTypeDef",
     "ListInstanceProfilesRequestListInstanceProfilesPaginateTypeDef",
     "ListJobsRequestListJobsPaginateTypeDef",
     "ListNetworkProfilesRequestListNetworkProfilesPaginateTypeDef",
     "ListOfferingPromotionsRequestListOfferingPromotionsPaginateTypeDef",
     "ListOfferingTransactionsRequestListOfferingTransactionsPaginateTypeDef",
     "ListOfferingsRequestListOfferingsPaginateTypeDef",
     "ListProjectsRequestListProjectsPaginateTypeDef",
@@ -211,28 +210,33 @@
     "ListTestGridSessionsResultTypeDef",
     "ListOfferingPromotionsResultTypeDef",
     "ListSamplesResultTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "ListTestGridSessionActionsResultTypeDef",
     "ListTestGridSessionArtifactsResultTypeDef",
+    "ListTestGridSessionsRequestRequestTypeDef",
     "RecurringChargeTypeDef",
     "ProjectTypeDef",
+    "VpcConfigUnionTypeDef",
     "ScheduleRunConfigurationTypeDef",
     "TestGridProjectTypeDef",
+    "TestGridVpcConfigUnionTypeDef",
     "GetAccountSettingsResultTypeDef",
     "CreateDevicePoolResultTypeDef",
     "GetDevicePoolResultTypeDef",
     "ListDevicePoolsResultTypeDef",
     "UpdateDevicePoolResultTypeDef",
     "DeviceTypeDef",
     "GetDeviceInstanceResultTypeDef",
     "ListDeviceInstancesResultTypeDef",
     "UpdateDeviceInstanceResultTypeDef",
     "RunTypeDef",
+    "ListDevicesRequestListDevicesPaginateTypeDef",
+    "ListDevicesRequestRequestTypeDef",
     "GetSuiteResultTypeDef",
     "ListSuitesResultTypeDef",
     "GetTestResultTypeDef",
     "ListTestsResultTypeDef",
     "OfferingTypeDef",
     "CreateProjectResultTypeDef",
     "GetProjectResultTypeDef",
@@ -1151,40 +1155,15 @@
         "filename": str,
         "type": TestGridSessionArtifactTypeType,
         "url": str,
     },
     total=False,
 )
 
-_RequiredListTestGridSessionsRequestRequestTypeDef = TypedDict(
-    "_RequiredListTestGridSessionsRequestRequestTypeDef",
-    {
-        "projectArn": str,
-    },
-)
-_OptionalListTestGridSessionsRequestRequestTypeDef = TypedDict(
-    "_OptionalListTestGridSessionsRequestRequestTypeDef",
-    {
-        "status": TestGridSessionStatusType,
-        "creationTimeAfter": Union[datetime, str],
-        "creationTimeBefore": Union[datetime, str],
-        "endTimeAfter": Union[datetime, str],
-        "endTimeBefore": Union[datetime, str],
-        "maxResult": int,
-        "nextToken": str,
-    },
-    total=False,
-)
-
-class ListTestGridSessionsRequestRequestTypeDef(
-    _RequiredListTestGridSessionsRequestRequestTypeDef,
-    _OptionalListTestGridSessionsRequestRequestTypeDef,
-):
-    pass
-
+TimestampTypeDef = Union[datetime, str]
 _RequiredListTestsRequestRequestTypeDef = TypedDict(
     "_RequiredListTestsRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 _OptionalListTestsRequestRequestTypeDef = TypedDict(
@@ -1844,32 +1823,23 @@
         "filters": List[DeviceFilterOutputTypeDef],
         "matchedDevicesCount": int,
         "maxDevices": int,
     },
     total=False,
 )
 
+DeviceFilterUnionTypeDef = Union[DeviceFilterTypeDef, DeviceFilterOutputTypeDef]
 DeviceSelectionConfigurationTypeDef = TypedDict(
     "DeviceSelectionConfigurationTypeDef",
     {
         "filters": Sequence[DeviceFilterTypeDef],
         "maxDevices": int,
     },
 )
 
-ListDevicesRequestRequestTypeDef = TypedDict(
-    "ListDevicesRequestRequestTypeDef",
-    {
-        "arn": str,
-        "nextToken": str,
-        "filters": Sequence[Union[DeviceFilterTypeDef, DeviceFilterOutputTypeDef]],
-    },
-    total=False,
-)
-
 SuiteTypeDef = TypedDict(
     "SuiteTypeDef",
     {
         "arn": str,
         "name": str,
         "type": TestTypeType,
         "created": datetime,
@@ -1956,24 +1926,14 @@
 
 class ListDevicePoolsRequestListDevicePoolsPaginateTypeDef(
     _RequiredListDevicePoolsRequestListDevicePoolsPaginateTypeDef,
     _OptionalListDevicePoolsRequestListDevicePoolsPaginateTypeDef,
 ):
     pass
 
-ListDevicesRequestListDevicesPaginateTypeDef = TypedDict(
-    "ListDevicesRequestListDevicesPaginateTypeDef",
-    {
-        "arn": str,
-        "filters": Sequence[Union[DeviceFilterTypeDef, DeviceFilterOutputTypeDef]],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 ListInstanceProfilesRequestListInstanceProfilesPaginateTypeDef = TypedDict(
     "ListInstanceProfilesRequestListInstanceProfilesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -2264,14 +2224,40 @@
     {
         "artifacts": List[TestGridSessionArtifactTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredListTestGridSessionsRequestRequestTypeDef = TypedDict(
+    "_RequiredListTestGridSessionsRequestRequestTypeDef",
+    {
+        "projectArn": str,
+    },
+)
+_OptionalListTestGridSessionsRequestRequestTypeDef = TypedDict(
+    "_OptionalListTestGridSessionsRequestRequestTypeDef",
+    {
+        "status": TestGridSessionStatusType,
+        "creationTimeAfter": TimestampTypeDef,
+        "creationTimeBefore": TimestampTypeDef,
+        "endTimeAfter": TimestampTypeDef,
+        "endTimeBefore": TimestampTypeDef,
+        "maxResult": int,
+        "nextToken": str,
+    },
+    total=False,
+)
+
+class ListTestGridSessionsRequestRequestTypeDef(
+    _RequiredListTestGridSessionsRequestRequestTypeDef,
+    _OptionalListTestGridSessionsRequestRequestTypeDef,
+):
+    pass
+
 RecurringChargeTypeDef = TypedDict(
     "RecurringChargeTypeDef",
     {
         "cost": MonetaryAmountTypeDef,
         "frequency": Literal["MONTHLY"],
     },
     total=False,
@@ -2285,14 +2271,15 @@
         "defaultJobTimeoutMinutes": int,
         "created": datetime,
         "vpcConfig": VpcConfigOutputTypeDef,
     },
     total=False,
 )
 
+VpcConfigUnionTypeDef = Union[VpcConfigTypeDef, VpcConfigOutputTypeDef]
 ScheduleRunConfigurationTypeDef = TypedDict(
     "ScheduleRunConfigurationTypeDef",
     {
         "extraDataPackageArn": str,
         "networkProfileArn": str,
         "locale": str,
         "location": LocationTypeDef,
@@ -2313,14 +2300,15 @@
         "description": str,
         "vpcConfig": TestGridVpcConfigOutputTypeDef,
         "created": datetime,
     },
     total=False,
 )
 
+TestGridVpcConfigUnionTypeDef = Union[TestGridVpcConfigTypeDef, TestGridVpcConfigOutputTypeDef]
 GetAccountSettingsResultTypeDef = TypedDict(
     "GetAccountSettingsResultTypeDef",
     {
         "accountSettings": AccountSettingsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2446,14 +2434,34 @@
         "testSpecArn": str,
         "deviceSelectionResult": DeviceSelectionResultTypeDef,
         "vpcConfig": VpcConfigOutputTypeDef,
     },
     total=False,
 )
 
+ListDevicesRequestListDevicesPaginateTypeDef = TypedDict(
+    "ListDevicesRequestListDevicesPaginateTypeDef",
+    {
+        "arn": str,
+        "filters": Sequence[DeviceFilterUnionTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListDevicesRequestRequestTypeDef = TypedDict(
+    "ListDevicesRequestRequestTypeDef",
+    {
+        "arn": str,
+        "nextToken": str,
+        "filters": Sequence[DeviceFilterUnionTypeDef],
+    },
+    total=False,
+)
+
 GetSuiteResultTypeDef = TypedDict(
     "GetSuiteResultTypeDef",
     {
         "suite": SuiteTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-devicefarm-1.28.15.post1/mypy_boto3_devicefarm.egg-info/PKG-INFO` & `mypy-boto3-devicefarm-1.28.16/mypy_boto3_devicefarm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-devicefarm
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.DeviceFarm 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.DeviceFarm 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 devicefarm type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 devicefarm type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-devicefarm.svg?color=blue)](https://pypi.org/project/mypy-boto3-devicefarm)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-devicefarm)](https://pepy.tech/project/mypy-boto3-devicefarm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DeviceFarm 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm)
+[boto3.DeviceFarm 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm)
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
 [mypy-boto3-devicefarm docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/).
 
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
@@ -414,20 +414,20 @@
 )
 
 
 def check_value(value: ArtifactCategoryType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_devicefarm.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_devicefarm.type_defs import (
     TrialMinutesTypeDef,
     ArtifactTypeDef,
     CPUTypeDef,
     CountersTypeDef,
@@ -501,15 +501,15 @@
     ListTagsForResourceRequestRequestTypeDef,
     TagTypeDef,
     ListTestGridProjectsRequestRequestTypeDef,
     ListTestGridSessionActionsRequestRequestTypeDef,
     TestGridSessionActionTypeDef,
     ListTestGridSessionArtifactsRequestRequestTypeDef,
     TestGridSessionArtifactTypeDef,
-    ListTestGridSessionsRequestRequestTypeDef,
+    TimestampTypeDef,
     ListTestsRequestRequestTypeDef,
     ListUniqueProblemsRequestRequestTypeDef,
     ListUploadsRequestRequestTypeDef,
     ListVPCEConfigurationsRequestRequestTypeDef,
     LocationTypeDef,
     MonetaryAmountTypeDef,
     ProblemDetailTypeDef,
@@ -553,23 +553,22 @@
     ListUploadsResultTypeDef,
     UpdateUploadResultTypeDef,
     CreateVPCEConfigurationResultTypeDef,
     GetVPCEConfigurationResultTypeDef,
     ListVPCEConfigurationsResultTypeDef,
     UpdateVPCEConfigurationResultTypeDef,
     DeviceSelectionResultTypeDef,
+    DeviceFilterUnionTypeDef,
     DeviceSelectionConfigurationTypeDef,
-    ListDevicesRequestRequestTypeDef,
     SuiteTypeDef,
     TestTypeDef,
     GetOfferingStatusRequestGetOfferingStatusPaginateTypeDef,
     ListArtifactsRequestListArtifactsPaginateTypeDef,
     ListDeviceInstancesRequestListDeviceInstancesPaginateTypeDef,
     ListDevicePoolsRequestListDevicePoolsPaginateTypeDef,
-    ListDevicesRequestListDevicesPaginateTypeDef,
     ListInstanceProfilesRequestListInstanceProfilesPaginateTypeDef,
     ListJobsRequestListJobsPaginateTypeDef,
     ListNetworkProfilesRequestListNetworkProfilesPaginateTypeDef,
     ListOfferingPromotionsRequestListOfferingPromotionsPaginateTypeDef,
     ListOfferingTransactionsRequestListOfferingTransactionsPaginateTypeDef,
     ListOfferingsRequestListOfferingsPaginateTypeDef,
     ListProjectsRequestListProjectsPaginateTypeDef,
@@ -585,28 +584,33 @@
     ListTestGridSessionsResultTypeDef,
     ListOfferingPromotionsResultTypeDef,
     ListSamplesResultTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     ListTestGridSessionActionsResultTypeDef,
     ListTestGridSessionArtifactsResultTypeDef,
+    ListTestGridSessionsRequestRequestTypeDef,
     RecurringChargeTypeDef,
     ProjectTypeDef,
+    VpcConfigUnionTypeDef,
     ScheduleRunConfigurationTypeDef,
     TestGridProjectTypeDef,
+    TestGridVpcConfigUnionTypeDef,
     GetAccountSettingsResultTypeDef,
     CreateDevicePoolResultTypeDef,
     GetDevicePoolResultTypeDef,
     ListDevicePoolsResultTypeDef,
     UpdateDevicePoolResultTypeDef,
     DeviceTypeDef,
     GetDeviceInstanceResultTypeDef,
     ListDeviceInstancesResultTypeDef,
     UpdateDeviceInstanceResultTypeDef,
     RunTypeDef,
+    ListDevicesRequestListDevicesPaginateTypeDef,
+    ListDevicesRequestRequestTypeDef,
     GetSuiteResultTypeDef,
     ListSuitesResultTypeDef,
     GetTestResultTypeDef,
     ListTestsResultTypeDef,
     OfferingTypeDef,
     CreateProjectResultTypeDef,
     GetProjectResultTypeDef,
@@ -644,15 +648,15 @@
     ListUniqueProblemsResultTypeDef,
     ListOfferingTransactionsResultTypeDef,
     PurchaseOfferingResultTypeDef,
     RenewOfferingResultTypeDef,
 )
 
 
-def get_structure() -> TrialMinutesTypeDef:
+def get_value() -> TrialMinutesTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-devicefarm-1.28.15.post1/mypy_boto3_devicefarm.egg-info/SOURCES.txt` & `mypy-boto3-devicefarm-1.28.16/mypy_boto3_devicefarm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-devicefarm-1.28.15.post1/setup.py` & `mypy-boto3-devicefarm-1.28.16/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-devicefarm",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_devicefarm"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.DeviceFarm 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.2"
+        "Type annotations for boto3.DeviceFarm 1.28.16 service generated with mypy-boto3-builder"
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
-    keywords="boto3 devicefarm type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 devicefarm type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_devicefarm": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

