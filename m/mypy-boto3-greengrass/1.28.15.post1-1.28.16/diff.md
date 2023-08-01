# Comparing `tmp/mypy-boto3-greengrass-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-greengrass-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-greengrass-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:13 2023, max compression
+gzip compressed data, was "mypy-boto3-greengrass-1.28.16.tar", last modified: Tue Aug  1 11:36:52 2023, max compression
```

## Comparing `mypy-boto3-greengrass-1.28.15.post1.tar` & `mypy-boto3-greengrass-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:13.117168 mypy-boto3-greengrass-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:46:33.000000 mypy-boto3-greengrass-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    28281 2023-07-29 10:03:13.117168 mypy-boto3-greengrass-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    26776 2023-07-29 09:46:33.000000 mypy-boto3-greengrass-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:13.097167 mypy-boto3-greengrass-1.28.15.post1/mypy_boto3_greengrass/
--rw-r--r--   0 runner    (1001) docker     (123)     5256 2023-07-29 09:46:33.000000 mypy-boto3-greengrass-1.28.15.post1/mypy_boto3_greengrass/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-07-29 09:46:33.000000 mypy-boto3-greengrass-1.28.15.post1/mypy_boto3_greengrass/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-29 09:46:33.000000 mypy-boto3-greengrass-1.28.15.post1/mypy_boto3_greengrass/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    69678 2023-07-29 09:46:33.000000 mypy-boto3-greengrass-1.28.15.post1/mypy_boto3_greengrass/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    69560 2023-07-29 09:46:33.000000 mypy-boto3-greengrass-1.28.15.post1/mypy_boto3_greengrass/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12358 2023-07-29 09:46:34.000000 mypy-boto3-greengrass-1.28.15.post1/mypy_boto3_greengrass/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12356 2023-07-29 09:46:33.000000 mypy-boto3-greengrass-1.28.15.post1/mypy_boto3_greengrass/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    23035 2023-07-29 09:46:33.000000 mypy-boto3-greengrass-1.28.15.post1/mypy_boto3_greengrass/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    23014 2023-07-29 09:46:33.000000 mypy-boto3-greengrass-1.28.15.post1/mypy_boto3_greengrass/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:46:33.000000 mypy-boto3-greengrass-1.28.15.post1/mypy_boto3_greengrass/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    93410 2023-07-29 09:46:38.000000 mypy-boto3-greengrass-1.28.15.post1/mypy_boto3_greengrass/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    93289 2023-07-29 09:46:37.000000 mypy-boto3-greengrass-1.28.15.post1/mypy_boto3_greengrass/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:46:33.000000 mypy-boto3-greengrass-1.28.15.post1/mypy_boto3_greengrass/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:13.117168 mypy-boto3-greengrass-1.28.15.post1/mypy_boto3_greengrass.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    28281 2023-07-29 10:03:12.000000 mypy-boto3-greengrass-1.28.15.post1/mypy_boto3_greengrass.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-29 10:03:12.000000 mypy-boto3-greengrass-1.28.15.post1/mypy_boto3_greengrass.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:12.000000 mypy-boto3-greengrass-1.28.15.post1/mypy_boto3_greengrass.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:12.000000 mypy-boto3-greengrass-1.28.15.post1/mypy_boto3_greengrass.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:12.000000 mypy-boto3-greengrass-1.28.15.post1/mypy_boto3_greengrass.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-29 10:03:12.000000 mypy-boto3-greengrass-1.28.15.post1/mypy_boto3_greengrass.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:13.117168 mypy-boto3-greengrass-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-07-29 09:46:32.000000 mypy-boto3-greengrass-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:52.776880 mypy-boto3-greengrass-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:19:10.000000 mypy-boto3-greengrass-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    28648 2023-08-01 11:36:52.776880 mypy-boto3-greengrass-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    27152 2023-08-01 11:19:10.000000 mypy-boto3-greengrass-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:52.764880 mypy-boto3-greengrass-1.28.16/mypy_boto3_greengrass/
+-rw-r--r--   0 runner    (1001) docker     (123)     5256 2023-08-01 11:19:10.000000 mypy-boto3-greengrass-1.28.16/mypy_boto3_greengrass/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-08-01 11:19:10.000000 mypy-boto3-greengrass-1.28.16/mypy_boto3_greengrass/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-08-01 11:19:10.000000 mypy-boto3-greengrass-1.28.16/mypy_boto3_greengrass/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68813 2023-08-01 11:19:12.000000 mypy-boto3-greengrass-1.28.16/mypy_boto3_greengrass/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68695 2023-08-01 11:19:10.000000 mypy-boto3-greengrass-1.28.16/mypy_boto3_greengrass/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12358 2023-08-01 11:19:13.000000 mypy-boto3-greengrass-1.28.16/mypy_boto3_greengrass/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12356 2023-08-01 11:19:13.000000 mypy-boto3-greengrass-1.28.16/mypy_boto3_greengrass/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    23035 2023-08-01 11:19:13.000000 mypy-boto3-greengrass-1.28.16/mypy_boto3_greengrass/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23014 2023-08-01 11:19:13.000000 mypy-boto3-greengrass-1.28.16/mypy_boto3_greengrass/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:19:10.000000 mypy-boto3-greengrass-1.28.16/mypy_boto3_greengrass/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    94811 2023-08-01 11:19:15.000000 mypy-boto3-greengrass-1.28.16/mypy_boto3_greengrass/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    94691 2023-08-01 11:19:14.000000 mypy-boto3-greengrass-1.28.16/mypy_boto3_greengrass/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:19:10.000000 mypy-boto3-greengrass-1.28.16/mypy_boto3_greengrass/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:52.776880 mypy-boto3-greengrass-1.28.16/mypy_boto3_greengrass.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    28648 2023-08-01 11:36:52.000000 mypy-boto3-greengrass-1.28.16/mypy_boto3_greengrass.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-08-01 11:36:52.000000 mypy-boto3-greengrass-1.28.16/mypy_boto3_greengrass.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:52.000000 mypy-boto3-greengrass-1.28.16/mypy_boto3_greengrass.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:52.000000 mypy-boto3-greengrass-1.28.16/mypy_boto3_greengrass.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:52.000000 mypy-boto3-greengrass-1.28.16/mypy_boto3_greengrass.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-01 11:36:52.000000 mypy-boto3-greengrass-1.28.16/mypy_boto3_greengrass.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:52.776880 mypy-boto3-greengrass-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-08-01 11:19:10.000000 mypy-boto3-greengrass-1.28.16/setup.py
```

### Comparing `mypy-boto3-greengrass-1.28.15.post1/LICENSE` & `mypy-boto3-greengrass-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-greengrass-1.28.15.post1/PKG-INFO` & `mypy-boto3-greengrass-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,61 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-greengrass
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.Greengrass 1.28.15 service generated with mypy-boto3-builder 7.16.2
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 greengrass type-annotations boto3-stubs mypy typeshed autocomplete
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <a id="mypy-boto3-greengrass"></a>
 
 # mypy-boto3-greengrass
 
 [![PyPI - mypy-boto3-greengrass](https://img.shields.io/pypi/v/mypy-boto3-greengrass.svg?color=blue)](https://pypi.org/project/mypy-boto3-greengrass)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-greengrass.svg?color=blue)](https://pypi.org/project/mypy-boto3-greengrass)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-greengrass)](https://pepy.tech/project/mypy-boto3-greengrass)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Greengrass 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass)
+[boto3.Greengrass 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass)
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
 [mypy-boto3-greengrass docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/).
 
 See how it helps to find and fix potential bugs:
 
@@ -74,15 +42,15 @@
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
@@ -413,20 +381,20 @@
 )
 
 
 def check_value(value: BulkDeploymentStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_greengrass.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_greengrass.type_defs import (
     AssociateRoleToGroupRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     AssociateServiceRoleToAccountRequestRequestTypeDef,
     BulkDeploymentMetricsTypeDef,
@@ -570,15 +538,15 @@
     GetBulkDeploymentStatusResponseTypeDef,
     GetDeploymentStatusResponseTypeDef,
     ListBulkDeploymentsResponseTypeDef,
     GetConnectivityInfoResponseTypeDef,
     UpdateConnectivityInfoRequestRequestTypeDef,
     ConnectorDefinitionVersionOutputTypeDef,
     ConnectorDefinitionVersionTypeDef,
-    CreateConnectorDefinitionVersionRequestRequestTypeDef,
+    ConnectorUnionTypeDef,
     CoreDefinitionVersionOutputTypeDef,
     CoreDefinitionVersionTypeDef,
     CreateCoreDefinitionVersionRequestRequestTypeDef,
     CreateDeviceDefinitionVersionRequestRequestTypeDef,
     DeviceDefinitionVersionOutputTypeDef,
     DeviceDefinitionVersionTypeDef,
     CreateGroupRequestRequestTypeDef,
@@ -632,49 +600,59 @@
     ListSubscriptionDefinitionVersionsResponseTypeDef,
     S3MachineLearningModelResourceDataTypeDef,
     SageMakerMachineLearningModelResourceDataTypeDef,
     RuntimeConfigurationTypeDef,
     UpdateThingRuntimeConfigurationRequestRequestTypeDef,
     ListBulkDeploymentDetailedReportsResponseTypeDef,
     GetConnectorDefinitionVersionResponseTypeDef,
+    ConnectorDefinitionVersionUnionTypeDef,
     CreateConnectorDefinitionRequestRequestTypeDef,
+    CreateConnectorDefinitionVersionRequestRequestTypeDef,
     GetCoreDefinitionVersionResponseTypeDef,
+    CoreDefinitionVersionUnionTypeDef,
     CreateCoreDefinitionRequestRequestTypeDef,
     GetDeviceDefinitionVersionResponseTypeDef,
     CreateDeviceDefinitionRequestRequestTypeDef,
+    DeviceDefinitionVersionUnionTypeDef,
     GetLoggerDefinitionVersionResponseTypeDef,
     CreateLoggerDefinitionRequestRequestTypeDef,
+    LoggerDefinitionVersionUnionTypeDef,
     GetSubscriptionDefinitionVersionResponseTypeDef,
     CreateSubscriptionDefinitionRequestRequestTypeDef,
+    SubscriptionDefinitionVersionUnionTypeDef,
     FunctionDefaultConfigTypeDef,
     FunctionConfigurationEnvironmentOutputTypeDef,
     FunctionConfigurationEnvironmentTypeDef,
     ResourceDataContainerOutputTypeDef,
     ResourceDataContainerTypeDef,
     GetThingRuntimeConfigurationResponseTypeDef,
     FunctionConfigurationOutputTypeDef,
     FunctionConfigurationTypeDef,
     ResourceOutputTypeDef,
     ResourceTypeDef,
     FunctionOutputTypeDef,
     FunctionTypeDef,
     ResourceDefinitionVersionOutputTypeDef,
-    CreateResourceDefinitionVersionRequestRequestTypeDef,
     ResourceDefinitionVersionTypeDef,
+    ResourceUnionTypeDef,
     FunctionDefinitionVersionOutputTypeDef,
-    CreateFunctionDefinitionVersionRequestRequestTypeDef,
     FunctionDefinitionVersionTypeDef,
+    FunctionUnionTypeDef,
     GetResourceDefinitionVersionResponseTypeDef,
     CreateResourceDefinitionRequestRequestTypeDef,
+    ResourceDefinitionVersionUnionTypeDef,
+    CreateResourceDefinitionVersionRequestRequestTypeDef,
     GetFunctionDefinitionVersionResponseTypeDef,
     CreateFunctionDefinitionRequestRequestTypeDef,
+    FunctionDefinitionVersionUnionTypeDef,
+    CreateFunctionDefinitionVersionRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AssociateRoleToGroupRequestRequestTypeDef:
+def get_value() -> AssociateRoleToGroupRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-greengrass-1.28.15.post1/README.md` & `mypy-boto3-greengrass-1.28.16/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-greengrass
+Version: 1.28.16
+Summary: Type annotations for boto3.Greengrass 1.28.16 service generated with mypy-boto3-builder 7.17.1
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 greengrass type-annotations botocore mypy typeshed autocomplete
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Typing :: Typed
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <a id="mypy-boto3-greengrass"></a>
 
 # mypy-boto3-greengrass
 
 [![PyPI - mypy-boto3-greengrass](https://img.shields.io/pypi/v/mypy-boto3-greengrass.svg?color=blue)](https://pypi.org/project/mypy-boto3-greengrass)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-greengrass.svg?color=blue)](https://pypi.org/project/mypy-boto3-greengrass)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-greengrass)](https://pepy.tech/project/mypy-boto3-greengrass)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Greengrass 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass)
+[boto3.Greengrass 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass)
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
 [mypy-boto3-greengrass docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/).
 
 See how it helps to find and fix potential bugs:
 
@@ -42,15 +74,15 @@
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
@@ -381,20 +413,20 @@
 )
 
 
 def check_value(value: BulkDeploymentStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_greengrass.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_greengrass.type_defs import (
     AssociateRoleToGroupRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     AssociateServiceRoleToAccountRequestRequestTypeDef,
     BulkDeploymentMetricsTypeDef,
@@ -538,15 +570,15 @@
     GetBulkDeploymentStatusResponseTypeDef,
     GetDeploymentStatusResponseTypeDef,
     ListBulkDeploymentsResponseTypeDef,
     GetConnectivityInfoResponseTypeDef,
     UpdateConnectivityInfoRequestRequestTypeDef,
     ConnectorDefinitionVersionOutputTypeDef,
     ConnectorDefinitionVersionTypeDef,
-    CreateConnectorDefinitionVersionRequestRequestTypeDef,
+    ConnectorUnionTypeDef,
     CoreDefinitionVersionOutputTypeDef,
     CoreDefinitionVersionTypeDef,
     CreateCoreDefinitionVersionRequestRequestTypeDef,
     CreateDeviceDefinitionVersionRequestRequestTypeDef,
     DeviceDefinitionVersionOutputTypeDef,
     DeviceDefinitionVersionTypeDef,
     CreateGroupRequestRequestTypeDef,
@@ -600,49 +632,59 @@
     ListSubscriptionDefinitionVersionsResponseTypeDef,
     S3MachineLearningModelResourceDataTypeDef,
     SageMakerMachineLearningModelResourceDataTypeDef,
     RuntimeConfigurationTypeDef,
     UpdateThingRuntimeConfigurationRequestRequestTypeDef,
     ListBulkDeploymentDetailedReportsResponseTypeDef,
     GetConnectorDefinitionVersionResponseTypeDef,
+    ConnectorDefinitionVersionUnionTypeDef,
     CreateConnectorDefinitionRequestRequestTypeDef,
+    CreateConnectorDefinitionVersionRequestRequestTypeDef,
     GetCoreDefinitionVersionResponseTypeDef,
+    CoreDefinitionVersionUnionTypeDef,
     CreateCoreDefinitionRequestRequestTypeDef,
     GetDeviceDefinitionVersionResponseTypeDef,
     CreateDeviceDefinitionRequestRequestTypeDef,
+    DeviceDefinitionVersionUnionTypeDef,
     GetLoggerDefinitionVersionResponseTypeDef,
     CreateLoggerDefinitionRequestRequestTypeDef,
+    LoggerDefinitionVersionUnionTypeDef,
     GetSubscriptionDefinitionVersionResponseTypeDef,
     CreateSubscriptionDefinitionRequestRequestTypeDef,
+    SubscriptionDefinitionVersionUnionTypeDef,
     FunctionDefaultConfigTypeDef,
     FunctionConfigurationEnvironmentOutputTypeDef,
     FunctionConfigurationEnvironmentTypeDef,
     ResourceDataContainerOutputTypeDef,
     ResourceDataContainerTypeDef,
     GetThingRuntimeConfigurationResponseTypeDef,
     FunctionConfigurationOutputTypeDef,
     FunctionConfigurationTypeDef,
     ResourceOutputTypeDef,
     ResourceTypeDef,
     FunctionOutputTypeDef,
     FunctionTypeDef,
     ResourceDefinitionVersionOutputTypeDef,
-    CreateResourceDefinitionVersionRequestRequestTypeDef,
     ResourceDefinitionVersionTypeDef,
+    ResourceUnionTypeDef,
     FunctionDefinitionVersionOutputTypeDef,
-    CreateFunctionDefinitionVersionRequestRequestTypeDef,
     FunctionDefinitionVersionTypeDef,
+    FunctionUnionTypeDef,
     GetResourceDefinitionVersionResponseTypeDef,
     CreateResourceDefinitionRequestRequestTypeDef,
+    ResourceDefinitionVersionUnionTypeDef,
+    CreateResourceDefinitionVersionRequestRequestTypeDef,
     GetFunctionDefinitionVersionResponseTypeDef,
     CreateFunctionDefinitionRequestRequestTypeDef,
+    FunctionDefinitionVersionUnionTypeDef,
+    CreateFunctionDefinitionVersionRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AssociateRoleToGroupRequestRequestTypeDef:
+def get_value() -> AssociateRoleToGroupRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-greengrass-1.28.15.post1/mypy_boto3_greengrass/__init__.py` & `mypy-boto3-greengrass-1.28.16/mypy_boto3_greengrass/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-greengrass-1.28.15.post1/mypy_boto3_greengrass/__init__.pyi` & `mypy-boto3-greengrass-1.28.16/mypy_boto3_greengrass/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-greengrass-1.28.15.post1/mypy_boto3_greengrass/__main__.py` & `mypy-boto3-greengrass-1.28.16/mypy_boto3_greengrass/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Greengrass 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.Greengrass 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass\nOther"
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

### Comparing `mypy-boto3-greengrass-1.28.15.post1/mypy_boto3_greengrass/client.py` & `mypy-boto3-greengrass-1.28.16/mypy_boto3_greengrass/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_greengrass.client import GreengrassClient
 
     session = Session()
     client: GreengrassClient = session.client("greengrass")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     DeploymentTypeType,
     SoftwareToUpdateType,
     UpdateAgentLogLevelType,
@@ -46,20 +46,17 @@
     ListSubscriptionDefinitionsPaginator,
     ListSubscriptionDefinitionVersionsPaginator,
 )
 from .type_defs import (
     AssociateRoleToGroupResponseTypeDef,
     AssociateServiceRoleToAccountResponseTypeDef,
     ConnectivityInfoTypeDef,
-    ConnectorDefinitionVersionOutputTypeDef,
-    ConnectorDefinitionVersionTypeDef,
-    ConnectorOutputTypeDef,
-    ConnectorTypeDef,
-    CoreDefinitionVersionOutputTypeDef,
-    CoreDefinitionVersionTypeDef,
+    ConnectorDefinitionVersionUnionTypeDef,
+    ConnectorUnionTypeDef,
+    CoreDefinitionVersionUnionTypeDef,
     CoreTypeDef,
     CreateConnectorDefinitionResponseTypeDef,
     CreateConnectorDefinitionVersionResponseTypeDef,
     CreateCoreDefinitionResponseTypeDef,
     CreateCoreDefinitionVersionResponseTypeDef,
     CreateDeploymentResponseTypeDef,
     CreateDeviceDefinitionResponseTypeDef,
@@ -72,25 +69,22 @@
     CreateLoggerDefinitionResponseTypeDef,
     CreateLoggerDefinitionVersionResponseTypeDef,
     CreateResourceDefinitionResponseTypeDef,
     CreateResourceDefinitionVersionResponseTypeDef,
     CreateSoftwareUpdateJobResponseTypeDef,
     CreateSubscriptionDefinitionResponseTypeDef,
     CreateSubscriptionDefinitionVersionResponseTypeDef,
-    DeviceDefinitionVersionOutputTypeDef,
-    DeviceDefinitionVersionTypeDef,
+    DeviceDefinitionVersionUnionTypeDef,
     DeviceTypeDef,
     DisassociateRoleFromGroupResponseTypeDef,
     DisassociateServiceRoleFromAccountResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     FunctionDefaultConfigTypeDef,
-    FunctionDefinitionVersionOutputTypeDef,
-    FunctionDefinitionVersionTypeDef,
-    FunctionOutputTypeDef,
-    FunctionTypeDef,
+    FunctionDefinitionVersionUnionTypeDef,
+    FunctionUnionTypeDef,
     GetAssociatedRoleResponseTypeDef,
     GetBulkDeploymentStatusResponseTypeDef,
     GetConnectivityInfoResponseTypeDef,
     GetConnectorDefinitionResponseTypeDef,
     GetConnectorDefinitionVersionResponseTypeDef,
     GetCoreDefinitionResponseTypeDef,
     GetCoreDefinitionVersionResponseTypeDef,
@@ -129,25 +123,21 @@
     ListLoggerDefinitionsResponseTypeDef,
     ListLoggerDefinitionVersionsResponseTypeDef,
     ListResourceDefinitionsResponseTypeDef,
     ListResourceDefinitionVersionsResponseTypeDef,
     ListSubscriptionDefinitionsResponseTypeDef,
     ListSubscriptionDefinitionVersionsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    LoggerDefinitionVersionOutputTypeDef,
-    LoggerDefinitionVersionTypeDef,
+    LoggerDefinitionVersionUnionTypeDef,
     LoggerTypeDef,
     ResetDeploymentsResponseTypeDef,
-    ResourceDefinitionVersionOutputTypeDef,
-    ResourceDefinitionVersionTypeDef,
-    ResourceOutputTypeDef,
-    ResourceTypeDef,
+    ResourceDefinitionVersionUnionTypeDef,
+    ResourceUnionTypeDef,
     StartBulkDeploymentResponseTypeDef,
-    SubscriptionDefinitionVersionOutputTypeDef,
-    SubscriptionDefinitionVersionTypeDef,
+    SubscriptionDefinitionVersionUnionTypeDef,
     SubscriptionTypeDef,
     TelemetryConfigurationUpdateTypeDef,
     UpdateConnectivityInfoResponseTypeDef,
     UpdateGroupCertificateConfigurationResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
@@ -226,17 +216,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/client/#close)
         """
 
     def create_connector_definition(
         self,
         *,
         AmznClientToken: str = ...,
-        InitialVersion: Union[
-            ConnectorDefinitionVersionTypeDef, ConnectorDefinitionVersionOutputTypeDef
-        ] = ...,
+        InitialVersion: ConnectorDefinitionVersionUnionTypeDef = ...,
         Name: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateConnectorDefinitionResponseTypeDef:
         """
         Creates a connector definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.create_connector_definition)
@@ -244,30 +232,28 @@
         """
 
     def create_connector_definition_version(
         self,
         *,
         ConnectorDefinitionId: str,
         AmznClientToken: str = ...,
-        Connectors: Sequence[Union[ConnectorTypeDef, ConnectorOutputTypeDef]] = ...
+        Connectors: Sequence[ConnectorUnionTypeDef] = ...
     ) -> CreateConnectorDefinitionVersionResponseTypeDef:
         """
         Creates a version of a connector definition which has already been defined.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.create_connector_definition_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/client/#create_connector_definition_version)
         """
 
     def create_core_definition(
         self,
         *,
         AmznClientToken: str = ...,
-        InitialVersion: Union[
-            CoreDefinitionVersionTypeDef, CoreDefinitionVersionOutputTypeDef
-        ] = ...,
+        InitialVersion: CoreDefinitionVersionUnionTypeDef = ...,
         Name: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateCoreDefinitionResponseTypeDef:
         """
         Creates a core definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.create_core_definition)
@@ -304,17 +290,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/client/#create_deployment)
         """
 
     def create_device_definition(
         self,
         *,
         AmznClientToken: str = ...,
-        InitialVersion: Union[
-            DeviceDefinitionVersionTypeDef, DeviceDefinitionVersionOutputTypeDef
-        ] = ...,
+        InitialVersion: DeviceDefinitionVersionUnionTypeDef = ...,
         Name: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateDeviceDefinitionResponseTypeDef:
         """
         Creates a device definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.create_device_definition)
@@ -335,17 +319,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/client/#create_device_definition_version)
         """
 
     def create_function_definition(
         self,
         *,
         AmznClientToken: str = ...,
-        InitialVersion: Union[
-            FunctionDefinitionVersionTypeDef, FunctionDefinitionVersionOutputTypeDef
-        ] = ...,
+        InitialVersion: FunctionDefinitionVersionUnionTypeDef = ...,
         Name: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateFunctionDefinitionResponseTypeDef:
         """
         Creates a Lambda function definition which contains a list of Lambda functions
         and their configurations to be used in a group.
 
@@ -355,15 +337,15 @@
 
     def create_function_definition_version(
         self,
         *,
         FunctionDefinitionId: str,
         AmznClientToken: str = ...,
         DefaultConfig: FunctionDefaultConfigTypeDef = ...,
-        Functions: Sequence[Union[FunctionTypeDef, FunctionOutputTypeDef]] = ...
+        Functions: Sequence[FunctionUnionTypeDef] = ...
     ) -> CreateFunctionDefinitionVersionResponseTypeDef:
         """
         Creates a version of a Lambda function definition that has already been defined.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.create_function_definition_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/client/#create_function_definition_version)
         """
@@ -413,17 +395,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/client/#create_group_version)
         """
 
     def create_logger_definition(
         self,
         *,
         AmznClientToken: str = ...,
-        InitialVersion: Union[
-            LoggerDefinitionVersionTypeDef, LoggerDefinitionVersionOutputTypeDef
-        ] = ...,
+        InitialVersion: LoggerDefinitionVersionUnionTypeDef = ...,
         Name: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateLoggerDefinitionResponseTypeDef:
         """
         Creates a logger definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.create_logger_definition)
@@ -444,17 +424,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/client/#create_logger_definition_version)
         """
 
     def create_resource_definition(
         self,
         *,
         AmznClientToken: str = ...,
-        InitialVersion: Union[
-            ResourceDefinitionVersionTypeDef, ResourceDefinitionVersionOutputTypeDef
-        ] = ...,
+        InitialVersion: ResourceDefinitionVersionUnionTypeDef = ...,
         Name: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateResourceDefinitionResponseTypeDef:
         """
         Creates a resource definition which contains a list of resources to be used in a
         group.
 
@@ -463,15 +441,15 @@
         """
 
     def create_resource_definition_version(
         self,
         *,
         ResourceDefinitionId: str,
         AmznClientToken: str = ...,
-        Resources: Sequence[Union[ResourceTypeDef, ResourceOutputTypeDef]] = ...
+        Resources: Sequence[ResourceUnionTypeDef] = ...
     ) -> CreateResourceDefinitionVersionResponseTypeDef:
         """
         Creates a version of a resource definition that has already been defined.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.create_resource_definition_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/client/#create_resource_definition_version)
         """
@@ -496,17 +474,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/client/#create_software_update_job)
         """
 
     def create_subscription_definition(
         self,
         *,
         AmznClientToken: str = ...,
-        InitialVersion: Union[
-            SubscriptionDefinitionVersionTypeDef, SubscriptionDefinitionVersionOutputTypeDef
-        ] = ...,
+        InitialVersion: SubscriptionDefinitionVersionUnionTypeDef = ...,
         Name: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateSubscriptionDefinitionResponseTypeDef:
         """
         Creates a subscription definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.create_subscription_definition)
```

### Comparing `mypy-boto3-greengrass-1.28.15.post1/mypy_boto3_greengrass/client.pyi` & `mypy-boto3-greengrass-1.28.16/mypy_boto3_greengrass/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_greengrass.client import GreengrassClient
 
     session = Session()
     client: GreengrassClient = session.client("greengrass")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     DeploymentTypeType,
     SoftwareToUpdateType,
     UpdateAgentLogLevelType,
@@ -46,20 +46,17 @@
     ListSubscriptionDefinitionsPaginator,
     ListSubscriptionDefinitionVersionsPaginator,
 )
 from .type_defs import (
     AssociateRoleToGroupResponseTypeDef,
     AssociateServiceRoleToAccountResponseTypeDef,
     ConnectivityInfoTypeDef,
-    ConnectorDefinitionVersionOutputTypeDef,
-    ConnectorDefinitionVersionTypeDef,
-    ConnectorOutputTypeDef,
-    ConnectorTypeDef,
-    CoreDefinitionVersionOutputTypeDef,
-    CoreDefinitionVersionTypeDef,
+    ConnectorDefinitionVersionUnionTypeDef,
+    ConnectorUnionTypeDef,
+    CoreDefinitionVersionUnionTypeDef,
     CoreTypeDef,
     CreateConnectorDefinitionResponseTypeDef,
     CreateConnectorDefinitionVersionResponseTypeDef,
     CreateCoreDefinitionResponseTypeDef,
     CreateCoreDefinitionVersionResponseTypeDef,
     CreateDeploymentResponseTypeDef,
     CreateDeviceDefinitionResponseTypeDef,
@@ -72,25 +69,22 @@
     CreateLoggerDefinitionResponseTypeDef,
     CreateLoggerDefinitionVersionResponseTypeDef,
     CreateResourceDefinitionResponseTypeDef,
     CreateResourceDefinitionVersionResponseTypeDef,
     CreateSoftwareUpdateJobResponseTypeDef,
     CreateSubscriptionDefinitionResponseTypeDef,
     CreateSubscriptionDefinitionVersionResponseTypeDef,
-    DeviceDefinitionVersionOutputTypeDef,
-    DeviceDefinitionVersionTypeDef,
+    DeviceDefinitionVersionUnionTypeDef,
     DeviceTypeDef,
     DisassociateRoleFromGroupResponseTypeDef,
     DisassociateServiceRoleFromAccountResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     FunctionDefaultConfigTypeDef,
-    FunctionDefinitionVersionOutputTypeDef,
-    FunctionDefinitionVersionTypeDef,
-    FunctionOutputTypeDef,
-    FunctionTypeDef,
+    FunctionDefinitionVersionUnionTypeDef,
+    FunctionUnionTypeDef,
     GetAssociatedRoleResponseTypeDef,
     GetBulkDeploymentStatusResponseTypeDef,
     GetConnectivityInfoResponseTypeDef,
     GetConnectorDefinitionResponseTypeDef,
     GetConnectorDefinitionVersionResponseTypeDef,
     GetCoreDefinitionResponseTypeDef,
     GetCoreDefinitionVersionResponseTypeDef,
@@ -129,25 +123,21 @@
     ListLoggerDefinitionsResponseTypeDef,
     ListLoggerDefinitionVersionsResponseTypeDef,
     ListResourceDefinitionsResponseTypeDef,
     ListResourceDefinitionVersionsResponseTypeDef,
     ListSubscriptionDefinitionsResponseTypeDef,
     ListSubscriptionDefinitionVersionsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    LoggerDefinitionVersionOutputTypeDef,
-    LoggerDefinitionVersionTypeDef,
+    LoggerDefinitionVersionUnionTypeDef,
     LoggerTypeDef,
     ResetDeploymentsResponseTypeDef,
-    ResourceDefinitionVersionOutputTypeDef,
-    ResourceDefinitionVersionTypeDef,
-    ResourceOutputTypeDef,
-    ResourceTypeDef,
+    ResourceDefinitionVersionUnionTypeDef,
+    ResourceUnionTypeDef,
     StartBulkDeploymentResponseTypeDef,
-    SubscriptionDefinitionVersionOutputTypeDef,
-    SubscriptionDefinitionVersionTypeDef,
+    SubscriptionDefinitionVersionUnionTypeDef,
     SubscriptionTypeDef,
     TelemetryConfigurationUpdateTypeDef,
     UpdateConnectivityInfoResponseTypeDef,
     UpdateGroupCertificateConfigurationResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
@@ -217,46 +207,42 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/client/#close)
         """
     def create_connector_definition(
         self,
         *,
         AmznClientToken: str = ...,
-        InitialVersion: Union[
-            ConnectorDefinitionVersionTypeDef, ConnectorDefinitionVersionOutputTypeDef
-        ] = ...,
+        InitialVersion: ConnectorDefinitionVersionUnionTypeDef = ...,
         Name: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateConnectorDefinitionResponseTypeDef:
         """
         Creates a connector definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.create_connector_definition)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/client/#create_connector_definition)
         """
     def create_connector_definition_version(
         self,
         *,
         ConnectorDefinitionId: str,
         AmznClientToken: str = ...,
-        Connectors: Sequence[Union[ConnectorTypeDef, ConnectorOutputTypeDef]] = ...
+        Connectors: Sequence[ConnectorUnionTypeDef] = ...
     ) -> CreateConnectorDefinitionVersionResponseTypeDef:
         """
         Creates a version of a connector definition which has already been defined.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.create_connector_definition_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/client/#create_connector_definition_version)
         """
     def create_core_definition(
         self,
         *,
         AmznClientToken: str = ...,
-        InitialVersion: Union[
-            CoreDefinitionVersionTypeDef, CoreDefinitionVersionOutputTypeDef
-        ] = ...,
+        InitialVersion: CoreDefinitionVersionUnionTypeDef = ...,
         Name: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateCoreDefinitionResponseTypeDef:
         """
         Creates a core definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.create_core_definition)
@@ -290,17 +276,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.create_deployment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/client/#create_deployment)
         """
     def create_device_definition(
         self,
         *,
         AmznClientToken: str = ...,
-        InitialVersion: Union[
-            DeviceDefinitionVersionTypeDef, DeviceDefinitionVersionOutputTypeDef
-        ] = ...,
+        InitialVersion: DeviceDefinitionVersionUnionTypeDef = ...,
         Name: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateDeviceDefinitionResponseTypeDef:
         """
         Creates a device definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.create_device_definition)
@@ -319,17 +303,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.create_device_definition_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/client/#create_device_definition_version)
         """
     def create_function_definition(
         self,
         *,
         AmznClientToken: str = ...,
-        InitialVersion: Union[
-            FunctionDefinitionVersionTypeDef, FunctionDefinitionVersionOutputTypeDef
-        ] = ...,
+        InitialVersion: FunctionDefinitionVersionUnionTypeDef = ...,
         Name: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateFunctionDefinitionResponseTypeDef:
         """
         Creates a Lambda function definition which contains a list of Lambda functions
         and their configurations to be used in a group.
 
@@ -338,15 +320,15 @@
         """
     def create_function_definition_version(
         self,
         *,
         FunctionDefinitionId: str,
         AmznClientToken: str = ...,
         DefaultConfig: FunctionDefaultConfigTypeDef = ...,
-        Functions: Sequence[Union[FunctionTypeDef, FunctionOutputTypeDef]] = ...
+        Functions: Sequence[FunctionUnionTypeDef] = ...
     ) -> CreateFunctionDefinitionVersionResponseTypeDef:
         """
         Creates a version of a Lambda function definition that has already been defined.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.create_function_definition_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/client/#create_function_definition_version)
         """
@@ -392,17 +374,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.create_group_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/client/#create_group_version)
         """
     def create_logger_definition(
         self,
         *,
         AmznClientToken: str = ...,
-        InitialVersion: Union[
-            LoggerDefinitionVersionTypeDef, LoggerDefinitionVersionOutputTypeDef
-        ] = ...,
+        InitialVersion: LoggerDefinitionVersionUnionTypeDef = ...,
         Name: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateLoggerDefinitionResponseTypeDef:
         """
         Creates a logger definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.create_logger_definition)
@@ -421,17 +401,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.create_logger_definition_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/client/#create_logger_definition_version)
         """
     def create_resource_definition(
         self,
         *,
         AmznClientToken: str = ...,
-        InitialVersion: Union[
-            ResourceDefinitionVersionTypeDef, ResourceDefinitionVersionOutputTypeDef
-        ] = ...,
+        InitialVersion: ResourceDefinitionVersionUnionTypeDef = ...,
         Name: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateResourceDefinitionResponseTypeDef:
         """
         Creates a resource definition which contains a list of resources to be used in a
         group.
 
@@ -439,15 +417,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/client/#create_resource_definition)
         """
     def create_resource_definition_version(
         self,
         *,
         ResourceDefinitionId: str,
         AmznClientToken: str = ...,
-        Resources: Sequence[Union[ResourceTypeDef, ResourceOutputTypeDef]] = ...
+        Resources: Sequence[ResourceUnionTypeDef] = ...
     ) -> CreateResourceDefinitionVersionResponseTypeDef:
         """
         Creates a version of a resource definition that has already been defined.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.create_resource_definition_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/client/#create_resource_definition_version)
         """
@@ -470,17 +448,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.create_software_update_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/client/#create_software_update_job)
         """
     def create_subscription_definition(
         self,
         *,
         AmznClientToken: str = ...,
-        InitialVersion: Union[
-            SubscriptionDefinitionVersionTypeDef, SubscriptionDefinitionVersionOutputTypeDef
-        ] = ...,
+        InitialVersion: SubscriptionDefinitionVersionUnionTypeDef = ...,
         Name: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateSubscriptionDefinitionResponseTypeDef:
         """
         Creates a subscription definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass.Client.create_subscription_definition)
```

### Comparing `mypy-boto3-greengrass-1.28.15.post1/mypy_boto3_greengrass/literals.py` & `mypy-boto3-greengrass-1.28.16/mypy_boto3_greengrass/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-greengrass-1.28.15.post1/mypy_boto3_greengrass/literals.pyi` & `mypy-boto3-greengrass-1.28.16/mypy_boto3_greengrass/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-greengrass-1.28.15.post1/mypy_boto3_greengrass/paginator.py` & `mypy-boto3-greengrass-1.28.16/mypy_boto3_greengrass/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-greengrass-1.28.15.post1/mypy_boto3_greengrass/paginator.pyi` & `mypy-boto3-greengrass-1.28.16/mypy_boto3_greengrass/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-greengrass-1.28.15.post1/mypy_boto3_greengrass/type_defs.py` & `mypy-boto3-greengrass-1.28.16/mypy_boto3_greengrass/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_greengrass.type_defs import AssociateRoleToGroupRequestRequestTypeDef
 
-    data: AssociateRoleToGroupRequestRequestTypeDef = {...}
+    data: AssociateRoleToGroupRequestRequestTypeDef = ...
     ```
 """
 import sys
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     BulkDeploymentStatusType,
@@ -182,15 +182,15 @@
     "GetBulkDeploymentStatusResponseTypeDef",
     "GetDeploymentStatusResponseTypeDef",
     "ListBulkDeploymentsResponseTypeDef",
     "GetConnectivityInfoResponseTypeDef",
     "UpdateConnectivityInfoRequestRequestTypeDef",
     "ConnectorDefinitionVersionOutputTypeDef",
     "ConnectorDefinitionVersionTypeDef",
-    "CreateConnectorDefinitionVersionRequestRequestTypeDef",
+    "ConnectorUnionTypeDef",
     "CoreDefinitionVersionOutputTypeDef",
     "CoreDefinitionVersionTypeDef",
     "CreateCoreDefinitionVersionRequestRequestTypeDef",
     "CreateDeviceDefinitionVersionRequestRequestTypeDef",
     "DeviceDefinitionVersionOutputTypeDef",
     "DeviceDefinitionVersionTypeDef",
     "CreateGroupRequestRequestTypeDef",
@@ -244,45 +244,55 @@
     "ListSubscriptionDefinitionVersionsResponseTypeDef",
     "S3MachineLearningModelResourceDataTypeDef",
     "SageMakerMachineLearningModelResourceDataTypeDef",
     "RuntimeConfigurationTypeDef",
     "UpdateThingRuntimeConfigurationRequestRequestTypeDef",
     "ListBulkDeploymentDetailedReportsResponseTypeDef",
     "GetConnectorDefinitionVersionResponseTypeDef",
+    "ConnectorDefinitionVersionUnionTypeDef",
     "CreateConnectorDefinitionRequestRequestTypeDef",
+    "CreateConnectorDefinitionVersionRequestRequestTypeDef",
     "GetCoreDefinitionVersionResponseTypeDef",
+    "CoreDefinitionVersionUnionTypeDef",
     "CreateCoreDefinitionRequestRequestTypeDef",
     "GetDeviceDefinitionVersionResponseTypeDef",
     "CreateDeviceDefinitionRequestRequestTypeDef",
+    "DeviceDefinitionVersionUnionTypeDef",
     "GetLoggerDefinitionVersionResponseTypeDef",
     "CreateLoggerDefinitionRequestRequestTypeDef",
+    "LoggerDefinitionVersionUnionTypeDef",
     "GetSubscriptionDefinitionVersionResponseTypeDef",
     "CreateSubscriptionDefinitionRequestRequestTypeDef",
+    "SubscriptionDefinitionVersionUnionTypeDef",
     "FunctionDefaultConfigTypeDef",
     "FunctionConfigurationEnvironmentOutputTypeDef",
     "FunctionConfigurationEnvironmentTypeDef",
     "ResourceDataContainerOutputTypeDef",
     "ResourceDataContainerTypeDef",
     "GetThingRuntimeConfigurationResponseTypeDef",
     "FunctionConfigurationOutputTypeDef",
     "FunctionConfigurationTypeDef",
     "ResourceOutputTypeDef",
     "ResourceTypeDef",
     "FunctionOutputTypeDef",
     "FunctionTypeDef",
     "ResourceDefinitionVersionOutputTypeDef",
-    "CreateResourceDefinitionVersionRequestRequestTypeDef",
     "ResourceDefinitionVersionTypeDef",
+    "ResourceUnionTypeDef",
     "FunctionDefinitionVersionOutputTypeDef",
-    "CreateFunctionDefinitionVersionRequestRequestTypeDef",
     "FunctionDefinitionVersionTypeDef",
+    "FunctionUnionTypeDef",
     "GetResourceDefinitionVersionResponseTypeDef",
     "CreateResourceDefinitionRequestRequestTypeDef",
+    "ResourceDefinitionVersionUnionTypeDef",
+    "CreateResourceDefinitionVersionRequestRequestTypeDef",
     "GetFunctionDefinitionVersionResponseTypeDef",
     "CreateFunctionDefinitionRequestRequestTypeDef",
+    "FunctionDefinitionVersionUnionTypeDef",
+    "CreateFunctionDefinitionVersionRequestRequestTypeDef",
 )
 
 AssociateRoleToGroupRequestRequestTypeDef = TypedDict(
     "AssociateRoleToGroupRequestRequestTypeDef",
     {
         "GroupId": str,
         "RoleArn": str,
@@ -2213,37 +2223,15 @@
     "ConnectorDefinitionVersionTypeDef",
     {
         "Connectors": Sequence[ConnectorTypeDef],
     },
     total=False,
 )
 
-_RequiredCreateConnectorDefinitionVersionRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateConnectorDefinitionVersionRequestRequestTypeDef",
-    {
-        "ConnectorDefinitionId": str,
-    },
-)
-_OptionalCreateConnectorDefinitionVersionRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateConnectorDefinitionVersionRequestRequestTypeDef",
-    {
-        "AmznClientToken": str,
-        "Connectors": Sequence[Union[ConnectorTypeDef, ConnectorOutputTypeDef]],
-    },
-    total=False,
-)
-
-
-class CreateConnectorDefinitionVersionRequestRequestTypeDef(
-    _RequiredCreateConnectorDefinitionVersionRequestRequestTypeDef,
-    _OptionalCreateConnectorDefinitionVersionRequestRequestTypeDef,
-):
-    pass
-
-
+ConnectorUnionTypeDef = Union[ConnectorTypeDef, ConnectorOutputTypeDef]
 CoreDefinitionVersionOutputTypeDef = TypedDict(
     "CoreDefinitionVersionOutputTypeDef",
     {
         "Cores": List[CoreTypeDef],
     },
     total=False,
 )
@@ -2989,38 +2977,67 @@
         "Id": str,
         "NextToken": str,
         "Version": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ConnectorDefinitionVersionUnionTypeDef = Union[
+    ConnectorDefinitionVersionTypeDef, ConnectorDefinitionVersionOutputTypeDef
+]
 CreateConnectorDefinitionRequestRequestTypeDef = TypedDict(
     "CreateConnectorDefinitionRequestRequestTypeDef",
     {
         "AmznClientToken": str,
         "InitialVersion": ConnectorDefinitionVersionTypeDef,
         "Name": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+_RequiredCreateConnectorDefinitionVersionRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateConnectorDefinitionVersionRequestRequestTypeDef",
+    {
+        "ConnectorDefinitionId": str,
+    },
+)
+_OptionalCreateConnectorDefinitionVersionRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateConnectorDefinitionVersionRequestRequestTypeDef",
+    {
+        "AmznClientToken": str,
+        "Connectors": Sequence[ConnectorUnionTypeDef],
+    },
+    total=False,
+)
+
+
+class CreateConnectorDefinitionVersionRequestRequestTypeDef(
+    _RequiredCreateConnectorDefinitionVersionRequestRequestTypeDef,
+    _OptionalCreateConnectorDefinitionVersionRequestRequestTypeDef,
+):
+    pass
+
+
 GetCoreDefinitionVersionResponseTypeDef = TypedDict(
     "GetCoreDefinitionVersionResponseTypeDef",
     {
         "Arn": str,
         "CreationTimestamp": str,
         "Definition": CoreDefinitionVersionOutputTypeDef,
         "Id": str,
         "NextToken": str,
         "Version": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+CoreDefinitionVersionUnionTypeDef = Union[
+    CoreDefinitionVersionTypeDef, CoreDefinitionVersionOutputTypeDef
+]
 CreateCoreDefinitionRequestRequestTypeDef = TypedDict(
     "CreateCoreDefinitionRequestRequestTypeDef",
     {
         "AmznClientToken": str,
         "InitialVersion": CoreDefinitionVersionTypeDef,
         "Name": str,
         "tags": Mapping[str, str],
@@ -3048,14 +3065,17 @@
         "InitialVersion": DeviceDefinitionVersionTypeDef,
         "Name": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+DeviceDefinitionVersionUnionTypeDef = Union[
+    DeviceDefinitionVersionTypeDef, DeviceDefinitionVersionOutputTypeDef
+]
 GetLoggerDefinitionVersionResponseTypeDef = TypedDict(
     "GetLoggerDefinitionVersionResponseTypeDef",
     {
         "Arn": str,
         "CreationTimestamp": str,
         "Definition": LoggerDefinitionVersionOutputTypeDef,
         "Id": str,
@@ -3071,14 +3091,17 @@
         "InitialVersion": LoggerDefinitionVersionTypeDef,
         "Name": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+LoggerDefinitionVersionUnionTypeDef = Union[
+    LoggerDefinitionVersionTypeDef, LoggerDefinitionVersionOutputTypeDef
+]
 GetSubscriptionDefinitionVersionResponseTypeDef = TypedDict(
     "GetSubscriptionDefinitionVersionResponseTypeDef",
     {
         "Arn": str,
         "CreationTimestamp": str,
         "Definition": SubscriptionDefinitionVersionOutputTypeDef,
         "Id": str,
@@ -3095,14 +3118,17 @@
         "InitialVersion": SubscriptionDefinitionVersionTypeDef,
         "Name": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+SubscriptionDefinitionVersionUnionTypeDef = Union[
+    SubscriptionDefinitionVersionTypeDef, SubscriptionDefinitionVersionOutputTypeDef
+]
 FunctionDefaultConfigTypeDef = TypedDict(
     "FunctionDefaultConfigTypeDef",
     {
         "Execution": FunctionDefaultExecutionConfigTypeDef,
     },
     total=False,
 )
@@ -3257,87 +3283,42 @@
     "ResourceDefinitionVersionOutputTypeDef",
     {
         "Resources": List[ResourceOutputTypeDef],
     },
     total=False,
 )
 
-_RequiredCreateResourceDefinitionVersionRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateResourceDefinitionVersionRequestRequestTypeDef",
-    {
-        "ResourceDefinitionId": str,
-    },
-)
-_OptionalCreateResourceDefinitionVersionRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateResourceDefinitionVersionRequestRequestTypeDef",
-    {
-        "AmznClientToken": str,
-        "Resources": Sequence[Union[ResourceTypeDef, ResourceOutputTypeDef]],
-    },
-    total=False,
-)
-
-
-class CreateResourceDefinitionVersionRequestRequestTypeDef(
-    _RequiredCreateResourceDefinitionVersionRequestRequestTypeDef,
-    _OptionalCreateResourceDefinitionVersionRequestRequestTypeDef,
-):
-    pass
-
-
 ResourceDefinitionVersionTypeDef = TypedDict(
     "ResourceDefinitionVersionTypeDef",
     {
         "Resources": Sequence[ResourceTypeDef],
     },
     total=False,
 )
 
+ResourceUnionTypeDef = Union[ResourceTypeDef, ResourceOutputTypeDef]
 FunctionDefinitionVersionOutputTypeDef = TypedDict(
     "FunctionDefinitionVersionOutputTypeDef",
     {
         "DefaultConfig": FunctionDefaultConfigTypeDef,
         "Functions": List[FunctionOutputTypeDef],
     },
     total=False,
 )
 
-_RequiredCreateFunctionDefinitionVersionRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateFunctionDefinitionVersionRequestRequestTypeDef",
-    {
-        "FunctionDefinitionId": str,
-    },
-)
-_OptionalCreateFunctionDefinitionVersionRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateFunctionDefinitionVersionRequestRequestTypeDef",
-    {
-        "AmznClientToken": str,
-        "DefaultConfig": FunctionDefaultConfigTypeDef,
-        "Functions": Sequence[Union[FunctionTypeDef, FunctionOutputTypeDef]],
-    },
-    total=False,
-)
-
-
-class CreateFunctionDefinitionVersionRequestRequestTypeDef(
-    _RequiredCreateFunctionDefinitionVersionRequestRequestTypeDef,
-    _OptionalCreateFunctionDefinitionVersionRequestRequestTypeDef,
-):
-    pass
-
-
 FunctionDefinitionVersionTypeDef = TypedDict(
     "FunctionDefinitionVersionTypeDef",
     {
         "DefaultConfig": FunctionDefaultConfigTypeDef,
         "Functions": Sequence[FunctionTypeDef],
     },
     total=False,
 )
 
+FunctionUnionTypeDef = Union[FunctionTypeDef, FunctionOutputTypeDef]
 GetResourceDefinitionVersionResponseTypeDef = TypedDict(
     "GetResourceDefinitionVersionResponseTypeDef",
     {
         "Arn": str,
         "CreationTimestamp": str,
         "Definition": ResourceDefinitionVersionOutputTypeDef,
         "Id": str,
@@ -3353,14 +3334,40 @@
         "InitialVersion": ResourceDefinitionVersionTypeDef,
         "Name": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+ResourceDefinitionVersionUnionTypeDef = Union[
+    ResourceDefinitionVersionTypeDef, ResourceDefinitionVersionOutputTypeDef
+]
+_RequiredCreateResourceDefinitionVersionRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateResourceDefinitionVersionRequestRequestTypeDef",
+    {
+        "ResourceDefinitionId": str,
+    },
+)
+_OptionalCreateResourceDefinitionVersionRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateResourceDefinitionVersionRequestRequestTypeDef",
+    {
+        "AmznClientToken": str,
+        "Resources": Sequence[ResourceUnionTypeDef],
+    },
+    total=False,
+)
+
+
+class CreateResourceDefinitionVersionRequestRequestTypeDef(
+    _RequiredCreateResourceDefinitionVersionRequestRequestTypeDef,
+    _OptionalCreateResourceDefinitionVersionRequestRequestTypeDef,
+):
+    pass
+
+
 GetFunctionDefinitionVersionResponseTypeDef = TypedDict(
     "GetFunctionDefinitionVersionResponseTypeDef",
     {
         "Arn": str,
         "CreationTimestamp": str,
         "Definition": FunctionDefinitionVersionOutputTypeDef,
         "Id": str,
@@ -3376,7 +3383,33 @@
         "AmznClientToken": str,
         "InitialVersion": FunctionDefinitionVersionTypeDef,
         "Name": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
+
+FunctionDefinitionVersionUnionTypeDef = Union[
+    FunctionDefinitionVersionTypeDef, FunctionDefinitionVersionOutputTypeDef
+]
+_RequiredCreateFunctionDefinitionVersionRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateFunctionDefinitionVersionRequestRequestTypeDef",
+    {
+        "FunctionDefinitionId": str,
+    },
+)
+_OptionalCreateFunctionDefinitionVersionRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateFunctionDefinitionVersionRequestRequestTypeDef",
+    {
+        "AmznClientToken": str,
+        "DefaultConfig": FunctionDefaultConfigTypeDef,
+        "Functions": Sequence[FunctionUnionTypeDef],
+    },
+    total=False,
+)
+
+
+class CreateFunctionDefinitionVersionRequestRequestTypeDef(
+    _RequiredCreateFunctionDefinitionVersionRequestRequestTypeDef,
+    _OptionalCreateFunctionDefinitionVersionRequestRequestTypeDef,
+):
+    pass
```

### Comparing `mypy-boto3-greengrass-1.28.15.post1/mypy_boto3_greengrass/type_defs.pyi` & `mypy-boto3-greengrass-1.28.16/mypy_boto3_greengrass/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_greengrass.type_defs import AssociateRoleToGroupRequestRequestTypeDef
 
-    data: AssociateRoleToGroupRequestRequestTypeDef = {...}
+    data: AssociateRoleToGroupRequestRequestTypeDef = ...
     ```
 """
 import sys
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     BulkDeploymentStatusType,
@@ -181,15 +181,15 @@
     "GetBulkDeploymentStatusResponseTypeDef",
     "GetDeploymentStatusResponseTypeDef",
     "ListBulkDeploymentsResponseTypeDef",
     "GetConnectivityInfoResponseTypeDef",
     "UpdateConnectivityInfoRequestRequestTypeDef",
     "ConnectorDefinitionVersionOutputTypeDef",
     "ConnectorDefinitionVersionTypeDef",
-    "CreateConnectorDefinitionVersionRequestRequestTypeDef",
+    "ConnectorUnionTypeDef",
     "CoreDefinitionVersionOutputTypeDef",
     "CoreDefinitionVersionTypeDef",
     "CreateCoreDefinitionVersionRequestRequestTypeDef",
     "CreateDeviceDefinitionVersionRequestRequestTypeDef",
     "DeviceDefinitionVersionOutputTypeDef",
     "DeviceDefinitionVersionTypeDef",
     "CreateGroupRequestRequestTypeDef",
@@ -243,45 +243,55 @@
     "ListSubscriptionDefinitionVersionsResponseTypeDef",
     "S3MachineLearningModelResourceDataTypeDef",
     "SageMakerMachineLearningModelResourceDataTypeDef",
     "RuntimeConfigurationTypeDef",
     "UpdateThingRuntimeConfigurationRequestRequestTypeDef",
     "ListBulkDeploymentDetailedReportsResponseTypeDef",
     "GetConnectorDefinitionVersionResponseTypeDef",
+    "ConnectorDefinitionVersionUnionTypeDef",
     "CreateConnectorDefinitionRequestRequestTypeDef",
+    "CreateConnectorDefinitionVersionRequestRequestTypeDef",
     "GetCoreDefinitionVersionResponseTypeDef",
+    "CoreDefinitionVersionUnionTypeDef",
     "CreateCoreDefinitionRequestRequestTypeDef",
     "GetDeviceDefinitionVersionResponseTypeDef",
     "CreateDeviceDefinitionRequestRequestTypeDef",
+    "DeviceDefinitionVersionUnionTypeDef",
     "GetLoggerDefinitionVersionResponseTypeDef",
     "CreateLoggerDefinitionRequestRequestTypeDef",
+    "LoggerDefinitionVersionUnionTypeDef",
     "GetSubscriptionDefinitionVersionResponseTypeDef",
     "CreateSubscriptionDefinitionRequestRequestTypeDef",
+    "SubscriptionDefinitionVersionUnionTypeDef",
     "FunctionDefaultConfigTypeDef",
     "FunctionConfigurationEnvironmentOutputTypeDef",
     "FunctionConfigurationEnvironmentTypeDef",
     "ResourceDataContainerOutputTypeDef",
     "ResourceDataContainerTypeDef",
     "GetThingRuntimeConfigurationResponseTypeDef",
     "FunctionConfigurationOutputTypeDef",
     "FunctionConfigurationTypeDef",
     "ResourceOutputTypeDef",
     "ResourceTypeDef",
     "FunctionOutputTypeDef",
     "FunctionTypeDef",
     "ResourceDefinitionVersionOutputTypeDef",
-    "CreateResourceDefinitionVersionRequestRequestTypeDef",
     "ResourceDefinitionVersionTypeDef",
+    "ResourceUnionTypeDef",
     "FunctionDefinitionVersionOutputTypeDef",
-    "CreateFunctionDefinitionVersionRequestRequestTypeDef",
     "FunctionDefinitionVersionTypeDef",
+    "FunctionUnionTypeDef",
     "GetResourceDefinitionVersionResponseTypeDef",
     "CreateResourceDefinitionRequestRequestTypeDef",
+    "ResourceDefinitionVersionUnionTypeDef",
+    "CreateResourceDefinitionVersionRequestRequestTypeDef",
     "GetFunctionDefinitionVersionResponseTypeDef",
     "CreateFunctionDefinitionRequestRequestTypeDef",
+    "FunctionDefinitionVersionUnionTypeDef",
+    "CreateFunctionDefinitionVersionRequestRequestTypeDef",
 )
 
 AssociateRoleToGroupRequestRequestTypeDef = TypedDict(
     "AssociateRoleToGroupRequestRequestTypeDef",
     {
         "GroupId": str,
         "RoleArn": str,
@@ -2134,35 +2144,15 @@
     "ConnectorDefinitionVersionTypeDef",
     {
         "Connectors": Sequence[ConnectorTypeDef],
     },
     total=False,
 )
 
-_RequiredCreateConnectorDefinitionVersionRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateConnectorDefinitionVersionRequestRequestTypeDef",
-    {
-        "ConnectorDefinitionId": str,
-    },
-)
-_OptionalCreateConnectorDefinitionVersionRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateConnectorDefinitionVersionRequestRequestTypeDef",
-    {
-        "AmznClientToken": str,
-        "Connectors": Sequence[Union[ConnectorTypeDef, ConnectorOutputTypeDef]],
-    },
-    total=False,
-)
-
-class CreateConnectorDefinitionVersionRequestRequestTypeDef(
-    _RequiredCreateConnectorDefinitionVersionRequestRequestTypeDef,
-    _OptionalCreateConnectorDefinitionVersionRequestRequestTypeDef,
-):
-    pass
-
+ConnectorUnionTypeDef = Union[ConnectorTypeDef, ConnectorOutputTypeDef]
 CoreDefinitionVersionOutputTypeDef = TypedDict(
     "CoreDefinitionVersionOutputTypeDef",
     {
         "Cores": List[CoreTypeDef],
     },
     total=False,
 )
@@ -2876,38 +2866,65 @@
         "Id": str,
         "NextToken": str,
         "Version": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ConnectorDefinitionVersionUnionTypeDef = Union[
+    ConnectorDefinitionVersionTypeDef, ConnectorDefinitionVersionOutputTypeDef
+]
 CreateConnectorDefinitionRequestRequestTypeDef = TypedDict(
     "CreateConnectorDefinitionRequestRequestTypeDef",
     {
         "AmznClientToken": str,
         "InitialVersion": ConnectorDefinitionVersionTypeDef,
         "Name": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+_RequiredCreateConnectorDefinitionVersionRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateConnectorDefinitionVersionRequestRequestTypeDef",
+    {
+        "ConnectorDefinitionId": str,
+    },
+)
+_OptionalCreateConnectorDefinitionVersionRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateConnectorDefinitionVersionRequestRequestTypeDef",
+    {
+        "AmznClientToken": str,
+        "Connectors": Sequence[ConnectorUnionTypeDef],
+    },
+    total=False,
+)
+
+class CreateConnectorDefinitionVersionRequestRequestTypeDef(
+    _RequiredCreateConnectorDefinitionVersionRequestRequestTypeDef,
+    _OptionalCreateConnectorDefinitionVersionRequestRequestTypeDef,
+):
+    pass
+
 GetCoreDefinitionVersionResponseTypeDef = TypedDict(
     "GetCoreDefinitionVersionResponseTypeDef",
     {
         "Arn": str,
         "CreationTimestamp": str,
         "Definition": CoreDefinitionVersionOutputTypeDef,
         "Id": str,
         "NextToken": str,
         "Version": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+CoreDefinitionVersionUnionTypeDef = Union[
+    CoreDefinitionVersionTypeDef, CoreDefinitionVersionOutputTypeDef
+]
 CreateCoreDefinitionRequestRequestTypeDef = TypedDict(
     "CreateCoreDefinitionRequestRequestTypeDef",
     {
         "AmznClientToken": str,
         "InitialVersion": CoreDefinitionVersionTypeDef,
         "Name": str,
         "tags": Mapping[str, str],
@@ -2935,14 +2952,17 @@
         "InitialVersion": DeviceDefinitionVersionTypeDef,
         "Name": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+DeviceDefinitionVersionUnionTypeDef = Union[
+    DeviceDefinitionVersionTypeDef, DeviceDefinitionVersionOutputTypeDef
+]
 GetLoggerDefinitionVersionResponseTypeDef = TypedDict(
     "GetLoggerDefinitionVersionResponseTypeDef",
     {
         "Arn": str,
         "CreationTimestamp": str,
         "Definition": LoggerDefinitionVersionOutputTypeDef,
         "Id": str,
@@ -2958,14 +2978,17 @@
         "InitialVersion": LoggerDefinitionVersionTypeDef,
         "Name": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+LoggerDefinitionVersionUnionTypeDef = Union[
+    LoggerDefinitionVersionTypeDef, LoggerDefinitionVersionOutputTypeDef
+]
 GetSubscriptionDefinitionVersionResponseTypeDef = TypedDict(
     "GetSubscriptionDefinitionVersionResponseTypeDef",
     {
         "Arn": str,
         "CreationTimestamp": str,
         "Definition": SubscriptionDefinitionVersionOutputTypeDef,
         "Id": str,
@@ -2982,14 +3005,17 @@
         "InitialVersion": SubscriptionDefinitionVersionTypeDef,
         "Name": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+SubscriptionDefinitionVersionUnionTypeDef = Union[
+    SubscriptionDefinitionVersionTypeDef, SubscriptionDefinitionVersionOutputTypeDef
+]
 FunctionDefaultConfigTypeDef = TypedDict(
     "FunctionDefaultConfigTypeDef",
     {
         "Execution": FunctionDefaultExecutionConfigTypeDef,
     },
     total=False,
 )
@@ -3140,83 +3166,42 @@
     "ResourceDefinitionVersionOutputTypeDef",
     {
         "Resources": List[ResourceOutputTypeDef],
     },
     total=False,
 )
 
-_RequiredCreateResourceDefinitionVersionRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateResourceDefinitionVersionRequestRequestTypeDef",
-    {
-        "ResourceDefinitionId": str,
-    },
-)
-_OptionalCreateResourceDefinitionVersionRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateResourceDefinitionVersionRequestRequestTypeDef",
-    {
-        "AmznClientToken": str,
-        "Resources": Sequence[Union[ResourceTypeDef, ResourceOutputTypeDef]],
-    },
-    total=False,
-)
-
-class CreateResourceDefinitionVersionRequestRequestTypeDef(
-    _RequiredCreateResourceDefinitionVersionRequestRequestTypeDef,
-    _OptionalCreateResourceDefinitionVersionRequestRequestTypeDef,
-):
-    pass
-
 ResourceDefinitionVersionTypeDef = TypedDict(
     "ResourceDefinitionVersionTypeDef",
     {
         "Resources": Sequence[ResourceTypeDef],
     },
     total=False,
 )
 
+ResourceUnionTypeDef = Union[ResourceTypeDef, ResourceOutputTypeDef]
 FunctionDefinitionVersionOutputTypeDef = TypedDict(
     "FunctionDefinitionVersionOutputTypeDef",
     {
         "DefaultConfig": FunctionDefaultConfigTypeDef,
         "Functions": List[FunctionOutputTypeDef],
     },
     total=False,
 )
 
-_RequiredCreateFunctionDefinitionVersionRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateFunctionDefinitionVersionRequestRequestTypeDef",
-    {
-        "FunctionDefinitionId": str,
-    },
-)
-_OptionalCreateFunctionDefinitionVersionRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateFunctionDefinitionVersionRequestRequestTypeDef",
-    {
-        "AmznClientToken": str,
-        "DefaultConfig": FunctionDefaultConfigTypeDef,
-        "Functions": Sequence[Union[FunctionTypeDef, FunctionOutputTypeDef]],
-    },
-    total=False,
-)
-
-class CreateFunctionDefinitionVersionRequestRequestTypeDef(
-    _RequiredCreateFunctionDefinitionVersionRequestRequestTypeDef,
-    _OptionalCreateFunctionDefinitionVersionRequestRequestTypeDef,
-):
-    pass
-
 FunctionDefinitionVersionTypeDef = TypedDict(
     "FunctionDefinitionVersionTypeDef",
     {
         "DefaultConfig": FunctionDefaultConfigTypeDef,
         "Functions": Sequence[FunctionTypeDef],
     },
     total=False,
 )
 
+FunctionUnionTypeDef = Union[FunctionTypeDef, FunctionOutputTypeDef]
 GetResourceDefinitionVersionResponseTypeDef = TypedDict(
     "GetResourceDefinitionVersionResponseTypeDef",
     {
         "Arn": str,
         "CreationTimestamp": str,
         "Definition": ResourceDefinitionVersionOutputTypeDef,
         "Id": str,
@@ -3232,14 +3217,38 @@
         "InitialVersion": ResourceDefinitionVersionTypeDef,
         "Name": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+ResourceDefinitionVersionUnionTypeDef = Union[
+    ResourceDefinitionVersionTypeDef, ResourceDefinitionVersionOutputTypeDef
+]
+_RequiredCreateResourceDefinitionVersionRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateResourceDefinitionVersionRequestRequestTypeDef",
+    {
+        "ResourceDefinitionId": str,
+    },
+)
+_OptionalCreateResourceDefinitionVersionRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateResourceDefinitionVersionRequestRequestTypeDef",
+    {
+        "AmznClientToken": str,
+        "Resources": Sequence[ResourceUnionTypeDef],
+    },
+    total=False,
+)
+
+class CreateResourceDefinitionVersionRequestRequestTypeDef(
+    _RequiredCreateResourceDefinitionVersionRequestRequestTypeDef,
+    _OptionalCreateResourceDefinitionVersionRequestRequestTypeDef,
+):
+    pass
+
 GetFunctionDefinitionVersionResponseTypeDef = TypedDict(
     "GetFunctionDefinitionVersionResponseTypeDef",
     {
         "Arn": str,
         "CreationTimestamp": str,
         "Definition": FunctionDefinitionVersionOutputTypeDef,
         "Id": str,
@@ -3255,7 +3264,32 @@
         "AmznClientToken": str,
         "InitialVersion": FunctionDefinitionVersionTypeDef,
         "Name": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
+
+FunctionDefinitionVersionUnionTypeDef = Union[
+    FunctionDefinitionVersionTypeDef, FunctionDefinitionVersionOutputTypeDef
+]
+_RequiredCreateFunctionDefinitionVersionRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateFunctionDefinitionVersionRequestRequestTypeDef",
+    {
+        "FunctionDefinitionId": str,
+    },
+)
+_OptionalCreateFunctionDefinitionVersionRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateFunctionDefinitionVersionRequestRequestTypeDef",
+    {
+        "AmznClientToken": str,
+        "DefaultConfig": FunctionDefaultConfigTypeDef,
+        "Functions": Sequence[FunctionUnionTypeDef],
+    },
+    total=False,
+)
+
+class CreateFunctionDefinitionVersionRequestRequestTypeDef(
+    _RequiredCreateFunctionDefinitionVersionRequestRequestTypeDef,
+    _OptionalCreateFunctionDefinitionVersionRequestRequestTypeDef,
+):
+    pass
```

### Comparing `mypy-boto3-greengrass-1.28.15.post1/mypy_boto3_greengrass.egg-info/PKG-INFO` & `mypy-boto3-greengrass-1.28.16/mypy_boto3_greengrass.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-greengrass
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.Greengrass 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.Greengrass 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 greengrass type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 greengrass type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-greengrass.svg?color=blue)](https://pypi.org/project/mypy-boto3-greengrass)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-greengrass)](https://pepy.tech/project/mypy-boto3-greengrass)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Greengrass 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass)
+[boto3.Greengrass 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#Greengrass)
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
 [mypy-boto3-greengrass docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/).
 
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
@@ -413,20 +413,20 @@
 )
 
 
 def check_value(value: BulkDeploymentStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_greengrass.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_greengrass.type_defs import (
     AssociateRoleToGroupRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     AssociateServiceRoleToAccountRequestRequestTypeDef,
     BulkDeploymentMetricsTypeDef,
@@ -570,15 +570,15 @@
     GetBulkDeploymentStatusResponseTypeDef,
     GetDeploymentStatusResponseTypeDef,
     ListBulkDeploymentsResponseTypeDef,
     GetConnectivityInfoResponseTypeDef,
     UpdateConnectivityInfoRequestRequestTypeDef,
     ConnectorDefinitionVersionOutputTypeDef,
     ConnectorDefinitionVersionTypeDef,
-    CreateConnectorDefinitionVersionRequestRequestTypeDef,
+    ConnectorUnionTypeDef,
     CoreDefinitionVersionOutputTypeDef,
     CoreDefinitionVersionTypeDef,
     CreateCoreDefinitionVersionRequestRequestTypeDef,
     CreateDeviceDefinitionVersionRequestRequestTypeDef,
     DeviceDefinitionVersionOutputTypeDef,
     DeviceDefinitionVersionTypeDef,
     CreateGroupRequestRequestTypeDef,
@@ -632,49 +632,59 @@
     ListSubscriptionDefinitionVersionsResponseTypeDef,
     S3MachineLearningModelResourceDataTypeDef,
     SageMakerMachineLearningModelResourceDataTypeDef,
     RuntimeConfigurationTypeDef,
     UpdateThingRuntimeConfigurationRequestRequestTypeDef,
     ListBulkDeploymentDetailedReportsResponseTypeDef,
     GetConnectorDefinitionVersionResponseTypeDef,
+    ConnectorDefinitionVersionUnionTypeDef,
     CreateConnectorDefinitionRequestRequestTypeDef,
+    CreateConnectorDefinitionVersionRequestRequestTypeDef,
     GetCoreDefinitionVersionResponseTypeDef,
+    CoreDefinitionVersionUnionTypeDef,
     CreateCoreDefinitionRequestRequestTypeDef,
     GetDeviceDefinitionVersionResponseTypeDef,
     CreateDeviceDefinitionRequestRequestTypeDef,
+    DeviceDefinitionVersionUnionTypeDef,
     GetLoggerDefinitionVersionResponseTypeDef,
     CreateLoggerDefinitionRequestRequestTypeDef,
+    LoggerDefinitionVersionUnionTypeDef,
     GetSubscriptionDefinitionVersionResponseTypeDef,
     CreateSubscriptionDefinitionRequestRequestTypeDef,
+    SubscriptionDefinitionVersionUnionTypeDef,
     FunctionDefaultConfigTypeDef,
     FunctionConfigurationEnvironmentOutputTypeDef,
     FunctionConfigurationEnvironmentTypeDef,
     ResourceDataContainerOutputTypeDef,
     ResourceDataContainerTypeDef,
     GetThingRuntimeConfigurationResponseTypeDef,
     FunctionConfigurationOutputTypeDef,
     FunctionConfigurationTypeDef,
     ResourceOutputTypeDef,
     ResourceTypeDef,
     FunctionOutputTypeDef,
     FunctionTypeDef,
     ResourceDefinitionVersionOutputTypeDef,
-    CreateResourceDefinitionVersionRequestRequestTypeDef,
     ResourceDefinitionVersionTypeDef,
+    ResourceUnionTypeDef,
     FunctionDefinitionVersionOutputTypeDef,
-    CreateFunctionDefinitionVersionRequestRequestTypeDef,
     FunctionDefinitionVersionTypeDef,
+    FunctionUnionTypeDef,
     GetResourceDefinitionVersionResponseTypeDef,
     CreateResourceDefinitionRequestRequestTypeDef,
+    ResourceDefinitionVersionUnionTypeDef,
+    CreateResourceDefinitionVersionRequestRequestTypeDef,
     GetFunctionDefinitionVersionResponseTypeDef,
     CreateFunctionDefinitionRequestRequestTypeDef,
+    FunctionDefinitionVersionUnionTypeDef,
+    CreateFunctionDefinitionVersionRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AssociateRoleToGroupRequestRequestTypeDef:
+def get_value() -> AssociateRoleToGroupRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-greengrass-1.28.15.post1/mypy_boto3_greengrass.egg-info/SOURCES.txt` & `mypy-boto3-greengrass-1.28.16/mypy_boto3_greengrass.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-greengrass-1.28.15.post1/setup.py` & `mypy-boto3-greengrass-1.28.16/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-greengrass",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_greengrass"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Greengrass 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.2"
+        "Type annotations for boto3.Greengrass 1.28.16 service generated with mypy-boto3-builder"
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
-    keywords="boto3 greengrass type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 greengrass type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_greengrass": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrass/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

