# Comparing `tmp/mypy-boto3-opsworks-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-opsworks-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-opsworks-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:48 2023, max compression
+gzip compressed data, was "mypy-boto3-opsworks-1.28.16.tar", last modified: Tue Aug  1 11:37:28 2023, max compression
```

## Comparing `mypy-boto3-opsworks-1.28.15.post1.tar` & `mypy-boto3-opsworks-1.28.16.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:48.437318 mypy-boto3-opsworks-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:52:36.000000 mypy-boto3-opsworks-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    22926 2023-07-29 10:03:48.433318 mypy-boto3-opsworks-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21429 2023-07-29 09:52:36.000000 mypy-boto3-opsworks-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:48.429318 mypy-boto3-opsworks-1.28.15.post1/mypy_boto3_opsworks/
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-07-29 09:52:36.000000 mypy-boto3-opsworks-1.28.15.post1/mypy_boto3_opsworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-29 09:52:36.000000 mypy-boto3-opsworks-1.28.15.post1/mypy_boto3_opsworks/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-29 09:52:36.000000 mypy-boto3-opsworks-1.28.15.post1/mypy_boto3_opsworks/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    52378 2023-07-29 09:52:37.000000 mypy-boto3-opsworks-1.28.15.post1/mypy_boto3_opsworks/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    52290 2023-07-29 09:52:36.000000 mypy-boto3-opsworks-1.28.15.post1/mypy_boto3_opsworks/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12515 2023-07-29 09:52:37.000000 mypy-boto3-opsworks-1.28.15.post1/mypy_boto3_opsworks/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12513 2023-07-29 09:52:37.000000 mypy-boto3-opsworks-1.28.15.post1/mypy_boto3_opsworks/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-29 09:52:37.000000 mypy-boto3-opsworks-1.28.15.post1/mypy_boto3_opsworks/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-07-29 09:52:37.000000 mypy-boto3-opsworks-1.28.15.post1/mypy_boto3_opsworks/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:52:36.000000 mypy-boto3-opsworks-1.28.15.post1/mypy_boto3_opsworks/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    19326 2023-07-29 09:52:37.000000 mypy-boto3-opsworks-1.28.15.post1/mypy_boto3_opsworks/service_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    19290 2023-07-29 09:52:37.000000 mypy-boto3-opsworks-1.28.15.post1/mypy_boto3_opsworks/service_resource.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    65372 2023-07-29 09:52:39.000000 mypy-boto3-opsworks-1.28.15.post1/mypy_boto3_opsworks/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    65303 2023-07-29 09:52:38.000000 mypy-boto3-opsworks-1.28.15.post1/mypy_boto3_opsworks/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:52:36.000000 mypy-boto3-opsworks-1.28.15.post1/mypy_boto3_opsworks/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6633 2023-07-29 09:52:37.000000 mypy-boto3-opsworks-1.28.15.post1/mypy_boto3_opsworks/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6627 2023-07-29 09:52:37.000000 mypy-boto3-opsworks-1.28.15.post1/mypy_boto3_opsworks/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:48.433318 mypy-boto3-opsworks-1.28.15.post1/mypy_boto3_opsworks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22926 2023-07-29 10:03:48.000000 mypy-boto3-opsworks-1.28.15.post1/mypy_boto3_opsworks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-29 10:03:48.000000 mypy-boto3-opsworks-1.28.15.post1/mypy_boto3_opsworks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:48.000000 mypy-boto3-opsworks-1.28.15.post1/mypy_boto3_opsworks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:48.000000 mypy-boto3-opsworks-1.28.15.post1/mypy_boto3_opsworks.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:48.000000 mypy-boto3-opsworks-1.28.15.post1/mypy_boto3_opsworks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-29 10:03:48.000000 mypy-boto3-opsworks-1.28.15.post1/mypy_boto3_opsworks.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:48.437318 mypy-boto3-opsworks-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-07-29 09:52:36.000000 mypy-boto3-opsworks-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:28.380802 mypy-boto3-opsworks-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:25:34.000000 mypy-boto3-opsworks-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    23103 2023-08-01 11:37:28.380802 mypy-boto3-opsworks-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21615 2023-08-01 11:25:34.000000 mypy-boto3-opsworks-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:28.380802 mypy-boto3-opsworks-1.28.16/mypy_boto3_opsworks/
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-08-01 11:25:34.000000 mypy-boto3-opsworks-1.28.16/mypy_boto3_opsworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-08-01 11:25:34.000000 mypy-boto3-opsworks-1.28.16/mypy_boto3_opsworks/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-08-01 11:25:34.000000 mypy-boto3-opsworks-1.28.16/mypy_boto3_opsworks/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51826 2023-08-01 11:25:35.000000 mypy-boto3-opsworks-1.28.16/mypy_boto3_opsworks/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51738 2023-08-01 11:25:35.000000 mypy-boto3-opsworks-1.28.16/mypy_boto3_opsworks/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12515 2023-08-01 11:25:36.000000 mypy-boto3-opsworks-1.28.16/mypy_boto3_opsworks/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12513 2023-08-01 11:25:35.000000 mypy-boto3-opsworks-1.28.16/mypy_boto3_opsworks/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-08-01 11:25:35.000000 mypy-boto3-opsworks-1.28.16/mypy_boto3_opsworks/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-08-01 11:25:35.000000 mypy-boto3-opsworks-1.28.16/mypy_boto3_opsworks/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:25:34.000000 mypy-boto3-opsworks-1.28.16/mypy_boto3_opsworks/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    19326 2023-08-01 11:25:35.000000 mypy-boto3-opsworks-1.28.16/mypy_boto3_opsworks/service_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19290 2023-08-01 11:25:35.000000 mypy-boto3-opsworks-1.28.16/mypy_boto3_opsworks/service_resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    66092 2023-08-01 11:25:40.000000 mypy-boto3-opsworks-1.28.16/mypy_boto3_opsworks/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66023 2023-08-01 11:25:36.000000 mypy-boto3-opsworks-1.28.16/mypy_boto3_opsworks/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:25:34.000000 mypy-boto3-opsworks-1.28.16/mypy_boto3_opsworks/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6633 2023-08-01 11:25:35.000000 mypy-boto3-opsworks-1.28.16/mypy_boto3_opsworks/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6627 2023-08-01 11:25:35.000000 mypy-boto3-opsworks-1.28.16/mypy_boto3_opsworks/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:28.380802 mypy-boto3-opsworks-1.28.16/mypy_boto3_opsworks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23103 2023-08-01 11:37:28.000000 mypy-boto3-opsworks-1.28.16/mypy_boto3_opsworks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-08-01 11:37:28.000000 mypy-boto3-opsworks-1.28.16/mypy_boto3_opsworks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:28.000000 mypy-boto3-opsworks-1.28.16/mypy_boto3_opsworks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:28.000000 mypy-boto3-opsworks-1.28.16/mypy_boto3_opsworks.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:28.000000 mypy-boto3-opsworks-1.28.16/mypy_boto3_opsworks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-01 11:37:28.000000 mypy-boto3-opsworks-1.28.16/mypy_boto3_opsworks.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:28.380802 mypy-boto3-opsworks-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-08-01 11:25:34.000000 mypy-boto3-opsworks-1.28.16/setup.py
```

### Comparing `mypy-boto3-opsworks-1.28.15.post1/LICENSE` & `mypy-boto3-opsworks-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opsworks-1.28.15.post1/PKG-INFO` & `mypy-boto3-opsworks-1.28.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-opsworks
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.OpsWorks 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.OpsWorks 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 opsworks type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 opsworks type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-opsworks.svg?color=blue)](https://pypi.org/project/mypy-boto3-opsworks)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-opsworks)](https://pepy.tech/project/mypy-boto3-opsworks)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.OpsWorks 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks)
+[boto3.OpsWorks 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks)
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
 [mypy-boto3-opsworks docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/).
 
 See how it helps to find and fix potential bugs:
 
@@ -78,15 +78,15 @@
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Waiters annotations](#waiters-annotations)
     - [Service Resource annotations](#service-resource-annotations)
     - [Other resources annotations](#other-resources-annotations)
     - [Collections annotations](#collections-annotations)
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
@@ -429,20 +429,20 @@
 )
 
 
 def check_value(value: AppAttributesKeysType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_opsworks.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_opsworks.type_defs import (
     StackConfigurationManagerTypeDef,
     DataSourceTypeDef,
     EnvironmentVariableTypeDef,
     SourceTypeDef,
@@ -455,15 +455,14 @@
     AutoScalingThresholdsTypeDef,
     EbsBlockDeviceTypeDef,
     ResponseMetadataTypeDef,
     ChefConfigurationTypeDef,
     CloudWatchLogsLogStreamTypeDef,
     CommandTypeDef,
     DeploymentCommandTypeDef,
-    RecipesTypeDef,
     VolumeConfigurationTypeDef,
     CreateUserProfileRequestRequestTypeDef,
     DeleteAppRequestRequestTypeDef,
     DeleteInstanceRequestRequestTypeDef,
     DeleteLayerRequestRequestTypeDef,
     DeleteStackRequestRequestTypeDef,
     DeleteUserProfileRequestRequestTypeDef,
@@ -540,14 +539,15 @@
     UpdateVolumeRequestRequestTypeDef,
     AgentVersionTypeDef,
     DescribeAgentVersionsRequestRequestTypeDef,
     AppTypeDef,
     CreateAppRequestRequestTypeDef,
     UpdateAppRequestRequestTypeDef,
     LoadBasedAutoScalingConfigurationTypeDef,
+    AutoScalingThresholdsUnionTypeDef,
     SetLoadBasedAutoScalingRequestRequestTypeDef,
     BlockDeviceMappingTypeDef,
     ChefConfigurationResponseTypeDef,
     CloneStackResultTypeDef,
     CreateAppResultTypeDef,
     CreateDeploymentResultTypeDef,
     CreateInstanceResultTypeDef,
@@ -555,14 +555,15 @@
     CreateStackResultTypeDef,
     CreateUserProfileResultTypeDef,
     DescribeStackProvisioningParametersResultTypeDef,
     EmptyResponseMetadataTypeDef,
     GetHostnameSuggestionResultTypeDef,
     InstancesCountResponseTypeDef,
     ListTagsResultTypeDef,
+    RecipesTypeDef,
     RegisterEcsClusterResultTypeDef,
     RegisterElasticIpResultTypeDef,
     RegisterInstanceResultTypeDef,
     RegisterVolumeResultTypeDef,
     SourceResponseTypeDef,
     StackConfigurationManagerResponseTypeDef,
     CloneStackRequestRequestTypeDef,
@@ -570,14 +571,15 @@
     CreateStackRequestServiceResourceCreateStackTypeDef,
     StackTypeDef,
     UpdateStackRequestRequestTypeDef,
     CloudWatchLogsConfigurationOutputTypeDef,
     CloudWatchLogsConfigurationTypeDef,
     DescribeCommandsResultTypeDef,
     CreateDeploymentRequestRequestTypeDef,
+    DeploymentCommandUnionTypeDef,
     DeploymentTypeDef,
     DescribeAppsRequestAppExistsWaitTypeDef,
     DescribeDeploymentsRequestDeploymentSuccessfulWaitTypeDef,
     DescribeInstancesRequestInstanceOnlineWaitTypeDef,
     DescribeInstancesRequestInstanceRegisteredWaitTypeDef,
     DescribeInstancesRequestInstanceStoppedWaitTypeDef,
     DescribeInstancesRequestInstanceTerminatedWaitTypeDef,
@@ -596,34 +598,37 @@
     RegisterInstanceRequestRequestTypeDef,
     StackSummaryTypeDef,
     LifecycleEventConfigurationResponseTypeDef,
     LifecycleEventConfigurationTypeDef,
     OperatingSystemTypeDef,
     SetTimeBasedAutoScalingRequestRequestTypeDef,
     TimeBasedAutoScalingConfigurationTypeDef,
+    WeeklyAutoScalingScheduleUnionTypeDef,
     DescribeAgentVersionsResultTypeDef,
     DescribeAppsResultTypeDef,
     DescribeLoadBasedAutoScalingResultTypeDef,
     CreateInstanceRequestRequestTypeDef,
     InstanceTypeDef,
+    RecipesUnionTypeDef,
     DescribeStacksResultTypeDef,
+    CloudWatchLogsConfigurationUnionTypeDef,
     DescribeDeploymentsResultTypeDef,
     DescribeStackSummaryResultTypeDef,
     CreateLayerRequestRequestTypeDef,
     CreateLayerRequestStackCreateLayerTypeDef,
     LayerTypeDef,
     UpdateLayerRequestRequestTypeDef,
     DescribeOperatingSystemsResponseTypeDef,
     DescribeTimeBasedAutoScalingResultTypeDef,
     DescribeInstancesResultTypeDef,
     DescribeLayersResultTypeDef,
 )
 
 
-def get_structure() -> StackConfigurationManagerTypeDef:
+def get_value() -> StackConfigurationManagerTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-opsworks-1.28.15.post1/README.md` & `mypy-boto3-opsworks-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-opsworks.svg?color=blue)](https://pypi.org/project/mypy-boto3-opsworks)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-opsworks)](https://pepy.tech/project/mypy-boto3-opsworks)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.OpsWorks 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks)
+[boto3.OpsWorks 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks)
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
 [mypy-boto3-opsworks docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/).
 
 See how it helps to find and fix potential bugs:
 
@@ -46,15 +46,15 @@
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Waiters annotations](#waiters-annotations)
     - [Service Resource annotations](#service-resource-annotations)
     - [Other resources annotations](#other-resources-annotations)
     - [Collections annotations](#collections-annotations)
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
@@ -397,20 +397,20 @@
 )
 
 
 def check_value(value: AppAttributesKeysType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_opsworks.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_opsworks.type_defs import (
     StackConfigurationManagerTypeDef,
     DataSourceTypeDef,
     EnvironmentVariableTypeDef,
     SourceTypeDef,
@@ -423,15 +423,14 @@
     AutoScalingThresholdsTypeDef,
     EbsBlockDeviceTypeDef,
     ResponseMetadataTypeDef,
     ChefConfigurationTypeDef,
     CloudWatchLogsLogStreamTypeDef,
     CommandTypeDef,
     DeploymentCommandTypeDef,
-    RecipesTypeDef,
     VolumeConfigurationTypeDef,
     CreateUserProfileRequestRequestTypeDef,
     DeleteAppRequestRequestTypeDef,
     DeleteInstanceRequestRequestTypeDef,
     DeleteLayerRequestRequestTypeDef,
     DeleteStackRequestRequestTypeDef,
     DeleteUserProfileRequestRequestTypeDef,
@@ -508,14 +507,15 @@
     UpdateVolumeRequestRequestTypeDef,
     AgentVersionTypeDef,
     DescribeAgentVersionsRequestRequestTypeDef,
     AppTypeDef,
     CreateAppRequestRequestTypeDef,
     UpdateAppRequestRequestTypeDef,
     LoadBasedAutoScalingConfigurationTypeDef,
+    AutoScalingThresholdsUnionTypeDef,
     SetLoadBasedAutoScalingRequestRequestTypeDef,
     BlockDeviceMappingTypeDef,
     ChefConfigurationResponseTypeDef,
     CloneStackResultTypeDef,
     CreateAppResultTypeDef,
     CreateDeploymentResultTypeDef,
     CreateInstanceResultTypeDef,
@@ -523,14 +523,15 @@
     CreateStackResultTypeDef,
     CreateUserProfileResultTypeDef,
     DescribeStackProvisioningParametersResultTypeDef,
     EmptyResponseMetadataTypeDef,
     GetHostnameSuggestionResultTypeDef,
     InstancesCountResponseTypeDef,
     ListTagsResultTypeDef,
+    RecipesTypeDef,
     RegisterEcsClusterResultTypeDef,
     RegisterElasticIpResultTypeDef,
     RegisterInstanceResultTypeDef,
     RegisterVolumeResultTypeDef,
     SourceResponseTypeDef,
     StackConfigurationManagerResponseTypeDef,
     CloneStackRequestRequestTypeDef,
@@ -538,14 +539,15 @@
     CreateStackRequestServiceResourceCreateStackTypeDef,
     StackTypeDef,
     UpdateStackRequestRequestTypeDef,
     CloudWatchLogsConfigurationOutputTypeDef,
     CloudWatchLogsConfigurationTypeDef,
     DescribeCommandsResultTypeDef,
     CreateDeploymentRequestRequestTypeDef,
+    DeploymentCommandUnionTypeDef,
     DeploymentTypeDef,
     DescribeAppsRequestAppExistsWaitTypeDef,
     DescribeDeploymentsRequestDeploymentSuccessfulWaitTypeDef,
     DescribeInstancesRequestInstanceOnlineWaitTypeDef,
     DescribeInstancesRequestInstanceRegisteredWaitTypeDef,
     DescribeInstancesRequestInstanceStoppedWaitTypeDef,
     DescribeInstancesRequestInstanceTerminatedWaitTypeDef,
@@ -564,34 +566,37 @@
     RegisterInstanceRequestRequestTypeDef,
     StackSummaryTypeDef,
     LifecycleEventConfigurationResponseTypeDef,
     LifecycleEventConfigurationTypeDef,
     OperatingSystemTypeDef,
     SetTimeBasedAutoScalingRequestRequestTypeDef,
     TimeBasedAutoScalingConfigurationTypeDef,
+    WeeklyAutoScalingScheduleUnionTypeDef,
     DescribeAgentVersionsResultTypeDef,
     DescribeAppsResultTypeDef,
     DescribeLoadBasedAutoScalingResultTypeDef,
     CreateInstanceRequestRequestTypeDef,
     InstanceTypeDef,
+    RecipesUnionTypeDef,
     DescribeStacksResultTypeDef,
+    CloudWatchLogsConfigurationUnionTypeDef,
     DescribeDeploymentsResultTypeDef,
     DescribeStackSummaryResultTypeDef,
     CreateLayerRequestRequestTypeDef,
     CreateLayerRequestStackCreateLayerTypeDef,
     LayerTypeDef,
     UpdateLayerRequestRequestTypeDef,
     DescribeOperatingSystemsResponseTypeDef,
     DescribeTimeBasedAutoScalingResultTypeDef,
     DescribeInstancesResultTypeDef,
     DescribeLayersResultTypeDef,
 )
 
 
-def get_structure() -> StackConfigurationManagerTypeDef:
+def get_value() -> StackConfigurationManagerTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-opsworks-1.28.15.post1/mypy_boto3_opsworks/__init__.py` & `mypy-boto3-opsworks-1.28.16/mypy_boto3_opsworks/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opsworks-1.28.15.post1/mypy_boto3_opsworks/__init__.pyi` & `mypy-boto3-opsworks-1.28.16/mypy_boto3_opsworks/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opsworks-1.28.15.post1/mypy_boto3_opsworks/__main__.py` & `mypy-boto3-opsworks-1.28.16/mypy_boto3_opsworks/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.OpsWorks 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.OpsWorks 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks\nOther"
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

### Comparing `mypy-boto3-opsworks-1.28.15.post1/mypy_boto3_opsworks/client.py` & `mypy-boto3-opsworks-1.28.16/mypy_boto3_opsworks/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,45 +10,42 @@
     from mypy_boto3_opsworks.client import OpsWorksClient
 
     session = Session()
     client: OpsWorksClient = session.client("opsworks")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AppAttributesKeysType,
     AppTypeType,
     ArchitectureType,
     AutoScalingTypeType,
     LayerAttributesKeysType,
     LayerTypeType,
     RootDeviceTypeType,
 )
 from .paginator import DescribeEcsClustersPaginator
 from .type_defs import (
-    AutoScalingThresholdsOutputTypeDef,
-    AutoScalingThresholdsTypeDef,
+    AutoScalingThresholdsUnionTypeDef,
     BlockDeviceMappingTypeDef,
     ChefConfigurationTypeDef,
     CloneStackResultTypeDef,
-    CloudWatchLogsConfigurationOutputTypeDef,
-    CloudWatchLogsConfigurationTypeDef,
+    CloudWatchLogsConfigurationUnionTypeDef,
     CreateAppResultTypeDef,
     CreateDeploymentResultTypeDef,
     CreateInstanceResultTypeDef,
     CreateLayerResultTypeDef,
     CreateStackResultTypeDef,
     CreateUserProfileResultTypeDef,
     DataSourceTypeDef,
-    DeploymentCommandOutputTypeDef,
-    DeploymentCommandTypeDef,
+    DeploymentCommandUnionTypeDef,
     DescribeAgentVersionsResultTypeDef,
     DescribeAppsResultTypeDef,
     DescribeCommandsResultTypeDef,
     DescribeDeploymentsResultTypeDef,
     DescribeEcsClustersResultTypeDef,
     DescribeElasticIpsResultTypeDef,
     DescribeElasticLoadBalancersResultTypeDef,
@@ -70,26 +67,24 @@
     EmptyResponseMetadataTypeDef,
     EnvironmentVariableTypeDef,
     GetHostnameSuggestionResultTypeDef,
     GrantAccessResultTypeDef,
     InstanceIdentityTypeDef,
     LifecycleEventConfigurationTypeDef,
     ListTagsResultTypeDef,
-    RecipesOutputTypeDef,
-    RecipesTypeDef,
+    RecipesUnionTypeDef,
     RegisterEcsClusterResultTypeDef,
     RegisterElasticIpResultTypeDef,
     RegisterInstanceResultTypeDef,
     RegisterVolumeResultTypeDef,
     SourceTypeDef,
     SslConfigurationTypeDef,
     StackConfigurationManagerTypeDef,
     VolumeConfigurationTypeDef,
-    WeeklyAutoScalingScheduleOutputTypeDef,
-    WeeklyAutoScalingScheduleTypeDef,
+    WeeklyAutoScalingScheduleUnionTypeDef,
 )
 from .waiter import (
     AppExistsWaiter,
     DeploymentSuccessfulWaiter,
     InstanceOnlineWaiter,
     InstanceRegisteredWaiter,
     InstanceStoppedWaiter,
@@ -250,15 +245,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/client/#create_app)
         """
 
     def create_deployment(
         self,
         *,
         StackId: str,
-        Command: Union[DeploymentCommandTypeDef, DeploymentCommandOutputTypeDef],
+        Command: DeploymentCommandUnionTypeDef,
         AppId: str = ...,
         InstanceIds: Sequence[str] = ...,
         LayerIds: Sequence[str] = ...,
         Comment: str = ...,
         CustomJson: str = ...
     ) -> CreateDeploymentResultTypeDef:
         """
@@ -301,26 +296,24 @@
         self,
         *,
         StackId: str,
         Type: LayerTypeType,
         Name: str,
         Shortname: str,
         Attributes: Mapping[LayerAttributesKeysType, str] = ...,
-        CloudWatchLogsConfiguration: Union[
-            CloudWatchLogsConfigurationTypeDef, CloudWatchLogsConfigurationOutputTypeDef
-        ] = ...,
+        CloudWatchLogsConfiguration: CloudWatchLogsConfigurationUnionTypeDef = ...,
         CustomInstanceProfileArn: str = ...,
         CustomJson: str = ...,
         CustomSecurityGroupIds: Sequence[str] = ...,
         Packages: Sequence[str] = ...,
         VolumeConfigurations: Sequence[VolumeConfigurationTypeDef] = ...,
         EnableAutoHealing: bool = ...,
         AutoAssignElasticIps: bool = ...,
         AutoAssignPublicIps: bool = ...,
-        CustomRecipes: Union[RecipesTypeDef, RecipesOutputTypeDef] = ...,
+        CustomRecipes: RecipesUnionTypeDef = ...,
         InstallUpdatesOnBoot: bool = ...,
         UseEbsOptimizedInstances: bool = ...,
         LifecycleEventConfiguration: LifecycleEventConfigurationTypeDef = ...
     ) -> CreateLayerResultTypeDef:
         """
         Creates a layer.
 
@@ -810,16 +803,16 @@
         """
 
     def set_load_based_auto_scaling(
         self,
         *,
         LayerId: str,
         Enable: bool = ...,
-        UpScaling: Union[AutoScalingThresholdsTypeDef, AutoScalingThresholdsOutputTypeDef] = ...,
-        DownScaling: Union[AutoScalingThresholdsTypeDef, AutoScalingThresholdsOutputTypeDef] = ...
+        UpScaling: AutoScalingThresholdsUnionTypeDef = ...,
+        DownScaling: AutoScalingThresholdsUnionTypeDef = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Specify the load-based auto scaling configuration for a specified layer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.set_load_based_auto_scaling)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/client/#set_load_based_auto_scaling)
         """
@@ -837,20 +830,15 @@
         Specifies a user's permissions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.set_permission)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/client/#set_permission)
         """
 
     def set_time_based_auto_scaling(
-        self,
-        *,
-        InstanceId: str,
-        AutoScalingSchedule: Union[
-            WeeklyAutoScalingScheduleTypeDef, WeeklyAutoScalingScheduleOutputTypeDef
-        ] = ...
+        self, *, InstanceId: str, AutoScalingSchedule: WeeklyAutoScalingScheduleUnionTypeDef = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Specify the time-based auto scaling configuration for a specified instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.set_time_based_auto_scaling)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/client/#set_time_based_auto_scaling)
         """
@@ -979,26 +967,24 @@
     def update_layer(
         self,
         *,
         LayerId: str,
         Name: str = ...,
         Shortname: str = ...,
         Attributes: Mapping[LayerAttributesKeysType, str] = ...,
-        CloudWatchLogsConfiguration: Union[
-            CloudWatchLogsConfigurationTypeDef, CloudWatchLogsConfigurationOutputTypeDef
-        ] = ...,
+        CloudWatchLogsConfiguration: CloudWatchLogsConfigurationUnionTypeDef = ...,
         CustomInstanceProfileArn: str = ...,
         CustomJson: str = ...,
         CustomSecurityGroupIds: Sequence[str] = ...,
         Packages: Sequence[str] = ...,
         VolumeConfigurations: Sequence[VolumeConfigurationTypeDef] = ...,
         EnableAutoHealing: bool = ...,
         AutoAssignElasticIps: bool = ...,
         AutoAssignPublicIps: bool = ...,
-        CustomRecipes: Union[RecipesTypeDef, RecipesOutputTypeDef] = ...,
+        CustomRecipes: RecipesUnionTypeDef = ...,
         InstallUpdatesOnBoot: bool = ...,
         UseEbsOptimizedInstances: bool = ...,
         LifecycleEventConfiguration: LifecycleEventConfigurationTypeDef = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates a specified layer.
```

### Comparing `mypy-boto3-opsworks-1.28.15.post1/mypy_boto3_opsworks/client.pyi` & `mypy-boto3-opsworks-1.28.16/mypy_boto3_opsworks/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -10,45 +10,42 @@
     from mypy_boto3_opsworks.client import OpsWorksClient
 
     session = Session()
     client: OpsWorksClient = session.client("opsworks")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AppAttributesKeysType,
     AppTypeType,
     ArchitectureType,
     AutoScalingTypeType,
     LayerAttributesKeysType,
     LayerTypeType,
     RootDeviceTypeType,
 )
 from .paginator import DescribeEcsClustersPaginator
 from .type_defs import (
-    AutoScalingThresholdsOutputTypeDef,
-    AutoScalingThresholdsTypeDef,
+    AutoScalingThresholdsUnionTypeDef,
     BlockDeviceMappingTypeDef,
     ChefConfigurationTypeDef,
     CloneStackResultTypeDef,
-    CloudWatchLogsConfigurationOutputTypeDef,
-    CloudWatchLogsConfigurationTypeDef,
+    CloudWatchLogsConfigurationUnionTypeDef,
     CreateAppResultTypeDef,
     CreateDeploymentResultTypeDef,
     CreateInstanceResultTypeDef,
     CreateLayerResultTypeDef,
     CreateStackResultTypeDef,
     CreateUserProfileResultTypeDef,
     DataSourceTypeDef,
-    DeploymentCommandOutputTypeDef,
-    DeploymentCommandTypeDef,
+    DeploymentCommandUnionTypeDef,
     DescribeAgentVersionsResultTypeDef,
     DescribeAppsResultTypeDef,
     DescribeCommandsResultTypeDef,
     DescribeDeploymentsResultTypeDef,
     DescribeEcsClustersResultTypeDef,
     DescribeElasticIpsResultTypeDef,
     DescribeElasticLoadBalancersResultTypeDef,
@@ -70,26 +67,24 @@
     EmptyResponseMetadataTypeDef,
     EnvironmentVariableTypeDef,
     GetHostnameSuggestionResultTypeDef,
     GrantAccessResultTypeDef,
     InstanceIdentityTypeDef,
     LifecycleEventConfigurationTypeDef,
     ListTagsResultTypeDef,
-    RecipesOutputTypeDef,
-    RecipesTypeDef,
+    RecipesUnionTypeDef,
     RegisterEcsClusterResultTypeDef,
     RegisterElasticIpResultTypeDef,
     RegisterInstanceResultTypeDef,
     RegisterVolumeResultTypeDef,
     SourceTypeDef,
     SslConfigurationTypeDef,
     StackConfigurationManagerTypeDef,
     VolumeConfigurationTypeDef,
-    WeeklyAutoScalingScheduleOutputTypeDef,
-    WeeklyAutoScalingScheduleTypeDef,
+    WeeklyAutoScalingScheduleUnionTypeDef,
 )
 from .waiter import (
     AppExistsWaiter,
     DeploymentSuccessfulWaiter,
     InstanceOnlineWaiter,
     InstanceRegisteredWaiter,
     InstanceStoppedWaiter,
@@ -237,15 +232,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.create_app)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/client/#create_app)
         """
     def create_deployment(
         self,
         *,
         StackId: str,
-        Command: Union[DeploymentCommandTypeDef, DeploymentCommandOutputTypeDef],
+        Command: DeploymentCommandUnionTypeDef,
         AppId: str = ...,
         InstanceIds: Sequence[str] = ...,
         LayerIds: Sequence[str] = ...,
         Comment: str = ...,
         CustomJson: str = ...
     ) -> CreateDeploymentResultTypeDef:
         """
@@ -286,26 +281,24 @@
         self,
         *,
         StackId: str,
         Type: LayerTypeType,
         Name: str,
         Shortname: str,
         Attributes: Mapping[LayerAttributesKeysType, str] = ...,
-        CloudWatchLogsConfiguration: Union[
-            CloudWatchLogsConfigurationTypeDef, CloudWatchLogsConfigurationOutputTypeDef
-        ] = ...,
+        CloudWatchLogsConfiguration: CloudWatchLogsConfigurationUnionTypeDef = ...,
         CustomInstanceProfileArn: str = ...,
         CustomJson: str = ...,
         CustomSecurityGroupIds: Sequence[str] = ...,
         Packages: Sequence[str] = ...,
         VolumeConfigurations: Sequence[VolumeConfigurationTypeDef] = ...,
         EnableAutoHealing: bool = ...,
         AutoAssignElasticIps: bool = ...,
         AutoAssignPublicIps: bool = ...,
-        CustomRecipes: Union[RecipesTypeDef, RecipesOutputTypeDef] = ...,
+        CustomRecipes: RecipesUnionTypeDef = ...,
         InstallUpdatesOnBoot: bool = ...,
         UseEbsOptimizedInstances: bool = ...,
         LifecycleEventConfiguration: LifecycleEventConfigurationTypeDef = ...
     ) -> CreateLayerResultTypeDef:
         """
         Creates a layer.
 
@@ -748,16 +741,16 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/client/#register_volume)
         """
     def set_load_based_auto_scaling(
         self,
         *,
         LayerId: str,
         Enable: bool = ...,
-        UpScaling: Union[AutoScalingThresholdsTypeDef, AutoScalingThresholdsOutputTypeDef] = ...,
-        DownScaling: Union[AutoScalingThresholdsTypeDef, AutoScalingThresholdsOutputTypeDef] = ...
+        UpScaling: AutoScalingThresholdsUnionTypeDef = ...,
+        DownScaling: AutoScalingThresholdsUnionTypeDef = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Specify the load-based auto scaling configuration for a specified layer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.set_load_based_auto_scaling)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/client/#set_load_based_auto_scaling)
         """
@@ -773,20 +766,15 @@
         """
         Specifies a user's permissions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.set_permission)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/client/#set_permission)
         """
     def set_time_based_auto_scaling(
-        self,
-        *,
-        InstanceId: str,
-        AutoScalingSchedule: Union[
-            WeeklyAutoScalingScheduleTypeDef, WeeklyAutoScalingScheduleOutputTypeDef
-        ] = ...
+        self, *, InstanceId: str, AutoScalingSchedule: WeeklyAutoScalingScheduleUnionTypeDef = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Specify the time-based auto scaling configuration for a specified instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.set_time_based_auto_scaling)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/client/#set_time_based_auto_scaling)
         """
@@ -903,26 +891,24 @@
     def update_layer(
         self,
         *,
         LayerId: str,
         Name: str = ...,
         Shortname: str = ...,
         Attributes: Mapping[LayerAttributesKeysType, str] = ...,
-        CloudWatchLogsConfiguration: Union[
-            CloudWatchLogsConfigurationTypeDef, CloudWatchLogsConfigurationOutputTypeDef
-        ] = ...,
+        CloudWatchLogsConfiguration: CloudWatchLogsConfigurationUnionTypeDef = ...,
         CustomInstanceProfileArn: str = ...,
         CustomJson: str = ...,
         CustomSecurityGroupIds: Sequence[str] = ...,
         Packages: Sequence[str] = ...,
         VolumeConfigurations: Sequence[VolumeConfigurationTypeDef] = ...,
         EnableAutoHealing: bool = ...,
         AutoAssignElasticIps: bool = ...,
         AutoAssignPublicIps: bool = ...,
-        CustomRecipes: Union[RecipesTypeDef, RecipesOutputTypeDef] = ...,
+        CustomRecipes: RecipesUnionTypeDef = ...,
         InstallUpdatesOnBoot: bool = ...,
         UseEbsOptimizedInstances: bool = ...,
         LifecycleEventConfiguration: LifecycleEventConfigurationTypeDef = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates a specified layer.
```

### Comparing `mypy-boto3-opsworks-1.28.15.post1/mypy_boto3_opsworks/literals.py` & `mypy-boto3-opsworks-1.28.16/mypy_boto3_opsworks/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opsworks-1.28.15.post1/mypy_boto3_opsworks/literals.pyi` & `mypy-boto3-opsworks-1.28.16/mypy_boto3_opsworks/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opsworks-1.28.15.post1/mypy_boto3_opsworks/paginator.py` & `mypy-boto3-opsworks-1.28.16/mypy_boto3_opsworks/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opsworks-1.28.15.post1/mypy_boto3_opsworks/paginator.pyi` & `mypy-boto3-opsworks-1.28.16/mypy_boto3_opsworks/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opsworks-1.28.15.post1/mypy_boto3_opsworks/service_resource.py` & `mypy-boto3-opsworks-1.28.16/mypy_boto3_opsworks/service_resource.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opsworks-1.28.15.post1/mypy_boto3_opsworks/service_resource.pyi` & `mypy-boto3-opsworks-1.28.16/mypy_boto3_opsworks/service_resource.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opsworks-1.28.15.post1/mypy_boto3_opsworks/type_defs.py` & `mypy-boto3-opsworks-1.28.16/mypy_boto3_opsworks/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_opsworks.type_defs import StackConfigurationManagerTypeDef
 
-    data: StackConfigurationManagerTypeDef = {...}
+    data: StackConfigurationManagerTypeDef = ...
     ```
 """
 import sys
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AppAttributesKeysType,
     AppTypeType,
     ArchitectureType,
     AutoScalingTypeType,
     CloudWatchLogsEncodingType,
@@ -55,15 +55,14 @@
     "AutoScalingThresholdsTypeDef",
     "EbsBlockDeviceTypeDef",
     "ResponseMetadataTypeDef",
     "ChefConfigurationTypeDef",
     "CloudWatchLogsLogStreamTypeDef",
     "CommandTypeDef",
     "DeploymentCommandTypeDef",
-    "RecipesTypeDef",
     "VolumeConfigurationTypeDef",
     "CreateUserProfileRequestRequestTypeDef",
     "DeleteAppRequestRequestTypeDef",
     "DeleteInstanceRequestRequestTypeDef",
     "DeleteLayerRequestRequestTypeDef",
     "DeleteStackRequestRequestTypeDef",
     "DeleteUserProfileRequestRequestTypeDef",
@@ -140,14 +139,15 @@
     "UpdateVolumeRequestRequestTypeDef",
     "AgentVersionTypeDef",
     "DescribeAgentVersionsRequestRequestTypeDef",
     "AppTypeDef",
     "CreateAppRequestRequestTypeDef",
     "UpdateAppRequestRequestTypeDef",
     "LoadBasedAutoScalingConfigurationTypeDef",
+    "AutoScalingThresholdsUnionTypeDef",
     "SetLoadBasedAutoScalingRequestRequestTypeDef",
     "BlockDeviceMappingTypeDef",
     "ChefConfigurationResponseTypeDef",
     "CloneStackResultTypeDef",
     "CreateAppResultTypeDef",
     "CreateDeploymentResultTypeDef",
     "CreateInstanceResultTypeDef",
@@ -155,14 +155,15 @@
     "CreateStackResultTypeDef",
     "CreateUserProfileResultTypeDef",
     "DescribeStackProvisioningParametersResultTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetHostnameSuggestionResultTypeDef",
     "InstancesCountResponseTypeDef",
     "ListTagsResultTypeDef",
+    "RecipesTypeDef",
     "RegisterEcsClusterResultTypeDef",
     "RegisterElasticIpResultTypeDef",
     "RegisterInstanceResultTypeDef",
     "RegisterVolumeResultTypeDef",
     "SourceResponseTypeDef",
     "StackConfigurationManagerResponseTypeDef",
     "CloneStackRequestRequestTypeDef",
@@ -170,14 +171,15 @@
     "CreateStackRequestServiceResourceCreateStackTypeDef",
     "StackTypeDef",
     "UpdateStackRequestRequestTypeDef",
     "CloudWatchLogsConfigurationOutputTypeDef",
     "CloudWatchLogsConfigurationTypeDef",
     "DescribeCommandsResultTypeDef",
     "CreateDeploymentRequestRequestTypeDef",
+    "DeploymentCommandUnionTypeDef",
     "DeploymentTypeDef",
     "DescribeAppsRequestAppExistsWaitTypeDef",
     "DescribeDeploymentsRequestDeploymentSuccessfulWaitTypeDef",
     "DescribeInstancesRequestInstanceOnlineWaitTypeDef",
     "DescribeInstancesRequestInstanceRegisteredWaitTypeDef",
     "DescribeInstancesRequestInstanceStoppedWaitTypeDef",
     "DescribeInstancesRequestInstanceTerminatedWaitTypeDef",
@@ -196,20 +198,23 @@
     "RegisterInstanceRequestRequestTypeDef",
     "StackSummaryTypeDef",
     "LifecycleEventConfigurationResponseTypeDef",
     "LifecycleEventConfigurationTypeDef",
     "OperatingSystemTypeDef",
     "SetTimeBasedAutoScalingRequestRequestTypeDef",
     "TimeBasedAutoScalingConfigurationTypeDef",
+    "WeeklyAutoScalingScheduleUnionTypeDef",
     "DescribeAgentVersionsResultTypeDef",
     "DescribeAppsResultTypeDef",
     "DescribeLoadBasedAutoScalingResultTypeDef",
     "CreateInstanceRequestRequestTypeDef",
     "InstanceTypeDef",
+    "RecipesUnionTypeDef",
     "DescribeStacksResultTypeDef",
+    "CloudWatchLogsConfigurationUnionTypeDef",
     "DescribeDeploymentsResultTypeDef",
     "DescribeStackSummaryResultTypeDef",
     "CreateLayerRequestRequestTypeDef",
     "CreateLayerRequestStackCreateLayerTypeDef",
     "LayerTypeDef",
     "UpdateLayerRequestRequestTypeDef",
     "DescribeOperatingSystemsResponseTypeDef",
@@ -463,26 +468,14 @@
 
 class DeploymentCommandTypeDef(
     _RequiredDeploymentCommandTypeDef, _OptionalDeploymentCommandTypeDef
 ):
     pass
 
 
-RecipesTypeDef = TypedDict(
-    "RecipesTypeDef",
-    {
-        "Setup": Sequence[str],
-        "Configure": Sequence[str],
-        "Deploy": Sequence[str],
-        "Undeploy": Sequence[str],
-        "Shutdown": Sequence[str],
-    },
-    total=False,
-)
-
 _RequiredVolumeConfigurationTypeDef = TypedDict(
     "_RequiredVolumeConfigurationTypeDef",
     {
         "MountPoint": str,
         "NumberOfDisks": int,
         "Size": int,
     },
@@ -1546,14 +1539,17 @@
         "Enable": bool,
         "UpScaling": AutoScalingThresholdsOutputTypeDef,
         "DownScaling": AutoScalingThresholdsOutputTypeDef,
     },
     total=False,
 )
 
+AutoScalingThresholdsUnionTypeDef = Union[
+    AutoScalingThresholdsTypeDef, AutoScalingThresholdsOutputTypeDef
+]
 _RequiredSetLoadBasedAutoScalingRequestRequestTypeDef = TypedDict(
     "_RequiredSetLoadBasedAutoScalingRequestRequestTypeDef",
     {
         "LayerId": str,
     },
 )
 _OptionalSetLoadBasedAutoScalingRequestRequestTypeDef = TypedDict(
@@ -1707,14 +1703,26 @@
     {
         "Tags": Dict[str, str],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+RecipesTypeDef = TypedDict(
+    "RecipesTypeDef",
+    {
+        "Setup": List[str],
+        "Configure": List[str],
+        "Deploy": List[str],
+        "Undeploy": List[str],
+        "Shutdown": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 RegisterEcsClusterResultTypeDef = TypedDict(
     "RegisterEcsClusterResultTypeDef",
     {
         "EcsClusterArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1958,17 +1966,17 @@
     total=False,
 )
 
 CloudWatchLogsConfigurationTypeDef = TypedDict(
     "CloudWatchLogsConfigurationTypeDef",
     {
         "Enabled": bool,
-        "LogStreams": List[CloudWatchLogsLogStreamTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "LogStreams": Sequence[CloudWatchLogsLogStreamTypeDef],
     },
+    total=False,
 )
 
 DescribeCommandsResultTypeDef = TypedDict(
     "DescribeCommandsResultTypeDef",
     {
         "Commands": List[CommandTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1997,14 +2005,15 @@
 
 class CreateDeploymentRequestRequestTypeDef(
     _RequiredCreateDeploymentRequestRequestTypeDef, _OptionalCreateDeploymentRequestRequestTypeDef
 ):
     pass
 
 
+DeploymentCommandUnionTypeDef = Union[DeploymentCommandTypeDef, DeploymentCommandOutputTypeDef]
 DeploymentTypeDef = TypedDict(
     "DeploymentTypeDef",
     {
         "DeploymentId": str,
         "StackId": str,
         "AppId": str,
         "CreatedAt": str,
@@ -2280,14 +2289,17 @@
     {
         "InstanceId": str,
         "AutoScalingSchedule": WeeklyAutoScalingScheduleOutputTypeDef,
     },
     total=False,
 )
 
+WeeklyAutoScalingScheduleUnionTypeDef = Union[
+    WeeklyAutoScalingScheduleTypeDef, WeeklyAutoScalingScheduleOutputTypeDef
+]
 DescribeAgentVersionsResultTypeDef = TypedDict(
     "DescribeAgentVersionsResultTypeDef",
     {
         "AgentVersions": List[AgentVersionTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2389,22 +2401,26 @@
         "SubnetId": str,
         "Tenancy": str,
         "VirtualizationType": VirtualizationTypeType,
     },
     total=False,
 )
 
+RecipesUnionTypeDef = Union[RecipesTypeDef, RecipesOutputTypeDef]
 DescribeStacksResultTypeDef = TypedDict(
     "DescribeStacksResultTypeDef",
     {
         "Stacks": List[StackTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+CloudWatchLogsConfigurationUnionTypeDef = Union[
+    CloudWatchLogsConfigurationTypeDef, CloudWatchLogsConfigurationOutputTypeDef
+]
 DescribeDeploymentsResultTypeDef = TypedDict(
     "DescribeDeploymentsResultTypeDef",
     {
         "Deployments": List[DeploymentTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-opsworks-1.28.15.post1/mypy_boto3_opsworks/type_defs.pyi` & `mypy-boto3-opsworks-1.28.16/mypy_boto3_opsworks/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_opsworks.type_defs import StackConfigurationManagerTypeDef
 
-    data: StackConfigurationManagerTypeDef = {...}
+    data: StackConfigurationManagerTypeDef = ...
     ```
 """
 import sys
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AppAttributesKeysType,
     AppTypeType,
     ArchitectureType,
     AutoScalingTypeType,
     CloudWatchLogsEncodingType,
@@ -54,15 +54,14 @@
     "AutoScalingThresholdsTypeDef",
     "EbsBlockDeviceTypeDef",
     "ResponseMetadataTypeDef",
     "ChefConfigurationTypeDef",
     "CloudWatchLogsLogStreamTypeDef",
     "CommandTypeDef",
     "DeploymentCommandTypeDef",
-    "RecipesTypeDef",
     "VolumeConfigurationTypeDef",
     "CreateUserProfileRequestRequestTypeDef",
     "DeleteAppRequestRequestTypeDef",
     "DeleteInstanceRequestRequestTypeDef",
     "DeleteLayerRequestRequestTypeDef",
     "DeleteStackRequestRequestTypeDef",
     "DeleteUserProfileRequestRequestTypeDef",
@@ -139,14 +138,15 @@
     "UpdateVolumeRequestRequestTypeDef",
     "AgentVersionTypeDef",
     "DescribeAgentVersionsRequestRequestTypeDef",
     "AppTypeDef",
     "CreateAppRequestRequestTypeDef",
     "UpdateAppRequestRequestTypeDef",
     "LoadBasedAutoScalingConfigurationTypeDef",
+    "AutoScalingThresholdsUnionTypeDef",
     "SetLoadBasedAutoScalingRequestRequestTypeDef",
     "BlockDeviceMappingTypeDef",
     "ChefConfigurationResponseTypeDef",
     "CloneStackResultTypeDef",
     "CreateAppResultTypeDef",
     "CreateDeploymentResultTypeDef",
     "CreateInstanceResultTypeDef",
@@ -154,14 +154,15 @@
     "CreateStackResultTypeDef",
     "CreateUserProfileResultTypeDef",
     "DescribeStackProvisioningParametersResultTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetHostnameSuggestionResultTypeDef",
     "InstancesCountResponseTypeDef",
     "ListTagsResultTypeDef",
+    "RecipesTypeDef",
     "RegisterEcsClusterResultTypeDef",
     "RegisterElasticIpResultTypeDef",
     "RegisterInstanceResultTypeDef",
     "RegisterVolumeResultTypeDef",
     "SourceResponseTypeDef",
     "StackConfigurationManagerResponseTypeDef",
     "CloneStackRequestRequestTypeDef",
@@ -169,14 +170,15 @@
     "CreateStackRequestServiceResourceCreateStackTypeDef",
     "StackTypeDef",
     "UpdateStackRequestRequestTypeDef",
     "CloudWatchLogsConfigurationOutputTypeDef",
     "CloudWatchLogsConfigurationTypeDef",
     "DescribeCommandsResultTypeDef",
     "CreateDeploymentRequestRequestTypeDef",
+    "DeploymentCommandUnionTypeDef",
     "DeploymentTypeDef",
     "DescribeAppsRequestAppExistsWaitTypeDef",
     "DescribeDeploymentsRequestDeploymentSuccessfulWaitTypeDef",
     "DescribeInstancesRequestInstanceOnlineWaitTypeDef",
     "DescribeInstancesRequestInstanceRegisteredWaitTypeDef",
     "DescribeInstancesRequestInstanceStoppedWaitTypeDef",
     "DescribeInstancesRequestInstanceTerminatedWaitTypeDef",
@@ -195,20 +197,23 @@
     "RegisterInstanceRequestRequestTypeDef",
     "StackSummaryTypeDef",
     "LifecycleEventConfigurationResponseTypeDef",
     "LifecycleEventConfigurationTypeDef",
     "OperatingSystemTypeDef",
     "SetTimeBasedAutoScalingRequestRequestTypeDef",
     "TimeBasedAutoScalingConfigurationTypeDef",
+    "WeeklyAutoScalingScheduleUnionTypeDef",
     "DescribeAgentVersionsResultTypeDef",
     "DescribeAppsResultTypeDef",
     "DescribeLoadBasedAutoScalingResultTypeDef",
     "CreateInstanceRequestRequestTypeDef",
     "InstanceTypeDef",
+    "RecipesUnionTypeDef",
     "DescribeStacksResultTypeDef",
+    "CloudWatchLogsConfigurationUnionTypeDef",
     "DescribeDeploymentsResultTypeDef",
     "DescribeStackSummaryResultTypeDef",
     "CreateLayerRequestRequestTypeDef",
     "CreateLayerRequestStackCreateLayerTypeDef",
     "LayerTypeDef",
     "UpdateLayerRequestRequestTypeDef",
     "DescribeOperatingSystemsResponseTypeDef",
@@ -452,26 +457,14 @@
 )
 
 class DeploymentCommandTypeDef(
     _RequiredDeploymentCommandTypeDef, _OptionalDeploymentCommandTypeDef
 ):
     pass
 
-RecipesTypeDef = TypedDict(
-    "RecipesTypeDef",
-    {
-        "Setup": Sequence[str],
-        "Configure": Sequence[str],
-        "Deploy": Sequence[str],
-        "Undeploy": Sequence[str],
-        "Shutdown": Sequence[str],
-    },
-    total=False,
-)
-
 _RequiredVolumeConfigurationTypeDef = TypedDict(
     "_RequiredVolumeConfigurationTypeDef",
     {
         "MountPoint": str,
         "NumberOfDisks": int,
         "Size": int,
     },
@@ -1501,14 +1494,17 @@
         "Enable": bool,
         "UpScaling": AutoScalingThresholdsOutputTypeDef,
         "DownScaling": AutoScalingThresholdsOutputTypeDef,
     },
     total=False,
 )
 
+AutoScalingThresholdsUnionTypeDef = Union[
+    AutoScalingThresholdsTypeDef, AutoScalingThresholdsOutputTypeDef
+]
 _RequiredSetLoadBasedAutoScalingRequestRequestTypeDef = TypedDict(
     "_RequiredSetLoadBasedAutoScalingRequestRequestTypeDef",
     {
         "LayerId": str,
     },
 )
 _OptionalSetLoadBasedAutoScalingRequestRequestTypeDef = TypedDict(
@@ -1660,14 +1656,26 @@
     {
         "Tags": Dict[str, str],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+RecipesTypeDef = TypedDict(
+    "RecipesTypeDef",
+    {
+        "Setup": List[str],
+        "Configure": List[str],
+        "Deploy": List[str],
+        "Undeploy": List[str],
+        "Shutdown": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 RegisterEcsClusterResultTypeDef = TypedDict(
     "RegisterEcsClusterResultTypeDef",
     {
         "EcsClusterArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1903,17 +1911,17 @@
     total=False,
 )
 
 CloudWatchLogsConfigurationTypeDef = TypedDict(
     "CloudWatchLogsConfigurationTypeDef",
     {
         "Enabled": bool,
-        "LogStreams": List[CloudWatchLogsLogStreamTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "LogStreams": Sequence[CloudWatchLogsLogStreamTypeDef],
     },
+    total=False,
 )
 
 DescribeCommandsResultTypeDef = TypedDict(
     "DescribeCommandsResultTypeDef",
     {
         "Commands": List[CommandTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1940,14 +1948,15 @@
 )
 
 class CreateDeploymentRequestRequestTypeDef(
     _RequiredCreateDeploymentRequestRequestTypeDef, _OptionalCreateDeploymentRequestRequestTypeDef
 ):
     pass
 
+DeploymentCommandUnionTypeDef = Union[DeploymentCommandTypeDef, DeploymentCommandOutputTypeDef]
 DeploymentTypeDef = TypedDict(
     "DeploymentTypeDef",
     {
         "DeploymentId": str,
         "StackId": str,
         "AppId": str,
         "CreatedAt": str,
@@ -2219,14 +2228,17 @@
     {
         "InstanceId": str,
         "AutoScalingSchedule": WeeklyAutoScalingScheduleOutputTypeDef,
     },
     total=False,
 )
 
+WeeklyAutoScalingScheduleUnionTypeDef = Union[
+    WeeklyAutoScalingScheduleTypeDef, WeeklyAutoScalingScheduleOutputTypeDef
+]
 DescribeAgentVersionsResultTypeDef = TypedDict(
     "DescribeAgentVersionsResultTypeDef",
     {
         "AgentVersions": List[AgentVersionTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2326,22 +2338,26 @@
         "SubnetId": str,
         "Tenancy": str,
         "VirtualizationType": VirtualizationTypeType,
     },
     total=False,
 )
 
+RecipesUnionTypeDef = Union[RecipesTypeDef, RecipesOutputTypeDef]
 DescribeStacksResultTypeDef = TypedDict(
     "DescribeStacksResultTypeDef",
     {
         "Stacks": List[StackTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+CloudWatchLogsConfigurationUnionTypeDef = Union[
+    CloudWatchLogsConfigurationTypeDef, CloudWatchLogsConfigurationOutputTypeDef
+]
 DescribeDeploymentsResultTypeDef = TypedDict(
     "DescribeDeploymentsResultTypeDef",
     {
         "Deployments": List[DeploymentTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-opsworks-1.28.15.post1/mypy_boto3_opsworks/waiter.py` & `mypy-boto3-opsworks-1.28.16/mypy_boto3_opsworks/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opsworks-1.28.15.post1/mypy_boto3_opsworks/waiter.pyi` & `mypy-boto3-opsworks-1.28.16/mypy_boto3_opsworks/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opsworks-1.28.15.post1/mypy_boto3_opsworks.egg-info/PKG-INFO` & `mypy-boto3-opsworks-1.28.16/mypy_boto3_opsworks.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-opsworks
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.OpsWorks 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.OpsWorks 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 opsworks type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 opsworks type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-opsworks.svg?color=blue)](https://pypi.org/project/mypy-boto3-opsworks)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-opsworks)](https://pepy.tech/project/mypy-boto3-opsworks)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.OpsWorks 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks)
+[boto3.OpsWorks 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks)
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
 [mypy-boto3-opsworks docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/).
 
 See how it helps to find and fix potential bugs:
 
@@ -78,15 +78,15 @@
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Waiters annotations](#waiters-annotations)
     - [Service Resource annotations](#service-resource-annotations)
     - [Other resources annotations](#other-resources-annotations)
     - [Collections annotations](#collections-annotations)
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
@@ -429,20 +429,20 @@
 )
 
 
 def check_value(value: AppAttributesKeysType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_opsworks.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_opsworks.type_defs import (
     StackConfigurationManagerTypeDef,
     DataSourceTypeDef,
     EnvironmentVariableTypeDef,
     SourceTypeDef,
@@ -455,15 +455,14 @@
     AutoScalingThresholdsTypeDef,
     EbsBlockDeviceTypeDef,
     ResponseMetadataTypeDef,
     ChefConfigurationTypeDef,
     CloudWatchLogsLogStreamTypeDef,
     CommandTypeDef,
     DeploymentCommandTypeDef,
-    RecipesTypeDef,
     VolumeConfigurationTypeDef,
     CreateUserProfileRequestRequestTypeDef,
     DeleteAppRequestRequestTypeDef,
     DeleteInstanceRequestRequestTypeDef,
     DeleteLayerRequestRequestTypeDef,
     DeleteStackRequestRequestTypeDef,
     DeleteUserProfileRequestRequestTypeDef,
@@ -540,14 +539,15 @@
     UpdateVolumeRequestRequestTypeDef,
     AgentVersionTypeDef,
     DescribeAgentVersionsRequestRequestTypeDef,
     AppTypeDef,
     CreateAppRequestRequestTypeDef,
     UpdateAppRequestRequestTypeDef,
     LoadBasedAutoScalingConfigurationTypeDef,
+    AutoScalingThresholdsUnionTypeDef,
     SetLoadBasedAutoScalingRequestRequestTypeDef,
     BlockDeviceMappingTypeDef,
     ChefConfigurationResponseTypeDef,
     CloneStackResultTypeDef,
     CreateAppResultTypeDef,
     CreateDeploymentResultTypeDef,
     CreateInstanceResultTypeDef,
@@ -555,14 +555,15 @@
     CreateStackResultTypeDef,
     CreateUserProfileResultTypeDef,
     DescribeStackProvisioningParametersResultTypeDef,
     EmptyResponseMetadataTypeDef,
     GetHostnameSuggestionResultTypeDef,
     InstancesCountResponseTypeDef,
     ListTagsResultTypeDef,
+    RecipesTypeDef,
     RegisterEcsClusterResultTypeDef,
     RegisterElasticIpResultTypeDef,
     RegisterInstanceResultTypeDef,
     RegisterVolumeResultTypeDef,
     SourceResponseTypeDef,
     StackConfigurationManagerResponseTypeDef,
     CloneStackRequestRequestTypeDef,
@@ -570,14 +571,15 @@
     CreateStackRequestServiceResourceCreateStackTypeDef,
     StackTypeDef,
     UpdateStackRequestRequestTypeDef,
     CloudWatchLogsConfigurationOutputTypeDef,
     CloudWatchLogsConfigurationTypeDef,
     DescribeCommandsResultTypeDef,
     CreateDeploymentRequestRequestTypeDef,
+    DeploymentCommandUnionTypeDef,
     DeploymentTypeDef,
     DescribeAppsRequestAppExistsWaitTypeDef,
     DescribeDeploymentsRequestDeploymentSuccessfulWaitTypeDef,
     DescribeInstancesRequestInstanceOnlineWaitTypeDef,
     DescribeInstancesRequestInstanceRegisteredWaitTypeDef,
     DescribeInstancesRequestInstanceStoppedWaitTypeDef,
     DescribeInstancesRequestInstanceTerminatedWaitTypeDef,
@@ -596,34 +598,37 @@
     RegisterInstanceRequestRequestTypeDef,
     StackSummaryTypeDef,
     LifecycleEventConfigurationResponseTypeDef,
     LifecycleEventConfigurationTypeDef,
     OperatingSystemTypeDef,
     SetTimeBasedAutoScalingRequestRequestTypeDef,
     TimeBasedAutoScalingConfigurationTypeDef,
+    WeeklyAutoScalingScheduleUnionTypeDef,
     DescribeAgentVersionsResultTypeDef,
     DescribeAppsResultTypeDef,
     DescribeLoadBasedAutoScalingResultTypeDef,
     CreateInstanceRequestRequestTypeDef,
     InstanceTypeDef,
+    RecipesUnionTypeDef,
     DescribeStacksResultTypeDef,
+    CloudWatchLogsConfigurationUnionTypeDef,
     DescribeDeploymentsResultTypeDef,
     DescribeStackSummaryResultTypeDef,
     CreateLayerRequestRequestTypeDef,
     CreateLayerRequestStackCreateLayerTypeDef,
     LayerTypeDef,
     UpdateLayerRequestRequestTypeDef,
     DescribeOperatingSystemsResponseTypeDef,
     DescribeTimeBasedAutoScalingResultTypeDef,
     DescribeInstancesResultTypeDef,
     DescribeLayersResultTypeDef,
 )
 
 
-def get_structure() -> StackConfigurationManagerTypeDef:
+def get_value() -> StackConfigurationManagerTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-opsworks-1.28.15.post1/mypy_boto3_opsworks.egg-info/SOURCES.txt` & `mypy-boto3-opsworks-1.28.16/mypy_boto3_opsworks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opsworks-1.28.15.post1/setup.py` & `mypy-boto3-opsworks-1.28.16/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-opsworks",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_opsworks"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.OpsWorks 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.2"
+        "Type annotations for boto3.OpsWorks 1.28.16 service generated with mypy-boto3-builder"
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
-    keywords="boto3 opsworks type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 opsworks type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_opsworks": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

