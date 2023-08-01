# Comparing `tmp/mypy-boto3-gamelift-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-gamelift-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-gamelift-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:11 2023, max compression
+gzip compressed data, was "mypy-boto3-gamelift-1.28.16.tar", last modified: Tue Aug  1 11:36:51 2023, max compression
```

## Comparing `mypy-boto3-gamelift-1.28.15.post1.tar` & `mypy-boto3-gamelift-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:11.289161 mypy-boto3-gamelift-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:45:53.000000 mypy-boto3-gamelift-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    29060 2023-07-29 10:03:11.289161 mypy-boto3-gamelift-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    27563 2023-07-29 09:45:53.000000 mypy-boto3-gamelift-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:11.285161 mypy-boto3-gamelift-1.28.15.post1/mypy_boto3_gamelift/
--rw-r--r--   0 runner    (1001) docker     (123)     5348 2023-07-29 09:45:53.000000 mypy-boto3-gamelift-1.28.15.post1/mypy_boto3_gamelift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5347 2023-07-29 09:45:53.000000 mypy-boto3-gamelift-1.28.15.post1/mypy_boto3_gamelift/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-29 09:45:53.000000 mypy-boto3-gamelift-1.28.15.post1/mypy_boto3_gamelift/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    85312 2023-07-29 09:45:54.000000 mypy-boto3-gamelift-1.28.15.post1/mypy_boto3_gamelift/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    85179 2023-07-29 09:45:54.000000 mypy-boto3-gamelift-1.28.15.post1/mypy_boto3_gamelift/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    20730 2023-07-29 09:45:55.000000 mypy-boto3-gamelift-1.28.15.post1/mypy_boto3_gamelift/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    20728 2023-07-29 09:45:55.000000 mypy-boto3-gamelift-1.28.15.post1/mypy_boto3_gamelift/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    26546 2023-07-29 09:45:54.000000 mypy-boto3-gamelift-1.28.15.post1/mypy_boto3_gamelift/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    26522 2023-07-29 09:45:54.000000 mypy-boto3-gamelift-1.28.15.post1/mypy_boto3_gamelift/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:45:53.000000 mypy-boto3-gamelift-1.28.15.post1/mypy_boto3_gamelift/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    99374 2023-07-29 09:45:59.000000 mypy-boto3-gamelift-1.28.15.post1/mypy_boto3_gamelift/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    99275 2023-07-29 09:45:56.000000 mypy-boto3-gamelift-1.28.15.post1/mypy_boto3_gamelift/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:45:53.000000 mypy-boto3-gamelift-1.28.15.post1/mypy_boto3_gamelift/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:11.289161 mypy-boto3-gamelift-1.28.15.post1/mypy_boto3_gamelift.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    29060 2023-07-29 10:03:11.000000 mypy-boto3-gamelift-1.28.15.post1/mypy_boto3_gamelift.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-29 10:03:11.000000 mypy-boto3-gamelift-1.28.15.post1/mypy_boto3_gamelift.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:11.000000 mypy-boto3-gamelift-1.28.15.post1/mypy_boto3_gamelift.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:11.000000 mypy-boto3-gamelift-1.28.15.post1/mypy_boto3_gamelift.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:11.000000 mypy-boto3-gamelift-1.28.15.post1/mypy_boto3_gamelift.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-29 10:03:11.000000 mypy-boto3-gamelift-1.28.15.post1/mypy_boto3_gamelift.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:11.289161 mypy-boto3-gamelift-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-07-29 09:45:53.000000 mypy-boto3-gamelift-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:51.848882 mypy-boto3-gamelift-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:18:30.000000 mypy-boto3-gamelift-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    29227 2023-08-01 11:36:51.848882 mypy-boto3-gamelift-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    27739 2023-08-01 11:18:30.000000 mypy-boto3-gamelift-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:51.848882 mypy-boto3-gamelift-1.28.16/mypy_boto3_gamelift/
+-rw-r--r--   0 runner    (1001) docker     (123)     5348 2023-08-01 11:18:30.000000 mypy-boto3-gamelift-1.28.16/mypy_boto3_gamelift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5347 2023-08-01 11:18:30.000000 mypy-boto3-gamelift-1.28.16/mypy_boto3_gamelift/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-08-01 11:18:30.000000 mypy-boto3-gamelift-1.28.16/mypy_boto3_gamelift/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    84642 2023-08-01 11:18:31.000000 mypy-boto3-gamelift-1.28.16/mypy_boto3_gamelift/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    84509 2023-08-01 11:18:31.000000 mypy-boto3-gamelift-1.28.16/mypy_boto3_gamelift/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    20730 2023-08-01 11:18:32.000000 mypy-boto3-gamelift-1.28.16/mypy_boto3_gamelift/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20728 2023-08-01 11:18:31.000000 mypy-boto3-gamelift-1.28.16/mypy_boto3_gamelift/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    26523 2023-08-01 11:18:31.000000 mypy-boto3-gamelift-1.28.16/mypy_boto3_gamelift/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26499 2023-08-01 11:18:31.000000 mypy-boto3-gamelift-1.28.16/mypy_boto3_gamelift/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:18:30.000000 mypy-boto3-gamelift-1.28.16/mypy_boto3_gamelift/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    99931 2023-08-01 11:18:36.000000 mypy-boto3-gamelift-1.28.16/mypy_boto3_gamelift/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    99832 2023-08-01 11:18:35.000000 mypy-boto3-gamelift-1.28.16/mypy_boto3_gamelift/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:18:30.000000 mypy-boto3-gamelift-1.28.16/mypy_boto3_gamelift/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:51.848882 mypy-boto3-gamelift-1.28.16/mypy_boto3_gamelift.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    29227 2023-08-01 11:36:51.000000 mypy-boto3-gamelift-1.28.16/mypy_boto3_gamelift.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-08-01 11:36:51.000000 mypy-boto3-gamelift-1.28.16/mypy_boto3_gamelift.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:51.000000 mypy-boto3-gamelift-1.28.16/mypy_boto3_gamelift.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:51.000000 mypy-boto3-gamelift-1.28.16/mypy_boto3_gamelift.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:51.000000 mypy-boto3-gamelift-1.28.16/mypy_boto3_gamelift.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-01 11:36:51.000000 mypy-boto3-gamelift-1.28.16/mypy_boto3_gamelift.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:51.848882 mypy-boto3-gamelift-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-08-01 11:18:30.000000 mypy-boto3-gamelift-1.28.16/setup.py
```

### Comparing `mypy-boto3-gamelift-1.28.15.post1/LICENSE` & `mypy-boto3-gamelift-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-gamelift-1.28.15.post1/PKG-INFO` & `mypy-boto3-gamelift-1.28.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-gamelift
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.GameLift 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.GameLift 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 gamelift type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 gamelift type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-gamelift.svg?color=blue)](https://pypi.org/project/mypy-boto3-gamelift)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-gamelift)](https://pepy.tech/project/mypy-boto3-gamelift)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.GameLift 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift)
+[boto3.GameLift 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift)
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
 [mypy-boto3-gamelift docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/).
 
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
@@ -447,29 +447,30 @@
 )
 
 
 def check_value(value: AcceptanceTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_gamelift.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_gamelift.type_defs import (
     AcceptMatchInputRequestTypeDef,
     RoutingStrategyTypeDef,
     AnywhereConfigurationTypeDef,
     AttributeValueOutputTypeDef,
     AttributeValueTypeDef,
     AwsCredentialsTypeDef,
+    BlobTypeDef,
     BuildTypeDef,
     CertificateConfigurationTypeDef,
     ClaimFilterOptionTypeDef,
     GameServerTypeDef,
     ResponseMetadataTypeDef,
     ComputeTypeDef,
     TagTypeDef,
@@ -512,15 +513,15 @@
     DescribeBuildInputRequestTypeDef,
     DescribeComputeInputRequestTypeDef,
     DescribeEC2InstanceLimitsInputRequestTypeDef,
     EC2InstanceLimitTypeDef,
     PaginatorConfigTypeDef,
     DescribeFleetAttributesInputRequestTypeDef,
     DescribeFleetCapacityInputRequestTypeDef,
-    DescribeFleetEventsInputRequestTypeDef,
+    TimestampTypeDef,
     EventTypeDef,
     DescribeFleetLocationAttributesInputRequestTypeDef,
     DescribeFleetLocationCapacityInputRequestTypeDef,
     DescribeFleetLocationUtilizationInputRequestTypeDef,
     FleetUtilizationTypeDef,
     DescribeFleetPortSettingsInputRequestTypeDef,
     DescribeFleetUtilizationInputRequestTypeDef,
@@ -649,15 +650,14 @@
     CreatePlayerSessionsOutputTypeDef,
     DescribePlayerSessionsOutputTypeDef,
     CreateVpcPeeringAuthorizationOutputTypeDef,
     DescribeVpcPeeringAuthorizationsOutputTypeDef,
     DescribeEC2InstanceLimitsOutputTypeDef,
     DescribeFleetAttributesInputDescribeFleetAttributesPaginateTypeDef,
     DescribeFleetCapacityInputDescribeFleetCapacityPaginateTypeDef,
-    DescribeFleetEventsInputDescribeFleetEventsPaginateTypeDef,
     DescribeFleetUtilizationInputDescribeFleetUtilizationPaginateTypeDef,
     DescribeGameServerInstancesInputDescribeGameServerInstancesPaginateTypeDef,
     DescribeGameSessionDetailsInputDescribeGameSessionDetailsPaginateTypeDef,
     DescribeGameSessionQueuesInputDescribeGameSessionQueuesPaginateTypeDef,
     DescribeGameSessionsInputDescribeGameSessionsPaginateTypeDef,
     DescribeInstancesInputDescribeInstancesPaginateTypeDef,
     DescribeMatchmakingConfigurationsInputDescribeMatchmakingConfigurationsPaginateTypeDef,
@@ -669,37 +669,40 @@
     ListComputeInputListComputePaginateTypeDef,
     ListFleetsInputListFleetsPaginateTypeDef,
     ListGameServerGroupsInputListGameServerGroupsPaginateTypeDef,
     ListGameServersInputListGameServersPaginateTypeDef,
     ListLocationsInputListLocationsPaginateTypeDef,
     ListScriptsInputListScriptsPaginateTypeDef,
     SearchGameSessionsInputSearchGameSessionsPaginateTypeDef,
+    DescribeFleetEventsInputDescribeFleetEventsPaginateTypeDef,
+    DescribeFleetEventsInputRequestTypeDef,
     DescribeFleetEventsOutputTypeDef,
     DescribeFleetLocationUtilizationOutputTypeDef,
     DescribeFleetUtilizationOutputTypeDef,
     DescribeGameServerInstancesOutputTypeDef,
     DescribeInstancesOutputTypeDef,
     FleetCapacityTypeDef,
+    FilterConfigurationUnionTypeDef,
     GameServerGroupAutoScalingPolicyTypeDef,
     GameSessionConnectionInfoTypeDef,
     GameSessionPlacementTypeDef,
     StartGameSessionPlacementInputRequestTypeDef,
     GameSessionQueueTypeDef,
+    PriorityConfigurationUnionTypeDef,
     InstanceAccessTypeDef,
     PutScalingPolicyInputRequestTypeDef,
     ScalingPolicyTypeDef,
     RuntimeConfigurationOutputTypeDef,
     RuntimeConfigurationTypeDef,
     VpcPeeringConnectionTypeDef,
     CreateAliasOutputTypeDef,
     DescribeAliasOutputTypeDef,
     ListAliasesOutputTypeDef,
     UpdateAliasOutputTypeDef,
-    StartMatchBackfillInputRequestTypeDef,
-    StartMatchmakingInputRequestTypeDef,
+    PlayerUnionTypeDef,
     CreateScriptOutputTypeDef,
     DescribeScriptOutputTypeDef,
     ListScriptsOutputTypeDef,
     UpdateScriptOutputTypeDef,
     CreateFleetOutputTypeDef,
     DescribeFleetAttributesOutputTypeDef,
     DescribeFleetLocationAttributesOutputTypeDef,
@@ -729,24 +732,27 @@
     DescribeGameSessionQueuesOutputTypeDef,
     UpdateGameSessionQueueOutputTypeDef,
     GetInstanceAccessOutputTypeDef,
     DescribeScalingPoliciesOutputTypeDef,
     DescribeRuntimeConfigurationOutputTypeDef,
     UpdateRuntimeConfigurationOutputTypeDef,
     CreateFleetInputRequestTypeDef,
+    RuntimeConfigurationUnionTypeDef,
     UpdateRuntimeConfigurationInputRequestTypeDef,
     DescribeVpcPeeringConnectionsOutputTypeDef,
+    StartMatchBackfillInputRequestTypeDef,
+    StartMatchmakingInputRequestTypeDef,
     DescribeGameSessionDetailsOutputTypeDef,
     DescribeMatchmakingOutputTypeDef,
     StartMatchBackfillOutputTypeDef,
     StartMatchmakingOutputTypeDef,
 )
 
 
-def get_structure() -> AcceptMatchInputRequestTypeDef:
+def get_value() -> AcceptMatchInputRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-gamelift-1.28.15.post1/README.md` & `mypy-boto3-gamelift-1.28.16/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-gamelift.svg?color=blue)](https://pypi.org/project/mypy-boto3-gamelift)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-gamelift)](https://pepy.tech/project/mypy-boto3-gamelift)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.GameLift 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift)
+[boto3.GameLift 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift)
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
 [mypy-boto3-gamelift docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/).
 
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
@@ -415,29 +415,30 @@
 )
 
 
 def check_value(value: AcceptanceTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_gamelift.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_gamelift.type_defs import (
     AcceptMatchInputRequestTypeDef,
     RoutingStrategyTypeDef,
     AnywhereConfigurationTypeDef,
     AttributeValueOutputTypeDef,
     AttributeValueTypeDef,
     AwsCredentialsTypeDef,
+    BlobTypeDef,
     BuildTypeDef,
     CertificateConfigurationTypeDef,
     ClaimFilterOptionTypeDef,
     GameServerTypeDef,
     ResponseMetadataTypeDef,
     ComputeTypeDef,
     TagTypeDef,
@@ -480,15 +481,15 @@
     DescribeBuildInputRequestTypeDef,
     DescribeComputeInputRequestTypeDef,
     DescribeEC2InstanceLimitsInputRequestTypeDef,
     EC2InstanceLimitTypeDef,
     PaginatorConfigTypeDef,
     DescribeFleetAttributesInputRequestTypeDef,
     DescribeFleetCapacityInputRequestTypeDef,
-    DescribeFleetEventsInputRequestTypeDef,
+    TimestampTypeDef,
     EventTypeDef,
     DescribeFleetLocationAttributesInputRequestTypeDef,
     DescribeFleetLocationCapacityInputRequestTypeDef,
     DescribeFleetLocationUtilizationInputRequestTypeDef,
     FleetUtilizationTypeDef,
     DescribeFleetPortSettingsInputRequestTypeDef,
     DescribeFleetUtilizationInputRequestTypeDef,
@@ -617,15 +618,14 @@
     CreatePlayerSessionsOutputTypeDef,
     DescribePlayerSessionsOutputTypeDef,
     CreateVpcPeeringAuthorizationOutputTypeDef,
     DescribeVpcPeeringAuthorizationsOutputTypeDef,
     DescribeEC2InstanceLimitsOutputTypeDef,
     DescribeFleetAttributesInputDescribeFleetAttributesPaginateTypeDef,
     DescribeFleetCapacityInputDescribeFleetCapacityPaginateTypeDef,
-    DescribeFleetEventsInputDescribeFleetEventsPaginateTypeDef,
     DescribeFleetUtilizationInputDescribeFleetUtilizationPaginateTypeDef,
     DescribeGameServerInstancesInputDescribeGameServerInstancesPaginateTypeDef,
     DescribeGameSessionDetailsInputDescribeGameSessionDetailsPaginateTypeDef,
     DescribeGameSessionQueuesInputDescribeGameSessionQueuesPaginateTypeDef,
     DescribeGameSessionsInputDescribeGameSessionsPaginateTypeDef,
     DescribeInstancesInputDescribeInstancesPaginateTypeDef,
     DescribeMatchmakingConfigurationsInputDescribeMatchmakingConfigurationsPaginateTypeDef,
@@ -637,37 +637,40 @@
     ListComputeInputListComputePaginateTypeDef,
     ListFleetsInputListFleetsPaginateTypeDef,
     ListGameServerGroupsInputListGameServerGroupsPaginateTypeDef,
     ListGameServersInputListGameServersPaginateTypeDef,
     ListLocationsInputListLocationsPaginateTypeDef,
     ListScriptsInputListScriptsPaginateTypeDef,
     SearchGameSessionsInputSearchGameSessionsPaginateTypeDef,
+    DescribeFleetEventsInputDescribeFleetEventsPaginateTypeDef,
+    DescribeFleetEventsInputRequestTypeDef,
     DescribeFleetEventsOutputTypeDef,
     DescribeFleetLocationUtilizationOutputTypeDef,
     DescribeFleetUtilizationOutputTypeDef,
     DescribeGameServerInstancesOutputTypeDef,
     DescribeInstancesOutputTypeDef,
     FleetCapacityTypeDef,
+    FilterConfigurationUnionTypeDef,
     GameServerGroupAutoScalingPolicyTypeDef,
     GameSessionConnectionInfoTypeDef,
     GameSessionPlacementTypeDef,
     StartGameSessionPlacementInputRequestTypeDef,
     GameSessionQueueTypeDef,
+    PriorityConfigurationUnionTypeDef,
     InstanceAccessTypeDef,
     PutScalingPolicyInputRequestTypeDef,
     ScalingPolicyTypeDef,
     RuntimeConfigurationOutputTypeDef,
     RuntimeConfigurationTypeDef,
     VpcPeeringConnectionTypeDef,
     CreateAliasOutputTypeDef,
     DescribeAliasOutputTypeDef,
     ListAliasesOutputTypeDef,
     UpdateAliasOutputTypeDef,
-    StartMatchBackfillInputRequestTypeDef,
-    StartMatchmakingInputRequestTypeDef,
+    PlayerUnionTypeDef,
     CreateScriptOutputTypeDef,
     DescribeScriptOutputTypeDef,
     ListScriptsOutputTypeDef,
     UpdateScriptOutputTypeDef,
     CreateFleetOutputTypeDef,
     DescribeFleetAttributesOutputTypeDef,
     DescribeFleetLocationAttributesOutputTypeDef,
@@ -697,24 +700,27 @@
     DescribeGameSessionQueuesOutputTypeDef,
     UpdateGameSessionQueueOutputTypeDef,
     GetInstanceAccessOutputTypeDef,
     DescribeScalingPoliciesOutputTypeDef,
     DescribeRuntimeConfigurationOutputTypeDef,
     UpdateRuntimeConfigurationOutputTypeDef,
     CreateFleetInputRequestTypeDef,
+    RuntimeConfigurationUnionTypeDef,
     UpdateRuntimeConfigurationInputRequestTypeDef,
     DescribeVpcPeeringConnectionsOutputTypeDef,
+    StartMatchBackfillInputRequestTypeDef,
+    StartMatchmakingInputRequestTypeDef,
     DescribeGameSessionDetailsOutputTypeDef,
     DescribeMatchmakingOutputTypeDef,
     StartMatchBackfillOutputTypeDef,
     StartMatchmakingOutputTypeDef,
 )
 
 
-def get_structure() -> AcceptMatchInputRequestTypeDef:
+def get_value() -> AcceptMatchInputRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-gamelift-1.28.15.post1/mypy_boto3_gamelift/__init__.py` & `mypy-boto3-gamelift-1.28.16/mypy_boto3_gamelift/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-gamelift-1.28.15.post1/mypy_boto3_gamelift/__init__.pyi` & `mypy-boto3-gamelift-1.28.16/mypy_boto3_gamelift/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-gamelift-1.28.15.post1/mypy_boto3_gamelift/__main__.py` & `mypy-boto3-gamelift-1.28.16/mypy_boto3_gamelift/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.GameLift 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.GameLift 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift\nOther"
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

### Comparing `mypy-boto3-gamelift-1.28.15.post1/mypy_boto3_gamelift/client.py` & `mypy-boto3-gamelift-1.28.16/mypy_boto3_gamelift/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,19 +10,17 @@
     from mypy_boto3_gamelift.client import GameLiftClient
 
     session = Session()
     client: GameLiftClient = session.client("gamelift")
     ```
 """
 import sys
-from datetime import datetime
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
-from botocore.response import StreamingBody
 
 from .literals import (
     AcceptanceTypeType,
     BackfillModeType,
     BalancingStrategyType,
     BuildStatusType,
     ComparisonOperatorTypeType,
@@ -66,14 +64,15 @@
     ListGameServersPaginator,
     ListLocationsPaginator,
     ListScriptsPaginator,
     SearchGameSessionsPaginator,
 )
 from .type_defs import (
     AnywhereConfigurationTypeDef,
+    BlobTypeDef,
     CertificateConfigurationTypeDef,
     ClaimFilterOptionTypeDef,
     ClaimGameServerOutputTypeDef,
     CreateAliasOutputTypeDef,
     CreateBuildOutputTypeDef,
     CreateFleetLocationsOutputTypeDef,
     CreateFleetOutputTypeDef,
@@ -116,16 +115,15 @@
     DescribeRuntimeConfigurationOutputTypeDef,
     DescribeScalingPoliciesOutputTypeDef,
     DescribeScriptOutputTypeDef,
     DescribeVpcPeeringAuthorizationsOutputTypeDef,
     DescribeVpcPeeringConnectionsOutputTypeDef,
     DesiredPlayerSessionTypeDef,
     EmptyResponseMetadataTypeDef,
-    FilterConfigurationOutputTypeDef,
-    FilterConfigurationTypeDef,
+    FilterConfigurationUnionTypeDef,
     GamePropertyTypeDef,
     GameServerGroupAutoScalingPolicyTypeDef,
     GameSessionQueueDestinationTypeDef,
     GetComputeAccessOutputTypeDef,
     GetComputeAuthTokenOutputTypeDef,
     GetGameSessionLogUrlOutputTypeDef,
     GetInstanceAccessOutputTypeDef,
@@ -140,39 +138,37 @@
     ListGameServersOutputTypeDef,
     ListLocationsOutputTypeDef,
     ListScriptsOutputTypeDef,
     ListTagsForResourceResponseTypeDef,
     LocationConfigurationTypeDef,
     PlayerLatencyPolicyTypeDef,
     PlayerLatencyTypeDef,
-    PlayerOutputTypeDef,
-    PlayerTypeDef,
-    PriorityConfigurationOutputTypeDef,
-    PriorityConfigurationTypeDef,
+    PlayerUnionTypeDef,
+    PriorityConfigurationUnionTypeDef,
     PutScalingPolicyOutputTypeDef,
     RegisterComputeOutputTypeDef,
     RegisterGameServerOutputTypeDef,
     RequestUploadCredentialsOutputTypeDef,
     ResolveAliasOutputTypeDef,
     ResourceCreationLimitPolicyTypeDef,
     ResumeGameServerGroupOutputTypeDef,
     RoutingStrategyTypeDef,
-    RuntimeConfigurationOutputTypeDef,
-    RuntimeConfigurationTypeDef,
+    RuntimeConfigurationUnionTypeDef,
     S3LocationTypeDef,
     SearchGameSessionsOutputTypeDef,
     StartFleetActionsOutputTypeDef,
     StartGameSessionPlacementOutputTypeDef,
     StartMatchBackfillOutputTypeDef,
     StartMatchmakingOutputTypeDef,
     StopFleetActionsOutputTypeDef,
     StopGameSessionPlacementOutputTypeDef,
     SuspendGameServerGroupOutputTypeDef,
     TagTypeDef,
     TargetConfigurationTypeDef,
+    TimestampTypeDef,
     UpdateAliasOutputTypeDef,
     UpdateBuildOutputTypeDef,
     UpdateFleetAttributesOutputTypeDef,
     UpdateFleetCapacityOutputTypeDef,
     UpdateFleetPortSettingsOutputTypeDef,
     UpdateGameServerGroupOutputTypeDef,
     UpdateGameServerOutputTypeDef,
@@ -321,17 +317,15 @@
         ScriptId: str = ...,
         ServerLaunchPath: str = ...,
         ServerLaunchParameters: str = ...,
         LogPaths: Sequence[str] = ...,
         EC2InstanceType: EC2InstanceTypeType = ...,
         EC2InboundPermissions: Sequence[IpPermissionTypeDef] = ...,
         NewGameSessionProtectionPolicy: ProtectionPolicyType = ...,
-        RuntimeConfiguration: Union[
-            RuntimeConfigurationTypeDef, RuntimeConfigurationOutputTypeDef
-        ] = ...,
+        RuntimeConfiguration: RuntimeConfigurationUnionTypeDef = ...,
         ResourceCreationLimitPolicy: ResourceCreationLimitPolicyTypeDef = ...,
         MetricGroups: Sequence[str] = ...,
         PeerVpcAwsAccountId: str = ...,
         PeerVpcId: str = ...,
         FleetType: FleetTypeType = ...,
         InstanceRoleArn: str = ...,
         CertificateConfiguration: CertificateConfigurationTypeDef = ...,
@@ -408,20 +402,16 @@
     def create_game_session_queue(
         self,
         *,
         Name: str,
         TimeoutInSeconds: int = ...,
         PlayerLatencyPolicies: Sequence[PlayerLatencyPolicyTypeDef] = ...,
         Destinations: Sequence[GameSessionQueueDestinationTypeDef] = ...,
-        FilterConfiguration: Union[
-            FilterConfigurationTypeDef, FilterConfigurationOutputTypeDef
-        ] = ...,
-        PriorityConfiguration: Union[
-            PriorityConfigurationTypeDef, PriorityConfigurationOutputTypeDef
-        ] = ...,
+        FilterConfiguration: FilterConfigurationUnionTypeDef = ...,
+        PriorityConfiguration: PriorityConfigurationUnionTypeDef = ...,
         CustomEventData: str = ...,
         NotificationTarget: str = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateGameSessionQueueOutputTypeDef:
         """
         Creates a placement queue that processes requests for new game sessions.
 
@@ -501,15 +491,15 @@
 
     def create_script(
         self,
         *,
         Name: str = ...,
         Version: str = ...,
         StorageLocation: S3LocationTypeDef = ...,
-        ZipFile: Union[str, bytes, IO[Any], StreamingBody] = ...,
+        ZipFile: BlobTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateScriptOutputTypeDef:
         """
         Creates a new script record for your Realtime Servers script.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.create_script)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#create_script)
@@ -727,16 +717,16 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#describe_fleet_capacity)
         """
 
     def describe_fleet_events(
         self,
         *,
         FleetId: str,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         Limit: int = ...,
         NextToken: str = ...
     ) -> DescribeFleetEventsOutputTypeDef:
         """
         Retrieves entries from a fleet's event log.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.describe_fleet_events)
@@ -1308,31 +1298,27 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#start_game_session_placement)
         """
 
     def start_match_backfill(
         self,
         *,
         ConfigurationName: str,
-        Players: Sequence[Union[PlayerTypeDef, PlayerOutputTypeDef]],
+        Players: Sequence[PlayerUnionTypeDef],
         TicketId: str = ...,
         GameSessionArn: str = ...
     ) -> StartMatchBackfillOutputTypeDef:
         """
         Finds new players to fill open slots in currently running game sessions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.start_match_backfill)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#start_match_backfill)
         """
 
     def start_matchmaking(
-        self,
-        *,
-        ConfigurationName: str,
-        Players: Sequence[Union[PlayerTypeDef, PlayerOutputTypeDef]],
-        TicketId: str = ...
+        self, *, ConfigurationName: str, Players: Sequence[PlayerUnionTypeDef], TicketId: str = ...
     ) -> StartMatchmakingOutputTypeDef:
         """
         Uses FlexMatch to create a game match for a group of players based on custom
         matchmaking rules.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.start_matchmaking)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#start_matchmaking)
@@ -1528,20 +1514,16 @@
     def update_game_session_queue(
         self,
         *,
         Name: str,
         TimeoutInSeconds: int = ...,
         PlayerLatencyPolicies: Sequence[PlayerLatencyPolicyTypeDef] = ...,
         Destinations: Sequence[GameSessionQueueDestinationTypeDef] = ...,
-        FilterConfiguration: Union[
-            FilterConfigurationTypeDef, FilterConfigurationOutputTypeDef
-        ] = ...,
-        PriorityConfiguration: Union[
-            PriorityConfigurationTypeDef, PriorityConfigurationOutputTypeDef
-        ] = ...,
+        FilterConfiguration: FilterConfigurationUnionTypeDef = ...,
+        PriorityConfiguration: PriorityConfigurationUnionTypeDef = ...,
         CustomEventData: str = ...,
         NotificationTarget: str = ...
     ) -> UpdateGameSessionQueueOutputTypeDef:
         """
         Updates the configuration of a game session queue, which determines how the
         queue processes new game session requests.
 
@@ -1571,18 +1553,15 @@
         Updates settings for a FlexMatch matchmaking configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.update_matchmaking_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#update_matchmaking_configuration)
         """
 
     def update_runtime_configuration(
-        self,
-        *,
-        FleetId: str,
-        RuntimeConfiguration: Union[RuntimeConfigurationTypeDef, RuntimeConfigurationOutputTypeDef]
+        self, *, FleetId: str, RuntimeConfiguration: RuntimeConfigurationUnionTypeDef
     ) -> UpdateRuntimeConfigurationOutputTypeDef:
         """
         Updates the current runtime configuration for the specified fleet, which tells
         Amazon GameLift how to launch server processes on all instances in the fleet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.update_runtime_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#update_runtime_configuration)
@@ -1591,15 +1570,15 @@
     def update_script(
         self,
         *,
         ScriptId: str,
         Name: str = ...,
         Version: str = ...,
         StorageLocation: S3LocationTypeDef = ...,
-        ZipFile: Union[str, bytes, IO[Any], StreamingBody] = ...
+        ZipFile: BlobTypeDef = ...
     ) -> UpdateScriptOutputTypeDef:
         """
         Updates Realtime script metadata and content.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.update_script)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#update_script)
         """
```

### Comparing `mypy-boto3-gamelift-1.28.15.post1/mypy_boto3_gamelift/client.pyi` & `mypy-boto3-gamelift-1.28.16/mypy_boto3_gamelift/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -10,19 +10,17 @@
     from mypy_boto3_gamelift.client import GameLiftClient
 
     session = Session()
     client: GameLiftClient = session.client("gamelift")
     ```
 """
 import sys
-from datetime import datetime
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
-from botocore.response import StreamingBody
 
 from .literals import (
     AcceptanceTypeType,
     BackfillModeType,
     BalancingStrategyType,
     BuildStatusType,
     ComparisonOperatorTypeType,
@@ -66,14 +64,15 @@
     ListGameServersPaginator,
     ListLocationsPaginator,
     ListScriptsPaginator,
     SearchGameSessionsPaginator,
 )
 from .type_defs import (
     AnywhereConfigurationTypeDef,
+    BlobTypeDef,
     CertificateConfigurationTypeDef,
     ClaimFilterOptionTypeDef,
     ClaimGameServerOutputTypeDef,
     CreateAliasOutputTypeDef,
     CreateBuildOutputTypeDef,
     CreateFleetLocationsOutputTypeDef,
     CreateFleetOutputTypeDef,
@@ -116,16 +115,15 @@
     DescribeRuntimeConfigurationOutputTypeDef,
     DescribeScalingPoliciesOutputTypeDef,
     DescribeScriptOutputTypeDef,
     DescribeVpcPeeringAuthorizationsOutputTypeDef,
     DescribeVpcPeeringConnectionsOutputTypeDef,
     DesiredPlayerSessionTypeDef,
     EmptyResponseMetadataTypeDef,
-    FilterConfigurationOutputTypeDef,
-    FilterConfigurationTypeDef,
+    FilterConfigurationUnionTypeDef,
     GamePropertyTypeDef,
     GameServerGroupAutoScalingPolicyTypeDef,
     GameSessionQueueDestinationTypeDef,
     GetComputeAccessOutputTypeDef,
     GetComputeAuthTokenOutputTypeDef,
     GetGameSessionLogUrlOutputTypeDef,
     GetInstanceAccessOutputTypeDef,
@@ -140,39 +138,37 @@
     ListGameServersOutputTypeDef,
     ListLocationsOutputTypeDef,
     ListScriptsOutputTypeDef,
     ListTagsForResourceResponseTypeDef,
     LocationConfigurationTypeDef,
     PlayerLatencyPolicyTypeDef,
     PlayerLatencyTypeDef,
-    PlayerOutputTypeDef,
-    PlayerTypeDef,
-    PriorityConfigurationOutputTypeDef,
-    PriorityConfigurationTypeDef,
+    PlayerUnionTypeDef,
+    PriorityConfigurationUnionTypeDef,
     PutScalingPolicyOutputTypeDef,
     RegisterComputeOutputTypeDef,
     RegisterGameServerOutputTypeDef,
     RequestUploadCredentialsOutputTypeDef,
     ResolveAliasOutputTypeDef,
     ResourceCreationLimitPolicyTypeDef,
     ResumeGameServerGroupOutputTypeDef,
     RoutingStrategyTypeDef,
-    RuntimeConfigurationOutputTypeDef,
-    RuntimeConfigurationTypeDef,
+    RuntimeConfigurationUnionTypeDef,
     S3LocationTypeDef,
     SearchGameSessionsOutputTypeDef,
     StartFleetActionsOutputTypeDef,
     StartGameSessionPlacementOutputTypeDef,
     StartMatchBackfillOutputTypeDef,
     StartMatchmakingOutputTypeDef,
     StopFleetActionsOutputTypeDef,
     StopGameSessionPlacementOutputTypeDef,
     SuspendGameServerGroupOutputTypeDef,
     TagTypeDef,
     TargetConfigurationTypeDef,
+    TimestampTypeDef,
     UpdateAliasOutputTypeDef,
     UpdateBuildOutputTypeDef,
     UpdateFleetAttributesOutputTypeDef,
     UpdateFleetCapacityOutputTypeDef,
     UpdateFleetPortSettingsOutputTypeDef,
     UpdateGameServerGroupOutputTypeDef,
     UpdateGameServerOutputTypeDef,
@@ -310,17 +306,15 @@
         ScriptId: str = ...,
         ServerLaunchPath: str = ...,
         ServerLaunchParameters: str = ...,
         LogPaths: Sequence[str] = ...,
         EC2InstanceType: EC2InstanceTypeType = ...,
         EC2InboundPermissions: Sequence[IpPermissionTypeDef] = ...,
         NewGameSessionProtectionPolicy: ProtectionPolicyType = ...,
-        RuntimeConfiguration: Union[
-            RuntimeConfigurationTypeDef, RuntimeConfigurationOutputTypeDef
-        ] = ...,
+        RuntimeConfiguration: RuntimeConfigurationUnionTypeDef = ...,
         ResourceCreationLimitPolicy: ResourceCreationLimitPolicyTypeDef = ...,
         MetricGroups: Sequence[str] = ...,
         PeerVpcAwsAccountId: str = ...,
         PeerVpcId: str = ...,
         FleetType: FleetTypeType = ...,
         InstanceRoleArn: str = ...,
         CertificateConfiguration: CertificateConfigurationTypeDef = ...,
@@ -393,20 +387,16 @@
     def create_game_session_queue(
         self,
         *,
         Name: str,
         TimeoutInSeconds: int = ...,
         PlayerLatencyPolicies: Sequence[PlayerLatencyPolicyTypeDef] = ...,
         Destinations: Sequence[GameSessionQueueDestinationTypeDef] = ...,
-        FilterConfiguration: Union[
-            FilterConfigurationTypeDef, FilterConfigurationOutputTypeDef
-        ] = ...,
-        PriorityConfiguration: Union[
-            PriorityConfigurationTypeDef, PriorityConfigurationOutputTypeDef
-        ] = ...,
+        FilterConfiguration: FilterConfigurationUnionTypeDef = ...,
+        PriorityConfiguration: PriorityConfigurationUnionTypeDef = ...,
         CustomEventData: str = ...,
         NotificationTarget: str = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateGameSessionQueueOutputTypeDef:
         """
         Creates a placement queue that processes requests for new game sessions.
 
@@ -480,15 +470,15 @@
         """
     def create_script(
         self,
         *,
         Name: str = ...,
         Version: str = ...,
         StorageLocation: S3LocationTypeDef = ...,
-        ZipFile: Union[str, bytes, IO[Any], StreamingBody] = ...,
+        ZipFile: BlobTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateScriptOutputTypeDef:
         """
         Creates a new script record for your Realtime Servers script.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.create_script)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#create_script)
@@ -682,16 +672,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.describe_fleet_capacity)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#describe_fleet_capacity)
         """
     def describe_fleet_events(
         self,
         *,
         FleetId: str,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         Limit: int = ...,
         NextToken: str = ...
     ) -> DescribeFleetEventsOutputTypeDef:
         """
         Retrieves entries from a fleet's event log.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.describe_fleet_events)
@@ -1217,30 +1207,26 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.start_game_session_placement)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#start_game_session_placement)
         """
     def start_match_backfill(
         self,
         *,
         ConfigurationName: str,
-        Players: Sequence[Union[PlayerTypeDef, PlayerOutputTypeDef]],
+        Players: Sequence[PlayerUnionTypeDef],
         TicketId: str = ...,
         GameSessionArn: str = ...
     ) -> StartMatchBackfillOutputTypeDef:
         """
         Finds new players to fill open slots in currently running game sessions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.start_match_backfill)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#start_match_backfill)
         """
     def start_matchmaking(
-        self,
-        *,
-        ConfigurationName: str,
-        Players: Sequence[Union[PlayerTypeDef, PlayerOutputTypeDef]],
-        TicketId: str = ...
+        self, *, ConfigurationName: str, Players: Sequence[PlayerUnionTypeDef], TicketId: str = ...
     ) -> StartMatchmakingOutputTypeDef:
         """
         Uses FlexMatch to create a game match for a group of players based on custom
         matchmaking rules.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.start_matchmaking)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#start_matchmaking)
@@ -1421,20 +1407,16 @@
     def update_game_session_queue(
         self,
         *,
         Name: str,
         TimeoutInSeconds: int = ...,
         PlayerLatencyPolicies: Sequence[PlayerLatencyPolicyTypeDef] = ...,
         Destinations: Sequence[GameSessionQueueDestinationTypeDef] = ...,
-        FilterConfiguration: Union[
-            FilterConfigurationTypeDef, FilterConfigurationOutputTypeDef
-        ] = ...,
-        PriorityConfiguration: Union[
-            PriorityConfigurationTypeDef, PriorityConfigurationOutputTypeDef
-        ] = ...,
+        FilterConfiguration: FilterConfigurationUnionTypeDef = ...,
+        PriorityConfiguration: PriorityConfigurationUnionTypeDef = ...,
         CustomEventData: str = ...,
         NotificationTarget: str = ...
     ) -> UpdateGameSessionQueueOutputTypeDef:
         """
         Updates the configuration of a game session queue, which determines how the
         queue processes new game session requests.
 
@@ -1462,18 +1444,15 @@
         """
         Updates settings for a FlexMatch matchmaking configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.update_matchmaking_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#update_matchmaking_configuration)
         """
     def update_runtime_configuration(
-        self,
-        *,
-        FleetId: str,
-        RuntimeConfiguration: Union[RuntimeConfigurationTypeDef, RuntimeConfigurationOutputTypeDef]
+        self, *, FleetId: str, RuntimeConfiguration: RuntimeConfigurationUnionTypeDef
     ) -> UpdateRuntimeConfigurationOutputTypeDef:
         """
         Updates the current runtime configuration for the specified fleet, which tells
         Amazon GameLift how to launch server processes on all instances in the fleet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.update_runtime_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#update_runtime_configuration)
@@ -1481,15 +1460,15 @@
     def update_script(
         self,
         *,
         ScriptId: str,
         Name: str = ...,
         Version: str = ...,
         StorageLocation: S3LocationTypeDef = ...,
-        ZipFile: Union[str, bytes, IO[Any], StreamingBody] = ...
+        ZipFile: BlobTypeDef = ...
     ) -> UpdateScriptOutputTypeDef:
         """
         Updates Realtime script metadata and content.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.update_script)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#update_script)
         """
```

### Comparing `mypy-boto3-gamelift-1.28.15.post1/mypy_boto3_gamelift/literals.py` & `mypy-boto3-gamelift-1.28.16/mypy_boto3_gamelift/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-gamelift-1.28.15.post1/mypy_boto3_gamelift/literals.pyi` & `mypy-boto3-gamelift-1.28.16/mypy_boto3_gamelift/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-gamelift-1.28.15.post1/mypy_boto3_gamelift/paginator.py` & `mypy-boto3-gamelift-1.28.16/mypy_boto3_gamelift/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,16 +57,15 @@
     list_game_server_groups_paginator: ListGameServerGroupsPaginator = client.get_paginator("list_game_server_groups")
     list_game_servers_paginator: ListGameServersPaginator = client.get_paginator("list_game_servers")
     list_locations_paginator: ListLocationsPaginator = client.get_paginator("list_locations")
     list_scripts_paginator: ListScriptsPaginator = client.get_paginator("list_scripts")
     search_game_sessions_paginator: SearchGameSessionsPaginator = client.get_paginator("search_game_sessions")
     ```
 """
-from datetime import datetime
-from typing import Generic, Iterator, Sequence, TypeVar, Union
+from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import (
     BuildStatusType,
     LocationFilterType,
     RoutingStrategyTypeType,
@@ -93,14 +92,15 @@
     ListFleetsOutputTypeDef,
     ListGameServerGroupsOutputTypeDef,
     ListGameServersOutputTypeDef,
     ListLocationsOutputTypeDef,
     ListScriptsOutputTypeDef,
     PaginatorConfigTypeDef,
     SearchGameSessionsOutputTypeDef,
+    TimestampTypeDef,
 )
 
 __all__ = (
     "DescribeFleetAttributesPaginator",
     "DescribeFleetCapacityPaginator",
     "DescribeFleetEventsPaginator",
     "DescribeFleetUtilizationPaginator",
@@ -171,16 +171,16 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/paginators/#describefleeteventspaginator)
     """
 
     def paginate(
         self,
         *,
         FleetId: str,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeFleetEventsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Paginator.DescribeFleetEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/paginators/#describefleeteventspaginator)
         """
```

### Comparing `mypy-boto3-gamelift-1.28.15.post1/mypy_boto3_gamelift/paginator.pyi` & `mypy-boto3-gamelift-1.28.16/mypy_boto3_gamelift/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -57,16 +57,15 @@
     list_game_server_groups_paginator: ListGameServerGroupsPaginator = client.get_paginator("list_game_server_groups")
     list_game_servers_paginator: ListGameServersPaginator = client.get_paginator("list_game_servers")
     list_locations_paginator: ListLocationsPaginator = client.get_paginator("list_locations")
     list_scripts_paginator: ListScriptsPaginator = client.get_paginator("list_scripts")
     search_game_sessions_paginator: SearchGameSessionsPaginator = client.get_paginator("search_game_sessions")
     ```
 """
-from datetime import datetime
-from typing import Generic, Iterator, Sequence, TypeVar, Union
+from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import (
     BuildStatusType,
     LocationFilterType,
     RoutingStrategyTypeType,
@@ -93,14 +92,15 @@
     ListFleetsOutputTypeDef,
     ListGameServerGroupsOutputTypeDef,
     ListGameServersOutputTypeDef,
     ListLocationsOutputTypeDef,
     ListScriptsOutputTypeDef,
     PaginatorConfigTypeDef,
     SearchGameSessionsOutputTypeDef,
+    TimestampTypeDef,
 )
 
 __all__ = (
     "DescribeFleetAttributesPaginator",
     "DescribeFleetCapacityPaginator",
     "DescribeFleetEventsPaginator",
     "DescribeFleetUtilizationPaginator",
@@ -166,16 +166,16 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/paginators/#describefleeteventspaginator)
     """
 
     def paginate(
         self,
         *,
         FleetId: str,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeFleetEventsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Paginator.DescribeFleetEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/paginators/#describefleeteventspaginator)
         """
```

### Comparing `mypy-boto3-gamelift-1.28.15.post1/mypy_boto3_gamelift/type_defs.py` & `mypy-boto3-gamelift-1.28.16/mypy_boto3_gamelift/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_gamelift.type_defs import AcceptMatchInputRequestTypeDef
 
-    data: AcceptMatchInputRequestTypeDef = {...}
+    data: AcceptMatchInputRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -70,14 +70,15 @@
 __all__ = (
     "AcceptMatchInputRequestTypeDef",
     "RoutingStrategyTypeDef",
     "AnywhereConfigurationTypeDef",
     "AttributeValueOutputTypeDef",
     "AttributeValueTypeDef",
     "AwsCredentialsTypeDef",
+    "BlobTypeDef",
     "BuildTypeDef",
     "CertificateConfigurationTypeDef",
     "ClaimFilterOptionTypeDef",
     "GameServerTypeDef",
     "ResponseMetadataTypeDef",
     "ComputeTypeDef",
     "TagTypeDef",
@@ -120,15 +121,15 @@
     "DescribeBuildInputRequestTypeDef",
     "DescribeComputeInputRequestTypeDef",
     "DescribeEC2InstanceLimitsInputRequestTypeDef",
     "EC2InstanceLimitTypeDef",
     "PaginatorConfigTypeDef",
     "DescribeFleetAttributesInputRequestTypeDef",
     "DescribeFleetCapacityInputRequestTypeDef",
-    "DescribeFleetEventsInputRequestTypeDef",
+    "TimestampTypeDef",
     "EventTypeDef",
     "DescribeFleetLocationAttributesInputRequestTypeDef",
     "DescribeFleetLocationCapacityInputRequestTypeDef",
     "DescribeFleetLocationUtilizationInputRequestTypeDef",
     "FleetUtilizationTypeDef",
     "DescribeFleetPortSettingsInputRequestTypeDef",
     "DescribeFleetUtilizationInputRequestTypeDef",
@@ -257,15 +258,14 @@
     "CreatePlayerSessionsOutputTypeDef",
     "DescribePlayerSessionsOutputTypeDef",
     "CreateVpcPeeringAuthorizationOutputTypeDef",
     "DescribeVpcPeeringAuthorizationsOutputTypeDef",
     "DescribeEC2InstanceLimitsOutputTypeDef",
     "DescribeFleetAttributesInputDescribeFleetAttributesPaginateTypeDef",
     "DescribeFleetCapacityInputDescribeFleetCapacityPaginateTypeDef",
-    "DescribeFleetEventsInputDescribeFleetEventsPaginateTypeDef",
     "DescribeFleetUtilizationInputDescribeFleetUtilizationPaginateTypeDef",
     "DescribeGameServerInstancesInputDescribeGameServerInstancesPaginateTypeDef",
     "DescribeGameSessionDetailsInputDescribeGameSessionDetailsPaginateTypeDef",
     "DescribeGameSessionQueuesInputDescribeGameSessionQueuesPaginateTypeDef",
     "DescribeGameSessionsInputDescribeGameSessionsPaginateTypeDef",
     "DescribeInstancesInputDescribeInstancesPaginateTypeDef",
     "DescribeMatchmakingConfigurationsInputDescribeMatchmakingConfigurationsPaginateTypeDef",
@@ -277,37 +277,40 @@
     "ListComputeInputListComputePaginateTypeDef",
     "ListFleetsInputListFleetsPaginateTypeDef",
     "ListGameServerGroupsInputListGameServerGroupsPaginateTypeDef",
     "ListGameServersInputListGameServersPaginateTypeDef",
     "ListLocationsInputListLocationsPaginateTypeDef",
     "ListScriptsInputListScriptsPaginateTypeDef",
     "SearchGameSessionsInputSearchGameSessionsPaginateTypeDef",
+    "DescribeFleetEventsInputDescribeFleetEventsPaginateTypeDef",
+    "DescribeFleetEventsInputRequestTypeDef",
     "DescribeFleetEventsOutputTypeDef",
     "DescribeFleetLocationUtilizationOutputTypeDef",
     "DescribeFleetUtilizationOutputTypeDef",
     "DescribeGameServerInstancesOutputTypeDef",
     "DescribeInstancesOutputTypeDef",
     "FleetCapacityTypeDef",
+    "FilterConfigurationUnionTypeDef",
     "GameServerGroupAutoScalingPolicyTypeDef",
     "GameSessionConnectionInfoTypeDef",
     "GameSessionPlacementTypeDef",
     "StartGameSessionPlacementInputRequestTypeDef",
     "GameSessionQueueTypeDef",
+    "PriorityConfigurationUnionTypeDef",
     "InstanceAccessTypeDef",
     "PutScalingPolicyInputRequestTypeDef",
     "ScalingPolicyTypeDef",
     "RuntimeConfigurationOutputTypeDef",
     "RuntimeConfigurationTypeDef",
     "VpcPeeringConnectionTypeDef",
     "CreateAliasOutputTypeDef",
     "DescribeAliasOutputTypeDef",
     "ListAliasesOutputTypeDef",
     "UpdateAliasOutputTypeDef",
-    "StartMatchBackfillInputRequestTypeDef",
-    "StartMatchmakingInputRequestTypeDef",
+    "PlayerUnionTypeDef",
     "CreateScriptOutputTypeDef",
     "DescribeScriptOutputTypeDef",
     "ListScriptsOutputTypeDef",
     "UpdateScriptOutputTypeDef",
     "CreateFleetOutputTypeDef",
     "DescribeFleetAttributesOutputTypeDef",
     "DescribeFleetLocationAttributesOutputTypeDef",
@@ -337,16 +340,19 @@
     "DescribeGameSessionQueuesOutputTypeDef",
     "UpdateGameSessionQueueOutputTypeDef",
     "GetInstanceAccessOutputTypeDef",
     "DescribeScalingPoliciesOutputTypeDef",
     "DescribeRuntimeConfigurationOutputTypeDef",
     "UpdateRuntimeConfigurationOutputTypeDef",
     "CreateFleetInputRequestTypeDef",
+    "RuntimeConfigurationUnionTypeDef",
     "UpdateRuntimeConfigurationInputRequestTypeDef",
     "DescribeVpcPeeringConnectionsOutputTypeDef",
+    "StartMatchBackfillInputRequestTypeDef",
+    "StartMatchmakingInputRequestTypeDef",
     "DescribeGameSessionDetailsOutputTypeDef",
     "DescribeMatchmakingOutputTypeDef",
     "StartMatchBackfillOutputTypeDef",
     "StartMatchmakingOutputTypeDef",
 )
 
 AcceptMatchInputRequestTypeDef = TypedDict(
@@ -403,14 +409,15 @@
         "AccessKeyId": str,
         "SecretAccessKey": str,
         "SessionToken": str,
     },
     total=False,
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 BuildTypeDef = TypedDict(
     "BuildTypeDef",
     {
         "BuildId": str,
         "BuildArn": str,
         "Name": str,
         "Version": str,
@@ -932,38 +939,15 @@
         "FleetIds": Sequence[str],
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
-_RequiredDescribeFleetEventsInputRequestTypeDef = TypedDict(
-    "_RequiredDescribeFleetEventsInputRequestTypeDef",
-    {
-        "FleetId": str,
-    },
-)
-_OptionalDescribeFleetEventsInputRequestTypeDef = TypedDict(
-    "_OptionalDescribeFleetEventsInputRequestTypeDef",
-    {
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "Limit": int,
-        "NextToken": str,
-    },
-    total=False,
-)
-
-
-class DescribeFleetEventsInputRequestTypeDef(
-    _RequiredDescribeFleetEventsInputRequestTypeDef, _OptionalDescribeFleetEventsInputRequestTypeDef
-):
-    pass
-
-
+TimestampTypeDef = Union[datetime, str]
 EventTypeDef = TypedDict(
     "EventTypeDef",
     {
         "EventId": str,
         "ResourceId": str,
         "EventCode": EventCodeType,
         "Message": str,
@@ -2208,15 +2192,15 @@
 
 CreateScriptInputRequestTypeDef = TypedDict(
     "CreateScriptInputRequestTypeDef",
     {
         "Name": str,
         "Version": str,
         "StorageLocation": S3LocationTypeDef,
-        "ZipFile": Union[str, bytes, IO[Any], StreamingBody],
+        "ZipFile": BlobTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
 RequestUploadCredentialsOutputTypeDef = TypedDict(
     "RequestUploadCredentialsOutputTypeDef",
@@ -2249,15 +2233,15 @@
 )
 _OptionalUpdateScriptInputRequestTypeDef = TypedDict(
     "_OptionalUpdateScriptInputRequestTypeDef",
     {
         "Name": str,
         "Version": str,
         "StorageLocation": S3LocationTypeDef,
-        "ZipFile": Union[str, bytes, IO[Any], StreamingBody],
+        "ZipFile": BlobTypeDef,
     },
     total=False,
 )
 
 
 class UpdateScriptInputRequestTypeDef(
     _RequiredUpdateScriptInputRequestTypeDef, _OptionalUpdateScriptInputRequestTypeDef
@@ -2743,38 +2727,14 @@
     {
         "FleetIds": Sequence[str],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-_RequiredDescribeFleetEventsInputDescribeFleetEventsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeFleetEventsInputDescribeFleetEventsPaginateTypeDef",
-    {
-        "FleetId": str,
-    },
-)
-_OptionalDescribeFleetEventsInputDescribeFleetEventsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeFleetEventsInputDescribeFleetEventsPaginateTypeDef",
-    {
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class DescribeFleetEventsInputDescribeFleetEventsPaginateTypeDef(
-    _RequiredDescribeFleetEventsInputDescribeFleetEventsPaginateTypeDef,
-    _OptionalDescribeFleetEventsInputDescribeFleetEventsPaginateTypeDef,
-):
-    pass
-
-
 DescribeFleetUtilizationInputDescribeFleetUtilizationPaginateTypeDef = TypedDict(
     "DescribeFleetUtilizationInputDescribeFleetUtilizationPaginateTypeDef",
     {
         "FleetIds": Sequence[str],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -3026,14 +2986,62 @@
         "FilterExpression": str,
         "SortExpression": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+_RequiredDescribeFleetEventsInputDescribeFleetEventsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeFleetEventsInputDescribeFleetEventsPaginateTypeDef",
+    {
+        "FleetId": str,
+    },
+)
+_OptionalDescribeFleetEventsInputDescribeFleetEventsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeFleetEventsInputDescribeFleetEventsPaginateTypeDef",
+    {
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeFleetEventsInputDescribeFleetEventsPaginateTypeDef(
+    _RequiredDescribeFleetEventsInputDescribeFleetEventsPaginateTypeDef,
+    _OptionalDescribeFleetEventsInputDescribeFleetEventsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredDescribeFleetEventsInputRequestTypeDef = TypedDict(
+    "_RequiredDescribeFleetEventsInputRequestTypeDef",
+    {
+        "FleetId": str,
+    },
+)
+_OptionalDescribeFleetEventsInputRequestTypeDef = TypedDict(
+    "_OptionalDescribeFleetEventsInputRequestTypeDef",
+    {
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "Limit": int,
+        "NextToken": str,
+    },
+    total=False,
+)
+
+
+class DescribeFleetEventsInputRequestTypeDef(
+    _RequiredDescribeFleetEventsInputRequestTypeDef, _OptionalDescribeFleetEventsInputRequestTypeDef
+):
+    pass
+
+
 DescribeFleetEventsOutputTypeDef = TypedDict(
     "DescribeFleetEventsOutputTypeDef",
     {
         "Events": List[EventTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -3082,14 +3090,17 @@
         "InstanceType": EC2InstanceTypeType,
         "InstanceCounts": EC2InstanceCountsTypeDef,
         "Location": str,
     },
     total=False,
 )
 
+FilterConfigurationUnionTypeDef = Union[
+    FilterConfigurationTypeDef, FilterConfigurationOutputTypeDef
+]
 _RequiredGameServerGroupAutoScalingPolicyTypeDef = TypedDict(
     "_RequiredGameServerGroupAutoScalingPolicyTypeDef",
     {
         "TargetTrackingConfiguration": TargetTrackingConfigurationTypeDef,
     },
 )
 _OptionalGameServerGroupAutoScalingPolicyTypeDef = TypedDict(
@@ -3185,14 +3196,17 @@
         "PriorityConfiguration": PriorityConfigurationOutputTypeDef,
         "CustomEventData": str,
         "NotificationTarget": str,
     },
     total=False,
 )
 
+PriorityConfigurationUnionTypeDef = Union[
+    PriorityConfigurationTypeDef, PriorityConfigurationOutputTypeDef
+]
 InstanceAccessTypeDef = TypedDict(
     "InstanceAccessTypeDef",
     {
         "FleetId": str,
         "InstanceId": str,
         "IpAddress": str,
         "OperatingSystem": OperatingSystemType,
@@ -3314,59 +3328,15 @@
     "UpdateAliasOutputTypeDef",
     {
         "Alias": AliasTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredStartMatchBackfillInputRequestTypeDef = TypedDict(
-    "_RequiredStartMatchBackfillInputRequestTypeDef",
-    {
-        "ConfigurationName": str,
-        "Players": Sequence[Union[PlayerTypeDef, PlayerOutputTypeDef]],
-    },
-)
-_OptionalStartMatchBackfillInputRequestTypeDef = TypedDict(
-    "_OptionalStartMatchBackfillInputRequestTypeDef",
-    {
-        "TicketId": str,
-        "GameSessionArn": str,
-    },
-    total=False,
-)
-
-
-class StartMatchBackfillInputRequestTypeDef(
-    _RequiredStartMatchBackfillInputRequestTypeDef, _OptionalStartMatchBackfillInputRequestTypeDef
-):
-    pass
-
-
-_RequiredStartMatchmakingInputRequestTypeDef = TypedDict(
-    "_RequiredStartMatchmakingInputRequestTypeDef",
-    {
-        "ConfigurationName": str,
-        "Players": Sequence[Union[PlayerTypeDef, PlayerOutputTypeDef]],
-    },
-)
-_OptionalStartMatchmakingInputRequestTypeDef = TypedDict(
-    "_OptionalStartMatchmakingInputRequestTypeDef",
-    {
-        "TicketId": str,
-    },
-    total=False,
-)
-
-
-class StartMatchmakingInputRequestTypeDef(
-    _RequiredStartMatchmakingInputRequestTypeDef, _OptionalStartMatchmakingInputRequestTypeDef
-):
-    pass
-
-
+PlayerUnionTypeDef = Union[PlayerTypeDef, PlayerOutputTypeDef]
 CreateScriptOutputTypeDef = TypedDict(
     "CreateScriptOutputTypeDef",
     {
         "Script": ScriptTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -3735,14 +3705,17 @@
 
 class CreateFleetInputRequestTypeDef(
     _RequiredCreateFleetInputRequestTypeDef, _OptionalCreateFleetInputRequestTypeDef
 ):
     pass
 
 
+RuntimeConfigurationUnionTypeDef = Union[
+    RuntimeConfigurationTypeDef, RuntimeConfigurationOutputTypeDef
+]
 UpdateRuntimeConfigurationInputRequestTypeDef = TypedDict(
     "UpdateRuntimeConfigurationInputRequestTypeDef",
     {
         "FleetId": str,
         "RuntimeConfiguration": RuntimeConfigurationTypeDef,
     },
 )
@@ -3751,14 +3724,59 @@
     "DescribeVpcPeeringConnectionsOutputTypeDef",
     {
         "VpcPeeringConnections": List[VpcPeeringConnectionTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredStartMatchBackfillInputRequestTypeDef = TypedDict(
+    "_RequiredStartMatchBackfillInputRequestTypeDef",
+    {
+        "ConfigurationName": str,
+        "Players": Sequence[PlayerUnionTypeDef],
+    },
+)
+_OptionalStartMatchBackfillInputRequestTypeDef = TypedDict(
+    "_OptionalStartMatchBackfillInputRequestTypeDef",
+    {
+        "TicketId": str,
+        "GameSessionArn": str,
+    },
+    total=False,
+)
+
+
+class StartMatchBackfillInputRequestTypeDef(
+    _RequiredStartMatchBackfillInputRequestTypeDef, _OptionalStartMatchBackfillInputRequestTypeDef
+):
+    pass
+
+
+_RequiredStartMatchmakingInputRequestTypeDef = TypedDict(
+    "_RequiredStartMatchmakingInputRequestTypeDef",
+    {
+        "ConfigurationName": str,
+        "Players": Sequence[PlayerUnionTypeDef],
+    },
+)
+_OptionalStartMatchmakingInputRequestTypeDef = TypedDict(
+    "_OptionalStartMatchmakingInputRequestTypeDef",
+    {
+        "TicketId": str,
+    },
+    total=False,
+)
+
+
+class StartMatchmakingInputRequestTypeDef(
+    _RequiredStartMatchmakingInputRequestTypeDef, _OptionalStartMatchmakingInputRequestTypeDef
+):
+    pass
+
+
 DescribeGameSessionDetailsOutputTypeDef = TypedDict(
     "DescribeGameSessionDetailsOutputTypeDef",
     {
         "GameSessionDetails": List[GameSessionDetailTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-gamelift-1.28.15.post1/mypy_boto3_gamelift/type_defs.pyi` & `mypy-boto3-gamelift-1.28.16/mypy_boto3_gamelift/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_gamelift.type_defs import AcceptMatchInputRequestTypeDef
 
-    data: AcceptMatchInputRequestTypeDef = {...}
+    data: AcceptMatchInputRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -69,14 +69,15 @@
 __all__ = (
     "AcceptMatchInputRequestTypeDef",
     "RoutingStrategyTypeDef",
     "AnywhereConfigurationTypeDef",
     "AttributeValueOutputTypeDef",
     "AttributeValueTypeDef",
     "AwsCredentialsTypeDef",
+    "BlobTypeDef",
     "BuildTypeDef",
     "CertificateConfigurationTypeDef",
     "ClaimFilterOptionTypeDef",
     "GameServerTypeDef",
     "ResponseMetadataTypeDef",
     "ComputeTypeDef",
     "TagTypeDef",
@@ -119,15 +120,15 @@
     "DescribeBuildInputRequestTypeDef",
     "DescribeComputeInputRequestTypeDef",
     "DescribeEC2InstanceLimitsInputRequestTypeDef",
     "EC2InstanceLimitTypeDef",
     "PaginatorConfigTypeDef",
     "DescribeFleetAttributesInputRequestTypeDef",
     "DescribeFleetCapacityInputRequestTypeDef",
-    "DescribeFleetEventsInputRequestTypeDef",
+    "TimestampTypeDef",
     "EventTypeDef",
     "DescribeFleetLocationAttributesInputRequestTypeDef",
     "DescribeFleetLocationCapacityInputRequestTypeDef",
     "DescribeFleetLocationUtilizationInputRequestTypeDef",
     "FleetUtilizationTypeDef",
     "DescribeFleetPortSettingsInputRequestTypeDef",
     "DescribeFleetUtilizationInputRequestTypeDef",
@@ -256,15 +257,14 @@
     "CreatePlayerSessionsOutputTypeDef",
     "DescribePlayerSessionsOutputTypeDef",
     "CreateVpcPeeringAuthorizationOutputTypeDef",
     "DescribeVpcPeeringAuthorizationsOutputTypeDef",
     "DescribeEC2InstanceLimitsOutputTypeDef",
     "DescribeFleetAttributesInputDescribeFleetAttributesPaginateTypeDef",
     "DescribeFleetCapacityInputDescribeFleetCapacityPaginateTypeDef",
-    "DescribeFleetEventsInputDescribeFleetEventsPaginateTypeDef",
     "DescribeFleetUtilizationInputDescribeFleetUtilizationPaginateTypeDef",
     "DescribeGameServerInstancesInputDescribeGameServerInstancesPaginateTypeDef",
     "DescribeGameSessionDetailsInputDescribeGameSessionDetailsPaginateTypeDef",
     "DescribeGameSessionQueuesInputDescribeGameSessionQueuesPaginateTypeDef",
     "DescribeGameSessionsInputDescribeGameSessionsPaginateTypeDef",
     "DescribeInstancesInputDescribeInstancesPaginateTypeDef",
     "DescribeMatchmakingConfigurationsInputDescribeMatchmakingConfigurationsPaginateTypeDef",
@@ -276,37 +276,40 @@
     "ListComputeInputListComputePaginateTypeDef",
     "ListFleetsInputListFleetsPaginateTypeDef",
     "ListGameServerGroupsInputListGameServerGroupsPaginateTypeDef",
     "ListGameServersInputListGameServersPaginateTypeDef",
     "ListLocationsInputListLocationsPaginateTypeDef",
     "ListScriptsInputListScriptsPaginateTypeDef",
     "SearchGameSessionsInputSearchGameSessionsPaginateTypeDef",
+    "DescribeFleetEventsInputDescribeFleetEventsPaginateTypeDef",
+    "DescribeFleetEventsInputRequestTypeDef",
     "DescribeFleetEventsOutputTypeDef",
     "DescribeFleetLocationUtilizationOutputTypeDef",
     "DescribeFleetUtilizationOutputTypeDef",
     "DescribeGameServerInstancesOutputTypeDef",
     "DescribeInstancesOutputTypeDef",
     "FleetCapacityTypeDef",
+    "FilterConfigurationUnionTypeDef",
     "GameServerGroupAutoScalingPolicyTypeDef",
     "GameSessionConnectionInfoTypeDef",
     "GameSessionPlacementTypeDef",
     "StartGameSessionPlacementInputRequestTypeDef",
     "GameSessionQueueTypeDef",
+    "PriorityConfigurationUnionTypeDef",
     "InstanceAccessTypeDef",
     "PutScalingPolicyInputRequestTypeDef",
     "ScalingPolicyTypeDef",
     "RuntimeConfigurationOutputTypeDef",
     "RuntimeConfigurationTypeDef",
     "VpcPeeringConnectionTypeDef",
     "CreateAliasOutputTypeDef",
     "DescribeAliasOutputTypeDef",
     "ListAliasesOutputTypeDef",
     "UpdateAliasOutputTypeDef",
-    "StartMatchBackfillInputRequestTypeDef",
-    "StartMatchmakingInputRequestTypeDef",
+    "PlayerUnionTypeDef",
     "CreateScriptOutputTypeDef",
     "DescribeScriptOutputTypeDef",
     "ListScriptsOutputTypeDef",
     "UpdateScriptOutputTypeDef",
     "CreateFleetOutputTypeDef",
     "DescribeFleetAttributesOutputTypeDef",
     "DescribeFleetLocationAttributesOutputTypeDef",
@@ -336,16 +339,19 @@
     "DescribeGameSessionQueuesOutputTypeDef",
     "UpdateGameSessionQueueOutputTypeDef",
     "GetInstanceAccessOutputTypeDef",
     "DescribeScalingPoliciesOutputTypeDef",
     "DescribeRuntimeConfigurationOutputTypeDef",
     "UpdateRuntimeConfigurationOutputTypeDef",
     "CreateFleetInputRequestTypeDef",
+    "RuntimeConfigurationUnionTypeDef",
     "UpdateRuntimeConfigurationInputRequestTypeDef",
     "DescribeVpcPeeringConnectionsOutputTypeDef",
+    "StartMatchBackfillInputRequestTypeDef",
+    "StartMatchmakingInputRequestTypeDef",
     "DescribeGameSessionDetailsOutputTypeDef",
     "DescribeMatchmakingOutputTypeDef",
     "StartMatchBackfillOutputTypeDef",
     "StartMatchmakingOutputTypeDef",
 )
 
 AcceptMatchInputRequestTypeDef = TypedDict(
@@ -402,14 +408,15 @@
         "AccessKeyId": str,
         "SecretAccessKey": str,
         "SessionToken": str,
     },
     total=False,
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 BuildTypeDef = TypedDict(
     "BuildTypeDef",
     {
         "BuildId": str,
         "BuildArn": str,
         "Name": str,
         "Version": str,
@@ -921,36 +928,15 @@
         "FleetIds": Sequence[str],
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
-_RequiredDescribeFleetEventsInputRequestTypeDef = TypedDict(
-    "_RequiredDescribeFleetEventsInputRequestTypeDef",
-    {
-        "FleetId": str,
-    },
-)
-_OptionalDescribeFleetEventsInputRequestTypeDef = TypedDict(
-    "_OptionalDescribeFleetEventsInputRequestTypeDef",
-    {
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "Limit": int,
-        "NextToken": str,
-    },
-    total=False,
-)
-
-class DescribeFleetEventsInputRequestTypeDef(
-    _RequiredDescribeFleetEventsInputRequestTypeDef, _OptionalDescribeFleetEventsInputRequestTypeDef
-):
-    pass
-
+TimestampTypeDef = Union[datetime, str]
 EventTypeDef = TypedDict(
     "EventTypeDef",
     {
         "EventId": str,
         "ResourceId": str,
         "EventCode": EventCodeType,
         "Message": str,
@@ -2153,15 +2139,15 @@
 
 CreateScriptInputRequestTypeDef = TypedDict(
     "CreateScriptInputRequestTypeDef",
     {
         "Name": str,
         "Version": str,
         "StorageLocation": S3LocationTypeDef,
-        "ZipFile": Union[str, bytes, IO[Any], StreamingBody],
+        "ZipFile": BlobTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
 RequestUploadCredentialsOutputTypeDef = TypedDict(
     "RequestUploadCredentialsOutputTypeDef",
@@ -2194,15 +2180,15 @@
 )
 _OptionalUpdateScriptInputRequestTypeDef = TypedDict(
     "_OptionalUpdateScriptInputRequestTypeDef",
     {
         "Name": str,
         "Version": str,
         "StorageLocation": S3LocationTypeDef,
-        "ZipFile": Union[str, bytes, IO[Any], StreamingBody],
+        "ZipFile": BlobTypeDef,
     },
     total=False,
 )
 
 class UpdateScriptInputRequestTypeDef(
     _RequiredUpdateScriptInputRequestTypeDef, _OptionalUpdateScriptInputRequestTypeDef
 ):
@@ -2670,36 +2656,14 @@
     {
         "FleetIds": Sequence[str],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-_RequiredDescribeFleetEventsInputDescribeFleetEventsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeFleetEventsInputDescribeFleetEventsPaginateTypeDef",
-    {
-        "FleetId": str,
-    },
-)
-_OptionalDescribeFleetEventsInputDescribeFleetEventsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeFleetEventsInputDescribeFleetEventsPaginateTypeDef",
-    {
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class DescribeFleetEventsInputDescribeFleetEventsPaginateTypeDef(
-    _RequiredDescribeFleetEventsInputDescribeFleetEventsPaginateTypeDef,
-    _OptionalDescribeFleetEventsInputDescribeFleetEventsPaginateTypeDef,
-):
-    pass
-
 DescribeFleetUtilizationInputDescribeFleetUtilizationPaginateTypeDef = TypedDict(
     "DescribeFleetUtilizationInputDescribeFleetUtilizationPaginateTypeDef",
     {
         "FleetIds": Sequence[str],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -2941,14 +2905,58 @@
         "FilterExpression": str,
         "SortExpression": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+_RequiredDescribeFleetEventsInputDescribeFleetEventsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeFleetEventsInputDescribeFleetEventsPaginateTypeDef",
+    {
+        "FleetId": str,
+    },
+)
+_OptionalDescribeFleetEventsInputDescribeFleetEventsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeFleetEventsInputDescribeFleetEventsPaginateTypeDef",
+    {
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeFleetEventsInputDescribeFleetEventsPaginateTypeDef(
+    _RequiredDescribeFleetEventsInputDescribeFleetEventsPaginateTypeDef,
+    _OptionalDescribeFleetEventsInputDescribeFleetEventsPaginateTypeDef,
+):
+    pass
+
+_RequiredDescribeFleetEventsInputRequestTypeDef = TypedDict(
+    "_RequiredDescribeFleetEventsInputRequestTypeDef",
+    {
+        "FleetId": str,
+    },
+)
+_OptionalDescribeFleetEventsInputRequestTypeDef = TypedDict(
+    "_OptionalDescribeFleetEventsInputRequestTypeDef",
+    {
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "Limit": int,
+        "NextToken": str,
+    },
+    total=False,
+)
+
+class DescribeFleetEventsInputRequestTypeDef(
+    _RequiredDescribeFleetEventsInputRequestTypeDef, _OptionalDescribeFleetEventsInputRequestTypeDef
+):
+    pass
+
 DescribeFleetEventsOutputTypeDef = TypedDict(
     "DescribeFleetEventsOutputTypeDef",
     {
         "Events": List[EventTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2997,14 +3005,17 @@
         "InstanceType": EC2InstanceTypeType,
         "InstanceCounts": EC2InstanceCountsTypeDef,
         "Location": str,
     },
     total=False,
 )
 
+FilterConfigurationUnionTypeDef = Union[
+    FilterConfigurationTypeDef, FilterConfigurationOutputTypeDef
+]
 _RequiredGameServerGroupAutoScalingPolicyTypeDef = TypedDict(
     "_RequiredGameServerGroupAutoScalingPolicyTypeDef",
     {
         "TargetTrackingConfiguration": TargetTrackingConfigurationTypeDef,
     },
 )
 _OptionalGameServerGroupAutoScalingPolicyTypeDef = TypedDict(
@@ -3096,14 +3107,17 @@
         "PriorityConfiguration": PriorityConfigurationOutputTypeDef,
         "CustomEventData": str,
         "NotificationTarget": str,
     },
     total=False,
 )
 
+PriorityConfigurationUnionTypeDef = Union[
+    PriorityConfigurationTypeDef, PriorityConfigurationOutputTypeDef
+]
 InstanceAccessTypeDef = TypedDict(
     "InstanceAccessTypeDef",
     {
         "FleetId": str,
         "InstanceId": str,
         "IpAddress": str,
         "OperatingSystem": OperatingSystemType,
@@ -3223,55 +3237,15 @@
     "UpdateAliasOutputTypeDef",
     {
         "Alias": AliasTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredStartMatchBackfillInputRequestTypeDef = TypedDict(
-    "_RequiredStartMatchBackfillInputRequestTypeDef",
-    {
-        "ConfigurationName": str,
-        "Players": Sequence[Union[PlayerTypeDef, PlayerOutputTypeDef]],
-    },
-)
-_OptionalStartMatchBackfillInputRequestTypeDef = TypedDict(
-    "_OptionalStartMatchBackfillInputRequestTypeDef",
-    {
-        "TicketId": str,
-        "GameSessionArn": str,
-    },
-    total=False,
-)
-
-class StartMatchBackfillInputRequestTypeDef(
-    _RequiredStartMatchBackfillInputRequestTypeDef, _OptionalStartMatchBackfillInputRequestTypeDef
-):
-    pass
-
-_RequiredStartMatchmakingInputRequestTypeDef = TypedDict(
-    "_RequiredStartMatchmakingInputRequestTypeDef",
-    {
-        "ConfigurationName": str,
-        "Players": Sequence[Union[PlayerTypeDef, PlayerOutputTypeDef]],
-    },
-)
-_OptionalStartMatchmakingInputRequestTypeDef = TypedDict(
-    "_OptionalStartMatchmakingInputRequestTypeDef",
-    {
-        "TicketId": str,
-    },
-    total=False,
-)
-
-class StartMatchmakingInputRequestTypeDef(
-    _RequiredStartMatchmakingInputRequestTypeDef, _OptionalStartMatchmakingInputRequestTypeDef
-):
-    pass
-
+PlayerUnionTypeDef = Union[PlayerTypeDef, PlayerOutputTypeDef]
 CreateScriptOutputTypeDef = TypedDict(
     "CreateScriptOutputTypeDef",
     {
         "Script": ScriptTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -3636,14 +3610,17 @@
 )
 
 class CreateFleetInputRequestTypeDef(
     _RequiredCreateFleetInputRequestTypeDef, _OptionalCreateFleetInputRequestTypeDef
 ):
     pass
 
+RuntimeConfigurationUnionTypeDef = Union[
+    RuntimeConfigurationTypeDef, RuntimeConfigurationOutputTypeDef
+]
 UpdateRuntimeConfigurationInputRequestTypeDef = TypedDict(
     "UpdateRuntimeConfigurationInputRequestTypeDef",
     {
         "FleetId": str,
         "RuntimeConfiguration": RuntimeConfigurationTypeDef,
     },
 )
@@ -3652,14 +3629,55 @@
     "DescribeVpcPeeringConnectionsOutputTypeDef",
     {
         "VpcPeeringConnections": List[VpcPeeringConnectionTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredStartMatchBackfillInputRequestTypeDef = TypedDict(
+    "_RequiredStartMatchBackfillInputRequestTypeDef",
+    {
+        "ConfigurationName": str,
+        "Players": Sequence[PlayerUnionTypeDef],
+    },
+)
+_OptionalStartMatchBackfillInputRequestTypeDef = TypedDict(
+    "_OptionalStartMatchBackfillInputRequestTypeDef",
+    {
+        "TicketId": str,
+        "GameSessionArn": str,
+    },
+    total=False,
+)
+
+class StartMatchBackfillInputRequestTypeDef(
+    _RequiredStartMatchBackfillInputRequestTypeDef, _OptionalStartMatchBackfillInputRequestTypeDef
+):
+    pass
+
+_RequiredStartMatchmakingInputRequestTypeDef = TypedDict(
+    "_RequiredStartMatchmakingInputRequestTypeDef",
+    {
+        "ConfigurationName": str,
+        "Players": Sequence[PlayerUnionTypeDef],
+    },
+)
+_OptionalStartMatchmakingInputRequestTypeDef = TypedDict(
+    "_OptionalStartMatchmakingInputRequestTypeDef",
+    {
+        "TicketId": str,
+    },
+    total=False,
+)
+
+class StartMatchmakingInputRequestTypeDef(
+    _RequiredStartMatchmakingInputRequestTypeDef, _OptionalStartMatchmakingInputRequestTypeDef
+):
+    pass
+
 DescribeGameSessionDetailsOutputTypeDef = TypedDict(
     "DescribeGameSessionDetailsOutputTypeDef",
     {
         "GameSessionDetails": List[GameSessionDetailTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-gamelift-1.28.15.post1/mypy_boto3_gamelift.egg-info/PKG-INFO` & `mypy-boto3-gamelift-1.28.16/mypy_boto3_gamelift.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-gamelift
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.GameLift 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.GameLift 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 gamelift type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 gamelift type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-gamelift.svg?color=blue)](https://pypi.org/project/mypy-boto3-gamelift)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-gamelift)](https://pepy.tech/project/mypy-boto3-gamelift)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.GameLift 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift)
+[boto3.GameLift 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift)
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
 [mypy-boto3-gamelift docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/).
 
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
@@ -447,29 +447,30 @@
 )
 
 
 def check_value(value: AcceptanceTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_gamelift.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_gamelift.type_defs import (
     AcceptMatchInputRequestTypeDef,
     RoutingStrategyTypeDef,
     AnywhereConfigurationTypeDef,
     AttributeValueOutputTypeDef,
     AttributeValueTypeDef,
     AwsCredentialsTypeDef,
+    BlobTypeDef,
     BuildTypeDef,
     CertificateConfigurationTypeDef,
     ClaimFilterOptionTypeDef,
     GameServerTypeDef,
     ResponseMetadataTypeDef,
     ComputeTypeDef,
     TagTypeDef,
@@ -512,15 +513,15 @@
     DescribeBuildInputRequestTypeDef,
     DescribeComputeInputRequestTypeDef,
     DescribeEC2InstanceLimitsInputRequestTypeDef,
     EC2InstanceLimitTypeDef,
     PaginatorConfigTypeDef,
     DescribeFleetAttributesInputRequestTypeDef,
     DescribeFleetCapacityInputRequestTypeDef,
-    DescribeFleetEventsInputRequestTypeDef,
+    TimestampTypeDef,
     EventTypeDef,
     DescribeFleetLocationAttributesInputRequestTypeDef,
     DescribeFleetLocationCapacityInputRequestTypeDef,
     DescribeFleetLocationUtilizationInputRequestTypeDef,
     FleetUtilizationTypeDef,
     DescribeFleetPortSettingsInputRequestTypeDef,
     DescribeFleetUtilizationInputRequestTypeDef,
@@ -649,15 +650,14 @@
     CreatePlayerSessionsOutputTypeDef,
     DescribePlayerSessionsOutputTypeDef,
     CreateVpcPeeringAuthorizationOutputTypeDef,
     DescribeVpcPeeringAuthorizationsOutputTypeDef,
     DescribeEC2InstanceLimitsOutputTypeDef,
     DescribeFleetAttributesInputDescribeFleetAttributesPaginateTypeDef,
     DescribeFleetCapacityInputDescribeFleetCapacityPaginateTypeDef,
-    DescribeFleetEventsInputDescribeFleetEventsPaginateTypeDef,
     DescribeFleetUtilizationInputDescribeFleetUtilizationPaginateTypeDef,
     DescribeGameServerInstancesInputDescribeGameServerInstancesPaginateTypeDef,
     DescribeGameSessionDetailsInputDescribeGameSessionDetailsPaginateTypeDef,
     DescribeGameSessionQueuesInputDescribeGameSessionQueuesPaginateTypeDef,
     DescribeGameSessionsInputDescribeGameSessionsPaginateTypeDef,
     DescribeInstancesInputDescribeInstancesPaginateTypeDef,
     DescribeMatchmakingConfigurationsInputDescribeMatchmakingConfigurationsPaginateTypeDef,
@@ -669,37 +669,40 @@
     ListComputeInputListComputePaginateTypeDef,
     ListFleetsInputListFleetsPaginateTypeDef,
     ListGameServerGroupsInputListGameServerGroupsPaginateTypeDef,
     ListGameServersInputListGameServersPaginateTypeDef,
     ListLocationsInputListLocationsPaginateTypeDef,
     ListScriptsInputListScriptsPaginateTypeDef,
     SearchGameSessionsInputSearchGameSessionsPaginateTypeDef,
+    DescribeFleetEventsInputDescribeFleetEventsPaginateTypeDef,
+    DescribeFleetEventsInputRequestTypeDef,
     DescribeFleetEventsOutputTypeDef,
     DescribeFleetLocationUtilizationOutputTypeDef,
     DescribeFleetUtilizationOutputTypeDef,
     DescribeGameServerInstancesOutputTypeDef,
     DescribeInstancesOutputTypeDef,
     FleetCapacityTypeDef,
+    FilterConfigurationUnionTypeDef,
     GameServerGroupAutoScalingPolicyTypeDef,
     GameSessionConnectionInfoTypeDef,
     GameSessionPlacementTypeDef,
     StartGameSessionPlacementInputRequestTypeDef,
     GameSessionQueueTypeDef,
+    PriorityConfigurationUnionTypeDef,
     InstanceAccessTypeDef,
     PutScalingPolicyInputRequestTypeDef,
     ScalingPolicyTypeDef,
     RuntimeConfigurationOutputTypeDef,
     RuntimeConfigurationTypeDef,
     VpcPeeringConnectionTypeDef,
     CreateAliasOutputTypeDef,
     DescribeAliasOutputTypeDef,
     ListAliasesOutputTypeDef,
     UpdateAliasOutputTypeDef,
-    StartMatchBackfillInputRequestTypeDef,
-    StartMatchmakingInputRequestTypeDef,
+    PlayerUnionTypeDef,
     CreateScriptOutputTypeDef,
     DescribeScriptOutputTypeDef,
     ListScriptsOutputTypeDef,
     UpdateScriptOutputTypeDef,
     CreateFleetOutputTypeDef,
     DescribeFleetAttributesOutputTypeDef,
     DescribeFleetLocationAttributesOutputTypeDef,
@@ -729,24 +732,27 @@
     DescribeGameSessionQueuesOutputTypeDef,
     UpdateGameSessionQueueOutputTypeDef,
     GetInstanceAccessOutputTypeDef,
     DescribeScalingPoliciesOutputTypeDef,
     DescribeRuntimeConfigurationOutputTypeDef,
     UpdateRuntimeConfigurationOutputTypeDef,
     CreateFleetInputRequestTypeDef,
+    RuntimeConfigurationUnionTypeDef,
     UpdateRuntimeConfigurationInputRequestTypeDef,
     DescribeVpcPeeringConnectionsOutputTypeDef,
+    StartMatchBackfillInputRequestTypeDef,
+    StartMatchmakingInputRequestTypeDef,
     DescribeGameSessionDetailsOutputTypeDef,
     DescribeMatchmakingOutputTypeDef,
     StartMatchBackfillOutputTypeDef,
     StartMatchmakingOutputTypeDef,
 )
 
 
-def get_structure() -> AcceptMatchInputRequestTypeDef:
+def get_value() -> AcceptMatchInputRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-gamelift-1.28.15.post1/mypy_boto3_gamelift.egg-info/SOURCES.txt` & `mypy-boto3-gamelift-1.28.16/mypy_boto3_gamelift.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-gamelift-1.28.15.post1/setup.py` & `mypy-boto3-gamelift-1.28.16/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-gamelift",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_gamelift"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.GameLift 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.2"
+        "Type annotations for boto3.GameLift 1.28.16 service generated with mypy-boto3-builder"
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
-    keywords="boto3 gamelift type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 gamelift type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_gamelift": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

