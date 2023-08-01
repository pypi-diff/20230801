# Comparing `tmp/mypy-boto3-emr-serverless-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-emr-serverless-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-emr-serverless-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:06 2023, max compression
+gzip compressed data, was "mypy-boto3-emr-serverless-1.28.16.tar", last modified: Tue Aug  1 11:36:45 2023, max compression
```

## Comparing `mypy-boto3-emr-serverless-1.28.15.post1.tar` & `mypy-boto3-emr-serverless-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:06.157143 mypy-boto3-emr-serverless-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:45:03.000000 mypy-boto3-emr-serverless-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15272 2023-07-29 10:03:06.149143 mypy-boto3-emr-serverless-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13752 2023-07-29 09:45:03.000000 mypy-boto3-emr-serverless-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:06.141143 mypy-boto3-emr-serverless-1.28.15.post1/mypy_boto3_emr_serverless/
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-29 09:45:03.000000 mypy-boto3-emr-serverless-1.28.15.post1/mypy_boto3_emr_serverless/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-29 09:45:03.000000 mypy-boto3-emr-serverless-1.28.15.post1/mypy_boto3_emr_serverless/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-29 09:45:03.000000 mypy-boto3-emr-serverless-1.28.15.post1/mypy_boto3_emr_serverless/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14559 2023-07-29 09:45:03.000000 mypy-boto3-emr-serverless-1.28.15.post1/mypy_boto3_emr_serverless/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    14535 2023-07-29 09:45:03.000000 mypy-boto3-emr-serverless-1.28.15.post1/mypy_boto3_emr_serverless/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8650 2023-07-29 09:45:03.000000 mypy-boto3-emr-serverless-1.28.15.post1/mypy_boto3_emr_serverless/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8648 2023-07-29 09:45:03.000000 mypy-boto3-emr-serverless-1.28.15.post1/mypy_boto3_emr_serverless/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-07-29 09:45:03.000000 mypy-boto3-emr-serverless-1.28.15.post1/mypy_boto3_emr_serverless/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-07-29 09:45:03.000000 mypy-boto3-emr-serverless-1.28.15.post1/mypy_boto3_emr_serverless/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:45:03.000000 mypy-boto3-emr-serverless-1.28.15.post1/mypy_boto3_emr_serverless/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    23608 2023-07-29 09:45:04.000000 mypy-boto3-emr-serverless-1.28.15.post1/mypy_boto3_emr_serverless/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    23567 2023-07-29 09:45:03.000000 mypy-boto3-emr-serverless-1.28.15.post1/mypy_boto3_emr_serverless/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:45:03.000000 mypy-boto3-emr-serverless-1.28.15.post1/mypy_boto3_emr_serverless/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:06.149143 mypy-boto3-emr-serverless-1.28.15.post1/mypy_boto3_emr_serverless.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15272 2023-07-29 10:03:05.000000 mypy-boto3-emr-serverless-1.28.15.post1/mypy_boto3_emr_serverless.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-29 10:03:05.000000 mypy-boto3-emr-serverless-1.28.15.post1/mypy_boto3_emr_serverless.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:05.000000 mypy-boto3-emr-serverless-1.28.15.post1/mypy_boto3_emr_serverless.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:05.000000 mypy-boto3-emr-serverless-1.28.15.post1/mypy_boto3_emr_serverless.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:05.000000 mypy-boto3-emr-serverless-1.28.15.post1/mypy_boto3_emr_serverless.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-29 10:03:05.000000 mypy-boto3-emr-serverless-1.28.15.post1/mypy_boto3_emr_serverless.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:06.157143 mypy-boto3-emr-serverless-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-29 09:45:02.000000 mypy-boto3-emr-serverless-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:45.900894 mypy-boto3-emr-serverless-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:17:39.000000 mypy-boto3-emr-serverless-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15389 2023-08-01 11:36:45.896894 mypy-boto3-emr-serverless-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13878 2023-08-01 11:17:39.000000 mypy-boto3-emr-serverless-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:45.892894 mypy-boto3-emr-serverless-1.28.16/mypy_boto3_emr_serverless/
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-08-01 11:17:39.000000 mypy-boto3-emr-serverless-1.28.16/mypy_boto3_emr_serverless/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-08-01 11:17:39.000000 mypy-boto3-emr-serverless-1.28.16/mypy_boto3_emr_serverless/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-08-01 11:17:39.000000 mypy-boto3-emr-serverless-1.28.16/mypy_boto3_emr_serverless/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14238 2023-08-01 11:17:39.000000 mypy-boto3-emr-serverless-1.28.16/mypy_boto3_emr_serverless/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14214 2023-08-01 11:17:39.000000 mypy-boto3-emr-serverless-1.28.16/mypy_boto3_emr_serverless/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8650 2023-08-01 11:17:39.000000 mypy-boto3-emr-serverless-1.28.16/mypy_boto3_emr_serverless/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8648 2023-08-01 11:17:39.000000 mypy-boto3-emr-serverless-1.28.16/mypy_boto3_emr_serverless/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-08-01 11:17:39.000000 mypy-boto3-emr-serverless-1.28.16/mypy_boto3_emr_serverless/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-08-01 11:17:39.000000 mypy-boto3-emr-serverless-1.28.16/mypy_boto3_emr_serverless/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:17:39.000000 mypy-boto3-emr-serverless-1.28.16/mypy_boto3_emr_serverless/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    24065 2023-08-01 11:17:40.000000 mypy-boto3-emr-serverless-1.28.16/mypy_boto3_emr_serverless/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24024 2023-08-01 11:17:40.000000 mypy-boto3-emr-serverless-1.28.16/mypy_boto3_emr_serverless/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:17:39.000000 mypy-boto3-emr-serverless-1.28.16/mypy_boto3_emr_serverless/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:45.896894 mypy-boto3-emr-serverless-1.28.16/mypy_boto3_emr_serverless.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15389 2023-08-01 11:36:45.000000 mypy-boto3-emr-serverless-1.28.16/mypy_boto3_emr_serverless.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-08-01 11:36:45.000000 mypy-boto3-emr-serverless-1.28.16/mypy_boto3_emr_serverless.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:45.000000 mypy-boto3-emr-serverless-1.28.16/mypy_boto3_emr_serverless.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:45.000000 mypy-boto3-emr-serverless-1.28.16/mypy_boto3_emr_serverless.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:45.000000 mypy-boto3-emr-serverless-1.28.16/mypy_boto3_emr_serverless.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-01 11:36:45.000000 mypy-boto3-emr-serverless-1.28.16/mypy_boto3_emr_serverless.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:45.900894 mypy-boto3-emr-serverless-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-08-01 11:17:39.000000 mypy-boto3-emr-serverless-1.28.16/setup.py
```

### Comparing `mypy-boto3-emr-serverless-1.28.15.post1/LICENSE` & `mypy-boto3-emr-serverless-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-serverless-1.28.15.post1/PKG-INFO` & `mypy-boto3-emr-serverless-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-emr-serverless
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.EMRServerless 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.EMRServerless 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 emr-serverless type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 emr-serverless type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-emr-serverless.svg?color=blue)](https://pypi.org/project/mypy-boto3-emr-serverless)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-emr-serverless)](https://pepy.tech/project/mypy-boto3-emr-serverless)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EMRServerless 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless)
+[boto3.EMRServerless 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless)
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
 [mypy-boto3-emr-serverless docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/).
 
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
@@ -316,20 +316,20 @@
 )
 
 
 def check_value(value: ApplicationStateType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_emr_serverless.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_emr_serverless.type_defs import (
     ApplicationSummaryTypeDef,
     AutoStartConfigTypeDef,
     AutoStopConfigTypeDef,
     ImageConfigurationTypeDef,
@@ -352,15 +352,15 @@
     SparkSubmitOutputTypeDef,
     SparkSubmitTypeDef,
     JobRunSummaryTypeDef,
     ResourceUtilizationTypeDef,
     TotalResourceUtilizationTypeDef,
     PaginatorConfigTypeDef,
     ListApplicationsRequestRequestTypeDef,
-    ListJobRunsRequestRequestTypeDef,
+    TimestampTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ManagedPersistenceMonitoringConfigurationTypeDef,
     S3MonitoringConfigurationTypeDef,
     StartApplicationRequestRequestTypeDef,
     StopApplicationRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
@@ -368,36 +368,40 @@
     CancelJobRunResponseTypeDef,
     CreateApplicationResponseTypeDef,
     GetDashboardForJobRunResponseTypeDef,
     ListApplicationsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     StartJobRunResponseTypeDef,
     WorkerTypeSpecificationInputTypeDef,
+    NetworkConfigurationUnionTypeDef,
     InitialCapacityConfigTypeDef,
     JobDriverOutputTypeDef,
     JobDriverTypeDef,
     ListJobRunsResponseTypeDef,
     ListApplicationsRequestListApplicationsPaginateTypeDef,
     ListJobRunsRequestListJobRunsPaginateTypeDef,
+    ListJobRunsRequestRequestTypeDef,
     MonitoringConfigurationOutputTypeDef,
     MonitoringConfigurationTypeDef,
     ApplicationTypeDef,
     CreateApplicationRequestRequestTypeDef,
     UpdateApplicationRequestRequestTypeDef,
+    JobDriverUnionTypeDef,
     ConfigurationOverridesOutputTypeDef,
     ConfigurationOverridesTypeDef,
     GetApplicationResponseTypeDef,
     UpdateApplicationResponseTypeDef,
     JobRunTypeDef,
+    ConfigurationOverridesUnionTypeDef,
     StartJobRunRequestRequestTypeDef,
     GetJobRunResponseTypeDef,
 )
 
 
-def get_structure() -> ApplicationSummaryTypeDef:
+def get_value() -> ApplicationSummaryTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-emr-serverless-1.28.15.post1/README.md` & `mypy-boto3-emr-serverless-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-emr-serverless.svg?color=blue)](https://pypi.org/project/mypy-boto3-emr-serverless)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-emr-serverless)](https://pepy.tech/project/mypy-boto3-emr-serverless)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EMRServerless 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless)
+[boto3.EMRServerless 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless)
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
 [mypy-boto3-emr-serverless docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/).
 
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
@@ -284,20 +284,20 @@
 )
 
 
 def check_value(value: ApplicationStateType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_emr_serverless.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_emr_serverless.type_defs import (
     ApplicationSummaryTypeDef,
     AutoStartConfigTypeDef,
     AutoStopConfigTypeDef,
     ImageConfigurationTypeDef,
@@ -320,15 +320,15 @@
     SparkSubmitOutputTypeDef,
     SparkSubmitTypeDef,
     JobRunSummaryTypeDef,
     ResourceUtilizationTypeDef,
     TotalResourceUtilizationTypeDef,
     PaginatorConfigTypeDef,
     ListApplicationsRequestRequestTypeDef,
-    ListJobRunsRequestRequestTypeDef,
+    TimestampTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ManagedPersistenceMonitoringConfigurationTypeDef,
     S3MonitoringConfigurationTypeDef,
     StartApplicationRequestRequestTypeDef,
     StopApplicationRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
@@ -336,36 +336,40 @@
     CancelJobRunResponseTypeDef,
     CreateApplicationResponseTypeDef,
     GetDashboardForJobRunResponseTypeDef,
     ListApplicationsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     StartJobRunResponseTypeDef,
     WorkerTypeSpecificationInputTypeDef,
+    NetworkConfigurationUnionTypeDef,
     InitialCapacityConfigTypeDef,
     JobDriverOutputTypeDef,
     JobDriverTypeDef,
     ListJobRunsResponseTypeDef,
     ListApplicationsRequestListApplicationsPaginateTypeDef,
     ListJobRunsRequestListJobRunsPaginateTypeDef,
+    ListJobRunsRequestRequestTypeDef,
     MonitoringConfigurationOutputTypeDef,
     MonitoringConfigurationTypeDef,
     ApplicationTypeDef,
     CreateApplicationRequestRequestTypeDef,
     UpdateApplicationRequestRequestTypeDef,
+    JobDriverUnionTypeDef,
     ConfigurationOverridesOutputTypeDef,
     ConfigurationOverridesTypeDef,
     GetApplicationResponseTypeDef,
     UpdateApplicationResponseTypeDef,
     JobRunTypeDef,
+    ConfigurationOverridesUnionTypeDef,
     StartJobRunRequestRequestTypeDef,
     GetJobRunResponseTypeDef,
 )
 
 
-def get_structure() -> ApplicationSummaryTypeDef:
+def get_value() -> ApplicationSummaryTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-emr-serverless-1.28.15.post1/mypy_boto3_emr_serverless/__init__.py` & `mypy-boto3-emr-serverless-1.28.16/mypy_boto3_emr_serverless/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-serverless-1.28.15.post1/mypy_boto3_emr_serverless/__init__.pyi` & `mypy-boto3-emr-serverless-1.28.16/mypy_boto3_emr_serverless/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-serverless-1.28.15.post1/mypy_boto3_emr_serverless/__main__.py` & `mypy-boto3-emr-serverless-1.28.16/mypy_boto3_emr_serverless/__main__.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.EMRServerless 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.EMRServerless 1.28.16\nVersion:         1.28.16\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless\nOther"
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

### Comparing `mypy-boto3-emr-serverless-1.28.15.post1/mypy_boto3_emr_serverless/client.py` & `mypy-boto3-emr-serverless-1.28.16/mypy_boto3_emr_serverless/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -10,72 +10,65 @@
     from mypy_boto3_emr_serverless.client import EMRServerlessClient
 
     session = Session()
     client: EMRServerlessClient = session.client("emr-serverless")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import ApplicationStateType, ArchitectureType, JobRunStateType
 from .paginator import ListApplicationsPaginator, ListJobRunsPaginator
 from .type_defs import (
     AutoStartConfigTypeDef,
     AutoStopConfigTypeDef,
     CancelJobRunResponseTypeDef,
-    ConfigurationOverridesOutputTypeDef,
-    ConfigurationOverridesTypeDef,
+    ConfigurationOverridesUnionTypeDef,
     CreateApplicationResponseTypeDef,
     GetApplicationResponseTypeDef,
     GetDashboardForJobRunResponseTypeDef,
     GetJobRunResponseTypeDef,
     ImageConfigurationInputTypeDef,
     InitialCapacityConfigTypeDef,
-    JobDriverOutputTypeDef,
-    JobDriverTypeDef,
+    JobDriverUnionTypeDef,
     ListApplicationsResponseTypeDef,
     ListJobRunsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     MaximumAllowedResourcesTypeDef,
-    NetworkConfigurationOutputTypeDef,
-    NetworkConfigurationTypeDef,
+    NetworkConfigurationUnionTypeDef,
     StartJobRunResponseTypeDef,
+    TimestampTypeDef,
     UpdateApplicationResponseTypeDef,
     WorkerTypeSpecificationInputTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("EMRServerlessClient",)
 
-
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ServiceQuotaExceededException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
-
 class EMRServerlessClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/client/)
     """
 
     meta: ClientMeta
@@ -84,238 +77,212 @@
     def exceptions(self) -> Exceptions:
         """
         EMRServerlessClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/client/#exceptions)
         """
-
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/client/#can_paginate)
         """
-
     def cancel_job_run(self, *, applicationId: str, jobRunId: str) -> CancelJobRunResponseTypeDef:
         """
         Cancels a job run.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Client.cancel_job_run)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/client/#cancel_job_run)
         """
-
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/client/#close)
         """
-
     def create_application(
         self,
         *,
         releaseLabel: str,
         type: str,
         clientToken: str,
         name: str = ...,
         initialCapacity: Mapping[str, InitialCapacityConfigTypeDef] = ...,
         maximumCapacity: MaximumAllowedResourcesTypeDef = ...,
         tags: Mapping[str, str] = ...,
         autoStartConfiguration: AutoStartConfigTypeDef = ...,
         autoStopConfiguration: AutoStopConfigTypeDef = ...,
-        networkConfiguration: Union[
-            NetworkConfigurationTypeDef, NetworkConfigurationOutputTypeDef
-        ] = ...,
+        networkConfiguration: NetworkConfigurationUnionTypeDef = ...,
         architecture: ArchitectureType = ...,
         imageConfiguration: ImageConfigurationInputTypeDef = ...,
         workerTypeSpecifications: Mapping[str, WorkerTypeSpecificationInputTypeDef] = ...
     ) -> CreateApplicationResponseTypeDef:
         """
         Creates an application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Client.create_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/client/#create_application)
         """
-
     def delete_application(self, *, applicationId: str) -> Dict[str, Any]:
         """
         Deletes an application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Client.delete_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/client/#delete_application)
         """
-
     def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/client/#generate_presigned_url)
         """
-
     def get_application(self, *, applicationId: str) -> GetApplicationResponseTypeDef:
         """
         Displays detailed information about a specified application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Client.get_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/client/#get_application)
         """
-
     def get_dashboard_for_job_run(
         self, *, applicationId: str, jobRunId: str
     ) -> GetDashboardForJobRunResponseTypeDef:
         """
         Creates and returns a URL that you can use to access the application UIs for a
         job run.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Client.get_dashboard_for_job_run)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/client/#get_dashboard_for_job_run)
         """
-
     def get_job_run(self, *, applicationId: str, jobRunId: str) -> GetJobRunResponseTypeDef:
         """
         Displays detailed information about a job run.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Client.get_job_run)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/client/#get_job_run)
         """
-
     def list_applications(
         self,
         *,
         nextToken: str = ...,
         maxResults: int = ...,
         states: Sequence[ApplicationStateType] = ...
     ) -> ListApplicationsResponseTypeDef:
         """
         Lists applications based on a set of parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Client.list_applications)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/client/#list_applications)
         """
-
     def list_job_runs(
         self,
         *,
         applicationId: str,
         nextToken: str = ...,
         maxResults: int = ...,
-        createdAtAfter: Union[datetime, str] = ...,
-        createdAtBefore: Union[datetime, str] = ...,
+        createdAtAfter: TimestampTypeDef = ...,
+        createdAtBefore: TimestampTypeDef = ...,
         states: Sequence[JobRunStateType] = ...
     ) -> ListJobRunsResponseTypeDef:
         """
         Lists job runs based on a set of parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Client.list_job_runs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/client/#list_job_runs)
         """
-
     def list_tags_for_resource(self, *, resourceArn: str) -> ListTagsForResourceResponseTypeDef:
         """
         Lists the tags assigned to the resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/client/#list_tags_for_resource)
         """
-
     def start_application(self, *, applicationId: str) -> Dict[str, Any]:
         """
         Starts a specified application and initializes initial capacity if configured.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Client.start_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/client/#start_application)
         """
-
     def start_job_run(
         self,
         *,
         applicationId: str,
         clientToken: str,
         executionRoleArn: str,
-        jobDriver: Union[JobDriverTypeDef, JobDriverOutputTypeDef] = ...,
-        configurationOverrides: Union[
-            ConfigurationOverridesTypeDef, ConfigurationOverridesOutputTypeDef
-        ] = ...,
+        jobDriver: JobDriverUnionTypeDef = ...,
+        configurationOverrides: ConfigurationOverridesUnionTypeDef = ...,
         tags: Mapping[str, str] = ...,
         executionTimeoutMinutes: int = ...,
         name: str = ...
     ) -> StartJobRunResponseTypeDef:
         """
         Starts a job run.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Client.start_job_run)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/client/#start_job_run)
         """
-
     def stop_application(self, *, applicationId: str) -> Dict[str, Any]:
         """
         Stops a specified application and releases initial capacity if configured.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Client.stop_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/client/#stop_application)
         """
-
     def tag_resource(self, *, resourceArn: str, tags: Mapping[str, str]) -> Dict[str, Any]:
         """
         Assigns tags to resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/client/#tag_resource)
         """
-
     def untag_resource(self, *, resourceArn: str, tagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Removes tags from resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/client/#untag_resource)
         """
-
     def update_application(
         self,
         *,
         applicationId: str,
         clientToken: str,
         initialCapacity: Mapping[str, InitialCapacityConfigTypeDef] = ...,
         maximumCapacity: MaximumAllowedResourcesTypeDef = ...,
         autoStartConfiguration: AutoStartConfigTypeDef = ...,
         autoStopConfiguration: AutoStopConfigTypeDef = ...,
-        networkConfiguration: Union[
-            NetworkConfigurationTypeDef, NetworkConfigurationOutputTypeDef
-        ] = ...,
+        networkConfiguration: NetworkConfigurationUnionTypeDef = ...,
         architecture: ArchitectureType = ...,
         imageConfiguration: ImageConfigurationInputTypeDef = ...,
         workerTypeSpecifications: Mapping[str, WorkerTypeSpecificationInputTypeDef] = ...,
         releaseLabel: str = ...
     ) -> UpdateApplicationResponseTypeDef:
         """
         Updates a specified application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Client.update_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/client/#update_application)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_applications"]
     ) -> ListApplicationsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["list_job_runs"]) -> ListJobRunsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/client/#get_paginator)
         """
```

### Comparing `mypy-boto3-emr-serverless-1.28.15.post1/mypy_boto3_emr_serverless/client.pyi` & `mypy-boto3-emr-serverless-1.28.16/mypy_boto3_emr_serverless/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,68 +10,69 @@
     from mypy_boto3_emr_serverless.client import EMRServerlessClient
 
     session = Session()
     client: EMRServerlessClient = session.client("emr-serverless")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import ApplicationStateType, ArchitectureType, JobRunStateType
 from .paginator import ListApplicationsPaginator, ListJobRunsPaginator
 from .type_defs import (
     AutoStartConfigTypeDef,
     AutoStopConfigTypeDef,
     CancelJobRunResponseTypeDef,
-    ConfigurationOverridesOutputTypeDef,
-    ConfigurationOverridesTypeDef,
+    ConfigurationOverridesUnionTypeDef,
     CreateApplicationResponseTypeDef,
     GetApplicationResponseTypeDef,
     GetDashboardForJobRunResponseTypeDef,
     GetJobRunResponseTypeDef,
     ImageConfigurationInputTypeDef,
     InitialCapacityConfigTypeDef,
-    JobDriverOutputTypeDef,
-    JobDriverTypeDef,
+    JobDriverUnionTypeDef,
     ListApplicationsResponseTypeDef,
     ListJobRunsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     MaximumAllowedResourcesTypeDef,
-    NetworkConfigurationOutputTypeDef,
-    NetworkConfigurationTypeDef,
+    NetworkConfigurationUnionTypeDef,
     StartJobRunResponseTypeDef,
+    TimestampTypeDef,
     UpdateApplicationResponseTypeDef,
     WorkerTypeSpecificationInputTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = ("EMRServerlessClient",)
 
+
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ServiceQuotaExceededException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
+
 class EMRServerlessClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/client/)
     """
 
     meta: ClientMeta
@@ -80,218 +81,232 @@
     def exceptions(self) -> Exceptions:
         """
         EMRServerlessClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/client/#exceptions)
         """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/client/#can_paginate)
         """
+
     def cancel_job_run(self, *, applicationId: str, jobRunId: str) -> CancelJobRunResponseTypeDef:
         """
         Cancels a job run.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Client.cancel_job_run)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/client/#cancel_job_run)
         """
+
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/client/#close)
         """
+
     def create_application(
         self,
         *,
         releaseLabel: str,
         type: str,
         clientToken: str,
         name: str = ...,
         initialCapacity: Mapping[str, InitialCapacityConfigTypeDef] = ...,
         maximumCapacity: MaximumAllowedResourcesTypeDef = ...,
         tags: Mapping[str, str] = ...,
         autoStartConfiguration: AutoStartConfigTypeDef = ...,
         autoStopConfiguration: AutoStopConfigTypeDef = ...,
-        networkConfiguration: Union[
-            NetworkConfigurationTypeDef, NetworkConfigurationOutputTypeDef
-        ] = ...,
+        networkConfiguration: NetworkConfigurationUnionTypeDef = ...,
         architecture: ArchitectureType = ...,
         imageConfiguration: ImageConfigurationInputTypeDef = ...,
         workerTypeSpecifications: Mapping[str, WorkerTypeSpecificationInputTypeDef] = ...
     ) -> CreateApplicationResponseTypeDef:
         """
         Creates an application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Client.create_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/client/#create_application)
         """
+
     def delete_application(self, *, applicationId: str) -> Dict[str, Any]:
         """
         Deletes an application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Client.delete_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/client/#delete_application)
         """
+
     def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/client/#generate_presigned_url)
         """
+
     def get_application(self, *, applicationId: str) -> GetApplicationResponseTypeDef:
         """
         Displays detailed information about a specified application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Client.get_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/client/#get_application)
         """
+
     def get_dashboard_for_job_run(
         self, *, applicationId: str, jobRunId: str
     ) -> GetDashboardForJobRunResponseTypeDef:
         """
         Creates and returns a URL that you can use to access the application UIs for a
         job run.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Client.get_dashboard_for_job_run)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/client/#get_dashboard_for_job_run)
         """
+
     def get_job_run(self, *, applicationId: str, jobRunId: str) -> GetJobRunResponseTypeDef:
         """
         Displays detailed information about a job run.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Client.get_job_run)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/client/#get_job_run)
         """
+
     def list_applications(
         self,
         *,
         nextToken: str = ...,
         maxResults: int = ...,
         states: Sequence[ApplicationStateType] = ...
     ) -> ListApplicationsResponseTypeDef:
         """
         Lists applications based on a set of parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Client.list_applications)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/client/#list_applications)
         """
+
     def list_job_runs(
         self,
         *,
         applicationId: str,
         nextToken: str = ...,
         maxResults: int = ...,
-        createdAtAfter: Union[datetime, str] = ...,
-        createdAtBefore: Union[datetime, str] = ...,
+        createdAtAfter: TimestampTypeDef = ...,
+        createdAtBefore: TimestampTypeDef = ...,
         states: Sequence[JobRunStateType] = ...
     ) -> ListJobRunsResponseTypeDef:
         """
         Lists job runs based on a set of parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Client.list_job_runs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/client/#list_job_runs)
         """
+
     def list_tags_for_resource(self, *, resourceArn: str) -> ListTagsForResourceResponseTypeDef:
         """
         Lists the tags assigned to the resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/client/#list_tags_for_resource)
         """
+
     def start_application(self, *, applicationId: str) -> Dict[str, Any]:
         """
         Starts a specified application and initializes initial capacity if configured.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Client.start_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/client/#start_application)
         """
+
     def start_job_run(
         self,
         *,
         applicationId: str,
         clientToken: str,
         executionRoleArn: str,
-        jobDriver: Union[JobDriverTypeDef, JobDriverOutputTypeDef] = ...,
-        configurationOverrides: Union[
-            ConfigurationOverridesTypeDef, ConfigurationOverridesOutputTypeDef
-        ] = ...,
+        jobDriver: JobDriverUnionTypeDef = ...,
+        configurationOverrides: ConfigurationOverridesUnionTypeDef = ...,
         tags: Mapping[str, str] = ...,
         executionTimeoutMinutes: int = ...,
         name: str = ...
     ) -> StartJobRunResponseTypeDef:
         """
         Starts a job run.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Client.start_job_run)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/client/#start_job_run)
         """
+
     def stop_application(self, *, applicationId: str) -> Dict[str, Any]:
         """
         Stops a specified application and releases initial capacity if configured.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Client.stop_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/client/#stop_application)
         """
+
     def tag_resource(self, *, resourceArn: str, tags: Mapping[str, str]) -> Dict[str, Any]:
         """
         Assigns tags to resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/client/#tag_resource)
         """
+
     def untag_resource(self, *, resourceArn: str, tagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Removes tags from resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/client/#untag_resource)
         """
+
     def update_application(
         self,
         *,
         applicationId: str,
         clientToken: str,
         initialCapacity: Mapping[str, InitialCapacityConfigTypeDef] = ...,
         maximumCapacity: MaximumAllowedResourcesTypeDef = ...,
         autoStartConfiguration: AutoStartConfigTypeDef = ...,
         autoStopConfiguration: AutoStopConfigTypeDef = ...,
-        networkConfiguration: Union[
-            NetworkConfigurationTypeDef, NetworkConfigurationOutputTypeDef
-        ] = ...,
+        networkConfiguration: NetworkConfigurationUnionTypeDef = ...,
         architecture: ArchitectureType = ...,
         imageConfiguration: ImageConfigurationInputTypeDef = ...,
         workerTypeSpecifications: Mapping[str, WorkerTypeSpecificationInputTypeDef] = ...,
         releaseLabel: str = ...
     ) -> UpdateApplicationResponseTypeDef:
         """
         Updates a specified application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Client.update_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/client/#update_application)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_applications"]
     ) -> ListApplicationsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["list_job_runs"]) -> ListJobRunsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/client/#get_paginator)
         """
```

### Comparing `mypy-boto3-emr-serverless-1.28.15.post1/mypy_boto3_emr_serverless/literals.py` & `mypy-boto3-emr-serverless-1.28.16/mypy_boto3_emr_serverless/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-serverless-1.28.15.post1/mypy_boto3_emr_serverless/literals.pyi` & `mypy-boto3-emr-serverless-1.28.16/mypy_boto3_emr_serverless/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-serverless-1.28.15.post1/mypy_boto3_emr_serverless/paginator.py` & `mypy-boto3-emr-serverless-1.28.16/mypy_boto3_emr_serverless/paginator.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,24 +17,24 @@
     session = Session()
     client: EMRServerlessClient = session.client("emr-serverless")
 
     list_applications_paginator: ListApplicationsPaginator = client.get_paginator("list_applications")
     list_job_runs_paginator: ListJobRunsPaginator = client.get_paginator("list_job_runs")
     ```
 """
-from datetime import datetime
-from typing import Generic, Iterator, Sequence, TypeVar, Union
+from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import ApplicationStateType, JobRunStateType
 from .type_defs import (
     ListApplicationsResponseTypeDef,
     ListJobRunsResponseTypeDef,
     PaginatorConfigTypeDef,
+    TimestampTypeDef,
 )
 
 __all__ = ("ListApplicationsPaginator", "ListJobRunsPaginator")
 
 
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
@@ -70,16 +70,16 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/paginators/#listjobrunspaginator)
     """
 
     def paginate(
         self,
         *,
         applicationId: str,
-        createdAtAfter: Union[datetime, str] = ...,
-        createdAtBefore: Union[datetime, str] = ...,
+        createdAtAfter: TimestampTypeDef = ...,
+        createdAtBefore: TimestampTypeDef = ...,
         states: Sequence[JobRunStateType] = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListJobRunsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Paginator.ListJobRuns.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/paginators/#listjobrunspaginator)
         """
```

### Comparing `mypy-boto3-emr-serverless-1.28.15.post1/mypy_boto3_emr_serverless/paginator.pyi` & `mypy-boto3-emr-serverless-1.28.16/mypy_boto3_emr_serverless/paginator.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -17,24 +17,24 @@
     session = Session()
     client: EMRServerlessClient = session.client("emr-serverless")
 
     list_applications_paginator: ListApplicationsPaginator = client.get_paginator("list_applications")
     list_job_runs_paginator: ListJobRunsPaginator = client.get_paginator("list_job_runs")
     ```
 """
-from datetime import datetime
-from typing import Generic, Iterator, Sequence, TypeVar, Union
+from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import ApplicationStateType, JobRunStateType
 from .type_defs import (
     ListApplicationsResponseTypeDef,
     ListJobRunsResponseTypeDef,
     PaginatorConfigTypeDef,
+    TimestampTypeDef,
 )
 
 __all__ = ("ListApplicationsPaginator", "ListJobRunsPaginator")
 
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
@@ -66,16 +66,16 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/paginators/#listjobrunspaginator)
     """
 
     def paginate(
         self,
         *,
         applicationId: str,
-        createdAtAfter: Union[datetime, str] = ...,
-        createdAtBefore: Union[datetime, str] = ...,
+        createdAtAfter: TimestampTypeDef = ...,
+        createdAtBefore: TimestampTypeDef = ...,
         states: Sequence[JobRunStateType] = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListJobRunsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Paginator.ListJobRuns.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/paginators/#listjobrunspaginator)
         """
```

### Comparing `mypy-boto3-emr-serverless-1.28.15.post1/mypy_boto3_emr_serverless/type_defs.py` & `mypy-boto3-emr-serverless-1.28.16/mypy_boto3_emr_serverless/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_emr_serverless.type_defs import ApplicationSummaryTypeDef
 
-    data: ApplicationSummaryTypeDef = {...}
+    data: ApplicationSummaryTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from .literals import ApplicationStateType, ArchitectureType, JobRunStateType
@@ -47,15 +47,15 @@
     "SparkSubmitOutputTypeDef",
     "SparkSubmitTypeDef",
     "JobRunSummaryTypeDef",
     "ResourceUtilizationTypeDef",
     "TotalResourceUtilizationTypeDef",
     "PaginatorConfigTypeDef",
     "ListApplicationsRequestRequestTypeDef",
-    "ListJobRunsRequestRequestTypeDef",
+    "TimestampTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ManagedPersistenceMonitoringConfigurationTypeDef",
     "S3MonitoringConfigurationTypeDef",
     "StartApplicationRequestRequestTypeDef",
     "StopApplicationRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
@@ -63,30 +63,34 @@
     "CancelJobRunResponseTypeDef",
     "CreateApplicationResponseTypeDef",
     "GetDashboardForJobRunResponseTypeDef",
     "ListApplicationsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "StartJobRunResponseTypeDef",
     "WorkerTypeSpecificationInputTypeDef",
+    "NetworkConfigurationUnionTypeDef",
     "InitialCapacityConfigTypeDef",
     "JobDriverOutputTypeDef",
     "JobDriverTypeDef",
     "ListJobRunsResponseTypeDef",
     "ListApplicationsRequestListApplicationsPaginateTypeDef",
     "ListJobRunsRequestListJobRunsPaginateTypeDef",
+    "ListJobRunsRequestRequestTypeDef",
     "MonitoringConfigurationOutputTypeDef",
     "MonitoringConfigurationTypeDef",
     "ApplicationTypeDef",
     "CreateApplicationRequestRequestTypeDef",
     "UpdateApplicationRequestRequestTypeDef",
+    "JobDriverUnionTypeDef",
     "ConfigurationOverridesOutputTypeDef",
     "ConfigurationOverridesTypeDef",
     "GetApplicationResponseTypeDef",
     "UpdateApplicationResponseTypeDef",
     "JobRunTypeDef",
+    "ConfigurationOverridesUnionTypeDef",
     "StartJobRunRequestRequestTypeDef",
     "GetJobRunResponseTypeDef",
 )
 
 _RequiredApplicationSummaryTypeDef = TypedDict(
     "_RequiredApplicationSummaryTypeDef",
     {
@@ -491,39 +495,15 @@
         "nextToken": str,
         "maxResults": int,
         "states": Sequence[ApplicationStateType],
     },
     total=False,
 )
 
-_RequiredListJobRunsRequestRequestTypeDef = TypedDict(
-    "_RequiredListJobRunsRequestRequestTypeDef",
-    {
-        "applicationId": str,
-    },
-)
-_OptionalListJobRunsRequestRequestTypeDef = TypedDict(
-    "_OptionalListJobRunsRequestRequestTypeDef",
-    {
-        "nextToken": str,
-        "maxResults": int,
-        "createdAtAfter": Union[datetime, str],
-        "createdAtBefore": Union[datetime, str],
-        "states": Sequence[JobRunStateType],
-    },
-    total=False,
-)
-
-
-class ListJobRunsRequestRequestTypeDef(
-    _RequiredListJobRunsRequestRequestTypeDef, _OptionalListJobRunsRequestRequestTypeDef
-):
-    pass
-
-
+TimestampTypeDef = Union[datetime, str]
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
@@ -641,14 +621,17 @@
     "WorkerTypeSpecificationInputTypeDef",
     {
         "imageConfiguration": ImageConfigurationInputTypeDef,
     },
     total=False,
 )
 
+NetworkConfigurationUnionTypeDef = Union[
+    NetworkConfigurationTypeDef, NetworkConfigurationOutputTypeDef
+]
 _RequiredInitialCapacityConfigTypeDef = TypedDict(
     "_RequiredInitialCapacityConfigTypeDef",
     {
         "workerCount": int,
     },
 )
 _OptionalInitialCapacityConfigTypeDef = TypedDict(
@@ -707,30 +690,55 @@
     {
         "applicationId": str,
     },
 )
 _OptionalListJobRunsRequestListJobRunsPaginateTypeDef = TypedDict(
     "_OptionalListJobRunsRequestListJobRunsPaginateTypeDef",
     {
-        "createdAtAfter": Union[datetime, str],
-        "createdAtBefore": Union[datetime, str],
+        "createdAtAfter": TimestampTypeDef,
+        "createdAtBefore": TimestampTypeDef,
         "states": Sequence[JobRunStateType],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class ListJobRunsRequestListJobRunsPaginateTypeDef(
     _RequiredListJobRunsRequestListJobRunsPaginateTypeDef,
     _OptionalListJobRunsRequestListJobRunsPaginateTypeDef,
 ):
     pass
 
 
+_RequiredListJobRunsRequestRequestTypeDef = TypedDict(
+    "_RequiredListJobRunsRequestRequestTypeDef",
+    {
+        "applicationId": str,
+    },
+)
+_OptionalListJobRunsRequestRequestTypeDef = TypedDict(
+    "_OptionalListJobRunsRequestRequestTypeDef",
+    {
+        "nextToken": str,
+        "maxResults": int,
+        "createdAtAfter": TimestampTypeDef,
+        "createdAtBefore": TimestampTypeDef,
+        "states": Sequence[JobRunStateType],
+    },
+    total=False,
+)
+
+
+class ListJobRunsRequestRequestTypeDef(
+    _RequiredListJobRunsRequestRequestTypeDef, _OptionalListJobRunsRequestRequestTypeDef
+):
+    pass
+
+
 MonitoringConfigurationOutputTypeDef = TypedDict(
     "MonitoringConfigurationOutputTypeDef",
     {
         "s3MonitoringConfiguration": S3MonitoringConfigurationTypeDef,
         "managedPersistenceMonitoringConfiguration": (
             ManagedPersistenceMonitoringConfigurationTypeDef
         ),
@@ -844,14 +852,15 @@
 
 class UpdateApplicationRequestRequestTypeDef(
     _RequiredUpdateApplicationRequestRequestTypeDef, _OptionalUpdateApplicationRequestRequestTypeDef
 ):
     pass
 
 
+JobDriverUnionTypeDef = Union[JobDriverTypeDef, JobDriverOutputTypeDef]
 ConfigurationOverridesOutputTypeDef = TypedDict(
     "ConfigurationOverridesOutputTypeDef",
     {
         "applicationConfiguration": List["ConfigurationOutputTypeDef"],
         "monitoringConfiguration": MonitoringConfigurationOutputTypeDef,
     },
     total=False,
@@ -914,14 +923,17 @@
 )
 
 
 class JobRunTypeDef(_RequiredJobRunTypeDef, _OptionalJobRunTypeDef):
     pass
 
 
+ConfigurationOverridesUnionTypeDef = Union[
+    ConfigurationOverridesTypeDef, ConfigurationOverridesOutputTypeDef
+]
 _RequiredStartJobRunRequestRequestTypeDef = TypedDict(
     "_RequiredStartJobRunRequestRequestTypeDef",
     {
         "applicationId": str,
         "clientToken": str,
         "executionRoleArn": str,
     },
```

### Comparing `mypy-boto3-emr-serverless-1.28.15.post1/mypy_boto3_emr_serverless/type_defs.pyi` & `mypy-boto3-emr-serverless-1.28.16/mypy_boto3_emr_serverless/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_emr_serverless.type_defs import ApplicationSummaryTypeDef
 
-    data: ApplicationSummaryTypeDef = {...}
+    data: ApplicationSummaryTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from .literals import ApplicationStateType, ArchitectureType, JobRunStateType
@@ -46,15 +46,15 @@
     "SparkSubmitOutputTypeDef",
     "SparkSubmitTypeDef",
     "JobRunSummaryTypeDef",
     "ResourceUtilizationTypeDef",
     "TotalResourceUtilizationTypeDef",
     "PaginatorConfigTypeDef",
     "ListApplicationsRequestRequestTypeDef",
-    "ListJobRunsRequestRequestTypeDef",
+    "TimestampTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ManagedPersistenceMonitoringConfigurationTypeDef",
     "S3MonitoringConfigurationTypeDef",
     "StartApplicationRequestRequestTypeDef",
     "StopApplicationRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
@@ -62,30 +62,34 @@
     "CancelJobRunResponseTypeDef",
     "CreateApplicationResponseTypeDef",
     "GetDashboardForJobRunResponseTypeDef",
     "ListApplicationsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "StartJobRunResponseTypeDef",
     "WorkerTypeSpecificationInputTypeDef",
+    "NetworkConfigurationUnionTypeDef",
     "InitialCapacityConfigTypeDef",
     "JobDriverOutputTypeDef",
     "JobDriverTypeDef",
     "ListJobRunsResponseTypeDef",
     "ListApplicationsRequestListApplicationsPaginateTypeDef",
     "ListJobRunsRequestListJobRunsPaginateTypeDef",
+    "ListJobRunsRequestRequestTypeDef",
     "MonitoringConfigurationOutputTypeDef",
     "MonitoringConfigurationTypeDef",
     "ApplicationTypeDef",
     "CreateApplicationRequestRequestTypeDef",
     "UpdateApplicationRequestRequestTypeDef",
+    "JobDriverUnionTypeDef",
     "ConfigurationOverridesOutputTypeDef",
     "ConfigurationOverridesTypeDef",
     "GetApplicationResponseTypeDef",
     "UpdateApplicationResponseTypeDef",
     "JobRunTypeDef",
+    "ConfigurationOverridesUnionTypeDef",
     "StartJobRunRequestRequestTypeDef",
     "GetJobRunResponseTypeDef",
 )
 
 _RequiredApplicationSummaryTypeDef = TypedDict(
     "_RequiredApplicationSummaryTypeDef",
     {
@@ -466,37 +470,15 @@
         "nextToken": str,
         "maxResults": int,
         "states": Sequence[ApplicationStateType],
     },
     total=False,
 )
 
-_RequiredListJobRunsRequestRequestTypeDef = TypedDict(
-    "_RequiredListJobRunsRequestRequestTypeDef",
-    {
-        "applicationId": str,
-    },
-)
-_OptionalListJobRunsRequestRequestTypeDef = TypedDict(
-    "_OptionalListJobRunsRequestRequestTypeDef",
-    {
-        "nextToken": str,
-        "maxResults": int,
-        "createdAtAfter": Union[datetime, str],
-        "createdAtBefore": Union[datetime, str],
-        "states": Sequence[JobRunStateType],
-    },
-    total=False,
-)
-
-class ListJobRunsRequestRequestTypeDef(
-    _RequiredListJobRunsRequestRequestTypeDef, _OptionalListJobRunsRequestRequestTypeDef
-):
-    pass
-
+TimestampTypeDef = Union[datetime, str]
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
@@ -614,14 +596,17 @@
     "WorkerTypeSpecificationInputTypeDef",
     {
         "imageConfiguration": ImageConfigurationInputTypeDef,
     },
     total=False,
 )
 
+NetworkConfigurationUnionTypeDef = Union[
+    NetworkConfigurationTypeDef, NetworkConfigurationOutputTypeDef
+]
 _RequiredInitialCapacityConfigTypeDef = TypedDict(
     "_RequiredInitialCapacityConfigTypeDef",
     {
         "workerCount": int,
     },
 )
 _OptionalInitialCapacityConfigTypeDef = TypedDict(
@@ -678,28 +663,51 @@
     {
         "applicationId": str,
     },
 )
 _OptionalListJobRunsRequestListJobRunsPaginateTypeDef = TypedDict(
     "_OptionalListJobRunsRequestListJobRunsPaginateTypeDef",
     {
-        "createdAtAfter": Union[datetime, str],
-        "createdAtBefore": Union[datetime, str],
+        "createdAtAfter": TimestampTypeDef,
+        "createdAtBefore": TimestampTypeDef,
         "states": Sequence[JobRunStateType],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class ListJobRunsRequestListJobRunsPaginateTypeDef(
     _RequiredListJobRunsRequestListJobRunsPaginateTypeDef,
     _OptionalListJobRunsRequestListJobRunsPaginateTypeDef,
 ):
     pass
 
+_RequiredListJobRunsRequestRequestTypeDef = TypedDict(
+    "_RequiredListJobRunsRequestRequestTypeDef",
+    {
+        "applicationId": str,
+    },
+)
+_OptionalListJobRunsRequestRequestTypeDef = TypedDict(
+    "_OptionalListJobRunsRequestRequestTypeDef",
+    {
+        "nextToken": str,
+        "maxResults": int,
+        "createdAtAfter": TimestampTypeDef,
+        "createdAtBefore": TimestampTypeDef,
+        "states": Sequence[JobRunStateType],
+    },
+    total=False,
+)
+
+class ListJobRunsRequestRequestTypeDef(
+    _RequiredListJobRunsRequestRequestTypeDef, _OptionalListJobRunsRequestRequestTypeDef
+):
+    pass
+
 MonitoringConfigurationOutputTypeDef = TypedDict(
     "MonitoringConfigurationOutputTypeDef",
     {
         "s3MonitoringConfiguration": S3MonitoringConfigurationTypeDef,
         "managedPersistenceMonitoringConfiguration": (
             ManagedPersistenceMonitoringConfigurationTypeDef
         ),
@@ -807,14 +815,15 @@
 )
 
 class UpdateApplicationRequestRequestTypeDef(
     _RequiredUpdateApplicationRequestRequestTypeDef, _OptionalUpdateApplicationRequestRequestTypeDef
 ):
     pass
 
+JobDriverUnionTypeDef = Union[JobDriverTypeDef, JobDriverOutputTypeDef]
 ConfigurationOverridesOutputTypeDef = TypedDict(
     "ConfigurationOverridesOutputTypeDef",
     {
         "applicationConfiguration": List["ConfigurationOutputTypeDef"],
         "monitoringConfiguration": MonitoringConfigurationOutputTypeDef,
     },
     total=False,
@@ -875,14 +884,17 @@
     },
     total=False,
 )
 
 class JobRunTypeDef(_RequiredJobRunTypeDef, _OptionalJobRunTypeDef):
     pass
 
+ConfigurationOverridesUnionTypeDef = Union[
+    ConfigurationOverridesTypeDef, ConfigurationOverridesOutputTypeDef
+]
 _RequiredStartJobRunRequestRequestTypeDef = TypedDict(
     "_RequiredStartJobRunRequestRequestTypeDef",
     {
         "applicationId": str,
         "clientToken": str,
         "executionRoleArn": str,
     },
```

### Comparing `mypy-boto3-emr-serverless-1.28.15.post1/mypy_boto3_emr_serverless.egg-info/PKG-INFO` & `mypy-boto3-emr-serverless-1.28.16/mypy_boto3_emr_serverless.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-emr-serverless
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.EMRServerless 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.EMRServerless 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 emr-serverless type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 emr-serverless type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-emr-serverless.svg?color=blue)](https://pypi.org/project/mypy-boto3-emr-serverless)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-emr-serverless)](https://pepy.tech/project/mypy-boto3-emr-serverless)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EMRServerless 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless)
+[boto3.EMRServerless 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless)
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
 [mypy-boto3-emr-serverless docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/).
 
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
@@ -316,20 +316,20 @@
 )
 
 
 def check_value(value: ApplicationStateType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_emr_serverless.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_emr_serverless.type_defs import (
     ApplicationSummaryTypeDef,
     AutoStartConfigTypeDef,
     AutoStopConfigTypeDef,
     ImageConfigurationTypeDef,
@@ -352,15 +352,15 @@
     SparkSubmitOutputTypeDef,
     SparkSubmitTypeDef,
     JobRunSummaryTypeDef,
     ResourceUtilizationTypeDef,
     TotalResourceUtilizationTypeDef,
     PaginatorConfigTypeDef,
     ListApplicationsRequestRequestTypeDef,
-    ListJobRunsRequestRequestTypeDef,
+    TimestampTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ManagedPersistenceMonitoringConfigurationTypeDef,
     S3MonitoringConfigurationTypeDef,
     StartApplicationRequestRequestTypeDef,
     StopApplicationRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
@@ -368,36 +368,40 @@
     CancelJobRunResponseTypeDef,
     CreateApplicationResponseTypeDef,
     GetDashboardForJobRunResponseTypeDef,
     ListApplicationsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     StartJobRunResponseTypeDef,
     WorkerTypeSpecificationInputTypeDef,
+    NetworkConfigurationUnionTypeDef,
     InitialCapacityConfigTypeDef,
     JobDriverOutputTypeDef,
     JobDriverTypeDef,
     ListJobRunsResponseTypeDef,
     ListApplicationsRequestListApplicationsPaginateTypeDef,
     ListJobRunsRequestListJobRunsPaginateTypeDef,
+    ListJobRunsRequestRequestTypeDef,
     MonitoringConfigurationOutputTypeDef,
     MonitoringConfigurationTypeDef,
     ApplicationTypeDef,
     CreateApplicationRequestRequestTypeDef,
     UpdateApplicationRequestRequestTypeDef,
+    JobDriverUnionTypeDef,
     ConfigurationOverridesOutputTypeDef,
     ConfigurationOverridesTypeDef,
     GetApplicationResponseTypeDef,
     UpdateApplicationResponseTypeDef,
     JobRunTypeDef,
+    ConfigurationOverridesUnionTypeDef,
     StartJobRunRequestRequestTypeDef,
     GetJobRunResponseTypeDef,
 )
 
 
-def get_structure() -> ApplicationSummaryTypeDef:
+def get_value() -> ApplicationSummaryTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-emr-serverless-1.28.15.post1/mypy_boto3_emr_serverless.egg-info/SOURCES.txt` & `mypy-boto3-emr-serverless-1.28.16/mypy_boto3_emr_serverless.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-serverless-1.28.15.post1/setup.py` & `mypy-boto3-emr-serverless-1.28.16/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-emr-serverless",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_emr_serverless"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.EMRServerless 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.2"
+        "Type annotations for boto3.EMRServerless 1.28.16 service generated with mypy-boto3-builder"
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
-    keywords="boto3 emr-serverless type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 emr-serverless type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_emr_serverless": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

