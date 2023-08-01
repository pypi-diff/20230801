# Comparing `tmp/mypy-boto3-greengrassv2-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-greengrassv2-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-greengrassv2-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:13 2023, max compression
+gzip compressed data, was "mypy-boto3-greengrassv2-1.28.16.tar", last modified: Tue Aug  1 11:36:52 2023, max compression
```

## Comparing `mypy-boto3-greengrassv2-1.28.15.post1.tar` & `mypy-boto3-greengrassv2-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:13.225168 mypy-boto3-greengrassv2-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:46:38.000000 mypy-boto3-greengrassv2-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19305 2023-07-29 10:03:13.225168 mypy-boto3-greengrassv2-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17792 2023-07-29 09:46:38.000000 mypy-boto3-greengrassv2-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:13.221168 mypy-boto3-greengrassv2-1.28.15.post1/mypy_boto3_greengrassv2/
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-07-29 09:46:38.000000 mypy-boto3-greengrassv2-1.28.15.post1/mypy_boto3_greengrassv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-07-29 09:46:38.000000 mypy-boto3-greengrassv2-1.28.15.post1/mypy_boto3_greengrassv2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-29 09:46:38.000000 mypy-boto3-greengrassv2-1.28.15.post1/mypy_boto3_greengrassv2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26049 2023-07-29 09:46:39.000000 mypy-boto3-greengrassv2-1.28.15.post1/mypy_boto3_greengrassv2/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    26006 2023-07-29 09:46:38.000000 mypy-boto3-greengrassv2-1.28.15.post1/mypy_boto3_greengrassv2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11123 2023-07-29 09:46:39.000000 mypy-boto3-greengrassv2-1.28.15.post1/mypy_boto3_greengrassv2/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11121 2023-07-29 09:46:39.000000 mypy-boto3-greengrassv2-1.28.15.post1/mypy_boto3_greengrassv2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9476 2023-07-29 09:46:39.000000 mypy-boto3-greengrassv2-1.28.15.post1/mypy_boto3_greengrassv2/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9467 2023-07-29 09:46:39.000000 mypy-boto3-greengrassv2-1.28.15.post1/mypy_boto3_greengrassv2/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:46:38.000000 mypy-boto3-greengrassv2-1.28.15.post1/mypy_boto3_greengrassv2/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    38670 2023-07-29 09:46:40.000000 mypy-boto3-greengrassv2-1.28.15.post1/mypy_boto3_greengrassv2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    38637 2023-07-29 09:46:39.000000 mypy-boto3-greengrassv2-1.28.15.post1/mypy_boto3_greengrassv2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:46:38.000000 mypy-boto3-greengrassv2-1.28.15.post1/mypy_boto3_greengrassv2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:13.225168 mypy-boto3-greengrassv2-1.28.15.post1/mypy_boto3_greengrassv2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19305 2023-07-29 10:03:12.000000 mypy-boto3-greengrassv2-1.28.15.post1/mypy_boto3_greengrassv2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-29 10:03:13.000000 mypy-boto3-greengrassv2-1.28.15.post1/mypy_boto3_greengrassv2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:12.000000 mypy-boto3-greengrassv2-1.28.15.post1/mypy_boto3_greengrassv2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:12.000000 mypy-boto3-greengrassv2-1.28.15.post1/mypy_boto3_greengrassv2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:12.000000 mypy-boto3-greengrassv2-1.28.15.post1/mypy_boto3_greengrassv2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-29 10:03:12.000000 mypy-boto3-greengrassv2-1.28.15.post1/mypy_boto3_greengrassv2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:13.225168 mypy-boto3-greengrassv2-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-07-29 09:46:38.000000 mypy-boto3-greengrassv2-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:52.832880 mypy-boto3-greengrassv2-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:19:16.000000 mypy-boto3-greengrassv2-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19444 2023-08-01 11:36:52.832880 mypy-boto3-greengrassv2-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17940 2023-08-01 11:19:16.000000 mypy-boto3-greengrassv2-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:52.832880 mypy-boto3-greengrassv2-1.28.16/mypy_boto3_greengrassv2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-08-01 11:19:16.000000 mypy-boto3-greengrassv2-1.28.16/mypy_boto3_greengrassv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-08-01 11:19:16.000000 mypy-boto3-greengrassv2-1.28.16/mypy_boto3_greengrassv2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-08-01 11:19:16.000000 mypy-boto3-greengrassv2-1.28.16/mypy_boto3_greengrassv2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25628 2023-08-01 11:19:16.000000 mypy-boto3-greengrassv2-1.28.16/mypy_boto3_greengrassv2/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25585 2023-08-01 11:19:16.000000 mypy-boto3-greengrassv2-1.28.16/mypy_boto3_greengrassv2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11123 2023-08-01 11:19:17.000000 mypy-boto3-greengrassv2-1.28.16/mypy_boto3_greengrassv2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11121 2023-08-01 11:19:16.000000 mypy-boto3-greengrassv2-1.28.16/mypy_boto3_greengrassv2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9476 2023-08-01 11:19:16.000000 mypy-boto3-greengrassv2-1.28.16/mypy_boto3_greengrassv2/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9467 2023-08-01 11:19:16.000000 mypy-boto3-greengrassv2-1.28.16/mypy_boto3_greengrassv2/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:19:16.000000 mypy-boto3-greengrassv2-1.28.16/mypy_boto3_greengrassv2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    39101 2023-08-01 11:19:18.000000 mypy-boto3-greengrassv2-1.28.16/mypy_boto3_greengrassv2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39068 2023-08-01 11:19:17.000000 mypy-boto3-greengrassv2-1.28.16/mypy_boto3_greengrassv2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:19:16.000000 mypy-boto3-greengrassv2-1.28.16/mypy_boto3_greengrassv2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:52.832880 mypy-boto3-greengrassv2-1.28.16/mypy_boto3_greengrassv2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19444 2023-08-01 11:36:52.000000 mypy-boto3-greengrassv2-1.28.16/mypy_boto3_greengrassv2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-08-01 11:36:52.000000 mypy-boto3-greengrassv2-1.28.16/mypy_boto3_greengrassv2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:52.000000 mypy-boto3-greengrassv2-1.28.16/mypy_boto3_greengrassv2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:52.000000 mypy-boto3-greengrassv2-1.28.16/mypy_boto3_greengrassv2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:52.000000 mypy-boto3-greengrassv2-1.28.16/mypy_boto3_greengrassv2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-01 11:36:52.000000 mypy-boto3-greengrassv2-1.28.16/mypy_boto3_greengrassv2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:52.832880 mypy-boto3-greengrassv2-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-08-01 11:19:16.000000 mypy-boto3-greengrassv2-1.28.16/setup.py
```

### Comparing `mypy-boto3-greengrassv2-1.28.15.post1/LICENSE` & `mypy-boto3-greengrassv2-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-greengrassv2-1.28.15.post1/PKG-INFO` & `mypy-boto3-greengrassv2-1.28.16/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-greengrassv2
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.GreengrassV2 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.GreengrassV2 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 greengrassv2 type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 greengrassv2 type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-greengrassv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-greengrassv2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-greengrassv2)](https://pepy.tech/project/mypy-boto3-greengrassv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.GreengrassV2 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2)
+[boto3.GreengrassV2 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2)
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
 [mypy-boto3-greengrassv2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/).
 
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
@@ -357,30 +357,31 @@
 )
 
 
 def check_value(value: CloudComponentStateType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_greengrassv2.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_greengrassv2.type_defs import (
     AssociateClientDeviceWithCoreDeviceEntryTypeDef,
     AssociateClientDeviceWithCoreDeviceErrorEntryTypeDef,
     AssociateServiceRoleToAccountRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     AssociatedClientDeviceTypeDef,
     DisassociateClientDeviceFromCoreDeviceEntryTypeDef,
     DisassociateClientDeviceFromCoreDeviceErrorEntryTypeDef,
+    BlobTypeDef,
     CancelDeploymentRequestRequestTypeDef,
     CloudComponentStatusTypeDef,
     ComponentCandidateTypeDef,
     ComponentConfigurationUpdateOutputTypeDef,
     ComponentConfigurationUpdateTypeDef,
     ComponentDependencyRequirementTypeDef,
     ComponentPlatformOutputTypeDef,
@@ -436,14 +437,15 @@
     UpdateConnectivityInfoResponseTypeDef,
     ListClientDevicesAssociatedWithCoreDeviceResponseTypeDef,
     BatchDisassociateClientDeviceFromCoreDeviceRequestRequestTypeDef,
     BatchDisassociateClientDeviceFromCoreDeviceResponseTypeDef,
     CreateComponentVersionResponseTypeDef,
     ComponentLatestVersionTypeDef,
     DescribeComponentResponseTypeDef,
+    ComponentPlatformUnionTypeDef,
     ResolveComponentCandidatesRequestRequestTypeDef,
     ComponentRunWithTypeDef,
     ListComponentVersionsResponseTypeDef,
     GetConnectivityInfoResponseTypeDef,
     UpdateConnectivityInfoRequestRequestTypeDef,
     ListCoreDevicesResponseTypeDef,
     DeploymentPoliciesTypeDef,
@@ -465,25 +467,27 @@
     ComponentTypeDef,
     ComponentDeploymentSpecificationOutputTypeDef,
     ComponentDeploymentSpecificationTypeDef,
     ListEffectiveDeploymentsResponseTypeDef,
     IoTJobExecutionsRolloutConfigTypeDef,
     LambdaLinuxProcessParamsTypeDef,
     ListComponentsResponseTypeDef,
+    ComponentDeploymentSpecificationUnionTypeDef,
     DeploymentIoTJobConfigurationOutputTypeDef,
     DeploymentIoTJobConfigurationTypeDef,
     LambdaExecutionParametersTypeDef,
     GetDeploymentResponseTypeDef,
     CreateDeploymentRequestRequestTypeDef,
+    DeploymentIoTJobConfigurationUnionTypeDef,
     LambdaFunctionRecipeSourceTypeDef,
     CreateComponentVersionRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AssociateClientDeviceWithCoreDeviceEntryTypeDef:
+def get_value() -> AssociateClientDeviceWithCoreDeviceEntryTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-greengrassv2-1.28.15.post1/README.md` & `mypy-boto3-greengrassv2-1.28.16/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-greengrassv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-greengrassv2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-greengrassv2)](https://pepy.tech/project/mypy-boto3-greengrassv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.GreengrassV2 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2)
+[boto3.GreengrassV2 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2)
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
 [mypy-boto3-greengrassv2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/).
 
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
@@ -325,30 +325,31 @@
 )
 
 
 def check_value(value: CloudComponentStateType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_greengrassv2.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_greengrassv2.type_defs import (
     AssociateClientDeviceWithCoreDeviceEntryTypeDef,
     AssociateClientDeviceWithCoreDeviceErrorEntryTypeDef,
     AssociateServiceRoleToAccountRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     AssociatedClientDeviceTypeDef,
     DisassociateClientDeviceFromCoreDeviceEntryTypeDef,
     DisassociateClientDeviceFromCoreDeviceErrorEntryTypeDef,
+    BlobTypeDef,
     CancelDeploymentRequestRequestTypeDef,
     CloudComponentStatusTypeDef,
     ComponentCandidateTypeDef,
     ComponentConfigurationUpdateOutputTypeDef,
     ComponentConfigurationUpdateTypeDef,
     ComponentDependencyRequirementTypeDef,
     ComponentPlatformOutputTypeDef,
@@ -404,14 +405,15 @@
     UpdateConnectivityInfoResponseTypeDef,
     ListClientDevicesAssociatedWithCoreDeviceResponseTypeDef,
     BatchDisassociateClientDeviceFromCoreDeviceRequestRequestTypeDef,
     BatchDisassociateClientDeviceFromCoreDeviceResponseTypeDef,
     CreateComponentVersionResponseTypeDef,
     ComponentLatestVersionTypeDef,
     DescribeComponentResponseTypeDef,
+    ComponentPlatformUnionTypeDef,
     ResolveComponentCandidatesRequestRequestTypeDef,
     ComponentRunWithTypeDef,
     ListComponentVersionsResponseTypeDef,
     GetConnectivityInfoResponseTypeDef,
     UpdateConnectivityInfoRequestRequestTypeDef,
     ListCoreDevicesResponseTypeDef,
     DeploymentPoliciesTypeDef,
@@ -433,25 +435,27 @@
     ComponentTypeDef,
     ComponentDeploymentSpecificationOutputTypeDef,
     ComponentDeploymentSpecificationTypeDef,
     ListEffectiveDeploymentsResponseTypeDef,
     IoTJobExecutionsRolloutConfigTypeDef,
     LambdaLinuxProcessParamsTypeDef,
     ListComponentsResponseTypeDef,
+    ComponentDeploymentSpecificationUnionTypeDef,
     DeploymentIoTJobConfigurationOutputTypeDef,
     DeploymentIoTJobConfigurationTypeDef,
     LambdaExecutionParametersTypeDef,
     GetDeploymentResponseTypeDef,
     CreateDeploymentRequestRequestTypeDef,
+    DeploymentIoTJobConfigurationUnionTypeDef,
     LambdaFunctionRecipeSourceTypeDef,
     CreateComponentVersionRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AssociateClientDeviceWithCoreDeviceEntryTypeDef:
+def get_value() -> AssociateClientDeviceWithCoreDeviceEntryTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-greengrassv2-1.28.15.post1/mypy_boto3_greengrassv2/__init__.py` & `mypy-boto3-greengrassv2-1.28.16/mypy_boto3_greengrassv2/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-greengrassv2-1.28.15.post1/mypy_boto3_greengrassv2/__init__.pyi` & `mypy-boto3-greengrassv2-1.28.16/mypy_boto3_greengrassv2/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-greengrassv2-1.28.15.post1/mypy_boto3_greengrassv2/__main__.py` & `mypy-boto3-greengrassv2-1.28.16/mypy_boto3_greengrassv2/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.GreengrassV2 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.GreengrassV2 1.28.16\nVersion:         1.28.16\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2\nOther"
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

### Comparing `mypy-boto3-greengrassv2-1.28.15.post1/mypy_boto3_greengrassv2/client.py` & `mypy-boto3-greengrassv2-1.28.16/mypy_boto3_greengrassv2/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,18 +10,17 @@
     from mypy_boto3_greengrassv2.client import GreengrassV2Client
 
     session = Session()
     client: GreengrassV2Client = session.client("greengrassv2")
     ```
 """
 import sys
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
-from botocore.response import StreamingBody
 
 from .literals import (
     ComponentVisibilityScopeType,
     CoreDeviceStatusType,
     DeploymentHistoryFilterType,
     InstalledComponentTopologyFilterType,
     RecipeOutputFormatType,
@@ -36,25 +35,23 @@
     ListInstalledComponentsPaginator,
 )
 from .type_defs import (
     AssociateClientDeviceWithCoreDeviceEntryTypeDef,
     AssociateServiceRoleToAccountResponseTypeDef,
     BatchAssociateClientDeviceWithCoreDeviceResponseTypeDef,
     BatchDisassociateClientDeviceFromCoreDeviceResponseTypeDef,
+    BlobTypeDef,
     CancelDeploymentResponseTypeDef,
     ComponentCandidateTypeDef,
-    ComponentDeploymentSpecificationOutputTypeDef,
-    ComponentDeploymentSpecificationTypeDef,
-    ComponentPlatformOutputTypeDef,
-    ComponentPlatformTypeDef,
+    ComponentDeploymentSpecificationUnionTypeDef,
+    ComponentPlatformUnionTypeDef,
     ConnectivityInfoTypeDef,
     CreateComponentVersionResponseTypeDef,
     CreateDeploymentResponseTypeDef,
-    DeploymentIoTJobConfigurationOutputTypeDef,
-    DeploymentIoTJobConfigurationTypeDef,
+    DeploymentIoTJobConfigurationUnionTypeDef,
     DeploymentPoliciesTypeDef,
     DescribeComponentResponseTypeDef,
     DisassociateClientDeviceFromCoreDeviceEntryTypeDef,
     DisassociateServiceRoleFromAccountResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetComponentResponseTypeDef,
     GetComponentVersionArtifactResponseTypeDef,
@@ -181,15 +178,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/client/#close)
         """
 
     def create_component_version(
         self,
         *,
-        inlineRecipe: Union[str, bytes, IO[Any], StreamingBody] = ...,
+        inlineRecipe: BlobTypeDef = ...,
         lambdaFunction: LambdaFunctionRecipeSourceTypeDef = ...,
         tags: Mapping[str, str] = ...,
         clientToken: str = ...
     ) -> CreateComponentVersionResponseTypeDef:
         """
         Creates a component.
 
@@ -198,24 +195,16 @@
         """
 
     def create_deployment(
         self,
         *,
         targetArn: str,
         deploymentName: str = ...,
-        components: Mapping[
-            str,
-            Union[
-                ComponentDeploymentSpecificationTypeDef,
-                ComponentDeploymentSpecificationOutputTypeDef,
-            ],
-        ] = ...,
-        iotJobConfiguration: Union[
-            DeploymentIoTJobConfigurationTypeDef, DeploymentIoTJobConfigurationOutputTypeDef
-        ] = ...,
+        components: Mapping[str, ComponentDeploymentSpecificationUnionTypeDef] = ...,
+        iotJobConfiguration: DeploymentIoTJobConfigurationUnionTypeDef = ...,
         deploymentPolicies: DeploymentPoliciesTypeDef = ...,
         parentTargetArn: str = ...,
         tags: Mapping[str, str] = ...,
         clientToken: str = ...
     ) -> CreateDeploymentResponseTypeDef:
         """
         Creates a continuous deployment for a target, which is a Greengrass core device
@@ -434,15 +423,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/client/#list_tags_for_resource)
         """
 
     def resolve_component_candidates(
         self,
         *,
-        platform: Union[ComponentPlatformTypeDef, ComponentPlatformOutputTypeDef] = ...,
+        platform: ComponentPlatformUnionTypeDef = ...,
         componentCandidates: Sequence[ComponentCandidateTypeDef] = ...
     ) -> ResolveComponentCandidatesResponseTypeDef:
         """
         Retrieves a list of components that meet the component, version, and platform
         requirements of a deployment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Client.resolve_component_candidates)
```

### Comparing `mypy-boto3-greengrassv2-1.28.15.post1/mypy_boto3_greengrassv2/client.pyi` & `mypy-boto3-greengrassv2-1.28.16/mypy_boto3_greengrassv2/client.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -10,18 +10,17 @@
     from mypy_boto3_greengrassv2.client import GreengrassV2Client
 
     session = Session()
     client: GreengrassV2Client = session.client("greengrassv2")
     ```
 """
 import sys
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
-from botocore.response import StreamingBody
 
 from .literals import (
     ComponentVisibilityScopeType,
     CoreDeviceStatusType,
     DeploymentHistoryFilterType,
     InstalledComponentTopologyFilterType,
     RecipeOutputFormatType,
@@ -36,25 +35,23 @@
     ListInstalledComponentsPaginator,
 )
 from .type_defs import (
     AssociateClientDeviceWithCoreDeviceEntryTypeDef,
     AssociateServiceRoleToAccountResponseTypeDef,
     BatchAssociateClientDeviceWithCoreDeviceResponseTypeDef,
     BatchDisassociateClientDeviceFromCoreDeviceResponseTypeDef,
+    BlobTypeDef,
     CancelDeploymentResponseTypeDef,
     ComponentCandidateTypeDef,
-    ComponentDeploymentSpecificationOutputTypeDef,
-    ComponentDeploymentSpecificationTypeDef,
-    ComponentPlatformOutputTypeDef,
-    ComponentPlatformTypeDef,
+    ComponentDeploymentSpecificationUnionTypeDef,
+    ComponentPlatformUnionTypeDef,
     ConnectivityInfoTypeDef,
     CreateComponentVersionResponseTypeDef,
     CreateDeploymentResponseTypeDef,
-    DeploymentIoTJobConfigurationOutputTypeDef,
-    DeploymentIoTJobConfigurationTypeDef,
+    DeploymentIoTJobConfigurationUnionTypeDef,
     DeploymentPoliciesTypeDef,
     DescribeComponentResponseTypeDef,
     DisassociateClientDeviceFromCoreDeviceEntryTypeDef,
     DisassociateServiceRoleFromAccountResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetComponentResponseTypeDef,
     GetComponentVersionArtifactResponseTypeDef,
@@ -170,15 +167,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/client/#close)
         """
     def create_component_version(
         self,
         *,
-        inlineRecipe: Union[str, bytes, IO[Any], StreamingBody] = ...,
+        inlineRecipe: BlobTypeDef = ...,
         lambdaFunction: LambdaFunctionRecipeSourceTypeDef = ...,
         tags: Mapping[str, str] = ...,
         clientToken: str = ...
     ) -> CreateComponentVersionResponseTypeDef:
         """
         Creates a component.
 
@@ -186,24 +183,16 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/client/#create_component_version)
         """
     def create_deployment(
         self,
         *,
         targetArn: str,
         deploymentName: str = ...,
-        components: Mapping[
-            str,
-            Union[
-                ComponentDeploymentSpecificationTypeDef,
-                ComponentDeploymentSpecificationOutputTypeDef,
-            ],
-        ] = ...,
-        iotJobConfiguration: Union[
-            DeploymentIoTJobConfigurationTypeDef, DeploymentIoTJobConfigurationOutputTypeDef
-        ] = ...,
+        components: Mapping[str, ComponentDeploymentSpecificationUnionTypeDef] = ...,
+        iotJobConfiguration: DeploymentIoTJobConfigurationUnionTypeDef = ...,
         deploymentPolicies: DeploymentPoliciesTypeDef = ...,
         parentTargetArn: str = ...,
         tags: Mapping[str, str] = ...,
         clientToken: str = ...
     ) -> CreateDeploymentResponseTypeDef:
         """
         Creates a continuous deployment for a target, which is a Greengrass core device
@@ -401,15 +390,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/client/#list_tags_for_resource)
         """
     def resolve_component_candidates(
         self,
         *,
-        platform: Union[ComponentPlatformTypeDef, ComponentPlatformOutputTypeDef] = ...,
+        platform: ComponentPlatformUnionTypeDef = ...,
         componentCandidates: Sequence[ComponentCandidateTypeDef] = ...
     ) -> ResolveComponentCandidatesResponseTypeDef:
         """
         Retrieves a list of components that meet the component, version, and platform
         requirements of a deployment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Client.resolve_component_candidates)
```

### Comparing `mypy-boto3-greengrassv2-1.28.15.post1/mypy_boto3_greengrassv2/literals.py` & `mypy-boto3-greengrassv2-1.28.16/mypy_boto3_greengrassv2/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-greengrassv2-1.28.15.post1/mypy_boto3_greengrassv2/literals.pyi` & `mypy-boto3-greengrassv2-1.28.16/mypy_boto3_greengrassv2/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-greengrassv2-1.28.15.post1/mypy_boto3_greengrassv2/paginator.py` & `mypy-boto3-greengrassv2-1.28.16/mypy_boto3_greengrassv2/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-greengrassv2-1.28.15.post1/mypy_boto3_greengrassv2/paginator.pyi` & `mypy-boto3-greengrassv2-1.28.16/mypy_boto3_greengrassv2/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-greengrassv2-1.28.15.post1/mypy_boto3_greengrassv2/type_defs.py` & `mypy-boto3-greengrassv2-1.28.16/mypy_boto3_greengrassv2/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_greengrassv2.type_defs import AssociateClientDeviceWithCoreDeviceEntryTypeDef
 
-    data: AssociateClientDeviceWithCoreDeviceEntryTypeDef = {...}
+    data: AssociateClientDeviceWithCoreDeviceEntryTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -52,14 +52,15 @@
     "AssociateClientDeviceWithCoreDeviceEntryTypeDef",
     "AssociateClientDeviceWithCoreDeviceErrorEntryTypeDef",
     "AssociateServiceRoleToAccountRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "AssociatedClientDeviceTypeDef",
     "DisassociateClientDeviceFromCoreDeviceEntryTypeDef",
     "DisassociateClientDeviceFromCoreDeviceErrorEntryTypeDef",
+    "BlobTypeDef",
     "CancelDeploymentRequestRequestTypeDef",
     "CloudComponentStatusTypeDef",
     "ComponentCandidateTypeDef",
     "ComponentConfigurationUpdateOutputTypeDef",
     "ComponentConfigurationUpdateTypeDef",
     "ComponentDependencyRequirementTypeDef",
     "ComponentPlatformOutputTypeDef",
@@ -115,14 +116,15 @@
     "UpdateConnectivityInfoResponseTypeDef",
     "ListClientDevicesAssociatedWithCoreDeviceResponseTypeDef",
     "BatchDisassociateClientDeviceFromCoreDeviceRequestRequestTypeDef",
     "BatchDisassociateClientDeviceFromCoreDeviceResponseTypeDef",
     "CreateComponentVersionResponseTypeDef",
     "ComponentLatestVersionTypeDef",
     "DescribeComponentResponseTypeDef",
+    "ComponentPlatformUnionTypeDef",
     "ResolveComponentCandidatesRequestRequestTypeDef",
     "ComponentRunWithTypeDef",
     "ListComponentVersionsResponseTypeDef",
     "GetConnectivityInfoResponseTypeDef",
     "UpdateConnectivityInfoRequestRequestTypeDef",
     "ListCoreDevicesResponseTypeDef",
     "DeploymentPoliciesTypeDef",
@@ -144,19 +146,21 @@
     "ComponentTypeDef",
     "ComponentDeploymentSpecificationOutputTypeDef",
     "ComponentDeploymentSpecificationTypeDef",
     "ListEffectiveDeploymentsResponseTypeDef",
     "IoTJobExecutionsRolloutConfigTypeDef",
     "LambdaLinuxProcessParamsTypeDef",
     "ListComponentsResponseTypeDef",
+    "ComponentDeploymentSpecificationUnionTypeDef",
     "DeploymentIoTJobConfigurationOutputTypeDef",
     "DeploymentIoTJobConfigurationTypeDef",
     "LambdaExecutionParametersTypeDef",
     "GetDeploymentResponseTypeDef",
     "CreateDeploymentRequestRequestTypeDef",
+    "DeploymentIoTJobConfigurationUnionTypeDef",
     "LambdaFunctionRecipeSourceTypeDef",
     "CreateComponentVersionRequestRequestTypeDef",
 )
 
 AssociateClientDeviceWithCoreDeviceEntryTypeDef = TypedDict(
     "AssociateClientDeviceWithCoreDeviceEntryTypeDef",
     {
@@ -214,14 +218,15 @@
         "thingName": str,
         "code": str,
         "message": str,
     },
     total=False,
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 CancelDeploymentRequestRequestTypeDef = TypedDict(
     "CancelDeploymentRequestRequestTypeDef",
     {
         "deploymentId": str,
     },
 )
 
@@ -924,14 +929,15 @@
         "status": CloudComponentStatusTypeDef,
         "platforms": List[ComponentPlatformOutputTypeDef],
         "tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ComponentPlatformUnionTypeDef = Union[ComponentPlatformTypeDef, ComponentPlatformOutputTypeDef]
 ResolveComponentCandidatesRequestRequestTypeDef = TypedDict(
     "ResolveComponentCandidatesRequestRequestTypeDef",
     {
         "platform": ComponentPlatformTypeDef,
         "componentCandidates": Sequence[ComponentCandidateTypeDef],
     },
     total=False,
@@ -1263,14 +1269,17 @@
     {
         "components": List[ComponentTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ComponentDeploymentSpecificationUnionTypeDef = Union[
+    ComponentDeploymentSpecificationTypeDef, ComponentDeploymentSpecificationOutputTypeDef
+]
 DeploymentIoTJobConfigurationOutputTypeDef = TypedDict(
     "DeploymentIoTJobConfigurationOutputTypeDef",
     {
         "jobExecutionsRolloutConfig": IoTJobExecutionsRolloutConfigTypeDef,
         "abortConfig": IoTJobAbortConfigOutputTypeDef,
         "timeoutConfig": IoTJobTimeoutConfigTypeDef,
     },
@@ -1332,21 +1341,15 @@
         "targetArn": str,
     },
 )
 _OptionalCreateDeploymentRequestRequestTypeDef = TypedDict(
     "_OptionalCreateDeploymentRequestRequestTypeDef",
     {
         "deploymentName": str,
-        "components": Mapping[
-            str,
-            Union[
-                ComponentDeploymentSpecificationTypeDef,
-                ComponentDeploymentSpecificationOutputTypeDef,
-            ],
-        ],
+        "components": Mapping[str, ComponentDeploymentSpecificationUnionTypeDef],
         "iotJobConfiguration": DeploymentIoTJobConfigurationTypeDef,
         "deploymentPolicies": DeploymentPoliciesTypeDef,
         "parentTargetArn": str,
         "tags": Mapping[str, str],
         "clientToken": str,
     },
     total=False,
@@ -1355,14 +1358,17 @@
 
 class CreateDeploymentRequestRequestTypeDef(
     _RequiredCreateDeploymentRequestRequestTypeDef, _OptionalCreateDeploymentRequestRequestTypeDef
 ):
     pass
 
 
+DeploymentIoTJobConfigurationUnionTypeDef = Union[
+    DeploymentIoTJobConfigurationTypeDef, DeploymentIoTJobConfigurationOutputTypeDef
+]
 _RequiredLambdaFunctionRecipeSourceTypeDef = TypedDict(
     "_RequiredLambdaFunctionRecipeSourceTypeDef",
     {
         "lambdaArn": str,
     },
 )
 _OptionalLambdaFunctionRecipeSourceTypeDef = TypedDict(
@@ -1383,14 +1389,14 @@
 ):
     pass
 
 
 CreateComponentVersionRequestRequestTypeDef = TypedDict(
     "CreateComponentVersionRequestRequestTypeDef",
     {
-        "inlineRecipe": Union[str, bytes, IO[Any], StreamingBody],
+        "inlineRecipe": BlobTypeDef,
         "lambdaFunction": LambdaFunctionRecipeSourceTypeDef,
         "tags": Mapping[str, str],
         "clientToken": str,
     },
     total=False,
 )
```

### Comparing `mypy-boto3-greengrassv2-1.28.15.post1/mypy_boto3_greengrassv2/type_defs.pyi` & `mypy-boto3-greengrassv2-1.28.16/mypy_boto3_greengrassv2/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_greengrassv2.type_defs import AssociateClientDeviceWithCoreDeviceEntryTypeDef
 
-    data: AssociateClientDeviceWithCoreDeviceEntryTypeDef = {...}
+    data: AssociateClientDeviceWithCoreDeviceEntryTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -51,14 +51,15 @@
     "AssociateClientDeviceWithCoreDeviceEntryTypeDef",
     "AssociateClientDeviceWithCoreDeviceErrorEntryTypeDef",
     "AssociateServiceRoleToAccountRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "AssociatedClientDeviceTypeDef",
     "DisassociateClientDeviceFromCoreDeviceEntryTypeDef",
     "DisassociateClientDeviceFromCoreDeviceErrorEntryTypeDef",
+    "BlobTypeDef",
     "CancelDeploymentRequestRequestTypeDef",
     "CloudComponentStatusTypeDef",
     "ComponentCandidateTypeDef",
     "ComponentConfigurationUpdateOutputTypeDef",
     "ComponentConfigurationUpdateTypeDef",
     "ComponentDependencyRequirementTypeDef",
     "ComponentPlatformOutputTypeDef",
@@ -114,14 +115,15 @@
     "UpdateConnectivityInfoResponseTypeDef",
     "ListClientDevicesAssociatedWithCoreDeviceResponseTypeDef",
     "BatchDisassociateClientDeviceFromCoreDeviceRequestRequestTypeDef",
     "BatchDisassociateClientDeviceFromCoreDeviceResponseTypeDef",
     "CreateComponentVersionResponseTypeDef",
     "ComponentLatestVersionTypeDef",
     "DescribeComponentResponseTypeDef",
+    "ComponentPlatformUnionTypeDef",
     "ResolveComponentCandidatesRequestRequestTypeDef",
     "ComponentRunWithTypeDef",
     "ListComponentVersionsResponseTypeDef",
     "GetConnectivityInfoResponseTypeDef",
     "UpdateConnectivityInfoRequestRequestTypeDef",
     "ListCoreDevicesResponseTypeDef",
     "DeploymentPoliciesTypeDef",
@@ -143,19 +145,21 @@
     "ComponentTypeDef",
     "ComponentDeploymentSpecificationOutputTypeDef",
     "ComponentDeploymentSpecificationTypeDef",
     "ListEffectiveDeploymentsResponseTypeDef",
     "IoTJobExecutionsRolloutConfigTypeDef",
     "LambdaLinuxProcessParamsTypeDef",
     "ListComponentsResponseTypeDef",
+    "ComponentDeploymentSpecificationUnionTypeDef",
     "DeploymentIoTJobConfigurationOutputTypeDef",
     "DeploymentIoTJobConfigurationTypeDef",
     "LambdaExecutionParametersTypeDef",
     "GetDeploymentResponseTypeDef",
     "CreateDeploymentRequestRequestTypeDef",
+    "DeploymentIoTJobConfigurationUnionTypeDef",
     "LambdaFunctionRecipeSourceTypeDef",
     "CreateComponentVersionRequestRequestTypeDef",
 )
 
 AssociateClientDeviceWithCoreDeviceEntryTypeDef = TypedDict(
     "AssociateClientDeviceWithCoreDeviceEntryTypeDef",
     {
@@ -213,14 +217,15 @@
         "thingName": str,
         "code": str,
         "message": str,
     },
     total=False,
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 CancelDeploymentRequestRequestTypeDef = TypedDict(
     "CancelDeploymentRequestRequestTypeDef",
     {
         "deploymentId": str,
     },
 )
 
@@ -905,14 +910,15 @@
         "status": CloudComponentStatusTypeDef,
         "platforms": List[ComponentPlatformOutputTypeDef],
         "tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ComponentPlatformUnionTypeDef = Union[ComponentPlatformTypeDef, ComponentPlatformOutputTypeDef]
 ResolveComponentCandidatesRequestRequestTypeDef = TypedDict(
     "ResolveComponentCandidatesRequestRequestTypeDef",
     {
         "platform": ComponentPlatformTypeDef,
         "componentCandidates": Sequence[ComponentCandidateTypeDef],
     },
     total=False,
@@ -1234,14 +1240,17 @@
     {
         "components": List[ComponentTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ComponentDeploymentSpecificationUnionTypeDef = Union[
+    ComponentDeploymentSpecificationTypeDef, ComponentDeploymentSpecificationOutputTypeDef
+]
 DeploymentIoTJobConfigurationOutputTypeDef = TypedDict(
     "DeploymentIoTJobConfigurationOutputTypeDef",
     {
         "jobExecutionsRolloutConfig": IoTJobExecutionsRolloutConfigTypeDef,
         "abortConfig": IoTJobAbortConfigOutputTypeDef,
         "timeoutConfig": IoTJobTimeoutConfigTypeDef,
     },
@@ -1303,35 +1312,32 @@
         "targetArn": str,
     },
 )
 _OptionalCreateDeploymentRequestRequestTypeDef = TypedDict(
     "_OptionalCreateDeploymentRequestRequestTypeDef",
     {
         "deploymentName": str,
-        "components": Mapping[
-            str,
-            Union[
-                ComponentDeploymentSpecificationTypeDef,
-                ComponentDeploymentSpecificationOutputTypeDef,
-            ],
-        ],
+        "components": Mapping[str, ComponentDeploymentSpecificationUnionTypeDef],
         "iotJobConfiguration": DeploymentIoTJobConfigurationTypeDef,
         "deploymentPolicies": DeploymentPoliciesTypeDef,
         "parentTargetArn": str,
         "tags": Mapping[str, str],
         "clientToken": str,
     },
     total=False,
 )
 
 class CreateDeploymentRequestRequestTypeDef(
     _RequiredCreateDeploymentRequestRequestTypeDef, _OptionalCreateDeploymentRequestRequestTypeDef
 ):
     pass
 
+DeploymentIoTJobConfigurationUnionTypeDef = Union[
+    DeploymentIoTJobConfigurationTypeDef, DeploymentIoTJobConfigurationOutputTypeDef
+]
 _RequiredLambdaFunctionRecipeSourceTypeDef = TypedDict(
     "_RequiredLambdaFunctionRecipeSourceTypeDef",
     {
         "lambdaArn": str,
     },
 )
 _OptionalLambdaFunctionRecipeSourceTypeDef = TypedDict(
@@ -1350,14 +1356,14 @@
     _RequiredLambdaFunctionRecipeSourceTypeDef, _OptionalLambdaFunctionRecipeSourceTypeDef
 ):
     pass
 
 CreateComponentVersionRequestRequestTypeDef = TypedDict(
     "CreateComponentVersionRequestRequestTypeDef",
     {
-        "inlineRecipe": Union[str, bytes, IO[Any], StreamingBody],
+        "inlineRecipe": BlobTypeDef,
         "lambdaFunction": LambdaFunctionRecipeSourceTypeDef,
         "tags": Mapping[str, str],
         "clientToken": str,
     },
     total=False,
 )
```

### Comparing `mypy-boto3-greengrassv2-1.28.15.post1/mypy_boto3_greengrassv2.egg-info/PKG-INFO` & `mypy-boto3-greengrassv2-1.28.16/mypy_boto3_greengrassv2.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-greengrassv2
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.GreengrassV2 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.GreengrassV2 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 greengrassv2 type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 greengrassv2 type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-greengrassv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-greengrassv2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-greengrassv2)](https://pepy.tech/project/mypy-boto3-greengrassv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.GreengrassV2 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2)
+[boto3.GreengrassV2 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2)
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
 [mypy-boto3-greengrassv2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/).
 
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
@@ -357,30 +357,31 @@
 )
 
 
 def check_value(value: CloudComponentStateType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_greengrassv2.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_greengrassv2.type_defs import (
     AssociateClientDeviceWithCoreDeviceEntryTypeDef,
     AssociateClientDeviceWithCoreDeviceErrorEntryTypeDef,
     AssociateServiceRoleToAccountRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     AssociatedClientDeviceTypeDef,
     DisassociateClientDeviceFromCoreDeviceEntryTypeDef,
     DisassociateClientDeviceFromCoreDeviceErrorEntryTypeDef,
+    BlobTypeDef,
     CancelDeploymentRequestRequestTypeDef,
     CloudComponentStatusTypeDef,
     ComponentCandidateTypeDef,
     ComponentConfigurationUpdateOutputTypeDef,
     ComponentConfigurationUpdateTypeDef,
     ComponentDependencyRequirementTypeDef,
     ComponentPlatformOutputTypeDef,
@@ -436,14 +437,15 @@
     UpdateConnectivityInfoResponseTypeDef,
     ListClientDevicesAssociatedWithCoreDeviceResponseTypeDef,
     BatchDisassociateClientDeviceFromCoreDeviceRequestRequestTypeDef,
     BatchDisassociateClientDeviceFromCoreDeviceResponseTypeDef,
     CreateComponentVersionResponseTypeDef,
     ComponentLatestVersionTypeDef,
     DescribeComponentResponseTypeDef,
+    ComponentPlatformUnionTypeDef,
     ResolveComponentCandidatesRequestRequestTypeDef,
     ComponentRunWithTypeDef,
     ListComponentVersionsResponseTypeDef,
     GetConnectivityInfoResponseTypeDef,
     UpdateConnectivityInfoRequestRequestTypeDef,
     ListCoreDevicesResponseTypeDef,
     DeploymentPoliciesTypeDef,
@@ -465,25 +467,27 @@
     ComponentTypeDef,
     ComponentDeploymentSpecificationOutputTypeDef,
     ComponentDeploymentSpecificationTypeDef,
     ListEffectiveDeploymentsResponseTypeDef,
     IoTJobExecutionsRolloutConfigTypeDef,
     LambdaLinuxProcessParamsTypeDef,
     ListComponentsResponseTypeDef,
+    ComponentDeploymentSpecificationUnionTypeDef,
     DeploymentIoTJobConfigurationOutputTypeDef,
     DeploymentIoTJobConfigurationTypeDef,
     LambdaExecutionParametersTypeDef,
     GetDeploymentResponseTypeDef,
     CreateDeploymentRequestRequestTypeDef,
+    DeploymentIoTJobConfigurationUnionTypeDef,
     LambdaFunctionRecipeSourceTypeDef,
     CreateComponentVersionRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AssociateClientDeviceWithCoreDeviceEntryTypeDef:
+def get_value() -> AssociateClientDeviceWithCoreDeviceEntryTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-greengrassv2-1.28.15.post1/mypy_boto3_greengrassv2.egg-info/SOURCES.txt` & `mypy-boto3-greengrassv2-1.28.16/mypy_boto3_greengrassv2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-greengrassv2-1.28.15.post1/setup.py` & `mypy-boto3-greengrassv2-1.28.16/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-greengrassv2",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_greengrassv2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.GreengrassV2 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.2"
+        "Type annotations for boto3.GreengrassV2 1.28.16 service generated with mypy-boto3-builder"
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
-    keywords="boto3 greengrassv2 type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 greengrassv2 type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_greengrassv2": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_greengrassv2/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

