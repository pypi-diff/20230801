# Comparing `tmp/mypy-boto3-robomaker-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-robomaker-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-robomaker-1.28.15.post1.tar", last modified: Sat Jul 29 10:04:01 2023, max compression
+gzip compressed data, was "mypy-boto3-robomaker-1.28.16.tar", last modified: Tue Aug  1 11:37:41 2023, max compression
```

## Comparing `mypy-boto3-robomaker-1.28.15.post1.tar` & `mypy-boto3-robomaker-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:01.381365 mypy-boto3-robomaker-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:57:07.000000 mypy-boto3-robomaker-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    22090 2023-07-29 10:04:01.381365 mypy-boto3-robomaker-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20589 2023-07-29 09:57:07.000000 mypy-boto3-robomaker-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:01.381365 mypy-boto3-robomaker-1.28.15.post1/mypy_boto3_robomaker/
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-07-29 09:57:07.000000 mypy-boto3-robomaker-1.28.15.post1/mypy_boto3_robomaker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-07-29 09:57:07.000000 mypy-boto3-robomaker-1.28.15.post1/mypy_boto3_robomaker/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-29 09:57:07.000000 mypy-boto3-robomaker-1.28.15.post1/mypy_boto3_robomaker/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42816 2023-07-29 09:57:08.000000 mypy-boto3-robomaker-1.28.15.post1/mypy_boto3_robomaker/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    42741 2023-07-29 09:57:07.000000 mypy-boto3-robomaker-1.28.15.post1/mypy_boto3_robomaker/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13921 2023-07-29 09:57:08.000000 mypy-boto3-robomaker-1.28.15.post1/mypy_boto3_robomaker/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13919 2023-07-29 09:57:08.000000 mypy-boto3-robomaker-1.28.15.post1/mypy_boto3_robomaker/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13390 2023-07-29 09:57:08.000000 mypy-boto3-robomaker-1.28.15.post1/mypy_boto3_robomaker/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13377 2023-07-29 09:57:08.000000 mypy-boto3-robomaker-1.28.15.post1/mypy_boto3_robomaker/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:57:07.000000 mypy-boto3-robomaker-1.28.15.post1/mypy_boto3_robomaker/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    69081 2023-07-29 09:57:10.000000 mypy-boto3-robomaker-1.28.15.post1/mypy_boto3_robomaker/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    69014 2023-07-29 09:57:09.000000 mypy-boto3-robomaker-1.28.15.post1/mypy_boto3_robomaker/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:57:07.000000 mypy-boto3-robomaker-1.28.15.post1/mypy_boto3_robomaker/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:01.381365 mypy-boto3-robomaker-1.28.15.post1/mypy_boto3_robomaker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22090 2023-07-29 10:04:01.000000 mypy-boto3-robomaker-1.28.15.post1/mypy_boto3_robomaker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-29 10:04:01.000000 mypy-boto3-robomaker-1.28.15.post1/mypy_boto3_robomaker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:01.000000 mypy-boto3-robomaker-1.28.15.post1/mypy_boto3_robomaker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:01.000000 mypy-boto3-robomaker-1.28.15.post1/mypy_boto3_robomaker.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:04:01.000000 mypy-boto3-robomaker-1.28.15.post1/mypy_boto3_robomaker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-29 10:04:01.000000 mypy-boto3-robomaker-1.28.15.post1/mypy_boto3_robomaker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:04:01.381365 mypy-boto3-robomaker-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-07-29 09:57:07.000000 mypy-boto3-robomaker-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:41.464766 mypy-boto3-robomaker-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:30:30.000000 mypy-boto3-robomaker-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22309 2023-08-01 11:37:41.452767 mypy-boto3-robomaker-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20817 2023-08-01 11:30:30.000000 mypy-boto3-robomaker-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:41.444766 mypy-boto3-robomaker-1.28.16/mypy_boto3_robomaker/
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-08-01 11:30:30.000000 mypy-boto3-robomaker-1.28.16/mypy_boto3_robomaker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-08-01 11:30:30.000000 mypy-boto3-robomaker-1.28.16/mypy_boto3_robomaker/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-08-01 11:30:30.000000 mypy-boto3-robomaker-1.28.16/mypy_boto3_robomaker/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42293 2023-08-01 11:30:30.000000 mypy-boto3-robomaker-1.28.16/mypy_boto3_robomaker/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42218 2023-08-01 11:30:30.000000 mypy-boto3-robomaker-1.28.16/mypy_boto3_robomaker/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13921 2023-08-01 11:30:31.000000 mypy-boto3-robomaker-1.28.16/mypy_boto3_robomaker/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13919 2023-08-01 11:30:31.000000 mypy-boto3-robomaker-1.28.16/mypy_boto3_robomaker/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13390 2023-08-01 11:30:31.000000 mypy-boto3-robomaker-1.28.16/mypy_boto3_robomaker/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13377 2023-08-01 11:30:31.000000 mypy-boto3-robomaker-1.28.16/mypy_boto3_robomaker/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:30:30.000000 mypy-boto3-robomaker-1.28.16/mypy_boto3_robomaker/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    69691 2023-08-01 11:30:37.000000 mypy-boto3-robomaker-1.28.16/mypy_boto3_robomaker/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69625 2023-08-01 11:30:32.000000 mypy-boto3-robomaker-1.28.16/mypy_boto3_robomaker/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:30:30.000000 mypy-boto3-robomaker-1.28.16/mypy_boto3_robomaker/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:41.452767 mypy-boto3-robomaker-1.28.16/mypy_boto3_robomaker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22309 2023-08-01 11:37:41.000000 mypy-boto3-robomaker-1.28.16/mypy_boto3_robomaker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-08-01 11:37:41.000000 mypy-boto3-robomaker-1.28.16/mypy_boto3_robomaker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:41.000000 mypy-boto3-robomaker-1.28.16/mypy_boto3_robomaker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:41.000000 mypy-boto3-robomaker-1.28.16/mypy_boto3_robomaker.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:41.000000 mypy-boto3-robomaker-1.28.16/mypy_boto3_robomaker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-01 11:37:41.000000 mypy-boto3-robomaker-1.28.16/mypy_boto3_robomaker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:41.464766 mypy-boto3-robomaker-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-08-01 11:30:30.000000 mypy-boto3-robomaker-1.28.16/setup.py
```

### Comparing `mypy-boto3-robomaker-1.28.15.post1/LICENSE` & `mypy-boto3-robomaker-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-robomaker-1.28.15.post1/PKG-INFO` & `mypy-boto3-robomaker-1.28.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-robomaker
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.RoboMaker 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.RoboMaker 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 robomaker type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 robomaker type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-robomaker.svg?color=blue)](https://pypi.org/project/mypy-boto3-robomaker)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-robomaker)](https://pepy.tech/project/mypy-boto3-robomaker)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.RoboMaker 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker)
+[boto3.RoboMaker 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker)
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
 [mypy-boto3-robomaker docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/).
 
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
@@ -379,20 +379,20 @@
 )
 
 
 def check_value(value: ArchitectureType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_robomaker.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_robomaker.type_defs import (
     BatchDeleteWorldsRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     BatchDescribeSimulationJobRequestRequestTypeDef,
     BatchPolicyTypeDef,
@@ -409,22 +409,22 @@
     SourceConfigTypeDef,
     SourceTypeDef,
     CreateRobotApplicationVersionRequestRequestTypeDef,
     CreateRobotRequestRequestTypeDef,
     RenderingEngineTypeDef,
     SimulationSoftwareSuiteTypeDef,
     CreateSimulationApplicationVersionRequestRequestTypeDef,
-    DataSourceConfigOutputTypeDef,
-    DataSourceConfigTypeDef,
     LoggingConfigTypeDef,
     OutputLocationTypeDef,
     VPCConfigTypeDef,
     VPCConfigResponseTypeDef,
     WorldCountTypeDef,
     TemplateLocationTypeDef,
+    DataSourceConfigOutputTypeDef,
+    DataSourceConfigTypeDef,
     S3KeyOutputTypeDef,
     DeleteFleetRequestRequestTypeDef,
     DeleteRobotApplicationRequestRequestTypeDef,
     DeleteRobotRequestRequestTypeDef,
     DeleteSimulationApplicationRequestRequestTypeDef,
     DeleteWorldTemplateRequestRequestTypeDef,
     DeploymentLaunchConfigOutputTypeDef,
@@ -497,14 +497,15 @@
     DescribeWorldExportJobResponseTypeDef,
     WorldExportJobSummaryTypeDef,
     CreateWorldGenerationJobRequestRequestTypeDef,
     CreateWorldGenerationJobResponseTypeDef,
     WorldGenerationJobSummaryTypeDef,
     CreateWorldTemplateRequestRequestTypeDef,
     UpdateWorldTemplateRequestRequestTypeDef,
+    DataSourceConfigUnionTypeDef,
     DataSourceTypeDef,
     DeploymentApplicationConfigOutputTypeDef,
     DeploymentApplicationConfigTypeDef,
     DeploymentConfigTypeDef,
     DescribeFleetResponseTypeDef,
     ListRobotsResponseTypeDef,
     ListSimulationJobsResponseTypeDef,
@@ -533,47 +534,52 @@
     ListWorldsRequestListWorldsPaginateTypeDef,
     ListSimulationJobBatchesResponseTypeDef,
     ListWorldTemplatesResponseTypeDef,
     ListWorldsResponseTypeDef,
     PortForwardingConfigOutputTypeDef,
     PortForwardingConfigTypeDef,
     RobotDeploymentTypeDef,
+    VPCConfigUnionTypeDef,
     ListRobotApplicationsResponseTypeDef,
     ListSimulationApplicationsResponseTypeDef,
     ListWorldExportJobsResponseTypeDef,
     ListWorldGenerationJobsResponseTypeDef,
-    CreateDeploymentJobRequestRequestTypeDef,
+    DeploymentApplicationConfigUnionTypeDef,
     CreateDeploymentJobResponseTypeDef,
     DeploymentJobTypeDef,
     SyncDeploymentJobResponseTypeDef,
     FinishedWorldsSummaryTypeDef,
     LaunchConfigOutputTypeDef,
     LaunchConfigTypeDef,
     DescribeDeploymentJobResponseTypeDef,
+    CreateDeploymentJobRequestRequestTypeDef,
     ListDeploymentJobsResponseTypeDef,
     DescribeWorldGenerationJobResponseTypeDef,
     RobotApplicationConfigOutputTypeDef,
     SimulationApplicationConfigOutputTypeDef,
     RobotApplicationConfigTypeDef,
     SimulationApplicationConfigTypeDef,
     CreateSimulationJobResponseTypeDef,
     DescribeSimulationJobResponseTypeDef,
     SimulationJobRequestOutputTypeDef,
     SimulationJobTypeDef,
-    CreateSimulationJobRequestRequestTypeDef,
+    RobotApplicationConfigUnionTypeDef,
+    SimulationApplicationConfigUnionTypeDef,
     SimulationJobRequestTypeDef,
     FailedCreateSimulationJobRequestTypeDef,
     BatchDescribeSimulationJobResponseTypeDef,
-    StartSimulationJobBatchRequestRequestTypeDef,
+    CreateSimulationJobRequestRequestTypeDef,
+    SimulationJobRequestUnionTypeDef,
     DescribeSimulationJobBatchResponseTypeDef,
     StartSimulationJobBatchResponseTypeDef,
+    StartSimulationJobBatchRequestRequestTypeDef,
 )
 
 
-def get_structure() -> BatchDeleteWorldsRequestRequestTypeDef:
+def get_value() -> BatchDeleteWorldsRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-robomaker-1.28.15.post1/README.md` & `mypy-boto3-robomaker-1.28.16/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-robomaker.svg?color=blue)](https://pypi.org/project/mypy-boto3-robomaker)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-robomaker)](https://pepy.tech/project/mypy-boto3-robomaker)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.RoboMaker 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker)
+[boto3.RoboMaker 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker)
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
 [mypy-boto3-robomaker docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/).
 
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
@@ -347,20 +347,20 @@
 )
 
 
 def check_value(value: ArchitectureType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_robomaker.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_robomaker.type_defs import (
     BatchDeleteWorldsRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     BatchDescribeSimulationJobRequestRequestTypeDef,
     BatchPolicyTypeDef,
@@ -377,22 +377,22 @@
     SourceConfigTypeDef,
     SourceTypeDef,
     CreateRobotApplicationVersionRequestRequestTypeDef,
     CreateRobotRequestRequestTypeDef,
     RenderingEngineTypeDef,
     SimulationSoftwareSuiteTypeDef,
     CreateSimulationApplicationVersionRequestRequestTypeDef,
-    DataSourceConfigOutputTypeDef,
-    DataSourceConfigTypeDef,
     LoggingConfigTypeDef,
     OutputLocationTypeDef,
     VPCConfigTypeDef,
     VPCConfigResponseTypeDef,
     WorldCountTypeDef,
     TemplateLocationTypeDef,
+    DataSourceConfigOutputTypeDef,
+    DataSourceConfigTypeDef,
     S3KeyOutputTypeDef,
     DeleteFleetRequestRequestTypeDef,
     DeleteRobotApplicationRequestRequestTypeDef,
     DeleteRobotRequestRequestTypeDef,
     DeleteSimulationApplicationRequestRequestTypeDef,
     DeleteWorldTemplateRequestRequestTypeDef,
     DeploymentLaunchConfigOutputTypeDef,
@@ -465,14 +465,15 @@
     DescribeWorldExportJobResponseTypeDef,
     WorldExportJobSummaryTypeDef,
     CreateWorldGenerationJobRequestRequestTypeDef,
     CreateWorldGenerationJobResponseTypeDef,
     WorldGenerationJobSummaryTypeDef,
     CreateWorldTemplateRequestRequestTypeDef,
     UpdateWorldTemplateRequestRequestTypeDef,
+    DataSourceConfigUnionTypeDef,
     DataSourceTypeDef,
     DeploymentApplicationConfigOutputTypeDef,
     DeploymentApplicationConfigTypeDef,
     DeploymentConfigTypeDef,
     DescribeFleetResponseTypeDef,
     ListRobotsResponseTypeDef,
     ListSimulationJobsResponseTypeDef,
@@ -501,47 +502,52 @@
     ListWorldsRequestListWorldsPaginateTypeDef,
     ListSimulationJobBatchesResponseTypeDef,
     ListWorldTemplatesResponseTypeDef,
     ListWorldsResponseTypeDef,
     PortForwardingConfigOutputTypeDef,
     PortForwardingConfigTypeDef,
     RobotDeploymentTypeDef,
+    VPCConfigUnionTypeDef,
     ListRobotApplicationsResponseTypeDef,
     ListSimulationApplicationsResponseTypeDef,
     ListWorldExportJobsResponseTypeDef,
     ListWorldGenerationJobsResponseTypeDef,
-    CreateDeploymentJobRequestRequestTypeDef,
+    DeploymentApplicationConfigUnionTypeDef,
     CreateDeploymentJobResponseTypeDef,
     DeploymentJobTypeDef,
     SyncDeploymentJobResponseTypeDef,
     FinishedWorldsSummaryTypeDef,
     LaunchConfigOutputTypeDef,
     LaunchConfigTypeDef,
     DescribeDeploymentJobResponseTypeDef,
+    CreateDeploymentJobRequestRequestTypeDef,
     ListDeploymentJobsResponseTypeDef,
     DescribeWorldGenerationJobResponseTypeDef,
     RobotApplicationConfigOutputTypeDef,
     SimulationApplicationConfigOutputTypeDef,
     RobotApplicationConfigTypeDef,
     SimulationApplicationConfigTypeDef,
     CreateSimulationJobResponseTypeDef,
     DescribeSimulationJobResponseTypeDef,
     SimulationJobRequestOutputTypeDef,
     SimulationJobTypeDef,
-    CreateSimulationJobRequestRequestTypeDef,
+    RobotApplicationConfigUnionTypeDef,
+    SimulationApplicationConfigUnionTypeDef,
     SimulationJobRequestTypeDef,
     FailedCreateSimulationJobRequestTypeDef,
     BatchDescribeSimulationJobResponseTypeDef,
-    StartSimulationJobBatchRequestRequestTypeDef,
+    CreateSimulationJobRequestRequestTypeDef,
+    SimulationJobRequestUnionTypeDef,
     DescribeSimulationJobBatchResponseTypeDef,
     StartSimulationJobBatchResponseTypeDef,
+    StartSimulationJobBatchRequestRequestTypeDef,
 )
 
 
-def get_structure() -> BatchDeleteWorldsRequestRequestTypeDef:
+def get_value() -> BatchDeleteWorldsRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-robomaker-1.28.15.post1/mypy_boto3_robomaker/__init__.py` & `mypy-boto3-robomaker-1.28.16/mypy_boto3_robomaker/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-robomaker-1.28.15.post1/mypy_boto3_robomaker/__init__.pyi` & `mypy-boto3-robomaker-1.28.16/mypy_boto3_robomaker/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-robomaker-1.28.15.post1/mypy_boto3_robomaker/__main__.py` & `mypy-boto3-robomaker-1.28.16/mypy_boto3_robomaker/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.RoboMaker 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.RoboMaker 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker\nOther"
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

### Comparing `mypy-boto3-robomaker-1.28.15.post1/mypy_boto3_robomaker/client.py` & `mypy-boto3-robomaker-1.28.16/mypy_boto3_robomaker/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_robomaker.client import RoboMakerClient
 
     session = Session()
     client: RoboMakerClient = session.client("robomaker")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import ArchitectureType, FailureBehaviorType
 from .paginator import (
     ListDeploymentJobsPaginator,
     ListFleetsPaginator,
@@ -44,18 +44,16 @@
     CreateRobotResponseTypeDef,
     CreateSimulationApplicationResponseTypeDef,
     CreateSimulationApplicationVersionResponseTypeDef,
     CreateSimulationJobResponseTypeDef,
     CreateWorldExportJobResponseTypeDef,
     CreateWorldGenerationJobResponseTypeDef,
     CreateWorldTemplateResponseTypeDef,
-    DataSourceConfigOutputTypeDef,
-    DataSourceConfigTypeDef,
-    DeploymentApplicationConfigOutputTypeDef,
-    DeploymentApplicationConfigTypeDef,
+    DataSourceConfigUnionTypeDef,
+    DeploymentApplicationConfigUnionTypeDef,
     DeploymentConfigTypeDef,
     DeregisterRobotResponseTypeDef,
     DescribeDeploymentJobResponseTypeDef,
     DescribeFleetResponseTypeDef,
     DescribeRobotApplicationResponseTypeDef,
     DescribeRobotResponseTypeDef,
     DescribeSimulationApplicationResponseTypeDef,
@@ -80,31 +78,27 @@
     ListWorldGenerationJobsResponseTypeDef,
     ListWorldsResponseTypeDef,
     ListWorldTemplatesResponseTypeDef,
     LoggingConfigTypeDef,
     OutputLocationTypeDef,
     RegisterRobotResponseTypeDef,
     RenderingEngineTypeDef,
-    RobotApplicationConfigOutputTypeDef,
-    RobotApplicationConfigTypeDef,
+    RobotApplicationConfigUnionTypeDef,
     RobotSoftwareSuiteTypeDef,
-    SimulationApplicationConfigOutputTypeDef,
-    SimulationApplicationConfigTypeDef,
-    SimulationJobRequestOutputTypeDef,
-    SimulationJobRequestTypeDef,
+    SimulationApplicationConfigUnionTypeDef,
+    SimulationJobRequestUnionTypeDef,
     SimulationSoftwareSuiteTypeDef,
     SourceConfigTypeDef,
     StartSimulationJobBatchResponseTypeDef,
     SyncDeploymentJobResponseTypeDef,
     TemplateLocationTypeDef,
     UpdateRobotApplicationResponseTypeDef,
     UpdateSimulationApplicationResponseTypeDef,
     UpdateWorldTemplateResponseTypeDef,
-    VPCConfigOutputTypeDef,
-    VPCConfigTypeDef,
+    VPCConfigUnionTypeDef,
     WorldCountTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -226,17 +220,15 @@
         """
 
     def create_deployment_job(
         self,
         *,
         clientRequestToken: str,
         fleet: str,
-        deploymentApplicationConfigs: Sequence[
-            Union[DeploymentApplicationConfigTypeDef, DeploymentApplicationConfigOutputTypeDef]
-        ],
+        deploymentApplicationConfigs: Sequence[DeploymentApplicationConfigUnionTypeDef],
         deploymentConfig: DeploymentConfigTypeDef = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateDeploymentJobResponseTypeDef:
         """
         Deploys a specific version of a robot application to robots in a fleet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.create_deployment_job)
@@ -337,23 +329,19 @@
         *,
         maxJobDurationInSeconds: int,
         iamRole: str,
         clientRequestToken: str = ...,
         outputLocation: OutputLocationTypeDef = ...,
         loggingConfig: LoggingConfigTypeDef = ...,
         failureBehavior: FailureBehaviorType = ...,
-        robotApplications: Sequence[
-            Union[RobotApplicationConfigTypeDef, RobotApplicationConfigOutputTypeDef]
-        ] = ...,
-        simulationApplications: Sequence[
-            Union[SimulationApplicationConfigTypeDef, SimulationApplicationConfigOutputTypeDef]
-        ] = ...,
-        dataSources: Sequence[Union[DataSourceConfigTypeDef, DataSourceConfigOutputTypeDef]] = ...,
+        robotApplications: Sequence[RobotApplicationConfigUnionTypeDef] = ...,
+        simulationApplications: Sequence[SimulationApplicationConfigUnionTypeDef] = ...,
+        dataSources: Sequence[DataSourceConfigUnionTypeDef] = ...,
         tags: Mapping[str, str] = ...,
-        vpcConfig: Union[VPCConfigTypeDef, VPCConfigOutputTypeDef] = ...,
+        vpcConfig: VPCConfigUnionTypeDef = ...,
         compute: ComputeTypeDef = ...
     ) -> CreateSimulationJobResponseTypeDef:
         """
         Creates a simulation job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.create_simulation_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/client/#create_simulation_job)
@@ -722,17 +710,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.restart_simulation_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/client/#restart_simulation_job)
         """
 
     def start_simulation_job_batch(
         self,
         *,
-        createSimulationJobRequests: Sequence[
-            Union[SimulationJobRequestTypeDef, SimulationJobRequestOutputTypeDef]
-        ],
+        createSimulationJobRequests: Sequence[SimulationJobRequestUnionTypeDef],
         clientRequestToken: str = ...,
         batchPolicy: BatchPolicyTypeDef = ...,
         tags: Mapping[str, str] = ...
     ) -> StartSimulationJobBatchResponseTypeDef:
         """
         Starts a new simulation job batch.
```

### Comparing `mypy-boto3-robomaker-1.28.15.post1/mypy_boto3_robomaker/client.pyi` & `mypy-boto3-robomaker-1.28.16/mypy_boto3_robomaker/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_robomaker.client import RoboMakerClient
 
     session = Session()
     client: RoboMakerClient = session.client("robomaker")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import ArchitectureType, FailureBehaviorType
 from .paginator import (
     ListDeploymentJobsPaginator,
     ListFleetsPaginator,
@@ -44,18 +44,16 @@
     CreateRobotResponseTypeDef,
     CreateSimulationApplicationResponseTypeDef,
     CreateSimulationApplicationVersionResponseTypeDef,
     CreateSimulationJobResponseTypeDef,
     CreateWorldExportJobResponseTypeDef,
     CreateWorldGenerationJobResponseTypeDef,
     CreateWorldTemplateResponseTypeDef,
-    DataSourceConfigOutputTypeDef,
-    DataSourceConfigTypeDef,
-    DeploymentApplicationConfigOutputTypeDef,
-    DeploymentApplicationConfigTypeDef,
+    DataSourceConfigUnionTypeDef,
+    DeploymentApplicationConfigUnionTypeDef,
     DeploymentConfigTypeDef,
     DeregisterRobotResponseTypeDef,
     DescribeDeploymentJobResponseTypeDef,
     DescribeFleetResponseTypeDef,
     DescribeRobotApplicationResponseTypeDef,
     DescribeRobotResponseTypeDef,
     DescribeSimulationApplicationResponseTypeDef,
@@ -80,31 +78,27 @@
     ListWorldGenerationJobsResponseTypeDef,
     ListWorldsResponseTypeDef,
     ListWorldTemplatesResponseTypeDef,
     LoggingConfigTypeDef,
     OutputLocationTypeDef,
     RegisterRobotResponseTypeDef,
     RenderingEngineTypeDef,
-    RobotApplicationConfigOutputTypeDef,
-    RobotApplicationConfigTypeDef,
+    RobotApplicationConfigUnionTypeDef,
     RobotSoftwareSuiteTypeDef,
-    SimulationApplicationConfigOutputTypeDef,
-    SimulationApplicationConfigTypeDef,
-    SimulationJobRequestOutputTypeDef,
-    SimulationJobRequestTypeDef,
+    SimulationApplicationConfigUnionTypeDef,
+    SimulationJobRequestUnionTypeDef,
     SimulationSoftwareSuiteTypeDef,
     SourceConfigTypeDef,
     StartSimulationJobBatchResponseTypeDef,
     SyncDeploymentJobResponseTypeDef,
     TemplateLocationTypeDef,
     UpdateRobotApplicationResponseTypeDef,
     UpdateSimulationApplicationResponseTypeDef,
     UpdateWorldTemplateResponseTypeDef,
-    VPCConfigOutputTypeDef,
-    VPCConfigTypeDef,
+    VPCConfigUnionTypeDef,
     WorldCountTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -212,17 +206,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/client/#close)
         """
     def create_deployment_job(
         self,
         *,
         clientRequestToken: str,
         fleet: str,
-        deploymentApplicationConfigs: Sequence[
-            Union[DeploymentApplicationConfigTypeDef, DeploymentApplicationConfigOutputTypeDef]
-        ],
+        deploymentApplicationConfigs: Sequence[DeploymentApplicationConfigUnionTypeDef],
         deploymentConfig: DeploymentConfigTypeDef = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateDeploymentJobResponseTypeDef:
         """
         Deploys a specific version of a robot application to robots in a fleet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.create_deployment_job)
@@ -316,23 +308,19 @@
         *,
         maxJobDurationInSeconds: int,
         iamRole: str,
         clientRequestToken: str = ...,
         outputLocation: OutputLocationTypeDef = ...,
         loggingConfig: LoggingConfigTypeDef = ...,
         failureBehavior: FailureBehaviorType = ...,
-        robotApplications: Sequence[
-            Union[RobotApplicationConfigTypeDef, RobotApplicationConfigOutputTypeDef]
-        ] = ...,
-        simulationApplications: Sequence[
-            Union[SimulationApplicationConfigTypeDef, SimulationApplicationConfigOutputTypeDef]
-        ] = ...,
-        dataSources: Sequence[Union[DataSourceConfigTypeDef, DataSourceConfigOutputTypeDef]] = ...,
+        robotApplications: Sequence[RobotApplicationConfigUnionTypeDef] = ...,
+        simulationApplications: Sequence[SimulationApplicationConfigUnionTypeDef] = ...,
+        dataSources: Sequence[DataSourceConfigUnionTypeDef] = ...,
         tags: Mapping[str, str] = ...,
-        vpcConfig: Union[VPCConfigTypeDef, VPCConfigOutputTypeDef] = ...,
+        vpcConfig: VPCConfigUnionTypeDef = ...,
         compute: ComputeTypeDef = ...
     ) -> CreateSimulationJobResponseTypeDef:
         """
         Creates a simulation job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.create_simulation_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/client/#create_simulation_job)
@@ -664,17 +652,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.restart_simulation_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/client/#restart_simulation_job)
         """
     def start_simulation_job_batch(
         self,
         *,
-        createSimulationJobRequests: Sequence[
-            Union[SimulationJobRequestTypeDef, SimulationJobRequestOutputTypeDef]
-        ],
+        createSimulationJobRequests: Sequence[SimulationJobRequestUnionTypeDef],
         clientRequestToken: str = ...,
         batchPolicy: BatchPolicyTypeDef = ...,
         tags: Mapping[str, str] = ...
     ) -> StartSimulationJobBatchResponseTypeDef:
         """
         Starts a new simulation job batch.
```

### Comparing `mypy-boto3-robomaker-1.28.15.post1/mypy_boto3_robomaker/literals.py` & `mypy-boto3-robomaker-1.28.16/mypy_boto3_robomaker/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-robomaker-1.28.15.post1/mypy_boto3_robomaker/literals.pyi` & `mypy-boto3-robomaker-1.28.16/mypy_boto3_robomaker/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-robomaker-1.28.15.post1/mypy_boto3_robomaker/paginator.py` & `mypy-boto3-robomaker-1.28.16/mypy_boto3_robomaker/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-robomaker-1.28.15.post1/mypy_boto3_robomaker/paginator.pyi` & `mypy-boto3-robomaker-1.28.16/mypy_boto3_robomaker/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-robomaker-1.28.15.post1/mypy_boto3_robomaker/type_defs.py` & `mypy-boto3-robomaker-1.28.16/mypy_boto3_robomaker/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_robomaker.type_defs import BatchDeleteWorldsRequestRequestTypeDef
 
-    data: BatchDeleteWorldsRequestRequestTypeDef = {...}
+    data: BatchDeleteWorldsRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -66,22 +66,22 @@
     "SourceConfigTypeDef",
     "SourceTypeDef",
     "CreateRobotApplicationVersionRequestRequestTypeDef",
     "CreateRobotRequestRequestTypeDef",
     "RenderingEngineTypeDef",
     "SimulationSoftwareSuiteTypeDef",
     "CreateSimulationApplicationVersionRequestRequestTypeDef",
-    "DataSourceConfigOutputTypeDef",
-    "DataSourceConfigTypeDef",
     "LoggingConfigTypeDef",
     "OutputLocationTypeDef",
     "VPCConfigTypeDef",
     "VPCConfigResponseTypeDef",
     "WorldCountTypeDef",
     "TemplateLocationTypeDef",
+    "DataSourceConfigOutputTypeDef",
+    "DataSourceConfigTypeDef",
     "S3KeyOutputTypeDef",
     "DeleteFleetRequestRequestTypeDef",
     "DeleteRobotApplicationRequestRequestTypeDef",
     "DeleteRobotRequestRequestTypeDef",
     "DeleteSimulationApplicationRequestRequestTypeDef",
     "DeleteWorldTemplateRequestRequestTypeDef",
     "DeploymentLaunchConfigOutputTypeDef",
@@ -154,14 +154,15 @@
     "DescribeWorldExportJobResponseTypeDef",
     "WorldExportJobSummaryTypeDef",
     "CreateWorldGenerationJobRequestRequestTypeDef",
     "CreateWorldGenerationJobResponseTypeDef",
     "WorldGenerationJobSummaryTypeDef",
     "CreateWorldTemplateRequestRequestTypeDef",
     "UpdateWorldTemplateRequestRequestTypeDef",
+    "DataSourceConfigUnionTypeDef",
     "DataSourceTypeDef",
     "DeploymentApplicationConfigOutputTypeDef",
     "DeploymentApplicationConfigTypeDef",
     "DeploymentConfigTypeDef",
     "DescribeFleetResponseTypeDef",
     "ListRobotsResponseTypeDef",
     "ListSimulationJobsResponseTypeDef",
@@ -190,43 +191,48 @@
     "ListWorldsRequestListWorldsPaginateTypeDef",
     "ListSimulationJobBatchesResponseTypeDef",
     "ListWorldTemplatesResponseTypeDef",
     "ListWorldsResponseTypeDef",
     "PortForwardingConfigOutputTypeDef",
     "PortForwardingConfigTypeDef",
     "RobotDeploymentTypeDef",
+    "VPCConfigUnionTypeDef",
     "ListRobotApplicationsResponseTypeDef",
     "ListSimulationApplicationsResponseTypeDef",
     "ListWorldExportJobsResponseTypeDef",
     "ListWorldGenerationJobsResponseTypeDef",
-    "CreateDeploymentJobRequestRequestTypeDef",
+    "DeploymentApplicationConfigUnionTypeDef",
     "CreateDeploymentJobResponseTypeDef",
     "DeploymentJobTypeDef",
     "SyncDeploymentJobResponseTypeDef",
     "FinishedWorldsSummaryTypeDef",
     "LaunchConfigOutputTypeDef",
     "LaunchConfigTypeDef",
     "DescribeDeploymentJobResponseTypeDef",
+    "CreateDeploymentJobRequestRequestTypeDef",
     "ListDeploymentJobsResponseTypeDef",
     "DescribeWorldGenerationJobResponseTypeDef",
     "RobotApplicationConfigOutputTypeDef",
     "SimulationApplicationConfigOutputTypeDef",
     "RobotApplicationConfigTypeDef",
     "SimulationApplicationConfigTypeDef",
     "CreateSimulationJobResponseTypeDef",
     "DescribeSimulationJobResponseTypeDef",
     "SimulationJobRequestOutputTypeDef",
     "SimulationJobTypeDef",
-    "CreateSimulationJobRequestRequestTypeDef",
+    "RobotApplicationConfigUnionTypeDef",
+    "SimulationApplicationConfigUnionTypeDef",
     "SimulationJobRequestTypeDef",
     "FailedCreateSimulationJobRequestTypeDef",
     "BatchDescribeSimulationJobResponseTypeDef",
-    "StartSimulationJobBatchRequestRequestTypeDef",
+    "CreateSimulationJobRequestRequestTypeDef",
+    "SimulationJobRequestUnionTypeDef",
     "DescribeSimulationJobBatchResponseTypeDef",
     "StartSimulationJobBatchResponseTypeDef",
+    "StartSimulationJobBatchRequestRequestTypeDef",
 )
 
 BatchDeleteWorldsRequestRequestTypeDef = TypedDict(
     "BatchDeleteWorldsRequestRequestTypeDef",
     {
         "worlds": Sequence[str],
     },
@@ -458,60 +464,14 @@
 class CreateSimulationApplicationVersionRequestRequestTypeDef(
     _RequiredCreateSimulationApplicationVersionRequestRequestTypeDef,
     _OptionalCreateSimulationApplicationVersionRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredDataSourceConfigOutputTypeDef = TypedDict(
-    "_RequiredDataSourceConfigOutputTypeDef",
-    {
-        "name": str,
-        "s3Bucket": str,
-        "s3Keys": List[str],
-    },
-)
-_OptionalDataSourceConfigOutputTypeDef = TypedDict(
-    "_OptionalDataSourceConfigOutputTypeDef",
-    {
-        "type": DataSourceTypeType,
-        "destination": str,
-    },
-    total=False,
-)
-
-
-class DataSourceConfigOutputTypeDef(
-    _RequiredDataSourceConfigOutputTypeDef, _OptionalDataSourceConfigOutputTypeDef
-):
-    pass
-
-
-_RequiredDataSourceConfigTypeDef = TypedDict(
-    "_RequiredDataSourceConfigTypeDef",
-    {
-        "name": str,
-        "s3Bucket": str,
-        "s3Keys": Sequence[str],
-    },
-)
-_OptionalDataSourceConfigTypeDef = TypedDict(
-    "_OptionalDataSourceConfigTypeDef",
-    {
-        "type": DataSourceTypeType,
-        "destination": str,
-    },
-    total=False,
-)
-
-
-class DataSourceConfigTypeDef(_RequiredDataSourceConfigTypeDef, _OptionalDataSourceConfigTypeDef):
-    pass
-
-
 LoggingConfigTypeDef = TypedDict(
     "LoggingConfigTypeDef",
     {
         "recordAllRosTopics": bool,
     },
     total=False,
 )
@@ -569,14 +529,60 @@
     "TemplateLocationTypeDef",
     {
         "s3Bucket": str,
         "s3Key": str,
     },
 )
 
+_RequiredDataSourceConfigOutputTypeDef = TypedDict(
+    "_RequiredDataSourceConfigOutputTypeDef",
+    {
+        "name": str,
+        "s3Bucket": str,
+        "s3Keys": List[str],
+    },
+)
+_OptionalDataSourceConfigOutputTypeDef = TypedDict(
+    "_OptionalDataSourceConfigOutputTypeDef",
+    {
+        "type": DataSourceTypeType,
+        "destination": str,
+    },
+    total=False,
+)
+
+
+class DataSourceConfigOutputTypeDef(
+    _RequiredDataSourceConfigOutputTypeDef, _OptionalDataSourceConfigOutputTypeDef
+):
+    pass
+
+
+_RequiredDataSourceConfigTypeDef = TypedDict(
+    "_RequiredDataSourceConfigTypeDef",
+    {
+        "name": str,
+        "s3Bucket": str,
+        "s3Keys": Sequence[str],
+    },
+)
+_OptionalDataSourceConfigTypeDef = TypedDict(
+    "_OptionalDataSourceConfigTypeDef",
+    {
+        "type": DataSourceTypeType,
+        "destination": str,
+    },
+    total=False,
+)
+
+
+class DataSourceConfigTypeDef(_RequiredDataSourceConfigTypeDef, _OptionalDataSourceConfigTypeDef):
+    pass
+
+
 S3KeyOutputTypeDef = TypedDict(
     "S3KeyOutputTypeDef",
     {
         "s3Key": str,
         "etag": str,
     },
     total=False,
@@ -1656,14 +1662,15 @@
 class UpdateWorldTemplateRequestRequestTypeDef(
     _RequiredUpdateWorldTemplateRequestRequestTypeDef,
     _OptionalUpdateWorldTemplateRequestRequestTypeDef,
 ):
     pass
 
 
+DataSourceConfigUnionTypeDef = Union[DataSourceConfigTypeDef, DataSourceConfigOutputTypeDef]
 DataSourceTypeDef = TypedDict(
     "DataSourceTypeDef",
     {
         "name": str,
         "s3Bucket": str,
         "s3Keys": List[S3KeyOutputTypeDef],
         "type": DataSourceTypeType,
@@ -2007,14 +2014,15 @@
         "progressDetail": ProgressDetailTypeDef,
         "failureReason": str,
         "failureCode": DeploymentJobErrorCodeType,
     },
     total=False,
 )
 
+VPCConfigUnionTypeDef = Union[VPCConfigTypeDef, VPCConfigOutputTypeDef]
 ListRobotApplicationsResponseTypeDef = TypedDict(
     "ListRobotApplicationsResponseTypeDef",
     {
         "robotApplicationSummaries": List[RobotApplicationSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2043,41 +2051,17 @@
     {
         "worldGenerationJobSummaries": List[WorldGenerationJobSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateDeploymentJobRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateDeploymentJobRequestRequestTypeDef",
-    {
-        "clientRequestToken": str,
-        "fleet": str,
-        "deploymentApplicationConfigs": Sequence[
-            Union[DeploymentApplicationConfigTypeDef, DeploymentApplicationConfigOutputTypeDef]
-        ],
-    },
-)
-_OptionalCreateDeploymentJobRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateDeploymentJobRequestRequestTypeDef",
-    {
-        "deploymentConfig": DeploymentConfigTypeDef,
-        "tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-
-class CreateDeploymentJobRequestRequestTypeDef(
-    _RequiredCreateDeploymentJobRequestRequestTypeDef,
-    _OptionalCreateDeploymentJobRequestRequestTypeDef,
-):
-    pass
-
-
+DeploymentApplicationConfigUnionTypeDef = Union[
+    DeploymentApplicationConfigTypeDef, DeploymentApplicationConfigOutputTypeDef
+]
 CreateDeploymentJobResponseTypeDef = TypedDict(
     "CreateDeploymentJobResponseTypeDef",
     {
         "arn": str,
         "fleet": str,
         "status": DeploymentStatusType,
         "deploymentApplicationConfigs": List[DeploymentApplicationConfigOutputTypeDef],
@@ -2169,14 +2153,39 @@
         "createdAt": datetime,
         "robotDeploymentSummary": List[RobotDeploymentTypeDef],
         "tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredCreateDeploymentJobRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateDeploymentJobRequestRequestTypeDef",
+    {
+        "clientRequestToken": str,
+        "fleet": str,
+        "deploymentApplicationConfigs": Sequence[DeploymentApplicationConfigUnionTypeDef],
+    },
+)
+_OptionalCreateDeploymentJobRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateDeploymentJobRequestRequestTypeDef",
+    {
+        "deploymentConfig": DeploymentConfigTypeDef,
+        "tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+
+class CreateDeploymentJobRequestRequestTypeDef(
+    _RequiredCreateDeploymentJobRequestRequestTypeDef,
+    _OptionalCreateDeploymentJobRequestRequestTypeDef,
+):
+    pass
+
+
 ListDeploymentJobsResponseTypeDef = TypedDict(
     "ListDeploymentJobsResponseTypeDef",
     {
         "deploymentJobs": List[DeploymentJobTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2415,50 +2424,20 @@
         "vpcConfig": VPCConfigResponseTypeDef,
         "networkInterface": NetworkInterfaceTypeDef,
         "compute": ComputeResponseTypeDef,
     },
     total=False,
 )
 
-_RequiredCreateSimulationJobRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateSimulationJobRequestRequestTypeDef",
-    {
-        "maxJobDurationInSeconds": int,
-        "iamRole": str,
-    },
-)
-_OptionalCreateSimulationJobRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateSimulationJobRequestRequestTypeDef",
-    {
-        "clientRequestToken": str,
-        "outputLocation": OutputLocationTypeDef,
-        "loggingConfig": LoggingConfigTypeDef,
-        "failureBehavior": FailureBehaviorType,
-        "robotApplications": Sequence[
-            Union[RobotApplicationConfigTypeDef, RobotApplicationConfigOutputTypeDef]
-        ],
-        "simulationApplications": Sequence[
-            Union[SimulationApplicationConfigTypeDef, SimulationApplicationConfigOutputTypeDef]
-        ],
-        "dataSources": Sequence[Union[DataSourceConfigTypeDef, DataSourceConfigOutputTypeDef]],
-        "tags": Mapping[str, str],
-        "vpcConfig": VPCConfigTypeDef,
-        "compute": ComputeTypeDef,
-    },
-    total=False,
-)
-
-
-class CreateSimulationJobRequestRequestTypeDef(
-    _RequiredCreateSimulationJobRequestRequestTypeDef,
-    _OptionalCreateSimulationJobRequestRequestTypeDef,
-):
-    pass
-
-
+RobotApplicationConfigUnionTypeDef = Union[
+    RobotApplicationConfigTypeDef, RobotApplicationConfigOutputTypeDef
+]
+SimulationApplicationConfigUnionTypeDef = Union[
+    SimulationApplicationConfigTypeDef, SimulationApplicationConfigOutputTypeDef
+]
 _RequiredSimulationJobRequestTypeDef = TypedDict(
     "_RequiredSimulationJobRequestTypeDef",
     {
         "maxJobDurationInSeconds": int,
     },
 )
 _OptionalSimulationJobRequestTypeDef = TypedDict(
@@ -2502,40 +2481,49 @@
     {
         "jobs": List[SimulationJobTypeDef],
         "unprocessedJobs": List[str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredStartSimulationJobBatchRequestRequestTypeDef = TypedDict(
-    "_RequiredStartSimulationJobBatchRequestRequestTypeDef",
+_RequiredCreateSimulationJobRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateSimulationJobRequestRequestTypeDef",
     {
-        "createSimulationJobRequests": Sequence[
-            Union[SimulationJobRequestTypeDef, SimulationJobRequestOutputTypeDef]
-        ],
+        "maxJobDurationInSeconds": int,
+        "iamRole": str,
     },
 )
-_OptionalStartSimulationJobBatchRequestRequestTypeDef = TypedDict(
-    "_OptionalStartSimulationJobBatchRequestRequestTypeDef",
+_OptionalCreateSimulationJobRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateSimulationJobRequestRequestTypeDef",
     {
         "clientRequestToken": str,
-        "batchPolicy": BatchPolicyTypeDef,
+        "outputLocation": OutputLocationTypeDef,
+        "loggingConfig": LoggingConfigTypeDef,
+        "failureBehavior": FailureBehaviorType,
+        "robotApplications": Sequence[RobotApplicationConfigUnionTypeDef],
+        "simulationApplications": Sequence[SimulationApplicationConfigUnionTypeDef],
+        "dataSources": Sequence[DataSourceConfigUnionTypeDef],
         "tags": Mapping[str, str],
+        "vpcConfig": VPCConfigTypeDef,
+        "compute": ComputeTypeDef,
     },
     total=False,
 )
 
 
-class StartSimulationJobBatchRequestRequestTypeDef(
-    _RequiredStartSimulationJobBatchRequestRequestTypeDef,
-    _OptionalStartSimulationJobBatchRequestRequestTypeDef,
+class CreateSimulationJobRequestRequestTypeDef(
+    _RequiredCreateSimulationJobRequestRequestTypeDef,
+    _OptionalCreateSimulationJobRequestRequestTypeDef,
 ):
     pass
 
 
+SimulationJobRequestUnionTypeDef = Union[
+    SimulationJobRequestTypeDef, SimulationJobRequestOutputTypeDef
+]
 DescribeSimulationJobBatchResponseTypeDef = TypedDict(
     "DescribeSimulationJobBatchResponseTypeDef",
     {
         "arn": str,
         "status": SimulationJobBatchStatusType,
         "lastUpdatedAt": datetime,
         "createdAt": datetime,
@@ -2564,7 +2552,30 @@
         "failedRequests": List[FailedCreateSimulationJobRequestTypeDef],
         "pendingRequests": List[SimulationJobRequestOutputTypeDef],
         "createdRequests": List[SimulationJobSummaryTypeDef],
         "tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+
+_RequiredStartSimulationJobBatchRequestRequestTypeDef = TypedDict(
+    "_RequiredStartSimulationJobBatchRequestRequestTypeDef",
+    {
+        "createSimulationJobRequests": Sequence[SimulationJobRequestUnionTypeDef],
+    },
+)
+_OptionalStartSimulationJobBatchRequestRequestTypeDef = TypedDict(
+    "_OptionalStartSimulationJobBatchRequestRequestTypeDef",
+    {
+        "clientRequestToken": str,
+        "batchPolicy": BatchPolicyTypeDef,
+        "tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+
+class StartSimulationJobBatchRequestRequestTypeDef(
+    _RequiredStartSimulationJobBatchRequestRequestTypeDef,
+    _OptionalStartSimulationJobBatchRequestRequestTypeDef,
+):
+    pass
```

### Comparing `mypy-boto3-robomaker-1.28.15.post1/mypy_boto3_robomaker/type_defs.pyi` & `mypy-boto3-robomaker-1.28.16/mypy_boto3_robomaker/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_robomaker.type_defs import BatchDeleteWorldsRequestRequestTypeDef
 
-    data: BatchDeleteWorldsRequestRequestTypeDef = {...}
+    data: BatchDeleteWorldsRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -65,22 +65,22 @@
     "SourceConfigTypeDef",
     "SourceTypeDef",
     "CreateRobotApplicationVersionRequestRequestTypeDef",
     "CreateRobotRequestRequestTypeDef",
     "RenderingEngineTypeDef",
     "SimulationSoftwareSuiteTypeDef",
     "CreateSimulationApplicationVersionRequestRequestTypeDef",
-    "DataSourceConfigOutputTypeDef",
-    "DataSourceConfigTypeDef",
     "LoggingConfigTypeDef",
     "OutputLocationTypeDef",
     "VPCConfigTypeDef",
     "VPCConfigResponseTypeDef",
     "WorldCountTypeDef",
     "TemplateLocationTypeDef",
+    "DataSourceConfigOutputTypeDef",
+    "DataSourceConfigTypeDef",
     "S3KeyOutputTypeDef",
     "DeleteFleetRequestRequestTypeDef",
     "DeleteRobotApplicationRequestRequestTypeDef",
     "DeleteRobotRequestRequestTypeDef",
     "DeleteSimulationApplicationRequestRequestTypeDef",
     "DeleteWorldTemplateRequestRequestTypeDef",
     "DeploymentLaunchConfigOutputTypeDef",
@@ -153,14 +153,15 @@
     "DescribeWorldExportJobResponseTypeDef",
     "WorldExportJobSummaryTypeDef",
     "CreateWorldGenerationJobRequestRequestTypeDef",
     "CreateWorldGenerationJobResponseTypeDef",
     "WorldGenerationJobSummaryTypeDef",
     "CreateWorldTemplateRequestRequestTypeDef",
     "UpdateWorldTemplateRequestRequestTypeDef",
+    "DataSourceConfigUnionTypeDef",
     "DataSourceTypeDef",
     "DeploymentApplicationConfigOutputTypeDef",
     "DeploymentApplicationConfigTypeDef",
     "DeploymentConfigTypeDef",
     "DescribeFleetResponseTypeDef",
     "ListRobotsResponseTypeDef",
     "ListSimulationJobsResponseTypeDef",
@@ -189,43 +190,48 @@
     "ListWorldsRequestListWorldsPaginateTypeDef",
     "ListSimulationJobBatchesResponseTypeDef",
     "ListWorldTemplatesResponseTypeDef",
     "ListWorldsResponseTypeDef",
     "PortForwardingConfigOutputTypeDef",
     "PortForwardingConfigTypeDef",
     "RobotDeploymentTypeDef",
+    "VPCConfigUnionTypeDef",
     "ListRobotApplicationsResponseTypeDef",
     "ListSimulationApplicationsResponseTypeDef",
     "ListWorldExportJobsResponseTypeDef",
     "ListWorldGenerationJobsResponseTypeDef",
-    "CreateDeploymentJobRequestRequestTypeDef",
+    "DeploymentApplicationConfigUnionTypeDef",
     "CreateDeploymentJobResponseTypeDef",
     "DeploymentJobTypeDef",
     "SyncDeploymentJobResponseTypeDef",
     "FinishedWorldsSummaryTypeDef",
     "LaunchConfigOutputTypeDef",
     "LaunchConfigTypeDef",
     "DescribeDeploymentJobResponseTypeDef",
+    "CreateDeploymentJobRequestRequestTypeDef",
     "ListDeploymentJobsResponseTypeDef",
     "DescribeWorldGenerationJobResponseTypeDef",
     "RobotApplicationConfigOutputTypeDef",
     "SimulationApplicationConfigOutputTypeDef",
     "RobotApplicationConfigTypeDef",
     "SimulationApplicationConfigTypeDef",
     "CreateSimulationJobResponseTypeDef",
     "DescribeSimulationJobResponseTypeDef",
     "SimulationJobRequestOutputTypeDef",
     "SimulationJobTypeDef",
-    "CreateSimulationJobRequestRequestTypeDef",
+    "RobotApplicationConfigUnionTypeDef",
+    "SimulationApplicationConfigUnionTypeDef",
     "SimulationJobRequestTypeDef",
     "FailedCreateSimulationJobRequestTypeDef",
     "BatchDescribeSimulationJobResponseTypeDef",
-    "StartSimulationJobBatchRequestRequestTypeDef",
+    "CreateSimulationJobRequestRequestTypeDef",
+    "SimulationJobRequestUnionTypeDef",
     "DescribeSimulationJobBatchResponseTypeDef",
     "StartSimulationJobBatchResponseTypeDef",
+    "StartSimulationJobBatchRequestRequestTypeDef",
 )
 
 BatchDeleteWorldsRequestRequestTypeDef = TypedDict(
     "BatchDeleteWorldsRequestRequestTypeDef",
     {
         "worlds": Sequence[str],
     },
@@ -449,56 +455,14 @@
 
 class CreateSimulationApplicationVersionRequestRequestTypeDef(
     _RequiredCreateSimulationApplicationVersionRequestRequestTypeDef,
     _OptionalCreateSimulationApplicationVersionRequestRequestTypeDef,
 ):
     pass
 
-_RequiredDataSourceConfigOutputTypeDef = TypedDict(
-    "_RequiredDataSourceConfigOutputTypeDef",
-    {
-        "name": str,
-        "s3Bucket": str,
-        "s3Keys": List[str],
-    },
-)
-_OptionalDataSourceConfigOutputTypeDef = TypedDict(
-    "_OptionalDataSourceConfigOutputTypeDef",
-    {
-        "type": DataSourceTypeType,
-        "destination": str,
-    },
-    total=False,
-)
-
-class DataSourceConfigOutputTypeDef(
-    _RequiredDataSourceConfigOutputTypeDef, _OptionalDataSourceConfigOutputTypeDef
-):
-    pass
-
-_RequiredDataSourceConfigTypeDef = TypedDict(
-    "_RequiredDataSourceConfigTypeDef",
-    {
-        "name": str,
-        "s3Bucket": str,
-        "s3Keys": Sequence[str],
-    },
-)
-_OptionalDataSourceConfigTypeDef = TypedDict(
-    "_OptionalDataSourceConfigTypeDef",
-    {
-        "type": DataSourceTypeType,
-        "destination": str,
-    },
-    total=False,
-)
-
-class DataSourceConfigTypeDef(_RequiredDataSourceConfigTypeDef, _OptionalDataSourceConfigTypeDef):
-    pass
-
 LoggingConfigTypeDef = TypedDict(
     "LoggingConfigTypeDef",
     {
         "recordAllRosTopics": bool,
     },
     total=False,
 )
@@ -554,14 +518,56 @@
     "TemplateLocationTypeDef",
     {
         "s3Bucket": str,
         "s3Key": str,
     },
 )
 
+_RequiredDataSourceConfigOutputTypeDef = TypedDict(
+    "_RequiredDataSourceConfigOutputTypeDef",
+    {
+        "name": str,
+        "s3Bucket": str,
+        "s3Keys": List[str],
+    },
+)
+_OptionalDataSourceConfigOutputTypeDef = TypedDict(
+    "_OptionalDataSourceConfigOutputTypeDef",
+    {
+        "type": DataSourceTypeType,
+        "destination": str,
+    },
+    total=False,
+)
+
+class DataSourceConfigOutputTypeDef(
+    _RequiredDataSourceConfigOutputTypeDef, _OptionalDataSourceConfigOutputTypeDef
+):
+    pass
+
+_RequiredDataSourceConfigTypeDef = TypedDict(
+    "_RequiredDataSourceConfigTypeDef",
+    {
+        "name": str,
+        "s3Bucket": str,
+        "s3Keys": Sequence[str],
+    },
+)
+_OptionalDataSourceConfigTypeDef = TypedDict(
+    "_OptionalDataSourceConfigTypeDef",
+    {
+        "type": DataSourceTypeType,
+        "destination": str,
+    },
+    total=False,
+)
+
+class DataSourceConfigTypeDef(_RequiredDataSourceConfigTypeDef, _OptionalDataSourceConfigTypeDef):
+    pass
+
 S3KeyOutputTypeDef = TypedDict(
     "S3KeyOutputTypeDef",
     {
         "s3Key": str,
         "etag": str,
     },
     total=False,
@@ -1607,14 +1613,15 @@
 
 class UpdateWorldTemplateRequestRequestTypeDef(
     _RequiredUpdateWorldTemplateRequestRequestTypeDef,
     _OptionalUpdateWorldTemplateRequestRequestTypeDef,
 ):
     pass
 
+DataSourceConfigUnionTypeDef = Union[DataSourceConfigTypeDef, DataSourceConfigOutputTypeDef]
 DataSourceTypeDef = TypedDict(
     "DataSourceTypeDef",
     {
         "name": str,
         "s3Bucket": str,
         "s3Keys": List[S3KeyOutputTypeDef],
         "type": DataSourceTypeType,
@@ -1958,14 +1965,15 @@
         "progressDetail": ProgressDetailTypeDef,
         "failureReason": str,
         "failureCode": DeploymentJobErrorCodeType,
     },
     total=False,
 )
 
+VPCConfigUnionTypeDef = Union[VPCConfigTypeDef, VPCConfigOutputTypeDef]
 ListRobotApplicationsResponseTypeDef = TypedDict(
     "ListRobotApplicationsResponseTypeDef",
     {
         "robotApplicationSummaries": List[RobotApplicationSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1994,39 +2002,17 @@
     {
         "worldGenerationJobSummaries": List[WorldGenerationJobSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateDeploymentJobRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateDeploymentJobRequestRequestTypeDef",
-    {
-        "clientRequestToken": str,
-        "fleet": str,
-        "deploymentApplicationConfigs": Sequence[
-            Union[DeploymentApplicationConfigTypeDef, DeploymentApplicationConfigOutputTypeDef]
-        ],
-    },
-)
-_OptionalCreateDeploymentJobRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateDeploymentJobRequestRequestTypeDef",
-    {
-        "deploymentConfig": DeploymentConfigTypeDef,
-        "tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-class CreateDeploymentJobRequestRequestTypeDef(
-    _RequiredCreateDeploymentJobRequestRequestTypeDef,
-    _OptionalCreateDeploymentJobRequestRequestTypeDef,
-):
-    pass
-
+DeploymentApplicationConfigUnionTypeDef = Union[
+    DeploymentApplicationConfigTypeDef, DeploymentApplicationConfigOutputTypeDef
+]
 CreateDeploymentJobResponseTypeDef = TypedDict(
     "CreateDeploymentJobResponseTypeDef",
     {
         "arn": str,
         "fleet": str,
         "status": DeploymentStatusType,
         "deploymentApplicationConfigs": List[DeploymentApplicationConfigOutputTypeDef],
@@ -2118,14 +2104,37 @@
         "createdAt": datetime,
         "robotDeploymentSummary": List[RobotDeploymentTypeDef],
         "tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredCreateDeploymentJobRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateDeploymentJobRequestRequestTypeDef",
+    {
+        "clientRequestToken": str,
+        "fleet": str,
+        "deploymentApplicationConfigs": Sequence[DeploymentApplicationConfigUnionTypeDef],
+    },
+)
+_OptionalCreateDeploymentJobRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateDeploymentJobRequestRequestTypeDef",
+    {
+        "deploymentConfig": DeploymentConfigTypeDef,
+        "tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+class CreateDeploymentJobRequestRequestTypeDef(
+    _RequiredCreateDeploymentJobRequestRequestTypeDef,
+    _OptionalCreateDeploymentJobRequestRequestTypeDef,
+):
+    pass
+
 ListDeploymentJobsResponseTypeDef = TypedDict(
     "ListDeploymentJobsResponseTypeDef",
     {
         "deploymentJobs": List[DeploymentJobTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2354,48 +2363,20 @@
         "vpcConfig": VPCConfigResponseTypeDef,
         "networkInterface": NetworkInterfaceTypeDef,
         "compute": ComputeResponseTypeDef,
     },
     total=False,
 )
 
-_RequiredCreateSimulationJobRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateSimulationJobRequestRequestTypeDef",
-    {
-        "maxJobDurationInSeconds": int,
-        "iamRole": str,
-    },
-)
-_OptionalCreateSimulationJobRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateSimulationJobRequestRequestTypeDef",
-    {
-        "clientRequestToken": str,
-        "outputLocation": OutputLocationTypeDef,
-        "loggingConfig": LoggingConfigTypeDef,
-        "failureBehavior": FailureBehaviorType,
-        "robotApplications": Sequence[
-            Union[RobotApplicationConfigTypeDef, RobotApplicationConfigOutputTypeDef]
-        ],
-        "simulationApplications": Sequence[
-            Union[SimulationApplicationConfigTypeDef, SimulationApplicationConfigOutputTypeDef]
-        ],
-        "dataSources": Sequence[Union[DataSourceConfigTypeDef, DataSourceConfigOutputTypeDef]],
-        "tags": Mapping[str, str],
-        "vpcConfig": VPCConfigTypeDef,
-        "compute": ComputeTypeDef,
-    },
-    total=False,
-)
-
-class CreateSimulationJobRequestRequestTypeDef(
-    _RequiredCreateSimulationJobRequestRequestTypeDef,
-    _OptionalCreateSimulationJobRequestRequestTypeDef,
-):
-    pass
-
+RobotApplicationConfigUnionTypeDef = Union[
+    RobotApplicationConfigTypeDef, RobotApplicationConfigOutputTypeDef
+]
+SimulationApplicationConfigUnionTypeDef = Union[
+    SimulationApplicationConfigTypeDef, SimulationApplicationConfigOutputTypeDef
+]
 _RequiredSimulationJobRequestTypeDef = TypedDict(
     "_RequiredSimulationJobRequestTypeDef",
     {
         "maxJobDurationInSeconds": int,
     },
 )
 _OptionalSimulationJobRequestTypeDef = TypedDict(
@@ -2437,38 +2418,47 @@
     {
         "jobs": List[SimulationJobTypeDef],
         "unprocessedJobs": List[str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredStartSimulationJobBatchRequestRequestTypeDef = TypedDict(
-    "_RequiredStartSimulationJobBatchRequestRequestTypeDef",
+_RequiredCreateSimulationJobRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateSimulationJobRequestRequestTypeDef",
     {
-        "createSimulationJobRequests": Sequence[
-            Union[SimulationJobRequestTypeDef, SimulationJobRequestOutputTypeDef]
-        ],
+        "maxJobDurationInSeconds": int,
+        "iamRole": str,
     },
 )
-_OptionalStartSimulationJobBatchRequestRequestTypeDef = TypedDict(
-    "_OptionalStartSimulationJobBatchRequestRequestTypeDef",
+_OptionalCreateSimulationJobRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateSimulationJobRequestRequestTypeDef",
     {
         "clientRequestToken": str,
-        "batchPolicy": BatchPolicyTypeDef,
+        "outputLocation": OutputLocationTypeDef,
+        "loggingConfig": LoggingConfigTypeDef,
+        "failureBehavior": FailureBehaviorType,
+        "robotApplications": Sequence[RobotApplicationConfigUnionTypeDef],
+        "simulationApplications": Sequence[SimulationApplicationConfigUnionTypeDef],
+        "dataSources": Sequence[DataSourceConfigUnionTypeDef],
         "tags": Mapping[str, str],
+        "vpcConfig": VPCConfigTypeDef,
+        "compute": ComputeTypeDef,
     },
     total=False,
 )
 
-class StartSimulationJobBatchRequestRequestTypeDef(
-    _RequiredStartSimulationJobBatchRequestRequestTypeDef,
-    _OptionalStartSimulationJobBatchRequestRequestTypeDef,
+class CreateSimulationJobRequestRequestTypeDef(
+    _RequiredCreateSimulationJobRequestRequestTypeDef,
+    _OptionalCreateSimulationJobRequestRequestTypeDef,
 ):
     pass
 
+SimulationJobRequestUnionTypeDef = Union[
+    SimulationJobRequestTypeDef, SimulationJobRequestOutputTypeDef
+]
 DescribeSimulationJobBatchResponseTypeDef = TypedDict(
     "DescribeSimulationJobBatchResponseTypeDef",
     {
         "arn": str,
         "status": SimulationJobBatchStatusType,
         "lastUpdatedAt": datetime,
         "createdAt": datetime,
@@ -2497,7 +2487,29 @@
         "failedRequests": List[FailedCreateSimulationJobRequestTypeDef],
         "pendingRequests": List[SimulationJobRequestOutputTypeDef],
         "createdRequests": List[SimulationJobSummaryTypeDef],
         "tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+
+_RequiredStartSimulationJobBatchRequestRequestTypeDef = TypedDict(
+    "_RequiredStartSimulationJobBatchRequestRequestTypeDef",
+    {
+        "createSimulationJobRequests": Sequence[SimulationJobRequestUnionTypeDef],
+    },
+)
+_OptionalStartSimulationJobBatchRequestRequestTypeDef = TypedDict(
+    "_OptionalStartSimulationJobBatchRequestRequestTypeDef",
+    {
+        "clientRequestToken": str,
+        "batchPolicy": BatchPolicyTypeDef,
+        "tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+class StartSimulationJobBatchRequestRequestTypeDef(
+    _RequiredStartSimulationJobBatchRequestRequestTypeDef,
+    _OptionalStartSimulationJobBatchRequestRequestTypeDef,
+):
+    pass
```

### Comparing `mypy-boto3-robomaker-1.28.15.post1/mypy_boto3_robomaker.egg-info/PKG-INFO` & `mypy-boto3-robomaker-1.28.16/mypy_boto3_robomaker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-robomaker
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.RoboMaker 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.RoboMaker 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 robomaker type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 robomaker type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-robomaker.svg?color=blue)](https://pypi.org/project/mypy-boto3-robomaker)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-robomaker)](https://pepy.tech/project/mypy-boto3-robomaker)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.RoboMaker 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker)
+[boto3.RoboMaker 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker)
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
 [mypy-boto3-robomaker docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/).
 
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
@@ -379,20 +379,20 @@
 )
 
 
 def check_value(value: ArchitectureType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_robomaker.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_robomaker.type_defs import (
     BatchDeleteWorldsRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     BatchDescribeSimulationJobRequestRequestTypeDef,
     BatchPolicyTypeDef,
@@ -409,22 +409,22 @@
     SourceConfigTypeDef,
     SourceTypeDef,
     CreateRobotApplicationVersionRequestRequestTypeDef,
     CreateRobotRequestRequestTypeDef,
     RenderingEngineTypeDef,
     SimulationSoftwareSuiteTypeDef,
     CreateSimulationApplicationVersionRequestRequestTypeDef,
-    DataSourceConfigOutputTypeDef,
-    DataSourceConfigTypeDef,
     LoggingConfigTypeDef,
     OutputLocationTypeDef,
     VPCConfigTypeDef,
     VPCConfigResponseTypeDef,
     WorldCountTypeDef,
     TemplateLocationTypeDef,
+    DataSourceConfigOutputTypeDef,
+    DataSourceConfigTypeDef,
     S3KeyOutputTypeDef,
     DeleteFleetRequestRequestTypeDef,
     DeleteRobotApplicationRequestRequestTypeDef,
     DeleteRobotRequestRequestTypeDef,
     DeleteSimulationApplicationRequestRequestTypeDef,
     DeleteWorldTemplateRequestRequestTypeDef,
     DeploymentLaunchConfigOutputTypeDef,
@@ -497,14 +497,15 @@
     DescribeWorldExportJobResponseTypeDef,
     WorldExportJobSummaryTypeDef,
     CreateWorldGenerationJobRequestRequestTypeDef,
     CreateWorldGenerationJobResponseTypeDef,
     WorldGenerationJobSummaryTypeDef,
     CreateWorldTemplateRequestRequestTypeDef,
     UpdateWorldTemplateRequestRequestTypeDef,
+    DataSourceConfigUnionTypeDef,
     DataSourceTypeDef,
     DeploymentApplicationConfigOutputTypeDef,
     DeploymentApplicationConfigTypeDef,
     DeploymentConfigTypeDef,
     DescribeFleetResponseTypeDef,
     ListRobotsResponseTypeDef,
     ListSimulationJobsResponseTypeDef,
@@ -533,47 +534,52 @@
     ListWorldsRequestListWorldsPaginateTypeDef,
     ListSimulationJobBatchesResponseTypeDef,
     ListWorldTemplatesResponseTypeDef,
     ListWorldsResponseTypeDef,
     PortForwardingConfigOutputTypeDef,
     PortForwardingConfigTypeDef,
     RobotDeploymentTypeDef,
+    VPCConfigUnionTypeDef,
     ListRobotApplicationsResponseTypeDef,
     ListSimulationApplicationsResponseTypeDef,
     ListWorldExportJobsResponseTypeDef,
     ListWorldGenerationJobsResponseTypeDef,
-    CreateDeploymentJobRequestRequestTypeDef,
+    DeploymentApplicationConfigUnionTypeDef,
     CreateDeploymentJobResponseTypeDef,
     DeploymentJobTypeDef,
     SyncDeploymentJobResponseTypeDef,
     FinishedWorldsSummaryTypeDef,
     LaunchConfigOutputTypeDef,
     LaunchConfigTypeDef,
     DescribeDeploymentJobResponseTypeDef,
+    CreateDeploymentJobRequestRequestTypeDef,
     ListDeploymentJobsResponseTypeDef,
     DescribeWorldGenerationJobResponseTypeDef,
     RobotApplicationConfigOutputTypeDef,
     SimulationApplicationConfigOutputTypeDef,
     RobotApplicationConfigTypeDef,
     SimulationApplicationConfigTypeDef,
     CreateSimulationJobResponseTypeDef,
     DescribeSimulationJobResponseTypeDef,
     SimulationJobRequestOutputTypeDef,
     SimulationJobTypeDef,
-    CreateSimulationJobRequestRequestTypeDef,
+    RobotApplicationConfigUnionTypeDef,
+    SimulationApplicationConfigUnionTypeDef,
     SimulationJobRequestTypeDef,
     FailedCreateSimulationJobRequestTypeDef,
     BatchDescribeSimulationJobResponseTypeDef,
-    StartSimulationJobBatchRequestRequestTypeDef,
+    CreateSimulationJobRequestRequestTypeDef,
+    SimulationJobRequestUnionTypeDef,
     DescribeSimulationJobBatchResponseTypeDef,
     StartSimulationJobBatchResponseTypeDef,
+    StartSimulationJobBatchRequestRequestTypeDef,
 )
 
 
-def get_structure() -> BatchDeleteWorldsRequestRequestTypeDef:
+def get_value() -> BatchDeleteWorldsRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-robomaker-1.28.15.post1/mypy_boto3_robomaker.egg-info/SOURCES.txt` & `mypy-boto3-robomaker-1.28.16/mypy_boto3_robomaker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-robomaker-1.28.15.post1/setup.py` & `mypy-boto3-robomaker-1.28.16/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-robomaker",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_robomaker"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.RoboMaker 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.2"
+        "Type annotations for boto3.RoboMaker 1.28.16 service generated with mypy-boto3-builder"
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
-    keywords="boto3 robomaker type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 robomaker type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_robomaker": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

