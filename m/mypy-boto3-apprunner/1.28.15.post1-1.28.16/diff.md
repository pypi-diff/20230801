# Comparing `tmp/mypy-boto3-apprunner-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-apprunner-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-apprunner-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:31 2023, max compression
+gzip compressed data, was "mypy-boto3-apprunner-1.28.16.tar", last modified: Tue Aug  1 11:36:11 2023, max compression
```

## Comparing `mypy-boto3-apprunner-1.28.15.post1.tar` & `mypy-boto3-apprunner-1.28.16.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:31.193008 mypy-boto3-apprunner-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:38:25.000000 mypy-boto3-apprunner-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16886 2023-07-29 10:02:31.193008 mypy-boto3-apprunner-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15385 2023-07-29 09:38:25.000000 mypy-boto3-apprunner-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:31.185008 mypy-boto3-apprunner-1.28.15.post1/mypy_boto3_apprunner/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-29 09:38:25.000000 mypy-boto3-apprunner-1.28.15.post1/mypy_boto3_apprunner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-29 09:38:25.000000 mypy-boto3-apprunner-1.28.15.post1/mypy_boto3_apprunner/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-29 09:38:25.000000 mypy-boto3-apprunner-1.28.15.post1/mypy_boto3_apprunner/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25827 2023-07-29 09:38:26.000000 mypy-boto3-apprunner-1.28.15.post1/mypy_boto3_apprunner/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    25785 2023-07-29 09:38:25.000000 mypy-boto3-apprunner-1.28.15.post1/mypy_boto3_apprunner/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10153 2023-07-29 09:38:26.000000 mypy-boto3-apprunner-1.28.15.post1/mypy_boto3_apprunner/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10151 2023-07-29 09:38:26.000000 mypy-boto3-apprunner-1.28.15.post1/mypy_boto3_apprunner/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:38:25.000000 mypy-boto3-apprunner-1.28.15.post1/mypy_boto3_apprunner/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    38636 2023-07-29 09:38:27.000000 mypy-boto3-apprunner-1.28.15.post1/mypy_boto3_apprunner/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    38593 2023-07-29 09:38:26.000000 mypy-boto3-apprunner-1.28.15.post1/mypy_boto3_apprunner/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:38:25.000000 mypy-boto3-apprunner-1.28.15.post1/mypy_boto3_apprunner/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:31.193008 mypy-boto3-apprunner-1.28.15.post1/mypy_boto3_apprunner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16886 2023-07-29 10:02:30.000000 mypy-boto3-apprunner-1.28.15.post1/mypy_boto3_apprunner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-29 10:02:30.000000 mypy-boto3-apprunner-1.28.15.post1/mypy_boto3_apprunner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:30.000000 mypy-boto3-apprunner-1.28.15.post1/mypy_boto3_apprunner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:30.000000 mypy-boto3-apprunner-1.28.15.post1/mypy_boto3_apprunner.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:30.000000 mypy-boto3-apprunner-1.28.15.post1/mypy_boto3_apprunner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-29 10:02:30.000000 mypy-boto3-apprunner-1.28.15.post1/mypy_boto3_apprunner.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:31.193008 mypy-boto3-apprunner-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-07-29 09:38:25.000000 mypy-boto3-apprunner-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:11.936950 mypy-boto3-apprunner-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:10:57.000000 mypy-boto3-apprunner-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16913 2023-08-01 11:36:11.928950 mypy-boto3-apprunner-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15421 2023-08-01 11:10:57.000000 mypy-boto3-apprunner-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:11.928950 mypy-boto3-apprunner-1.28.16/mypy_boto3_apprunner/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-08-01 11:10:57.000000 mypy-boto3-apprunner-1.28.16/mypy_boto3_apprunner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-08-01 11:10:57.000000 mypy-boto3-apprunner-1.28.16/mypy_boto3_apprunner/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-08-01 11:10:57.000000 mypy-boto3-apprunner-1.28.16/mypy_boto3_apprunner/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25693 2023-08-01 11:10:57.000000 mypy-boto3-apprunner-1.28.16/mypy_boto3_apprunner/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25651 2023-08-01 11:10:57.000000 mypy-boto3-apprunner-1.28.16/mypy_boto3_apprunner/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10153 2023-08-01 11:10:57.000000 mypy-boto3-apprunner-1.28.16/mypy_boto3_apprunner/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10151 2023-08-01 11:10:57.000000 mypy-boto3-apprunner-1.28.16/mypy_boto3_apprunner/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:10:57.000000 mypy-boto3-apprunner-1.28.16/mypy_boto3_apprunner/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    38788 2023-08-01 11:10:59.000000 mypy-boto3-apprunner-1.28.16/mypy_boto3_apprunner/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38745 2023-08-01 11:10:59.000000 mypy-boto3-apprunner-1.28.16/mypy_boto3_apprunner/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:10:57.000000 mypy-boto3-apprunner-1.28.16/mypy_boto3_apprunner/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:11.928950 mypy-boto3-apprunner-1.28.16/mypy_boto3_apprunner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16913 2023-08-01 11:36:11.000000 mypy-boto3-apprunner-1.28.16/mypy_boto3_apprunner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-08-01 11:36:11.000000 mypy-boto3-apprunner-1.28.16/mypy_boto3_apprunner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:11.000000 mypy-boto3-apprunner-1.28.16/mypy_boto3_apprunner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:11.000000 mypy-boto3-apprunner-1.28.16/mypy_boto3_apprunner.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:11.000000 mypy-boto3-apprunner-1.28.16/mypy_boto3_apprunner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-01 11:36:11.000000 mypy-boto3-apprunner-1.28.16/mypy_boto3_apprunner.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:11.936950 mypy-boto3-apprunner-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-08-01 11:10:57.000000 mypy-boto3-apprunner-1.28.16/setup.py
```

### Comparing `mypy-boto3-apprunner-1.28.15.post1/LICENSE` & `mypy-boto3-apprunner-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-apprunner-1.28.15.post1/PKG-INFO` & `mypy-boto3-apprunner-1.28.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-apprunner
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.AppRunner 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.AppRunner 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apprunner/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 apprunner type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 apprunner type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-apprunner.svg?color=blue)](https://pypi.org/project/mypy-boto3-apprunner)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apprunner/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-apprunner)](https://pepy.tech/project/mypy-boto3-apprunner)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AppRunner 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apprunner.html#AppRunner)
+[boto3.AppRunner 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apprunner.html#AppRunner)
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
 [mypy-boto3-apprunner docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apprunner/).
 
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
@@ -304,20 +304,20 @@
 )
 
 
 def check_value(value: AutoScalingConfigurationStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_apprunner.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_apprunner.type_defs import (
     AssociateCustomDomainRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     VpcDNSTargetTypeDef,
     AuthenticationConfigurationTypeDef,
@@ -415,25 +415,26 @@
     DeleteVpcIngressConnectionResponseTypeDef,
     DescribeVpcIngressConnectionResponseTypeDef,
     UpdateVpcIngressConnectionResponseTypeDef,
     SourceConfigurationOutputTypeDef,
     SourceConfigurationTypeDef,
     ServiceTypeDef,
     CreateServiceRequestRequestTypeDef,
+    SourceConfigurationUnionTypeDef,
     UpdateServiceRequestRequestTypeDef,
     CreateServiceResponseTypeDef,
     DeleteServiceResponseTypeDef,
     DescribeServiceResponseTypeDef,
     PauseServiceResponseTypeDef,
     ResumeServiceResponseTypeDef,
     UpdateServiceResponseTypeDef,
 )
 
 
-def get_structure() -> AssociateCustomDomainRequestRequestTypeDef:
+def get_value() -> AssociateCustomDomainRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-apprunner-1.28.15.post1/README.md` & `mypy-boto3-apprunner-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-apprunner.svg?color=blue)](https://pypi.org/project/mypy-boto3-apprunner)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apprunner/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-apprunner)](https://pepy.tech/project/mypy-boto3-apprunner)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AppRunner 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apprunner.html#AppRunner)
+[boto3.AppRunner 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apprunner.html#AppRunner)
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
 [mypy-boto3-apprunner docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apprunner/).
 
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
@@ -272,20 +272,20 @@
 )
 
 
 def check_value(value: AutoScalingConfigurationStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_apprunner.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_apprunner.type_defs import (
     AssociateCustomDomainRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     VpcDNSTargetTypeDef,
     AuthenticationConfigurationTypeDef,
@@ -383,25 +383,26 @@
     DeleteVpcIngressConnectionResponseTypeDef,
     DescribeVpcIngressConnectionResponseTypeDef,
     UpdateVpcIngressConnectionResponseTypeDef,
     SourceConfigurationOutputTypeDef,
     SourceConfigurationTypeDef,
     ServiceTypeDef,
     CreateServiceRequestRequestTypeDef,
+    SourceConfigurationUnionTypeDef,
     UpdateServiceRequestRequestTypeDef,
     CreateServiceResponseTypeDef,
     DeleteServiceResponseTypeDef,
     DescribeServiceResponseTypeDef,
     PauseServiceResponseTypeDef,
     ResumeServiceResponseTypeDef,
     UpdateServiceResponseTypeDef,
 )
 
 
-def get_structure() -> AssociateCustomDomainRequestRequestTypeDef:
+def get_value() -> AssociateCustomDomainRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-apprunner-1.28.15.post1/mypy_boto3_apprunner/__main__.py` & `mypy-boto3-apprunner-1.28.16/mypy_boto3_apprunner/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.AppRunner 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.AppRunner 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apprunner//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apprunner.html#AppRunner\nOther"
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

### Comparing `mypy-boto3-apprunner-1.28.15.post1/mypy_boto3_apprunner/client.py` & `mypy-boto3-apprunner-1.28.16/mypy_boto3_apprunner/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_apprunner.client import AppRunnerClient
 
     session = Session()
     client: AppRunnerClient = session.client("apprunner")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .type_defs import (
     AssociateCustomDomainResponseTypeDef,
     CreateAutoScalingConfigurationResponseTypeDef,
     CreateConnectionResponseTypeDef,
@@ -52,16 +52,15 @@
     ListVpcConnectorsResponseTypeDef,
     ListVpcIngressConnectionsFilterTypeDef,
     ListVpcIngressConnectionsResponseTypeDef,
     NetworkConfigurationTypeDef,
     PauseServiceResponseTypeDef,
     ResumeServiceResponseTypeDef,
     ServiceObservabilityConfigurationTypeDef,
-    SourceConfigurationOutputTypeDef,
-    SourceConfigurationTypeDef,
+    SourceConfigurationUnionTypeDef,
     StartDeploymentResponseTypeDef,
     TagTypeDef,
     TraceConfigurationTypeDef,
     UpdateServiceResponseTypeDef,
     UpdateVpcIngressConnectionResponseTypeDef,
 )
 
@@ -179,15 +178,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apprunner/client/#create_observability_configuration)
         """
 
     def create_service(
         self,
         *,
         ServiceName: str,
-        SourceConfiguration: Union[SourceConfigurationTypeDef, SourceConfigurationOutputTypeDef],
+        SourceConfiguration: SourceConfigurationUnionTypeDef,
         InstanceConfiguration: InstanceConfigurationTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         EncryptionConfiguration: EncryptionConfigurationTypeDef = ...,
         HealthCheckConfiguration: HealthCheckConfigurationTypeDef = ...,
         AutoScalingConfigurationArn: str = ...,
         NetworkConfiguration: NetworkConfigurationTypeDef = ...,
         ObservabilityConfiguration: ServiceObservabilityConfigurationTypeDef = ...
@@ -506,17 +505,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apprunner/client/#untag_resource)
         """
 
     def update_service(
         self,
         *,
         ServiceArn: str,
-        SourceConfiguration: Union[
-            SourceConfigurationTypeDef, SourceConfigurationOutputTypeDef
-        ] = ...,
+        SourceConfiguration: SourceConfigurationUnionTypeDef = ...,
         InstanceConfiguration: InstanceConfigurationTypeDef = ...,
         AutoScalingConfigurationArn: str = ...,
         HealthCheckConfiguration: HealthCheckConfigurationTypeDef = ...,
         NetworkConfiguration: NetworkConfigurationTypeDef = ...,
         ObservabilityConfiguration: ServiceObservabilityConfigurationTypeDef = ...
     ) -> UpdateServiceResponseTypeDef:
         """
```

### Comparing `mypy-boto3-apprunner-1.28.15.post1/mypy_boto3_apprunner/client.pyi` & `mypy-boto3-apprunner-1.28.16/mypy_boto3_apprunner/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_apprunner.client import AppRunnerClient
 
     session = Session()
     client: AppRunnerClient = session.client("apprunner")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .type_defs import (
     AssociateCustomDomainResponseTypeDef,
     CreateAutoScalingConfigurationResponseTypeDef,
     CreateConnectionResponseTypeDef,
@@ -52,16 +52,15 @@
     ListVpcConnectorsResponseTypeDef,
     ListVpcIngressConnectionsFilterTypeDef,
     ListVpcIngressConnectionsResponseTypeDef,
     NetworkConfigurationTypeDef,
     PauseServiceResponseTypeDef,
     ResumeServiceResponseTypeDef,
     ServiceObservabilityConfigurationTypeDef,
-    SourceConfigurationOutputTypeDef,
-    SourceConfigurationTypeDef,
+    SourceConfigurationUnionTypeDef,
     StartDeploymentResponseTypeDef,
     TagTypeDef,
     TraceConfigurationTypeDef,
     UpdateServiceResponseTypeDef,
     UpdateVpcIngressConnectionResponseTypeDef,
 )
 
@@ -168,15 +167,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apprunner.html#AppRunner.Client.create_observability_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apprunner/client/#create_observability_configuration)
         """
     def create_service(
         self,
         *,
         ServiceName: str,
-        SourceConfiguration: Union[SourceConfigurationTypeDef, SourceConfigurationOutputTypeDef],
+        SourceConfiguration: SourceConfigurationUnionTypeDef,
         InstanceConfiguration: InstanceConfigurationTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         EncryptionConfiguration: EncryptionConfigurationTypeDef = ...,
         HealthCheckConfiguration: HealthCheckConfigurationTypeDef = ...,
         AutoScalingConfigurationArn: str = ...,
         NetworkConfiguration: NetworkConfigurationTypeDef = ...,
         ObservabilityConfiguration: ServiceObservabilityConfigurationTypeDef = ...
@@ -465,17 +464,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apprunner.html#AppRunner.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apprunner/client/#untag_resource)
         """
     def update_service(
         self,
         *,
         ServiceArn: str,
-        SourceConfiguration: Union[
-            SourceConfigurationTypeDef, SourceConfigurationOutputTypeDef
-        ] = ...,
+        SourceConfiguration: SourceConfigurationUnionTypeDef = ...,
         InstanceConfiguration: InstanceConfigurationTypeDef = ...,
         AutoScalingConfigurationArn: str = ...,
         HealthCheckConfiguration: HealthCheckConfigurationTypeDef = ...,
         NetworkConfiguration: NetworkConfigurationTypeDef = ...,
         ObservabilityConfiguration: ServiceObservabilityConfigurationTypeDef = ...
     ) -> UpdateServiceResponseTypeDef:
         """
```

### Comparing `mypy-boto3-apprunner-1.28.15.post1/mypy_boto3_apprunner/literals.py` & `mypy-boto3-apprunner-1.28.16/mypy_boto3_apprunner/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-apprunner-1.28.15.post1/mypy_boto3_apprunner/literals.pyi` & `mypy-boto3-apprunner-1.28.16/mypy_boto3_apprunner/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-apprunner-1.28.15.post1/mypy_boto3_apprunner/type_defs.py` & `mypy-boto3-apprunner-1.28.16/mypy_boto3_apprunner/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apprunner/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_apprunner.type_defs import AssociateCustomDomainRequestRequestTypeDef
 
-    data: AssociateCustomDomainRequestRequestTypeDef = {...}
+    data: AssociateCustomDomainRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AutoScalingConfigurationStatusType,
     CertificateValidationRecordStatusType,
     ConfigurationSourceType,
     ConnectionStatusType,
     CustomDomainAssociationStatusType,
@@ -38,15 +38,14 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AssociateCustomDomainRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "VpcDNSTargetTypeDef",
     "AuthenticationConfigurationTypeDef",
     "AutoScalingConfigurationSummaryTypeDef",
     "AutoScalingConfigurationTypeDef",
@@ -142,14 +141,15 @@
     "DeleteVpcIngressConnectionResponseTypeDef",
     "DescribeVpcIngressConnectionResponseTypeDef",
     "UpdateVpcIngressConnectionResponseTypeDef",
     "SourceConfigurationOutputTypeDef",
     "SourceConfigurationTypeDef",
     "ServiceTypeDef",
     "CreateServiceRequestRequestTypeDef",
+    "SourceConfigurationUnionTypeDef",
     "UpdateServiceRequestRequestTypeDef",
     "CreateServiceResponseTypeDef",
     "DeleteServiceResponseTypeDef",
     "DescribeServiceResponseTypeDef",
     "PauseServiceResponseTypeDef",
     "ResumeServiceResponseTypeDef",
     "UpdateServiceResponseTypeDef",
@@ -166,22 +166,20 @@
     "_OptionalAssociateCustomDomainRequestRequestTypeDef",
     {
         "EnableWWWSubdomain": bool,
     },
     total=False,
 )
 
-
 class AssociateCustomDomainRequestRequestTypeDef(
     _RequiredAssociateCustomDomainRequestRequestTypeDef,
     _OptionalAssociateCustomDomainRequestRequestTypeDef,
 ):
     pass
 
-
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -260,21 +258,19 @@
         "Port": str,
         "RuntimeEnvironmentVariables": Dict[str, str],
         "RuntimeEnvironmentSecrets": Dict[str, str],
     },
     total=False,
 )
 
-
 class CodeConfigurationValuesOutputTypeDef(
     _RequiredCodeConfigurationValuesOutputTypeDef, _OptionalCodeConfigurationValuesOutputTypeDef
 ):
     pass
 
-
 _RequiredCodeConfigurationValuesTypeDef = TypedDict(
     "_RequiredCodeConfigurationValuesTypeDef",
     {
         "Runtime": RuntimeType,
     },
 )
 _OptionalCodeConfigurationValuesTypeDef = TypedDict(
@@ -285,21 +281,19 @@
         "Port": str,
         "RuntimeEnvironmentVariables": Mapping[str, str],
         "RuntimeEnvironmentSecrets": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CodeConfigurationValuesTypeDef(
     _RequiredCodeConfigurationValuesTypeDef, _OptionalCodeConfigurationValuesTypeDef
 ):
     pass
 
-
 SourceCodeVersionTypeDef = TypedDict(
     "SourceCodeVersionTypeDef",
     {
         "Type": Literal["BRANCH"],
         "Value": str,
     },
 )
@@ -384,22 +378,20 @@
     "_OptionalServiceObservabilityConfigurationTypeDef",
     {
         "ObservabilityConfigurationArn": str,
     },
     total=False,
 )
 
-
 class ServiceObservabilityConfigurationTypeDef(
     _RequiredServiceObservabilityConfigurationTypeDef,
     _OptionalServiceObservabilityConfigurationTypeDef,
 ):
     pass
 
-
 VpcConnectorTypeDef = TypedDict(
     "VpcConnectorTypeDef",
     {
         "VpcConnectorName": str,
         "VpcConnectorArn": str,
         "VpcConnectorRevision": int,
         "Subnets": List[str],
@@ -480,22 +472,20 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class DescribeCustomDomainsRequestRequestTypeDef(
     _RequiredDescribeCustomDomainsRequestRequestTypeDef,
     _OptionalDescribeCustomDomainsRequestRequestTypeDef,
 ):
     pass
 
-
 DescribeObservabilityConfigurationRequestRequestTypeDef = TypedDict(
     "DescribeObservabilityConfigurationRequestRequestTypeDef",
     {
         "ObservabilityConfigurationArn": str,
     },
 )
 
@@ -620,21 +610,19 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListOperationsRequestRequestTypeDef(
     _RequiredListOperationsRequestRequestTypeDef, _OptionalListOperationsRequestRequestTypeDef
 ):
     pass
 
-
 OperationSummaryTypeDef = TypedDict(
     "OperationSummaryTypeDef",
     {
         "Id": str,
         "Type": OperationTypeType,
         "Status": OperationStatusType,
         "TargetArn": str,
@@ -784,61 +772,55 @@
     "_OptionalCustomDomainTypeDef",
     {
         "CertificateValidationRecords": List[CertificateValidationRecordTypeDef],
     },
     total=False,
 )
 
-
 class CustomDomainTypeDef(_RequiredCustomDomainTypeDef, _OptionalCustomDomainTypeDef):
     pass
 
-
 _RequiredCodeConfigurationOutputTypeDef = TypedDict(
     "_RequiredCodeConfigurationOutputTypeDef",
     {
         "ConfigurationSource": ConfigurationSourceType,
     },
 )
 _OptionalCodeConfigurationOutputTypeDef = TypedDict(
     "_OptionalCodeConfigurationOutputTypeDef",
     {
         "CodeConfigurationValues": CodeConfigurationValuesOutputTypeDef,
     },
     total=False,
 )
 
-
 class CodeConfigurationOutputTypeDef(
     _RequiredCodeConfigurationOutputTypeDef, _OptionalCodeConfigurationOutputTypeDef
 ):
     pass
 
-
 _RequiredCodeConfigurationTypeDef = TypedDict(
     "_RequiredCodeConfigurationTypeDef",
     {
         "ConfigurationSource": ConfigurationSourceType,
     },
 )
 _OptionalCodeConfigurationTypeDef = TypedDict(
     "_OptionalCodeConfigurationTypeDef",
     {
         "CodeConfigurationValues": CodeConfigurationValuesTypeDef,
     },
     total=False,
 )
 
-
 class CodeConfigurationTypeDef(
     _RequiredCodeConfigurationTypeDef, _OptionalCodeConfigurationTypeDef
 ):
     pass
 
-
 ListConnectionsResponseTypeDef = TypedDict(
     "ListConnectionsResponseTypeDef",
     {
         "ConnectionSummaryList": List[ConnectionSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -873,22 +855,20 @@
         "MinSize": int,
         "MaxSize": int,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateAutoScalingConfigurationRequestRequestTypeDef(
     _RequiredCreateAutoScalingConfigurationRequestRequestTypeDef,
     _OptionalCreateAutoScalingConfigurationRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateConnectionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateConnectionRequestRequestTypeDef",
     {
         "ConnectionName": str,
         "ProviderType": Literal["GITHUB"],
     },
 )
@@ -896,21 +876,19 @@
     "_OptionalCreateConnectionRequestRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateConnectionRequestRequestTypeDef(
     _RequiredCreateConnectionRequestRequestTypeDef, _OptionalCreateConnectionRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateVpcConnectorRequestRequestTypeDef = TypedDict(
     "_RequiredCreateVpcConnectorRequestRequestTypeDef",
     {
         "VpcConnectorName": str,
         "Subnets": Sequence[str],
     },
 )
@@ -919,22 +897,20 @@
     {
         "SecurityGroups": Sequence[str],
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateVpcConnectorRequestRequestTypeDef(
     _RequiredCreateVpcConnectorRequestRequestTypeDef,
     _OptionalCreateVpcConnectorRequestRequestTypeDef,
 ):
     pass
 
-
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -958,22 +934,20 @@
     {
         "TraceConfiguration": TraceConfigurationTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateObservabilityConfigurationRequestRequestTypeDef(
     _RequiredCreateObservabilityConfigurationRequestRequestTypeDef,
     _OptionalCreateObservabilityConfigurationRequestRequestTypeDef,
 ):
     pass
 
-
 ObservabilityConfigurationTypeDef = TypedDict(
     "ObservabilityConfigurationTypeDef",
     {
         "ObservabilityConfigurationArn": str,
         "ObservabilityConfigurationName": str,
         "TraceConfiguration": TraceConfigurationTypeDef,
         "ObservabilityConfigurationRevision": int,
@@ -1030,22 +1004,20 @@
     "_OptionalCreateVpcIngressConnectionRequestRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateVpcIngressConnectionRequestRequestTypeDef(
     _RequiredCreateVpcIngressConnectionRequestRequestTypeDef,
     _OptionalCreateVpcIngressConnectionRequestRequestTypeDef,
 ):
     pass
 
-
 UpdateVpcIngressConnectionRequestRequestTypeDef = TypedDict(
     "UpdateVpcIngressConnectionRequestRequestTypeDef",
     {
         "VpcIngressConnectionArn": str,
         "IngressVpcConfiguration": IngressVpcConfigurationTypeDef,
     },
 )
@@ -1077,21 +1049,19 @@
     "_OptionalImageRepositoryOutputTypeDef",
     {
         "ImageConfiguration": ImageConfigurationOutputTypeDef,
     },
     total=False,
 )
 
-
 class ImageRepositoryOutputTypeDef(
     _RequiredImageRepositoryOutputTypeDef, _OptionalImageRepositoryOutputTypeDef
 ):
     pass
 
-
 _RequiredImageRepositoryTypeDef = TypedDict(
     "_RequiredImageRepositoryTypeDef",
     {
         "ImageIdentifier": str,
         "ImageRepositoryType": ImageRepositoryTypeType,
     },
 )
@@ -1099,19 +1069,17 @@
     "_OptionalImageRepositoryTypeDef",
     {
         "ImageConfiguration": ImageConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class ImageRepositoryTypeDef(_RequiredImageRepositoryTypeDef, _OptionalImageRepositoryTypeDef):
     pass
 
-
 NetworkConfigurationTypeDef = TypedDict(
     "NetworkConfigurationTypeDef",
     {
         "EgressConfiguration": EgressConfigurationTypeDef,
         "IngressConfiguration": IngressConfigurationTypeDef,
     },
     total=False,
@@ -1208,21 +1176,19 @@
     "_OptionalCodeRepositoryOutputTypeDef",
     {
         "CodeConfiguration": CodeConfigurationOutputTypeDef,
     },
     total=False,
 )
 
-
 class CodeRepositoryOutputTypeDef(
     _RequiredCodeRepositoryOutputTypeDef, _OptionalCodeRepositoryOutputTypeDef
 ):
     pass
 
-
 _RequiredCodeRepositoryTypeDef = TypedDict(
     "_RequiredCodeRepositoryTypeDef",
     {
         "RepositoryUrl": str,
         "SourceCodeVersion": SourceCodeVersionTypeDef,
     },
 )
@@ -1230,19 +1196,17 @@
     "_OptionalCodeRepositoryTypeDef",
     {
         "CodeConfiguration": CodeConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class CodeRepositoryTypeDef(_RequiredCodeRepositoryTypeDef, _OptionalCodeRepositoryTypeDef):
     pass
 
-
 CreateObservabilityConfigurationResponseTypeDef = TypedDict(
     "CreateObservabilityConfigurationResponseTypeDef",
     {
         "ObservabilityConfiguration": ObservabilityConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1340,19 +1304,17 @@
         "EncryptionConfiguration": EncryptionConfigurationTypeDef,
         "HealthCheckConfiguration": HealthCheckConfigurationTypeDef,
         "ObservabilityConfiguration": ServiceObservabilityConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class ServiceTypeDef(_RequiredServiceTypeDef, _OptionalServiceTypeDef):
     pass
 
-
 _RequiredCreateServiceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateServiceRequestRequestTypeDef",
     {
         "ServiceName": str,
         "SourceConfiguration": SourceConfigurationTypeDef,
     },
 )
@@ -1366,21 +1328,22 @@
         "AutoScalingConfigurationArn": str,
         "NetworkConfiguration": NetworkConfigurationTypeDef,
         "ObservabilityConfiguration": ServiceObservabilityConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class CreateServiceRequestRequestTypeDef(
     _RequiredCreateServiceRequestRequestTypeDef, _OptionalCreateServiceRequestRequestTypeDef
 ):
     pass
 
-
+SourceConfigurationUnionTypeDef = Union[
+    SourceConfigurationTypeDef, SourceConfigurationOutputTypeDef
+]
 _RequiredUpdateServiceRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateServiceRequestRequestTypeDef",
     {
         "ServiceArn": str,
     },
 )
 _OptionalUpdateServiceRequestRequestTypeDef = TypedDict(
@@ -1392,21 +1355,19 @@
         "HealthCheckConfiguration": HealthCheckConfigurationTypeDef,
         "NetworkConfiguration": NetworkConfigurationTypeDef,
         "ObservabilityConfiguration": ServiceObservabilityConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class UpdateServiceRequestRequestTypeDef(
     _RequiredUpdateServiceRequestRequestTypeDef, _OptionalUpdateServiceRequestRequestTypeDef
 ):
     pass
 
-
 CreateServiceResponseTypeDef = TypedDict(
     "CreateServiceResponseTypeDef",
     {
         "Service": ServiceTypeDef,
         "OperationId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-apprunner-1.28.15.post1/mypy_boto3_apprunner/type_defs.pyi` & `mypy-boto3-apprunner-1.28.16/mypy_boto3_apprunner/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apprunner/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_apprunner.type_defs import AssociateCustomDomainRequestRequestTypeDef
 
-    data: AssociateCustomDomainRequestRequestTypeDef = {...}
+    data: AssociateCustomDomainRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AutoScalingConfigurationStatusType,
     CertificateValidationRecordStatusType,
     ConfigurationSourceType,
     ConnectionStatusType,
     CustomDomainAssociationStatusType,
@@ -38,14 +38,15 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AssociateCustomDomainRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "VpcDNSTargetTypeDef",
     "AuthenticationConfigurationTypeDef",
     "AutoScalingConfigurationSummaryTypeDef",
     "AutoScalingConfigurationTypeDef",
@@ -141,14 +142,15 @@
     "DeleteVpcIngressConnectionResponseTypeDef",
     "DescribeVpcIngressConnectionResponseTypeDef",
     "UpdateVpcIngressConnectionResponseTypeDef",
     "SourceConfigurationOutputTypeDef",
     "SourceConfigurationTypeDef",
     "ServiceTypeDef",
     "CreateServiceRequestRequestTypeDef",
+    "SourceConfigurationUnionTypeDef",
     "UpdateServiceRequestRequestTypeDef",
     "CreateServiceResponseTypeDef",
     "DeleteServiceResponseTypeDef",
     "DescribeServiceResponseTypeDef",
     "PauseServiceResponseTypeDef",
     "ResumeServiceResponseTypeDef",
     "UpdateServiceResponseTypeDef",
@@ -165,20 +167,22 @@
     "_OptionalAssociateCustomDomainRequestRequestTypeDef",
     {
         "EnableWWWSubdomain": bool,
     },
     total=False,
 )
 
+
 class AssociateCustomDomainRequestRequestTypeDef(
     _RequiredAssociateCustomDomainRequestRequestTypeDef,
     _OptionalAssociateCustomDomainRequestRequestTypeDef,
 ):
     pass
 
+
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -257,19 +261,21 @@
         "Port": str,
         "RuntimeEnvironmentVariables": Dict[str, str],
         "RuntimeEnvironmentSecrets": Dict[str, str],
     },
     total=False,
 )
 
+
 class CodeConfigurationValuesOutputTypeDef(
     _RequiredCodeConfigurationValuesOutputTypeDef, _OptionalCodeConfigurationValuesOutputTypeDef
 ):
     pass
 
+
 _RequiredCodeConfigurationValuesTypeDef = TypedDict(
     "_RequiredCodeConfigurationValuesTypeDef",
     {
         "Runtime": RuntimeType,
     },
 )
 _OptionalCodeConfigurationValuesTypeDef = TypedDict(
@@ -280,19 +286,21 @@
         "Port": str,
         "RuntimeEnvironmentVariables": Mapping[str, str],
         "RuntimeEnvironmentSecrets": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CodeConfigurationValuesTypeDef(
     _RequiredCodeConfigurationValuesTypeDef, _OptionalCodeConfigurationValuesTypeDef
 ):
     pass
 
+
 SourceCodeVersionTypeDef = TypedDict(
     "SourceCodeVersionTypeDef",
     {
         "Type": Literal["BRANCH"],
         "Value": str,
     },
 )
@@ -377,20 +385,22 @@
     "_OptionalServiceObservabilityConfigurationTypeDef",
     {
         "ObservabilityConfigurationArn": str,
     },
     total=False,
 )
 
+
 class ServiceObservabilityConfigurationTypeDef(
     _RequiredServiceObservabilityConfigurationTypeDef,
     _OptionalServiceObservabilityConfigurationTypeDef,
 ):
     pass
 
+
 VpcConnectorTypeDef = TypedDict(
     "VpcConnectorTypeDef",
     {
         "VpcConnectorName": str,
         "VpcConnectorArn": str,
         "VpcConnectorRevision": int,
         "Subnets": List[str],
@@ -471,20 +481,22 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class DescribeCustomDomainsRequestRequestTypeDef(
     _RequiredDescribeCustomDomainsRequestRequestTypeDef,
     _OptionalDescribeCustomDomainsRequestRequestTypeDef,
 ):
     pass
 
+
 DescribeObservabilityConfigurationRequestRequestTypeDef = TypedDict(
     "DescribeObservabilityConfigurationRequestRequestTypeDef",
     {
         "ObservabilityConfigurationArn": str,
     },
 )
 
@@ -609,19 +621,21 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListOperationsRequestRequestTypeDef(
     _RequiredListOperationsRequestRequestTypeDef, _OptionalListOperationsRequestRequestTypeDef
 ):
     pass
 
+
 OperationSummaryTypeDef = TypedDict(
     "OperationSummaryTypeDef",
     {
         "Id": str,
         "Type": OperationTypeType,
         "Status": OperationStatusType,
         "TargetArn": str,
@@ -771,55 +785,61 @@
     "_OptionalCustomDomainTypeDef",
     {
         "CertificateValidationRecords": List[CertificateValidationRecordTypeDef],
     },
     total=False,
 )
 
+
 class CustomDomainTypeDef(_RequiredCustomDomainTypeDef, _OptionalCustomDomainTypeDef):
     pass
 
+
 _RequiredCodeConfigurationOutputTypeDef = TypedDict(
     "_RequiredCodeConfigurationOutputTypeDef",
     {
         "ConfigurationSource": ConfigurationSourceType,
     },
 )
 _OptionalCodeConfigurationOutputTypeDef = TypedDict(
     "_OptionalCodeConfigurationOutputTypeDef",
     {
         "CodeConfigurationValues": CodeConfigurationValuesOutputTypeDef,
     },
     total=False,
 )
 
+
 class CodeConfigurationOutputTypeDef(
     _RequiredCodeConfigurationOutputTypeDef, _OptionalCodeConfigurationOutputTypeDef
 ):
     pass
 
+
 _RequiredCodeConfigurationTypeDef = TypedDict(
     "_RequiredCodeConfigurationTypeDef",
     {
         "ConfigurationSource": ConfigurationSourceType,
     },
 )
 _OptionalCodeConfigurationTypeDef = TypedDict(
     "_OptionalCodeConfigurationTypeDef",
     {
         "CodeConfigurationValues": CodeConfigurationValuesTypeDef,
     },
     total=False,
 )
 
+
 class CodeConfigurationTypeDef(
     _RequiredCodeConfigurationTypeDef, _OptionalCodeConfigurationTypeDef
 ):
     pass
 
+
 ListConnectionsResponseTypeDef = TypedDict(
     "ListConnectionsResponseTypeDef",
     {
         "ConnectionSummaryList": List[ConnectionSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -854,20 +874,22 @@
         "MinSize": int,
         "MaxSize": int,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateAutoScalingConfigurationRequestRequestTypeDef(
     _RequiredCreateAutoScalingConfigurationRequestRequestTypeDef,
     _OptionalCreateAutoScalingConfigurationRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateConnectionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateConnectionRequestRequestTypeDef",
     {
         "ConnectionName": str,
         "ProviderType": Literal["GITHUB"],
     },
 )
@@ -875,19 +897,21 @@
     "_OptionalCreateConnectionRequestRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateConnectionRequestRequestTypeDef(
     _RequiredCreateConnectionRequestRequestTypeDef, _OptionalCreateConnectionRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateVpcConnectorRequestRequestTypeDef = TypedDict(
     "_RequiredCreateVpcConnectorRequestRequestTypeDef",
     {
         "VpcConnectorName": str,
         "Subnets": Sequence[str],
     },
 )
@@ -896,20 +920,22 @@
     {
         "SecurityGroups": Sequence[str],
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateVpcConnectorRequestRequestTypeDef(
     _RequiredCreateVpcConnectorRequestRequestTypeDef,
     _OptionalCreateVpcConnectorRequestRequestTypeDef,
 ):
     pass
 
+
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -933,20 +959,22 @@
     {
         "TraceConfiguration": TraceConfigurationTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateObservabilityConfigurationRequestRequestTypeDef(
     _RequiredCreateObservabilityConfigurationRequestRequestTypeDef,
     _OptionalCreateObservabilityConfigurationRequestRequestTypeDef,
 ):
     pass
 
+
 ObservabilityConfigurationTypeDef = TypedDict(
     "ObservabilityConfigurationTypeDef",
     {
         "ObservabilityConfigurationArn": str,
         "ObservabilityConfigurationName": str,
         "TraceConfiguration": TraceConfigurationTypeDef,
         "ObservabilityConfigurationRevision": int,
@@ -1003,20 +1031,22 @@
     "_OptionalCreateVpcIngressConnectionRequestRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateVpcIngressConnectionRequestRequestTypeDef(
     _RequiredCreateVpcIngressConnectionRequestRequestTypeDef,
     _OptionalCreateVpcIngressConnectionRequestRequestTypeDef,
 ):
     pass
 
+
 UpdateVpcIngressConnectionRequestRequestTypeDef = TypedDict(
     "UpdateVpcIngressConnectionRequestRequestTypeDef",
     {
         "VpcIngressConnectionArn": str,
         "IngressVpcConfiguration": IngressVpcConfigurationTypeDef,
     },
 )
@@ -1048,19 +1078,21 @@
     "_OptionalImageRepositoryOutputTypeDef",
     {
         "ImageConfiguration": ImageConfigurationOutputTypeDef,
     },
     total=False,
 )
 
+
 class ImageRepositoryOutputTypeDef(
     _RequiredImageRepositoryOutputTypeDef, _OptionalImageRepositoryOutputTypeDef
 ):
     pass
 
+
 _RequiredImageRepositoryTypeDef = TypedDict(
     "_RequiredImageRepositoryTypeDef",
     {
         "ImageIdentifier": str,
         "ImageRepositoryType": ImageRepositoryTypeType,
     },
 )
@@ -1068,17 +1100,19 @@
     "_OptionalImageRepositoryTypeDef",
     {
         "ImageConfiguration": ImageConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class ImageRepositoryTypeDef(_RequiredImageRepositoryTypeDef, _OptionalImageRepositoryTypeDef):
     pass
 
+
 NetworkConfigurationTypeDef = TypedDict(
     "NetworkConfigurationTypeDef",
     {
         "EgressConfiguration": EgressConfigurationTypeDef,
         "IngressConfiguration": IngressConfigurationTypeDef,
     },
     total=False,
@@ -1175,19 +1209,21 @@
     "_OptionalCodeRepositoryOutputTypeDef",
     {
         "CodeConfiguration": CodeConfigurationOutputTypeDef,
     },
     total=False,
 )
 
+
 class CodeRepositoryOutputTypeDef(
     _RequiredCodeRepositoryOutputTypeDef, _OptionalCodeRepositoryOutputTypeDef
 ):
     pass
 
+
 _RequiredCodeRepositoryTypeDef = TypedDict(
     "_RequiredCodeRepositoryTypeDef",
     {
         "RepositoryUrl": str,
         "SourceCodeVersion": SourceCodeVersionTypeDef,
     },
 )
@@ -1195,17 +1231,19 @@
     "_OptionalCodeRepositoryTypeDef",
     {
         "CodeConfiguration": CodeConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class CodeRepositoryTypeDef(_RequiredCodeRepositoryTypeDef, _OptionalCodeRepositoryTypeDef):
     pass
 
+
 CreateObservabilityConfigurationResponseTypeDef = TypedDict(
     "CreateObservabilityConfigurationResponseTypeDef",
     {
         "ObservabilityConfiguration": ObservabilityConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1303,17 +1341,19 @@
         "EncryptionConfiguration": EncryptionConfigurationTypeDef,
         "HealthCheckConfiguration": HealthCheckConfigurationTypeDef,
         "ObservabilityConfiguration": ServiceObservabilityConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class ServiceTypeDef(_RequiredServiceTypeDef, _OptionalServiceTypeDef):
     pass
 
+
 _RequiredCreateServiceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateServiceRequestRequestTypeDef",
     {
         "ServiceName": str,
         "SourceConfiguration": SourceConfigurationTypeDef,
     },
 )
@@ -1327,19 +1367,24 @@
         "AutoScalingConfigurationArn": str,
         "NetworkConfiguration": NetworkConfigurationTypeDef,
         "ObservabilityConfiguration": ServiceObservabilityConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class CreateServiceRequestRequestTypeDef(
     _RequiredCreateServiceRequestRequestTypeDef, _OptionalCreateServiceRequestRequestTypeDef
 ):
     pass
 
+
+SourceConfigurationUnionTypeDef = Union[
+    SourceConfigurationTypeDef, SourceConfigurationOutputTypeDef
+]
 _RequiredUpdateServiceRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateServiceRequestRequestTypeDef",
     {
         "ServiceArn": str,
     },
 )
 _OptionalUpdateServiceRequestRequestTypeDef = TypedDict(
@@ -1351,19 +1396,21 @@
         "HealthCheckConfiguration": HealthCheckConfigurationTypeDef,
         "NetworkConfiguration": NetworkConfigurationTypeDef,
         "ObservabilityConfiguration": ServiceObservabilityConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class UpdateServiceRequestRequestTypeDef(
     _RequiredUpdateServiceRequestRequestTypeDef, _OptionalUpdateServiceRequestRequestTypeDef
 ):
     pass
 
+
 CreateServiceResponseTypeDef = TypedDict(
     "CreateServiceResponseTypeDef",
     {
         "Service": ServiceTypeDef,
         "OperationId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-apprunner-1.28.15.post1/mypy_boto3_apprunner.egg-info/PKG-INFO` & `mypy-boto3-apprunner-1.28.16/mypy_boto3_apprunner.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-apprunner
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.AppRunner 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.AppRunner 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apprunner/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 apprunner type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 apprunner type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-apprunner.svg?color=blue)](https://pypi.org/project/mypy-boto3-apprunner)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apprunner/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-apprunner)](https://pepy.tech/project/mypy-boto3-apprunner)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AppRunner 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apprunner.html#AppRunner)
+[boto3.AppRunner 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apprunner.html#AppRunner)
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
 [mypy-boto3-apprunner docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apprunner/).
 
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
@@ -304,20 +304,20 @@
 )
 
 
 def check_value(value: AutoScalingConfigurationStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_apprunner.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_apprunner.type_defs import (
     AssociateCustomDomainRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     VpcDNSTargetTypeDef,
     AuthenticationConfigurationTypeDef,
@@ -415,25 +415,26 @@
     DeleteVpcIngressConnectionResponseTypeDef,
     DescribeVpcIngressConnectionResponseTypeDef,
     UpdateVpcIngressConnectionResponseTypeDef,
     SourceConfigurationOutputTypeDef,
     SourceConfigurationTypeDef,
     ServiceTypeDef,
     CreateServiceRequestRequestTypeDef,
+    SourceConfigurationUnionTypeDef,
     UpdateServiceRequestRequestTypeDef,
     CreateServiceResponseTypeDef,
     DeleteServiceResponseTypeDef,
     DescribeServiceResponseTypeDef,
     PauseServiceResponseTypeDef,
     ResumeServiceResponseTypeDef,
     UpdateServiceResponseTypeDef,
 )
 
 
-def get_structure() -> AssociateCustomDomainRequestRequestTypeDef:
+def get_value() -> AssociateCustomDomainRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-apprunner-1.28.15.post1/mypy_boto3_apprunner.egg-info/SOURCES.txt` & `mypy-boto3-apprunner-1.28.16/mypy_boto3_apprunner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-apprunner-1.28.15.post1/setup.py` & `mypy-boto3-apprunner-1.28.16/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-apprunner",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_apprunner"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.AppRunner 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.2"
+        "Type annotations for boto3.AppRunner 1.28.16 service generated with mypy-boto3-builder"
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
-    keywords="boto3 apprunner type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 apprunner type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_apprunner": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apprunner/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

