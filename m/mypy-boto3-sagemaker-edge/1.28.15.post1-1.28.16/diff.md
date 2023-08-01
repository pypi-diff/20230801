# Comparing `tmp/mypy-boto3-sagemaker-edge-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-sagemaker-edge-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-sagemaker-edge-1.28.15.post1.tar", last modified: Sat Jul 29 10:04:05 2023, max compression
+gzip compressed data, was "mypy-boto3-sagemaker-edge-1.28.16.tar", last modified: Tue Aug  1 11:37:45 2023, max compression
```

## Comparing `mypy-boto3-sagemaker-edge-1.28.15.post1.tar` & `mypy-boto3-sagemaker-edge-1.28.16.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:05.549380 mypy-boto3-sagemaker-edge-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:58:32.000000 mypy-boto3-sagemaker-edge-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12746 2023-07-29 10:04:05.549380 mypy-boto3-sagemaker-edge-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11219 2023-07-29 09:58:32.000000 mypy-boto3-sagemaker-edge-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:05.545380 mypy-boto3-sagemaker-edge-1.28.15.post1/mypy_boto3_sagemaker_edge/
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-29 09:58:32.000000 mypy-boto3-sagemaker-edge-1.28.15.post1/mypy_boto3_sagemaker_edge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-29 09:58:32.000000 mypy-boto3-sagemaker-edge-1.28.15.post1/mypy_boto3_sagemaker_edge/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-29 09:58:32.000000 mypy-boto3-sagemaker-edge-1.28.15.post1/mypy_boto3_sagemaker_edge/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5153 2023-07-29 09:58:32.000000 mypy-boto3-sagemaker-edge-1.28.15.post1/mypy_boto3_sagemaker_edge/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5144 2023-07-29 09:58:32.000000 mypy-boto3-sagemaker-edge-1.28.15.post1/mypy_boto3_sagemaker_edge/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8149 2023-07-29 09:58:32.000000 mypy-boto3-sagemaker-edge-1.28.15.post1/mypy_boto3_sagemaker_edge/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8147 2023-07-29 09:58:32.000000 mypy-boto3-sagemaker-edge-1.28.15.post1/mypy_boto3_sagemaker_edge/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:58:32.000000 mypy-boto3-sagemaker-edge-1.28.15.post1/mypy_boto3_sagemaker_edge/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-07-29 09:58:32.000000 mypy-boto3-sagemaker-edge-1.28.15.post1/mypy_boto3_sagemaker_edge/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-07-29 09:58:32.000000 mypy-boto3-sagemaker-edge-1.28.15.post1/mypy_boto3_sagemaker_edge/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:58:32.000000 mypy-boto3-sagemaker-edge-1.28.15.post1/mypy_boto3_sagemaker_edge/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:05.549380 mypy-boto3-sagemaker-edge-1.28.15.post1/mypy_boto3_sagemaker_edge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12746 2023-07-29 10:04:05.000000 mypy-boto3-sagemaker-edge-1.28.15.post1/mypy_boto3_sagemaker_edge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-29 10:04:05.000000 mypy-boto3-sagemaker-edge-1.28.15.post1/mypy_boto3_sagemaker_edge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:05.000000 mypy-boto3-sagemaker-edge-1.28.15.post1/mypy_boto3_sagemaker_edge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:05.000000 mypy-boto3-sagemaker-edge-1.28.15.post1/mypy_boto3_sagemaker_edge.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:04:05.000000 mypy-boto3-sagemaker-edge-1.28.15.post1/mypy_boto3_sagemaker_edge.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-29 10:04:05.000000 mypy-boto3-sagemaker-edge-1.28.15.post1/mypy_boto3_sagemaker_edge.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:04:05.549380 mypy-boto3-sagemaker-edge-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-07-29 09:58:32.000000 mypy-boto3-sagemaker-edge-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:45.148755 mypy-boto3-sagemaker-edge-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:31:59.000000 mypy-boto3-sagemaker-edge-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12758 2023-08-01 11:37:45.144755 mypy-boto3-sagemaker-edge-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11240 2023-08-01 11:31:59.000000 mypy-boto3-sagemaker-edge-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:45.136755 mypy-boto3-sagemaker-edge-1.28.16/mypy_boto3_sagemaker_edge/
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-08-01 11:31:59.000000 mypy-boto3-sagemaker-edge-1.28.16/mypy_boto3_sagemaker_edge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-08-01 11:31:59.000000 mypy-boto3-sagemaker-edge-1.28.16/mypy_boto3_sagemaker_edge/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-08-01 11:31:59.000000 mypy-boto3-sagemaker-edge-1.28.16/mypy_boto3_sagemaker_edge/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5153 2023-08-01 11:31:59.000000 mypy-boto3-sagemaker-edge-1.28.16/mypy_boto3_sagemaker_edge/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5144 2023-08-01 11:31:59.000000 mypy-boto3-sagemaker-edge-1.28.16/mypy_boto3_sagemaker_edge/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8149 2023-08-01 11:31:59.000000 mypy-boto3-sagemaker-edge-1.28.16/mypy_boto3_sagemaker_edge/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8147 2023-08-01 11:31:59.000000 mypy-boto3-sagemaker-edge-1.28.16/mypy_boto3_sagemaker_edge/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:31:59.000000 mypy-boto3-sagemaker-edge-1.28.16/mypy_boto3_sagemaker_edge/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-08-01 11:31:59.000000 mypy-boto3-sagemaker-edge-1.28.16/mypy_boto3_sagemaker_edge/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4864 2023-08-01 11:31:59.000000 mypy-boto3-sagemaker-edge-1.28.16/mypy_boto3_sagemaker_edge/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:31:59.000000 mypy-boto3-sagemaker-edge-1.28.16/mypy_boto3_sagemaker_edge/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:45.144755 mypy-boto3-sagemaker-edge-1.28.16/mypy_boto3_sagemaker_edge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12758 2023-08-01 11:37:44.000000 mypy-boto3-sagemaker-edge-1.28.16/mypy_boto3_sagemaker_edge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-08-01 11:37:44.000000 mypy-boto3-sagemaker-edge-1.28.16/mypy_boto3_sagemaker_edge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:44.000000 mypy-boto3-sagemaker-edge-1.28.16/mypy_boto3_sagemaker_edge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:44.000000 mypy-boto3-sagemaker-edge-1.28.16/mypy_boto3_sagemaker_edge.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:44.000000 mypy-boto3-sagemaker-edge-1.28.16/mypy_boto3_sagemaker_edge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-01 11:37:44.000000 mypy-boto3-sagemaker-edge-1.28.16/mypy_boto3_sagemaker_edge.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:45.148755 mypy-boto3-sagemaker-edge-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-08-01 11:31:59.000000 mypy-boto3-sagemaker-edge-1.28.16/setup.py
```

### Comparing `mypy-boto3-sagemaker-edge-1.28.15.post1/LICENSE` & `mypy-boto3-sagemaker-edge-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-edge-1.28.15.post1/PKG-INFO` & `mypy-boto3-sagemaker-edge-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sagemaker-edge
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.SagemakerEdgeManager 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.SagemakerEdgeManager 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_edge/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 sagemaker-edge type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 sagemaker-edge type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sagemaker-edge.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker-edge)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_edge/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sagemaker-edge)](https://pepy.tech/project/mypy-boto3-sagemaker-edge)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SagemakerEdgeManager 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-edge.html#SagemakerEdgeManager)
+[boto3.SagemakerEdgeManager 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-edge.html#SagemakerEdgeManager)
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
 [mypy-boto3-sagemaker-edge docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_edge/).
 
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
@@ -293,41 +293,42 @@
 )
 
 
 def check_value(value: ChecksumTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_sagemaker_edge.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_sagemaker_edge.type_defs import (
     ChecksumTypeDef,
     DeploymentModelTypeDef,
-    EdgeMetricTypeDef,
+    TimestampTypeDef,
     ResponseMetadataTypeDef,
     GetDeploymentsRequestRequestTypeDef,
     GetDeviceRegistrationRequestRequestTypeDef,
     DefinitionTypeDef,
     DeploymentResultTypeDef,
-    ModelTypeDef,
+    EdgeMetricTypeDef,
     EmptyResponseMetadataTypeDef,
     GetDeviceRegistrationResultTypeDef,
     EdgeDeploymentTypeDef,
-    SendHeartbeatRequestRequestTypeDef,
+    ModelTypeDef,
     GetDeploymentsResultTypeDef,
+    SendHeartbeatRequestRequestTypeDef,
 )
 
 
-def get_structure() -> ChecksumTypeDef:
+def get_value() -> ChecksumTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-sagemaker-edge-1.28.15.post1/README.md` & `mypy-boto3-sagemaker-edge-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sagemaker-edge.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker-edge)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_edge/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sagemaker-edge)](https://pepy.tech/project/mypy-boto3-sagemaker-edge)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SagemakerEdgeManager 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-edge.html#SagemakerEdgeManager)
+[boto3.SagemakerEdgeManager 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-edge.html#SagemakerEdgeManager)
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
 [mypy-boto3-sagemaker-edge docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_edge/).
 
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
@@ -261,41 +261,42 @@
 )
 
 
 def check_value(value: ChecksumTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_sagemaker_edge.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_sagemaker_edge.type_defs import (
     ChecksumTypeDef,
     DeploymentModelTypeDef,
-    EdgeMetricTypeDef,
+    TimestampTypeDef,
     ResponseMetadataTypeDef,
     GetDeploymentsRequestRequestTypeDef,
     GetDeviceRegistrationRequestRequestTypeDef,
     DefinitionTypeDef,
     DeploymentResultTypeDef,
-    ModelTypeDef,
+    EdgeMetricTypeDef,
     EmptyResponseMetadataTypeDef,
     GetDeviceRegistrationResultTypeDef,
     EdgeDeploymentTypeDef,
-    SendHeartbeatRequestRequestTypeDef,
+    ModelTypeDef,
     GetDeploymentsResultTypeDef,
+    SendHeartbeatRequestRequestTypeDef,
 )
 
 
-def get_structure() -> ChecksumTypeDef:
+def get_value() -> ChecksumTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-sagemaker-edge-1.28.15.post1/mypy_boto3_sagemaker_edge/__main__.py` & `mypy-boto3-sagemaker-edge-1.28.16/mypy_boto3_sagemaker_edge/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SagemakerEdgeManager 1.28.15\nVersion:        "
-        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.SagemakerEdgeManager 1.28.16\nVersion:         1.28.16\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_edge//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-edge.html#SagemakerEdgeManager\nOther"
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

### Comparing `mypy-boto3-sagemaker-edge-1.28.15.post1/mypy_boto3_sagemaker_edge/client.py` & `mypy-boto3-sagemaker-edge-1.28.16/mypy_boto3_sagemaker_edge/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-edge-1.28.15.post1/mypy_boto3_sagemaker_edge/client.pyi` & `mypy-boto3-sagemaker-edge-1.28.16/mypy_boto3_sagemaker_edge/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-edge-1.28.15.post1/mypy_boto3_sagemaker_edge/literals.py` & `mypy-boto3-sagemaker-edge-1.28.16/mypy_boto3_sagemaker_edge/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-edge-1.28.15.post1/mypy_boto3_sagemaker_edge/literals.pyi` & `mypy-boto3-sagemaker-edge-1.28.16/mypy_boto3_sagemaker_edge/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-edge-1.28.15.post1/mypy_boto3_sagemaker_edge/type_defs.py` & `mypy-boto3-sagemaker-edge-1.28.16/mypy_boto3_sagemaker_edge/type_defs.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_edge/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_sagemaker_edge.type_defs import ChecksumTypeDef
 
-    data: ChecksumTypeDef = {...}
+    data: ChecksumTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import DeploymentStatusType, FailureHandlingPolicyType, ModelStateType
@@ -26,26 +26,27 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "ChecksumTypeDef",
     "DeploymentModelTypeDef",
-    "EdgeMetricTypeDef",
+    "TimestampTypeDef",
     "ResponseMetadataTypeDef",
     "GetDeploymentsRequestRequestTypeDef",
     "GetDeviceRegistrationRequestRequestTypeDef",
     "DefinitionTypeDef",
     "DeploymentResultTypeDef",
-    "ModelTypeDef",
+    "EdgeMetricTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetDeviceRegistrationResultTypeDef",
     "EdgeDeploymentTypeDef",
-    "SendHeartbeatRequestRequestTypeDef",
+    "ModelTypeDef",
     "GetDeploymentsResultTypeDef",
+    "SendHeartbeatRequestRequestTypeDef",
 )
 
 ChecksumTypeDef = TypedDict(
     "ChecksumTypeDef",
     {
         "Type": Literal["SHA1"],
         "Sum": str,
@@ -64,25 +65,15 @@
         "Status": DeploymentStatusType,
         "StatusReason": str,
         "RollbackFailureReason": str,
     },
     total=False,
 )
 
-EdgeMetricTypeDef = TypedDict(
-    "EdgeMetricTypeDef",
-    {
-        "Dimension": str,
-        "MetricName": str,
-        "Value": float,
-        "Timestamp": Union[datetime, str],
-    },
-    total=False,
-)
-
+TimestampTypeDef = Union[datetime, str]
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -119,29 +110,28 @@
 
 DeploymentResultTypeDef = TypedDict(
     "DeploymentResultTypeDef",
     {
         "DeploymentName": str,
         "DeploymentStatus": str,
         "DeploymentStatusMessage": str,
-        "DeploymentStartTime": Union[datetime, str],
-        "DeploymentEndTime": Union[datetime, str],
+        "DeploymentStartTime": TimestampTypeDef,
+        "DeploymentEndTime": TimestampTypeDef,
         "DeploymentModels": Sequence[DeploymentModelTypeDef],
     },
     total=False,
 )
 
-ModelTypeDef = TypedDict(
-    "ModelTypeDef",
+EdgeMetricTypeDef = TypedDict(
+    "EdgeMetricTypeDef",
     {
-        "ModelName": str,
-        "ModelVersion": str,
-        "LatestSampleTime": Union[datetime, str],
-        "LatestInference": Union[datetime, str],
-        "ModelMetrics": Sequence[EdgeMetricTypeDef],
+        "Dimension": str,
+        "MetricName": str,
+        "Value": float,
+        "Timestamp": TimestampTypeDef,
     },
     total=False,
 )
 
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
@@ -165,14 +155,34 @@
         "Type": Literal["Model"],
         "FailureHandlingPolicy": FailureHandlingPolicyType,
         "Definitions": List[DefinitionTypeDef],
     },
     total=False,
 )
 
+ModelTypeDef = TypedDict(
+    "ModelTypeDef",
+    {
+        "ModelName": str,
+        "ModelVersion": str,
+        "LatestSampleTime": TimestampTypeDef,
+        "LatestInference": TimestampTypeDef,
+        "ModelMetrics": Sequence[EdgeMetricTypeDef],
+    },
+    total=False,
+)
+
+GetDeploymentsResultTypeDef = TypedDict(
+    "GetDeploymentsResultTypeDef",
+    {
+        "Deployments": List[EdgeDeploymentTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredSendHeartbeatRequestRequestTypeDef = TypedDict(
     "_RequiredSendHeartbeatRequestRequestTypeDef",
     {
         "AgentVersion": str,
         "DeviceName": str,
         "DeviceFleetName": str,
     },
@@ -188,16 +198,7 @@
 )
 
 
 class SendHeartbeatRequestRequestTypeDef(
     _RequiredSendHeartbeatRequestRequestTypeDef, _OptionalSendHeartbeatRequestRequestTypeDef
 ):
     pass
-
-
-GetDeploymentsResultTypeDef = TypedDict(
-    "GetDeploymentsResultTypeDef",
-    {
-        "Deployments": List[EdgeDeploymentTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
```

### Comparing `mypy-boto3-sagemaker-edge-1.28.15.post1/mypy_boto3_sagemaker_edge/type_defs.pyi` & `mypy-boto3-sagemaker-edge-1.28.16/mypy_boto3_sagemaker_edge/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_edge/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_sagemaker_edge.type_defs import ChecksumTypeDef
 
-    data: ChecksumTypeDef = {...}
+    data: ChecksumTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import DeploymentStatusType, FailureHandlingPolicyType, ModelStateType
@@ -25,26 +25,27 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "ChecksumTypeDef",
     "DeploymentModelTypeDef",
-    "EdgeMetricTypeDef",
+    "TimestampTypeDef",
     "ResponseMetadataTypeDef",
     "GetDeploymentsRequestRequestTypeDef",
     "GetDeviceRegistrationRequestRequestTypeDef",
     "DefinitionTypeDef",
     "DeploymentResultTypeDef",
-    "ModelTypeDef",
+    "EdgeMetricTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetDeviceRegistrationResultTypeDef",
     "EdgeDeploymentTypeDef",
-    "SendHeartbeatRequestRequestTypeDef",
+    "ModelTypeDef",
     "GetDeploymentsResultTypeDef",
+    "SendHeartbeatRequestRequestTypeDef",
 )
 
 ChecksumTypeDef = TypedDict(
     "ChecksumTypeDef",
     {
         "Type": Literal["SHA1"],
         "Sum": str,
@@ -63,25 +64,15 @@
         "Status": DeploymentStatusType,
         "StatusReason": str,
         "RollbackFailureReason": str,
     },
     total=False,
 )
 
-EdgeMetricTypeDef = TypedDict(
-    "EdgeMetricTypeDef",
-    {
-        "Dimension": str,
-        "MetricName": str,
-        "Value": float,
-        "Timestamp": Union[datetime, str],
-    },
-    total=False,
-)
-
+TimestampTypeDef = Union[datetime, str]
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -118,29 +109,28 @@
 
 DeploymentResultTypeDef = TypedDict(
     "DeploymentResultTypeDef",
     {
         "DeploymentName": str,
         "DeploymentStatus": str,
         "DeploymentStatusMessage": str,
-        "DeploymentStartTime": Union[datetime, str],
-        "DeploymentEndTime": Union[datetime, str],
+        "DeploymentStartTime": TimestampTypeDef,
+        "DeploymentEndTime": TimestampTypeDef,
         "DeploymentModels": Sequence[DeploymentModelTypeDef],
     },
     total=False,
 )
 
-ModelTypeDef = TypedDict(
-    "ModelTypeDef",
+EdgeMetricTypeDef = TypedDict(
+    "EdgeMetricTypeDef",
     {
-        "ModelName": str,
-        "ModelVersion": str,
-        "LatestSampleTime": Union[datetime, str],
-        "LatestInference": Union[datetime, str],
-        "ModelMetrics": Sequence[EdgeMetricTypeDef],
+        "Dimension": str,
+        "MetricName": str,
+        "Value": float,
+        "Timestamp": TimestampTypeDef,
     },
     total=False,
 )
 
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
@@ -164,14 +154,34 @@
         "Type": Literal["Model"],
         "FailureHandlingPolicy": FailureHandlingPolicyType,
         "Definitions": List[DefinitionTypeDef],
     },
     total=False,
 )
 
+ModelTypeDef = TypedDict(
+    "ModelTypeDef",
+    {
+        "ModelName": str,
+        "ModelVersion": str,
+        "LatestSampleTime": TimestampTypeDef,
+        "LatestInference": TimestampTypeDef,
+        "ModelMetrics": Sequence[EdgeMetricTypeDef],
+    },
+    total=False,
+)
+
+GetDeploymentsResultTypeDef = TypedDict(
+    "GetDeploymentsResultTypeDef",
+    {
+        "Deployments": List[EdgeDeploymentTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredSendHeartbeatRequestRequestTypeDef = TypedDict(
     "_RequiredSendHeartbeatRequestRequestTypeDef",
     {
         "AgentVersion": str,
         "DeviceName": str,
         "DeviceFleetName": str,
     },
@@ -186,15 +196,7 @@
     total=False,
 )
 
 class SendHeartbeatRequestRequestTypeDef(
     _RequiredSendHeartbeatRequestRequestTypeDef, _OptionalSendHeartbeatRequestRequestTypeDef
 ):
     pass
-
-GetDeploymentsResultTypeDef = TypedDict(
-    "GetDeploymentsResultTypeDef",
-    {
-        "Deployments": List[EdgeDeploymentTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
```

### Comparing `mypy-boto3-sagemaker-edge-1.28.15.post1/mypy_boto3_sagemaker_edge.egg-info/PKG-INFO` & `mypy-boto3-sagemaker-edge-1.28.16/mypy_boto3_sagemaker_edge.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sagemaker-edge
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.SagemakerEdgeManager 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.SagemakerEdgeManager 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_edge/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 sagemaker-edge type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 sagemaker-edge type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sagemaker-edge.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker-edge)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_edge/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sagemaker-edge)](https://pepy.tech/project/mypy-boto3-sagemaker-edge)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SagemakerEdgeManager 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-edge.html#SagemakerEdgeManager)
+[boto3.SagemakerEdgeManager 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-edge.html#SagemakerEdgeManager)
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
 [mypy-boto3-sagemaker-edge docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_edge/).
 
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
@@ -293,41 +293,42 @@
 )
 
 
 def check_value(value: ChecksumTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_sagemaker_edge.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_sagemaker_edge.type_defs import (
     ChecksumTypeDef,
     DeploymentModelTypeDef,
-    EdgeMetricTypeDef,
+    TimestampTypeDef,
     ResponseMetadataTypeDef,
     GetDeploymentsRequestRequestTypeDef,
     GetDeviceRegistrationRequestRequestTypeDef,
     DefinitionTypeDef,
     DeploymentResultTypeDef,
-    ModelTypeDef,
+    EdgeMetricTypeDef,
     EmptyResponseMetadataTypeDef,
     GetDeviceRegistrationResultTypeDef,
     EdgeDeploymentTypeDef,
-    SendHeartbeatRequestRequestTypeDef,
+    ModelTypeDef,
     GetDeploymentsResultTypeDef,
+    SendHeartbeatRequestRequestTypeDef,
 )
 
 
-def get_structure() -> ChecksumTypeDef:
+def get_value() -> ChecksumTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-sagemaker-edge-1.28.15.post1/mypy_boto3_sagemaker_edge.egg-info/SOURCES.txt` & `mypy-boto3-sagemaker-edge-1.28.16/mypy_boto3_sagemaker_edge.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-edge-1.28.15.post1/setup.py` & `mypy-boto3-sagemaker-edge-1.28.16/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-sagemaker-edge",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_sagemaker_edge"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.SagemakerEdgeManager 1.28.15 service generated with"
-        " mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.SagemakerEdgeManager 1.28.16 service generated with"
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
-    keywords="boto3 sagemaker-edge type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 sagemaker-edge type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_sagemaker_edge": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_edge/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

