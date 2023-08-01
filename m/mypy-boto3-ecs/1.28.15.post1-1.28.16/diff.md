# Comparing `tmp/mypy-boto3-ecs-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-ecs-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-ecs-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:02 2023, max compression
+gzip compressed data, was "mypy-boto3-ecs-1.28.16.tar", last modified: Tue Aug  1 11:36:42 2023, max compression
```

## Comparing `mypy-boto3-ecs-1.28.15.post1.tar` & `mypy-boto3-ecs-1.28.16.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:02.501128 mypy-boto3-ecs-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:44:21.000000 mypy-boto3-ecs-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    25110 2023-07-29 10:03:02.501128 mypy-boto3-ecs-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    23633 2023-07-29 09:44:21.000000 mypy-boto3-ecs-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:02.485128 mypy-boto3-ecs-1.28.15.post1/mypy_boto3_ecs/
--rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-07-29 09:44:21.000000 mypy-boto3-ecs-1.28.15.post1/mypy_boto3_ecs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-07-29 09:44:21.000000 mypy-boto3-ecs-1.28.15.post1/mypy_boto3_ecs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-29 09:44:21.000000 mypy-boto3-ecs-1.28.15.post1/mypy_boto3_ecs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    51100 2023-07-29 09:44:21.000000 mypy-boto3-ecs-1.28.15.post1/mypy_boto3_ecs/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    51024 2023-07-29 09:44:21.000000 mypy-boto3-ecs-1.28.15.post1/mypy_boto3_ecs/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15762 2023-07-29 09:44:22.000000 mypy-boto3-ecs-1.28.15.post1/mypy_boto3_ecs/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    15760 2023-07-29 09:44:22.000000 mypy-boto3-ecs-1.28.15.post1/mypy_boto3_ecs/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11519 2023-07-29 09:44:21.000000 mypy-boto3-ecs-1.28.15.post1/mypy_boto3_ecs/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11507 2023-07-29 09:44:21.000000 mypy-boto3-ecs-1.28.15.post1/mypy_boto3_ecs/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:44:21.000000 mypy-boto3-ecs-1.28.15.post1/mypy_boto3_ecs/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    95722 2023-07-29 09:44:26.000000 mypy-boto3-ecs-1.28.15.post1/mypy_boto3_ecs/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    95603 2023-07-29 09:44:23.000000 mypy-boto3-ecs-1.28.15.post1/mypy_boto3_ecs/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:44:21.000000 mypy-boto3-ecs-1.28.15.post1/mypy_boto3_ecs/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-07-29 09:44:21.000000 mypy-boto3-ecs-1.28.15.post1/mypy_boto3_ecs/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-07-29 09:44:21.000000 mypy-boto3-ecs-1.28.15.post1/mypy_boto3_ecs/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:02.501128 mypy-boto3-ecs-1.28.15.post1/mypy_boto3_ecs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    25110 2023-07-29 10:03:02.000000 mypy-boto3-ecs-1.28.15.post1/mypy_boto3_ecs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-29 10:03:02.000000 mypy-boto3-ecs-1.28.15.post1/mypy_boto3_ecs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:02.000000 mypy-boto3-ecs-1.28.15.post1/mypy_boto3_ecs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:02.000000 mypy-boto3-ecs-1.28.15.post1/mypy_boto3_ecs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:02.000000 mypy-boto3-ecs-1.28.15.post1/mypy_boto3_ecs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-29 10:03:02.000000 mypy-boto3-ecs-1.28.15.post1/mypy_boto3_ecs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:02.501128 mypy-boto3-ecs-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-29 09:44:20.000000 mypy-boto3-ecs-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:42.440901 mypy-boto3-ecs-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:16:55.000000 mypy-boto3-ecs-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    25399 2023-08-01 11:36:42.432901 mypy-boto3-ecs-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    23931 2023-08-01 11:16:55.000000 mypy-boto3-ecs-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:42.428901 mypy-boto3-ecs-1.28.16/mypy_boto3_ecs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-08-01 11:16:55.000000 mypy-boto3-ecs-1.28.16/mypy_boto3_ecs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-08-01 11:16:55.000000 mypy-boto3-ecs-1.28.16/mypy_boto3_ecs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-08-01 11:16:55.000000 mypy-boto3-ecs-1.28.16/mypy_boto3_ecs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50078 2023-08-01 11:16:56.000000 mypy-boto3-ecs-1.28.16/mypy_boto3_ecs/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50002 2023-08-01 11:16:55.000000 mypy-boto3-ecs-1.28.16/mypy_boto3_ecs/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15762 2023-08-01 11:16:58.000000 mypy-boto3-ecs-1.28.16/mypy_boto3_ecs/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15760 2023-08-01 11:16:56.000000 mypy-boto3-ecs-1.28.16/mypy_boto3_ecs/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11519 2023-08-01 11:16:56.000000 mypy-boto3-ecs-1.28.16/mypy_boto3_ecs/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11507 2023-08-01 11:16:56.000000 mypy-boto3-ecs-1.28.16/mypy_boto3_ecs/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:16:55.000000 mypy-boto3-ecs-1.28.16/mypy_boto3_ecs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    96742 2023-08-01 11:17:00.000000 mypy-boto3-ecs-1.28.16/mypy_boto3_ecs/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    96623 2023-08-01 11:16:59.000000 mypy-boto3-ecs-1.28.16/mypy_boto3_ecs/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:16:55.000000 mypy-boto3-ecs-1.28.16/mypy_boto3_ecs/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-08-01 11:16:56.000000 mypy-boto3-ecs-1.28.16/mypy_boto3_ecs/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-08-01 11:16:56.000000 mypy-boto3-ecs-1.28.16/mypy_boto3_ecs/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:42.432901 mypy-boto3-ecs-1.28.16/mypy_boto3_ecs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    25399 2023-08-01 11:36:42.000000 mypy-boto3-ecs-1.28.16/mypy_boto3_ecs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-08-01 11:36:42.000000 mypy-boto3-ecs-1.28.16/mypy_boto3_ecs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:42.000000 mypy-boto3-ecs-1.28.16/mypy_boto3_ecs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:42.000000 mypy-boto3-ecs-1.28.16/mypy_boto3_ecs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:42.000000 mypy-boto3-ecs-1.28.16/mypy_boto3_ecs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-01 11:36:42.000000 mypy-boto3-ecs-1.28.16/mypy_boto3_ecs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:42.440901 mypy-boto3-ecs-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-08-01 11:16:55.000000 mypy-boto3-ecs-1.28.16/setup.py
```

### Comparing `mypy-boto3-ecs-1.28.15.post1/LICENSE` & `mypy-boto3-ecs-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecs-1.28.15.post1/PKG-INFO` & `mypy-boto3-ecs-1.28.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ecs
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.ECS 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.ECS 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 ecs type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 ecs type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ecs.svg?color=blue)](https://pypi.org/project/mypy-boto3-ecs)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ecs)](https://pepy.tech/project/mypy-boto3-ecs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ECS 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS)
+[boto3.ECS 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS)
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
 [mypy-boto3-ecs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/).
 
 See how it helps to find and fix potential bugs:
 
@@ -75,15 +75,15 @@
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Waiters annotations](#waiters-annotations)
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
@@ -435,20 +435,20 @@
 )
 
 
 def check_value(value: AgentUpdateStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_ecs.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_ecs.type_defs import (
     AttachmentStateChangeTypeDef,
     KeyValuePairTypeDef,
     AttributeTypeDef,
     ManagedScalingTypeDef,
@@ -540,20 +540,21 @@
     ListTaskDefinitionFamiliesRequestRequestTypeDef,
     ListTaskDefinitionsRequestRequestTypeDef,
     ListTasksRequestRequestTypeDef,
     ManagedAgentStateChangeTypeDef,
     PlatformDeviceTypeDef,
     PutAccountSettingDefaultRequestRequestTypeDef,
     PutAccountSettingRequestRequestTypeDef,
-    ResourceTypeDef,
     RuntimePlatformTypeDef,
     TaskDefinitionPlacementConstraintTypeDef,
+    ResourceTypeDef,
     ServiceConnectClientAliasTypeDef,
     ServiceEventTypeDef,
     StopTaskRequestRequestTypeDef,
+    TimestampTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateContainerAgentRequestRequestTypeDef,
     UpdateContainerInstancesStateRequestRequestTypeDef,
     UpdateServicePrimaryTaskSetRequestRequestTypeDef,
     UpdateTaskProtectionRequestRequestTypeDef,
     SubmitAttachmentStateChangesRequestRequestTypeDef,
     AttachmentTypeDef,
@@ -615,57 +616,64 @@
     ListClustersRequestListClustersPaginateTypeDef,
     ListContainerInstancesRequestListContainerInstancesPaginateTypeDef,
     ListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef,
     ListServicesRequestListServicesPaginateTypeDef,
     ListTaskDefinitionFamiliesRequestListTaskDefinitionFamiliesPaginateTypeDef,
     ListTaskDefinitionsRequestListTaskDefinitionsPaginateTypeDef,
     ListTasksRequestListTasksPaginateTypeDef,
-    RegisterContainerInstanceRequestRequestTypeDef,
+    ResourceUnionTypeDef,
     ServiceConnectServiceOutputTypeDef,
     ServiceConnectServiceTypeDef,
+    ProxyConfigurationUnionTypeDef,
     CapacityProviderTypeDef,
     CreateCapacityProviderRequestRequestTypeDef,
     UpdateCapacityProviderRequestRequestTypeDef,
     TaskSetTypeDef,
     CreateTaskSetRequestRequestTypeDef,
+    NetworkConfigurationUnionTypeDef,
     TaskOverrideOutputTypeDef,
     TaskOverrideTypeDef,
     ContainerInstanceTypeDef,
     SubmitTaskStateChangeRequestRequestTypeDef,
+    DeploymentConfigurationUnionTypeDef,
     ClusterConfigurationTypeDef,
     VolumeOutputTypeDef,
     VolumeTypeDef,
     ContainerDefinitionOutputTypeDef,
     ContainerDefinitionTypeDef,
+    RegisterContainerInstanceRequestRequestTypeDef,
     ServiceConnectConfigurationOutputTypeDef,
     ServiceConnectConfigurationTypeDef,
     CreateCapacityProviderResponseTypeDef,
     DeleteCapacityProviderResponseTypeDef,
     DescribeCapacityProvidersResponseTypeDef,
     UpdateCapacityProviderResponseTypeDef,
     CreateTaskSetResponseTypeDef,
     DeleteTaskSetResponseTypeDef,
     DescribeTaskSetsResponseTypeDef,
     UpdateServicePrimaryTaskSetResponseTypeDef,
     UpdateTaskSetResponseTypeDef,
     TaskTypeDef,
     RunTaskRequestRequestTypeDef,
     StartTaskRequestRequestTypeDef,
+    TaskOverrideUnionTypeDef,
     DeregisterContainerInstanceResponseTypeDef,
     DescribeContainerInstancesResponseTypeDef,
     RegisterContainerInstanceResponseTypeDef,
     UpdateContainerAgentResponseTypeDef,
     UpdateContainerInstancesStateResponseTypeDef,
     ClusterTypeDef,
     CreateClusterRequestRequestTypeDef,
     UpdateClusterRequestRequestTypeDef,
+    VolumeUnionTypeDef,
     TaskDefinitionTypeDef,
-    RegisterTaskDefinitionRequestRequestTypeDef,
+    ContainerDefinitionUnionTypeDef,
     DeploymentTypeDef,
     CreateServiceRequestRequestTypeDef,
+    ServiceConnectConfigurationUnionTypeDef,
     UpdateServiceRequestRequestTypeDef,
     DescribeTasksResponseTypeDef,
     RunTaskResponseTypeDef,
     StartTaskResponseTypeDef,
     StopTaskResponseTypeDef,
     CreateClusterResponseTypeDef,
     DeleteClusterResponseTypeDef,
@@ -673,23 +681,24 @@
     PutClusterCapacityProvidersResponseTypeDef,
     UpdateClusterResponseTypeDef,
     UpdateClusterSettingsResponseTypeDef,
     DeleteTaskDefinitionsResponseTypeDef,
     DeregisterTaskDefinitionResponseTypeDef,
     DescribeTaskDefinitionResponseTypeDef,
     RegisterTaskDefinitionResponseTypeDef,
+    RegisterTaskDefinitionRequestRequestTypeDef,
     ServiceTypeDef,
     CreateServiceResponseTypeDef,
     DeleteServiceResponseTypeDef,
     DescribeServicesResponseTypeDef,
     UpdateServiceResponseTypeDef,
 )
 
 
-def get_structure() -> AttachmentStateChangeTypeDef:
+def get_value() -> AttachmentStateChangeTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-ecs-1.28.15.post1/README.md` & `mypy-boto3-ecs-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ecs.svg?color=blue)](https://pypi.org/project/mypy-boto3-ecs)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ecs)](https://pepy.tech/project/mypy-boto3-ecs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ECS 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS)
+[boto3.ECS 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS)
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
 [mypy-boto3-ecs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/).
 
 See how it helps to find and fix potential bugs:
 
@@ -43,15 +43,15 @@
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Waiters annotations](#waiters-annotations)
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
@@ -403,20 +403,20 @@
 )
 
 
 def check_value(value: AgentUpdateStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_ecs.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_ecs.type_defs import (
     AttachmentStateChangeTypeDef,
     KeyValuePairTypeDef,
     AttributeTypeDef,
     ManagedScalingTypeDef,
@@ -508,20 +508,21 @@
     ListTaskDefinitionFamiliesRequestRequestTypeDef,
     ListTaskDefinitionsRequestRequestTypeDef,
     ListTasksRequestRequestTypeDef,
     ManagedAgentStateChangeTypeDef,
     PlatformDeviceTypeDef,
     PutAccountSettingDefaultRequestRequestTypeDef,
     PutAccountSettingRequestRequestTypeDef,
-    ResourceTypeDef,
     RuntimePlatformTypeDef,
     TaskDefinitionPlacementConstraintTypeDef,
+    ResourceTypeDef,
     ServiceConnectClientAliasTypeDef,
     ServiceEventTypeDef,
     StopTaskRequestRequestTypeDef,
+    TimestampTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateContainerAgentRequestRequestTypeDef,
     UpdateContainerInstancesStateRequestRequestTypeDef,
     UpdateServicePrimaryTaskSetRequestRequestTypeDef,
     UpdateTaskProtectionRequestRequestTypeDef,
     SubmitAttachmentStateChangesRequestRequestTypeDef,
     AttachmentTypeDef,
@@ -583,57 +584,64 @@
     ListClustersRequestListClustersPaginateTypeDef,
     ListContainerInstancesRequestListContainerInstancesPaginateTypeDef,
     ListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef,
     ListServicesRequestListServicesPaginateTypeDef,
     ListTaskDefinitionFamiliesRequestListTaskDefinitionFamiliesPaginateTypeDef,
     ListTaskDefinitionsRequestListTaskDefinitionsPaginateTypeDef,
     ListTasksRequestListTasksPaginateTypeDef,
-    RegisterContainerInstanceRequestRequestTypeDef,
+    ResourceUnionTypeDef,
     ServiceConnectServiceOutputTypeDef,
     ServiceConnectServiceTypeDef,
+    ProxyConfigurationUnionTypeDef,
     CapacityProviderTypeDef,
     CreateCapacityProviderRequestRequestTypeDef,
     UpdateCapacityProviderRequestRequestTypeDef,
     TaskSetTypeDef,
     CreateTaskSetRequestRequestTypeDef,
+    NetworkConfigurationUnionTypeDef,
     TaskOverrideOutputTypeDef,
     TaskOverrideTypeDef,
     ContainerInstanceTypeDef,
     SubmitTaskStateChangeRequestRequestTypeDef,
+    DeploymentConfigurationUnionTypeDef,
     ClusterConfigurationTypeDef,
     VolumeOutputTypeDef,
     VolumeTypeDef,
     ContainerDefinitionOutputTypeDef,
     ContainerDefinitionTypeDef,
+    RegisterContainerInstanceRequestRequestTypeDef,
     ServiceConnectConfigurationOutputTypeDef,
     ServiceConnectConfigurationTypeDef,
     CreateCapacityProviderResponseTypeDef,
     DeleteCapacityProviderResponseTypeDef,
     DescribeCapacityProvidersResponseTypeDef,
     UpdateCapacityProviderResponseTypeDef,
     CreateTaskSetResponseTypeDef,
     DeleteTaskSetResponseTypeDef,
     DescribeTaskSetsResponseTypeDef,
     UpdateServicePrimaryTaskSetResponseTypeDef,
     UpdateTaskSetResponseTypeDef,
     TaskTypeDef,
     RunTaskRequestRequestTypeDef,
     StartTaskRequestRequestTypeDef,
+    TaskOverrideUnionTypeDef,
     DeregisterContainerInstanceResponseTypeDef,
     DescribeContainerInstancesResponseTypeDef,
     RegisterContainerInstanceResponseTypeDef,
     UpdateContainerAgentResponseTypeDef,
     UpdateContainerInstancesStateResponseTypeDef,
     ClusterTypeDef,
     CreateClusterRequestRequestTypeDef,
     UpdateClusterRequestRequestTypeDef,
+    VolumeUnionTypeDef,
     TaskDefinitionTypeDef,
-    RegisterTaskDefinitionRequestRequestTypeDef,
+    ContainerDefinitionUnionTypeDef,
     DeploymentTypeDef,
     CreateServiceRequestRequestTypeDef,
+    ServiceConnectConfigurationUnionTypeDef,
     UpdateServiceRequestRequestTypeDef,
     DescribeTasksResponseTypeDef,
     RunTaskResponseTypeDef,
     StartTaskResponseTypeDef,
     StopTaskResponseTypeDef,
     CreateClusterResponseTypeDef,
     DeleteClusterResponseTypeDef,
@@ -641,23 +649,24 @@
     PutClusterCapacityProvidersResponseTypeDef,
     UpdateClusterResponseTypeDef,
     UpdateClusterSettingsResponseTypeDef,
     DeleteTaskDefinitionsResponseTypeDef,
     DeregisterTaskDefinitionResponseTypeDef,
     DescribeTaskDefinitionResponseTypeDef,
     RegisterTaskDefinitionResponseTypeDef,
+    RegisterTaskDefinitionRequestRequestTypeDef,
     ServiceTypeDef,
     CreateServiceResponseTypeDef,
     DeleteServiceResponseTypeDef,
     DescribeServicesResponseTypeDef,
     UpdateServiceResponseTypeDef,
 )
 
 
-def get_structure() -> AttachmentStateChangeTypeDef:
+def get_value() -> AttachmentStateChangeTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-ecs-1.28.15.post1/mypy_boto3_ecs/__init__.py` & `mypy-boto3-ecs-1.28.16/mypy_boto3_ecs/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecs-1.28.15.post1/mypy_boto3_ecs/__init__.pyi` & `mypy-boto3-ecs-1.28.16/mypy_boto3_ecs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecs-1.28.15.post1/mypy_boto3_ecs/__main__.py` & `mypy-boto3-ecs-1.28.16/mypy_boto3_ecs/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ECS 1.28.15\nVersion:         1.28.15.post1\nBuilder version:"
-        " 7.16.2\nDocs:           "
+        "Type annotations for boto3.ECS 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS\nOther"
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

### Comparing `mypy-boto3-ecs-1.28.15.post1/mypy_boto3_ecs/client.py` & `mypy-boto3-ecs-1.28.16/mypy_boto3_ecs/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from mypy_boto3_ecs.client import ECSClient
 
     session = Session()
     client: ECSClient = session.client("ecs")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     ClusterFieldType,
     CompatibilityType,
     ContainerInstanceFieldType,
@@ -52,30 +51,28 @@
     AttributeTypeDef,
     AutoScalingGroupProviderTypeDef,
     AutoScalingGroupProviderUpdateTypeDef,
     CapacityProviderStrategyItemTypeDef,
     ClusterConfigurationTypeDef,
     ClusterServiceConnectDefaultsRequestTypeDef,
     ClusterSettingTypeDef,
-    ContainerDefinitionOutputTypeDef,
-    ContainerDefinitionTypeDef,
+    ContainerDefinitionUnionTypeDef,
     ContainerStateChangeTypeDef,
     CreateCapacityProviderResponseTypeDef,
     CreateClusterResponseTypeDef,
     CreateServiceResponseTypeDef,
     CreateTaskSetResponseTypeDef,
     DeleteAccountSettingResponseTypeDef,
     DeleteAttributesResponseTypeDef,
     DeleteCapacityProviderResponseTypeDef,
     DeleteClusterResponseTypeDef,
     DeleteServiceResponseTypeDef,
     DeleteTaskDefinitionsResponseTypeDef,
     DeleteTaskSetResponseTypeDef,
-    DeploymentConfigurationOutputTypeDef,
-    DeploymentConfigurationTypeDef,
+    DeploymentConfigurationUnionTypeDef,
     DeploymentControllerTypeDef,
     DeregisterContainerInstanceResponseTypeDef,
     DeregisterTaskDefinitionResponseTypeDef,
     DescribeCapacityProvidersResponseTypeDef,
     DescribeClustersResponseTypeDef,
     DescribeContainerInstancesResponseTypeDef,
     DescribeServicesResponseTypeDef,
@@ -96,56 +93,51 @@
     ListTagsForResourceResponseTypeDef,
     ListTaskDefinitionFamiliesResponseTypeDef,
     ListTaskDefinitionsResponseTypeDef,
     ListTasksResponseTypeDef,
     LoadBalancerTypeDef,
     ManagedAgentStateChangeTypeDef,
     NetworkBindingTypeDef,
-    NetworkConfigurationOutputTypeDef,
-    NetworkConfigurationTypeDef,
+    NetworkConfigurationUnionTypeDef,
     PlacementConstraintTypeDef,
     PlacementStrategyTypeDef,
     PlatformDeviceTypeDef,
-    ProxyConfigurationOutputTypeDef,
-    ProxyConfigurationTypeDef,
+    ProxyConfigurationUnionTypeDef,
     PutAccountSettingDefaultResponseTypeDef,
     PutAccountSettingResponseTypeDef,
     PutAttributesResponseTypeDef,
     PutClusterCapacityProvidersResponseTypeDef,
     RegisterContainerInstanceResponseTypeDef,
     RegisterTaskDefinitionResponseTypeDef,
-    ResourceOutputTypeDef,
-    ResourceTypeDef,
+    ResourceUnionTypeDef,
     RunTaskResponseTypeDef,
     RuntimePlatformTypeDef,
     ScaleTypeDef,
-    ServiceConnectConfigurationOutputTypeDef,
-    ServiceConnectConfigurationTypeDef,
+    ServiceConnectConfigurationUnionTypeDef,
     ServiceRegistryTypeDef,
     StartTaskResponseTypeDef,
     StopTaskResponseTypeDef,
     SubmitAttachmentStateChangesResponseTypeDef,
     SubmitContainerStateChangeResponseTypeDef,
     SubmitTaskStateChangeResponseTypeDef,
     TagTypeDef,
     TaskDefinitionPlacementConstraintTypeDef,
-    TaskOverrideOutputTypeDef,
-    TaskOverrideTypeDef,
+    TaskOverrideUnionTypeDef,
+    TimestampTypeDef,
     UpdateCapacityProviderResponseTypeDef,
     UpdateClusterResponseTypeDef,
     UpdateClusterSettingsResponseTypeDef,
     UpdateContainerAgentResponseTypeDef,
     UpdateContainerInstancesStateResponseTypeDef,
     UpdateServicePrimaryTaskSetResponseTypeDef,
     UpdateServiceResponseTypeDef,
     UpdateTaskProtectionResponseTypeDef,
     UpdateTaskSetResponseTypeDef,
     VersionInfoTypeDef,
-    VolumeOutputTypeDef,
-    VolumeTypeDef,
+    VolumeUnionTypeDef,
 )
 from .waiter import (
     ServicesInactiveWaiter,
     ServicesStableWaiter,
     TasksRunningWaiter,
     TasksStoppedWaiter,
 )
@@ -271,32 +263,26 @@
         serviceRegistries: Sequence[ServiceRegistryTypeDef] = ...,
         desiredCount: int = ...,
         clientToken: str = ...,
         launchType: LaunchTypeType = ...,
         capacityProviderStrategy: Sequence[CapacityProviderStrategyItemTypeDef] = ...,
         platformVersion: str = ...,
         role: str = ...,
-        deploymentConfiguration: Union[
-            DeploymentConfigurationTypeDef, DeploymentConfigurationOutputTypeDef
-        ] = ...,
+        deploymentConfiguration: DeploymentConfigurationUnionTypeDef = ...,
         placementConstraints: Sequence[PlacementConstraintTypeDef] = ...,
         placementStrategy: Sequence[PlacementStrategyTypeDef] = ...,
-        networkConfiguration: Union[
-            NetworkConfigurationTypeDef, NetworkConfigurationOutputTypeDef
-        ] = ...,
+        networkConfiguration: NetworkConfigurationUnionTypeDef = ...,
         healthCheckGracePeriodSeconds: int = ...,
         schedulingStrategy: SchedulingStrategyType = ...,
         deploymentController: DeploymentControllerTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...,
         enableECSManagedTags: bool = ...,
         propagateTags: PropagateTagsType = ...,
         enableExecuteCommand: bool = ...,
-        serviceConnectConfiguration: Union[
-            ServiceConnectConfigurationTypeDef, ServiceConnectConfigurationOutputTypeDef
-        ] = ...
+        serviceConnectConfiguration: ServiceConnectConfigurationUnionTypeDef = ...
     ) -> CreateServiceResponseTypeDef:
         """
         Runs and maintains your desired number of tasks from a specified task
         definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.create_service)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#create_service)
@@ -305,17 +291,15 @@
     def create_task_set(
         self,
         *,
         service: str,
         cluster: str,
         taskDefinition: str,
         externalId: str = ...,
-        networkConfiguration: Union[
-            NetworkConfigurationTypeDef, NetworkConfigurationOutputTypeDef
-        ] = ...,
+        networkConfiguration: NetworkConfigurationUnionTypeDef = ...,
         loadBalancers: Sequence[LoadBalancerTypeDef] = ...,
         serviceRegistries: Sequence[ServiceRegistryTypeDef] = ...,
         launchType: LaunchTypeType = ...,
         capacityProviderStrategy: Sequence[CapacityProviderStrategyItemTypeDef] = ...,
         platformVersion: str = ...,
         scale: ScaleTypeDef = ...,
         clientToken: str = ...,
@@ -750,15 +734,15 @@
 
     def register_container_instance(
         self,
         *,
         cluster: str = ...,
         instanceIdentityDocument: str = ...,
         instanceIdentityDocumentSignature: str = ...,
-        totalResources: Sequence[Union[ResourceTypeDef, ResourceOutputTypeDef]] = ...,
+        totalResources: Sequence[ResourceUnionTypeDef] = ...,
         versionInfo: VersionInfoTypeDef = ...,
         containerInstanceArn: str = ...,
         attributes: Sequence[AttributeTypeDef] = ...,
         platformDevices: Sequence[PlatformDeviceTypeDef] = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> RegisterContainerInstanceResponseTypeDef:
         """
@@ -768,29 +752,27 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#register_container_instance)
         """
 
     def register_task_definition(
         self,
         *,
         family: str,
-        containerDefinitions: Sequence[
-            Union[ContainerDefinitionTypeDef, ContainerDefinitionOutputTypeDef]
-        ],
+        containerDefinitions: Sequence[ContainerDefinitionUnionTypeDef],
         taskRoleArn: str = ...,
         executionRoleArn: str = ...,
         networkMode: NetworkModeType = ...,
-        volumes: Sequence[Union[VolumeTypeDef, VolumeOutputTypeDef]] = ...,
+        volumes: Sequence[VolumeUnionTypeDef] = ...,
         placementConstraints: Sequence[TaskDefinitionPlacementConstraintTypeDef] = ...,
         requiresCompatibilities: Sequence[CompatibilityType] = ...,
         cpu: str = ...,
         memory: str = ...,
         tags: Sequence[TagTypeDef] = ...,
         pidMode: PidModeType = ...,
         ipcMode: IpcModeType = ...,
-        proxyConfiguration: Union[ProxyConfigurationTypeDef, ProxyConfigurationOutputTypeDef] = ...,
+        proxyConfiguration: ProxyConfigurationUnionTypeDef = ...,
         inferenceAccelerators: Sequence[InferenceAcceleratorTypeDef] = ...,
         ephemeralStorage: EphemeralStorageTypeDef = ...,
         runtimePlatform: RuntimePlatformTypeDef = ...
     ) -> RegisterTaskDefinitionResponseTypeDef:
         """
         Registers a new task definition from the supplied `family` and
         `containerDefinitions`.
@@ -806,18 +788,16 @@
         capacityProviderStrategy: Sequence[CapacityProviderStrategyItemTypeDef] = ...,
         cluster: str = ...,
         count: int = ...,
         enableECSManagedTags: bool = ...,
         enableExecuteCommand: bool = ...,
         group: str = ...,
         launchType: LaunchTypeType = ...,
-        networkConfiguration: Union[
-            NetworkConfigurationTypeDef, NetworkConfigurationOutputTypeDef
-        ] = ...,
-        overrides: Union[TaskOverrideTypeDef, TaskOverrideOutputTypeDef] = ...,
+        networkConfiguration: NetworkConfigurationUnionTypeDef = ...,
+        overrides: TaskOverrideUnionTypeDef = ...,
         placementConstraints: Sequence[PlacementConstraintTypeDef] = ...,
         placementStrategy: Sequence[PlacementStrategyTypeDef] = ...,
         platformVersion: str = ...,
         propagateTags: PropagateTagsType = ...,
         referenceId: str = ...,
         startedBy: str = ...,
         tags: Sequence[TagTypeDef] = ...
@@ -834,18 +814,16 @@
         *,
         containerInstances: Sequence[str],
         taskDefinition: str,
         cluster: str = ...,
         enableECSManagedTags: bool = ...,
         enableExecuteCommand: bool = ...,
         group: str = ...,
-        networkConfiguration: Union[
-            NetworkConfigurationTypeDef, NetworkConfigurationOutputTypeDef
-        ] = ...,
-        overrides: Union[TaskOverrideTypeDef, TaskOverrideOutputTypeDef] = ...,
+        networkConfiguration: NetworkConfigurationUnionTypeDef = ...,
+        overrides: TaskOverrideUnionTypeDef = ...,
         propagateTags: PropagateTagsType = ...,
         referenceId: str = ...,
         startedBy: str = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> StartTaskResponseTypeDef:
         """
         Starts a new task from the specified task definition on the specified container
@@ -900,17 +878,17 @@
         cluster: str = ...,
         task: str = ...,
         status: str = ...,
         reason: str = ...,
         containers: Sequence[ContainerStateChangeTypeDef] = ...,
         attachments: Sequence[AttachmentStateChangeTypeDef] = ...,
         managedAgents: Sequence[ManagedAgentStateChangeTypeDef] = ...,
-        pullStartedAt: Union[datetime, str] = ...,
-        pullStoppedAt: Union[datetime, str] = ...,
-        executionStoppedAt: Union[datetime, str] = ...
+        pullStartedAt: TimestampTypeDef = ...,
+        pullStoppedAt: TimestampTypeDef = ...,
+        executionStoppedAt: TimestampTypeDef = ...
     ) -> SubmitTaskStateChangeResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.submit_task_state_change)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#submit_task_state_change)
         """
@@ -994,33 +972,27 @@
         self,
         *,
         service: str,
         cluster: str = ...,
         desiredCount: int = ...,
         taskDefinition: str = ...,
         capacityProviderStrategy: Sequence[CapacityProviderStrategyItemTypeDef] = ...,
-        deploymentConfiguration: Union[
-            DeploymentConfigurationTypeDef, DeploymentConfigurationOutputTypeDef
-        ] = ...,
-        networkConfiguration: Union[
-            NetworkConfigurationTypeDef, NetworkConfigurationOutputTypeDef
-        ] = ...,
+        deploymentConfiguration: DeploymentConfigurationUnionTypeDef = ...,
+        networkConfiguration: NetworkConfigurationUnionTypeDef = ...,
         placementConstraints: Sequence[PlacementConstraintTypeDef] = ...,
         placementStrategy: Sequence[PlacementStrategyTypeDef] = ...,
         platformVersion: str = ...,
         forceNewDeployment: bool = ...,
         healthCheckGracePeriodSeconds: int = ...,
         enableExecuteCommand: bool = ...,
         enableECSManagedTags: bool = ...,
         loadBalancers: Sequence[LoadBalancerTypeDef] = ...,
         propagateTags: PropagateTagsType = ...,
         serviceRegistries: Sequence[ServiceRegistryTypeDef] = ...,
-        serviceConnectConfiguration: Union[
-            ServiceConnectConfigurationTypeDef, ServiceConnectConfigurationOutputTypeDef
-        ] = ...
+        serviceConnectConfiguration: ServiceConnectConfigurationUnionTypeDef = ...
     ) -> UpdateServiceResponseTypeDef:
         """
         Modifies the parameters of a service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.update_service)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#update_service)
         """
```

### Comparing `mypy-boto3-ecs-1.28.15.post1/mypy_boto3_ecs/client.pyi` & `mypy-boto3-ecs-1.28.16/mypy_boto3_ecs/client.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from mypy_boto3_ecs.client import ECSClient
 
     session = Session()
     client: ECSClient = session.client("ecs")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     ClusterFieldType,
     CompatibilityType,
     ContainerInstanceFieldType,
@@ -52,30 +51,28 @@
     AttributeTypeDef,
     AutoScalingGroupProviderTypeDef,
     AutoScalingGroupProviderUpdateTypeDef,
     CapacityProviderStrategyItemTypeDef,
     ClusterConfigurationTypeDef,
     ClusterServiceConnectDefaultsRequestTypeDef,
     ClusterSettingTypeDef,
-    ContainerDefinitionOutputTypeDef,
-    ContainerDefinitionTypeDef,
+    ContainerDefinitionUnionTypeDef,
     ContainerStateChangeTypeDef,
     CreateCapacityProviderResponseTypeDef,
     CreateClusterResponseTypeDef,
     CreateServiceResponseTypeDef,
     CreateTaskSetResponseTypeDef,
     DeleteAccountSettingResponseTypeDef,
     DeleteAttributesResponseTypeDef,
     DeleteCapacityProviderResponseTypeDef,
     DeleteClusterResponseTypeDef,
     DeleteServiceResponseTypeDef,
     DeleteTaskDefinitionsResponseTypeDef,
     DeleteTaskSetResponseTypeDef,
-    DeploymentConfigurationOutputTypeDef,
-    DeploymentConfigurationTypeDef,
+    DeploymentConfigurationUnionTypeDef,
     DeploymentControllerTypeDef,
     DeregisterContainerInstanceResponseTypeDef,
     DeregisterTaskDefinitionResponseTypeDef,
     DescribeCapacityProvidersResponseTypeDef,
     DescribeClustersResponseTypeDef,
     DescribeContainerInstancesResponseTypeDef,
     DescribeServicesResponseTypeDef,
@@ -96,56 +93,51 @@
     ListTagsForResourceResponseTypeDef,
     ListTaskDefinitionFamiliesResponseTypeDef,
     ListTaskDefinitionsResponseTypeDef,
     ListTasksResponseTypeDef,
     LoadBalancerTypeDef,
     ManagedAgentStateChangeTypeDef,
     NetworkBindingTypeDef,
-    NetworkConfigurationOutputTypeDef,
-    NetworkConfigurationTypeDef,
+    NetworkConfigurationUnionTypeDef,
     PlacementConstraintTypeDef,
     PlacementStrategyTypeDef,
     PlatformDeviceTypeDef,
-    ProxyConfigurationOutputTypeDef,
-    ProxyConfigurationTypeDef,
+    ProxyConfigurationUnionTypeDef,
     PutAccountSettingDefaultResponseTypeDef,
     PutAccountSettingResponseTypeDef,
     PutAttributesResponseTypeDef,
     PutClusterCapacityProvidersResponseTypeDef,
     RegisterContainerInstanceResponseTypeDef,
     RegisterTaskDefinitionResponseTypeDef,
-    ResourceOutputTypeDef,
-    ResourceTypeDef,
+    ResourceUnionTypeDef,
     RunTaskResponseTypeDef,
     RuntimePlatformTypeDef,
     ScaleTypeDef,
-    ServiceConnectConfigurationOutputTypeDef,
-    ServiceConnectConfigurationTypeDef,
+    ServiceConnectConfigurationUnionTypeDef,
     ServiceRegistryTypeDef,
     StartTaskResponseTypeDef,
     StopTaskResponseTypeDef,
     SubmitAttachmentStateChangesResponseTypeDef,
     SubmitContainerStateChangeResponseTypeDef,
     SubmitTaskStateChangeResponseTypeDef,
     TagTypeDef,
     TaskDefinitionPlacementConstraintTypeDef,
-    TaskOverrideOutputTypeDef,
-    TaskOverrideTypeDef,
+    TaskOverrideUnionTypeDef,
+    TimestampTypeDef,
     UpdateCapacityProviderResponseTypeDef,
     UpdateClusterResponseTypeDef,
     UpdateClusterSettingsResponseTypeDef,
     UpdateContainerAgentResponseTypeDef,
     UpdateContainerInstancesStateResponseTypeDef,
     UpdateServicePrimaryTaskSetResponseTypeDef,
     UpdateServiceResponseTypeDef,
     UpdateTaskProtectionResponseTypeDef,
     UpdateTaskSetResponseTypeDef,
     VersionInfoTypeDef,
-    VolumeOutputTypeDef,
-    VolumeTypeDef,
+    VolumeUnionTypeDef,
 )
 from .waiter import (
     ServicesInactiveWaiter,
     ServicesStableWaiter,
     TasksRunningWaiter,
     TasksStoppedWaiter,
 )
@@ -262,32 +254,26 @@
         serviceRegistries: Sequence[ServiceRegistryTypeDef] = ...,
         desiredCount: int = ...,
         clientToken: str = ...,
         launchType: LaunchTypeType = ...,
         capacityProviderStrategy: Sequence[CapacityProviderStrategyItemTypeDef] = ...,
         platformVersion: str = ...,
         role: str = ...,
-        deploymentConfiguration: Union[
-            DeploymentConfigurationTypeDef, DeploymentConfigurationOutputTypeDef
-        ] = ...,
+        deploymentConfiguration: DeploymentConfigurationUnionTypeDef = ...,
         placementConstraints: Sequence[PlacementConstraintTypeDef] = ...,
         placementStrategy: Sequence[PlacementStrategyTypeDef] = ...,
-        networkConfiguration: Union[
-            NetworkConfigurationTypeDef, NetworkConfigurationOutputTypeDef
-        ] = ...,
+        networkConfiguration: NetworkConfigurationUnionTypeDef = ...,
         healthCheckGracePeriodSeconds: int = ...,
         schedulingStrategy: SchedulingStrategyType = ...,
         deploymentController: DeploymentControllerTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...,
         enableECSManagedTags: bool = ...,
         propagateTags: PropagateTagsType = ...,
         enableExecuteCommand: bool = ...,
-        serviceConnectConfiguration: Union[
-            ServiceConnectConfigurationTypeDef, ServiceConnectConfigurationOutputTypeDef
-        ] = ...
+        serviceConnectConfiguration: ServiceConnectConfigurationUnionTypeDef = ...
     ) -> CreateServiceResponseTypeDef:
         """
         Runs and maintains your desired number of tasks from a specified task
         definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.create_service)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#create_service)
@@ -295,17 +281,15 @@
     def create_task_set(
         self,
         *,
         service: str,
         cluster: str,
         taskDefinition: str,
         externalId: str = ...,
-        networkConfiguration: Union[
-            NetworkConfigurationTypeDef, NetworkConfigurationOutputTypeDef
-        ] = ...,
+        networkConfiguration: NetworkConfigurationUnionTypeDef = ...,
         loadBalancers: Sequence[LoadBalancerTypeDef] = ...,
         serviceRegistries: Sequence[ServiceRegistryTypeDef] = ...,
         launchType: LaunchTypeType = ...,
         capacityProviderStrategy: Sequence[CapacityProviderStrategyItemTypeDef] = ...,
         platformVersion: str = ...,
         scale: ScaleTypeDef = ...,
         clientToken: str = ...,
@@ -705,15 +689,15 @@
         """
     def register_container_instance(
         self,
         *,
         cluster: str = ...,
         instanceIdentityDocument: str = ...,
         instanceIdentityDocumentSignature: str = ...,
-        totalResources: Sequence[Union[ResourceTypeDef, ResourceOutputTypeDef]] = ...,
+        totalResources: Sequence[ResourceUnionTypeDef] = ...,
         versionInfo: VersionInfoTypeDef = ...,
         containerInstanceArn: str = ...,
         attributes: Sequence[AttributeTypeDef] = ...,
         platformDevices: Sequence[PlatformDeviceTypeDef] = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> RegisterContainerInstanceResponseTypeDef:
         """
@@ -722,29 +706,27 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.register_container_instance)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#register_container_instance)
         """
     def register_task_definition(
         self,
         *,
         family: str,
-        containerDefinitions: Sequence[
-            Union[ContainerDefinitionTypeDef, ContainerDefinitionOutputTypeDef]
-        ],
+        containerDefinitions: Sequence[ContainerDefinitionUnionTypeDef],
         taskRoleArn: str = ...,
         executionRoleArn: str = ...,
         networkMode: NetworkModeType = ...,
-        volumes: Sequence[Union[VolumeTypeDef, VolumeOutputTypeDef]] = ...,
+        volumes: Sequence[VolumeUnionTypeDef] = ...,
         placementConstraints: Sequence[TaskDefinitionPlacementConstraintTypeDef] = ...,
         requiresCompatibilities: Sequence[CompatibilityType] = ...,
         cpu: str = ...,
         memory: str = ...,
         tags: Sequence[TagTypeDef] = ...,
         pidMode: PidModeType = ...,
         ipcMode: IpcModeType = ...,
-        proxyConfiguration: Union[ProxyConfigurationTypeDef, ProxyConfigurationOutputTypeDef] = ...,
+        proxyConfiguration: ProxyConfigurationUnionTypeDef = ...,
         inferenceAccelerators: Sequence[InferenceAcceleratorTypeDef] = ...,
         ephemeralStorage: EphemeralStorageTypeDef = ...,
         runtimePlatform: RuntimePlatformTypeDef = ...
     ) -> RegisterTaskDefinitionResponseTypeDef:
         """
         Registers a new task definition from the supplied `family` and
         `containerDefinitions`.
@@ -759,18 +741,16 @@
         capacityProviderStrategy: Sequence[CapacityProviderStrategyItemTypeDef] = ...,
         cluster: str = ...,
         count: int = ...,
         enableECSManagedTags: bool = ...,
         enableExecuteCommand: bool = ...,
         group: str = ...,
         launchType: LaunchTypeType = ...,
-        networkConfiguration: Union[
-            NetworkConfigurationTypeDef, NetworkConfigurationOutputTypeDef
-        ] = ...,
-        overrides: Union[TaskOverrideTypeDef, TaskOverrideOutputTypeDef] = ...,
+        networkConfiguration: NetworkConfigurationUnionTypeDef = ...,
+        overrides: TaskOverrideUnionTypeDef = ...,
         placementConstraints: Sequence[PlacementConstraintTypeDef] = ...,
         placementStrategy: Sequence[PlacementStrategyTypeDef] = ...,
         platformVersion: str = ...,
         propagateTags: PropagateTagsType = ...,
         referenceId: str = ...,
         startedBy: str = ...,
         tags: Sequence[TagTypeDef] = ...
@@ -786,18 +766,16 @@
         *,
         containerInstances: Sequence[str],
         taskDefinition: str,
         cluster: str = ...,
         enableECSManagedTags: bool = ...,
         enableExecuteCommand: bool = ...,
         group: str = ...,
-        networkConfiguration: Union[
-            NetworkConfigurationTypeDef, NetworkConfigurationOutputTypeDef
-        ] = ...,
-        overrides: Union[TaskOverrideTypeDef, TaskOverrideOutputTypeDef] = ...,
+        networkConfiguration: NetworkConfigurationUnionTypeDef = ...,
+        overrides: TaskOverrideUnionTypeDef = ...,
         propagateTags: PropagateTagsType = ...,
         referenceId: str = ...,
         startedBy: str = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> StartTaskResponseTypeDef:
         """
         Starts a new task from the specified task definition on the specified container
@@ -848,17 +826,17 @@
         cluster: str = ...,
         task: str = ...,
         status: str = ...,
         reason: str = ...,
         containers: Sequence[ContainerStateChangeTypeDef] = ...,
         attachments: Sequence[AttachmentStateChangeTypeDef] = ...,
         managedAgents: Sequence[ManagedAgentStateChangeTypeDef] = ...,
-        pullStartedAt: Union[datetime, str] = ...,
-        pullStoppedAt: Union[datetime, str] = ...,
-        executionStoppedAt: Union[datetime, str] = ...
+        pullStartedAt: TimestampTypeDef = ...,
+        pullStoppedAt: TimestampTypeDef = ...,
+        executionStoppedAt: TimestampTypeDef = ...
     ) -> SubmitTaskStateChangeResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.submit_task_state_change)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#submit_task_state_change)
         """
@@ -934,33 +912,27 @@
         self,
         *,
         service: str,
         cluster: str = ...,
         desiredCount: int = ...,
         taskDefinition: str = ...,
         capacityProviderStrategy: Sequence[CapacityProviderStrategyItemTypeDef] = ...,
-        deploymentConfiguration: Union[
-            DeploymentConfigurationTypeDef, DeploymentConfigurationOutputTypeDef
-        ] = ...,
-        networkConfiguration: Union[
-            NetworkConfigurationTypeDef, NetworkConfigurationOutputTypeDef
-        ] = ...,
+        deploymentConfiguration: DeploymentConfigurationUnionTypeDef = ...,
+        networkConfiguration: NetworkConfigurationUnionTypeDef = ...,
         placementConstraints: Sequence[PlacementConstraintTypeDef] = ...,
         placementStrategy: Sequence[PlacementStrategyTypeDef] = ...,
         platformVersion: str = ...,
         forceNewDeployment: bool = ...,
         healthCheckGracePeriodSeconds: int = ...,
         enableExecuteCommand: bool = ...,
         enableECSManagedTags: bool = ...,
         loadBalancers: Sequence[LoadBalancerTypeDef] = ...,
         propagateTags: PropagateTagsType = ...,
         serviceRegistries: Sequence[ServiceRegistryTypeDef] = ...,
-        serviceConnectConfiguration: Union[
-            ServiceConnectConfigurationTypeDef, ServiceConnectConfigurationOutputTypeDef
-        ] = ...
+        serviceConnectConfiguration: ServiceConnectConfigurationUnionTypeDef = ...
     ) -> UpdateServiceResponseTypeDef:
         """
         Modifies the parameters of a service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.update_service)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#update_service)
         """
```

### Comparing `mypy-boto3-ecs-1.28.15.post1/mypy_boto3_ecs/literals.py` & `mypy-boto3-ecs-1.28.16/mypy_boto3_ecs/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecs-1.28.15.post1/mypy_boto3_ecs/literals.pyi` & `mypy-boto3-ecs-1.28.16/mypy_boto3_ecs/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecs-1.28.15.post1/mypy_boto3_ecs/paginator.py` & `mypy-boto3-ecs-1.28.16/mypy_boto3_ecs/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecs-1.28.15.post1/mypy_boto3_ecs/paginator.pyi` & `mypy-boto3-ecs-1.28.16/mypy_boto3_ecs/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecs-1.28.15.post1/mypy_boto3_ecs/type_defs.py` & `mypy-boto3-ecs-1.28.16/mypy_boto3_ecs/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_ecs.type_defs import AttachmentStateChangeTypeDef
 
-    data: AttachmentStateChangeTypeDef = {...}
+    data: AttachmentStateChangeTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -67,15 +67,14 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AttachmentStateChangeTypeDef",
     "KeyValuePairTypeDef",
     "AttributeTypeDef",
     "ManagedScalingTypeDef",
     "AwsVpcConfigurationOutputTypeDef",
     "AwsVpcConfigurationTypeDef",
@@ -165,20 +164,21 @@
     "ListTaskDefinitionFamiliesRequestRequestTypeDef",
     "ListTaskDefinitionsRequestRequestTypeDef",
     "ListTasksRequestRequestTypeDef",
     "ManagedAgentStateChangeTypeDef",
     "PlatformDeviceTypeDef",
     "PutAccountSettingDefaultRequestRequestTypeDef",
     "PutAccountSettingRequestRequestTypeDef",
-    "ResourceTypeDef",
     "RuntimePlatformTypeDef",
     "TaskDefinitionPlacementConstraintTypeDef",
+    "ResourceTypeDef",
     "ServiceConnectClientAliasTypeDef",
     "ServiceEventTypeDef",
     "StopTaskRequestRequestTypeDef",
+    "TimestampTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateContainerAgentRequestRequestTypeDef",
     "UpdateContainerInstancesStateRequestRequestTypeDef",
     "UpdateServicePrimaryTaskSetRequestRequestTypeDef",
     "UpdateTaskProtectionRequestRequestTypeDef",
     "SubmitAttachmentStateChangesRequestRequestTypeDef",
     "AttachmentTypeDef",
@@ -240,57 +240,64 @@
     "ListClustersRequestListClustersPaginateTypeDef",
     "ListContainerInstancesRequestListContainerInstancesPaginateTypeDef",
     "ListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef",
     "ListServicesRequestListServicesPaginateTypeDef",
     "ListTaskDefinitionFamiliesRequestListTaskDefinitionFamiliesPaginateTypeDef",
     "ListTaskDefinitionsRequestListTaskDefinitionsPaginateTypeDef",
     "ListTasksRequestListTasksPaginateTypeDef",
-    "RegisterContainerInstanceRequestRequestTypeDef",
+    "ResourceUnionTypeDef",
     "ServiceConnectServiceOutputTypeDef",
     "ServiceConnectServiceTypeDef",
+    "ProxyConfigurationUnionTypeDef",
     "CapacityProviderTypeDef",
     "CreateCapacityProviderRequestRequestTypeDef",
     "UpdateCapacityProviderRequestRequestTypeDef",
     "TaskSetTypeDef",
     "CreateTaskSetRequestRequestTypeDef",
+    "NetworkConfigurationUnionTypeDef",
     "TaskOverrideOutputTypeDef",
     "TaskOverrideTypeDef",
     "ContainerInstanceTypeDef",
     "SubmitTaskStateChangeRequestRequestTypeDef",
+    "DeploymentConfigurationUnionTypeDef",
     "ClusterConfigurationTypeDef",
     "VolumeOutputTypeDef",
     "VolumeTypeDef",
     "ContainerDefinitionOutputTypeDef",
     "ContainerDefinitionTypeDef",
+    "RegisterContainerInstanceRequestRequestTypeDef",
     "ServiceConnectConfigurationOutputTypeDef",
     "ServiceConnectConfigurationTypeDef",
     "CreateCapacityProviderResponseTypeDef",
     "DeleteCapacityProviderResponseTypeDef",
     "DescribeCapacityProvidersResponseTypeDef",
     "UpdateCapacityProviderResponseTypeDef",
     "CreateTaskSetResponseTypeDef",
     "DeleteTaskSetResponseTypeDef",
     "DescribeTaskSetsResponseTypeDef",
     "UpdateServicePrimaryTaskSetResponseTypeDef",
     "UpdateTaskSetResponseTypeDef",
     "TaskTypeDef",
     "RunTaskRequestRequestTypeDef",
     "StartTaskRequestRequestTypeDef",
+    "TaskOverrideUnionTypeDef",
     "DeregisterContainerInstanceResponseTypeDef",
     "DescribeContainerInstancesResponseTypeDef",
     "RegisterContainerInstanceResponseTypeDef",
     "UpdateContainerAgentResponseTypeDef",
     "UpdateContainerInstancesStateResponseTypeDef",
     "ClusterTypeDef",
     "CreateClusterRequestRequestTypeDef",
     "UpdateClusterRequestRequestTypeDef",
+    "VolumeUnionTypeDef",
     "TaskDefinitionTypeDef",
-    "RegisterTaskDefinitionRequestRequestTypeDef",
+    "ContainerDefinitionUnionTypeDef",
     "DeploymentTypeDef",
     "CreateServiceRequestRequestTypeDef",
+    "ServiceConnectConfigurationUnionTypeDef",
     "UpdateServiceRequestRequestTypeDef",
     "DescribeTasksResponseTypeDef",
     "RunTaskResponseTypeDef",
     "StartTaskResponseTypeDef",
     "StopTaskResponseTypeDef",
     "CreateClusterResponseTypeDef",
     "DeleteClusterResponseTypeDef",
@@ -298,14 +305,15 @@
     "PutClusterCapacityProvidersResponseTypeDef",
     "UpdateClusterResponseTypeDef",
     "UpdateClusterSettingsResponseTypeDef",
     "DeleteTaskDefinitionsResponseTypeDef",
     "DeregisterTaskDefinitionResponseTypeDef",
     "DescribeTaskDefinitionResponseTypeDef",
     "RegisterTaskDefinitionResponseTypeDef",
+    "RegisterTaskDefinitionRequestRequestTypeDef",
     "ServiceTypeDef",
     "CreateServiceResponseTypeDef",
     "DeleteServiceResponseTypeDef",
     "DescribeServicesResponseTypeDef",
     "UpdateServiceResponseTypeDef",
 )
 
@@ -338,19 +346,17 @@
         "value": str,
         "targetType": Literal["container-instance"],
         "targetId": str,
     },
     total=False,
 )
 
-
 class AttributeTypeDef(_RequiredAttributeTypeDef, _OptionalAttributeTypeDef):
     pass
 
-
 ManagedScalingTypeDef = TypedDict(
     "ManagedScalingTypeDef",
     {
         "status": ManagedScalingStatusType,
         "targetCapacity": int,
         "minimumScalingStepSize": int,
         "maximumScalingStepSize": int,
@@ -370,21 +376,19 @@
     {
         "securityGroups": List[str],
         "assignPublicIp": AssignPublicIpType,
     },
     total=False,
 )
 
-
 class AwsVpcConfigurationOutputTypeDef(
     _RequiredAwsVpcConfigurationOutputTypeDef, _OptionalAwsVpcConfigurationOutputTypeDef
 ):
     pass
 
-
 _RequiredAwsVpcConfigurationTypeDef = TypedDict(
     "_RequiredAwsVpcConfigurationTypeDef",
     {
         "subnets": Sequence[str],
     },
 )
 _OptionalAwsVpcConfigurationTypeDef = TypedDict(
@@ -392,21 +396,19 @@
     {
         "securityGroups": Sequence[str],
         "assignPublicIp": AssignPublicIpType,
     },
     total=False,
 )
 
-
 class AwsVpcConfigurationTypeDef(
     _RequiredAwsVpcConfigurationTypeDef, _OptionalAwsVpcConfigurationTypeDef
 ):
     pass
 
-
 _RequiredCapacityProviderStrategyItemTypeDef = TypedDict(
     "_RequiredCapacityProviderStrategyItemTypeDef",
     {
         "capacityProvider": str,
     },
 )
 _OptionalCapacityProviderStrategyItemTypeDef = TypedDict(
@@ -414,21 +416,19 @@
     {
         "weight": int,
         "base": int,
     },
     total=False,
 )
 
-
 class CapacityProviderStrategyItemTypeDef(
     _RequiredCapacityProviderStrategyItemTypeDef, _OptionalCapacityProviderStrategyItemTypeDef
 ):
     pass
 
-
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "key": str,
         "value": str,
     },
     total=False,
@@ -484,21 +484,19 @@
     "_OptionalFirelensConfigurationOutputTypeDef",
     {
         "options": Dict[str, str],
     },
     total=False,
 )
 
-
 class FirelensConfigurationOutputTypeDef(
     _RequiredFirelensConfigurationOutputTypeDef, _OptionalFirelensConfigurationOutputTypeDef
 ):
     pass
 
-
 _RequiredHealthCheckOutputTypeDef = TypedDict(
     "_RequiredHealthCheckOutputTypeDef",
     {
         "command": List[str],
     },
 )
 _OptionalHealthCheckOutputTypeDef = TypedDict(
@@ -508,21 +506,19 @@
         "timeout": int,
         "retries": int,
         "startPeriod": int,
     },
     total=False,
 )
 
-
 class HealthCheckOutputTypeDef(
     _RequiredHealthCheckOutputTypeDef, _OptionalHealthCheckOutputTypeDef
 ):
     pass
 
-
 HostEntryTypeDef = TypedDict(
     "HostEntryTypeDef",
     {
         "hostname": str,
         "ipAddress": str,
     },
 )
@@ -610,21 +606,19 @@
     "_OptionalFirelensConfigurationTypeDef",
     {
         "options": Mapping[str, str],
     },
     total=False,
 )
 
-
 class FirelensConfigurationTypeDef(
     _RequiredFirelensConfigurationTypeDef, _OptionalFirelensConfigurationTypeDef
 ):
     pass
 
-
 _RequiredHealthCheckTypeDef = TypedDict(
     "_RequiredHealthCheckTypeDef",
     {
         "command": Sequence[str],
     },
 )
 _OptionalHealthCheckTypeDef = TypedDict(
@@ -634,19 +628,17 @@
         "timeout": int,
         "retries": int,
         "startPeriod": int,
     },
     total=False,
 )
 
-
 class HealthCheckTypeDef(_RequiredHealthCheckTypeDef, _OptionalHealthCheckTypeDef):
     pass
 
-
 InstanceHealthCheckResultTypeDef = TypedDict(
     "InstanceHealthCheckResultTypeDef",
     {
         "type": Literal["CONTAINER_RUNTIME"],
         "status": InstanceHealthCheckStateType,
         "lastUpdated": datetime,
         "lastStatusChange": datetime,
@@ -788,22 +780,20 @@
     "_OptionalDeleteAccountSettingRequestRequestTypeDef",
     {
         "principalArn": str,
     },
     total=False,
 )
 
-
 class DeleteAccountSettingRequestRequestTypeDef(
     _RequiredDeleteAccountSettingRequestRequestTypeDef,
     _OptionalDeleteAccountSettingRequestRequestTypeDef,
 ):
     pass
 
-
 SettingTypeDef = TypedDict(
     "SettingTypeDef",
     {
         "name": SettingNameType,
         "value": str,
         "principalArn": str,
     },
@@ -835,21 +825,19 @@
     {
         "cluster": str,
         "force": bool,
     },
     total=False,
 )
 
-
 class DeleteServiceRequestRequestTypeDef(
     _RequiredDeleteServiceRequestRequestTypeDef, _OptionalDeleteServiceRequestRequestTypeDef
 ):
     pass
 
-
 DeleteTaskDefinitionsRequestRequestTypeDef = TypedDict(
     "DeleteTaskDefinitionsRequestRequestTypeDef",
     {
         "taskDefinitions": Sequence[str],
     },
 )
 
@@ -875,21 +863,19 @@
     "_OptionalDeleteTaskSetRequestRequestTypeDef",
     {
         "force": bool,
     },
     total=False,
 )
 
-
 class DeleteTaskSetRequestRequestTypeDef(
     _RequiredDeleteTaskSetRequestRequestTypeDef, _OptionalDeleteTaskSetRequestRequestTypeDef
 ):
     pass
 
-
 DeploymentAlarmsOutputTypeDef = TypedDict(
     "DeploymentAlarmsOutputTypeDef",
     {
         "alarmNames": List[str],
         "enable": bool,
         "rollback": bool,
     },
@@ -932,22 +918,20 @@
     {
         "cluster": str,
         "force": bool,
     },
     total=False,
 )
 
-
 class DeregisterContainerInstanceRequestRequestTypeDef(
     _RequiredDeregisterContainerInstanceRequestRequestTypeDef,
     _OptionalDeregisterContainerInstanceRequestRequestTypeDef,
 ):
     pass
 
-
 DeregisterTaskDefinitionRequestRequestTypeDef = TypedDict(
     "DeregisterTaskDefinitionRequestRequestTypeDef",
     {
         "taskDefinition": str,
     },
 )
 
@@ -982,22 +966,20 @@
     {
         "cluster": str,
         "include": Sequence[ContainerInstanceFieldType],
     },
     total=False,
 )
 
-
 class DescribeContainerInstancesRequestRequestTypeDef(
     _RequiredDescribeContainerInstancesRequestRequestTypeDef,
     _OptionalDescribeContainerInstancesRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDescribeServicesRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeServicesRequestRequestTypeDef",
     {
         "services": Sequence[str],
     },
 )
 _OptionalDescribeServicesRequestRequestTypeDef = TypedDict(
@@ -1005,21 +987,19 @@
     {
         "cluster": str,
         "include": Sequence[Literal["TAGS"]],
     },
     total=False,
 )
 
-
 class DescribeServicesRequestRequestTypeDef(
     _RequiredDescribeServicesRequestRequestTypeDef, _OptionalDescribeServicesRequestRequestTypeDef
 ):
     pass
 
-
 WaiterConfigTypeDef = TypedDict(
     "WaiterConfigTypeDef",
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
@@ -1035,22 +1015,20 @@
     "_OptionalDescribeTaskDefinitionRequestRequestTypeDef",
     {
         "include": Sequence[Literal["TAGS"]],
     },
     total=False,
 )
 
-
 class DescribeTaskDefinitionRequestRequestTypeDef(
     _RequiredDescribeTaskDefinitionRequestRequestTypeDef,
     _OptionalDescribeTaskDefinitionRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDescribeTaskSetsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeTaskSetsRequestRequestTypeDef",
     {
         "cluster": str,
         "service": str,
     },
 )
@@ -1059,21 +1037,19 @@
     {
         "taskSets": Sequence[str],
         "include": Sequence[Literal["TAGS"]],
     },
     total=False,
 )
 
-
 class DescribeTaskSetsRequestRequestTypeDef(
     _RequiredDescribeTaskSetsRequestRequestTypeDef, _OptionalDescribeTaskSetsRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredDescribeTasksRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeTasksRequestRequestTypeDef",
     {
         "tasks": Sequence[str],
     },
 )
 _OptionalDescribeTasksRequestRequestTypeDef = TypedDict(
@@ -1081,21 +1057,19 @@
     {
         "cluster": str,
         "include": Sequence[Literal["TAGS"]],
     },
     total=False,
 )
 
-
 class DescribeTasksRequestRequestTypeDef(
     _RequiredDescribeTasksRequestRequestTypeDef, _OptionalDescribeTasksRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredDeviceOutputTypeDef = TypedDict(
     "_RequiredDeviceOutputTypeDef",
     {
         "hostPath": str,
     },
 )
 _OptionalDeviceOutputTypeDef = TypedDict(
@@ -1103,19 +1077,17 @@
     {
         "containerPath": str,
         "permissions": List[DeviceCgroupPermissionType],
     },
     total=False,
 )
 
-
 class DeviceOutputTypeDef(_RequiredDeviceOutputTypeDef, _OptionalDeviceOutputTypeDef):
     pass
 
-
 _RequiredDeviceTypeDef = TypedDict(
     "_RequiredDeviceTypeDef",
     {
         "hostPath": str,
     },
 )
 _OptionalDeviceTypeDef = TypedDict(
@@ -1123,19 +1095,17 @@
     {
         "containerPath": str,
         "permissions": Sequence[DeviceCgroupPermissionType],
     },
     total=False,
 )
 
-
 class DeviceTypeDef(_RequiredDeviceTypeDef, _OptionalDeviceTypeDef):
     pass
 
-
 DiscoverPollEndpointRequestRequestTypeDef = TypedDict(
     "DiscoverPollEndpointRequestRequestTypeDef",
     {
         "containerInstance": str,
         "cluster": str,
     },
     total=False,
@@ -1206,21 +1176,19 @@
     {
         "cluster": str,
         "container": str,
     },
     total=False,
 )
 
-
 class ExecuteCommandRequestRequestTypeDef(
     _RequiredExecuteCommandRequestRequestTypeDef, _OptionalExecuteCommandRequestRequestTypeDef
 ):
     pass
 
-
 SessionTypeDef = TypedDict(
     "SessionTypeDef",
     {
         "sessionId": str,
         "streamUrl": str,
         "tokenValue": str,
     },
@@ -1245,21 +1213,19 @@
     "_OptionalGetTaskProtectionRequestRequestTypeDef",
     {
         "tasks": Sequence[str],
     },
     total=False,
 )
 
-
 class GetTaskProtectionRequestRequestTypeDef(
     _RequiredGetTaskProtectionRequestRequestTypeDef, _OptionalGetTaskProtectionRequestRequestTypeDef
 ):
     pass
 
-
 ProtectedTaskTypeDef = TypedDict(
     "ProtectedTaskTypeDef",
     {
         "taskArn": str,
         "protectionEnabled": bool,
         "expirationDate": datetime,
     },
@@ -1320,19 +1286,17 @@
     "_OptionalTmpfsOutputTypeDef",
     {
         "mountOptions": List[str],
     },
     total=False,
 )
 
-
 class TmpfsOutputTypeDef(_RequiredTmpfsOutputTypeDef, _OptionalTmpfsOutputTypeDef):
     pass
 
-
 _RequiredTmpfsTypeDef = TypedDict(
     "_RequiredTmpfsTypeDef",
     {
         "containerPath": str,
         "size": int,
     },
 )
@@ -1340,19 +1304,17 @@
     "_OptionalTmpfsTypeDef",
     {
         "mountOptions": Sequence[str],
     },
     total=False,
 )
 
-
 class TmpfsTypeDef(_RequiredTmpfsTypeDef, _OptionalTmpfsTypeDef):
     pass
 
-
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
@@ -1386,21 +1348,19 @@
         "attributeValue": str,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class ListAttributesRequestRequestTypeDef(
     _RequiredListAttributesRequestRequestTypeDef, _OptionalListAttributesRequestRequestTypeDef
 ):
     pass
 
-
 ListClustersRequestRequestTypeDef = TypedDict(
     "ListClustersRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
@@ -1429,22 +1389,20 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class ListServicesByNamespaceRequestRequestTypeDef(
     _RequiredListServicesByNamespaceRequestRequestTypeDef,
     _OptionalListServicesByNamespaceRequestRequestTypeDef,
 ):
     pass
 
-
 ListServicesRequestRequestTypeDef = TypedDict(
     "ListServicesRequestRequestTypeDef",
     {
         "cluster": str,
         "nextToken": str,
         "maxResults": int,
         "launchType": LaunchTypeType,
@@ -1511,21 +1469,19 @@
     "_OptionalManagedAgentStateChangeTypeDef",
     {
         "reason": str,
     },
     total=False,
 )
 
-
 class ManagedAgentStateChangeTypeDef(
     _RequiredManagedAgentStateChangeTypeDef, _OptionalManagedAgentStateChangeTypeDef
 ):
     pass
 
-
 PlatformDeviceTypeDef = TypedDict(
     "PlatformDeviceTypeDef",
     {
         "id": str,
         "type": Literal["GPU"],
     },
 )
@@ -1549,34 +1505,19 @@
     "_OptionalPutAccountSettingRequestRequestTypeDef",
     {
         "principalArn": str,
     },
     total=False,
 )
 
-
 class PutAccountSettingRequestRequestTypeDef(
     _RequiredPutAccountSettingRequestRequestTypeDef, _OptionalPutAccountSettingRequestRequestTypeDef
 ):
     pass
 
-
-ResourceTypeDef = TypedDict(
-    "ResourceTypeDef",
-    {
-        "name": str,
-        "type": str,
-        "doubleValue": float,
-        "longValue": int,
-        "integerValue": int,
-        "stringSetValue": Sequence[str],
-    },
-    total=False,
-)
-
 RuntimePlatformTypeDef = TypedDict(
     "RuntimePlatformTypeDef",
     {
         "cpuArchitecture": CPUArchitectureType,
         "operatingSystemFamily": OSFamilyType,
     },
     total=False,
@@ -1587,35 +1528,46 @@
     {
         "type": Literal["memberOf"],
         "expression": str,
     },
     total=False,
 )
 
+ResourceTypeDef = TypedDict(
+    "ResourceTypeDef",
+    {
+        "name": str,
+        "type": str,
+        "doubleValue": float,
+        "longValue": int,
+        "integerValue": int,
+        "stringSetValue": Sequence[str],
+    },
+    total=False,
+)
+
 _RequiredServiceConnectClientAliasTypeDef = TypedDict(
     "_RequiredServiceConnectClientAliasTypeDef",
     {
         "port": int,
     },
 )
 _OptionalServiceConnectClientAliasTypeDef = TypedDict(
     "_OptionalServiceConnectClientAliasTypeDef",
     {
         "dnsName": str,
     },
     total=False,
 )
 
-
 class ServiceConnectClientAliasTypeDef(
     _RequiredServiceConnectClientAliasTypeDef, _OptionalServiceConnectClientAliasTypeDef
 ):
     pass
 
-
 ServiceEventTypeDef = TypedDict(
     "ServiceEventTypeDef",
     {
         "id": str,
         "createdAt": datetime,
         "message": str,
     },
@@ -1633,21 +1585,20 @@
     {
         "cluster": str,
         "reason": str,
     },
     total=False,
 )
 
-
 class StopTaskRequestRequestTypeDef(
     _RequiredStopTaskRequestRequestTypeDef, _OptionalStopTaskRequestRequestTypeDef
 ):
     pass
 
-
+TimestampTypeDef = Union[datetime, str]
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
@@ -1662,22 +1613,20 @@
     "_OptionalUpdateContainerAgentRequestRequestTypeDef",
     {
         "cluster": str,
     },
     total=False,
 )
 
-
 class UpdateContainerAgentRequestRequestTypeDef(
     _RequiredUpdateContainerAgentRequestRequestTypeDef,
     _OptionalUpdateContainerAgentRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateContainerInstancesStateRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateContainerInstancesStateRequestRequestTypeDef",
     {
         "containerInstances": Sequence[str],
         "status": ContainerInstanceStatusType,
     },
 )
@@ -1685,22 +1634,20 @@
     "_OptionalUpdateContainerInstancesStateRequestRequestTypeDef",
     {
         "cluster": str,
     },
     total=False,
 )
 
-
 class UpdateContainerInstancesStateRequestRequestTypeDef(
     _RequiredUpdateContainerInstancesStateRequestRequestTypeDef,
     _OptionalUpdateContainerInstancesStateRequestRequestTypeDef,
 ):
     pass
 
-
 UpdateServicePrimaryTaskSetRequestRequestTypeDef = TypedDict(
     "UpdateServicePrimaryTaskSetRequestRequestTypeDef",
     {
         "cluster": str,
         "service": str,
         "primaryTaskSet": str,
     },
@@ -1718,44 +1665,40 @@
     "_OptionalUpdateTaskProtectionRequestRequestTypeDef",
     {
         "expiresInMinutes": int,
     },
     total=False,
 )
 
-
 class UpdateTaskProtectionRequestRequestTypeDef(
     _RequiredUpdateTaskProtectionRequestRequestTypeDef,
     _OptionalUpdateTaskProtectionRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredSubmitAttachmentStateChangesRequestRequestTypeDef = TypedDict(
     "_RequiredSubmitAttachmentStateChangesRequestRequestTypeDef",
     {
         "attachments": Sequence[AttachmentStateChangeTypeDef],
     },
 )
 _OptionalSubmitAttachmentStateChangesRequestRequestTypeDef = TypedDict(
     "_OptionalSubmitAttachmentStateChangesRequestRequestTypeDef",
     {
         "cluster": str,
     },
     total=False,
 )
 
-
 class SubmitAttachmentStateChangesRequestRequestTypeDef(
     _RequiredSubmitAttachmentStateChangesRequestRequestTypeDef,
     _OptionalSubmitAttachmentStateChangesRequestRequestTypeDef,
 ):
     pass
 
-
 AttachmentTypeDef = TypedDict(
     "AttachmentTypeDef",
     {
         "id": str,
         "type": str,
         "status": str,
         "details": List[KeyValuePairTypeDef],
@@ -1774,21 +1717,19 @@
     {
         "type": Literal["APPMESH"],
         "properties": List[KeyValuePairTypeDef],
     },
     total=False,
 )
 
-
 class ProxyConfigurationOutputTypeDef(
     _RequiredProxyConfigurationOutputTypeDef, _OptionalProxyConfigurationOutputTypeDef
 ):
     pass
 
-
 _RequiredProxyConfigurationTypeDef = TypedDict(
     "_RequiredProxyConfigurationTypeDef",
     {
         "containerName": str,
     },
 )
 _OptionalProxyConfigurationTypeDef = TypedDict(
@@ -1796,63 +1737,57 @@
     {
         "type": Literal["APPMESH"],
         "properties": Sequence[KeyValuePairTypeDef],
     },
     total=False,
 )
 
-
 class ProxyConfigurationTypeDef(
     _RequiredProxyConfigurationTypeDef, _OptionalProxyConfigurationTypeDef
 ):
     pass
 
-
 _RequiredDeleteAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteAttributesRequestRequestTypeDef",
     {
         "attributes": Sequence[AttributeTypeDef],
     },
 )
 _OptionalDeleteAttributesRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteAttributesRequestRequestTypeDef",
     {
         "cluster": str,
     },
     total=False,
 )
 
-
 class DeleteAttributesRequestRequestTypeDef(
     _RequiredDeleteAttributesRequestRequestTypeDef, _OptionalDeleteAttributesRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredPutAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredPutAttributesRequestRequestTypeDef",
     {
         "attributes": Sequence[AttributeTypeDef],
     },
 )
 _OptionalPutAttributesRequestRequestTypeDef = TypedDict(
     "_OptionalPutAttributesRequestRequestTypeDef",
     {
         "cluster": str,
     },
     total=False,
 )
 
-
 class PutAttributesRequestRequestTypeDef(
     _RequiredPutAttributesRequestRequestTypeDef, _OptionalPutAttributesRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredAutoScalingGroupProviderTypeDef = TypedDict(
     "_RequiredAutoScalingGroupProviderTypeDef",
     {
         "autoScalingGroupArn": str,
     },
 )
 _OptionalAutoScalingGroupProviderTypeDef = TypedDict(
@@ -1860,21 +1795,19 @@
     {
         "managedScaling": ManagedScalingTypeDef,
         "managedTerminationProtection": ManagedTerminationProtectionType,
     },
     total=False,
 )
 
-
 class AutoScalingGroupProviderTypeDef(
     _RequiredAutoScalingGroupProviderTypeDef, _OptionalAutoScalingGroupProviderTypeDef
 ):
     pass
 
-
 AutoScalingGroupProviderUpdateTypeDef = TypedDict(
     "AutoScalingGroupProviderUpdateTypeDef",
     {
         "managedScaling": ManagedScalingTypeDef,
         "managedTerminationProtection": ManagedTerminationProtectionType,
     },
     total=False,
@@ -1962,21 +1895,19 @@
     {
         "options": Dict[str, str],
         "secretOptions": List[SecretTypeDef],
     },
     total=False,
 )
 
-
 class LogConfigurationOutputTypeDef(
     _RequiredLogConfigurationOutputTypeDef, _OptionalLogConfigurationOutputTypeDef
 ):
     pass
 
-
 _RequiredLogConfigurationTypeDef = TypedDict(
     "_RequiredLogConfigurationTypeDef",
     {
         "logDriver": LogDriverType,
     },
 )
 _OptionalLogConfigurationTypeDef = TypedDict(
@@ -1984,19 +1915,17 @@
     {
         "options": Mapping[str, str],
         "secretOptions": Sequence[SecretTypeDef],
     },
     total=False,
 )
 
-
 class LogConfigurationTypeDef(_RequiredLogConfigurationTypeDef, _OptionalLogConfigurationTypeDef):
     pass
 
-
 ContainerInstanceHealthStatusTypeDef = TypedDict(
     "ContainerInstanceHealthStatusTypeDef",
     {
         "overallStatus": InstanceHealthCheckStateType,
         "details": List[InstanceHealthCheckResultTypeDef],
     },
     total=False,
@@ -2262,22 +2191,20 @@
         "cluster": str,
         "include": Sequence[Literal["TAGS"]],
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeServicesRequestServicesInactiveWaitTypeDef(
     _RequiredDescribeServicesRequestServicesInactiveWaitTypeDef,
     _OptionalDescribeServicesRequestServicesInactiveWaitTypeDef,
 ):
     pass
 
-
 _RequiredDescribeServicesRequestServicesStableWaitTypeDef = TypedDict(
     "_RequiredDescribeServicesRequestServicesStableWaitTypeDef",
     {
         "services": Sequence[str],
     },
 )
 _OptionalDescribeServicesRequestServicesStableWaitTypeDef = TypedDict(
@@ -2286,22 +2213,20 @@
         "cluster": str,
         "include": Sequence[Literal["TAGS"]],
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeServicesRequestServicesStableWaitTypeDef(
     _RequiredDescribeServicesRequestServicesStableWaitTypeDef,
     _OptionalDescribeServicesRequestServicesStableWaitTypeDef,
 ):
     pass
 
-
 _RequiredDescribeTasksRequestTasksRunningWaitTypeDef = TypedDict(
     "_RequiredDescribeTasksRequestTasksRunningWaitTypeDef",
     {
         "tasks": Sequence[str],
     },
 )
 _OptionalDescribeTasksRequestTasksRunningWaitTypeDef = TypedDict(
@@ -2310,22 +2235,20 @@
         "cluster": str,
         "include": Sequence[Literal["TAGS"]],
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeTasksRequestTasksRunningWaitTypeDef(
     _RequiredDescribeTasksRequestTasksRunningWaitTypeDef,
     _OptionalDescribeTasksRequestTasksRunningWaitTypeDef,
 ):
     pass
 
-
 _RequiredDescribeTasksRequestTasksStoppedWaitTypeDef = TypedDict(
     "_RequiredDescribeTasksRequestTasksStoppedWaitTypeDef",
     {
         "tasks": Sequence[str],
     },
 )
 _OptionalDescribeTasksRequestTasksStoppedWaitTypeDef = TypedDict(
@@ -2334,22 +2257,20 @@
         "cluster": str,
         "include": Sequence[Literal["TAGS"]],
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeTasksRequestTasksStoppedWaitTypeDef(
     _RequiredDescribeTasksRequestTasksStoppedWaitTypeDef,
     _OptionalDescribeTasksRequestTasksStoppedWaitTypeDef,
 ):
     pass
 
-
 _RequiredEFSVolumeConfigurationTypeDef = TypedDict(
     "_RequiredEFSVolumeConfigurationTypeDef",
     {
         "fileSystemId": str,
     },
 )
 _OptionalEFSVolumeConfigurationTypeDef = TypedDict(
@@ -2359,21 +2280,19 @@
         "transitEncryption": EFSTransitEncryptionType,
         "transitEncryptionPort": int,
         "authorizationConfig": EFSAuthorizationConfigTypeDef,
     },
     total=False,
 )
 
-
 class EFSVolumeConfigurationTypeDef(
     _RequiredEFSVolumeConfigurationTypeDef, _OptionalEFSVolumeConfigurationTypeDef
 ):
     pass
 
-
 ExecuteCommandConfigurationTypeDef = TypedDict(
     "ExecuteCommandConfigurationTypeDef",
     {
         "kmsKeyId": str,
         "logging": ExecuteCommandLoggingType,
         "logConfiguration": ExecuteCommandLogConfigurationTypeDef,
     },
@@ -2473,22 +2392,20 @@
         "attributeName": str,
         "attributeValue": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListAttributesRequestListAttributesPaginateTypeDef(
     _RequiredListAttributesRequestListAttributesPaginateTypeDef,
     _OptionalListAttributesRequestListAttributesPaginateTypeDef,
 ):
     pass
 
-
 ListClustersRequestListClustersPaginateTypeDef = TypedDict(
     "ListClustersRequestListClustersPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -2514,22 +2431,20 @@
     "_OptionalListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef(
     _RequiredListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef,
     _OptionalListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef,
 ):
     pass
 
-
 ListServicesRequestListServicesPaginateTypeDef = TypedDict(
     "ListServicesRequestListServicesPaginateTypeDef",
     {
         "cluster": str,
         "launchType": LaunchTypeType,
         "schedulingStrategy": SchedulingStrategyType,
         "PaginationConfig": PaginatorConfigTypeDef,
@@ -2569,30 +2484,15 @@
         "desiredStatus": DesiredStatusType,
         "launchType": LaunchTypeType,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-RegisterContainerInstanceRequestRequestTypeDef = TypedDict(
-    "RegisterContainerInstanceRequestRequestTypeDef",
-    {
-        "cluster": str,
-        "instanceIdentityDocument": str,
-        "instanceIdentityDocumentSignature": str,
-        "totalResources": Sequence[Union[ResourceTypeDef, ResourceOutputTypeDef]],
-        "versionInfo": VersionInfoTypeDef,
-        "containerInstanceArn": str,
-        "attributes": Sequence[AttributeTypeDef],
-        "platformDevices": Sequence[PlatformDeviceTypeDef],
-        "tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
+ResourceUnionTypeDef = Union[ResourceTypeDef, ResourceOutputTypeDef]
 _RequiredServiceConnectServiceOutputTypeDef = TypedDict(
     "_RequiredServiceConnectServiceOutputTypeDef",
     {
         "portName": str,
     },
 )
 _OptionalServiceConnectServiceOutputTypeDef = TypedDict(
@@ -2601,21 +2501,19 @@
         "discoveryName": str,
         "clientAliases": List[ServiceConnectClientAliasTypeDef],
         "ingressPortOverride": int,
     },
     total=False,
 )
 
-
 class ServiceConnectServiceOutputTypeDef(
     _RequiredServiceConnectServiceOutputTypeDef, _OptionalServiceConnectServiceOutputTypeDef
 ):
     pass
 
-
 _RequiredServiceConnectServiceTypeDef = TypedDict(
     "_RequiredServiceConnectServiceTypeDef",
     {
         "portName": str,
     },
 )
 _OptionalServiceConnectServiceTypeDef = TypedDict(
@@ -2624,21 +2522,20 @@
         "discoveryName": str,
         "clientAliases": Sequence[ServiceConnectClientAliasTypeDef],
         "ingressPortOverride": int,
     },
     total=False,
 )
 
-
 class ServiceConnectServiceTypeDef(
     _RequiredServiceConnectServiceTypeDef, _OptionalServiceConnectServiceTypeDef
 ):
     pass
 
-
+ProxyConfigurationUnionTypeDef = Union[ProxyConfigurationTypeDef, ProxyConfigurationOutputTypeDef]
 CapacityProviderTypeDef = TypedDict(
     "CapacityProviderTypeDef",
     {
         "capacityProviderArn": str,
         "name": str,
         "status": CapacityProviderStatusType,
         "autoScalingGroupProvider": AutoScalingGroupProviderTypeDef,
@@ -2660,22 +2557,20 @@
     "_OptionalCreateCapacityProviderRequestRequestTypeDef",
     {
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateCapacityProviderRequestRequestTypeDef(
     _RequiredCreateCapacityProviderRequestRequestTypeDef,
     _OptionalCreateCapacityProviderRequestRequestTypeDef,
 ):
     pass
 
-
 UpdateCapacityProviderRequestRequestTypeDef = TypedDict(
     "UpdateCapacityProviderRequestRequestTypeDef",
     {
         "name": str,
         "autoScalingGroupProvider": AutoScalingGroupProviderUpdateTypeDef,
     },
 )
@@ -2732,21 +2627,22 @@
         "scale": ScaleTypeDef,
         "clientToken": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateTaskSetRequestRequestTypeDef(
     _RequiredCreateTaskSetRequestRequestTypeDef, _OptionalCreateTaskSetRequestRequestTypeDef
 ):
     pass
 
-
+NetworkConfigurationUnionTypeDef = Union[
+    NetworkConfigurationTypeDef, NetworkConfigurationOutputTypeDef
+]
 TaskOverrideOutputTypeDef = TypedDict(
     "TaskOverrideOutputTypeDef",
     {
         "containerOverrides": List[ContainerOverrideOutputTypeDef],
         "cpu": str,
         "inferenceAcceleratorOverrides": List[InferenceAcceleratorOverrideTypeDef],
         "executionRoleArn": str,
@@ -2802,21 +2698,24 @@
         "cluster": str,
         "task": str,
         "status": str,
         "reason": str,
         "containers": Sequence[ContainerStateChangeTypeDef],
         "attachments": Sequence[AttachmentStateChangeTypeDef],
         "managedAgents": Sequence[ManagedAgentStateChangeTypeDef],
-        "pullStartedAt": Union[datetime, str],
-        "pullStoppedAt": Union[datetime, str],
-        "executionStoppedAt": Union[datetime, str],
+        "pullStartedAt": TimestampTypeDef,
+        "pullStoppedAt": TimestampTypeDef,
+        "executionStoppedAt": TimestampTypeDef,
     },
     total=False,
 )
 
+DeploymentConfigurationUnionTypeDef = Union[
+    DeploymentConfigurationTypeDef, DeploymentConfigurationOutputTypeDef
+]
 ClusterConfigurationTypeDef = TypedDict(
     "ClusterConfigurationTypeDef",
     {
         "executeCommandConfiguration": ExecuteCommandConfigurationTypeDef,
     },
     total=False,
 )
@@ -2935,14 +2834,30 @@
         "resourceRequirements": Sequence[ResourceRequirementTypeDef],
         "firelensConfiguration": FirelensConfigurationTypeDef,
         "credentialSpecs": Sequence[str],
     },
     total=False,
 )
 
+RegisterContainerInstanceRequestRequestTypeDef = TypedDict(
+    "RegisterContainerInstanceRequestRequestTypeDef",
+    {
+        "cluster": str,
+        "instanceIdentityDocument": str,
+        "instanceIdentityDocumentSignature": str,
+        "totalResources": Sequence[ResourceUnionTypeDef],
+        "versionInfo": VersionInfoTypeDef,
+        "containerInstanceArn": str,
+        "attributes": Sequence[AttributeTypeDef],
+        "platformDevices": Sequence[PlatformDeviceTypeDef],
+        "tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
 _RequiredServiceConnectConfigurationOutputTypeDef = TypedDict(
     "_RequiredServiceConnectConfigurationOutputTypeDef",
     {
         "enabled": bool,
     },
 )
 _OptionalServiceConnectConfigurationOutputTypeDef = TypedDict(
@@ -2951,22 +2866,20 @@
         "namespace": str,
         "services": List[ServiceConnectServiceOutputTypeDef],
         "logConfiguration": LogConfigurationOutputTypeDef,
     },
     total=False,
 )
 
-
 class ServiceConnectConfigurationOutputTypeDef(
     _RequiredServiceConnectConfigurationOutputTypeDef,
     _OptionalServiceConnectConfigurationOutputTypeDef,
 ):
     pass
 
-
 _RequiredServiceConnectConfigurationTypeDef = TypedDict(
     "_RequiredServiceConnectConfigurationTypeDef",
     {
         "enabled": bool,
     },
 )
 _OptionalServiceConnectConfigurationTypeDef = TypedDict(
@@ -2975,21 +2888,19 @@
         "namespace": str,
         "services": Sequence[ServiceConnectServiceTypeDef],
         "logConfiguration": LogConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class ServiceConnectConfigurationTypeDef(
     _RequiredServiceConnectConfigurationTypeDef, _OptionalServiceConnectConfigurationTypeDef
 ):
     pass
 
-
 CreateCapacityProviderResponseTypeDef = TypedDict(
     "CreateCapacityProviderResponseTypeDef",
     {
         "capacityProvider": CapacityProviderTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -3129,21 +3040,19 @@
         "referenceId": str,
         "startedBy": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class RunTaskRequestRequestTypeDef(
     _RequiredRunTaskRequestRequestTypeDef, _OptionalRunTaskRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredStartTaskRequestRequestTypeDef = TypedDict(
     "_RequiredStartTaskRequestRequestTypeDef",
     {
         "containerInstances": Sequence[str],
         "taskDefinition": str,
     },
 )
@@ -3160,21 +3069,20 @@
         "referenceId": str,
         "startedBy": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class StartTaskRequestRequestTypeDef(
     _RequiredStartTaskRequestRequestTypeDef, _OptionalStartTaskRequestRequestTypeDef
 ):
     pass
 
-
+TaskOverrideUnionTypeDef = Union[TaskOverrideTypeDef, TaskOverrideOutputTypeDef]
 DeregisterContainerInstanceResponseTypeDef = TypedDict(
     "DeregisterContainerInstanceResponseTypeDef",
     {
         "containerInstance": ContainerInstanceTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -3262,21 +3170,20 @@
         "settings": Sequence[ClusterSettingTypeDef],
         "configuration": ClusterConfigurationTypeDef,
         "serviceConnectDefaults": ClusterServiceConnectDefaultsRequestTypeDef,
     },
     total=False,
 )
 
-
 class UpdateClusterRequestRequestTypeDef(
     _RequiredUpdateClusterRequestRequestTypeDef, _OptionalUpdateClusterRequestRequestTypeDef
 ):
     pass
 
-
+VolumeUnionTypeDef = Union[VolumeTypeDef, VolumeOutputTypeDef]
 TaskDefinitionTypeDef = TypedDict(
     "TaskDefinitionTypeDef",
     {
         "taskDefinitionArn": str,
         "containerDefinitions": List[ContainerDefinitionOutputTypeDef],
         "family": str,
         "taskRoleArn": str,
@@ -3300,53 +3207,17 @@
         "deregisteredAt": datetime,
         "registeredBy": str,
         "ephemeralStorage": EphemeralStorageTypeDef,
     },
     total=False,
 )
 
-_RequiredRegisterTaskDefinitionRequestRequestTypeDef = TypedDict(
-    "_RequiredRegisterTaskDefinitionRequestRequestTypeDef",
-    {
-        "family": str,
-        "containerDefinitions": Sequence[
-            Union[ContainerDefinitionTypeDef, ContainerDefinitionOutputTypeDef]
-        ],
-    },
-)
-_OptionalRegisterTaskDefinitionRequestRequestTypeDef = TypedDict(
-    "_OptionalRegisterTaskDefinitionRequestRequestTypeDef",
-    {
-        "taskRoleArn": str,
-        "executionRoleArn": str,
-        "networkMode": NetworkModeType,
-        "volumes": Sequence[Union[VolumeTypeDef, VolumeOutputTypeDef]],
-        "placementConstraints": Sequence[TaskDefinitionPlacementConstraintTypeDef],
-        "requiresCompatibilities": Sequence[CompatibilityType],
-        "cpu": str,
-        "memory": str,
-        "tags": Sequence[TagTypeDef],
-        "pidMode": PidModeType,
-        "ipcMode": IpcModeType,
-        "proxyConfiguration": ProxyConfigurationTypeDef,
-        "inferenceAccelerators": Sequence[InferenceAcceleratorTypeDef],
-        "ephemeralStorage": EphemeralStorageTypeDef,
-        "runtimePlatform": RuntimePlatformTypeDef,
-    },
-    total=False,
-)
-
-
-class RegisterTaskDefinitionRequestRequestTypeDef(
-    _RequiredRegisterTaskDefinitionRequestRequestTypeDef,
-    _OptionalRegisterTaskDefinitionRequestRequestTypeDef,
-):
-    pass
-
-
+ContainerDefinitionUnionTypeDef = Union[
+    ContainerDefinitionTypeDef, ContainerDefinitionOutputTypeDef
+]
 DeploymentTypeDef = TypedDict(
     "DeploymentTypeDef",
     {
         "id": str,
         "status": str,
         "taskDefinition": str,
         "desiredCount": int,
@@ -3399,21 +3270,22 @@
         "propagateTags": PropagateTagsType,
         "enableExecuteCommand": bool,
         "serviceConnectConfiguration": ServiceConnectConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class CreateServiceRequestRequestTypeDef(
     _RequiredCreateServiceRequestRequestTypeDef, _OptionalCreateServiceRequestRequestTypeDef
 ):
     pass
 
-
+ServiceConnectConfigurationUnionTypeDef = Union[
+    ServiceConnectConfigurationTypeDef, ServiceConnectConfigurationOutputTypeDef
+]
 _RequiredUpdateServiceRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateServiceRequestRequestTypeDef",
     {
         "service": str,
     },
 )
 _OptionalUpdateServiceRequestRequestTypeDef = TypedDict(
@@ -3436,21 +3308,19 @@
         "propagateTags": PropagateTagsType,
         "serviceRegistries": Sequence[ServiceRegistryTypeDef],
         "serviceConnectConfiguration": ServiceConnectConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class UpdateServiceRequestRequestTypeDef(
     _RequiredUpdateServiceRequestRequestTypeDef, _OptionalUpdateServiceRequestRequestTypeDef
 ):
     pass
 
-
 DescribeTasksResponseTypeDef = TypedDict(
     "DescribeTasksResponseTypeDef",
     {
         "tasks": List[TaskTypeDef],
         "failures": List[FailureTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -3562,14 +3432,49 @@
     {
         "taskDefinition": TaskDefinitionTypeDef,
         "tags": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredRegisterTaskDefinitionRequestRequestTypeDef = TypedDict(
+    "_RequiredRegisterTaskDefinitionRequestRequestTypeDef",
+    {
+        "family": str,
+        "containerDefinitions": Sequence[ContainerDefinitionUnionTypeDef],
+    },
+)
+_OptionalRegisterTaskDefinitionRequestRequestTypeDef = TypedDict(
+    "_OptionalRegisterTaskDefinitionRequestRequestTypeDef",
+    {
+        "taskRoleArn": str,
+        "executionRoleArn": str,
+        "networkMode": NetworkModeType,
+        "volumes": Sequence[VolumeUnionTypeDef],
+        "placementConstraints": Sequence[TaskDefinitionPlacementConstraintTypeDef],
+        "requiresCompatibilities": Sequence[CompatibilityType],
+        "cpu": str,
+        "memory": str,
+        "tags": Sequence[TagTypeDef],
+        "pidMode": PidModeType,
+        "ipcMode": IpcModeType,
+        "proxyConfiguration": ProxyConfigurationTypeDef,
+        "inferenceAccelerators": Sequence[InferenceAcceleratorTypeDef],
+        "ephemeralStorage": EphemeralStorageTypeDef,
+        "runtimePlatform": RuntimePlatformTypeDef,
+    },
+    total=False,
+)
+
+class RegisterTaskDefinitionRequestRequestTypeDef(
+    _RequiredRegisterTaskDefinitionRequestRequestTypeDef,
+    _OptionalRegisterTaskDefinitionRequestRequestTypeDef,
+):
+    pass
+
 ServiceTypeDef = TypedDict(
     "ServiceTypeDef",
     {
         "serviceArn": str,
         "serviceName": str,
         "clusterArn": str,
         "loadBalancers": List[LoadBalancerTypeDef],
```

### Comparing `mypy-boto3-ecs-1.28.15.post1/mypy_boto3_ecs/type_defs.pyi` & `mypy-boto3-ecs-1.28.16/mypy_boto3_ecs/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_ecs.type_defs import AttachmentStateChangeTypeDef
 
-    data: AttachmentStateChangeTypeDef = {...}
+    data: AttachmentStateChangeTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -67,14 +67,15 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AttachmentStateChangeTypeDef",
     "KeyValuePairTypeDef",
     "AttributeTypeDef",
     "ManagedScalingTypeDef",
     "AwsVpcConfigurationOutputTypeDef",
     "AwsVpcConfigurationTypeDef",
@@ -164,20 +165,21 @@
     "ListTaskDefinitionFamiliesRequestRequestTypeDef",
     "ListTaskDefinitionsRequestRequestTypeDef",
     "ListTasksRequestRequestTypeDef",
     "ManagedAgentStateChangeTypeDef",
     "PlatformDeviceTypeDef",
     "PutAccountSettingDefaultRequestRequestTypeDef",
     "PutAccountSettingRequestRequestTypeDef",
-    "ResourceTypeDef",
     "RuntimePlatformTypeDef",
     "TaskDefinitionPlacementConstraintTypeDef",
+    "ResourceTypeDef",
     "ServiceConnectClientAliasTypeDef",
     "ServiceEventTypeDef",
     "StopTaskRequestRequestTypeDef",
+    "TimestampTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateContainerAgentRequestRequestTypeDef",
     "UpdateContainerInstancesStateRequestRequestTypeDef",
     "UpdateServicePrimaryTaskSetRequestRequestTypeDef",
     "UpdateTaskProtectionRequestRequestTypeDef",
     "SubmitAttachmentStateChangesRequestRequestTypeDef",
     "AttachmentTypeDef",
@@ -239,57 +241,64 @@
     "ListClustersRequestListClustersPaginateTypeDef",
     "ListContainerInstancesRequestListContainerInstancesPaginateTypeDef",
     "ListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef",
     "ListServicesRequestListServicesPaginateTypeDef",
     "ListTaskDefinitionFamiliesRequestListTaskDefinitionFamiliesPaginateTypeDef",
     "ListTaskDefinitionsRequestListTaskDefinitionsPaginateTypeDef",
     "ListTasksRequestListTasksPaginateTypeDef",
-    "RegisterContainerInstanceRequestRequestTypeDef",
+    "ResourceUnionTypeDef",
     "ServiceConnectServiceOutputTypeDef",
     "ServiceConnectServiceTypeDef",
+    "ProxyConfigurationUnionTypeDef",
     "CapacityProviderTypeDef",
     "CreateCapacityProviderRequestRequestTypeDef",
     "UpdateCapacityProviderRequestRequestTypeDef",
     "TaskSetTypeDef",
     "CreateTaskSetRequestRequestTypeDef",
+    "NetworkConfigurationUnionTypeDef",
     "TaskOverrideOutputTypeDef",
     "TaskOverrideTypeDef",
     "ContainerInstanceTypeDef",
     "SubmitTaskStateChangeRequestRequestTypeDef",
+    "DeploymentConfigurationUnionTypeDef",
     "ClusterConfigurationTypeDef",
     "VolumeOutputTypeDef",
     "VolumeTypeDef",
     "ContainerDefinitionOutputTypeDef",
     "ContainerDefinitionTypeDef",
+    "RegisterContainerInstanceRequestRequestTypeDef",
     "ServiceConnectConfigurationOutputTypeDef",
     "ServiceConnectConfigurationTypeDef",
     "CreateCapacityProviderResponseTypeDef",
     "DeleteCapacityProviderResponseTypeDef",
     "DescribeCapacityProvidersResponseTypeDef",
     "UpdateCapacityProviderResponseTypeDef",
     "CreateTaskSetResponseTypeDef",
     "DeleteTaskSetResponseTypeDef",
     "DescribeTaskSetsResponseTypeDef",
     "UpdateServicePrimaryTaskSetResponseTypeDef",
     "UpdateTaskSetResponseTypeDef",
     "TaskTypeDef",
     "RunTaskRequestRequestTypeDef",
     "StartTaskRequestRequestTypeDef",
+    "TaskOverrideUnionTypeDef",
     "DeregisterContainerInstanceResponseTypeDef",
     "DescribeContainerInstancesResponseTypeDef",
     "RegisterContainerInstanceResponseTypeDef",
     "UpdateContainerAgentResponseTypeDef",
     "UpdateContainerInstancesStateResponseTypeDef",
     "ClusterTypeDef",
     "CreateClusterRequestRequestTypeDef",
     "UpdateClusterRequestRequestTypeDef",
+    "VolumeUnionTypeDef",
     "TaskDefinitionTypeDef",
-    "RegisterTaskDefinitionRequestRequestTypeDef",
+    "ContainerDefinitionUnionTypeDef",
     "DeploymentTypeDef",
     "CreateServiceRequestRequestTypeDef",
+    "ServiceConnectConfigurationUnionTypeDef",
     "UpdateServiceRequestRequestTypeDef",
     "DescribeTasksResponseTypeDef",
     "RunTaskResponseTypeDef",
     "StartTaskResponseTypeDef",
     "StopTaskResponseTypeDef",
     "CreateClusterResponseTypeDef",
     "DeleteClusterResponseTypeDef",
@@ -297,14 +306,15 @@
     "PutClusterCapacityProvidersResponseTypeDef",
     "UpdateClusterResponseTypeDef",
     "UpdateClusterSettingsResponseTypeDef",
     "DeleteTaskDefinitionsResponseTypeDef",
     "DeregisterTaskDefinitionResponseTypeDef",
     "DescribeTaskDefinitionResponseTypeDef",
     "RegisterTaskDefinitionResponseTypeDef",
+    "RegisterTaskDefinitionRequestRequestTypeDef",
     "ServiceTypeDef",
     "CreateServiceResponseTypeDef",
     "DeleteServiceResponseTypeDef",
     "DescribeServicesResponseTypeDef",
     "UpdateServiceResponseTypeDef",
 )
 
@@ -337,17 +347,19 @@
         "value": str,
         "targetType": Literal["container-instance"],
         "targetId": str,
     },
     total=False,
 )
 
+
 class AttributeTypeDef(_RequiredAttributeTypeDef, _OptionalAttributeTypeDef):
     pass
 
+
 ManagedScalingTypeDef = TypedDict(
     "ManagedScalingTypeDef",
     {
         "status": ManagedScalingStatusType,
         "targetCapacity": int,
         "minimumScalingStepSize": int,
         "maximumScalingStepSize": int,
@@ -367,19 +379,21 @@
     {
         "securityGroups": List[str],
         "assignPublicIp": AssignPublicIpType,
     },
     total=False,
 )
 
+
 class AwsVpcConfigurationOutputTypeDef(
     _RequiredAwsVpcConfigurationOutputTypeDef, _OptionalAwsVpcConfigurationOutputTypeDef
 ):
     pass
 
+
 _RequiredAwsVpcConfigurationTypeDef = TypedDict(
     "_RequiredAwsVpcConfigurationTypeDef",
     {
         "subnets": Sequence[str],
     },
 )
 _OptionalAwsVpcConfigurationTypeDef = TypedDict(
@@ -387,19 +401,21 @@
     {
         "securityGroups": Sequence[str],
         "assignPublicIp": AssignPublicIpType,
     },
     total=False,
 )
 
+
 class AwsVpcConfigurationTypeDef(
     _RequiredAwsVpcConfigurationTypeDef, _OptionalAwsVpcConfigurationTypeDef
 ):
     pass
 
+
 _RequiredCapacityProviderStrategyItemTypeDef = TypedDict(
     "_RequiredCapacityProviderStrategyItemTypeDef",
     {
         "capacityProvider": str,
     },
 )
 _OptionalCapacityProviderStrategyItemTypeDef = TypedDict(
@@ -407,19 +423,21 @@
     {
         "weight": int,
         "base": int,
     },
     total=False,
 )
 
+
 class CapacityProviderStrategyItemTypeDef(
     _RequiredCapacityProviderStrategyItemTypeDef, _OptionalCapacityProviderStrategyItemTypeDef
 ):
     pass
 
+
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "key": str,
         "value": str,
     },
     total=False,
@@ -475,19 +493,21 @@
     "_OptionalFirelensConfigurationOutputTypeDef",
     {
         "options": Dict[str, str],
     },
     total=False,
 )
 
+
 class FirelensConfigurationOutputTypeDef(
     _RequiredFirelensConfigurationOutputTypeDef, _OptionalFirelensConfigurationOutputTypeDef
 ):
     pass
 
+
 _RequiredHealthCheckOutputTypeDef = TypedDict(
     "_RequiredHealthCheckOutputTypeDef",
     {
         "command": List[str],
     },
 )
 _OptionalHealthCheckOutputTypeDef = TypedDict(
@@ -497,19 +517,21 @@
         "timeout": int,
         "retries": int,
         "startPeriod": int,
     },
     total=False,
 )
 
+
 class HealthCheckOutputTypeDef(
     _RequiredHealthCheckOutputTypeDef, _OptionalHealthCheckOutputTypeDef
 ):
     pass
 
+
 HostEntryTypeDef = TypedDict(
     "HostEntryTypeDef",
     {
         "hostname": str,
         "ipAddress": str,
     },
 )
@@ -597,19 +619,21 @@
     "_OptionalFirelensConfigurationTypeDef",
     {
         "options": Mapping[str, str],
     },
     total=False,
 )
 
+
 class FirelensConfigurationTypeDef(
     _RequiredFirelensConfigurationTypeDef, _OptionalFirelensConfigurationTypeDef
 ):
     pass
 
+
 _RequiredHealthCheckTypeDef = TypedDict(
     "_RequiredHealthCheckTypeDef",
     {
         "command": Sequence[str],
     },
 )
 _OptionalHealthCheckTypeDef = TypedDict(
@@ -619,17 +643,19 @@
         "timeout": int,
         "retries": int,
         "startPeriod": int,
     },
     total=False,
 )
 
+
 class HealthCheckTypeDef(_RequiredHealthCheckTypeDef, _OptionalHealthCheckTypeDef):
     pass
 
+
 InstanceHealthCheckResultTypeDef = TypedDict(
     "InstanceHealthCheckResultTypeDef",
     {
         "type": Literal["CONTAINER_RUNTIME"],
         "status": InstanceHealthCheckStateType,
         "lastUpdated": datetime,
         "lastStatusChange": datetime,
@@ -771,20 +797,22 @@
     "_OptionalDeleteAccountSettingRequestRequestTypeDef",
     {
         "principalArn": str,
     },
     total=False,
 )
 
+
 class DeleteAccountSettingRequestRequestTypeDef(
     _RequiredDeleteAccountSettingRequestRequestTypeDef,
     _OptionalDeleteAccountSettingRequestRequestTypeDef,
 ):
     pass
 
+
 SettingTypeDef = TypedDict(
     "SettingTypeDef",
     {
         "name": SettingNameType,
         "value": str,
         "principalArn": str,
     },
@@ -816,19 +844,21 @@
     {
         "cluster": str,
         "force": bool,
     },
     total=False,
 )
 
+
 class DeleteServiceRequestRequestTypeDef(
     _RequiredDeleteServiceRequestRequestTypeDef, _OptionalDeleteServiceRequestRequestTypeDef
 ):
     pass
 
+
 DeleteTaskDefinitionsRequestRequestTypeDef = TypedDict(
     "DeleteTaskDefinitionsRequestRequestTypeDef",
     {
         "taskDefinitions": Sequence[str],
     },
 )
 
@@ -854,19 +884,21 @@
     "_OptionalDeleteTaskSetRequestRequestTypeDef",
     {
         "force": bool,
     },
     total=False,
 )
 
+
 class DeleteTaskSetRequestRequestTypeDef(
     _RequiredDeleteTaskSetRequestRequestTypeDef, _OptionalDeleteTaskSetRequestRequestTypeDef
 ):
     pass
 
+
 DeploymentAlarmsOutputTypeDef = TypedDict(
     "DeploymentAlarmsOutputTypeDef",
     {
         "alarmNames": List[str],
         "enable": bool,
         "rollback": bool,
     },
@@ -909,20 +941,22 @@
     {
         "cluster": str,
         "force": bool,
     },
     total=False,
 )
 
+
 class DeregisterContainerInstanceRequestRequestTypeDef(
     _RequiredDeregisterContainerInstanceRequestRequestTypeDef,
     _OptionalDeregisterContainerInstanceRequestRequestTypeDef,
 ):
     pass
 
+
 DeregisterTaskDefinitionRequestRequestTypeDef = TypedDict(
     "DeregisterTaskDefinitionRequestRequestTypeDef",
     {
         "taskDefinition": str,
     },
 )
 
@@ -957,20 +991,22 @@
     {
         "cluster": str,
         "include": Sequence[ContainerInstanceFieldType],
     },
     total=False,
 )
 
+
 class DescribeContainerInstancesRequestRequestTypeDef(
     _RequiredDescribeContainerInstancesRequestRequestTypeDef,
     _OptionalDescribeContainerInstancesRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDescribeServicesRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeServicesRequestRequestTypeDef",
     {
         "services": Sequence[str],
     },
 )
 _OptionalDescribeServicesRequestRequestTypeDef = TypedDict(
@@ -978,19 +1014,21 @@
     {
         "cluster": str,
         "include": Sequence[Literal["TAGS"]],
     },
     total=False,
 )
 
+
 class DescribeServicesRequestRequestTypeDef(
     _RequiredDescribeServicesRequestRequestTypeDef, _OptionalDescribeServicesRequestRequestTypeDef
 ):
     pass
 
+
 WaiterConfigTypeDef = TypedDict(
     "WaiterConfigTypeDef",
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
@@ -1006,20 +1044,22 @@
     "_OptionalDescribeTaskDefinitionRequestRequestTypeDef",
     {
         "include": Sequence[Literal["TAGS"]],
     },
     total=False,
 )
 
+
 class DescribeTaskDefinitionRequestRequestTypeDef(
     _RequiredDescribeTaskDefinitionRequestRequestTypeDef,
     _OptionalDescribeTaskDefinitionRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDescribeTaskSetsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeTaskSetsRequestRequestTypeDef",
     {
         "cluster": str,
         "service": str,
     },
 )
@@ -1028,19 +1068,21 @@
     {
         "taskSets": Sequence[str],
         "include": Sequence[Literal["TAGS"]],
     },
     total=False,
 )
 
+
 class DescribeTaskSetsRequestRequestTypeDef(
     _RequiredDescribeTaskSetsRequestRequestTypeDef, _OptionalDescribeTaskSetsRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredDescribeTasksRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeTasksRequestRequestTypeDef",
     {
         "tasks": Sequence[str],
     },
 )
 _OptionalDescribeTasksRequestRequestTypeDef = TypedDict(
@@ -1048,19 +1090,21 @@
     {
         "cluster": str,
         "include": Sequence[Literal["TAGS"]],
     },
     total=False,
 )
 
+
 class DescribeTasksRequestRequestTypeDef(
     _RequiredDescribeTasksRequestRequestTypeDef, _OptionalDescribeTasksRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredDeviceOutputTypeDef = TypedDict(
     "_RequiredDeviceOutputTypeDef",
     {
         "hostPath": str,
     },
 )
 _OptionalDeviceOutputTypeDef = TypedDict(
@@ -1068,17 +1112,19 @@
     {
         "containerPath": str,
         "permissions": List[DeviceCgroupPermissionType],
     },
     total=False,
 )
 
+
 class DeviceOutputTypeDef(_RequiredDeviceOutputTypeDef, _OptionalDeviceOutputTypeDef):
     pass
 
+
 _RequiredDeviceTypeDef = TypedDict(
     "_RequiredDeviceTypeDef",
     {
         "hostPath": str,
     },
 )
 _OptionalDeviceTypeDef = TypedDict(
@@ -1086,17 +1132,19 @@
     {
         "containerPath": str,
         "permissions": Sequence[DeviceCgroupPermissionType],
     },
     total=False,
 )
 
+
 class DeviceTypeDef(_RequiredDeviceTypeDef, _OptionalDeviceTypeDef):
     pass
 
+
 DiscoverPollEndpointRequestRequestTypeDef = TypedDict(
     "DiscoverPollEndpointRequestRequestTypeDef",
     {
         "containerInstance": str,
         "cluster": str,
     },
     total=False,
@@ -1167,19 +1215,21 @@
     {
         "cluster": str,
         "container": str,
     },
     total=False,
 )
 
+
 class ExecuteCommandRequestRequestTypeDef(
     _RequiredExecuteCommandRequestRequestTypeDef, _OptionalExecuteCommandRequestRequestTypeDef
 ):
     pass
 
+
 SessionTypeDef = TypedDict(
     "SessionTypeDef",
     {
         "sessionId": str,
         "streamUrl": str,
         "tokenValue": str,
     },
@@ -1204,19 +1254,21 @@
     "_OptionalGetTaskProtectionRequestRequestTypeDef",
     {
         "tasks": Sequence[str],
     },
     total=False,
 )
 
+
 class GetTaskProtectionRequestRequestTypeDef(
     _RequiredGetTaskProtectionRequestRequestTypeDef, _OptionalGetTaskProtectionRequestRequestTypeDef
 ):
     pass
 
+
 ProtectedTaskTypeDef = TypedDict(
     "ProtectedTaskTypeDef",
     {
         "taskArn": str,
         "protectionEnabled": bool,
         "expirationDate": datetime,
     },
@@ -1277,17 +1329,19 @@
     "_OptionalTmpfsOutputTypeDef",
     {
         "mountOptions": List[str],
     },
     total=False,
 )
 
+
 class TmpfsOutputTypeDef(_RequiredTmpfsOutputTypeDef, _OptionalTmpfsOutputTypeDef):
     pass
 
+
 _RequiredTmpfsTypeDef = TypedDict(
     "_RequiredTmpfsTypeDef",
     {
         "containerPath": str,
         "size": int,
     },
 )
@@ -1295,17 +1349,19 @@
     "_OptionalTmpfsTypeDef",
     {
         "mountOptions": Sequence[str],
     },
     total=False,
 )
 
+
 class TmpfsTypeDef(_RequiredTmpfsTypeDef, _OptionalTmpfsTypeDef):
     pass
 
+
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
@@ -1339,19 +1395,21 @@
         "attributeValue": str,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class ListAttributesRequestRequestTypeDef(
     _RequiredListAttributesRequestRequestTypeDef, _OptionalListAttributesRequestRequestTypeDef
 ):
     pass
 
+
 ListClustersRequestRequestTypeDef = TypedDict(
     "ListClustersRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
@@ -1380,20 +1438,22 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class ListServicesByNamespaceRequestRequestTypeDef(
     _RequiredListServicesByNamespaceRequestRequestTypeDef,
     _OptionalListServicesByNamespaceRequestRequestTypeDef,
 ):
     pass
 
+
 ListServicesRequestRequestTypeDef = TypedDict(
     "ListServicesRequestRequestTypeDef",
     {
         "cluster": str,
         "nextToken": str,
         "maxResults": int,
         "launchType": LaunchTypeType,
@@ -1460,19 +1520,21 @@
     "_OptionalManagedAgentStateChangeTypeDef",
     {
         "reason": str,
     },
     total=False,
 )
 
+
 class ManagedAgentStateChangeTypeDef(
     _RequiredManagedAgentStateChangeTypeDef, _OptionalManagedAgentStateChangeTypeDef
 ):
     pass
 
+
 PlatformDeviceTypeDef = TypedDict(
     "PlatformDeviceTypeDef",
     {
         "id": str,
         "type": Literal["GPU"],
     },
 )
@@ -1496,31 +1558,20 @@
     "_OptionalPutAccountSettingRequestRequestTypeDef",
     {
         "principalArn": str,
     },
     total=False,
 )
 
+
 class PutAccountSettingRequestRequestTypeDef(
     _RequiredPutAccountSettingRequestRequestTypeDef, _OptionalPutAccountSettingRequestRequestTypeDef
 ):
     pass
 
-ResourceTypeDef = TypedDict(
-    "ResourceTypeDef",
-    {
-        "name": str,
-        "type": str,
-        "doubleValue": float,
-        "longValue": int,
-        "integerValue": int,
-        "stringSetValue": Sequence[str],
-    },
-    total=False,
-)
 
 RuntimePlatformTypeDef = TypedDict(
     "RuntimePlatformTypeDef",
     {
         "cpuArchitecture": CPUArchitectureType,
         "operatingSystemFamily": OSFamilyType,
     },
@@ -1532,33 +1583,48 @@
     {
         "type": Literal["memberOf"],
         "expression": str,
     },
     total=False,
 )
 
+ResourceTypeDef = TypedDict(
+    "ResourceTypeDef",
+    {
+        "name": str,
+        "type": str,
+        "doubleValue": float,
+        "longValue": int,
+        "integerValue": int,
+        "stringSetValue": Sequence[str],
+    },
+    total=False,
+)
+
 _RequiredServiceConnectClientAliasTypeDef = TypedDict(
     "_RequiredServiceConnectClientAliasTypeDef",
     {
         "port": int,
     },
 )
 _OptionalServiceConnectClientAliasTypeDef = TypedDict(
     "_OptionalServiceConnectClientAliasTypeDef",
     {
         "dnsName": str,
     },
     total=False,
 )
 
+
 class ServiceConnectClientAliasTypeDef(
     _RequiredServiceConnectClientAliasTypeDef, _OptionalServiceConnectClientAliasTypeDef
 ):
     pass
 
+
 ServiceEventTypeDef = TypedDict(
     "ServiceEventTypeDef",
     {
         "id": str,
         "createdAt": datetime,
         "message": str,
     },
@@ -1576,19 +1642,22 @@
     {
         "cluster": str,
         "reason": str,
     },
     total=False,
 )
 
+
 class StopTaskRequestRequestTypeDef(
     _RequiredStopTaskRequestRequestTypeDef, _OptionalStopTaskRequestRequestTypeDef
 ):
     pass
 
+
+TimestampTypeDef = Union[datetime, str]
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
@@ -1603,20 +1672,22 @@
     "_OptionalUpdateContainerAgentRequestRequestTypeDef",
     {
         "cluster": str,
     },
     total=False,
 )
 
+
 class UpdateContainerAgentRequestRequestTypeDef(
     _RequiredUpdateContainerAgentRequestRequestTypeDef,
     _OptionalUpdateContainerAgentRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateContainerInstancesStateRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateContainerInstancesStateRequestRequestTypeDef",
     {
         "containerInstances": Sequence[str],
         "status": ContainerInstanceStatusType,
     },
 )
@@ -1624,20 +1695,22 @@
     "_OptionalUpdateContainerInstancesStateRequestRequestTypeDef",
     {
         "cluster": str,
     },
     total=False,
 )
 
+
 class UpdateContainerInstancesStateRequestRequestTypeDef(
     _RequiredUpdateContainerInstancesStateRequestRequestTypeDef,
     _OptionalUpdateContainerInstancesStateRequestRequestTypeDef,
 ):
     pass
 
+
 UpdateServicePrimaryTaskSetRequestRequestTypeDef = TypedDict(
     "UpdateServicePrimaryTaskSetRequestRequestTypeDef",
     {
         "cluster": str,
         "service": str,
         "primaryTaskSet": str,
     },
@@ -1655,40 +1728,44 @@
     "_OptionalUpdateTaskProtectionRequestRequestTypeDef",
     {
         "expiresInMinutes": int,
     },
     total=False,
 )
 
+
 class UpdateTaskProtectionRequestRequestTypeDef(
     _RequiredUpdateTaskProtectionRequestRequestTypeDef,
     _OptionalUpdateTaskProtectionRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredSubmitAttachmentStateChangesRequestRequestTypeDef = TypedDict(
     "_RequiredSubmitAttachmentStateChangesRequestRequestTypeDef",
     {
         "attachments": Sequence[AttachmentStateChangeTypeDef],
     },
 )
 _OptionalSubmitAttachmentStateChangesRequestRequestTypeDef = TypedDict(
     "_OptionalSubmitAttachmentStateChangesRequestRequestTypeDef",
     {
         "cluster": str,
     },
     total=False,
 )
 
+
 class SubmitAttachmentStateChangesRequestRequestTypeDef(
     _RequiredSubmitAttachmentStateChangesRequestRequestTypeDef,
     _OptionalSubmitAttachmentStateChangesRequestRequestTypeDef,
 ):
     pass
 
+
 AttachmentTypeDef = TypedDict(
     "AttachmentTypeDef",
     {
         "id": str,
         "type": str,
         "status": str,
         "details": List[KeyValuePairTypeDef],
@@ -1707,19 +1784,21 @@
     {
         "type": Literal["APPMESH"],
         "properties": List[KeyValuePairTypeDef],
     },
     total=False,
 )
 
+
 class ProxyConfigurationOutputTypeDef(
     _RequiredProxyConfigurationOutputTypeDef, _OptionalProxyConfigurationOutputTypeDef
 ):
     pass
 
+
 _RequiredProxyConfigurationTypeDef = TypedDict(
     "_RequiredProxyConfigurationTypeDef",
     {
         "containerName": str,
     },
 )
 _OptionalProxyConfigurationTypeDef = TypedDict(
@@ -1727,57 +1806,63 @@
     {
         "type": Literal["APPMESH"],
         "properties": Sequence[KeyValuePairTypeDef],
     },
     total=False,
 )
 
+
 class ProxyConfigurationTypeDef(
     _RequiredProxyConfigurationTypeDef, _OptionalProxyConfigurationTypeDef
 ):
     pass
 
+
 _RequiredDeleteAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteAttributesRequestRequestTypeDef",
     {
         "attributes": Sequence[AttributeTypeDef],
     },
 )
 _OptionalDeleteAttributesRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteAttributesRequestRequestTypeDef",
     {
         "cluster": str,
     },
     total=False,
 )
 
+
 class DeleteAttributesRequestRequestTypeDef(
     _RequiredDeleteAttributesRequestRequestTypeDef, _OptionalDeleteAttributesRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredPutAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredPutAttributesRequestRequestTypeDef",
     {
         "attributes": Sequence[AttributeTypeDef],
     },
 )
 _OptionalPutAttributesRequestRequestTypeDef = TypedDict(
     "_OptionalPutAttributesRequestRequestTypeDef",
     {
         "cluster": str,
     },
     total=False,
 )
 
+
 class PutAttributesRequestRequestTypeDef(
     _RequiredPutAttributesRequestRequestTypeDef, _OptionalPutAttributesRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredAutoScalingGroupProviderTypeDef = TypedDict(
     "_RequiredAutoScalingGroupProviderTypeDef",
     {
         "autoScalingGroupArn": str,
     },
 )
 _OptionalAutoScalingGroupProviderTypeDef = TypedDict(
@@ -1785,19 +1870,21 @@
     {
         "managedScaling": ManagedScalingTypeDef,
         "managedTerminationProtection": ManagedTerminationProtectionType,
     },
     total=False,
 )
 
+
 class AutoScalingGroupProviderTypeDef(
     _RequiredAutoScalingGroupProviderTypeDef, _OptionalAutoScalingGroupProviderTypeDef
 ):
     pass
 
+
 AutoScalingGroupProviderUpdateTypeDef = TypedDict(
     "AutoScalingGroupProviderUpdateTypeDef",
     {
         "managedScaling": ManagedScalingTypeDef,
         "managedTerminationProtection": ManagedTerminationProtectionType,
     },
     total=False,
@@ -1885,19 +1972,21 @@
     {
         "options": Dict[str, str],
         "secretOptions": List[SecretTypeDef],
     },
     total=False,
 )
 
+
 class LogConfigurationOutputTypeDef(
     _RequiredLogConfigurationOutputTypeDef, _OptionalLogConfigurationOutputTypeDef
 ):
     pass
 
+
 _RequiredLogConfigurationTypeDef = TypedDict(
     "_RequiredLogConfigurationTypeDef",
     {
         "logDriver": LogDriverType,
     },
 )
 _OptionalLogConfigurationTypeDef = TypedDict(
@@ -1905,17 +1994,19 @@
     {
         "options": Mapping[str, str],
         "secretOptions": Sequence[SecretTypeDef],
     },
     total=False,
 )
 
+
 class LogConfigurationTypeDef(_RequiredLogConfigurationTypeDef, _OptionalLogConfigurationTypeDef):
     pass
 
+
 ContainerInstanceHealthStatusTypeDef = TypedDict(
     "ContainerInstanceHealthStatusTypeDef",
     {
         "overallStatus": InstanceHealthCheckStateType,
         "details": List[InstanceHealthCheckResultTypeDef],
     },
     total=False,
@@ -2181,20 +2272,22 @@
         "cluster": str,
         "include": Sequence[Literal["TAGS"]],
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeServicesRequestServicesInactiveWaitTypeDef(
     _RequiredDescribeServicesRequestServicesInactiveWaitTypeDef,
     _OptionalDescribeServicesRequestServicesInactiveWaitTypeDef,
 ):
     pass
 
+
 _RequiredDescribeServicesRequestServicesStableWaitTypeDef = TypedDict(
     "_RequiredDescribeServicesRequestServicesStableWaitTypeDef",
     {
         "services": Sequence[str],
     },
 )
 _OptionalDescribeServicesRequestServicesStableWaitTypeDef = TypedDict(
@@ -2203,20 +2296,22 @@
         "cluster": str,
         "include": Sequence[Literal["TAGS"]],
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeServicesRequestServicesStableWaitTypeDef(
     _RequiredDescribeServicesRequestServicesStableWaitTypeDef,
     _OptionalDescribeServicesRequestServicesStableWaitTypeDef,
 ):
     pass
 
+
 _RequiredDescribeTasksRequestTasksRunningWaitTypeDef = TypedDict(
     "_RequiredDescribeTasksRequestTasksRunningWaitTypeDef",
     {
         "tasks": Sequence[str],
     },
 )
 _OptionalDescribeTasksRequestTasksRunningWaitTypeDef = TypedDict(
@@ -2225,20 +2320,22 @@
         "cluster": str,
         "include": Sequence[Literal["TAGS"]],
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeTasksRequestTasksRunningWaitTypeDef(
     _RequiredDescribeTasksRequestTasksRunningWaitTypeDef,
     _OptionalDescribeTasksRequestTasksRunningWaitTypeDef,
 ):
     pass
 
+
 _RequiredDescribeTasksRequestTasksStoppedWaitTypeDef = TypedDict(
     "_RequiredDescribeTasksRequestTasksStoppedWaitTypeDef",
     {
         "tasks": Sequence[str],
     },
 )
 _OptionalDescribeTasksRequestTasksStoppedWaitTypeDef = TypedDict(
@@ -2247,20 +2344,22 @@
         "cluster": str,
         "include": Sequence[Literal["TAGS"]],
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeTasksRequestTasksStoppedWaitTypeDef(
     _RequiredDescribeTasksRequestTasksStoppedWaitTypeDef,
     _OptionalDescribeTasksRequestTasksStoppedWaitTypeDef,
 ):
     pass
 
+
 _RequiredEFSVolumeConfigurationTypeDef = TypedDict(
     "_RequiredEFSVolumeConfigurationTypeDef",
     {
         "fileSystemId": str,
     },
 )
 _OptionalEFSVolumeConfigurationTypeDef = TypedDict(
@@ -2270,19 +2369,21 @@
         "transitEncryption": EFSTransitEncryptionType,
         "transitEncryptionPort": int,
         "authorizationConfig": EFSAuthorizationConfigTypeDef,
     },
     total=False,
 )
 
+
 class EFSVolumeConfigurationTypeDef(
     _RequiredEFSVolumeConfigurationTypeDef, _OptionalEFSVolumeConfigurationTypeDef
 ):
     pass
 
+
 ExecuteCommandConfigurationTypeDef = TypedDict(
     "ExecuteCommandConfigurationTypeDef",
     {
         "kmsKeyId": str,
         "logging": ExecuteCommandLoggingType,
         "logConfiguration": ExecuteCommandLogConfigurationTypeDef,
     },
@@ -2382,20 +2483,22 @@
         "attributeName": str,
         "attributeValue": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListAttributesRequestListAttributesPaginateTypeDef(
     _RequiredListAttributesRequestListAttributesPaginateTypeDef,
     _OptionalListAttributesRequestListAttributesPaginateTypeDef,
 ):
     pass
 
+
 ListClustersRequestListClustersPaginateTypeDef = TypedDict(
     "ListClustersRequestListClustersPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -2421,20 +2524,22 @@
     "_OptionalListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef(
     _RequiredListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef,
     _OptionalListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef,
 ):
     pass
 
+
 ListServicesRequestListServicesPaginateTypeDef = TypedDict(
     "ListServicesRequestListServicesPaginateTypeDef",
     {
         "cluster": str,
         "launchType": LaunchTypeType,
         "schedulingStrategy": SchedulingStrategyType,
         "PaginationConfig": PaginatorConfigTypeDef,
@@ -2474,30 +2579,15 @@
         "desiredStatus": DesiredStatusType,
         "launchType": LaunchTypeType,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-RegisterContainerInstanceRequestRequestTypeDef = TypedDict(
-    "RegisterContainerInstanceRequestRequestTypeDef",
-    {
-        "cluster": str,
-        "instanceIdentityDocument": str,
-        "instanceIdentityDocumentSignature": str,
-        "totalResources": Sequence[Union[ResourceTypeDef, ResourceOutputTypeDef]],
-        "versionInfo": VersionInfoTypeDef,
-        "containerInstanceArn": str,
-        "attributes": Sequence[AttributeTypeDef],
-        "platformDevices": Sequence[PlatformDeviceTypeDef],
-        "tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
+ResourceUnionTypeDef = Union[ResourceTypeDef, ResourceOutputTypeDef]
 _RequiredServiceConnectServiceOutputTypeDef = TypedDict(
     "_RequiredServiceConnectServiceOutputTypeDef",
     {
         "portName": str,
     },
 )
 _OptionalServiceConnectServiceOutputTypeDef = TypedDict(
@@ -2506,19 +2596,21 @@
         "discoveryName": str,
         "clientAliases": List[ServiceConnectClientAliasTypeDef],
         "ingressPortOverride": int,
     },
     total=False,
 )
 
+
 class ServiceConnectServiceOutputTypeDef(
     _RequiredServiceConnectServiceOutputTypeDef, _OptionalServiceConnectServiceOutputTypeDef
 ):
     pass
 
+
 _RequiredServiceConnectServiceTypeDef = TypedDict(
     "_RequiredServiceConnectServiceTypeDef",
     {
         "portName": str,
     },
 )
 _OptionalServiceConnectServiceTypeDef = TypedDict(
@@ -2527,19 +2619,22 @@
         "discoveryName": str,
         "clientAliases": Sequence[ServiceConnectClientAliasTypeDef],
         "ingressPortOverride": int,
     },
     total=False,
 )
 
+
 class ServiceConnectServiceTypeDef(
     _RequiredServiceConnectServiceTypeDef, _OptionalServiceConnectServiceTypeDef
 ):
     pass
 
+
+ProxyConfigurationUnionTypeDef = Union[ProxyConfigurationTypeDef, ProxyConfigurationOutputTypeDef]
 CapacityProviderTypeDef = TypedDict(
     "CapacityProviderTypeDef",
     {
         "capacityProviderArn": str,
         "name": str,
         "status": CapacityProviderStatusType,
         "autoScalingGroupProvider": AutoScalingGroupProviderTypeDef,
@@ -2561,20 +2656,22 @@
     "_OptionalCreateCapacityProviderRequestRequestTypeDef",
     {
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateCapacityProviderRequestRequestTypeDef(
     _RequiredCreateCapacityProviderRequestRequestTypeDef,
     _OptionalCreateCapacityProviderRequestRequestTypeDef,
 ):
     pass
 
+
 UpdateCapacityProviderRequestRequestTypeDef = TypedDict(
     "UpdateCapacityProviderRequestRequestTypeDef",
     {
         "name": str,
         "autoScalingGroupProvider": AutoScalingGroupProviderUpdateTypeDef,
     },
 )
@@ -2631,19 +2728,24 @@
         "scale": ScaleTypeDef,
         "clientToken": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateTaskSetRequestRequestTypeDef(
     _RequiredCreateTaskSetRequestRequestTypeDef, _OptionalCreateTaskSetRequestRequestTypeDef
 ):
     pass
 
+
+NetworkConfigurationUnionTypeDef = Union[
+    NetworkConfigurationTypeDef, NetworkConfigurationOutputTypeDef
+]
 TaskOverrideOutputTypeDef = TypedDict(
     "TaskOverrideOutputTypeDef",
     {
         "containerOverrides": List[ContainerOverrideOutputTypeDef],
         "cpu": str,
         "inferenceAcceleratorOverrides": List[InferenceAcceleratorOverrideTypeDef],
         "executionRoleArn": str,
@@ -2699,21 +2801,24 @@
         "cluster": str,
         "task": str,
         "status": str,
         "reason": str,
         "containers": Sequence[ContainerStateChangeTypeDef],
         "attachments": Sequence[AttachmentStateChangeTypeDef],
         "managedAgents": Sequence[ManagedAgentStateChangeTypeDef],
-        "pullStartedAt": Union[datetime, str],
-        "pullStoppedAt": Union[datetime, str],
-        "executionStoppedAt": Union[datetime, str],
+        "pullStartedAt": TimestampTypeDef,
+        "pullStoppedAt": TimestampTypeDef,
+        "executionStoppedAt": TimestampTypeDef,
     },
     total=False,
 )
 
+DeploymentConfigurationUnionTypeDef = Union[
+    DeploymentConfigurationTypeDef, DeploymentConfigurationOutputTypeDef
+]
 ClusterConfigurationTypeDef = TypedDict(
     "ClusterConfigurationTypeDef",
     {
         "executeCommandConfiguration": ExecuteCommandConfigurationTypeDef,
     },
     total=False,
 )
@@ -2832,14 +2937,30 @@
         "resourceRequirements": Sequence[ResourceRequirementTypeDef],
         "firelensConfiguration": FirelensConfigurationTypeDef,
         "credentialSpecs": Sequence[str],
     },
     total=False,
 )
 
+RegisterContainerInstanceRequestRequestTypeDef = TypedDict(
+    "RegisterContainerInstanceRequestRequestTypeDef",
+    {
+        "cluster": str,
+        "instanceIdentityDocument": str,
+        "instanceIdentityDocumentSignature": str,
+        "totalResources": Sequence[ResourceUnionTypeDef],
+        "versionInfo": VersionInfoTypeDef,
+        "containerInstanceArn": str,
+        "attributes": Sequence[AttributeTypeDef],
+        "platformDevices": Sequence[PlatformDeviceTypeDef],
+        "tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
 _RequiredServiceConnectConfigurationOutputTypeDef = TypedDict(
     "_RequiredServiceConnectConfigurationOutputTypeDef",
     {
         "enabled": bool,
     },
 )
 _OptionalServiceConnectConfigurationOutputTypeDef = TypedDict(
@@ -2848,20 +2969,22 @@
         "namespace": str,
         "services": List[ServiceConnectServiceOutputTypeDef],
         "logConfiguration": LogConfigurationOutputTypeDef,
     },
     total=False,
 )
 
+
 class ServiceConnectConfigurationOutputTypeDef(
     _RequiredServiceConnectConfigurationOutputTypeDef,
     _OptionalServiceConnectConfigurationOutputTypeDef,
 ):
     pass
 
+
 _RequiredServiceConnectConfigurationTypeDef = TypedDict(
     "_RequiredServiceConnectConfigurationTypeDef",
     {
         "enabled": bool,
     },
 )
 _OptionalServiceConnectConfigurationTypeDef = TypedDict(
@@ -2870,19 +2993,21 @@
         "namespace": str,
         "services": Sequence[ServiceConnectServiceTypeDef],
         "logConfiguration": LogConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class ServiceConnectConfigurationTypeDef(
     _RequiredServiceConnectConfigurationTypeDef, _OptionalServiceConnectConfigurationTypeDef
 ):
     pass
 
+
 CreateCapacityProviderResponseTypeDef = TypedDict(
     "CreateCapacityProviderResponseTypeDef",
     {
         "capacityProvider": CapacityProviderTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -3022,19 +3147,21 @@
         "referenceId": str,
         "startedBy": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class RunTaskRequestRequestTypeDef(
     _RequiredRunTaskRequestRequestTypeDef, _OptionalRunTaskRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredStartTaskRequestRequestTypeDef = TypedDict(
     "_RequiredStartTaskRequestRequestTypeDef",
     {
         "containerInstances": Sequence[str],
         "taskDefinition": str,
     },
 )
@@ -3051,19 +3178,22 @@
         "referenceId": str,
         "startedBy": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class StartTaskRequestRequestTypeDef(
     _RequiredStartTaskRequestRequestTypeDef, _OptionalStartTaskRequestRequestTypeDef
 ):
     pass
 
+
+TaskOverrideUnionTypeDef = Union[TaskOverrideTypeDef, TaskOverrideOutputTypeDef]
 DeregisterContainerInstanceResponseTypeDef = TypedDict(
     "DeregisterContainerInstanceResponseTypeDef",
     {
         "containerInstance": ContainerInstanceTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -3151,19 +3281,22 @@
         "settings": Sequence[ClusterSettingTypeDef],
         "configuration": ClusterConfigurationTypeDef,
         "serviceConnectDefaults": ClusterServiceConnectDefaultsRequestTypeDef,
     },
     total=False,
 )
 
+
 class UpdateClusterRequestRequestTypeDef(
     _RequiredUpdateClusterRequestRequestTypeDef, _OptionalUpdateClusterRequestRequestTypeDef
 ):
     pass
 
+
+VolumeUnionTypeDef = Union[VolumeTypeDef, VolumeOutputTypeDef]
 TaskDefinitionTypeDef = TypedDict(
     "TaskDefinitionTypeDef",
     {
         "taskDefinitionArn": str,
         "containerDefinitions": List[ContainerDefinitionOutputTypeDef],
         "family": str,
         "taskRoleArn": str,
@@ -3187,51 +3320,17 @@
         "deregisteredAt": datetime,
         "registeredBy": str,
         "ephemeralStorage": EphemeralStorageTypeDef,
     },
     total=False,
 )
 
-_RequiredRegisterTaskDefinitionRequestRequestTypeDef = TypedDict(
-    "_RequiredRegisterTaskDefinitionRequestRequestTypeDef",
-    {
-        "family": str,
-        "containerDefinitions": Sequence[
-            Union[ContainerDefinitionTypeDef, ContainerDefinitionOutputTypeDef]
-        ],
-    },
-)
-_OptionalRegisterTaskDefinitionRequestRequestTypeDef = TypedDict(
-    "_OptionalRegisterTaskDefinitionRequestRequestTypeDef",
-    {
-        "taskRoleArn": str,
-        "executionRoleArn": str,
-        "networkMode": NetworkModeType,
-        "volumes": Sequence[Union[VolumeTypeDef, VolumeOutputTypeDef]],
-        "placementConstraints": Sequence[TaskDefinitionPlacementConstraintTypeDef],
-        "requiresCompatibilities": Sequence[CompatibilityType],
-        "cpu": str,
-        "memory": str,
-        "tags": Sequence[TagTypeDef],
-        "pidMode": PidModeType,
-        "ipcMode": IpcModeType,
-        "proxyConfiguration": ProxyConfigurationTypeDef,
-        "inferenceAccelerators": Sequence[InferenceAcceleratorTypeDef],
-        "ephemeralStorage": EphemeralStorageTypeDef,
-        "runtimePlatform": RuntimePlatformTypeDef,
-    },
-    total=False,
-)
-
-class RegisterTaskDefinitionRequestRequestTypeDef(
-    _RequiredRegisterTaskDefinitionRequestRequestTypeDef,
-    _OptionalRegisterTaskDefinitionRequestRequestTypeDef,
-):
-    pass
-
+ContainerDefinitionUnionTypeDef = Union[
+    ContainerDefinitionTypeDef, ContainerDefinitionOutputTypeDef
+]
 DeploymentTypeDef = TypedDict(
     "DeploymentTypeDef",
     {
         "id": str,
         "status": str,
         "taskDefinition": str,
         "desiredCount": int,
@@ -3284,19 +3383,24 @@
         "propagateTags": PropagateTagsType,
         "enableExecuteCommand": bool,
         "serviceConnectConfiguration": ServiceConnectConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class CreateServiceRequestRequestTypeDef(
     _RequiredCreateServiceRequestRequestTypeDef, _OptionalCreateServiceRequestRequestTypeDef
 ):
     pass
 
+
+ServiceConnectConfigurationUnionTypeDef = Union[
+    ServiceConnectConfigurationTypeDef, ServiceConnectConfigurationOutputTypeDef
+]
 _RequiredUpdateServiceRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateServiceRequestRequestTypeDef",
     {
         "service": str,
     },
 )
 _OptionalUpdateServiceRequestRequestTypeDef = TypedDict(
@@ -3319,19 +3423,21 @@
         "propagateTags": PropagateTagsType,
         "serviceRegistries": Sequence[ServiceRegistryTypeDef],
         "serviceConnectConfiguration": ServiceConnectConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class UpdateServiceRequestRequestTypeDef(
     _RequiredUpdateServiceRequestRequestTypeDef, _OptionalUpdateServiceRequestRequestTypeDef
 ):
     pass
 
+
 DescribeTasksResponseTypeDef = TypedDict(
     "DescribeTasksResponseTypeDef",
     {
         "tasks": List[TaskTypeDef],
         "failures": List[FailureTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -3443,14 +3549,51 @@
     {
         "taskDefinition": TaskDefinitionTypeDef,
         "tags": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredRegisterTaskDefinitionRequestRequestTypeDef = TypedDict(
+    "_RequiredRegisterTaskDefinitionRequestRequestTypeDef",
+    {
+        "family": str,
+        "containerDefinitions": Sequence[ContainerDefinitionUnionTypeDef],
+    },
+)
+_OptionalRegisterTaskDefinitionRequestRequestTypeDef = TypedDict(
+    "_OptionalRegisterTaskDefinitionRequestRequestTypeDef",
+    {
+        "taskRoleArn": str,
+        "executionRoleArn": str,
+        "networkMode": NetworkModeType,
+        "volumes": Sequence[VolumeUnionTypeDef],
+        "placementConstraints": Sequence[TaskDefinitionPlacementConstraintTypeDef],
+        "requiresCompatibilities": Sequence[CompatibilityType],
+        "cpu": str,
+        "memory": str,
+        "tags": Sequence[TagTypeDef],
+        "pidMode": PidModeType,
+        "ipcMode": IpcModeType,
+        "proxyConfiguration": ProxyConfigurationTypeDef,
+        "inferenceAccelerators": Sequence[InferenceAcceleratorTypeDef],
+        "ephemeralStorage": EphemeralStorageTypeDef,
+        "runtimePlatform": RuntimePlatformTypeDef,
+    },
+    total=False,
+)
+
+
+class RegisterTaskDefinitionRequestRequestTypeDef(
+    _RequiredRegisterTaskDefinitionRequestRequestTypeDef,
+    _OptionalRegisterTaskDefinitionRequestRequestTypeDef,
+):
+    pass
+
+
 ServiceTypeDef = TypedDict(
     "ServiceTypeDef",
     {
         "serviceArn": str,
         "serviceName": str,
         "clusterArn": str,
         "loadBalancers": List[LoadBalancerTypeDef],
```

### Comparing `mypy-boto3-ecs-1.28.15.post1/mypy_boto3_ecs/waiter.py` & `mypy-boto3-ecs-1.28.16/mypy_boto3_ecs/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecs-1.28.15.post1/mypy_boto3_ecs/waiter.pyi` & `mypy-boto3-ecs-1.28.16/mypy_boto3_ecs/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecs-1.28.15.post1/mypy_boto3_ecs.egg-info/PKG-INFO` & `mypy-boto3-ecs-1.28.16/mypy_boto3_ecs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ecs
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.ECS 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.ECS 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 ecs type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 ecs type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ecs.svg?color=blue)](https://pypi.org/project/mypy-boto3-ecs)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ecs)](https://pepy.tech/project/mypy-boto3-ecs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ECS 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS)
+[boto3.ECS 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS)
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
 [mypy-boto3-ecs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/).
 
 See how it helps to find and fix potential bugs:
 
@@ -75,15 +75,15 @@
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Waiters annotations](#waiters-annotations)
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
@@ -435,20 +435,20 @@
 )
 
 
 def check_value(value: AgentUpdateStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_ecs.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_ecs.type_defs import (
     AttachmentStateChangeTypeDef,
     KeyValuePairTypeDef,
     AttributeTypeDef,
     ManagedScalingTypeDef,
@@ -540,20 +540,21 @@
     ListTaskDefinitionFamiliesRequestRequestTypeDef,
     ListTaskDefinitionsRequestRequestTypeDef,
     ListTasksRequestRequestTypeDef,
     ManagedAgentStateChangeTypeDef,
     PlatformDeviceTypeDef,
     PutAccountSettingDefaultRequestRequestTypeDef,
     PutAccountSettingRequestRequestTypeDef,
-    ResourceTypeDef,
     RuntimePlatformTypeDef,
     TaskDefinitionPlacementConstraintTypeDef,
+    ResourceTypeDef,
     ServiceConnectClientAliasTypeDef,
     ServiceEventTypeDef,
     StopTaskRequestRequestTypeDef,
+    TimestampTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateContainerAgentRequestRequestTypeDef,
     UpdateContainerInstancesStateRequestRequestTypeDef,
     UpdateServicePrimaryTaskSetRequestRequestTypeDef,
     UpdateTaskProtectionRequestRequestTypeDef,
     SubmitAttachmentStateChangesRequestRequestTypeDef,
     AttachmentTypeDef,
@@ -615,57 +616,64 @@
     ListClustersRequestListClustersPaginateTypeDef,
     ListContainerInstancesRequestListContainerInstancesPaginateTypeDef,
     ListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef,
     ListServicesRequestListServicesPaginateTypeDef,
     ListTaskDefinitionFamiliesRequestListTaskDefinitionFamiliesPaginateTypeDef,
     ListTaskDefinitionsRequestListTaskDefinitionsPaginateTypeDef,
     ListTasksRequestListTasksPaginateTypeDef,
-    RegisterContainerInstanceRequestRequestTypeDef,
+    ResourceUnionTypeDef,
     ServiceConnectServiceOutputTypeDef,
     ServiceConnectServiceTypeDef,
+    ProxyConfigurationUnionTypeDef,
     CapacityProviderTypeDef,
     CreateCapacityProviderRequestRequestTypeDef,
     UpdateCapacityProviderRequestRequestTypeDef,
     TaskSetTypeDef,
     CreateTaskSetRequestRequestTypeDef,
+    NetworkConfigurationUnionTypeDef,
     TaskOverrideOutputTypeDef,
     TaskOverrideTypeDef,
     ContainerInstanceTypeDef,
     SubmitTaskStateChangeRequestRequestTypeDef,
+    DeploymentConfigurationUnionTypeDef,
     ClusterConfigurationTypeDef,
     VolumeOutputTypeDef,
     VolumeTypeDef,
     ContainerDefinitionOutputTypeDef,
     ContainerDefinitionTypeDef,
+    RegisterContainerInstanceRequestRequestTypeDef,
     ServiceConnectConfigurationOutputTypeDef,
     ServiceConnectConfigurationTypeDef,
     CreateCapacityProviderResponseTypeDef,
     DeleteCapacityProviderResponseTypeDef,
     DescribeCapacityProvidersResponseTypeDef,
     UpdateCapacityProviderResponseTypeDef,
     CreateTaskSetResponseTypeDef,
     DeleteTaskSetResponseTypeDef,
     DescribeTaskSetsResponseTypeDef,
     UpdateServicePrimaryTaskSetResponseTypeDef,
     UpdateTaskSetResponseTypeDef,
     TaskTypeDef,
     RunTaskRequestRequestTypeDef,
     StartTaskRequestRequestTypeDef,
+    TaskOverrideUnionTypeDef,
     DeregisterContainerInstanceResponseTypeDef,
     DescribeContainerInstancesResponseTypeDef,
     RegisterContainerInstanceResponseTypeDef,
     UpdateContainerAgentResponseTypeDef,
     UpdateContainerInstancesStateResponseTypeDef,
     ClusterTypeDef,
     CreateClusterRequestRequestTypeDef,
     UpdateClusterRequestRequestTypeDef,
+    VolumeUnionTypeDef,
     TaskDefinitionTypeDef,
-    RegisterTaskDefinitionRequestRequestTypeDef,
+    ContainerDefinitionUnionTypeDef,
     DeploymentTypeDef,
     CreateServiceRequestRequestTypeDef,
+    ServiceConnectConfigurationUnionTypeDef,
     UpdateServiceRequestRequestTypeDef,
     DescribeTasksResponseTypeDef,
     RunTaskResponseTypeDef,
     StartTaskResponseTypeDef,
     StopTaskResponseTypeDef,
     CreateClusterResponseTypeDef,
     DeleteClusterResponseTypeDef,
@@ -673,23 +681,24 @@
     PutClusterCapacityProvidersResponseTypeDef,
     UpdateClusterResponseTypeDef,
     UpdateClusterSettingsResponseTypeDef,
     DeleteTaskDefinitionsResponseTypeDef,
     DeregisterTaskDefinitionResponseTypeDef,
     DescribeTaskDefinitionResponseTypeDef,
     RegisterTaskDefinitionResponseTypeDef,
+    RegisterTaskDefinitionRequestRequestTypeDef,
     ServiceTypeDef,
     CreateServiceResponseTypeDef,
     DeleteServiceResponseTypeDef,
     DescribeServicesResponseTypeDef,
     UpdateServiceResponseTypeDef,
 )
 
 
-def get_structure() -> AttachmentStateChangeTypeDef:
+def get_value() -> AttachmentStateChangeTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-ecs-1.28.15.post1/mypy_boto3_ecs.egg-info/SOURCES.txt` & `mypy-boto3-ecs-1.28.16/mypy_boto3_ecs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecs-1.28.15.post1/setup.py` & `mypy-boto3-ecs-1.28.16/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-ecs",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_ecs"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ECS 1.28.15 service generated with mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.ECS 1.28.16 service generated with mypy-boto3-builder 7.17.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
@@ -33,15 +33,15 @@
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
         "Typing :: Typed",
     ],
-    keywords="boto3 ecs type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 ecs type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_ecs": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

