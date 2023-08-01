# Comparing `tmp/mypy-boto3-appconfig-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-appconfig-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-appconfig-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:27 2023, max compression
+gzip compressed data, was "mypy-boto3-appconfig-1.28.16.tar", last modified: Tue Aug  1 11:36:08 2023, max compression
```

## Comparing `mypy-boto3-appconfig-1.28.15.post1.tar` & `mypy-boto3-appconfig-1.28.16.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:27.760993 mypy-boto3-appconfig-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:38:03.000000 mypy-boto3-appconfig-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15133 2023-07-29 10:02:27.756993 mypy-boto3-appconfig-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13632 2023-07-29 09:38:03.000000 mypy-boto3-appconfig-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:27.744993 mypy-boto3-appconfig-1.28.15.post1/mypy_boto3_appconfig/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-29 09:38:03.000000 mypy-boto3-appconfig-1.28.15.post1/mypy_boto3_appconfig/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-29 09:38:03.000000 mypy-boto3-appconfig-1.28.15.post1/mypy_boto3_appconfig/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-29 09:38:03.000000 mypy-boto3-appconfig-1.28.15.post1/mypy_boto3_appconfig/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28973 2023-07-29 09:38:03.000000 mypy-boto3-appconfig-1.28.15.post1/mypy_boto3_appconfig/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    28924 2023-07-29 09:38:03.000000 mypy-boto3-appconfig-1.28.15.post1/mypy_boto3_appconfig/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9264 2023-07-29 09:38:03.000000 mypy-boto3-appconfig-1.28.15.post1/mypy_boto3_appconfig/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9262 2023-07-29 09:38:03.000000 mypy-boto3-appconfig-1.28.15.post1/mypy_boto3_appconfig/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:38:03.000000 mypy-boto3-appconfig-1.28.15.post1/mypy_boto3_appconfig/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    31086 2023-07-29 09:38:04.000000 mypy-boto3-appconfig-1.28.15.post1/mypy_boto3_appconfig/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    31041 2023-07-29 09:38:04.000000 mypy-boto3-appconfig-1.28.15.post1/mypy_boto3_appconfig/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:38:03.000000 mypy-boto3-appconfig-1.28.15.post1/mypy_boto3_appconfig/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:27.756993 mypy-boto3-appconfig-1.28.15.post1/mypy_boto3_appconfig.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15133 2023-07-29 10:02:27.000000 mypy-boto3-appconfig-1.28.15.post1/mypy_boto3_appconfig.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-29 10:02:27.000000 mypy-boto3-appconfig-1.28.15.post1/mypy_boto3_appconfig.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:27.000000 mypy-boto3-appconfig-1.28.15.post1/mypy_boto3_appconfig.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:27.000000 mypy-boto3-appconfig-1.28.15.post1/mypy_boto3_appconfig.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:27.000000 mypy-boto3-appconfig-1.28.15.post1/mypy_boto3_appconfig.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-29 10:02:27.000000 mypy-boto3-appconfig-1.28.15.post1/mypy_boto3_appconfig.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:27.760993 mypy-boto3-appconfig-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-07-29 09:38:03.000000 mypy-boto3-appconfig-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:08.480956 mypy-boto3-appconfig-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:10:33.000000 mypy-boto3-appconfig-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15140 2023-08-01 11:36:08.472956 mypy-boto3-appconfig-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13648 2023-08-01 11:10:33.000000 mypy-boto3-appconfig-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:08.472956 mypy-boto3-appconfig-1.28.16/mypy_boto3_appconfig/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-08-01 11:10:33.000000 mypy-boto3-appconfig-1.28.16/mypy_boto3_appconfig/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-08-01 11:10:33.000000 mypy-boto3-appconfig-1.28.16/mypy_boto3_appconfig/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-08-01 11:10:33.000000 mypy-boto3-appconfig-1.28.16/mypy_boto3_appconfig/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28905 2023-08-01 11:10:33.000000 mypy-boto3-appconfig-1.28.16/mypy_boto3_appconfig/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28856 2023-08-01 11:10:33.000000 mypy-boto3-appconfig-1.28.16/mypy_boto3_appconfig/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9264 2023-08-01 11:10:34.000000 mypy-boto3-appconfig-1.28.16/mypy_boto3_appconfig/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9262 2023-08-01 11:10:33.000000 mypy-boto3-appconfig-1.28.16/mypy_boto3_appconfig/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:10:33.000000 mypy-boto3-appconfig-1.28.16/mypy_boto3_appconfig/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    31129 2023-08-01 11:10:34.000000 mypy-boto3-appconfig-1.28.16/mypy_boto3_appconfig/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31084 2023-08-01 11:10:34.000000 mypy-boto3-appconfig-1.28.16/mypy_boto3_appconfig/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:10:33.000000 mypy-boto3-appconfig-1.28.16/mypy_boto3_appconfig/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:08.472956 mypy-boto3-appconfig-1.28.16/mypy_boto3_appconfig.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15140 2023-08-01 11:36:08.000000 mypy-boto3-appconfig-1.28.16/mypy_boto3_appconfig.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-08-01 11:36:08.000000 mypy-boto3-appconfig-1.28.16/mypy_boto3_appconfig.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:08.000000 mypy-boto3-appconfig-1.28.16/mypy_boto3_appconfig.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:08.000000 mypy-boto3-appconfig-1.28.16/mypy_boto3_appconfig.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:08.000000 mypy-boto3-appconfig-1.28.16/mypy_boto3_appconfig.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-01 11:36:08.000000 mypy-boto3-appconfig-1.28.16/mypy_boto3_appconfig.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:08.480956 mypy-boto3-appconfig-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-08-01 11:10:33.000000 mypy-boto3-appconfig-1.28.16/setup.py
```

### Comparing `mypy-boto3-appconfig-1.28.15.post1/LICENSE` & `mypy-boto3-appconfig-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appconfig-1.28.15.post1/PKG-INFO` & `mypy-boto3-appconfig-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-appconfig
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.AppConfig 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.AppConfig 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appconfig/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 appconfig type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 appconfig type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-appconfig.svg?color=blue)](https://pypi.org/project/mypy-boto3-appconfig)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appconfig/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-appconfig)](https://pepy.tech/project/mypy-boto3-appconfig)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AppConfig 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig)
+[boto3.AppConfig 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig)
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
 [mypy-boto3-appconfig docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appconfig/).
 
 See how it helps to find and fix potential bugs:
 
@@ -73,15 +73,15 @@
     - [Sublime Text](#sublime-text)
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
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
@@ -294,36 +294,36 @@
 )
 
 
 def check_value(value: ActionPointType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_appconfig.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_appconfig.type_defs import (
     ActionInvocationTypeDef,
     ActionTypeDef,
     ResponseMetadataTypeDef,
     ApplicationTypeDef,
     AppliedExtensionTypeDef,
+    BlobTypeDef,
     ConfigurationProfileSummaryTypeDef,
     ValidatorTypeDef,
     CreateApplicationRequestRequestTypeDef,
     CreateDeploymentStrategyRequestRequestTypeDef,
     MonitorTypeDef,
     CreateExtensionAssociationRequestRequestTypeDef,
     ParameterTypeDef,
-    CreateHostedConfigurationVersionRequestRequestTypeDef,
     DeleteApplicationRequestRequestTypeDef,
     DeleteConfigurationProfileRequestRequestTypeDef,
     DeleteDeploymentStrategyRequestRequestTypeDef,
     DeleteEnvironmentRequestRequestTypeDef,
     DeleteExtensionAssociationRequestRequestTypeDef,
     DeleteExtensionRequestRequestTypeDef,
     DeleteHostedConfigurationVersionRequestRequestTypeDef,
@@ -363,14 +363,15 @@
     ConfigurationTypeDef,
     DeploymentStrategyResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     ExtensionAssociationTypeDef,
     HostedConfigurationVersionTypeDef,
     ResourceTagsTypeDef,
     ApplicationsTypeDef,
+    CreateHostedConfigurationVersionRequestRequestTypeDef,
     ConfigurationProfilesTypeDef,
     ConfigurationProfileTypeDef,
     CreateConfigurationProfileRequestRequestTypeDef,
     UpdateConfigurationProfileRequestRequestTypeDef,
     CreateEnvironmentRequestRequestTypeDef,
     EnvironmentResponseTypeDef,
     EnvironmentTypeDef,
@@ -384,15 +385,15 @@
     ExtensionsTypeDef,
     HostedConfigurationVersionsTypeDef,
     DeploymentTypeDef,
     EnvironmentsTypeDef,
 )
 
 
-def get_structure() -> ActionInvocationTypeDef:
+def get_value() -> ActionInvocationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-appconfig-1.28.15.post1/README.md` & `mypy-boto3-appconfig-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-appconfig.svg?color=blue)](https://pypi.org/project/mypy-boto3-appconfig)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appconfig/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-appconfig)](https://pepy.tech/project/mypy-boto3-appconfig)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AppConfig 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig)
+[boto3.AppConfig 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig)
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
 [mypy-boto3-appconfig docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appconfig/).
 
 See how it helps to find and fix potential bugs:
 
@@ -41,15 +41,15 @@
     - [Sublime Text](#sublime-text)
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
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
@@ -262,36 +262,36 @@
 )
 
 
 def check_value(value: ActionPointType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_appconfig.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_appconfig.type_defs import (
     ActionInvocationTypeDef,
     ActionTypeDef,
     ResponseMetadataTypeDef,
     ApplicationTypeDef,
     AppliedExtensionTypeDef,
+    BlobTypeDef,
     ConfigurationProfileSummaryTypeDef,
     ValidatorTypeDef,
     CreateApplicationRequestRequestTypeDef,
     CreateDeploymentStrategyRequestRequestTypeDef,
     MonitorTypeDef,
     CreateExtensionAssociationRequestRequestTypeDef,
     ParameterTypeDef,
-    CreateHostedConfigurationVersionRequestRequestTypeDef,
     DeleteApplicationRequestRequestTypeDef,
     DeleteConfigurationProfileRequestRequestTypeDef,
     DeleteDeploymentStrategyRequestRequestTypeDef,
     DeleteEnvironmentRequestRequestTypeDef,
     DeleteExtensionAssociationRequestRequestTypeDef,
     DeleteExtensionRequestRequestTypeDef,
     DeleteHostedConfigurationVersionRequestRequestTypeDef,
@@ -331,14 +331,15 @@
     ConfigurationTypeDef,
     DeploymentStrategyResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     ExtensionAssociationTypeDef,
     HostedConfigurationVersionTypeDef,
     ResourceTagsTypeDef,
     ApplicationsTypeDef,
+    CreateHostedConfigurationVersionRequestRequestTypeDef,
     ConfigurationProfilesTypeDef,
     ConfigurationProfileTypeDef,
     CreateConfigurationProfileRequestRequestTypeDef,
     UpdateConfigurationProfileRequestRequestTypeDef,
     CreateEnvironmentRequestRequestTypeDef,
     EnvironmentResponseTypeDef,
     EnvironmentTypeDef,
@@ -352,15 +353,15 @@
     ExtensionsTypeDef,
     HostedConfigurationVersionsTypeDef,
     DeploymentTypeDef,
     EnvironmentsTypeDef,
 )
 
 
-def get_structure() -> ActionInvocationTypeDef:
+def get_value() -> ActionInvocationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-appconfig-1.28.15.post1/mypy_boto3_appconfig/__main__.py` & `mypy-boto3-appconfig-1.28.16/mypy_boto3_appconfig/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.AppConfig 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.AppConfig 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appconfig//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig\nOther"
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

### Comparing `mypy-boto3-appconfig-1.28.15.post1/mypy_boto3_appconfig/client.py` & `mypy-boto3-appconfig-1.28.16/mypy_boto3_appconfig/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,24 +9,24 @@
     from boto3.session import Session
     from mypy_boto3_appconfig.client import AppConfigClient
 
     session = Session()
     client: AppConfigClient = session.client("appconfig")
     ```
 """
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
-from botocore.response import StreamingBody
 
 from .literals import ActionPointType, GrowthTypeType, ReplicateToType
 from .type_defs import (
     ActionTypeDef,
     ApplicationResponseTypeDef,
     ApplicationsTypeDef,
+    BlobTypeDef,
     ConfigurationProfilesTypeDef,
     ConfigurationProfileTypeDef,
     ConfigurationTypeDef,
     DeploymentStrategiesTypeDef,
     DeploymentStrategyResponseTypeDef,
     DeploymentsTypeDef,
     DeploymentTypeDef,
@@ -201,15 +201,15 @@
         """
 
     def create_hosted_configuration_version(
         self,
         *,
         ApplicationId: str,
         ConfigurationProfileId: str,
-        Content: Union[str, bytes, IO[Any], StreamingBody],
+        Content: BlobTypeDef,
         ContentType: str,
         Description: str = ...,
         LatestVersionNumber: int = ...,
         VersionLabel: str = ...
     ) -> HostedConfigurationVersionTypeDef:
         """
         Creates a new configuration in the AppConfig hosted configuration store.
```

### Comparing `mypy-boto3-appconfig-1.28.15.post1/mypy_boto3_appconfig/client.pyi` & `mypy-boto3-appconfig-1.28.16/mypy_boto3_appconfig/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -9,24 +9,24 @@
     from boto3.session import Session
     from mypy_boto3_appconfig.client import AppConfigClient
 
     session = Session()
     client: AppConfigClient = session.client("appconfig")
     ```
 """
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
-from botocore.response import StreamingBody
 
 from .literals import ActionPointType, GrowthTypeType, ReplicateToType
 from .type_defs import (
     ActionTypeDef,
     ApplicationResponseTypeDef,
     ApplicationsTypeDef,
+    BlobTypeDef,
     ConfigurationProfilesTypeDef,
     ConfigurationProfileTypeDef,
     ConfigurationTypeDef,
     DeploymentStrategiesTypeDef,
     DeploymentStrategyResponseTypeDef,
     DeploymentsTypeDef,
     DeploymentTypeDef,
@@ -189,15 +189,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appconfig/client/#create_extension_association)
         """
     def create_hosted_configuration_version(
         self,
         *,
         ApplicationId: str,
         ConfigurationProfileId: str,
-        Content: Union[str, bytes, IO[Any], StreamingBody],
+        Content: BlobTypeDef,
         ContentType: str,
         Description: str = ...,
         LatestVersionNumber: int = ...,
         VersionLabel: str = ...
     ) -> HostedConfigurationVersionTypeDef:
         """
         Creates a new configuration in the AppConfig hosted configuration store.
```

### Comparing `mypy-boto3-appconfig-1.28.15.post1/mypy_boto3_appconfig/literals.py` & `mypy-boto3-appconfig-1.28.16/mypy_boto3_appconfig/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appconfig-1.28.15.post1/mypy_boto3_appconfig/literals.pyi` & `mypy-boto3-appconfig-1.28.16/mypy_boto3_appconfig/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appconfig-1.28.15.post1/mypy_boto3_appconfig/type_defs.py` & `mypy-boto3-appconfig-1.28.16/mypy_boto3_appconfig/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appconfig/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_appconfig.type_defs import ActionInvocationTypeDef
 
-    data: ActionInvocationTypeDef = {...}
+    data: ActionInvocationTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -36,22 +36,22 @@
 
 __all__ = (
     "ActionInvocationTypeDef",
     "ActionTypeDef",
     "ResponseMetadataTypeDef",
     "ApplicationTypeDef",
     "AppliedExtensionTypeDef",
+    "BlobTypeDef",
     "ConfigurationProfileSummaryTypeDef",
     "ValidatorTypeDef",
     "CreateApplicationRequestRequestTypeDef",
     "CreateDeploymentStrategyRequestRequestTypeDef",
     "MonitorTypeDef",
     "CreateExtensionAssociationRequestRequestTypeDef",
     "ParameterTypeDef",
-    "CreateHostedConfigurationVersionRequestRequestTypeDef",
     "DeleteApplicationRequestRequestTypeDef",
     "DeleteConfigurationProfileRequestRequestTypeDef",
     "DeleteDeploymentStrategyRequestRequestTypeDef",
     "DeleteEnvironmentRequestRequestTypeDef",
     "DeleteExtensionAssociationRequestRequestTypeDef",
     "DeleteExtensionRequestRequestTypeDef",
     "DeleteHostedConfigurationVersionRequestRequestTypeDef",
@@ -91,14 +91,15 @@
     "ConfigurationTypeDef",
     "DeploymentStrategyResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "ExtensionAssociationTypeDef",
     "HostedConfigurationVersionTypeDef",
     "ResourceTagsTypeDef",
     "ApplicationsTypeDef",
+    "CreateHostedConfigurationVersionRequestRequestTypeDef",
     "ConfigurationProfilesTypeDef",
     "ConfigurationProfileTypeDef",
     "CreateConfigurationProfileRequestRequestTypeDef",
     "UpdateConfigurationProfileRequestRequestTypeDef",
     "CreateEnvironmentRequestRequestTypeDef",
     "EnvironmentResponseTypeDef",
     "EnvironmentTypeDef",
@@ -168,14 +169,15 @@
         "ExtensionAssociationId": str,
         "VersionNumber": int,
         "Parameters": Dict[str, str],
     },
     total=False,
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 ConfigurationProfileSummaryTypeDef = TypedDict(
     "ConfigurationProfileSummaryTypeDef",
     {
         "ApplicationId": str,
         "Id": str,
         "Name": str,
         "LocationUri": str,
@@ -292,41 +294,14 @@
     {
         "Description": str,
         "Required": bool,
     },
     total=False,
 )
 
-_RequiredCreateHostedConfigurationVersionRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateHostedConfigurationVersionRequestRequestTypeDef",
-    {
-        "ApplicationId": str,
-        "ConfigurationProfileId": str,
-        "Content": Union[str, bytes, IO[Any], StreamingBody],
-        "ContentType": str,
-    },
-)
-_OptionalCreateHostedConfigurationVersionRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateHostedConfigurationVersionRequestRequestTypeDef",
-    {
-        "Description": str,
-        "LatestVersionNumber": int,
-        "VersionLabel": str,
-    },
-    total=False,
-)
-
-
-class CreateHostedConfigurationVersionRequestRequestTypeDef(
-    _RequiredCreateHostedConfigurationVersionRequestRequestTypeDef,
-    _OptionalCreateHostedConfigurationVersionRequestRequestTypeDef,
-):
-    pass
-
-
 DeleteApplicationRequestRequestTypeDef = TypedDict(
     "DeleteApplicationRequestRequestTypeDef",
     {
         "ApplicationId": str,
     },
 )
 
@@ -924,14 +899,41 @@
     {
         "Items": List[ApplicationTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredCreateHostedConfigurationVersionRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateHostedConfigurationVersionRequestRequestTypeDef",
+    {
+        "ApplicationId": str,
+        "ConfigurationProfileId": str,
+        "Content": BlobTypeDef,
+        "ContentType": str,
+    },
+)
+_OptionalCreateHostedConfigurationVersionRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateHostedConfigurationVersionRequestRequestTypeDef",
+    {
+        "Description": str,
+        "LatestVersionNumber": int,
+        "VersionLabel": str,
+    },
+    total=False,
+)
+
+
+class CreateHostedConfigurationVersionRequestRequestTypeDef(
+    _RequiredCreateHostedConfigurationVersionRequestRequestTypeDef,
+    _OptionalCreateHostedConfigurationVersionRequestRequestTypeDef,
+):
+    pass
+
+
 ConfigurationProfilesTypeDef = TypedDict(
     "ConfigurationProfilesTypeDef",
     {
         "Items": List[ConfigurationProfileSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-appconfig-1.28.15.post1/mypy_boto3_appconfig/type_defs.pyi` & `mypy-boto3-appconfig-1.28.16/mypy_boto3_appconfig/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appconfig/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_appconfig.type_defs import ActionInvocationTypeDef
 
-    data: ActionInvocationTypeDef = {...}
+    data: ActionInvocationTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -35,22 +35,22 @@
 
 __all__ = (
     "ActionInvocationTypeDef",
     "ActionTypeDef",
     "ResponseMetadataTypeDef",
     "ApplicationTypeDef",
     "AppliedExtensionTypeDef",
+    "BlobTypeDef",
     "ConfigurationProfileSummaryTypeDef",
     "ValidatorTypeDef",
     "CreateApplicationRequestRequestTypeDef",
     "CreateDeploymentStrategyRequestRequestTypeDef",
     "MonitorTypeDef",
     "CreateExtensionAssociationRequestRequestTypeDef",
     "ParameterTypeDef",
-    "CreateHostedConfigurationVersionRequestRequestTypeDef",
     "DeleteApplicationRequestRequestTypeDef",
     "DeleteConfigurationProfileRequestRequestTypeDef",
     "DeleteDeploymentStrategyRequestRequestTypeDef",
     "DeleteEnvironmentRequestRequestTypeDef",
     "DeleteExtensionAssociationRequestRequestTypeDef",
     "DeleteExtensionRequestRequestTypeDef",
     "DeleteHostedConfigurationVersionRequestRequestTypeDef",
@@ -90,14 +90,15 @@
     "ConfigurationTypeDef",
     "DeploymentStrategyResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "ExtensionAssociationTypeDef",
     "HostedConfigurationVersionTypeDef",
     "ResourceTagsTypeDef",
     "ApplicationsTypeDef",
+    "CreateHostedConfigurationVersionRequestRequestTypeDef",
     "ConfigurationProfilesTypeDef",
     "ConfigurationProfileTypeDef",
     "CreateConfigurationProfileRequestRequestTypeDef",
     "UpdateConfigurationProfileRequestRequestTypeDef",
     "CreateEnvironmentRequestRequestTypeDef",
     "EnvironmentResponseTypeDef",
     "EnvironmentTypeDef",
@@ -167,14 +168,15 @@
         "ExtensionAssociationId": str,
         "VersionNumber": int,
         "Parameters": Dict[str, str],
     },
     total=False,
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 ConfigurationProfileSummaryTypeDef = TypedDict(
     "ConfigurationProfileSummaryTypeDef",
     {
         "ApplicationId": str,
         "Id": str,
         "Name": str,
         "LocationUri": str,
@@ -283,39 +285,14 @@
     {
         "Description": str,
         "Required": bool,
     },
     total=False,
 )
 
-_RequiredCreateHostedConfigurationVersionRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateHostedConfigurationVersionRequestRequestTypeDef",
-    {
-        "ApplicationId": str,
-        "ConfigurationProfileId": str,
-        "Content": Union[str, bytes, IO[Any], StreamingBody],
-        "ContentType": str,
-    },
-)
-_OptionalCreateHostedConfigurationVersionRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateHostedConfigurationVersionRequestRequestTypeDef",
-    {
-        "Description": str,
-        "LatestVersionNumber": int,
-        "VersionLabel": str,
-    },
-    total=False,
-)
-
-class CreateHostedConfigurationVersionRequestRequestTypeDef(
-    _RequiredCreateHostedConfigurationVersionRequestRequestTypeDef,
-    _OptionalCreateHostedConfigurationVersionRequestRequestTypeDef,
-):
-    pass
-
 DeleteApplicationRequestRequestTypeDef = TypedDict(
     "DeleteApplicationRequestRequestTypeDef",
     {
         "ApplicationId": str,
     },
 )
 
@@ -891,14 +868,39 @@
     {
         "Items": List[ApplicationTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredCreateHostedConfigurationVersionRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateHostedConfigurationVersionRequestRequestTypeDef",
+    {
+        "ApplicationId": str,
+        "ConfigurationProfileId": str,
+        "Content": BlobTypeDef,
+        "ContentType": str,
+    },
+)
+_OptionalCreateHostedConfigurationVersionRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateHostedConfigurationVersionRequestRequestTypeDef",
+    {
+        "Description": str,
+        "LatestVersionNumber": int,
+        "VersionLabel": str,
+    },
+    total=False,
+)
+
+class CreateHostedConfigurationVersionRequestRequestTypeDef(
+    _RequiredCreateHostedConfigurationVersionRequestRequestTypeDef,
+    _OptionalCreateHostedConfigurationVersionRequestRequestTypeDef,
+):
+    pass
+
 ConfigurationProfilesTypeDef = TypedDict(
     "ConfigurationProfilesTypeDef",
     {
         "Items": List[ConfigurationProfileSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-appconfig-1.28.15.post1/mypy_boto3_appconfig.egg-info/PKG-INFO` & `mypy-boto3-appconfig-1.28.16/mypy_boto3_appconfig.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-appconfig
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.AppConfig 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.AppConfig 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appconfig/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 appconfig type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 appconfig type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-appconfig.svg?color=blue)](https://pypi.org/project/mypy-boto3-appconfig)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appconfig/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-appconfig)](https://pepy.tech/project/mypy-boto3-appconfig)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AppConfig 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig)
+[boto3.AppConfig 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig)
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
 [mypy-boto3-appconfig docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appconfig/).
 
 See how it helps to find and fix potential bugs:
 
@@ -73,15 +73,15 @@
     - [Sublime Text](#sublime-text)
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
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
@@ -294,36 +294,36 @@
 )
 
 
 def check_value(value: ActionPointType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_appconfig.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_appconfig.type_defs import (
     ActionInvocationTypeDef,
     ActionTypeDef,
     ResponseMetadataTypeDef,
     ApplicationTypeDef,
     AppliedExtensionTypeDef,
+    BlobTypeDef,
     ConfigurationProfileSummaryTypeDef,
     ValidatorTypeDef,
     CreateApplicationRequestRequestTypeDef,
     CreateDeploymentStrategyRequestRequestTypeDef,
     MonitorTypeDef,
     CreateExtensionAssociationRequestRequestTypeDef,
     ParameterTypeDef,
-    CreateHostedConfigurationVersionRequestRequestTypeDef,
     DeleteApplicationRequestRequestTypeDef,
     DeleteConfigurationProfileRequestRequestTypeDef,
     DeleteDeploymentStrategyRequestRequestTypeDef,
     DeleteEnvironmentRequestRequestTypeDef,
     DeleteExtensionAssociationRequestRequestTypeDef,
     DeleteExtensionRequestRequestTypeDef,
     DeleteHostedConfigurationVersionRequestRequestTypeDef,
@@ -363,14 +363,15 @@
     ConfigurationTypeDef,
     DeploymentStrategyResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     ExtensionAssociationTypeDef,
     HostedConfigurationVersionTypeDef,
     ResourceTagsTypeDef,
     ApplicationsTypeDef,
+    CreateHostedConfigurationVersionRequestRequestTypeDef,
     ConfigurationProfilesTypeDef,
     ConfigurationProfileTypeDef,
     CreateConfigurationProfileRequestRequestTypeDef,
     UpdateConfigurationProfileRequestRequestTypeDef,
     CreateEnvironmentRequestRequestTypeDef,
     EnvironmentResponseTypeDef,
     EnvironmentTypeDef,
@@ -384,15 +385,15 @@
     ExtensionsTypeDef,
     HostedConfigurationVersionsTypeDef,
     DeploymentTypeDef,
     EnvironmentsTypeDef,
 )
 
 
-def get_structure() -> ActionInvocationTypeDef:
+def get_value() -> ActionInvocationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-appconfig-1.28.15.post1/mypy_boto3_appconfig.egg-info/SOURCES.txt` & `mypy-boto3-appconfig-1.28.16/mypy_boto3_appconfig.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appconfig-1.28.15.post1/setup.py` & `mypy-boto3-appconfig-1.28.16/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-appconfig",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_appconfig"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.AppConfig 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.2"
+        "Type annotations for boto3.AppConfig 1.28.16 service generated with mypy-boto3-builder"
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
-    keywords="boto3 appconfig type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 appconfig type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_appconfig": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appconfig/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

