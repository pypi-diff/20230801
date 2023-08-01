# Comparing `tmp/mypy-boto3-emr-containers-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-emr-containers-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-emr-containers-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:05 2023, max compression
+gzip compressed data, was "mypy-boto3-emr-containers-1.28.16.tar", last modified: Tue Aug  1 11:36:45 2023, max compression
```

## Comparing `mypy-boto3-emr-containers-1.28.15.post1.tar` & `mypy-boto3-emr-containers-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:05.913142 mypy-boto3-emr-containers-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:44:59.000000 mypy-boto3-emr-containers-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16598 2023-07-29 10:03:05.913142 mypy-boto3-emr-containers-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15078 2023-07-29 09:44:59.000000 mypy-boto3-emr-containers-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:05.913142 mypy-boto3-emr-containers-1.28.15.post1/mypy_boto3_emr_containers/
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-29 09:44:59.000000 mypy-boto3-emr-containers-1.28.15.post1/mypy_boto3_emr_containers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-07-29 09:44:59.000000 mypy-boto3-emr-containers-1.28.15.post1/mypy_boto3_emr_containers/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-29 09:44:59.000000 mypy-boto3-emr-containers-1.28.15.post1/mypy_boto3_emr_containers/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18682 2023-07-29 09:45:01.000000 mypy-boto3-emr-containers-1.28.15.post1/mypy_boto3_emr_containers/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    18651 2023-07-29 09:44:59.000000 mypy-boto3-emr-containers-1.28.15.post1/mypy_boto3_emr_containers/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9349 2023-07-29 09:45:01.000000 mypy-boto3-emr-containers-1.28.15.post1/mypy_boto3_emr_containers/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-07-29 09:45:01.000000 mypy-boto3-emr-containers-1.28.15.post1/mypy_boto3_emr_containers/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-07-29 09:45:01.000000 mypy-boto3-emr-containers-1.28.15.post1/mypy_boto3_emr_containers/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6293 2023-07-29 09:45:01.000000 mypy-boto3-emr-containers-1.28.15.post1/mypy_boto3_emr_containers/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:44:59.000000 mypy-boto3-emr-containers-1.28.15.post1/mypy_boto3_emr_containers/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    28645 2023-07-29 09:45:02.000000 mypy-boto3-emr-containers-1.28.15.post1/mypy_boto3_emr_containers/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    28608 2023-07-29 09:45:02.000000 mypy-boto3-emr-containers-1.28.15.post1/mypy_boto3_emr_containers/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:44:59.000000 mypy-boto3-emr-containers-1.28.15.post1/mypy_boto3_emr_containers/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:05.913142 mypy-boto3-emr-containers-1.28.15.post1/mypy_boto3_emr_containers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16598 2023-07-29 10:03:05.000000 mypy-boto3-emr-containers-1.28.15.post1/mypy_boto3_emr_containers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-29 10:03:05.000000 mypy-boto3-emr-containers-1.28.15.post1/mypy_boto3_emr_containers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:05.000000 mypy-boto3-emr-containers-1.28.15.post1/mypy_boto3_emr_containers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:05.000000 mypy-boto3-emr-containers-1.28.15.post1/mypy_boto3_emr_containers.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:05.000000 mypy-boto3-emr-containers-1.28.15.post1/mypy_boto3_emr_containers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-29 10:03:05.000000 mypy-boto3-emr-containers-1.28.15.post1/mypy_boto3_emr_containers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:05.913142 mypy-boto3-emr-containers-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-29 09:44:59.000000 mypy-boto3-emr-containers-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:45.772894 mypy-boto3-emr-containers-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:17:37.000000 mypy-boto3-emr-containers-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16710 2023-08-01 11:36:45.768895 mypy-boto3-emr-containers-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15199 2023-08-01 11:17:37.000000 mypy-boto3-emr-containers-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:45.760894 mypy-boto3-emr-containers-1.28.16/mypy_boto3_emr_containers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-08-01 11:17:37.000000 mypy-boto3-emr-containers-1.28.16/mypy_boto3_emr_containers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-08-01 11:17:37.000000 mypy-boto3-emr-containers-1.28.16/mypy_boto3_emr_containers/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-08-01 11:17:37.000000 mypy-boto3-emr-containers-1.28.16/mypy_boto3_emr_containers/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18367 2023-08-01 11:17:37.000000 mypy-boto3-emr-containers-1.28.16/mypy_boto3_emr_containers/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18336 2023-08-01 11:17:37.000000 mypy-boto3-emr-containers-1.28.16/mypy_boto3_emr_containers/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9367 2023-08-01 11:17:38.000000 mypy-boto3-emr-containers-1.28.16/mypy_boto3_emr_containers/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9365 2023-08-01 11:17:37.000000 mypy-boto3-emr-containers-1.28.16/mypy_boto3_emr_containers/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6253 2023-08-01 11:17:37.000000 mypy-boto3-emr-containers-1.28.16/mypy_boto3_emr_containers/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6246 2023-08-01 11:17:37.000000 mypy-boto3-emr-containers-1.28.16/mypy_boto3_emr_containers/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:17:37.000000 mypy-boto3-emr-containers-1.28.16/mypy_boto3_emr_containers/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    29028 2023-08-01 11:17:38.000000 mypy-boto3-emr-containers-1.28.16/mypy_boto3_emr_containers/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28991 2023-08-01 11:17:38.000000 mypy-boto3-emr-containers-1.28.16/mypy_boto3_emr_containers/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:17:37.000000 mypy-boto3-emr-containers-1.28.16/mypy_boto3_emr_containers/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:45.768895 mypy-boto3-emr-containers-1.28.16/mypy_boto3_emr_containers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16710 2023-08-01 11:36:45.000000 mypy-boto3-emr-containers-1.28.16/mypy_boto3_emr_containers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-08-01 11:36:45.000000 mypy-boto3-emr-containers-1.28.16/mypy_boto3_emr_containers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:45.000000 mypy-boto3-emr-containers-1.28.16/mypy_boto3_emr_containers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:45.000000 mypy-boto3-emr-containers-1.28.16/mypy_boto3_emr_containers.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:45.000000 mypy-boto3-emr-containers-1.28.16/mypy_boto3_emr_containers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-01 11:36:45.000000 mypy-boto3-emr-containers-1.28.16/mypy_boto3_emr_containers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:45.772894 mypy-boto3-emr-containers-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-08-01 11:17:37.000000 mypy-boto3-emr-containers-1.28.16/setup.py
```

### Comparing `mypy-boto3-emr-containers-1.28.15.post1/LICENSE` & `mypy-boto3-emr-containers-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-containers-1.28.15.post1/PKG-INFO` & `mypy-boto3-emr-containers-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-emr-containers
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.EMRContainers 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.EMRContainers 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 emr-containers type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 emr-containers type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-emr-containers.svg?color=blue)](https://pypi.org/project/mypy-boto3-emr-containers)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-emr-containers)](https://pepy.tech/project/mypy-boto3-emr-containers)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EMRContainers 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers)
+[boto3.EMRContainers 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers)
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
 [mypy-boto3-emr-containers docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/).
 
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
@@ -333,20 +333,20 @@
 )
 
 
 def check_value(value: ContainerProviderTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_emr_containers.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_emr_containers.type_defs import (
     CancelJobRunRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     CertificateTypeDef,
     CloudWatchMonitoringConfigurationTypeDef,
@@ -366,19 +366,16 @@
     SparkSqlJobDriverTypeDef,
     SparkSubmitJobDriverOutputTypeDef,
     SparkSubmitJobDriverTypeDef,
     RetryPolicyConfigurationTypeDef,
     RetryPolicyExecutionTypeDef,
     TemplateParameterConfigurationTypeDef,
     PaginatorConfigTypeDef,
-    ListJobRunsRequestRequestTypeDef,
-    ListJobTemplatesRequestRequestTypeDef,
-    ListManagedEndpointsRequestRequestTypeDef,
+    TimestampTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListVirtualClustersRequestRequestTypeDef,
     S3MonitoringConfigurationTypeDef,
     ParametricCloudWatchMonitoringConfigurationTypeDef,
     ParametricS3MonitoringConfigurationTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     CancelJobRunResponseTypeDef,
     CreateJobTemplateResponseTypeDef,
@@ -390,46 +387,53 @@
     ListTagsForResourceResponseTypeDef,
     StartJobRunResponseTypeDef,
     ContainerInfoTypeDef,
     GetManagedEndpointSessionCredentialsResponseTypeDef,
     JobDriverOutputTypeDef,
     JobDriverTypeDef,
     ListJobRunsRequestListJobRunsPaginateTypeDef,
+    ListJobRunsRequestRequestTypeDef,
     ListJobTemplatesRequestListJobTemplatesPaginateTypeDef,
+    ListJobTemplatesRequestRequestTypeDef,
     ListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef,
+    ListManagedEndpointsRequestRequestTypeDef,
     ListVirtualClustersRequestListVirtualClustersPaginateTypeDef,
+    ListVirtualClustersRequestRequestTypeDef,
     MonitoringConfigurationTypeDef,
     ParametricMonitoringConfigurationTypeDef,
     ContainerProviderTypeDef,
+    JobDriverUnionTypeDef,
     ConfigurationOverridesOutputTypeDef,
     ConfigurationOverridesTypeDef,
     ParametricConfigurationOverridesOutputTypeDef,
     ParametricConfigurationOverridesTypeDef,
     CreateVirtualClusterRequestRequestTypeDef,
     VirtualClusterTypeDef,
     EndpointTypeDef,
     JobRunTypeDef,
+    ConfigurationOverridesUnionTypeDef,
     CreateManagedEndpointRequestRequestTypeDef,
     StartJobRunRequestRequestTypeDef,
     JobTemplateDataOutputTypeDef,
     JobTemplateDataTypeDef,
     DescribeVirtualClusterResponseTypeDef,
     ListVirtualClustersResponseTypeDef,
     DescribeManagedEndpointResponseTypeDef,
     ListManagedEndpointsResponseTypeDef,
     DescribeJobRunResponseTypeDef,
     ListJobRunsResponseTypeDef,
     JobTemplateTypeDef,
     CreateJobTemplateRequestRequestTypeDef,
+    JobTemplateDataUnionTypeDef,
     DescribeJobTemplateResponseTypeDef,
     ListJobTemplatesResponseTypeDef,
 )
 
 
-def get_structure() -> CancelJobRunRequestRequestTypeDef:
+def get_value() -> CancelJobRunRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-emr-containers-1.28.15.post1/README.md` & `mypy-boto3-emr-containers-1.28.16/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-emr-containers.svg?color=blue)](https://pypi.org/project/mypy-boto3-emr-containers)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-emr-containers)](https://pepy.tech/project/mypy-boto3-emr-containers)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EMRContainers 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers)
+[boto3.EMRContainers 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers)
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
 [mypy-boto3-emr-containers docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/).
 
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
@@ -301,20 +301,20 @@
 )
 
 
 def check_value(value: ContainerProviderTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_emr_containers.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_emr_containers.type_defs import (
     CancelJobRunRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     CertificateTypeDef,
     CloudWatchMonitoringConfigurationTypeDef,
@@ -334,19 +334,16 @@
     SparkSqlJobDriverTypeDef,
     SparkSubmitJobDriverOutputTypeDef,
     SparkSubmitJobDriverTypeDef,
     RetryPolicyConfigurationTypeDef,
     RetryPolicyExecutionTypeDef,
     TemplateParameterConfigurationTypeDef,
     PaginatorConfigTypeDef,
-    ListJobRunsRequestRequestTypeDef,
-    ListJobTemplatesRequestRequestTypeDef,
-    ListManagedEndpointsRequestRequestTypeDef,
+    TimestampTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListVirtualClustersRequestRequestTypeDef,
     S3MonitoringConfigurationTypeDef,
     ParametricCloudWatchMonitoringConfigurationTypeDef,
     ParametricS3MonitoringConfigurationTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     CancelJobRunResponseTypeDef,
     CreateJobTemplateResponseTypeDef,
@@ -358,46 +355,53 @@
     ListTagsForResourceResponseTypeDef,
     StartJobRunResponseTypeDef,
     ContainerInfoTypeDef,
     GetManagedEndpointSessionCredentialsResponseTypeDef,
     JobDriverOutputTypeDef,
     JobDriverTypeDef,
     ListJobRunsRequestListJobRunsPaginateTypeDef,
+    ListJobRunsRequestRequestTypeDef,
     ListJobTemplatesRequestListJobTemplatesPaginateTypeDef,
+    ListJobTemplatesRequestRequestTypeDef,
     ListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef,
+    ListManagedEndpointsRequestRequestTypeDef,
     ListVirtualClustersRequestListVirtualClustersPaginateTypeDef,
+    ListVirtualClustersRequestRequestTypeDef,
     MonitoringConfigurationTypeDef,
     ParametricMonitoringConfigurationTypeDef,
     ContainerProviderTypeDef,
+    JobDriverUnionTypeDef,
     ConfigurationOverridesOutputTypeDef,
     ConfigurationOverridesTypeDef,
     ParametricConfigurationOverridesOutputTypeDef,
     ParametricConfigurationOverridesTypeDef,
     CreateVirtualClusterRequestRequestTypeDef,
     VirtualClusterTypeDef,
     EndpointTypeDef,
     JobRunTypeDef,
+    ConfigurationOverridesUnionTypeDef,
     CreateManagedEndpointRequestRequestTypeDef,
     StartJobRunRequestRequestTypeDef,
     JobTemplateDataOutputTypeDef,
     JobTemplateDataTypeDef,
     DescribeVirtualClusterResponseTypeDef,
     ListVirtualClustersResponseTypeDef,
     DescribeManagedEndpointResponseTypeDef,
     ListManagedEndpointsResponseTypeDef,
     DescribeJobRunResponseTypeDef,
     ListJobRunsResponseTypeDef,
     JobTemplateTypeDef,
     CreateJobTemplateRequestRequestTypeDef,
+    JobTemplateDataUnionTypeDef,
     DescribeJobTemplateResponseTypeDef,
     ListJobTemplatesResponseTypeDef,
 )
 
 
-def get_structure() -> CancelJobRunRequestRequestTypeDef:
+def get_value() -> CancelJobRunRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-emr-containers-1.28.15.post1/mypy_boto3_emr_containers/__init__.py` & `mypy-boto3-emr-containers-1.28.16/mypy_boto3_emr_containers/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-containers-1.28.15.post1/mypy_boto3_emr_containers/__init__.pyi` & `mypy-boto3-emr-containers-1.28.16/mypy_boto3_emr_containers/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-containers-1.28.15.post1/mypy_boto3_emr_containers/__main__.py` & `mypy-boto3-emr-containers-1.28.16/mypy_boto3_emr_containers/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.EMRContainers 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.EMRContainers 1.28.16\nVersion:         1.28.16\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers\nOther"
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

### Comparing `mypy-boto3-emr-containers-1.28.15.post1/mypy_boto3_emr_containers/client.py` & `mypy-boto3-emr-containers-1.28.16/mypy_boto3_emr_containers/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,53 +10,50 @@
     from mypy_boto3_emr_containers.client import EMRContainersClient
 
     session = Session()
     client: EMRContainersClient = session.client("emr-containers")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import EndpointStateType, JobRunStateType, VirtualClusterStateType
 from .paginator import (
     ListJobRunsPaginator,
     ListJobTemplatesPaginator,
     ListManagedEndpointsPaginator,
     ListVirtualClustersPaginator,
 )
 from .type_defs import (
     CancelJobRunResponseTypeDef,
-    ConfigurationOverridesOutputTypeDef,
-    ConfigurationOverridesTypeDef,
+    ConfigurationOverridesUnionTypeDef,
     ContainerProviderTypeDef,
     CreateJobTemplateResponseTypeDef,
     CreateManagedEndpointResponseTypeDef,
     CreateVirtualClusterResponseTypeDef,
     DeleteJobTemplateResponseTypeDef,
     DeleteManagedEndpointResponseTypeDef,
     DeleteVirtualClusterResponseTypeDef,
     DescribeJobRunResponseTypeDef,
     DescribeJobTemplateResponseTypeDef,
     DescribeManagedEndpointResponseTypeDef,
     DescribeVirtualClusterResponseTypeDef,
     GetManagedEndpointSessionCredentialsResponseTypeDef,
-    JobDriverOutputTypeDef,
-    JobDriverTypeDef,
-    JobTemplateDataOutputTypeDef,
-    JobTemplateDataTypeDef,
+    JobDriverUnionTypeDef,
+    JobTemplateDataUnionTypeDef,
     ListJobRunsResponseTypeDef,
     ListJobTemplatesResponseTypeDef,
     ListManagedEndpointsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListVirtualClustersResponseTypeDef,
     RetryPolicyConfigurationTypeDef,
     StartJobRunResponseTypeDef,
+    TimestampTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -122,15 +119,15 @@
         """
 
     def create_job_template(
         self,
         *,
         name: str,
         clientToken: str,
-        jobTemplateData: Union[JobTemplateDataTypeDef, JobTemplateDataOutputTypeDef],
+        jobTemplateData: JobTemplateDataUnionTypeDef,
         tags: Mapping[str, str] = ...,
         kmsKeyArn: str = ...
     ) -> CreateJobTemplateResponseTypeDef:
         """
         Creates a job template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.create_job_template)
@@ -143,17 +140,15 @@
         name: str,
         virtualClusterId: str,
         type: str,
         releaseLabel: str,
         executionRoleArn: str,
         clientToken: str,
         certificateArn: str = ...,
-        configurationOverrides: Union[
-            ConfigurationOverridesTypeDef, ConfigurationOverridesOutputTypeDef
-        ] = ...,
+        configurationOverrides: ConfigurationOverridesUnionTypeDef = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateManagedEndpointResponseTypeDef:
         """
         Creates a managed endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.create_managed_endpoint)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/client/#create_managed_endpoint)
@@ -266,16 +261,16 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/client/#get_managed_endpoint_session_credentials)
         """
 
     def list_job_runs(
         self,
         *,
         virtualClusterId: str,
-        createdBefore: Union[datetime, str] = ...,
-        createdAfter: Union[datetime, str] = ...,
+        createdBefore: TimestampTypeDef = ...,
+        createdAfter: TimestampTypeDef = ...,
         name: str = ...,
         states: Sequence[JobRunStateType] = ...,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> ListJobRunsResponseTypeDef:
         """
         Lists job runs based on a set of parameters.
@@ -283,32 +278,32 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.list_job_runs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/client/#list_job_runs)
         """
 
     def list_job_templates(
         self,
         *,
-        createdAfter: Union[datetime, str] = ...,
-        createdBefore: Union[datetime, str] = ...,
+        createdAfter: TimestampTypeDef = ...,
+        createdBefore: TimestampTypeDef = ...,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> ListJobTemplatesResponseTypeDef:
         """
         Lists job templates based on a set of parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.list_job_templates)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/client/#list_job_templates)
         """
 
     def list_managed_endpoints(
         self,
         *,
         virtualClusterId: str,
-        createdBefore: Union[datetime, str] = ...,
-        createdAfter: Union[datetime, str] = ...,
+        createdBefore: TimestampTypeDef = ...,
+        createdAfter: TimestampTypeDef = ...,
         types: Sequence[str] = ...,
         states: Sequence[EndpointStateType] = ...,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> ListManagedEndpointsResponseTypeDef:
         """
         Lists managed endpoints based on a set of parameters.
@@ -326,16 +321,16 @@
         """
 
     def list_virtual_clusters(
         self,
         *,
         containerProviderId: str = ...,
         containerProviderType: Literal["EKS"] = ...,
-        createdAfter: Union[datetime, str] = ...,
-        createdBefore: Union[datetime, str] = ...,
+        createdAfter: TimestampTypeDef = ...,
+        createdBefore: TimestampTypeDef = ...,
         states: Sequence[VirtualClusterStateType] = ...,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> ListVirtualClustersResponseTypeDef:
         """
         Lists information about the specified virtual cluster.
 
@@ -347,18 +342,16 @@
         self,
         *,
         virtualClusterId: str,
         clientToken: str,
         name: str = ...,
         executionRoleArn: str = ...,
         releaseLabel: str = ...,
-        jobDriver: Union[JobDriverTypeDef, JobDriverOutputTypeDef] = ...,
-        configurationOverrides: Union[
-            ConfigurationOverridesTypeDef, ConfigurationOverridesOutputTypeDef
-        ] = ...,
+        jobDriver: JobDriverUnionTypeDef = ...,
+        configurationOverrides: ConfigurationOverridesUnionTypeDef = ...,
         tags: Mapping[str, str] = ...,
         jobTemplateId: str = ...,
         jobTemplateParameters: Mapping[str, str] = ...,
         retryPolicyConfiguration: RetryPolicyConfigurationTypeDef = ...
     ) -> StartJobRunResponseTypeDef:
         """
         Starts a job run.
```

### Comparing `mypy-boto3-emr-containers-1.28.15.post1/mypy_boto3_emr_containers/client.pyi` & `mypy-boto3-emr-containers-1.28.16/mypy_boto3_emr_containers/client.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -10,53 +10,50 @@
     from mypy_boto3_emr_containers.client import EMRContainersClient
 
     session = Session()
     client: EMRContainersClient = session.client("emr-containers")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import EndpointStateType, JobRunStateType, VirtualClusterStateType
 from .paginator import (
     ListJobRunsPaginator,
     ListJobTemplatesPaginator,
     ListManagedEndpointsPaginator,
     ListVirtualClustersPaginator,
 )
 from .type_defs import (
     CancelJobRunResponseTypeDef,
-    ConfigurationOverridesOutputTypeDef,
-    ConfigurationOverridesTypeDef,
+    ConfigurationOverridesUnionTypeDef,
     ContainerProviderTypeDef,
     CreateJobTemplateResponseTypeDef,
     CreateManagedEndpointResponseTypeDef,
     CreateVirtualClusterResponseTypeDef,
     DeleteJobTemplateResponseTypeDef,
     DeleteManagedEndpointResponseTypeDef,
     DeleteVirtualClusterResponseTypeDef,
     DescribeJobRunResponseTypeDef,
     DescribeJobTemplateResponseTypeDef,
     DescribeManagedEndpointResponseTypeDef,
     DescribeVirtualClusterResponseTypeDef,
     GetManagedEndpointSessionCredentialsResponseTypeDef,
-    JobDriverOutputTypeDef,
-    JobDriverTypeDef,
-    JobTemplateDataOutputTypeDef,
-    JobTemplateDataTypeDef,
+    JobDriverUnionTypeDef,
+    JobTemplateDataUnionTypeDef,
     ListJobRunsResponseTypeDef,
     ListJobTemplatesResponseTypeDef,
     ListManagedEndpointsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListVirtualClustersResponseTypeDef,
     RetryPolicyConfigurationTypeDef,
     StartJobRunResponseTypeDef,
+    TimestampTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -114,15 +111,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/client/#close)
         """
     def create_job_template(
         self,
         *,
         name: str,
         clientToken: str,
-        jobTemplateData: Union[JobTemplateDataTypeDef, JobTemplateDataOutputTypeDef],
+        jobTemplateData: JobTemplateDataUnionTypeDef,
         tags: Mapping[str, str] = ...,
         kmsKeyArn: str = ...
     ) -> CreateJobTemplateResponseTypeDef:
         """
         Creates a job template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.create_job_template)
@@ -134,17 +131,15 @@
         name: str,
         virtualClusterId: str,
         type: str,
         releaseLabel: str,
         executionRoleArn: str,
         clientToken: str,
         certificateArn: str = ...,
-        configurationOverrides: Union[
-            ConfigurationOverridesTypeDef, ConfigurationOverridesOutputTypeDef
-        ] = ...,
+        configurationOverrides: ConfigurationOverridesUnionTypeDef = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateManagedEndpointResponseTypeDef:
         """
         Creates a managed endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.create_managed_endpoint)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/client/#create_managed_endpoint)
@@ -246,47 +241,47 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.get_managed_endpoint_session_credentials)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/client/#get_managed_endpoint_session_credentials)
         """
     def list_job_runs(
         self,
         *,
         virtualClusterId: str,
-        createdBefore: Union[datetime, str] = ...,
-        createdAfter: Union[datetime, str] = ...,
+        createdBefore: TimestampTypeDef = ...,
+        createdAfter: TimestampTypeDef = ...,
         name: str = ...,
         states: Sequence[JobRunStateType] = ...,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> ListJobRunsResponseTypeDef:
         """
         Lists job runs based on a set of parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.list_job_runs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/client/#list_job_runs)
         """
     def list_job_templates(
         self,
         *,
-        createdAfter: Union[datetime, str] = ...,
-        createdBefore: Union[datetime, str] = ...,
+        createdAfter: TimestampTypeDef = ...,
+        createdBefore: TimestampTypeDef = ...,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> ListJobTemplatesResponseTypeDef:
         """
         Lists job templates based on a set of parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.list_job_templates)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/client/#list_job_templates)
         """
     def list_managed_endpoints(
         self,
         *,
         virtualClusterId: str,
-        createdBefore: Union[datetime, str] = ...,
-        createdAfter: Union[datetime, str] = ...,
+        createdBefore: TimestampTypeDef = ...,
+        createdAfter: TimestampTypeDef = ...,
         types: Sequence[str] = ...,
         states: Sequence[EndpointStateType] = ...,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> ListManagedEndpointsResponseTypeDef:
         """
         Lists managed endpoints based on a set of parameters.
@@ -302,16 +297,16 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/client/#list_tags_for_resource)
         """
     def list_virtual_clusters(
         self,
         *,
         containerProviderId: str = ...,
         containerProviderType: Literal["EKS"] = ...,
-        createdAfter: Union[datetime, str] = ...,
-        createdBefore: Union[datetime, str] = ...,
+        createdAfter: TimestampTypeDef = ...,
+        createdBefore: TimestampTypeDef = ...,
         states: Sequence[VirtualClusterStateType] = ...,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> ListVirtualClustersResponseTypeDef:
         """
         Lists information about the specified virtual cluster.
 
@@ -322,18 +317,16 @@
         self,
         *,
         virtualClusterId: str,
         clientToken: str,
         name: str = ...,
         executionRoleArn: str = ...,
         releaseLabel: str = ...,
-        jobDriver: Union[JobDriverTypeDef, JobDriverOutputTypeDef] = ...,
-        configurationOverrides: Union[
-            ConfigurationOverridesTypeDef, ConfigurationOverridesOutputTypeDef
-        ] = ...,
+        jobDriver: JobDriverUnionTypeDef = ...,
+        configurationOverrides: ConfigurationOverridesUnionTypeDef = ...,
         tags: Mapping[str, str] = ...,
         jobTemplateId: str = ...,
         jobTemplateParameters: Mapping[str, str] = ...,
         retryPolicyConfiguration: RetryPolicyConfigurationTypeDef = ...
     ) -> StartJobRunResponseTypeDef:
         """
         Starts a job run.
```

### Comparing `mypy-boto3-emr-containers-1.28.15.post1/mypy_boto3_emr_containers/literals.py` & `mypy-boto3-emr-containers-1.28.16/mypy_boto3_emr_containers/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -424,14 +424,15 @@
     "sns",
     "sqs",
 ]
 PaginatorName = Literal[
     "list_job_runs", "list_job_templates", "list_managed_endpoints", "list_virtual_clusters"
 ]
 RegionName = Literal[
+    "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-south-1",
     "ap-southeast-1",
     "ap-southeast-2",
     "ca-central-1",
```

### Comparing `mypy-boto3-emr-containers-1.28.15.post1/mypy_boto3_emr_containers/literals.pyi` & `mypy-boto3-emr-containers-1.28.16/mypy_boto3_emr_containers/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -422,14 +422,15 @@
     "sns",
     "sqs",
 ]
 PaginatorName = Literal[
     "list_job_runs", "list_job_templates", "list_managed_endpoints", "list_virtual_clusters"
 ]
 RegionName = Literal[
+    "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-south-1",
     "ap-southeast-1",
     "ap-southeast-2",
     "ca-central-1",
```

### Comparing `mypy-boto3-emr-containers-1.28.15.post1/mypy_boto3_emr_containers/paginator.py` & `mypy-boto3-emr-containers-1.28.16/mypy_boto3_emr_containers/paginator.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -22,128 +22,121 @@
     list_job_runs_paginator: ListJobRunsPaginator = client.get_paginator("list_job_runs")
     list_job_templates_paginator: ListJobTemplatesPaginator = client.get_paginator("list_job_templates")
     list_managed_endpoints_paginator: ListManagedEndpointsPaginator = client.get_paginator("list_managed_endpoints")
     list_virtual_clusters_paginator: ListVirtualClustersPaginator = client.get_paginator("list_virtual_clusters")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Generic, Iterator, Sequence, TypeVar, Union
+from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import EndpointStateType, JobRunStateType, VirtualClusterStateType
 from .type_defs import (
     ListJobRunsResponseTypeDef,
     ListJobTemplatesResponseTypeDef,
     ListManagedEndpointsResponseTypeDef,
     ListVirtualClustersResponseTypeDef,
     PaginatorConfigTypeDef,
+    TimestampTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ListJobRunsPaginator",
     "ListJobTemplatesPaginator",
     "ListManagedEndpointsPaginator",
     "ListVirtualClustersPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class ListJobRunsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Paginator.ListJobRuns)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/paginators/#listjobrunspaginator)
     """
 
     def paginate(
         self,
         *,
         virtualClusterId: str,
-        createdBefore: Union[datetime, str] = ...,
-        createdAfter: Union[datetime, str] = ...,
+        createdBefore: TimestampTypeDef = ...,
+        createdAfter: TimestampTypeDef = ...,
         name: str = ...,
         states: Sequence[JobRunStateType] = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListJobRunsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Paginator.ListJobRuns.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/paginators/#listjobrunspaginator)
         """
 
-
 class ListJobTemplatesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Paginator.ListJobTemplates)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/paginators/#listjobtemplatespaginator)
     """
 
     def paginate(
         self,
         *,
-        createdAfter: Union[datetime, str] = ...,
-        createdBefore: Union[datetime, str] = ...,
+        createdAfter: TimestampTypeDef = ...,
+        createdBefore: TimestampTypeDef = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListJobTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Paginator.ListJobTemplates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/paginators/#listjobtemplatespaginator)
         """
 
-
 class ListManagedEndpointsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Paginator.ListManagedEndpoints)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/paginators/#listmanagedendpointspaginator)
     """
 
     def paginate(
         self,
         *,
         virtualClusterId: str,
-        createdBefore: Union[datetime, str] = ...,
-        createdAfter: Union[datetime, str] = ...,
+        createdBefore: TimestampTypeDef = ...,
+        createdAfter: TimestampTypeDef = ...,
         types: Sequence[str] = ...,
         states: Sequence[EndpointStateType] = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListManagedEndpointsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Paginator.ListManagedEndpoints.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/paginators/#listmanagedendpointspaginator)
         """
 
-
 class ListVirtualClustersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Paginator.ListVirtualClusters)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/paginators/#listvirtualclusterspaginator)
     """
 
     def paginate(
         self,
         *,
         containerProviderId: str = ...,
         containerProviderType: Literal["EKS"] = ...,
-        createdAfter: Union[datetime, str] = ...,
-        createdBefore: Union[datetime, str] = ...,
+        createdAfter: TimestampTypeDef = ...,
+        createdBefore: TimestampTypeDef = ...,
         states: Sequence[VirtualClusterStateType] = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListVirtualClustersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Paginator.ListVirtualClusters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/paginators/#listvirtualclusterspaginator)
         """
```

### Comparing `mypy-boto3-emr-containers-1.28.15.post1/mypy_boto3_emr_containers/paginator.pyi` & `mypy-boto3-emr-containers-1.28.16/mypy_boto3_emr_containers/paginator.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,121 +22,128 @@
     list_job_runs_paginator: ListJobRunsPaginator = client.get_paginator("list_job_runs")
     list_job_templates_paginator: ListJobTemplatesPaginator = client.get_paginator("list_job_templates")
     list_managed_endpoints_paginator: ListManagedEndpointsPaginator = client.get_paginator("list_managed_endpoints")
     list_virtual_clusters_paginator: ListVirtualClustersPaginator = client.get_paginator("list_virtual_clusters")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Generic, Iterator, Sequence, TypeVar, Union
+from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import EndpointStateType, JobRunStateType, VirtualClusterStateType
 from .type_defs import (
     ListJobRunsResponseTypeDef,
     ListJobTemplatesResponseTypeDef,
     ListManagedEndpointsResponseTypeDef,
     ListVirtualClustersResponseTypeDef,
     PaginatorConfigTypeDef,
+    TimestampTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "ListJobRunsPaginator",
     "ListJobTemplatesPaginator",
     "ListManagedEndpointsPaginator",
     "ListVirtualClustersPaginator",
 )
 
+
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class ListJobRunsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Paginator.ListJobRuns)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/paginators/#listjobrunspaginator)
     """
 
     def paginate(
         self,
         *,
         virtualClusterId: str,
-        createdBefore: Union[datetime, str] = ...,
-        createdAfter: Union[datetime, str] = ...,
+        createdBefore: TimestampTypeDef = ...,
+        createdAfter: TimestampTypeDef = ...,
         name: str = ...,
         states: Sequence[JobRunStateType] = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListJobRunsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Paginator.ListJobRuns.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/paginators/#listjobrunspaginator)
         """
 
+
 class ListJobTemplatesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Paginator.ListJobTemplates)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/paginators/#listjobtemplatespaginator)
     """
 
     def paginate(
         self,
         *,
-        createdAfter: Union[datetime, str] = ...,
-        createdBefore: Union[datetime, str] = ...,
+        createdAfter: TimestampTypeDef = ...,
+        createdBefore: TimestampTypeDef = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListJobTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Paginator.ListJobTemplates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/paginators/#listjobtemplatespaginator)
         """
 
+
 class ListManagedEndpointsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Paginator.ListManagedEndpoints)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/paginators/#listmanagedendpointspaginator)
     """
 
     def paginate(
         self,
         *,
         virtualClusterId: str,
-        createdBefore: Union[datetime, str] = ...,
-        createdAfter: Union[datetime, str] = ...,
+        createdBefore: TimestampTypeDef = ...,
+        createdAfter: TimestampTypeDef = ...,
         types: Sequence[str] = ...,
         states: Sequence[EndpointStateType] = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListManagedEndpointsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Paginator.ListManagedEndpoints.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/paginators/#listmanagedendpointspaginator)
         """
 
+
 class ListVirtualClustersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Paginator.ListVirtualClusters)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/paginators/#listvirtualclusterspaginator)
     """
 
     def paginate(
         self,
         *,
         containerProviderId: str = ...,
         containerProviderType: Literal["EKS"] = ...,
-        createdAfter: Union[datetime, str] = ...,
-        createdBefore: Union[datetime, str] = ...,
+        createdAfter: TimestampTypeDef = ...,
+        createdBefore: TimestampTypeDef = ...,
         states: Sequence[VirtualClusterStateType] = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListVirtualClustersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Paginator.ListVirtualClusters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/paginators/#listvirtualclusterspaginator)
         """
```

### Comparing `mypy-boto3-emr-containers-1.28.15.post1/mypy_boto3_emr_containers/type_defs.py` & `mypy-boto3-emr-containers-1.28.16/mypy_boto3_emr_containers/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_emr_containers.type_defs import CancelJobRunRequestRequestTypeDef
 
-    data: CancelJobRunRequestRequestTypeDef = {...}
+    data: CancelJobRunRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -55,19 +55,16 @@
     "SparkSqlJobDriverTypeDef",
     "SparkSubmitJobDriverOutputTypeDef",
     "SparkSubmitJobDriverTypeDef",
     "RetryPolicyConfigurationTypeDef",
     "RetryPolicyExecutionTypeDef",
     "TemplateParameterConfigurationTypeDef",
     "PaginatorConfigTypeDef",
-    "ListJobRunsRequestRequestTypeDef",
-    "ListJobTemplatesRequestRequestTypeDef",
-    "ListManagedEndpointsRequestRequestTypeDef",
+    "TimestampTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListVirtualClustersRequestRequestTypeDef",
     "S3MonitoringConfigurationTypeDef",
     "ParametricCloudWatchMonitoringConfigurationTypeDef",
     "ParametricS3MonitoringConfigurationTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "CancelJobRunResponseTypeDef",
     "CreateJobTemplateResponseTypeDef",
@@ -79,40 +76,47 @@
     "ListTagsForResourceResponseTypeDef",
     "StartJobRunResponseTypeDef",
     "ContainerInfoTypeDef",
     "GetManagedEndpointSessionCredentialsResponseTypeDef",
     "JobDriverOutputTypeDef",
     "JobDriverTypeDef",
     "ListJobRunsRequestListJobRunsPaginateTypeDef",
+    "ListJobRunsRequestRequestTypeDef",
     "ListJobTemplatesRequestListJobTemplatesPaginateTypeDef",
+    "ListJobTemplatesRequestRequestTypeDef",
     "ListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef",
+    "ListManagedEndpointsRequestRequestTypeDef",
     "ListVirtualClustersRequestListVirtualClustersPaginateTypeDef",
+    "ListVirtualClustersRequestRequestTypeDef",
     "MonitoringConfigurationTypeDef",
     "ParametricMonitoringConfigurationTypeDef",
     "ContainerProviderTypeDef",
+    "JobDriverUnionTypeDef",
     "ConfigurationOverridesOutputTypeDef",
     "ConfigurationOverridesTypeDef",
     "ParametricConfigurationOverridesOutputTypeDef",
     "ParametricConfigurationOverridesTypeDef",
     "CreateVirtualClusterRequestRequestTypeDef",
     "VirtualClusterTypeDef",
     "EndpointTypeDef",
     "JobRunTypeDef",
+    "ConfigurationOverridesUnionTypeDef",
     "CreateManagedEndpointRequestRequestTypeDef",
     "StartJobRunRequestRequestTypeDef",
     "JobTemplateDataOutputTypeDef",
     "JobTemplateDataTypeDef",
     "DescribeVirtualClusterResponseTypeDef",
     "ListVirtualClustersResponseTypeDef",
     "DescribeManagedEndpointResponseTypeDef",
     "ListManagedEndpointsResponseTypeDef",
     "DescribeJobRunResponseTypeDef",
     "ListJobRunsResponseTypeDef",
     "JobTemplateTypeDef",
     "CreateJobTemplateRequestRequestTypeDef",
+    "JobTemplateDataUnionTypeDef",
     "DescribeJobTemplateResponseTypeDef",
     "ListJobTemplatesResponseTypeDef",
 )
 
 CancelJobRunRequestRequestTypeDef = TypedDict(
     "CancelJobRunRequestRequestTypeDef",
     {
@@ -390,99 +394,22 @@
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
-_RequiredListJobRunsRequestRequestTypeDef = TypedDict(
-    "_RequiredListJobRunsRequestRequestTypeDef",
-    {
-        "virtualClusterId": str,
-    },
-)
-_OptionalListJobRunsRequestRequestTypeDef = TypedDict(
-    "_OptionalListJobRunsRequestRequestTypeDef",
-    {
-        "createdBefore": Union[datetime, str],
-        "createdAfter": Union[datetime, str],
-        "name": str,
-        "states": Sequence[JobRunStateType],
-        "maxResults": int,
-        "nextToken": str,
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
-ListJobTemplatesRequestRequestTypeDef = TypedDict(
-    "ListJobTemplatesRequestRequestTypeDef",
-    {
-        "createdAfter": Union[datetime, str],
-        "createdBefore": Union[datetime, str],
-        "maxResults": int,
-        "nextToken": str,
-    },
-    total=False,
-)
-
-_RequiredListManagedEndpointsRequestRequestTypeDef = TypedDict(
-    "_RequiredListManagedEndpointsRequestRequestTypeDef",
-    {
-        "virtualClusterId": str,
-    },
-)
-_OptionalListManagedEndpointsRequestRequestTypeDef = TypedDict(
-    "_OptionalListManagedEndpointsRequestRequestTypeDef",
-    {
-        "createdBefore": Union[datetime, str],
-        "createdAfter": Union[datetime, str],
-        "types": Sequence[str],
-        "states": Sequence[EndpointStateType],
-        "maxResults": int,
-        "nextToken": str,
-    },
-    total=False,
-)
-
-
-class ListManagedEndpointsRequestRequestTypeDef(
-    _RequiredListManagedEndpointsRequestRequestTypeDef,
-    _OptionalListManagedEndpointsRequestRequestTypeDef,
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
 
-ListVirtualClustersRequestRequestTypeDef = TypedDict(
-    "ListVirtualClustersRequestRequestTypeDef",
-    {
-        "containerProviderId": str,
-        "containerProviderType": Literal["EKS"],
-        "createdAfter": Union[datetime, str],
-        "createdBefore": Union[datetime, str],
-        "states": Sequence[VirtualClusterStateType],
-        "maxResults": int,
-        "nextToken": str,
-    },
-    total=False,
-)
-
 S3MonitoringConfigurationTypeDef = TypedDict(
     "S3MonitoringConfigurationTypeDef",
     {
         "logUri": str,
     },
 )
 
@@ -645,16 +572,16 @@
     {
         "virtualClusterId": str,
     },
 )
 _OptionalListJobRunsRequestListJobRunsPaginateTypeDef = TypedDict(
     "_OptionalListJobRunsRequestListJobRunsPaginateTypeDef",
     {
-        "createdBefore": Union[datetime, str],
-        "createdAfter": Union[datetime, str],
+        "createdBefore": TimestampTypeDef,
+        "createdAfter": TimestampTypeDef,
         "name": str,
         "states": Sequence[JobRunStateType],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
@@ -662,35 +589,72 @@
 class ListJobRunsRequestListJobRunsPaginateTypeDef(
     _RequiredListJobRunsRequestListJobRunsPaginateTypeDef,
     _OptionalListJobRunsRequestListJobRunsPaginateTypeDef,
 ):
     pass
 
 
+_RequiredListJobRunsRequestRequestTypeDef = TypedDict(
+    "_RequiredListJobRunsRequestRequestTypeDef",
+    {
+        "virtualClusterId": str,
+    },
+)
+_OptionalListJobRunsRequestRequestTypeDef = TypedDict(
+    "_OptionalListJobRunsRequestRequestTypeDef",
+    {
+        "createdBefore": TimestampTypeDef,
+        "createdAfter": TimestampTypeDef,
+        "name": str,
+        "states": Sequence[JobRunStateType],
+        "maxResults": int,
+        "nextToken": str,
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
 ListJobTemplatesRequestListJobTemplatesPaginateTypeDef = TypedDict(
     "ListJobTemplatesRequestListJobTemplatesPaginateTypeDef",
     {
-        "createdAfter": Union[datetime, str],
-        "createdBefore": Union[datetime, str],
+        "createdAfter": TimestampTypeDef,
+        "createdBefore": TimestampTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+ListJobTemplatesRequestRequestTypeDef = TypedDict(
+    "ListJobTemplatesRequestRequestTypeDef",
+    {
+        "createdAfter": TimestampTypeDef,
+        "createdBefore": TimestampTypeDef,
+        "maxResults": int,
+        "nextToken": str,
+    },
+    total=False,
+)
+
 _RequiredListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef = TypedDict(
     "_RequiredListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef",
     {
         "virtualClusterId": str,
     },
 )
 _OptionalListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef = TypedDict(
     "_OptionalListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef",
     {
-        "createdBefore": Union[datetime, str],
-        "createdAfter": Union[datetime, str],
+        "createdBefore": TimestampTypeDef,
+        "createdAfter": TimestampTypeDef,
         "types": Sequence[str],
         "states": Sequence[EndpointStateType],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
@@ -698,27 +662,68 @@
 class ListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef(
     _RequiredListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef,
     _OptionalListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef,
 ):
     pass
 
 
+_RequiredListManagedEndpointsRequestRequestTypeDef = TypedDict(
+    "_RequiredListManagedEndpointsRequestRequestTypeDef",
+    {
+        "virtualClusterId": str,
+    },
+)
+_OptionalListManagedEndpointsRequestRequestTypeDef = TypedDict(
+    "_OptionalListManagedEndpointsRequestRequestTypeDef",
+    {
+        "createdBefore": TimestampTypeDef,
+        "createdAfter": TimestampTypeDef,
+        "types": Sequence[str],
+        "states": Sequence[EndpointStateType],
+        "maxResults": int,
+        "nextToken": str,
+    },
+    total=False,
+)
+
+
+class ListManagedEndpointsRequestRequestTypeDef(
+    _RequiredListManagedEndpointsRequestRequestTypeDef,
+    _OptionalListManagedEndpointsRequestRequestTypeDef,
+):
+    pass
+
+
 ListVirtualClustersRequestListVirtualClustersPaginateTypeDef = TypedDict(
     "ListVirtualClustersRequestListVirtualClustersPaginateTypeDef",
     {
         "containerProviderId": str,
         "containerProviderType": Literal["EKS"],
-        "createdAfter": Union[datetime, str],
-        "createdBefore": Union[datetime, str],
+        "createdAfter": TimestampTypeDef,
+        "createdBefore": TimestampTypeDef,
         "states": Sequence[VirtualClusterStateType],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+ListVirtualClustersRequestRequestTypeDef = TypedDict(
+    "ListVirtualClustersRequestRequestTypeDef",
+    {
+        "containerProviderId": str,
+        "containerProviderType": Literal["EKS"],
+        "createdAfter": TimestampTypeDef,
+        "createdBefore": TimestampTypeDef,
+        "states": Sequence[VirtualClusterStateType],
+        "maxResults": int,
+        "nextToken": str,
+    },
+    total=False,
+)
+
 MonitoringConfigurationTypeDef = TypedDict(
     "MonitoringConfigurationTypeDef",
     {
         "persistentAppUI": PersistentAppUIType,
         "cloudWatchMonitoringConfiguration": CloudWatchMonitoringConfigurationTypeDef,
         "s3MonitoringConfiguration": S3MonitoringConfigurationTypeDef,
         "containerLogRotationConfiguration": ContainerLogRotationConfigurationTypeDef,
@@ -754,14 +759,15 @@
 
 class ContainerProviderTypeDef(
     _RequiredContainerProviderTypeDef, _OptionalContainerProviderTypeDef
 ):
     pass
 
 
+JobDriverUnionTypeDef = Union[JobDriverTypeDef, JobDriverOutputTypeDef]
 ConfigurationOverridesOutputTypeDef = TypedDict(
     "ConfigurationOverridesOutputTypeDef",
     {
         "applicationConfiguration": List["ConfigurationOutputTypeDef"],
         "monitoringConfiguration": MonitoringConfigurationTypeDef,
     },
     total=False,
@@ -878,14 +884,17 @@
         "tags": Dict[str, str],
         "retryPolicyConfiguration": RetryPolicyConfigurationTypeDef,
         "retryPolicyExecution": RetryPolicyExecutionTypeDef,
     },
     total=False,
 )
 
+ConfigurationOverridesUnionTypeDef = Union[
+    ConfigurationOverridesTypeDef, ConfigurationOverridesOutputTypeDef
+]
 _RequiredCreateManagedEndpointRequestRequestTypeDef = TypedDict(
     "_RequiredCreateManagedEndpointRequestRequestTypeDef",
     {
         "name": str,
         "virtualClusterId": str,
         "type": str,
         "releaseLabel": str,
@@ -1086,14 +1095,15 @@
 
 class CreateJobTemplateRequestRequestTypeDef(
     _RequiredCreateJobTemplateRequestRequestTypeDef, _OptionalCreateJobTemplateRequestRequestTypeDef
 ):
     pass
 
 
+JobTemplateDataUnionTypeDef = Union[JobTemplateDataTypeDef, JobTemplateDataOutputTypeDef]
 DescribeJobTemplateResponseTypeDef = TypedDict(
     "DescribeJobTemplateResponseTypeDef",
     {
         "jobTemplate": JobTemplateTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-emr-containers-1.28.15.post1/mypy_boto3_emr_containers/type_defs.pyi` & `mypy-boto3-emr-containers-1.28.16/mypy_boto3_emr_containers/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_emr_containers.type_defs import CancelJobRunRequestRequestTypeDef
 
-    data: CancelJobRunRequestRequestTypeDef = {...}
+    data: CancelJobRunRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -54,19 +54,16 @@
     "SparkSqlJobDriverTypeDef",
     "SparkSubmitJobDriverOutputTypeDef",
     "SparkSubmitJobDriverTypeDef",
     "RetryPolicyConfigurationTypeDef",
     "RetryPolicyExecutionTypeDef",
     "TemplateParameterConfigurationTypeDef",
     "PaginatorConfigTypeDef",
-    "ListJobRunsRequestRequestTypeDef",
-    "ListJobTemplatesRequestRequestTypeDef",
-    "ListManagedEndpointsRequestRequestTypeDef",
+    "TimestampTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListVirtualClustersRequestRequestTypeDef",
     "S3MonitoringConfigurationTypeDef",
     "ParametricCloudWatchMonitoringConfigurationTypeDef",
     "ParametricS3MonitoringConfigurationTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "CancelJobRunResponseTypeDef",
     "CreateJobTemplateResponseTypeDef",
@@ -78,40 +75,47 @@
     "ListTagsForResourceResponseTypeDef",
     "StartJobRunResponseTypeDef",
     "ContainerInfoTypeDef",
     "GetManagedEndpointSessionCredentialsResponseTypeDef",
     "JobDriverOutputTypeDef",
     "JobDriverTypeDef",
     "ListJobRunsRequestListJobRunsPaginateTypeDef",
+    "ListJobRunsRequestRequestTypeDef",
     "ListJobTemplatesRequestListJobTemplatesPaginateTypeDef",
+    "ListJobTemplatesRequestRequestTypeDef",
     "ListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef",
+    "ListManagedEndpointsRequestRequestTypeDef",
     "ListVirtualClustersRequestListVirtualClustersPaginateTypeDef",
+    "ListVirtualClustersRequestRequestTypeDef",
     "MonitoringConfigurationTypeDef",
     "ParametricMonitoringConfigurationTypeDef",
     "ContainerProviderTypeDef",
+    "JobDriverUnionTypeDef",
     "ConfigurationOverridesOutputTypeDef",
     "ConfigurationOverridesTypeDef",
     "ParametricConfigurationOverridesOutputTypeDef",
     "ParametricConfigurationOverridesTypeDef",
     "CreateVirtualClusterRequestRequestTypeDef",
     "VirtualClusterTypeDef",
     "EndpointTypeDef",
     "JobRunTypeDef",
+    "ConfigurationOverridesUnionTypeDef",
     "CreateManagedEndpointRequestRequestTypeDef",
     "StartJobRunRequestRequestTypeDef",
     "JobTemplateDataOutputTypeDef",
     "JobTemplateDataTypeDef",
     "DescribeVirtualClusterResponseTypeDef",
     "ListVirtualClustersResponseTypeDef",
     "DescribeManagedEndpointResponseTypeDef",
     "ListManagedEndpointsResponseTypeDef",
     "DescribeJobRunResponseTypeDef",
     "ListJobRunsResponseTypeDef",
     "JobTemplateTypeDef",
     "CreateJobTemplateRequestRequestTypeDef",
+    "JobTemplateDataUnionTypeDef",
     "DescribeJobTemplateResponseTypeDef",
     "ListJobTemplatesResponseTypeDef",
 )
 
 CancelJobRunRequestRequestTypeDef = TypedDict(
     "CancelJobRunRequestRequestTypeDef",
     {
@@ -377,95 +381,22 @@
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
-_RequiredListJobRunsRequestRequestTypeDef = TypedDict(
-    "_RequiredListJobRunsRequestRequestTypeDef",
-    {
-        "virtualClusterId": str,
-    },
-)
-_OptionalListJobRunsRequestRequestTypeDef = TypedDict(
-    "_OptionalListJobRunsRequestRequestTypeDef",
-    {
-        "createdBefore": Union[datetime, str],
-        "createdAfter": Union[datetime, str],
-        "name": str,
-        "states": Sequence[JobRunStateType],
-        "maxResults": int,
-        "nextToken": str,
-    },
-    total=False,
-)
-
-class ListJobRunsRequestRequestTypeDef(
-    _RequiredListJobRunsRequestRequestTypeDef, _OptionalListJobRunsRequestRequestTypeDef
-):
-    pass
-
-ListJobTemplatesRequestRequestTypeDef = TypedDict(
-    "ListJobTemplatesRequestRequestTypeDef",
-    {
-        "createdAfter": Union[datetime, str],
-        "createdBefore": Union[datetime, str],
-        "maxResults": int,
-        "nextToken": str,
-    },
-    total=False,
-)
-
-_RequiredListManagedEndpointsRequestRequestTypeDef = TypedDict(
-    "_RequiredListManagedEndpointsRequestRequestTypeDef",
-    {
-        "virtualClusterId": str,
-    },
-)
-_OptionalListManagedEndpointsRequestRequestTypeDef = TypedDict(
-    "_OptionalListManagedEndpointsRequestRequestTypeDef",
-    {
-        "createdBefore": Union[datetime, str],
-        "createdAfter": Union[datetime, str],
-        "types": Sequence[str],
-        "states": Sequence[EndpointStateType],
-        "maxResults": int,
-        "nextToken": str,
-    },
-    total=False,
-)
-
-class ListManagedEndpointsRequestRequestTypeDef(
-    _RequiredListManagedEndpointsRequestRequestTypeDef,
-    _OptionalListManagedEndpointsRequestRequestTypeDef,
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
 
-ListVirtualClustersRequestRequestTypeDef = TypedDict(
-    "ListVirtualClustersRequestRequestTypeDef",
-    {
-        "containerProviderId": str,
-        "containerProviderType": Literal["EKS"],
-        "createdAfter": Union[datetime, str],
-        "createdBefore": Union[datetime, str],
-        "states": Sequence[VirtualClusterStateType],
-        "maxResults": int,
-        "nextToken": str,
-    },
-    total=False,
-)
-
 S3MonitoringConfigurationTypeDef = TypedDict(
     "S3MonitoringConfigurationTypeDef",
     {
         "logUri": str,
     },
 )
 
@@ -628,76 +559,150 @@
     {
         "virtualClusterId": str,
     },
 )
 _OptionalListJobRunsRequestListJobRunsPaginateTypeDef = TypedDict(
     "_OptionalListJobRunsRequestListJobRunsPaginateTypeDef",
     {
-        "createdBefore": Union[datetime, str],
-        "createdAfter": Union[datetime, str],
+        "createdBefore": TimestampTypeDef,
+        "createdAfter": TimestampTypeDef,
         "name": str,
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
+        "virtualClusterId": str,
+    },
+)
+_OptionalListJobRunsRequestRequestTypeDef = TypedDict(
+    "_OptionalListJobRunsRequestRequestTypeDef",
+    {
+        "createdBefore": TimestampTypeDef,
+        "createdAfter": TimestampTypeDef,
+        "name": str,
+        "states": Sequence[JobRunStateType],
+        "maxResults": int,
+        "nextToken": str,
+    },
+    total=False,
+)
+
+class ListJobRunsRequestRequestTypeDef(
+    _RequiredListJobRunsRequestRequestTypeDef, _OptionalListJobRunsRequestRequestTypeDef
+):
+    pass
+
 ListJobTemplatesRequestListJobTemplatesPaginateTypeDef = TypedDict(
     "ListJobTemplatesRequestListJobTemplatesPaginateTypeDef",
     {
-        "createdAfter": Union[datetime, str],
-        "createdBefore": Union[datetime, str],
+        "createdAfter": TimestampTypeDef,
+        "createdBefore": TimestampTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+ListJobTemplatesRequestRequestTypeDef = TypedDict(
+    "ListJobTemplatesRequestRequestTypeDef",
+    {
+        "createdAfter": TimestampTypeDef,
+        "createdBefore": TimestampTypeDef,
+        "maxResults": int,
+        "nextToken": str,
+    },
+    total=False,
+)
+
 _RequiredListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef = TypedDict(
     "_RequiredListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef",
     {
         "virtualClusterId": str,
     },
 )
 _OptionalListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef = TypedDict(
     "_OptionalListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef",
     {
-        "createdBefore": Union[datetime, str],
-        "createdAfter": Union[datetime, str],
+        "createdBefore": TimestampTypeDef,
+        "createdAfter": TimestampTypeDef,
         "types": Sequence[str],
         "states": Sequence[EndpointStateType],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class ListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef(
     _RequiredListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef,
     _OptionalListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef,
 ):
     pass
 
+_RequiredListManagedEndpointsRequestRequestTypeDef = TypedDict(
+    "_RequiredListManagedEndpointsRequestRequestTypeDef",
+    {
+        "virtualClusterId": str,
+    },
+)
+_OptionalListManagedEndpointsRequestRequestTypeDef = TypedDict(
+    "_OptionalListManagedEndpointsRequestRequestTypeDef",
+    {
+        "createdBefore": TimestampTypeDef,
+        "createdAfter": TimestampTypeDef,
+        "types": Sequence[str],
+        "states": Sequence[EndpointStateType],
+        "maxResults": int,
+        "nextToken": str,
+    },
+    total=False,
+)
+
+class ListManagedEndpointsRequestRequestTypeDef(
+    _RequiredListManagedEndpointsRequestRequestTypeDef,
+    _OptionalListManagedEndpointsRequestRequestTypeDef,
+):
+    pass
+
 ListVirtualClustersRequestListVirtualClustersPaginateTypeDef = TypedDict(
     "ListVirtualClustersRequestListVirtualClustersPaginateTypeDef",
     {
         "containerProviderId": str,
         "containerProviderType": Literal["EKS"],
-        "createdAfter": Union[datetime, str],
-        "createdBefore": Union[datetime, str],
+        "createdAfter": TimestampTypeDef,
+        "createdBefore": TimestampTypeDef,
         "states": Sequence[VirtualClusterStateType],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+ListVirtualClustersRequestRequestTypeDef = TypedDict(
+    "ListVirtualClustersRequestRequestTypeDef",
+    {
+        "containerProviderId": str,
+        "containerProviderType": Literal["EKS"],
+        "createdAfter": TimestampTypeDef,
+        "createdBefore": TimestampTypeDef,
+        "states": Sequence[VirtualClusterStateType],
+        "maxResults": int,
+        "nextToken": str,
+    },
+    total=False,
+)
+
 MonitoringConfigurationTypeDef = TypedDict(
     "MonitoringConfigurationTypeDef",
     {
         "persistentAppUI": PersistentAppUIType,
         "cloudWatchMonitoringConfiguration": CloudWatchMonitoringConfigurationTypeDef,
         "s3MonitoringConfiguration": S3MonitoringConfigurationTypeDef,
         "containerLogRotationConfiguration": ContainerLogRotationConfigurationTypeDef,
@@ -731,14 +736,15 @@
 )
 
 class ContainerProviderTypeDef(
     _RequiredContainerProviderTypeDef, _OptionalContainerProviderTypeDef
 ):
     pass
 
+JobDriverUnionTypeDef = Union[JobDriverTypeDef, JobDriverOutputTypeDef]
 ConfigurationOverridesOutputTypeDef = TypedDict(
     "ConfigurationOverridesOutputTypeDef",
     {
         "applicationConfiguration": List["ConfigurationOutputTypeDef"],
         "monitoringConfiguration": MonitoringConfigurationTypeDef,
     },
     total=False,
@@ -853,14 +859,17 @@
         "tags": Dict[str, str],
         "retryPolicyConfiguration": RetryPolicyConfigurationTypeDef,
         "retryPolicyExecution": RetryPolicyExecutionTypeDef,
     },
     total=False,
 )
 
+ConfigurationOverridesUnionTypeDef = Union[
+    ConfigurationOverridesTypeDef, ConfigurationOverridesOutputTypeDef
+]
 _RequiredCreateManagedEndpointRequestRequestTypeDef = TypedDict(
     "_RequiredCreateManagedEndpointRequestRequestTypeDef",
     {
         "name": str,
         "virtualClusterId": str,
         "type": str,
         "releaseLabel": str,
@@ -1049,14 +1058,15 @@
 )
 
 class CreateJobTemplateRequestRequestTypeDef(
     _RequiredCreateJobTemplateRequestRequestTypeDef, _OptionalCreateJobTemplateRequestRequestTypeDef
 ):
     pass
 
+JobTemplateDataUnionTypeDef = Union[JobTemplateDataTypeDef, JobTemplateDataOutputTypeDef]
 DescribeJobTemplateResponseTypeDef = TypedDict(
     "DescribeJobTemplateResponseTypeDef",
     {
         "jobTemplate": JobTemplateTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-emr-containers-1.28.15.post1/mypy_boto3_emr_containers.egg-info/PKG-INFO` & `mypy-boto3-emr-containers-1.28.16/mypy_boto3_emr_containers.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-emr-containers
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.EMRContainers 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.EMRContainers 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 emr-containers type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 emr-containers type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-emr-containers.svg?color=blue)](https://pypi.org/project/mypy-boto3-emr-containers)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-emr-containers)](https://pepy.tech/project/mypy-boto3-emr-containers)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EMRContainers 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers)
+[boto3.EMRContainers 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers)
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
 [mypy-boto3-emr-containers docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/).
 
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
@@ -333,20 +333,20 @@
 )
 
 
 def check_value(value: ContainerProviderTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_emr_containers.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_emr_containers.type_defs import (
     CancelJobRunRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     CertificateTypeDef,
     CloudWatchMonitoringConfigurationTypeDef,
@@ -366,19 +366,16 @@
     SparkSqlJobDriverTypeDef,
     SparkSubmitJobDriverOutputTypeDef,
     SparkSubmitJobDriverTypeDef,
     RetryPolicyConfigurationTypeDef,
     RetryPolicyExecutionTypeDef,
     TemplateParameterConfigurationTypeDef,
     PaginatorConfigTypeDef,
-    ListJobRunsRequestRequestTypeDef,
-    ListJobTemplatesRequestRequestTypeDef,
-    ListManagedEndpointsRequestRequestTypeDef,
+    TimestampTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListVirtualClustersRequestRequestTypeDef,
     S3MonitoringConfigurationTypeDef,
     ParametricCloudWatchMonitoringConfigurationTypeDef,
     ParametricS3MonitoringConfigurationTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     CancelJobRunResponseTypeDef,
     CreateJobTemplateResponseTypeDef,
@@ -390,46 +387,53 @@
     ListTagsForResourceResponseTypeDef,
     StartJobRunResponseTypeDef,
     ContainerInfoTypeDef,
     GetManagedEndpointSessionCredentialsResponseTypeDef,
     JobDriverOutputTypeDef,
     JobDriverTypeDef,
     ListJobRunsRequestListJobRunsPaginateTypeDef,
+    ListJobRunsRequestRequestTypeDef,
     ListJobTemplatesRequestListJobTemplatesPaginateTypeDef,
+    ListJobTemplatesRequestRequestTypeDef,
     ListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef,
+    ListManagedEndpointsRequestRequestTypeDef,
     ListVirtualClustersRequestListVirtualClustersPaginateTypeDef,
+    ListVirtualClustersRequestRequestTypeDef,
     MonitoringConfigurationTypeDef,
     ParametricMonitoringConfigurationTypeDef,
     ContainerProviderTypeDef,
+    JobDriverUnionTypeDef,
     ConfigurationOverridesOutputTypeDef,
     ConfigurationOverridesTypeDef,
     ParametricConfigurationOverridesOutputTypeDef,
     ParametricConfigurationOverridesTypeDef,
     CreateVirtualClusterRequestRequestTypeDef,
     VirtualClusterTypeDef,
     EndpointTypeDef,
     JobRunTypeDef,
+    ConfigurationOverridesUnionTypeDef,
     CreateManagedEndpointRequestRequestTypeDef,
     StartJobRunRequestRequestTypeDef,
     JobTemplateDataOutputTypeDef,
     JobTemplateDataTypeDef,
     DescribeVirtualClusterResponseTypeDef,
     ListVirtualClustersResponseTypeDef,
     DescribeManagedEndpointResponseTypeDef,
     ListManagedEndpointsResponseTypeDef,
     DescribeJobRunResponseTypeDef,
     ListJobRunsResponseTypeDef,
     JobTemplateTypeDef,
     CreateJobTemplateRequestRequestTypeDef,
+    JobTemplateDataUnionTypeDef,
     DescribeJobTemplateResponseTypeDef,
     ListJobTemplatesResponseTypeDef,
 )
 
 
-def get_structure() -> CancelJobRunRequestRequestTypeDef:
+def get_value() -> CancelJobRunRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-emr-containers-1.28.15.post1/mypy_boto3_emr_containers.egg-info/SOURCES.txt` & `mypy-boto3-emr-containers-1.28.16/mypy_boto3_emr_containers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-containers-1.28.15.post1/setup.py` & `mypy-boto3-emr-containers-1.28.16/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-emr-containers",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_emr_containers"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.EMRContainers 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.2"
+        "Type annotations for boto3.EMRContainers 1.28.16 service generated with mypy-boto3-builder"
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
-    keywords="boto3 emr-containers type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 emr-containers type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_emr_containers": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

