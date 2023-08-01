# Comparing `tmp/mypy-boto3-migrationhub-config-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-migrationhub-config-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-migrationhub-config-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:44 2023, max compression
+gzip compressed data, was "mypy-boto3-migrationhub-config-1.28.16.tar", last modified: Tue Aug  1 11:37:23 2023, max compression
```

## Comparing `mypy-boto3-migrationhub-config-1.28.15.post1.tar` & `mypy-boto3-migrationhub-config-1.28.16.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:43.981299 mypy-boto3-migrationhub-config-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:51:40.000000 mypy-boto3-migrationhub-config-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12681 2023-07-29 10:03:43.981299 mypy-boto3-migrationhub-config-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11141 2023-07-29 09:51:40.000000 mypy-boto3-migrationhub-config-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:43.981299 mypy-boto3-migrationhub-config-1.28.15.post1/mypy_boto3_migrationhub_config/
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-29 09:51:40.000000 mypy-boto3-migrationhub-config-1.28.15.post1/mypy_boto3_migrationhub_config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-29 09:51:40.000000 mypy-boto3-migrationhub-config-1.28.15.post1/mypy_boto3_migrationhub_config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-07-29 09:51:40.000000 mypy-boto3-migrationhub-config-1.28.15.post1/mypy_boto3_migrationhub_config/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-07-29 09:51:40.000000 mypy-boto3-migrationhub-config-1.28.15.post1/mypy_boto3_migrationhub_config/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-07-29 09:51:40.000000 mypy-boto3-migrationhub-config-1.28.15.post1/mypy_boto3_migrationhub_config/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7696 2023-07-29 09:51:41.000000 mypy-boto3-migrationhub-config-1.28.15.post1/mypy_boto3_migrationhub_config/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7694 2023-07-29 09:51:40.000000 mypy-boto3-migrationhub-config-1.28.15.post1/mypy_boto3_migrationhub_config/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:51:40.000000 mypy-boto3-migrationhub-config-1.28.15.post1/mypy_boto3_migrationhub_config/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-07-29 09:51:41.000000 mypy-boto3-migrationhub-config-1.28.15.post1/mypy_boto3_migrationhub_config/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-07-29 09:51:41.000000 mypy-boto3-migrationhub-config-1.28.15.post1/mypy_boto3_migrationhub_config/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:51:40.000000 mypy-boto3-migrationhub-config-1.28.15.post1/mypy_boto3_migrationhub_config/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:43.981299 mypy-boto3-migrationhub-config-1.28.15.post1/mypy_boto3_migrationhub_config.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12681 2023-07-29 10:03:43.000000 mypy-boto3-migrationhub-config-1.28.15.post1/mypy_boto3_migrationhub_config.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-29 10:03:43.000000 mypy-boto3-migrationhub-config-1.28.15.post1/mypy_boto3_migrationhub_config.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:43.000000 mypy-boto3-migrationhub-config-1.28.15.post1/mypy_boto3_migrationhub_config.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:43.000000 mypy-boto3-migrationhub-config-1.28.15.post1/mypy_boto3_migrationhub_config.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:43.000000 mypy-boto3-migrationhub-config-1.28.15.post1/mypy_boto3_migrationhub_config.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-29 10:03:43.000000 mypy-boto3-migrationhub-config-1.28.15.post1/mypy_boto3_migrationhub_config.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:43.981299 mypy-boto3-migrationhub-config-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-07-29 09:51:40.000000 mypy-boto3-migrationhub-config-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:23.932813 mypy-boto3-migrationhub-config-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:24:40.000000 mypy-boto3-migrationhub-config-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12671 2023-08-01 11:37:23.924813 mypy-boto3-migrationhub-config-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11140 2023-08-01 11:24:40.000000 mypy-boto3-migrationhub-config-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:23.924813 mypy-boto3-migrationhub-config-1.28.16/mypy_boto3_migrationhub_config/
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-08-01 11:24:40.000000 mypy-boto3-migrationhub-config-1.28.16/mypy_boto3_migrationhub_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-08-01 11:24:40.000000 mypy-boto3-migrationhub-config-1.28.16/mypy_boto3_migrationhub_config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-08-01 11:24:40.000000 mypy-boto3-migrationhub-config-1.28.16/mypy_boto3_migrationhub_config/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-08-01 11:24:40.000000 mypy-boto3-migrationhub-config-1.28.16/mypy_boto3_migrationhub_config/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-08-01 11:24:40.000000 mypy-boto3-migrationhub-config-1.28.16/mypy_boto3_migrationhub_config/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7696 2023-08-01 11:24:40.000000 mypy-boto3-migrationhub-config-1.28.16/mypy_boto3_migrationhub_config/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7694 2023-08-01 11:24:40.000000 mypy-boto3-migrationhub-config-1.28.16/mypy_boto3_migrationhub_config/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:24:40.000000 mypy-boto3-migrationhub-config-1.28.16/mypy_boto3_migrationhub_config/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-08-01 11:24:40.000000 mypy-boto3-migrationhub-config-1.28.16/mypy_boto3_migrationhub_config/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-08-01 11:24:40.000000 mypy-boto3-migrationhub-config-1.28.16/mypy_boto3_migrationhub_config/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:24:40.000000 mypy-boto3-migrationhub-config-1.28.16/mypy_boto3_migrationhub_config/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:23.924813 mypy-boto3-migrationhub-config-1.28.16/mypy_boto3_migrationhub_config.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12671 2023-08-01 11:37:23.000000 mypy-boto3-migrationhub-config-1.28.16/mypy_boto3_migrationhub_config.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-08-01 11:37:23.000000 mypy-boto3-migrationhub-config-1.28.16/mypy_boto3_migrationhub_config.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:23.000000 mypy-boto3-migrationhub-config-1.28.16/mypy_boto3_migrationhub_config.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:23.000000 mypy-boto3-migrationhub-config-1.28.16/mypy_boto3_migrationhub_config.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:23.000000 mypy-boto3-migrationhub-config-1.28.16/mypy_boto3_migrationhub_config.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-01 11:37:23.000000 mypy-boto3-migrationhub-config-1.28.16/mypy_boto3_migrationhub_config.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:23.932813 mypy-boto3-migrationhub-config-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-08-01 11:24:40.000000 mypy-boto3-migrationhub-config-1.28.16/setup.py
```

### Comparing `mypy-boto3-migrationhub-config-1.28.15.post1/LICENSE` & `mypy-boto3-migrationhub-config-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migrationhub-config-1.28.15.post1/PKG-INFO` & `mypy-boto3-migrationhub-config-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-migrationhub-config
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.MigrationHubConfig 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.MigrationHubConfig 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhub_config/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 migrationhub-config type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 migrationhub-config type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-migrationhub-config.svg?color=blue)](https://pypi.org/project/mypy-boto3-migrationhub-config)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhub_config/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-migrationhub-config)](https://pepy.tech/project/mypy-boto3-migrationhub-config)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MigrationHubConfig 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhub-config.html#MigrationHubConfig)
+[boto3.MigrationHubConfig 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhub-config.html#MigrationHubConfig)
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
 [mypy-boto3-migrationhub-config docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhub_config/).
 
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
@@ -288,35 +288,35 @@
 )
 
 
 def check_value(value: TargetTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_migrationhub_config.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_migrationhub_config.type_defs import (
     TargetTypeDef,
     ResponseMetadataTypeDef,
     CreateHomeRegionControlRequestRequestTypeDef,
     DescribeHomeRegionControlsRequestRequestTypeDef,
     HomeRegionControlTypeDef,
     GetHomeRegionResultTypeDef,
     CreateHomeRegionControlResultTypeDef,
     DescribeHomeRegionControlsResultTypeDef,
 )
 
 
-def get_structure() -> TargetTypeDef:
+def get_value() -> TargetTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-migrationhub-config-1.28.15.post1/README.md` & `mypy-boto3-migrationhub-config-1.28.16/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-migrationhub-config.svg?color=blue)](https://pypi.org/project/mypy-boto3-migrationhub-config)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhub_config/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-migrationhub-config)](https://pepy.tech/project/mypy-boto3-migrationhub-config)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MigrationHubConfig 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhub-config.html#MigrationHubConfig)
+[boto3.MigrationHubConfig 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhub-config.html#MigrationHubConfig)
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
 [mypy-boto3-migrationhub-config docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhub_config/).
 
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
@@ -256,35 +256,35 @@
 )
 
 
 def check_value(value: TargetTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_migrationhub_config.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_migrationhub_config.type_defs import (
     TargetTypeDef,
     ResponseMetadataTypeDef,
     CreateHomeRegionControlRequestRequestTypeDef,
     DescribeHomeRegionControlsRequestRequestTypeDef,
     HomeRegionControlTypeDef,
     GetHomeRegionResultTypeDef,
     CreateHomeRegionControlResultTypeDef,
     DescribeHomeRegionControlsResultTypeDef,
 )
 
 
-def get_structure() -> TargetTypeDef:
+def get_value() -> TargetTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-migrationhub-config-1.28.15.post1/mypy_boto3_migrationhub_config/client.py` & `mypy-boto3-migrationhub-config-1.28.16/mypy_boto3_migrationhub_config/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migrationhub-config-1.28.15.post1/mypy_boto3_migrationhub_config/client.pyi` & `mypy-boto3-migrationhub-config-1.28.16/mypy_boto3_migrationhub_config/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migrationhub-config-1.28.15.post1/mypy_boto3_migrationhub_config/literals.py` & `mypy-boto3-migrationhub-config-1.28.16/mypy_boto3_migrationhub_config/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migrationhub-config-1.28.15.post1/mypy_boto3_migrationhub_config/literals.pyi` & `mypy-boto3-migrationhub-config-1.28.16/mypy_boto3_migrationhub_config/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migrationhub-config-1.28.15.post1/mypy_boto3_migrationhub_config/type_defs.py` & `mypy-boto3-migrationhub-config-1.28.16/mypy_boto3_migrationhub_config/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhub_config/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_migrationhub_config.type_defs import TargetTypeDef
 
-    data: TargetTypeDef = {...}
+    data: TargetTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List
 
 if sys.version_info >= (3, 9):
@@ -20,15 +20,14 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "TargetTypeDef",
     "ResponseMetadataTypeDef",
     "CreateHomeRegionControlRequestRequestTypeDef",
     "DescribeHomeRegionControlsRequestRequestTypeDef",
     "HomeRegionControlTypeDef",
     "GetHomeRegionResultTypeDef",
@@ -46,19 +45,17 @@
     "_OptionalTargetTypeDef",
     {
         "Id": str,
     },
     total=False,
 )
 
-
 class TargetTypeDef(_RequiredTargetTypeDef, _OptionalTargetTypeDef):
     pass
 
-
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -77,22 +74,20 @@
     "_OptionalCreateHomeRegionControlRequestRequestTypeDef",
     {
         "DryRun": bool,
     },
     total=False,
 )
 
-
 class CreateHomeRegionControlRequestRequestTypeDef(
     _RequiredCreateHomeRegionControlRequestRequestTypeDef,
     _OptionalCreateHomeRegionControlRequestRequestTypeDef,
 ):
     pass
 
-
 DescribeHomeRegionControlsRequestRequestTypeDef = TypedDict(
     "DescribeHomeRegionControlsRequestRequestTypeDef",
     {
         "ControlId": str,
         "HomeRegion": str,
         "Target": TargetTypeDef,
         "MaxResults": int,
```

### Comparing `mypy-boto3-migrationhub-config-1.28.15.post1/mypy_boto3_migrationhub_config/type_defs.pyi` & `mypy-boto3-migrationhub-config-1.28.16/mypy_boto3_migrationhub_config/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhub_config/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_migrationhub_config.type_defs import TargetTypeDef
 
-    data: TargetTypeDef = {...}
+    data: TargetTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List
 
 if sys.version_info >= (3, 9):
@@ -20,14 +20,15 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "TargetTypeDef",
     "ResponseMetadataTypeDef",
     "CreateHomeRegionControlRequestRequestTypeDef",
     "DescribeHomeRegionControlsRequestRequestTypeDef",
     "HomeRegionControlTypeDef",
     "GetHomeRegionResultTypeDef",
@@ -45,17 +46,19 @@
     "_OptionalTargetTypeDef",
     {
         "Id": str,
     },
     total=False,
 )
 
+
 class TargetTypeDef(_RequiredTargetTypeDef, _OptionalTargetTypeDef):
     pass
 
+
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -74,20 +77,22 @@
     "_OptionalCreateHomeRegionControlRequestRequestTypeDef",
     {
         "DryRun": bool,
     },
     total=False,
 )
 
+
 class CreateHomeRegionControlRequestRequestTypeDef(
     _RequiredCreateHomeRegionControlRequestRequestTypeDef,
     _OptionalCreateHomeRegionControlRequestRequestTypeDef,
 ):
     pass
 
+
 DescribeHomeRegionControlsRequestRequestTypeDef = TypedDict(
     "DescribeHomeRegionControlsRequestRequestTypeDef",
     {
         "ControlId": str,
         "HomeRegion": str,
         "Target": TargetTypeDef,
         "MaxResults": int,
```

### Comparing `mypy-boto3-migrationhub-config-1.28.15.post1/mypy_boto3_migrationhub_config.egg-info/PKG-INFO` & `mypy-boto3-migrationhub-config-1.28.16/mypy_boto3_migrationhub_config.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-migrationhub-config
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.MigrationHubConfig 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.MigrationHubConfig 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhub_config/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 migrationhub-config type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 migrationhub-config type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-migrationhub-config.svg?color=blue)](https://pypi.org/project/mypy-boto3-migrationhub-config)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhub_config/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-migrationhub-config)](https://pepy.tech/project/mypy-boto3-migrationhub-config)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MigrationHubConfig 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhub-config.html#MigrationHubConfig)
+[boto3.MigrationHubConfig 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhub-config.html#MigrationHubConfig)
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
 [mypy-boto3-migrationhub-config docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhub_config/).
 
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
@@ -288,35 +288,35 @@
 )
 
 
 def check_value(value: TargetTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_migrationhub_config.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_migrationhub_config.type_defs import (
     TargetTypeDef,
     ResponseMetadataTypeDef,
     CreateHomeRegionControlRequestRequestTypeDef,
     DescribeHomeRegionControlsRequestRequestTypeDef,
     HomeRegionControlTypeDef,
     GetHomeRegionResultTypeDef,
     CreateHomeRegionControlResultTypeDef,
     DescribeHomeRegionControlsResultTypeDef,
 )
 
 
-def get_structure() -> TargetTypeDef:
+def get_value() -> TargetTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-migrationhub-config-1.28.15.post1/mypy_boto3_migrationhub_config.egg-info/SOURCES.txt` & `mypy-boto3-migrationhub-config-1.28.16/mypy_boto3_migrationhub_config.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migrationhub-config-1.28.15.post1/setup.py` & `mypy-boto3-migrationhub-config-1.28.16/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-migrationhub-config",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_migrationhub_config"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.MigrationHubConfig 1.28.15 service generated with"
-        " mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.MigrationHubConfig 1.28.16 service generated with"
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
-    keywords="boto3 migrationhub-config type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 migrationhub-config type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_migrationhub_config": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhub_config/"
```
