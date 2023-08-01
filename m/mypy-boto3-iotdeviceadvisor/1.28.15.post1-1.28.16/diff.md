# Comparing `tmp/mypy-boto3-iotdeviceadvisor-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-iotdeviceadvisor-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-iotdeviceadvisor-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:20 2023, max compression
+gzip compressed data, was "mypy-boto3-iotdeviceadvisor-1.28.16.tar", last modified: Tue Aug  1 11:37:00 2023, max compression
```

## Comparing `mypy-boto3-iotdeviceadvisor-1.28.15.post1.tar` & `mypy-boto3-iotdeviceadvisor-1.28.16.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:20.173183 mypy-boto3-iotdeviceadvisor-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:47:52.000000 mypy-boto3-iotdeviceadvisor-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13766 2023-07-29 10:03:20.173183 mypy-boto3-iotdeviceadvisor-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12237 2023-07-29 09:47:52.000000 mypy-boto3-iotdeviceadvisor-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:20.173183 mypy-boto3-iotdeviceadvisor-1.28.15.post1/mypy_boto3_iotdeviceadvisor/
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-29 09:47:52.000000 mypy-boto3-iotdeviceadvisor-1.28.15.post1/mypy_boto3_iotdeviceadvisor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-29 09:47:52.000000 mypy-boto3-iotdeviceadvisor-1.28.15.post1/mypy_boto3_iotdeviceadvisor/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-29 09:47:52.000000 mypy-boto3-iotdeviceadvisor-1.28.15.post1/mypy_boto3_iotdeviceadvisor/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11906 2023-07-29 09:47:52.000000 mypy-boto3-iotdeviceadvisor-1.28.15.post1/mypy_boto3_iotdeviceadvisor/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11886 2023-07-29 09:47:52.000000 mypy-boto3-iotdeviceadvisor-1.28.15.post1/mypy_boto3_iotdeviceadvisor/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8681 2023-07-29 09:47:52.000000 mypy-boto3-iotdeviceadvisor-1.28.15.post1/mypy_boto3_iotdeviceadvisor/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8679 2023-07-29 09:47:52.000000 mypy-boto3-iotdeviceadvisor-1.28.15.post1/mypy_boto3_iotdeviceadvisor/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:47:52.000000 mypy-boto3-iotdeviceadvisor-1.28.15.post1/mypy_boto3_iotdeviceadvisor/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    13637 2023-07-29 09:47:53.000000 mypy-boto3-iotdeviceadvisor-1.28.15.post1/mypy_boto3_iotdeviceadvisor/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    13622 2023-07-29 09:47:53.000000 mypy-boto3-iotdeviceadvisor-1.28.15.post1/mypy_boto3_iotdeviceadvisor/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:47:52.000000 mypy-boto3-iotdeviceadvisor-1.28.15.post1/mypy_boto3_iotdeviceadvisor/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:20.173183 mypy-boto3-iotdeviceadvisor-1.28.15.post1/mypy_boto3_iotdeviceadvisor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13766 2023-07-29 10:03:19.000000 mypy-boto3-iotdeviceadvisor-1.28.15.post1/mypy_boto3_iotdeviceadvisor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-29 10:03:19.000000 mypy-boto3-iotdeviceadvisor-1.28.15.post1/mypy_boto3_iotdeviceadvisor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:19.000000 mypy-boto3-iotdeviceadvisor-1.28.15.post1/mypy_boto3_iotdeviceadvisor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:19.000000 mypy-boto3-iotdeviceadvisor-1.28.15.post1/mypy_boto3_iotdeviceadvisor.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:19.000000 mypy-boto3-iotdeviceadvisor-1.28.15.post1/mypy_boto3_iotdeviceadvisor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-29 10:03:19.000000 mypy-boto3-iotdeviceadvisor-1.28.15.post1/mypy_boto3_iotdeviceadvisor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:20.197183 mypy-boto3-iotdeviceadvisor-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-07-29 09:47:52.000000 mypy-boto3-iotdeviceadvisor-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:00.024865 mypy-boto3-iotdeviceadvisor-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:20:34.000000 mypy-boto3-iotdeviceadvisor-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13841 2023-08-01 11:37:00.024865 mypy-boto3-iotdeviceadvisor-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12321 2023-08-01 11:20:34.000000 mypy-boto3-iotdeviceadvisor-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:00.008865 mypy-boto3-iotdeviceadvisor-1.28.16/mypy_boto3_iotdeviceadvisor/
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-08-01 11:20:35.000000 mypy-boto3-iotdeviceadvisor-1.28.16/mypy_boto3_iotdeviceadvisor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-08-01 11:20:35.000000 mypy-boto3-iotdeviceadvisor-1.28.16/mypy_boto3_iotdeviceadvisor/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-08-01 11:20:35.000000 mypy-boto3-iotdeviceadvisor-1.28.16/mypy_boto3_iotdeviceadvisor/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11628 2023-08-01 11:20:35.000000 mypy-boto3-iotdeviceadvisor-1.28.16/mypy_boto3_iotdeviceadvisor/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11608 2023-08-01 11:20:35.000000 mypy-boto3-iotdeviceadvisor-1.28.16/mypy_boto3_iotdeviceadvisor/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8681 2023-08-01 11:20:35.000000 mypy-boto3-iotdeviceadvisor-1.28.16/mypy_boto3_iotdeviceadvisor/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8679 2023-08-01 11:20:35.000000 mypy-boto3-iotdeviceadvisor-1.28.16/mypy_boto3_iotdeviceadvisor/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:20:35.000000 mypy-boto3-iotdeviceadvisor-1.28.16/mypy_boto3_iotdeviceadvisor/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    13980 2023-08-01 11:20:35.000000 mypy-boto3-iotdeviceadvisor-1.28.16/mypy_boto3_iotdeviceadvisor/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13965 2023-08-01 11:20:35.000000 mypy-boto3-iotdeviceadvisor-1.28.16/mypy_boto3_iotdeviceadvisor/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:20:34.000000 mypy-boto3-iotdeviceadvisor-1.28.16/mypy_boto3_iotdeviceadvisor/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:00.024865 mypy-boto3-iotdeviceadvisor-1.28.16/mypy_boto3_iotdeviceadvisor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13841 2023-08-01 11:36:59.000000 mypy-boto3-iotdeviceadvisor-1.28.16/mypy_boto3_iotdeviceadvisor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-08-01 11:36:59.000000 mypy-boto3-iotdeviceadvisor-1.28.16/mypy_boto3_iotdeviceadvisor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:59.000000 mypy-boto3-iotdeviceadvisor-1.28.16/mypy_boto3_iotdeviceadvisor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:59.000000 mypy-boto3-iotdeviceadvisor-1.28.16/mypy_boto3_iotdeviceadvisor.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:59.000000 mypy-boto3-iotdeviceadvisor-1.28.16/mypy_boto3_iotdeviceadvisor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-01 11:36:59.000000 mypy-boto3-iotdeviceadvisor-1.28.16/mypy_boto3_iotdeviceadvisor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:00.024865 mypy-boto3-iotdeviceadvisor-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-08-01 11:20:34.000000 mypy-boto3-iotdeviceadvisor-1.28.16/setup.py
```

### Comparing `mypy-boto3-iotdeviceadvisor-1.28.15.post1/LICENSE` & `mypy-boto3-iotdeviceadvisor-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotdeviceadvisor-1.28.15.post1/PKG-INFO` & `mypy-boto3-iotdeviceadvisor-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iotdeviceadvisor
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.IoTDeviceAdvisor 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.IoTDeviceAdvisor 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotdeviceadvisor/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 iotdeviceadvisor type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 iotdeviceadvisor type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotdeviceadvisor.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotdeviceadvisor)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotdeviceadvisor/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iotdeviceadvisor)](https://pepy.tech/project/mypy-boto3-iotdeviceadvisor)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTDeviceAdvisor 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor)
+[boto3.IoTDeviceAdvisor 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor)
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
 [mypy-boto3-iotdeviceadvisor docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotdeviceadvisor/).
 
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
@@ -294,20 +294,20 @@
 )
 
 
 def check_value(value: AuthenticationMethodType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_iotdeviceadvisor.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_iotdeviceadvisor.type_defs import (
     ResponseMetadataTypeDef,
     DeleteSuiteDefinitionRequestRequestTypeDef,
     DeviceUnderTestTypeDef,
     GetEndpointRequestRequestTypeDef,
@@ -333,24 +333,26 @@
     SuiteDefinitionInformationTypeDef,
     SuiteRunConfigurationOutputTypeDef,
     SuiteRunConfigurationTypeDef,
     ListSuiteRunsResponseTypeDef,
     TestCaseRunTypeDef,
     GetSuiteDefinitionResponseTypeDef,
     CreateSuiteDefinitionRequestRequestTypeDef,
+    SuiteDefinitionConfigurationUnionTypeDef,
     UpdateSuiteDefinitionRequestRequestTypeDef,
     ListSuiteDefinitionsResponseTypeDef,
     StartSuiteRunRequestRequestTypeDef,
+    SuiteRunConfigurationUnionTypeDef,
     GroupResultTypeDef,
     TestResultTypeDef,
     GetSuiteRunResponseTypeDef,
 )
 
 
-def get_structure() -> ResponseMetadataTypeDef:
+def get_value() -> ResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-iotdeviceadvisor-1.28.15.post1/README.md` & `mypy-boto3-iotdeviceadvisor-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotdeviceadvisor.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotdeviceadvisor)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotdeviceadvisor/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iotdeviceadvisor)](https://pepy.tech/project/mypy-boto3-iotdeviceadvisor)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTDeviceAdvisor 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor)
+[boto3.IoTDeviceAdvisor 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor)
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
 [mypy-boto3-iotdeviceadvisor docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotdeviceadvisor/).
 
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
@@ -262,20 +262,20 @@
 )
 
 
 def check_value(value: AuthenticationMethodType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_iotdeviceadvisor.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_iotdeviceadvisor.type_defs import (
     ResponseMetadataTypeDef,
     DeleteSuiteDefinitionRequestRequestTypeDef,
     DeviceUnderTestTypeDef,
     GetEndpointRequestRequestTypeDef,
@@ -301,24 +301,26 @@
     SuiteDefinitionInformationTypeDef,
     SuiteRunConfigurationOutputTypeDef,
     SuiteRunConfigurationTypeDef,
     ListSuiteRunsResponseTypeDef,
     TestCaseRunTypeDef,
     GetSuiteDefinitionResponseTypeDef,
     CreateSuiteDefinitionRequestRequestTypeDef,
+    SuiteDefinitionConfigurationUnionTypeDef,
     UpdateSuiteDefinitionRequestRequestTypeDef,
     ListSuiteDefinitionsResponseTypeDef,
     StartSuiteRunRequestRequestTypeDef,
+    SuiteRunConfigurationUnionTypeDef,
     GroupResultTypeDef,
     TestResultTypeDef,
     GetSuiteRunResponseTypeDef,
 )
 
 
-def get_structure() -> ResponseMetadataTypeDef:
+def get_value() -> ResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-iotdeviceadvisor-1.28.15.post1/mypy_boto3_iotdeviceadvisor/__main__.py` & `mypy-boto3-iotdeviceadvisor-1.28.16/mypy_boto3_iotdeviceadvisor/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.IoTDeviceAdvisor 1.28.15\nVersion:        "
-        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.IoTDeviceAdvisor 1.28.16\nVersion:         1.28.16\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotdeviceadvisor//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor\nOther"
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

### Comparing `mypy-boto3-iotdeviceadvisor-1.28.15.post1/mypy_boto3_iotdeviceadvisor/client.py` & `mypy-boto3-iotdeviceadvisor-1.28.16/mypy_boto3_iotdeviceadvisor/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,33 +9,31 @@
     from boto3.session import Session
     from mypy_boto3_iotdeviceadvisor.client import IoTDeviceAdvisorClient
 
     session = Session()
     client: IoTDeviceAdvisorClient = session.client("iotdeviceadvisor")
     ```
 """
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import AuthenticationMethodType
 from .type_defs import (
     CreateSuiteDefinitionResponseTypeDef,
     GetEndpointResponseTypeDef,
     GetSuiteDefinitionResponseTypeDef,
     GetSuiteRunReportResponseTypeDef,
     GetSuiteRunResponseTypeDef,
     ListSuiteDefinitionsResponseTypeDef,
     ListSuiteRunsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     StartSuiteRunResponseTypeDef,
-    SuiteDefinitionConfigurationOutputTypeDef,
-    SuiteDefinitionConfigurationTypeDef,
-    SuiteRunConfigurationOutputTypeDef,
-    SuiteRunConfigurationTypeDef,
+    SuiteDefinitionConfigurationUnionTypeDef,
+    SuiteRunConfigurationUnionTypeDef,
     UpdateSuiteDefinitionResponseTypeDef,
 )
 
 __all__ = ("IoTDeviceAdvisorClient",)
 
 
 class BotocoreClientError(BaseException):
@@ -86,17 +84,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotdeviceadvisor/client/#close)
         """
 
     def create_suite_definition(
         self,
         *,
-        suiteDefinitionConfiguration: Union[
-            SuiteDefinitionConfigurationTypeDef, SuiteDefinitionConfigurationOutputTypeDef
-        ],
+        suiteDefinitionConfiguration: SuiteDefinitionConfigurationUnionTypeDef,
         tags: Mapping[str, str] = ...
     ) -> CreateSuiteDefinitionResponseTypeDef:
         """
         Creates a Device Advisor test suite.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor.Client.create_suite_definition)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotdeviceadvisor/client/#create_suite_definition)
@@ -203,17 +199,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotdeviceadvisor/client/#list_tags_for_resource)
         """
 
     def start_suite_run(
         self,
         *,
         suiteDefinitionId: str,
-        suiteRunConfiguration: Union[
-            SuiteRunConfigurationTypeDef, SuiteRunConfigurationOutputTypeDef
-        ],
+        suiteRunConfiguration: SuiteRunConfigurationUnionTypeDef,
         suiteDefinitionVersion: str = ...,
         tags: Mapping[str, str] = ...
     ) -> StartSuiteRunResponseTypeDef:
         """
         Starts a Device Advisor test suite run.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor.Client.start_suite_run)
@@ -244,17 +238,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotdeviceadvisor/client/#untag_resource)
         """
 
     def update_suite_definition(
         self,
         *,
         suiteDefinitionId: str,
-        suiteDefinitionConfiguration: Union[
-            SuiteDefinitionConfigurationTypeDef, SuiteDefinitionConfigurationOutputTypeDef
-        ]
+        suiteDefinitionConfiguration: SuiteDefinitionConfigurationUnionTypeDef
     ) -> UpdateSuiteDefinitionResponseTypeDef:
         """
         Updates a Device Advisor test suite.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor.Client.update_suite_definition)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotdeviceadvisor/client/#update_suite_definition)
         """
```

### Comparing `mypy-boto3-iotdeviceadvisor-1.28.15.post1/mypy_boto3_iotdeviceadvisor/client.pyi` & `mypy-boto3-iotdeviceadvisor-1.28.16/mypy_boto3_iotdeviceadvisor/client.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -9,33 +9,31 @@
     from boto3.session import Session
     from mypy_boto3_iotdeviceadvisor.client import IoTDeviceAdvisorClient
 
     session = Session()
     client: IoTDeviceAdvisorClient = session.client("iotdeviceadvisor")
     ```
 """
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import AuthenticationMethodType
 from .type_defs import (
     CreateSuiteDefinitionResponseTypeDef,
     GetEndpointResponseTypeDef,
     GetSuiteDefinitionResponseTypeDef,
     GetSuiteRunReportResponseTypeDef,
     GetSuiteRunResponseTypeDef,
     ListSuiteDefinitionsResponseTypeDef,
     ListSuiteRunsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     StartSuiteRunResponseTypeDef,
-    SuiteDefinitionConfigurationOutputTypeDef,
-    SuiteDefinitionConfigurationTypeDef,
-    SuiteRunConfigurationOutputTypeDef,
-    SuiteRunConfigurationTypeDef,
+    SuiteDefinitionConfigurationUnionTypeDef,
+    SuiteRunConfigurationUnionTypeDef,
     UpdateSuiteDefinitionResponseTypeDef,
 )
 
 __all__ = ("IoTDeviceAdvisorClient",)
 
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
@@ -80,17 +78,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotdeviceadvisor/client/#close)
         """
     def create_suite_definition(
         self,
         *,
-        suiteDefinitionConfiguration: Union[
-            SuiteDefinitionConfigurationTypeDef, SuiteDefinitionConfigurationOutputTypeDef
-        ],
+        suiteDefinitionConfiguration: SuiteDefinitionConfigurationUnionTypeDef,
         tags: Mapping[str, str] = ...
     ) -> CreateSuiteDefinitionResponseTypeDef:
         """
         Creates a Device Advisor test suite.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor.Client.create_suite_definition)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotdeviceadvisor/client/#create_suite_definition)
@@ -187,17 +183,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotdeviceadvisor/client/#list_tags_for_resource)
         """
     def start_suite_run(
         self,
         *,
         suiteDefinitionId: str,
-        suiteRunConfiguration: Union[
-            SuiteRunConfigurationTypeDef, SuiteRunConfigurationOutputTypeDef
-        ],
+        suiteRunConfiguration: SuiteRunConfigurationUnionTypeDef,
         suiteDefinitionVersion: str = ...,
         tags: Mapping[str, str] = ...
     ) -> StartSuiteRunResponseTypeDef:
         """
         Starts a Device Advisor test suite run.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor.Client.start_suite_run)
@@ -224,17 +218,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotdeviceadvisor/client/#untag_resource)
         """
     def update_suite_definition(
         self,
         *,
         suiteDefinitionId: str,
-        suiteDefinitionConfiguration: Union[
-            SuiteDefinitionConfigurationTypeDef, SuiteDefinitionConfigurationOutputTypeDef
-        ]
+        suiteDefinitionConfiguration: SuiteDefinitionConfigurationUnionTypeDef
     ) -> UpdateSuiteDefinitionResponseTypeDef:
         """
         Updates a Device Advisor test suite.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor.Client.update_suite_definition)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotdeviceadvisor/client/#update_suite_definition)
         """
```

### Comparing `mypy-boto3-iotdeviceadvisor-1.28.15.post1/mypy_boto3_iotdeviceadvisor/literals.py` & `mypy-boto3-iotdeviceadvisor-1.28.16/mypy_boto3_iotdeviceadvisor/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotdeviceadvisor-1.28.15.post1/mypy_boto3_iotdeviceadvisor/literals.pyi` & `mypy-boto3-iotdeviceadvisor-1.28.16/mypy_boto3_iotdeviceadvisor/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotdeviceadvisor-1.28.15.post1/mypy_boto3_iotdeviceadvisor/type_defs.py` & `mypy-boto3-iotdeviceadvisor-1.28.16/mypy_boto3_iotdeviceadvisor/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotdeviceadvisor/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_iotdeviceadvisor.type_defs import ResponseMetadataTypeDef
 
-    data: ResponseMetadataTypeDef = {...}
+    data: ResponseMetadataTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AuthenticationMethodType,
     ProtocolType,
     StatusType,
     SuiteRunStatusType,
     TestCaseScenarioStatusType,
@@ -57,17 +57,19 @@
     "SuiteDefinitionInformationTypeDef",
     "SuiteRunConfigurationOutputTypeDef",
     "SuiteRunConfigurationTypeDef",
     "ListSuiteRunsResponseTypeDef",
     "TestCaseRunTypeDef",
     "GetSuiteDefinitionResponseTypeDef",
     "CreateSuiteDefinitionRequestRequestTypeDef",
+    "SuiteDefinitionConfigurationUnionTypeDef",
     "UpdateSuiteDefinitionRequestRequestTypeDef",
     "ListSuiteDefinitionsResponseTypeDef",
     "StartSuiteRunRequestRequestTypeDef",
+    "SuiteRunConfigurationUnionTypeDef",
     "GroupResultTypeDef",
     "TestResultTypeDef",
     "GetSuiteRunResponseTypeDef",
 )
 
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
@@ -455,14 +457,17 @@
 class CreateSuiteDefinitionRequestRequestTypeDef(
     _RequiredCreateSuiteDefinitionRequestRequestTypeDef,
     _OptionalCreateSuiteDefinitionRequestRequestTypeDef,
 ):
     pass
 
 
+SuiteDefinitionConfigurationUnionTypeDef = Union[
+    SuiteDefinitionConfigurationTypeDef, SuiteDefinitionConfigurationOutputTypeDef
+]
 UpdateSuiteDefinitionRequestRequestTypeDef = TypedDict(
     "UpdateSuiteDefinitionRequestRequestTypeDef",
     {
         "suiteDefinitionId": str,
         "suiteDefinitionConfiguration": SuiteDefinitionConfigurationTypeDef,
     },
 )
@@ -495,14 +500,17 @@
 
 class StartSuiteRunRequestRequestTypeDef(
     _RequiredStartSuiteRunRequestRequestTypeDef, _OptionalStartSuiteRunRequestRequestTypeDef
 ):
     pass
 
 
+SuiteRunConfigurationUnionTypeDef = Union[
+    SuiteRunConfigurationTypeDef, SuiteRunConfigurationOutputTypeDef
+]
 GroupResultTypeDef = TypedDict(
     "GroupResultTypeDef",
     {
         "groupId": str,
         "groupName": str,
         "tests": List[TestCaseRunTypeDef],
     },
```

### Comparing `mypy-boto3-iotdeviceadvisor-1.28.15.post1/mypy_boto3_iotdeviceadvisor/type_defs.pyi` & `mypy-boto3-iotdeviceadvisor-1.28.16/mypy_boto3_iotdeviceadvisor/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotdeviceadvisor/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_iotdeviceadvisor.type_defs import ResponseMetadataTypeDef
 
-    data: ResponseMetadataTypeDef = {...}
+    data: ResponseMetadataTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AuthenticationMethodType,
     ProtocolType,
     StatusType,
     SuiteRunStatusType,
     TestCaseScenarioStatusType,
@@ -56,17 +56,19 @@
     "SuiteDefinitionInformationTypeDef",
     "SuiteRunConfigurationOutputTypeDef",
     "SuiteRunConfigurationTypeDef",
     "ListSuiteRunsResponseTypeDef",
     "TestCaseRunTypeDef",
     "GetSuiteDefinitionResponseTypeDef",
     "CreateSuiteDefinitionRequestRequestTypeDef",
+    "SuiteDefinitionConfigurationUnionTypeDef",
     "UpdateSuiteDefinitionRequestRequestTypeDef",
     "ListSuiteDefinitionsResponseTypeDef",
     "StartSuiteRunRequestRequestTypeDef",
+    "SuiteRunConfigurationUnionTypeDef",
     "GroupResultTypeDef",
     "TestResultTypeDef",
     "GetSuiteRunResponseTypeDef",
 )
 
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
@@ -442,14 +444,17 @@
 
 class CreateSuiteDefinitionRequestRequestTypeDef(
     _RequiredCreateSuiteDefinitionRequestRequestTypeDef,
     _OptionalCreateSuiteDefinitionRequestRequestTypeDef,
 ):
     pass
 
+SuiteDefinitionConfigurationUnionTypeDef = Union[
+    SuiteDefinitionConfigurationTypeDef, SuiteDefinitionConfigurationOutputTypeDef
+]
 UpdateSuiteDefinitionRequestRequestTypeDef = TypedDict(
     "UpdateSuiteDefinitionRequestRequestTypeDef",
     {
         "suiteDefinitionId": str,
         "suiteDefinitionConfiguration": SuiteDefinitionConfigurationTypeDef,
     },
 )
@@ -480,14 +485,17 @@
 )
 
 class StartSuiteRunRequestRequestTypeDef(
     _RequiredStartSuiteRunRequestRequestTypeDef, _OptionalStartSuiteRunRequestRequestTypeDef
 ):
     pass
 
+SuiteRunConfigurationUnionTypeDef = Union[
+    SuiteRunConfigurationTypeDef, SuiteRunConfigurationOutputTypeDef
+]
 GroupResultTypeDef = TypedDict(
     "GroupResultTypeDef",
     {
         "groupId": str,
         "groupName": str,
         "tests": List[TestCaseRunTypeDef],
     },
```

### Comparing `mypy-boto3-iotdeviceadvisor-1.28.15.post1/mypy_boto3_iotdeviceadvisor.egg-info/PKG-INFO` & `mypy-boto3-iotdeviceadvisor-1.28.16/mypy_boto3_iotdeviceadvisor.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iotdeviceadvisor
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.IoTDeviceAdvisor 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.IoTDeviceAdvisor 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotdeviceadvisor/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 iotdeviceadvisor type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 iotdeviceadvisor type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotdeviceadvisor.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotdeviceadvisor)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotdeviceadvisor/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iotdeviceadvisor)](https://pepy.tech/project/mypy-boto3-iotdeviceadvisor)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTDeviceAdvisor 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor)
+[boto3.IoTDeviceAdvisor 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor)
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
 [mypy-boto3-iotdeviceadvisor docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotdeviceadvisor/).
 
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
@@ -294,20 +294,20 @@
 )
 
 
 def check_value(value: AuthenticationMethodType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_iotdeviceadvisor.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_iotdeviceadvisor.type_defs import (
     ResponseMetadataTypeDef,
     DeleteSuiteDefinitionRequestRequestTypeDef,
     DeviceUnderTestTypeDef,
     GetEndpointRequestRequestTypeDef,
@@ -333,24 +333,26 @@
     SuiteDefinitionInformationTypeDef,
     SuiteRunConfigurationOutputTypeDef,
     SuiteRunConfigurationTypeDef,
     ListSuiteRunsResponseTypeDef,
     TestCaseRunTypeDef,
     GetSuiteDefinitionResponseTypeDef,
     CreateSuiteDefinitionRequestRequestTypeDef,
+    SuiteDefinitionConfigurationUnionTypeDef,
     UpdateSuiteDefinitionRequestRequestTypeDef,
     ListSuiteDefinitionsResponseTypeDef,
     StartSuiteRunRequestRequestTypeDef,
+    SuiteRunConfigurationUnionTypeDef,
     GroupResultTypeDef,
     TestResultTypeDef,
     GetSuiteRunResponseTypeDef,
 )
 
 
-def get_structure() -> ResponseMetadataTypeDef:
+def get_value() -> ResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-iotdeviceadvisor-1.28.15.post1/mypy_boto3_iotdeviceadvisor.egg-info/SOURCES.txt` & `mypy-boto3-iotdeviceadvisor-1.28.16/mypy_boto3_iotdeviceadvisor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotdeviceadvisor-1.28.15.post1/setup.py` & `mypy-boto3-iotdeviceadvisor-1.28.16/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-iotdeviceadvisor",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_iotdeviceadvisor"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.IoTDeviceAdvisor 1.28.15 service generated with"
-        " mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.IoTDeviceAdvisor 1.28.16 service generated with"
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
-    keywords="boto3 iotdeviceadvisor type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 iotdeviceadvisor type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_iotdeviceadvisor": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotdeviceadvisor/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

