# Comparing `tmp/mypy-boto3-iot-roborunner-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-iot-roborunner-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-iot-roborunner-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:19 2023, max compression
+gzip compressed data, was "mypy-boto3-iot-roborunner-1.28.16.tar", last modified: Tue Aug  1 11:36:59 2023, max compression
```

## Comparing `mypy-boto3-iot-roborunner-1.28.15.post1.tar` & `mypy-boto3-iot-roborunner-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:19.905182 mypy-boto3-iot-roborunner-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:47:44.000000 mypy-boto3-iot-roborunner-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15154 2023-07-29 10:03:19.901182 mypy-boto3-iot-roborunner-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13634 2023-07-29 09:47:44.000000 mypy-boto3-iot-roborunner-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:19.897182 mypy-boto3-iot-roborunner-1.28.15.post1/mypy_boto3_iot_roborunner/
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-07-29 09:47:44.000000 mypy-boto3-iot-roborunner-1.28.15.post1/mypy_boto3_iot_roborunner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-07-29 09:47:44.000000 mypy-boto3-iot-roborunner-1.28.15.post1/mypy_boto3_iot_roborunner/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-29 09:47:44.000000 mypy-boto3-iot-roborunner-1.28.15.post1/mypy_boto3_iot_roborunner/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19292 2023-07-29 09:47:44.000000 mypy-boto3-iot-roborunner-1.28.15.post1/mypy_boto3_iot_roborunner/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    19261 2023-07-29 09:47:44.000000 mypy-boto3-iot-roborunner-1.28.15.post1/mypy_boto3_iot_roborunner/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8289 2023-07-29 09:47:45.000000 mypy-boto3-iot-roborunner-1.28.15.post1/mypy_boto3_iot_roborunner/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8287 2023-07-29 09:47:44.000000 mypy-boto3-iot-roborunner-1.28.15.post1/mypy_boto3_iot_roborunner/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5194 2023-07-29 09:47:44.000000 mypy-boto3-iot-roborunner-1.28.15.post1/mypy_boto3_iot_roborunner/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-07-29 09:47:44.000000 mypy-boto3-iot-roborunner-1.28.15.post1/mypy_boto3_iot_roborunner/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:47:44.000000 mypy-boto3-iot-roborunner-1.28.15.post1/mypy_boto3_iot_roborunner/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    20216 2023-07-29 09:47:45.000000 mypy-boto3-iot-roborunner-1.28.15.post1/mypy_boto3_iot_roborunner/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    20177 2023-07-29 09:47:45.000000 mypy-boto3-iot-roborunner-1.28.15.post1/mypy_boto3_iot_roborunner/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:47:44.000000 mypy-boto3-iot-roborunner-1.28.15.post1/mypy_boto3_iot_roborunner/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:19.901182 mypy-boto3-iot-roborunner-1.28.15.post1/mypy_boto3_iot_roborunner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15154 2023-07-29 10:03:19.000000 mypy-boto3-iot-roborunner-1.28.15.post1/mypy_boto3_iot_roborunner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-29 10:03:19.000000 mypy-boto3-iot-roborunner-1.28.15.post1/mypy_boto3_iot_roborunner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:19.000000 mypy-boto3-iot-roborunner-1.28.15.post1/mypy_boto3_iot_roborunner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:19.000000 mypy-boto3-iot-roborunner-1.28.15.post1/mypy_boto3_iot_roborunner.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:19.000000 mypy-boto3-iot-roborunner-1.28.15.post1/mypy_boto3_iot_roborunner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-29 10:03:19.000000 mypy-boto3-iot-roborunner-1.28.15.post1/mypy_boto3_iot_roborunner.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:19.905182 mypy-boto3-iot-roborunner-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-29 09:47:44.000000 mypy-boto3-iot-roborunner-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:59.736866 mypy-boto3-iot-roborunner-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:20:26.000000 mypy-boto3-iot-roborunner-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15144 2023-08-01 11:36:59.728866 mypy-boto3-iot-roborunner-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13633 2023-08-01 11:20:26.000000 mypy-boto3-iot-roborunner-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:59.720866 mypy-boto3-iot-roborunner-1.28.16/mypy_boto3_iot_roborunner/
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-08-01 11:20:26.000000 mypy-boto3-iot-roborunner-1.28.16/mypy_boto3_iot_roborunner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-08-01 11:20:26.000000 mypy-boto3-iot-roborunner-1.28.16/mypy_boto3_iot_roborunner/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-08-01 11:20:26.000000 mypy-boto3-iot-roborunner-1.28.16/mypy_boto3_iot_roborunner/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19292 2023-08-01 11:20:26.000000 mypy-boto3-iot-roborunner-1.28.16/mypy_boto3_iot_roborunner/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19261 2023-08-01 11:20:26.000000 mypy-boto3-iot-roborunner-1.28.16/mypy_boto3_iot_roborunner/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8289 2023-08-01 11:20:26.000000 mypy-boto3-iot-roborunner-1.28.16/mypy_boto3_iot_roborunner/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8287 2023-08-01 11:20:26.000000 mypy-boto3-iot-roborunner-1.28.16/mypy_boto3_iot_roborunner/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5194 2023-08-01 11:20:26.000000 mypy-boto3-iot-roborunner-1.28.16/mypy_boto3_iot_roborunner/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-08-01 11:20:26.000000 mypy-boto3-iot-roborunner-1.28.16/mypy_boto3_iot_roborunner/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:20:26.000000 mypy-boto3-iot-roborunner-1.28.16/mypy_boto3_iot_roborunner/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    20214 2023-08-01 11:20:27.000000 mypy-boto3-iot-roborunner-1.28.16/mypy_boto3_iot_roborunner/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20175 2023-08-01 11:20:26.000000 mypy-boto3-iot-roborunner-1.28.16/mypy_boto3_iot_roborunner/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:20:26.000000 mypy-boto3-iot-roborunner-1.28.16/mypy_boto3_iot_roborunner/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:59.728866 mypy-boto3-iot-roborunner-1.28.16/mypy_boto3_iot_roborunner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15144 2023-08-01 11:36:59.000000 mypy-boto3-iot-roborunner-1.28.16/mypy_boto3_iot_roborunner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-08-01 11:36:59.000000 mypy-boto3-iot-roborunner-1.28.16/mypy_boto3_iot_roborunner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:59.000000 mypy-boto3-iot-roborunner-1.28.16/mypy_boto3_iot_roborunner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:59.000000 mypy-boto3-iot-roborunner-1.28.16/mypy_boto3_iot_roborunner.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:59.000000 mypy-boto3-iot-roborunner-1.28.16/mypy_boto3_iot_roborunner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-01 11:36:59.000000 mypy-boto3-iot-roborunner-1.28.16/mypy_boto3_iot_roborunner.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:59.736866 mypy-boto3-iot-roborunner-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-08-01 11:20:26.000000 mypy-boto3-iot-roborunner-1.28.16/setup.py
```

### Comparing `mypy-boto3-iot-roborunner-1.28.15.post1/LICENSE` & `mypy-boto3-iot-roborunner-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot-roborunner-1.28.15.post1/PKG-INFO` & `mypy-boto3-iot-roborunner-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iot-roborunner
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.IoTRoboRunner 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.IoTRoboRunner 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_roborunner/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 iot-roborunner type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 iot-roborunner type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iot-roborunner.svg?color=blue)](https://pypi.org/project/mypy-boto3-iot-roborunner)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_roborunner/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iot-roborunner)](https://pepy.tech/project/mypy-boto3-iot-roborunner)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTRoboRunner 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner)
+[boto3.IoTRoboRunner 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner)
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
 [mypy-boto3-iot-roborunner docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_roborunner/).
 
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
@@ -323,20 +323,20 @@
 )
 
 
 def check_value(value: DestinationStateType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_iot_roborunner.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_iot_roborunner.type_defs import (
     CartesianCoordinatesTypeDef,
     CreateDestinationRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     CreateSiteRequestRequestTypeDef,
@@ -385,15 +385,15 @@
     UpdateWorkerRequestRequestTypeDef,
     UpdateWorkerResponseTypeDef,
     WorkerTypeDef,
     ListWorkersResponseTypeDef,
 )
 
 
-def get_structure() -> CartesianCoordinatesTypeDef:
+def get_value() -> CartesianCoordinatesTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-iot-roborunner-1.28.15.post1/README.md` & `mypy-boto3-iot-roborunner-1.28.16/mypy_boto3_iot_roborunner.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-iot-roborunner
+Version: 1.28.16
+Summary: Type annotations for boto3.IoTRoboRunner 1.28.16 service generated with mypy-boto3-builder 7.17.1
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_roborunner/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 iot-roborunner type-annotations botocore mypy typeshed autocomplete
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
 <a id="mypy-boto3-iot-roborunner"></a>
 
 # mypy-boto3-iot-roborunner
 
 [![PyPI - mypy-boto3-iot-roborunner](https://img.shields.io/pypi/v/mypy-boto3-iot-roborunner.svg?color=blue)](https://pypi.org/project/mypy-boto3-iot-roborunner)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iot-roborunner.svg?color=blue)](https://pypi.org/project/mypy-boto3-iot-roborunner)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_roborunner/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iot-roborunner)](https://pepy.tech/project/mypy-boto3-iot-roborunner)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTRoboRunner 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner)
+[boto3.IoTRoboRunner 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner)
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
 [mypy-boto3-iot-roborunner docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_roborunner/).
 
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
@@ -291,20 +323,20 @@
 )
 
 
 def check_value(value: DestinationStateType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_iot_roborunner.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_iot_roborunner.type_defs import (
     CartesianCoordinatesTypeDef,
     CreateDestinationRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     CreateSiteRequestRequestTypeDef,
@@ -353,15 +385,15 @@
     UpdateWorkerRequestRequestTypeDef,
     UpdateWorkerResponseTypeDef,
     WorkerTypeDef,
     ListWorkersResponseTypeDef,
 )
 
 
-def get_structure() -> CartesianCoordinatesTypeDef:
+def get_value() -> CartesianCoordinatesTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-iot-roborunner-1.28.15.post1/mypy_boto3_iot_roborunner/__init__.py` & `mypy-boto3-iot-roborunner-1.28.16/mypy_boto3_iot_roborunner/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot-roborunner-1.28.15.post1/mypy_boto3_iot_roborunner/__init__.pyi` & `mypy-boto3-iot-roborunner-1.28.16/mypy_boto3_iot_roborunner/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot-roborunner-1.28.15.post1/mypy_boto3_iot_roborunner/__main__.py` & `mypy-boto3-iot-roborunner-1.28.16/mypy_boto3_iot_roborunner/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.IoTRoboRunner 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.IoTRoboRunner 1.28.16\nVersion:         1.28.16\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_roborunner//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner\nOther"
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

### Comparing `mypy-boto3-iot-roborunner-1.28.15.post1/mypy_boto3_iot_roborunner/client.py` & `mypy-boto3-iot-roborunner-1.28.16/mypy_boto3_iot_roborunner/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot-roborunner-1.28.15.post1/mypy_boto3_iot_roborunner/client.pyi` & `mypy-boto3-iot-roborunner-1.28.16/mypy_boto3_iot_roborunner/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot-roborunner-1.28.15.post1/mypy_boto3_iot_roborunner/literals.py` & `mypy-boto3-iot-roborunner-1.28.16/mypy_boto3_iot_roborunner/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot-roborunner-1.28.15.post1/mypy_boto3_iot_roborunner/literals.pyi` & `mypy-boto3-iot-roborunner-1.28.16/mypy_boto3_iot_roborunner/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot-roborunner-1.28.15.post1/mypy_boto3_iot_roborunner/paginator.py` & `mypy-boto3-iot-roborunner-1.28.16/mypy_boto3_iot_roborunner/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot-roborunner-1.28.15.post1/mypy_boto3_iot_roborunner/paginator.pyi` & `mypy-boto3-iot-roborunner-1.28.16/mypy_boto3_iot_roborunner/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot-roborunner-1.28.15.post1/mypy_boto3_iot_roborunner/type_defs.py` & `mypy-boto3-iot-roborunner-1.28.16/mypy_boto3_iot_roborunner/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_roborunner/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_iot_roborunner.type_defs import CartesianCoordinatesTypeDef
 
-    data: CartesianCoordinatesTypeDef = {...}
+    data: CartesianCoordinatesTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List
 
 from .literals import DestinationStateType
```

### Comparing `mypy-boto3-iot-roborunner-1.28.15.post1/mypy_boto3_iot_roborunner/type_defs.pyi` & `mypy-boto3-iot-roborunner-1.28.16/mypy_boto3_iot_roborunner/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_roborunner/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_iot_roborunner.type_defs import CartesianCoordinatesTypeDef
 
-    data: CartesianCoordinatesTypeDef = {...}
+    data: CartesianCoordinatesTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List
 
 from .literals import DestinationStateType
```

### Comparing `mypy-boto3-iot-roborunner-1.28.15.post1/mypy_boto3_iot_roborunner.egg-info/PKG-INFO` & `mypy-boto3-iot-roborunner-1.28.16/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,61 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-iot-roborunner
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.IoTRoboRunner 1.28.15 service generated with mypy-boto3-builder 7.16.2
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_roborunner/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 iot-roborunner type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-iot-roborunner"></a>
 
 # mypy-boto3-iot-roborunner
 
 [![PyPI - mypy-boto3-iot-roborunner](https://img.shields.io/pypi/v/mypy-boto3-iot-roborunner.svg?color=blue)](https://pypi.org/project/mypy-boto3-iot-roborunner)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iot-roborunner.svg?color=blue)](https://pypi.org/project/mypy-boto3-iot-roborunner)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_roborunner/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iot-roborunner)](https://pepy.tech/project/mypy-boto3-iot-roborunner)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTRoboRunner 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner)
+[boto3.IoTRoboRunner 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner)
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
 [mypy-boto3-iot-roborunner docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_roborunner/).
 
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
@@ -323,20 +291,20 @@
 )
 
 
 def check_value(value: DestinationStateType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_iot_roborunner.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_iot_roborunner.type_defs import (
     CartesianCoordinatesTypeDef,
     CreateDestinationRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     CreateSiteRequestRequestTypeDef,
@@ -385,15 +353,15 @@
     UpdateWorkerRequestRequestTypeDef,
     UpdateWorkerResponseTypeDef,
     WorkerTypeDef,
     ListWorkersResponseTypeDef,
 )
 
 
-def get_structure() -> CartesianCoordinatesTypeDef:
+def get_value() -> CartesianCoordinatesTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-iot-roborunner-1.28.15.post1/mypy_boto3_iot_roborunner.egg-info/SOURCES.txt` & `mypy-boto3-iot-roborunner-1.28.16/mypy_boto3_iot_roborunner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot-roborunner-1.28.15.post1/setup.py` & `mypy-boto3-iot-roborunner-1.28.16/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-iot-roborunner",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_iot_roborunner"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.IoTRoboRunner 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.2"
+        "Type annotations for boto3.IoTRoboRunner 1.28.16 service generated with mypy-boto3-builder"
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
-    keywords="boto3 iot-roborunner type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 iot-roborunner type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_iot_roborunner": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_roborunner/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

