# Comparing `tmp/mypy-boto3-pipes-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-pipes-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-pipes-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:54 2023, max compression
+gzip compressed data, was "mypy-boto3-pipes-1.28.16.tar", last modified: Tue Aug  1 11:37:34 2023, max compression
```

## Comparing `mypy-boto3-pipes-1.28.15.post1.tar` & `mypy-boto3-pipes-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:54.677343 mypy-boto3-pipes-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:53:26.000000 mypy-boto3-pipes-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16932 2023-07-29 10:03:54.677343 mypy-boto3-pipes-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15436 2023-07-29 09:53:26.000000 mypy-boto3-pipes-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:54.661343 mypy-boto3-pipes-1.28.15.post1/mypy_boto3_pipes/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-29 09:53:26.000000 mypy-boto3-pipes-1.28.15.post1/mypy_boto3_pipes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-29 09:53:26.000000 mypy-boto3-pipes-1.28.15.post1/mypy_boto3_pipes/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-29 09:53:26.000000 mypy-boto3-pipes-1.28.15.post1/mypy_boto3_pipes/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10101 2023-07-29 09:53:26.000000 mypy-boto3-pipes-1.28.15.post1/mypy_boto3_pipes/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10083 2023-07-29 09:53:26.000000 mypy-boto3-pipes-1.28.15.post1/mypy_boto3_pipes/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-07-29 09:53:26.000000 mypy-boto3-pipes-1.28.15.post1/mypy_boto3_pipes/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10140 2023-07-29 09:53:26.000000 mypy-boto3-pipes-1.28.15.post1/mypy_boto3_pipes/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-07-29 09:53:26.000000 mypy-boto3-pipes-1.28.15.post1/mypy_boto3_pipes/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-07-29 09:53:26.000000 mypy-boto3-pipes-1.28.15.post1/mypy_boto3_pipes/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:53:26.000000 mypy-boto3-pipes-1.28.15.post1/mypy_boto3_pipes/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    42541 2023-07-29 09:53:27.000000 mypy-boto3-pipes-1.28.15.post1/mypy_boto3_pipes/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    42499 2023-07-29 09:53:27.000000 mypy-boto3-pipes-1.28.15.post1/mypy_boto3_pipes/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:53:26.000000 mypy-boto3-pipes-1.28.15.post1/mypy_boto3_pipes/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:54.677343 mypy-boto3-pipes-1.28.15.post1/mypy_boto3_pipes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16932 2023-07-29 10:03:54.000000 mypy-boto3-pipes-1.28.15.post1/mypy_boto3_pipes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-29 10:03:54.000000 mypy-boto3-pipes-1.28.15.post1/mypy_boto3_pipes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:54.000000 mypy-boto3-pipes-1.28.15.post1/mypy_boto3_pipes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:54.000000 mypy-boto3-pipes-1.28.15.post1/mypy_boto3_pipes.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:54.000000 mypy-boto3-pipes-1.28.15.post1/mypy_boto3_pipes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-29 10:03:54.000000 mypy-boto3-pipes-1.28.15.post1/mypy_boto3_pipes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:54.677343 mypy-boto3-pipes-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-07-29 09:53:26.000000 mypy-boto3-pipes-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:34.336786 mypy-boto3-pipes-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:26:26.000000 mypy-boto3-pipes-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17062 2023-08-01 11:37:34.336786 mypy-boto3-pipes-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15575 2023-08-01 11:26:26.000000 mypy-boto3-pipes-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:34.332786 mypy-boto3-pipes-1.28.16/mypy_boto3_pipes/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-08-01 11:26:26.000000 mypy-boto3-pipes-1.28.16/mypy_boto3_pipes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-08-01 11:26:26.000000 mypy-boto3-pipes-1.28.16/mypy_boto3_pipes/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-08-01 11:26:26.000000 mypy-boto3-pipes-1.28.16/mypy_boto3_pipes/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9685 2023-08-01 11:26:26.000000 mypy-boto3-pipes-1.28.16/mypy_boto3_pipes/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9667 2023-08-01 11:26:26.000000 mypy-boto3-pipes-1.28.16/mypy_boto3_pipes/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-08-01 11:26:26.000000 mypy-boto3-pipes-1.28.16/mypy_boto3_pipes/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10140 2023-08-01 11:26:26.000000 mypy-boto3-pipes-1.28.16/mypy_boto3_pipes/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-08-01 11:26:26.000000 mypy-boto3-pipes-1.28.16/mypy_boto3_pipes/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-08-01 11:26:26.000000 mypy-boto3-pipes-1.28.16/mypy_boto3_pipes/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:26:26.000000 mypy-boto3-pipes-1.28.16/mypy_boto3_pipes/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    43068 2023-08-01 11:26:30.000000 mypy-boto3-pipes-1.28.16/mypy_boto3_pipes/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43026 2023-08-01 11:26:27.000000 mypy-boto3-pipes-1.28.16/mypy_boto3_pipes/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:26:26.000000 mypy-boto3-pipes-1.28.16/mypy_boto3_pipes/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:34.336786 mypy-boto3-pipes-1.28.16/mypy_boto3_pipes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17062 2023-08-01 11:37:34.000000 mypy-boto3-pipes-1.28.16/mypy_boto3_pipes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-08-01 11:37:34.000000 mypy-boto3-pipes-1.28.16/mypy_boto3_pipes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:34.000000 mypy-boto3-pipes-1.28.16/mypy_boto3_pipes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:34.000000 mypy-boto3-pipes-1.28.16/mypy_boto3_pipes.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:34.000000 mypy-boto3-pipes-1.28.16/mypy_boto3_pipes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-01 11:37:34.000000 mypy-boto3-pipes-1.28.16/mypy_boto3_pipes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:34.336786 mypy-boto3-pipes-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-08-01 11:26:26.000000 mypy-boto3-pipes-1.28.16/setup.py
```

### Comparing `mypy-boto3-pipes-1.28.15.post1/LICENSE` & `mypy-boto3-pipes-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pipes-1.28.15.post1/PKG-INFO` & `mypy-boto3-pipes-1.28.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-pipes
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.EventBridgePipes 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.EventBridgePipes 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pipes/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 pipes type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 pipes type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-pipes.svg?color=blue)](https://pypi.org/project/mypy-boto3-pipes)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pipes/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-pipes)](https://pepy.tech/project/mypy-boto3-pipes)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EventBridgePipes 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pipes.html#EventBridgePipes)
+[boto3.EventBridgePipes 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pipes.html#EventBridgePipes)
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
 [mypy-boto3-pipes docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pipes/).
 
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
@@ -327,20 +327,20 @@
 )
 
 
 def check_value(value: AssignPublicIpType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_pipes.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_pipes.type_defs import (
     AwsVpcConfigurationOutputTypeDef,
     AwsVpcConfigurationTypeDef,
     BatchArrayPropertiesTypeDef,
     BatchEnvironmentVariableTypeDef,
@@ -362,14 +362,15 @@
     ListPipesRequestRequestTypeDef,
     PipeTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     MQBrokerAccessCredentialsTypeDef,
     MSKAccessCredentialsTypeDef,
     PipeEnrichmentHttpParametersOutputTypeDef,
     PipeEnrichmentHttpParametersTypeDef,
+    TimestampTypeDef,
     PipeSourceSqsQueueParametersTypeDef,
     SelfManagedKafkaAccessConfigurationCredentialsTypeDef,
     SelfManagedKafkaAccessConfigurationVpcOutputTypeDef,
     SelfManagedKafkaAccessConfigurationVpcTypeDef,
     PipeTargetCloudWatchLogsParametersTypeDef,
     PlacementConstraintTypeDef,
     PlacementStrategyTypeDef,
@@ -398,15 +399,14 @@
     DeletePipeResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     StartPipeResponseTypeDef,
     StopPipeResponseTypeDef,
     UpdatePipeResponseTypeDef,
     PipeSourceDynamoDBStreamParametersTypeDef,
     PipeSourceKinesisStreamParametersOutputTypeDef,
-    PipeSourceKinesisStreamParametersTypeDef,
     UpdatePipeSourceDynamoDBStreamParametersTypeDef,
     UpdatePipeSourceKinesisStreamParametersTypeDef,
     EcsContainerOverrideOutputTypeDef,
     EcsContainerOverrideTypeDef,
     FilterCriteriaOutputTypeDef,
     FilterCriteriaTypeDef,
     ListPipesRequestListPipesPaginateTypeDef,
@@ -415,37 +415,41 @@
     PipeSourceRabbitMQBrokerParametersTypeDef,
     UpdatePipeSourceActiveMQBrokerParametersTypeDef,
     UpdatePipeSourceRabbitMQBrokerParametersTypeDef,
     PipeSourceManagedStreamingKafkaParametersTypeDef,
     UpdatePipeSourceManagedStreamingKafkaParametersTypeDef,
     PipeEnrichmentParametersOutputTypeDef,
     PipeEnrichmentParametersTypeDef,
+    PipeSourceKinesisStreamParametersTypeDef,
     PipeSourceSelfManagedKafkaParametersOutputTypeDef,
     PipeSourceSelfManagedKafkaParametersTypeDef,
     UpdatePipeSourceSelfManagedKafkaParametersTypeDef,
     PipeTargetSageMakerPipelineParametersOutputTypeDef,
     PipeTargetSageMakerPipelineParametersTypeDef,
     PipeTargetBatchJobParametersOutputTypeDef,
     PipeTargetBatchJobParametersTypeDef,
     EcsTaskOverrideOutputTypeDef,
     EcsTaskOverrideTypeDef,
+    PipeEnrichmentParametersUnionTypeDef,
     PipeSourceParametersOutputTypeDef,
     PipeSourceParametersTypeDef,
     UpdatePipeSourceParametersTypeDef,
     PipeTargetEcsTaskParametersOutputTypeDef,
     PipeTargetEcsTaskParametersTypeDef,
+    PipeSourceParametersUnionTypeDef,
     PipeTargetParametersOutputTypeDef,
     PipeTargetParametersTypeDef,
     DescribePipeResponseTypeDef,
     CreatePipeRequestRequestTypeDef,
+    PipeTargetParametersUnionTypeDef,
     UpdatePipeRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AwsVpcConfigurationOutputTypeDef:
+def get_value() -> AwsVpcConfigurationOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-pipes-1.28.15.post1/README.md` & `mypy-boto3-pipes-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-pipes.svg?color=blue)](https://pypi.org/project/mypy-boto3-pipes)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pipes/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-pipes)](https://pepy.tech/project/mypy-boto3-pipes)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EventBridgePipes 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pipes.html#EventBridgePipes)
+[boto3.EventBridgePipes 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pipes.html#EventBridgePipes)
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
 [mypy-boto3-pipes docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pipes/).
 
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
@@ -295,20 +295,20 @@
 )
 
 
 def check_value(value: AssignPublicIpType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_pipes.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_pipes.type_defs import (
     AwsVpcConfigurationOutputTypeDef,
     AwsVpcConfigurationTypeDef,
     BatchArrayPropertiesTypeDef,
     BatchEnvironmentVariableTypeDef,
@@ -330,14 +330,15 @@
     ListPipesRequestRequestTypeDef,
     PipeTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     MQBrokerAccessCredentialsTypeDef,
     MSKAccessCredentialsTypeDef,
     PipeEnrichmentHttpParametersOutputTypeDef,
     PipeEnrichmentHttpParametersTypeDef,
+    TimestampTypeDef,
     PipeSourceSqsQueueParametersTypeDef,
     SelfManagedKafkaAccessConfigurationCredentialsTypeDef,
     SelfManagedKafkaAccessConfigurationVpcOutputTypeDef,
     SelfManagedKafkaAccessConfigurationVpcTypeDef,
     PipeTargetCloudWatchLogsParametersTypeDef,
     PlacementConstraintTypeDef,
     PlacementStrategyTypeDef,
@@ -366,15 +367,14 @@
     DeletePipeResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     StartPipeResponseTypeDef,
     StopPipeResponseTypeDef,
     UpdatePipeResponseTypeDef,
     PipeSourceDynamoDBStreamParametersTypeDef,
     PipeSourceKinesisStreamParametersOutputTypeDef,
-    PipeSourceKinesisStreamParametersTypeDef,
     UpdatePipeSourceDynamoDBStreamParametersTypeDef,
     UpdatePipeSourceKinesisStreamParametersTypeDef,
     EcsContainerOverrideOutputTypeDef,
     EcsContainerOverrideTypeDef,
     FilterCriteriaOutputTypeDef,
     FilterCriteriaTypeDef,
     ListPipesRequestListPipesPaginateTypeDef,
@@ -383,37 +383,41 @@
     PipeSourceRabbitMQBrokerParametersTypeDef,
     UpdatePipeSourceActiveMQBrokerParametersTypeDef,
     UpdatePipeSourceRabbitMQBrokerParametersTypeDef,
     PipeSourceManagedStreamingKafkaParametersTypeDef,
     UpdatePipeSourceManagedStreamingKafkaParametersTypeDef,
     PipeEnrichmentParametersOutputTypeDef,
     PipeEnrichmentParametersTypeDef,
+    PipeSourceKinesisStreamParametersTypeDef,
     PipeSourceSelfManagedKafkaParametersOutputTypeDef,
     PipeSourceSelfManagedKafkaParametersTypeDef,
     UpdatePipeSourceSelfManagedKafkaParametersTypeDef,
     PipeTargetSageMakerPipelineParametersOutputTypeDef,
     PipeTargetSageMakerPipelineParametersTypeDef,
     PipeTargetBatchJobParametersOutputTypeDef,
     PipeTargetBatchJobParametersTypeDef,
     EcsTaskOverrideOutputTypeDef,
     EcsTaskOverrideTypeDef,
+    PipeEnrichmentParametersUnionTypeDef,
     PipeSourceParametersOutputTypeDef,
     PipeSourceParametersTypeDef,
     UpdatePipeSourceParametersTypeDef,
     PipeTargetEcsTaskParametersOutputTypeDef,
     PipeTargetEcsTaskParametersTypeDef,
+    PipeSourceParametersUnionTypeDef,
     PipeTargetParametersOutputTypeDef,
     PipeTargetParametersTypeDef,
     DescribePipeResponseTypeDef,
     CreatePipeRequestRequestTypeDef,
+    PipeTargetParametersUnionTypeDef,
     UpdatePipeRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AwsVpcConfigurationOutputTypeDef:
+def get_value() -> AwsVpcConfigurationOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-pipes-1.28.15.post1/mypy_boto3_pipes/__init__.py` & `mypy-boto3-pipes-1.28.16/mypy_boto3_pipes/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pipes-1.28.15.post1/mypy_boto3_pipes/__init__.pyi` & `mypy-boto3-pipes-1.28.16/mypy_boto3_pipes/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pipes-1.28.15.post1/mypy_boto3_pipes/__main__.py` & `mypy-boto3-pipes-1.28.16/mypy_boto3_pipes/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.EventBridgePipes 1.28.15\nVersion:        "
-        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.EventBridgePipes 1.28.16\nVersion:         1.28.16\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pipes//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pipes.html#EventBridgePipes\nOther"
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

### Comparing `mypy-boto3-pipes-1.28.15.post1/mypy_boto3_pipes/client.py` & `mypy-boto3-pipes-1.28.16/mypy_boto3_pipes/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,32 +10,29 @@
     from mypy_boto3_pipes.client import EventBridgePipesClient
 
     session = Session()
     client: EventBridgePipesClient = session.client("pipes")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import PipeStateType, RequestedPipeStateType
 from .paginator import ListPipesPaginator
 from .type_defs import (
     CreatePipeResponseTypeDef,
     DeletePipeResponseTypeDef,
     DescribePipeResponseTypeDef,
     ListPipesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    PipeEnrichmentParametersOutputTypeDef,
-    PipeEnrichmentParametersTypeDef,
-    PipeSourceParametersOutputTypeDef,
-    PipeSourceParametersTypeDef,
-    PipeTargetParametersOutputTypeDef,
-    PipeTargetParametersTypeDef,
+    PipeEnrichmentParametersUnionTypeDef,
+    PipeSourceParametersUnionTypeDef,
+    PipeTargetParametersUnionTypeDef,
     StartPipeResponseTypeDef,
     StopPipeResponseTypeDef,
     UpdatePipeResponseTypeDef,
     UpdatePipeSourceParametersTypeDef,
 )
 
 if sys.version_info >= (3, 9):
@@ -104,24 +101,18 @@
         Name: str,
         RoleArn: str,
         Source: str,
         Target: str,
         Description: str = ...,
         DesiredState: RequestedPipeStateType = ...,
         Enrichment: str = ...,
-        EnrichmentParameters: Union[
-            PipeEnrichmentParametersTypeDef, PipeEnrichmentParametersOutputTypeDef
-        ] = ...,
-        SourceParameters: Union[
-            PipeSourceParametersTypeDef, PipeSourceParametersOutputTypeDef
-        ] = ...,
+        EnrichmentParameters: PipeEnrichmentParametersUnionTypeDef = ...,
+        SourceParameters: PipeSourceParametersUnionTypeDef = ...,
         Tags: Mapping[str, str] = ...,
-        TargetParameters: Union[
-            PipeTargetParametersTypeDef, PipeTargetParametersOutputTypeDef
-        ] = ...
+        TargetParameters: PipeTargetParametersUnionTypeDef = ...
     ) -> CreatePipeResponseTypeDef:
         """
         Create a pipe.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pipes.html#EventBridgePipes.Client.create_pipe)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pipes/client/#create_pipe)
         """
@@ -218,22 +209,18 @@
         self,
         *,
         Name: str,
         RoleArn: str,
         Description: str = ...,
         DesiredState: RequestedPipeStateType = ...,
         Enrichment: str = ...,
-        EnrichmentParameters: Union[
-            PipeEnrichmentParametersTypeDef, PipeEnrichmentParametersOutputTypeDef
-        ] = ...,
+        EnrichmentParameters: PipeEnrichmentParametersUnionTypeDef = ...,
         SourceParameters: UpdatePipeSourceParametersTypeDef = ...,
         Target: str = ...,
-        TargetParameters: Union[
-            PipeTargetParametersTypeDef, PipeTargetParametersOutputTypeDef
-        ] = ...
+        TargetParameters: PipeTargetParametersUnionTypeDef = ...
     ) -> UpdatePipeResponseTypeDef:
         """
         Update an existing pipe.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pipes.html#EventBridgePipes.Client.update_pipe)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pipes/client/#update_pipe)
         """
```

### Comparing `mypy-boto3-pipes-1.28.15.post1/mypy_boto3_pipes/client.pyi` & `mypy-boto3-pipes-1.28.16/mypy_boto3_pipes/client.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -10,32 +10,29 @@
     from mypy_boto3_pipes.client import EventBridgePipesClient
 
     session = Session()
     client: EventBridgePipesClient = session.client("pipes")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import PipeStateType, RequestedPipeStateType
 from .paginator import ListPipesPaginator
 from .type_defs import (
     CreatePipeResponseTypeDef,
     DeletePipeResponseTypeDef,
     DescribePipeResponseTypeDef,
     ListPipesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    PipeEnrichmentParametersOutputTypeDef,
-    PipeEnrichmentParametersTypeDef,
-    PipeSourceParametersOutputTypeDef,
-    PipeSourceParametersTypeDef,
-    PipeTargetParametersOutputTypeDef,
-    PipeTargetParametersTypeDef,
+    PipeEnrichmentParametersUnionTypeDef,
+    PipeSourceParametersUnionTypeDef,
+    PipeTargetParametersUnionTypeDef,
     StartPipeResponseTypeDef,
     StopPipeResponseTypeDef,
     UpdatePipeResponseTypeDef,
     UpdatePipeSourceParametersTypeDef,
 )
 
 if sys.version_info >= (3, 9):
@@ -97,24 +94,18 @@
         Name: str,
         RoleArn: str,
         Source: str,
         Target: str,
         Description: str = ...,
         DesiredState: RequestedPipeStateType = ...,
         Enrichment: str = ...,
-        EnrichmentParameters: Union[
-            PipeEnrichmentParametersTypeDef, PipeEnrichmentParametersOutputTypeDef
-        ] = ...,
-        SourceParameters: Union[
-            PipeSourceParametersTypeDef, PipeSourceParametersOutputTypeDef
-        ] = ...,
+        EnrichmentParameters: PipeEnrichmentParametersUnionTypeDef = ...,
+        SourceParameters: PipeSourceParametersUnionTypeDef = ...,
         Tags: Mapping[str, str] = ...,
-        TargetParameters: Union[
-            PipeTargetParametersTypeDef, PipeTargetParametersOutputTypeDef
-        ] = ...
+        TargetParameters: PipeTargetParametersUnionTypeDef = ...
     ) -> CreatePipeResponseTypeDef:
         """
         Create a pipe.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pipes.html#EventBridgePipes.Client.create_pipe)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pipes/client/#create_pipe)
         """
@@ -201,22 +192,18 @@
         self,
         *,
         Name: str,
         RoleArn: str,
         Description: str = ...,
         DesiredState: RequestedPipeStateType = ...,
         Enrichment: str = ...,
-        EnrichmentParameters: Union[
-            PipeEnrichmentParametersTypeDef, PipeEnrichmentParametersOutputTypeDef
-        ] = ...,
+        EnrichmentParameters: PipeEnrichmentParametersUnionTypeDef = ...,
         SourceParameters: UpdatePipeSourceParametersTypeDef = ...,
         Target: str = ...,
-        TargetParameters: Union[
-            PipeTargetParametersTypeDef, PipeTargetParametersOutputTypeDef
-        ] = ...
+        TargetParameters: PipeTargetParametersUnionTypeDef = ...
     ) -> UpdatePipeResponseTypeDef:
         """
         Update an existing pipe.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pipes.html#EventBridgePipes.Client.update_pipe)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pipes/client/#update_pipe)
         """
```

### Comparing `mypy-boto3-pipes-1.28.15.post1/mypy_boto3_pipes/literals.py` & `mypy-boto3-pipes-1.28.16/mypy_boto3_pipes/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pipes-1.28.15.post1/mypy_boto3_pipes/literals.pyi` & `mypy-boto3-pipes-1.28.16/mypy_boto3_pipes/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pipes-1.28.15.post1/mypy_boto3_pipes/paginator.py` & `mypy-boto3-pipes-1.28.16/mypy_boto3_pipes/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pipes-1.28.15.post1/mypy_boto3_pipes/paginator.pyi` & `mypy-boto3-pipes-1.28.16/mypy_boto3_pipes/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pipes-1.28.15.post1/mypy_boto3_pipes/type_defs.py` & `mypy-boto3-pipes-1.28.16/mypy_boto3_pipes/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pipes/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_pipes.type_defs import AwsVpcConfigurationOutputTypeDef
 
-    data: AwsVpcConfigurationOutputTypeDef = {...}
+    data: AwsVpcConfigurationOutputTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -66,14 +66,15 @@
     "ListPipesRequestRequestTypeDef",
     "PipeTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "MQBrokerAccessCredentialsTypeDef",
     "MSKAccessCredentialsTypeDef",
     "PipeEnrichmentHttpParametersOutputTypeDef",
     "PipeEnrichmentHttpParametersTypeDef",
+    "TimestampTypeDef",
     "PipeSourceSqsQueueParametersTypeDef",
     "SelfManagedKafkaAccessConfigurationCredentialsTypeDef",
     "SelfManagedKafkaAccessConfigurationVpcOutputTypeDef",
     "SelfManagedKafkaAccessConfigurationVpcTypeDef",
     "PipeTargetCloudWatchLogsParametersTypeDef",
     "PlacementConstraintTypeDef",
     "PlacementStrategyTypeDef",
@@ -102,15 +103,14 @@
     "DeletePipeResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "StartPipeResponseTypeDef",
     "StopPipeResponseTypeDef",
     "UpdatePipeResponseTypeDef",
     "PipeSourceDynamoDBStreamParametersTypeDef",
     "PipeSourceKinesisStreamParametersOutputTypeDef",
-    "PipeSourceKinesisStreamParametersTypeDef",
     "UpdatePipeSourceDynamoDBStreamParametersTypeDef",
     "UpdatePipeSourceKinesisStreamParametersTypeDef",
     "EcsContainerOverrideOutputTypeDef",
     "EcsContainerOverrideTypeDef",
     "FilterCriteriaOutputTypeDef",
     "FilterCriteriaTypeDef",
     "ListPipesRequestListPipesPaginateTypeDef",
@@ -119,32 +119,36 @@
     "PipeSourceRabbitMQBrokerParametersTypeDef",
     "UpdatePipeSourceActiveMQBrokerParametersTypeDef",
     "UpdatePipeSourceRabbitMQBrokerParametersTypeDef",
     "PipeSourceManagedStreamingKafkaParametersTypeDef",
     "UpdatePipeSourceManagedStreamingKafkaParametersTypeDef",
     "PipeEnrichmentParametersOutputTypeDef",
     "PipeEnrichmentParametersTypeDef",
+    "PipeSourceKinesisStreamParametersTypeDef",
     "PipeSourceSelfManagedKafkaParametersOutputTypeDef",
     "PipeSourceSelfManagedKafkaParametersTypeDef",
     "UpdatePipeSourceSelfManagedKafkaParametersTypeDef",
     "PipeTargetSageMakerPipelineParametersOutputTypeDef",
     "PipeTargetSageMakerPipelineParametersTypeDef",
     "PipeTargetBatchJobParametersOutputTypeDef",
     "PipeTargetBatchJobParametersTypeDef",
     "EcsTaskOverrideOutputTypeDef",
     "EcsTaskOverrideTypeDef",
+    "PipeEnrichmentParametersUnionTypeDef",
     "PipeSourceParametersOutputTypeDef",
     "PipeSourceParametersTypeDef",
     "UpdatePipeSourceParametersTypeDef",
     "PipeTargetEcsTaskParametersOutputTypeDef",
     "PipeTargetEcsTaskParametersTypeDef",
+    "PipeSourceParametersUnionTypeDef",
     "PipeTargetParametersOutputTypeDef",
     "PipeTargetParametersTypeDef",
     "DescribePipeResponseTypeDef",
     "CreatePipeRequestRequestTypeDef",
+    "PipeTargetParametersUnionTypeDef",
     "UpdatePipeRequestRequestTypeDef",
 )
 
 _RequiredAwsVpcConfigurationOutputTypeDef = TypedDict(
     "_RequiredAwsVpcConfigurationOutputTypeDef",
     {
         "Subnets": List[str],
@@ -415,14 +419,15 @@
         "HeaderParameters": Mapping[str, str],
         "PathParameterValues": Sequence[str],
         "QueryStringParameters": Mapping[str, str],
     },
     total=False,
 )
 
+TimestampTypeDef = Union[datetime, str]
 PipeSourceSqsQueueParametersTypeDef = TypedDict(
     "PipeSourceSqsQueueParametersTypeDef",
     {
         "BatchSize": int,
         "MaximumBatchingWindowInSeconds": int,
     },
     total=False,
@@ -831,43 +836,14 @@
 class PipeSourceKinesisStreamParametersOutputTypeDef(
     _RequiredPipeSourceKinesisStreamParametersOutputTypeDef,
     _OptionalPipeSourceKinesisStreamParametersOutputTypeDef,
 ):
     pass
 
 
-_RequiredPipeSourceKinesisStreamParametersTypeDef = TypedDict(
-    "_RequiredPipeSourceKinesisStreamParametersTypeDef",
-    {
-        "StartingPosition": KinesisStreamStartPositionType,
-    },
-)
-_OptionalPipeSourceKinesisStreamParametersTypeDef = TypedDict(
-    "_OptionalPipeSourceKinesisStreamParametersTypeDef",
-    {
-        "BatchSize": int,
-        "DeadLetterConfig": DeadLetterConfigTypeDef,
-        "MaximumBatchingWindowInSeconds": int,
-        "MaximumRecordAgeInSeconds": int,
-        "MaximumRetryAttempts": int,
-        "OnPartialBatchItemFailure": Literal["AUTOMATIC_BISECT"],
-        "ParallelizationFactor": int,
-        "StartingPositionTimestamp": Union[datetime, str],
-    },
-    total=False,
-)
-
-
-class PipeSourceKinesisStreamParametersTypeDef(
-    _RequiredPipeSourceKinesisStreamParametersTypeDef,
-    _OptionalPipeSourceKinesisStreamParametersTypeDef,
-):
-    pass
-
-
 UpdatePipeSourceDynamoDBStreamParametersTypeDef = TypedDict(
     "UpdatePipeSourceDynamoDBStreamParametersTypeDef",
     {
         "BatchSize": int,
         "DeadLetterConfig": DeadLetterConfigTypeDef,
         "MaximumBatchingWindowInSeconds": int,
         "MaximumRecordAgeInSeconds": int,
@@ -1105,14 +1081,43 @@
     {
         "HttpParameters": PipeEnrichmentHttpParametersTypeDef,
         "InputTemplate": str,
     },
     total=False,
 )
 
+_RequiredPipeSourceKinesisStreamParametersTypeDef = TypedDict(
+    "_RequiredPipeSourceKinesisStreamParametersTypeDef",
+    {
+        "StartingPosition": KinesisStreamStartPositionType,
+    },
+)
+_OptionalPipeSourceKinesisStreamParametersTypeDef = TypedDict(
+    "_OptionalPipeSourceKinesisStreamParametersTypeDef",
+    {
+        "BatchSize": int,
+        "DeadLetterConfig": DeadLetterConfigTypeDef,
+        "MaximumBatchingWindowInSeconds": int,
+        "MaximumRecordAgeInSeconds": int,
+        "MaximumRetryAttempts": int,
+        "OnPartialBatchItemFailure": Literal["AUTOMATIC_BISECT"],
+        "ParallelizationFactor": int,
+        "StartingPositionTimestamp": TimestampTypeDef,
+    },
+    total=False,
+)
+
+
+class PipeSourceKinesisStreamParametersTypeDef(
+    _RequiredPipeSourceKinesisStreamParametersTypeDef,
+    _OptionalPipeSourceKinesisStreamParametersTypeDef,
+):
+    pass
+
+
 _RequiredPipeSourceSelfManagedKafkaParametersOutputTypeDef = TypedDict(
     "_RequiredPipeSourceSelfManagedKafkaParametersOutputTypeDef",
     {
         "TopicName": str,
     },
 )
 _OptionalPipeSourceSelfManagedKafkaParametersOutputTypeDef = TypedDict(
@@ -1272,14 +1277,17 @@
         "InferenceAcceleratorOverrides": Sequence[EcsInferenceAcceleratorOverrideTypeDef],
         "Memory": str,
         "TaskRoleArn": str,
     },
     total=False,
 )
 
+PipeEnrichmentParametersUnionTypeDef = Union[
+    PipeEnrichmentParametersTypeDef, PipeEnrichmentParametersOutputTypeDef
+]
 PipeSourceParametersOutputTypeDef = TypedDict(
     "PipeSourceParametersOutputTypeDef",
     {
         "ActiveMQBrokerParameters": PipeSourceActiveMQBrokerParametersTypeDef,
         "DynamoDBStreamParameters": PipeSourceDynamoDBStreamParametersTypeDef,
         "FilterCriteria": FilterCriteriaOutputTypeDef,
         "KinesisStreamParameters": PipeSourceKinesisStreamParametersOutputTypeDef,
@@ -1386,14 +1394,17 @@
 
 class PipeTargetEcsTaskParametersTypeDef(
     _RequiredPipeTargetEcsTaskParametersTypeDef, _OptionalPipeTargetEcsTaskParametersTypeDef
 ):
     pass
 
 
+PipeSourceParametersUnionTypeDef = Union[
+    PipeSourceParametersTypeDef, PipeSourceParametersOutputTypeDef
+]
 PipeTargetParametersOutputTypeDef = TypedDict(
     "PipeTargetParametersOutputTypeDef",
     {
         "BatchJobParameters": PipeTargetBatchJobParametersOutputTypeDef,
         "CloudWatchLogsParameters": PipeTargetCloudWatchLogsParametersTypeDef,
         "EcsTaskParameters": PipeTargetEcsTaskParametersOutputTypeDef,
         "EventBridgeEventBusParameters": PipeTargetEventBridgeEventBusParametersOutputTypeDef,
@@ -1477,14 +1488,17 @@
 
 class CreatePipeRequestRequestTypeDef(
     _RequiredCreatePipeRequestRequestTypeDef, _OptionalCreatePipeRequestRequestTypeDef
 ):
     pass
 
 
+PipeTargetParametersUnionTypeDef = Union[
+    PipeTargetParametersTypeDef, PipeTargetParametersOutputTypeDef
+]
 _RequiredUpdatePipeRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePipeRequestRequestTypeDef",
     {
         "Name": str,
         "RoleArn": str,
     },
 )
```

### Comparing `mypy-boto3-pipes-1.28.15.post1/mypy_boto3_pipes/type_defs.pyi` & `mypy-boto3-pipes-1.28.16/mypy_boto3_pipes/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pipes/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_pipes.type_defs import AwsVpcConfigurationOutputTypeDef
 
-    data: AwsVpcConfigurationOutputTypeDef = {...}
+    data: AwsVpcConfigurationOutputTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -65,14 +65,15 @@
     "ListPipesRequestRequestTypeDef",
     "PipeTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "MQBrokerAccessCredentialsTypeDef",
     "MSKAccessCredentialsTypeDef",
     "PipeEnrichmentHttpParametersOutputTypeDef",
     "PipeEnrichmentHttpParametersTypeDef",
+    "TimestampTypeDef",
     "PipeSourceSqsQueueParametersTypeDef",
     "SelfManagedKafkaAccessConfigurationCredentialsTypeDef",
     "SelfManagedKafkaAccessConfigurationVpcOutputTypeDef",
     "SelfManagedKafkaAccessConfigurationVpcTypeDef",
     "PipeTargetCloudWatchLogsParametersTypeDef",
     "PlacementConstraintTypeDef",
     "PlacementStrategyTypeDef",
@@ -101,15 +102,14 @@
     "DeletePipeResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "StartPipeResponseTypeDef",
     "StopPipeResponseTypeDef",
     "UpdatePipeResponseTypeDef",
     "PipeSourceDynamoDBStreamParametersTypeDef",
     "PipeSourceKinesisStreamParametersOutputTypeDef",
-    "PipeSourceKinesisStreamParametersTypeDef",
     "UpdatePipeSourceDynamoDBStreamParametersTypeDef",
     "UpdatePipeSourceKinesisStreamParametersTypeDef",
     "EcsContainerOverrideOutputTypeDef",
     "EcsContainerOverrideTypeDef",
     "FilterCriteriaOutputTypeDef",
     "FilterCriteriaTypeDef",
     "ListPipesRequestListPipesPaginateTypeDef",
@@ -118,32 +118,36 @@
     "PipeSourceRabbitMQBrokerParametersTypeDef",
     "UpdatePipeSourceActiveMQBrokerParametersTypeDef",
     "UpdatePipeSourceRabbitMQBrokerParametersTypeDef",
     "PipeSourceManagedStreamingKafkaParametersTypeDef",
     "UpdatePipeSourceManagedStreamingKafkaParametersTypeDef",
     "PipeEnrichmentParametersOutputTypeDef",
     "PipeEnrichmentParametersTypeDef",
+    "PipeSourceKinesisStreamParametersTypeDef",
     "PipeSourceSelfManagedKafkaParametersOutputTypeDef",
     "PipeSourceSelfManagedKafkaParametersTypeDef",
     "UpdatePipeSourceSelfManagedKafkaParametersTypeDef",
     "PipeTargetSageMakerPipelineParametersOutputTypeDef",
     "PipeTargetSageMakerPipelineParametersTypeDef",
     "PipeTargetBatchJobParametersOutputTypeDef",
     "PipeTargetBatchJobParametersTypeDef",
     "EcsTaskOverrideOutputTypeDef",
     "EcsTaskOverrideTypeDef",
+    "PipeEnrichmentParametersUnionTypeDef",
     "PipeSourceParametersOutputTypeDef",
     "PipeSourceParametersTypeDef",
     "UpdatePipeSourceParametersTypeDef",
     "PipeTargetEcsTaskParametersOutputTypeDef",
     "PipeTargetEcsTaskParametersTypeDef",
+    "PipeSourceParametersUnionTypeDef",
     "PipeTargetParametersOutputTypeDef",
     "PipeTargetParametersTypeDef",
     "DescribePipeResponseTypeDef",
     "CreatePipeRequestRequestTypeDef",
+    "PipeTargetParametersUnionTypeDef",
     "UpdatePipeRequestRequestTypeDef",
 )
 
 _RequiredAwsVpcConfigurationOutputTypeDef = TypedDict(
     "_RequiredAwsVpcConfigurationOutputTypeDef",
     {
         "Subnets": List[str],
@@ -408,14 +412,15 @@
         "HeaderParameters": Mapping[str, str],
         "PathParameterValues": Sequence[str],
         "QueryStringParameters": Mapping[str, str],
     },
     total=False,
 )
 
+TimestampTypeDef = Union[datetime, str]
 PipeSourceSqsQueueParametersTypeDef = TypedDict(
     "PipeSourceSqsQueueParametersTypeDef",
     {
         "BatchSize": int,
         "MaximumBatchingWindowInSeconds": int,
     },
     total=False,
@@ -816,41 +821,14 @@
 
 class PipeSourceKinesisStreamParametersOutputTypeDef(
     _RequiredPipeSourceKinesisStreamParametersOutputTypeDef,
     _OptionalPipeSourceKinesisStreamParametersOutputTypeDef,
 ):
     pass
 
-_RequiredPipeSourceKinesisStreamParametersTypeDef = TypedDict(
-    "_RequiredPipeSourceKinesisStreamParametersTypeDef",
-    {
-        "StartingPosition": KinesisStreamStartPositionType,
-    },
-)
-_OptionalPipeSourceKinesisStreamParametersTypeDef = TypedDict(
-    "_OptionalPipeSourceKinesisStreamParametersTypeDef",
-    {
-        "BatchSize": int,
-        "DeadLetterConfig": DeadLetterConfigTypeDef,
-        "MaximumBatchingWindowInSeconds": int,
-        "MaximumRecordAgeInSeconds": int,
-        "MaximumRetryAttempts": int,
-        "OnPartialBatchItemFailure": Literal["AUTOMATIC_BISECT"],
-        "ParallelizationFactor": int,
-        "StartingPositionTimestamp": Union[datetime, str],
-    },
-    total=False,
-)
-
-class PipeSourceKinesisStreamParametersTypeDef(
-    _RequiredPipeSourceKinesisStreamParametersTypeDef,
-    _OptionalPipeSourceKinesisStreamParametersTypeDef,
-):
-    pass
-
 UpdatePipeSourceDynamoDBStreamParametersTypeDef = TypedDict(
     "UpdatePipeSourceDynamoDBStreamParametersTypeDef",
     {
         "BatchSize": int,
         "DeadLetterConfig": DeadLetterConfigTypeDef,
         "MaximumBatchingWindowInSeconds": int,
         "MaximumRecordAgeInSeconds": int,
@@ -1078,14 +1056,41 @@
     {
         "HttpParameters": PipeEnrichmentHttpParametersTypeDef,
         "InputTemplate": str,
     },
     total=False,
 )
 
+_RequiredPipeSourceKinesisStreamParametersTypeDef = TypedDict(
+    "_RequiredPipeSourceKinesisStreamParametersTypeDef",
+    {
+        "StartingPosition": KinesisStreamStartPositionType,
+    },
+)
+_OptionalPipeSourceKinesisStreamParametersTypeDef = TypedDict(
+    "_OptionalPipeSourceKinesisStreamParametersTypeDef",
+    {
+        "BatchSize": int,
+        "DeadLetterConfig": DeadLetterConfigTypeDef,
+        "MaximumBatchingWindowInSeconds": int,
+        "MaximumRecordAgeInSeconds": int,
+        "MaximumRetryAttempts": int,
+        "OnPartialBatchItemFailure": Literal["AUTOMATIC_BISECT"],
+        "ParallelizationFactor": int,
+        "StartingPositionTimestamp": TimestampTypeDef,
+    },
+    total=False,
+)
+
+class PipeSourceKinesisStreamParametersTypeDef(
+    _RequiredPipeSourceKinesisStreamParametersTypeDef,
+    _OptionalPipeSourceKinesisStreamParametersTypeDef,
+):
+    pass
+
 _RequiredPipeSourceSelfManagedKafkaParametersOutputTypeDef = TypedDict(
     "_RequiredPipeSourceSelfManagedKafkaParametersOutputTypeDef",
     {
         "TopicName": str,
     },
 )
 _OptionalPipeSourceSelfManagedKafkaParametersOutputTypeDef = TypedDict(
@@ -1237,14 +1242,17 @@
         "InferenceAcceleratorOverrides": Sequence[EcsInferenceAcceleratorOverrideTypeDef],
         "Memory": str,
         "TaskRoleArn": str,
     },
     total=False,
 )
 
+PipeEnrichmentParametersUnionTypeDef = Union[
+    PipeEnrichmentParametersTypeDef, PipeEnrichmentParametersOutputTypeDef
+]
 PipeSourceParametersOutputTypeDef = TypedDict(
     "PipeSourceParametersOutputTypeDef",
     {
         "ActiveMQBrokerParameters": PipeSourceActiveMQBrokerParametersTypeDef,
         "DynamoDBStreamParameters": PipeSourceDynamoDBStreamParametersTypeDef,
         "FilterCriteria": FilterCriteriaOutputTypeDef,
         "KinesisStreamParameters": PipeSourceKinesisStreamParametersOutputTypeDef,
@@ -1347,14 +1355,17 @@
 )
 
 class PipeTargetEcsTaskParametersTypeDef(
     _RequiredPipeTargetEcsTaskParametersTypeDef, _OptionalPipeTargetEcsTaskParametersTypeDef
 ):
     pass
 
+PipeSourceParametersUnionTypeDef = Union[
+    PipeSourceParametersTypeDef, PipeSourceParametersOutputTypeDef
+]
 PipeTargetParametersOutputTypeDef = TypedDict(
     "PipeTargetParametersOutputTypeDef",
     {
         "BatchJobParameters": PipeTargetBatchJobParametersOutputTypeDef,
         "CloudWatchLogsParameters": PipeTargetCloudWatchLogsParametersTypeDef,
         "EcsTaskParameters": PipeTargetEcsTaskParametersOutputTypeDef,
         "EventBridgeEventBusParameters": PipeTargetEventBridgeEventBusParametersOutputTypeDef,
@@ -1436,14 +1447,17 @@
 )
 
 class CreatePipeRequestRequestTypeDef(
     _RequiredCreatePipeRequestRequestTypeDef, _OptionalCreatePipeRequestRequestTypeDef
 ):
     pass
 
+PipeTargetParametersUnionTypeDef = Union[
+    PipeTargetParametersTypeDef, PipeTargetParametersOutputTypeDef
+]
 _RequiredUpdatePipeRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePipeRequestRequestTypeDef",
     {
         "Name": str,
         "RoleArn": str,
     },
 )
```

### Comparing `mypy-boto3-pipes-1.28.15.post1/mypy_boto3_pipes.egg-info/PKG-INFO` & `mypy-boto3-pipes-1.28.16/mypy_boto3_pipes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-pipes
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.EventBridgePipes 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.EventBridgePipes 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pipes/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 pipes type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 pipes type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-pipes.svg?color=blue)](https://pypi.org/project/mypy-boto3-pipes)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pipes/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-pipes)](https://pepy.tech/project/mypy-boto3-pipes)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EventBridgePipes 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pipes.html#EventBridgePipes)
+[boto3.EventBridgePipes 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pipes.html#EventBridgePipes)
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
 [mypy-boto3-pipes docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pipes/).
 
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
@@ -327,20 +327,20 @@
 )
 
 
 def check_value(value: AssignPublicIpType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_pipes.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_pipes.type_defs import (
     AwsVpcConfigurationOutputTypeDef,
     AwsVpcConfigurationTypeDef,
     BatchArrayPropertiesTypeDef,
     BatchEnvironmentVariableTypeDef,
@@ -362,14 +362,15 @@
     ListPipesRequestRequestTypeDef,
     PipeTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     MQBrokerAccessCredentialsTypeDef,
     MSKAccessCredentialsTypeDef,
     PipeEnrichmentHttpParametersOutputTypeDef,
     PipeEnrichmentHttpParametersTypeDef,
+    TimestampTypeDef,
     PipeSourceSqsQueueParametersTypeDef,
     SelfManagedKafkaAccessConfigurationCredentialsTypeDef,
     SelfManagedKafkaAccessConfigurationVpcOutputTypeDef,
     SelfManagedKafkaAccessConfigurationVpcTypeDef,
     PipeTargetCloudWatchLogsParametersTypeDef,
     PlacementConstraintTypeDef,
     PlacementStrategyTypeDef,
@@ -398,15 +399,14 @@
     DeletePipeResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     StartPipeResponseTypeDef,
     StopPipeResponseTypeDef,
     UpdatePipeResponseTypeDef,
     PipeSourceDynamoDBStreamParametersTypeDef,
     PipeSourceKinesisStreamParametersOutputTypeDef,
-    PipeSourceKinesisStreamParametersTypeDef,
     UpdatePipeSourceDynamoDBStreamParametersTypeDef,
     UpdatePipeSourceKinesisStreamParametersTypeDef,
     EcsContainerOverrideOutputTypeDef,
     EcsContainerOverrideTypeDef,
     FilterCriteriaOutputTypeDef,
     FilterCriteriaTypeDef,
     ListPipesRequestListPipesPaginateTypeDef,
@@ -415,37 +415,41 @@
     PipeSourceRabbitMQBrokerParametersTypeDef,
     UpdatePipeSourceActiveMQBrokerParametersTypeDef,
     UpdatePipeSourceRabbitMQBrokerParametersTypeDef,
     PipeSourceManagedStreamingKafkaParametersTypeDef,
     UpdatePipeSourceManagedStreamingKafkaParametersTypeDef,
     PipeEnrichmentParametersOutputTypeDef,
     PipeEnrichmentParametersTypeDef,
+    PipeSourceKinesisStreamParametersTypeDef,
     PipeSourceSelfManagedKafkaParametersOutputTypeDef,
     PipeSourceSelfManagedKafkaParametersTypeDef,
     UpdatePipeSourceSelfManagedKafkaParametersTypeDef,
     PipeTargetSageMakerPipelineParametersOutputTypeDef,
     PipeTargetSageMakerPipelineParametersTypeDef,
     PipeTargetBatchJobParametersOutputTypeDef,
     PipeTargetBatchJobParametersTypeDef,
     EcsTaskOverrideOutputTypeDef,
     EcsTaskOverrideTypeDef,
+    PipeEnrichmentParametersUnionTypeDef,
     PipeSourceParametersOutputTypeDef,
     PipeSourceParametersTypeDef,
     UpdatePipeSourceParametersTypeDef,
     PipeTargetEcsTaskParametersOutputTypeDef,
     PipeTargetEcsTaskParametersTypeDef,
+    PipeSourceParametersUnionTypeDef,
     PipeTargetParametersOutputTypeDef,
     PipeTargetParametersTypeDef,
     DescribePipeResponseTypeDef,
     CreatePipeRequestRequestTypeDef,
+    PipeTargetParametersUnionTypeDef,
     UpdatePipeRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AwsVpcConfigurationOutputTypeDef:
+def get_value() -> AwsVpcConfigurationOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-pipes-1.28.15.post1/mypy_boto3_pipes.egg-info/SOURCES.txt` & `mypy-boto3-pipes-1.28.16/mypy_boto3_pipes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pipes-1.28.15.post1/setup.py` & `mypy-boto3-pipes-1.28.16/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-pipes",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_pipes"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.EventBridgePipes 1.28.15 service generated with"
-        " mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.EventBridgePipes 1.28.16 service generated with"
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
-    keywords="boto3 pipes type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 pipes type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_pipes": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pipes/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

