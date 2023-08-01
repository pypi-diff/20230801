# Comparing `tmp/mypy-boto3-resource-groups-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-resource-groups-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-resource-groups-1.28.15.post1.tar", last modified: Sat Jul 29 10:04:01 2023, max compression
+gzip compressed data, was "mypy-boto3-resource-groups-1.28.16.tar", last modified: Tue Aug  1 11:37:40 2023, max compression
```

## Comparing `mypy-boto3-resource-groups-1.28.15.post1.tar` & `mypy-boto3-resource-groups-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:01.221365 mypy-boto3-resource-groups-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:57:04.000000 mypy-boto3-resource-groups-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15425 2023-07-29 10:04:01.217365 mypy-boto3-resource-groups-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13901 2023-07-29 09:57:04.000000 mypy-boto3-resource-groups-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:01.205365 mypy-boto3-resource-groups-1.28.15.post1/mypy_boto3_resource_groups/
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-29 09:57:04.000000 mypy-boto3-resource-groups-1.28.15.post1/mypy_boto3_resource_groups/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-07-29 09:57:04.000000 mypy-boto3-resource-groups-1.28.15.post1/mypy_boto3_resource_groups/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-29 09:57:04.000000 mypy-boto3-resource-groups-1.28.15.post1/mypy_boto3_resource_groups/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15674 2023-07-29 09:57:04.000000 mypy-boto3-resource-groups-1.28.15.post1/mypy_boto3_resource_groups/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15646 2023-07-29 09:57:04.000000 mypy-boto3-resource-groups-1.28.15.post1/mypy_boto3_resource_groups/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9496 2023-07-29 09:57:05.000000 mypy-boto3-resource-groups-1.28.15.post1/mypy_boto3_resource_groups/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9494 2023-07-29 09:57:05.000000 mypy-boto3-resource-groups-1.28.15.post1/mypy_boto3_resource_groups/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4359 2023-07-29 09:57:04.000000 mypy-boto3-resource-groups-1.28.15.post1/mypy_boto3_resource_groups/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4354 2023-07-29 09:57:04.000000 mypy-boto3-resource-groups-1.28.15.post1/mypy_boto3_resource_groups/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:57:04.000000 mypy-boto3-resource-groups-1.28.15.post1/mypy_boto3_resource_groups/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    17125 2023-07-29 09:57:05.000000 mypy-boto3-resource-groups-1.28.15.post1/mypy_boto3_resource_groups/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    17106 2023-07-29 09:57:05.000000 mypy-boto3-resource-groups-1.28.15.post1/mypy_boto3_resource_groups/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:57:04.000000 mypy-boto3-resource-groups-1.28.15.post1/mypy_boto3_resource_groups/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:01.217365 mypy-boto3-resource-groups-1.28.15.post1/mypy_boto3_resource_groups.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15425 2023-07-29 10:04:00.000000 mypy-boto3-resource-groups-1.28.15.post1/mypy_boto3_resource_groups.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-29 10:04:01.000000 mypy-boto3-resource-groups-1.28.15.post1/mypy_boto3_resource_groups.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:00.000000 mypy-boto3-resource-groups-1.28.15.post1/mypy_boto3_resource_groups.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:00.000000 mypy-boto3-resource-groups-1.28.15.post1/mypy_boto3_resource_groups.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:04:00.000000 mypy-boto3-resource-groups-1.28.15.post1/mypy_boto3_resource_groups.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-29 10:04:00.000000 mypy-boto3-resource-groups-1.28.15.post1/mypy_boto3_resource_groups.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:04:01.221365 mypy-boto3-resource-groups-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-07-29 09:57:04.000000 mypy-boto3-resource-groups-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:40.844768 mypy-boto3-resource-groups-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:30:26.000000 mypy-boto3-resource-groups-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15455 2023-08-01 11:37:40.840768 mypy-boto3-resource-groups-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13940 2023-08-01 11:30:26.000000 mypy-boto3-resource-groups-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:40.836768 mypy-boto3-resource-groups-1.28.16/mypy_boto3_resource_groups/
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-08-01 11:30:26.000000 mypy-boto3-resource-groups-1.28.16/mypy_boto3_resource_groups/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-08-01 11:30:26.000000 mypy-boto3-resource-groups-1.28.16/mypy_boto3_resource_groups/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-08-01 11:30:26.000000 mypy-boto3-resource-groups-1.28.16/mypy_boto3_resource_groups/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15485 2023-08-01 11:30:26.000000 mypy-boto3-resource-groups-1.28.16/mypy_boto3_resource_groups/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15457 2023-08-01 11:30:26.000000 mypy-boto3-resource-groups-1.28.16/mypy_boto3_resource_groups/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9496 2023-08-01 11:30:27.000000 mypy-boto3-resource-groups-1.28.16/mypy_boto3_resource_groups/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9494 2023-08-01 11:30:27.000000 mypy-boto3-resource-groups-1.28.16/mypy_boto3_resource_groups/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4359 2023-08-01 11:30:26.000000 mypy-boto3-resource-groups-1.28.16/mypy_boto3_resource_groups/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4354 2023-08-01 11:30:26.000000 mypy-boto3-resource-groups-1.28.16/mypy_boto3_resource_groups/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:30:26.000000 mypy-boto3-resource-groups-1.28.16/mypy_boto3_resource_groups/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    17160 2023-08-01 11:30:27.000000 mypy-boto3-resource-groups-1.28.16/mypy_boto3_resource_groups/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17141 2023-08-01 11:30:27.000000 mypy-boto3-resource-groups-1.28.16/mypy_boto3_resource_groups/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:30:26.000000 mypy-boto3-resource-groups-1.28.16/mypy_boto3_resource_groups/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:40.840768 mypy-boto3-resource-groups-1.28.16/mypy_boto3_resource_groups.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15455 2023-08-01 11:37:40.000000 mypy-boto3-resource-groups-1.28.16/mypy_boto3_resource_groups.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-08-01 11:37:40.000000 mypy-boto3-resource-groups-1.28.16/mypy_boto3_resource_groups.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:40.000000 mypy-boto3-resource-groups-1.28.16/mypy_boto3_resource_groups.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:40.000000 mypy-boto3-resource-groups-1.28.16/mypy_boto3_resource_groups.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:40.000000 mypy-boto3-resource-groups-1.28.16/mypy_boto3_resource_groups.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-01 11:37:40.000000 mypy-boto3-resource-groups-1.28.16/mypy_boto3_resource_groups.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:40.844768 mypy-boto3-resource-groups-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-08-01 11:30:26.000000 mypy-boto3-resource-groups-1.28.16/setup.py
```

### Comparing `mypy-boto3-resource-groups-1.28.15.post1/LICENSE` & `mypy-boto3-resource-groups-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-resource-groups-1.28.15.post1/PKG-INFO` & `mypy-boto3-resource-groups-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-resource-groups
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.ResourceGroups 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.ResourceGroups 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_groups/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 resource-groups type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 resource-groups type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-resource-groups.svg?color=blue)](https://pypi.org/project/mypy-boto3-resource-groups)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_groups/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-resource-groups)](https://pepy.tech/project/mypy-boto3-resource-groups)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ResourceGroups 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups)
+[boto3.ResourceGroups 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups)
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
 [mypy-boto3-resource-groups docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_groups/).
 
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
@@ -329,20 +329,20 @@
 )
 
 
 def check_value(value: GroupConfigurationStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_resource_groups.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_resource_groups.type_defs import (
     AccountSettingsTypeDef,
     ResourceQueryTypeDef,
     GroupTypeDef,
     ResponseMetadataTypeDef,
@@ -390,23 +390,24 @@
     ListGroupResourcesInputListGroupResourcesPaginateTypeDef,
     ListGroupResourcesInputRequestTypeDef,
     ListGroupResourcesItemTypeDef,
     SearchResourcesOutputTypeDef,
     GetGroupQueryOutputTypeDef,
     UpdateGroupQueryOutputTypeDef,
     GroupConfigurationTypeDef,
-    CreateGroupInputRequestTypeDef,
-    PutGroupConfigurationInputRequestTypeDef,
+    GroupConfigurationItemUnionTypeDef,
     ListGroupResourcesOutputTypeDef,
     CreateGroupOutputTypeDef,
     GetGroupConfigurationOutputTypeDef,
+    CreateGroupInputRequestTypeDef,
+    PutGroupConfigurationInputRequestTypeDef,
 )
 
 
-def get_structure() -> AccountSettingsTypeDef:
+def get_value() -> AccountSettingsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-resource-groups-1.28.15.post1/README.md` & `mypy-boto3-resource-groups-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-resource-groups.svg?color=blue)](https://pypi.org/project/mypy-boto3-resource-groups)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_groups/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-resource-groups)](https://pepy.tech/project/mypy-boto3-resource-groups)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ResourceGroups 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups)
+[boto3.ResourceGroups 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups)
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
 [mypy-boto3-resource-groups docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_groups/).
 
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
@@ -297,20 +297,20 @@
 )
 
 
 def check_value(value: GroupConfigurationStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_resource_groups.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_resource_groups.type_defs import (
     AccountSettingsTypeDef,
     ResourceQueryTypeDef,
     GroupTypeDef,
     ResponseMetadataTypeDef,
@@ -358,23 +358,24 @@
     ListGroupResourcesInputListGroupResourcesPaginateTypeDef,
     ListGroupResourcesInputRequestTypeDef,
     ListGroupResourcesItemTypeDef,
     SearchResourcesOutputTypeDef,
     GetGroupQueryOutputTypeDef,
     UpdateGroupQueryOutputTypeDef,
     GroupConfigurationTypeDef,
-    CreateGroupInputRequestTypeDef,
-    PutGroupConfigurationInputRequestTypeDef,
+    GroupConfigurationItemUnionTypeDef,
     ListGroupResourcesOutputTypeDef,
     CreateGroupOutputTypeDef,
     GetGroupConfigurationOutputTypeDef,
+    CreateGroupInputRequestTypeDef,
+    PutGroupConfigurationInputRequestTypeDef,
 )
 
 
-def get_structure() -> AccountSettingsTypeDef:
+def get_value() -> AccountSettingsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-resource-groups-1.28.15.post1/mypy_boto3_resource_groups/__init__.py` & `mypy-boto3-resource-groups-1.28.16/mypy_boto3_resource_groups/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-resource-groups-1.28.15.post1/mypy_boto3_resource_groups/__init__.pyi` & `mypy-boto3-resource-groups-1.28.16/mypy_boto3_resource_groups/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-resource-groups-1.28.15.post1/mypy_boto3_resource_groups/__main__.py` & `mypy-boto3-resource-groups-1.28.16/mypy_boto3_resource_groups/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ResourceGroups 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.ResourceGroups 1.28.16\nVersion:         1.28.16\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_groups//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups\nOther"
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

### Comparing `mypy-boto3-resource-groups-1.28.15.post1/mypy_boto3_resource_groups/client.py` & `mypy-boto3-resource-groups-1.28.16/mypy_boto3_resource_groups/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,30 +10,29 @@
     from mypy_boto3_resource_groups.client import ResourceGroupsClient
 
     session = Session()
     client: ResourceGroupsClient = session.client("resource-groups")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import GroupLifecycleEventsDesiredStatusType
 from .paginator import ListGroupResourcesPaginator, ListGroupsPaginator, SearchResourcesPaginator
 from .type_defs import (
     CreateGroupOutputTypeDef,
     DeleteGroupOutputTypeDef,
     GetAccountSettingsOutputTypeDef,
     GetGroupConfigurationOutputTypeDef,
     GetGroupOutputTypeDef,
     GetGroupQueryOutputTypeDef,
     GetTagsOutputTypeDef,
-    GroupConfigurationItemOutputTypeDef,
-    GroupConfigurationItemTypeDef,
+    GroupConfigurationItemUnionTypeDef,
     GroupFilterTypeDef,
     GroupResourcesOutputTypeDef,
     ListGroupResourcesOutputTypeDef,
     ListGroupsOutputTypeDef,
     ResourceFilterTypeDef,
     ResourceQueryTypeDef,
     SearchResourcesOutputTypeDef,
@@ -109,17 +108,15 @@
     def create_group(
         self,
         *,
         Name: str,
         Description: str = ...,
         ResourceQuery: ResourceQueryTypeDef = ...,
         Tags: Mapping[str, str] = ...,
-        Configuration: Sequence[
-            Union[GroupConfigurationItemTypeDef, GroupConfigurationItemOutputTypeDef]
-        ] = ...
+        Configuration: Sequence[GroupConfigurationItemUnionTypeDef] = ...
     ) -> CreateGroupOutputTypeDef:
         """
         Creates a resource group with the specified name and description.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Client.create_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_groups/client/#create_group)
         """
@@ -228,20 +225,15 @@
         Returns a list of existing Resource Groups in your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Client.list_groups)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_groups/client/#list_groups)
         """
 
     def put_group_configuration(
-        self,
-        *,
-        Group: str = ...,
-        Configuration: Sequence[
-            Union[GroupConfigurationItemTypeDef, GroupConfigurationItemOutputTypeDef]
-        ] = ...
+        self, *, Group: str = ..., Configuration: Sequence[GroupConfigurationItemUnionTypeDef] = ...
     ) -> Dict[str, Any]:
         """
         Attaches a service configuration to the specified group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Client.put_group_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_groups/client/#put_group_configuration)
         """
```

### Comparing `mypy-boto3-resource-groups-1.28.15.post1/mypy_boto3_resource_groups/client.pyi` & `mypy-boto3-resource-groups-1.28.16/mypy_boto3_resource_groups/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -10,30 +10,29 @@
     from mypy_boto3_resource_groups.client import ResourceGroupsClient
 
     session = Session()
     client: ResourceGroupsClient = session.client("resource-groups")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import GroupLifecycleEventsDesiredStatusType
 from .paginator import ListGroupResourcesPaginator, ListGroupsPaginator, SearchResourcesPaginator
 from .type_defs import (
     CreateGroupOutputTypeDef,
     DeleteGroupOutputTypeDef,
     GetAccountSettingsOutputTypeDef,
     GetGroupConfigurationOutputTypeDef,
     GetGroupOutputTypeDef,
     GetGroupQueryOutputTypeDef,
     GetTagsOutputTypeDef,
-    GroupConfigurationItemOutputTypeDef,
-    GroupConfigurationItemTypeDef,
+    GroupConfigurationItemUnionTypeDef,
     GroupFilterTypeDef,
     GroupResourcesOutputTypeDef,
     ListGroupResourcesOutputTypeDef,
     ListGroupsOutputTypeDef,
     ResourceFilterTypeDef,
     ResourceQueryTypeDef,
     SearchResourcesOutputTypeDef,
@@ -102,17 +101,15 @@
     def create_group(
         self,
         *,
         Name: str,
         Description: str = ...,
         ResourceQuery: ResourceQueryTypeDef = ...,
         Tags: Mapping[str, str] = ...,
-        Configuration: Sequence[
-            Union[GroupConfigurationItemTypeDef, GroupConfigurationItemOutputTypeDef]
-        ] = ...
+        Configuration: Sequence[GroupConfigurationItemUnionTypeDef] = ...
     ) -> CreateGroupOutputTypeDef:
         """
         Creates a resource group with the specified name and description.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Client.create_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_groups/client/#create_group)
         """
@@ -210,20 +207,15 @@
         """
         Returns a list of existing Resource Groups in your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Client.list_groups)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_groups/client/#list_groups)
         """
     def put_group_configuration(
-        self,
-        *,
-        Group: str = ...,
-        Configuration: Sequence[
-            Union[GroupConfigurationItemTypeDef, GroupConfigurationItemOutputTypeDef]
-        ] = ...
+        self, *, Group: str = ..., Configuration: Sequence[GroupConfigurationItemUnionTypeDef] = ...
     ) -> Dict[str, Any]:
         """
         Attaches a service configuration to the specified group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Client.put_group_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_groups/client/#put_group_configuration)
         """
```

### Comparing `mypy-boto3-resource-groups-1.28.15.post1/mypy_boto3_resource_groups/literals.py` & `mypy-boto3-resource-groups-1.28.16/mypy_boto3_resource_groups/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-resource-groups-1.28.15.post1/mypy_boto3_resource_groups/literals.pyi` & `mypy-boto3-resource-groups-1.28.16/mypy_boto3_resource_groups/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-resource-groups-1.28.15.post1/mypy_boto3_resource_groups/paginator.py` & `mypy-boto3-resource-groups-1.28.16/mypy_boto3_resource_groups/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-resource-groups-1.28.15.post1/mypy_boto3_resource_groups/paginator.pyi` & `mypy-boto3-resource-groups-1.28.16/mypy_boto3_resource_groups/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-resource-groups-1.28.15.post1/mypy_boto3_resource_groups/type_defs.py` & `mypy-boto3-resource-groups-1.28.16/mypy_boto3_resource_groups/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_groups/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_resource_groups.type_defs import AccountSettingsTypeDef
 
-    data: AccountSettingsTypeDef = {...}
+    data: AccountSettingsTypeDef = ...
     ```
 """
 import sys
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     GroupConfigurationStatusType,
@@ -82,19 +82,20 @@
     "ListGroupResourcesInputListGroupResourcesPaginateTypeDef",
     "ListGroupResourcesInputRequestTypeDef",
     "ListGroupResourcesItemTypeDef",
     "SearchResourcesOutputTypeDef",
     "GetGroupQueryOutputTypeDef",
     "UpdateGroupQueryOutputTypeDef",
     "GroupConfigurationTypeDef",
-    "CreateGroupInputRequestTypeDef",
-    "PutGroupConfigurationInputRequestTypeDef",
+    "GroupConfigurationItemUnionTypeDef",
     "ListGroupResourcesOutputTypeDef",
     "CreateGroupOutputTypeDef",
     "GetGroupConfigurationOutputTypeDef",
+    "CreateGroupInputRequestTypeDef",
+    "PutGroupConfigurationInputRequestTypeDef",
 )
 
 AccountSettingsTypeDef = TypedDict(
     "AccountSettingsTypeDef",
     {
         "GroupLifecycleEventsDesiredStatus": GroupLifecycleEventsDesiredStatusType,
         "GroupLifecycleEventsStatus": GroupLifecycleEventsStatusType,
@@ -653,29 +654,60 @@
         "ProposedConfiguration": List[GroupConfigurationItemOutputTypeDef],
         "Status": GroupConfigurationStatusType,
         "FailureReason": str,
     },
     total=False,
 )
 
+GroupConfigurationItemUnionTypeDef = Union[
+    GroupConfigurationItemTypeDef, GroupConfigurationItemOutputTypeDef
+]
+ListGroupResourcesOutputTypeDef = TypedDict(
+    "ListGroupResourcesOutputTypeDef",
+    {
+        "Resources": List[ListGroupResourcesItemTypeDef],
+        "ResourceIdentifiers": List[ResourceIdentifierTypeDef],
+        "NextToken": str,
+        "QueryErrors": List[QueryErrorTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateGroupOutputTypeDef = TypedDict(
+    "CreateGroupOutputTypeDef",
+    {
+        "Group": GroupTypeDef,
+        "ResourceQuery": ResourceQueryTypeDef,
+        "Tags": Dict[str, str],
+        "GroupConfiguration": GroupConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetGroupConfigurationOutputTypeDef = TypedDict(
+    "GetGroupConfigurationOutputTypeDef",
+    {
+        "GroupConfiguration": GroupConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateGroupInputRequestTypeDef = TypedDict(
     "_RequiredCreateGroupInputRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalCreateGroupInputRequestTypeDef = TypedDict(
     "_OptionalCreateGroupInputRequestTypeDef",
     {
         "Description": str,
         "ResourceQuery": ResourceQueryTypeDef,
         "Tags": Mapping[str, str],
-        "Configuration": Sequence[
-            Union[GroupConfigurationItemTypeDef, GroupConfigurationItemOutputTypeDef]
-        ],
+        "Configuration": Sequence[GroupConfigurationItemUnionTypeDef],
     },
     total=False,
 )
 
 
 class CreateGroupInputRequestTypeDef(
     _RequiredCreateGroupInputRequestTypeDef, _OptionalCreateGroupInputRequestTypeDef
@@ -683,43 +715,11 @@
     pass
 
 
 PutGroupConfigurationInputRequestTypeDef = TypedDict(
     "PutGroupConfigurationInputRequestTypeDef",
     {
         "Group": str,
-        "Configuration": Sequence[
-            Union[GroupConfigurationItemTypeDef, GroupConfigurationItemOutputTypeDef]
-        ],
+        "Configuration": Sequence[GroupConfigurationItemUnionTypeDef],
     },
     total=False,
 )
-
-ListGroupResourcesOutputTypeDef = TypedDict(
-    "ListGroupResourcesOutputTypeDef",
-    {
-        "Resources": List[ListGroupResourcesItemTypeDef],
-        "ResourceIdentifiers": List[ResourceIdentifierTypeDef],
-        "NextToken": str,
-        "QueryErrors": List[QueryErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateGroupOutputTypeDef = TypedDict(
-    "CreateGroupOutputTypeDef",
-    {
-        "Group": GroupTypeDef,
-        "ResourceQuery": ResourceQueryTypeDef,
-        "Tags": Dict[str, str],
-        "GroupConfiguration": GroupConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetGroupConfigurationOutputTypeDef = TypedDict(
-    "GetGroupConfigurationOutputTypeDef",
-    {
-        "GroupConfiguration": GroupConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
```

### Comparing `mypy-boto3-resource-groups-1.28.15.post1/mypy_boto3_resource_groups/type_defs.pyi` & `mypy-boto3-resource-groups-1.28.16/mypy_boto3_resource_groups/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_groups/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_resource_groups.type_defs import AccountSettingsTypeDef
 
-    data: AccountSettingsTypeDef = {...}
+    data: AccountSettingsTypeDef = ...
     ```
 """
 import sys
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     GroupConfigurationStatusType,
@@ -81,19 +81,20 @@
     "ListGroupResourcesInputListGroupResourcesPaginateTypeDef",
     "ListGroupResourcesInputRequestTypeDef",
     "ListGroupResourcesItemTypeDef",
     "SearchResourcesOutputTypeDef",
     "GetGroupQueryOutputTypeDef",
     "UpdateGroupQueryOutputTypeDef",
     "GroupConfigurationTypeDef",
-    "CreateGroupInputRequestTypeDef",
-    "PutGroupConfigurationInputRequestTypeDef",
+    "GroupConfigurationItemUnionTypeDef",
     "ListGroupResourcesOutputTypeDef",
     "CreateGroupOutputTypeDef",
     "GetGroupConfigurationOutputTypeDef",
+    "CreateGroupInputRequestTypeDef",
+    "PutGroupConfigurationInputRequestTypeDef",
 )
 
 AccountSettingsTypeDef = TypedDict(
     "AccountSettingsTypeDef",
     {
         "GroupLifecycleEventsDesiredStatus": GroupLifecycleEventsDesiredStatusType,
         "GroupLifecycleEventsStatus": GroupLifecycleEventsStatusType,
@@ -636,49 +637,17 @@
         "ProposedConfiguration": List[GroupConfigurationItemOutputTypeDef],
         "Status": GroupConfigurationStatusType,
         "FailureReason": str,
     },
     total=False,
 )
 
-_RequiredCreateGroupInputRequestTypeDef = TypedDict(
-    "_RequiredCreateGroupInputRequestTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalCreateGroupInputRequestTypeDef = TypedDict(
-    "_OptionalCreateGroupInputRequestTypeDef",
-    {
-        "Description": str,
-        "ResourceQuery": ResourceQueryTypeDef,
-        "Tags": Mapping[str, str],
-        "Configuration": Sequence[
-            Union[GroupConfigurationItemTypeDef, GroupConfigurationItemOutputTypeDef]
-        ],
-    },
-    total=False,
-)
-
-class CreateGroupInputRequestTypeDef(
-    _RequiredCreateGroupInputRequestTypeDef, _OptionalCreateGroupInputRequestTypeDef
-):
-    pass
-
-PutGroupConfigurationInputRequestTypeDef = TypedDict(
-    "PutGroupConfigurationInputRequestTypeDef",
-    {
-        "Group": str,
-        "Configuration": Sequence[
-            Union[GroupConfigurationItemTypeDef, GroupConfigurationItemOutputTypeDef]
-        ],
-    },
-    total=False,
-)
-
+GroupConfigurationItemUnionTypeDef = Union[
+    GroupConfigurationItemTypeDef, GroupConfigurationItemOutputTypeDef
+]
 ListGroupResourcesOutputTypeDef = TypedDict(
     "ListGroupResourcesOutputTypeDef",
     {
         "Resources": List[ListGroupResourcesItemTypeDef],
         "ResourceIdentifiers": List[ResourceIdentifierTypeDef],
         "NextToken": str,
         "QueryErrors": List[QueryErrorTypeDef],
@@ -700,7 +669,38 @@
 GetGroupConfigurationOutputTypeDef = TypedDict(
     "GetGroupConfigurationOutputTypeDef",
     {
         "GroupConfiguration": GroupConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+
+_RequiredCreateGroupInputRequestTypeDef = TypedDict(
+    "_RequiredCreateGroupInputRequestTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalCreateGroupInputRequestTypeDef = TypedDict(
+    "_OptionalCreateGroupInputRequestTypeDef",
+    {
+        "Description": str,
+        "ResourceQuery": ResourceQueryTypeDef,
+        "Tags": Mapping[str, str],
+        "Configuration": Sequence[GroupConfigurationItemUnionTypeDef],
+    },
+    total=False,
+)
+
+class CreateGroupInputRequestTypeDef(
+    _RequiredCreateGroupInputRequestTypeDef, _OptionalCreateGroupInputRequestTypeDef
+):
+    pass
+
+PutGroupConfigurationInputRequestTypeDef = TypedDict(
+    "PutGroupConfigurationInputRequestTypeDef",
+    {
+        "Group": str,
+        "Configuration": Sequence[GroupConfigurationItemUnionTypeDef],
+    },
+    total=False,
+)
```

### Comparing `mypy-boto3-resource-groups-1.28.15.post1/mypy_boto3_resource_groups.egg-info/PKG-INFO` & `mypy-boto3-resource-groups-1.28.16/mypy_boto3_resource_groups.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-resource-groups
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.ResourceGroups 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.ResourceGroups 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_groups/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 resource-groups type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 resource-groups type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-resource-groups.svg?color=blue)](https://pypi.org/project/mypy-boto3-resource-groups)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_groups/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-resource-groups)](https://pepy.tech/project/mypy-boto3-resource-groups)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ResourceGroups 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups)
+[boto3.ResourceGroups 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups)
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
 [mypy-boto3-resource-groups docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_groups/).
 
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
@@ -329,20 +329,20 @@
 )
 
 
 def check_value(value: GroupConfigurationStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_resource_groups.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_resource_groups.type_defs import (
     AccountSettingsTypeDef,
     ResourceQueryTypeDef,
     GroupTypeDef,
     ResponseMetadataTypeDef,
@@ -390,23 +390,24 @@
     ListGroupResourcesInputListGroupResourcesPaginateTypeDef,
     ListGroupResourcesInputRequestTypeDef,
     ListGroupResourcesItemTypeDef,
     SearchResourcesOutputTypeDef,
     GetGroupQueryOutputTypeDef,
     UpdateGroupQueryOutputTypeDef,
     GroupConfigurationTypeDef,
-    CreateGroupInputRequestTypeDef,
-    PutGroupConfigurationInputRequestTypeDef,
+    GroupConfigurationItemUnionTypeDef,
     ListGroupResourcesOutputTypeDef,
     CreateGroupOutputTypeDef,
     GetGroupConfigurationOutputTypeDef,
+    CreateGroupInputRequestTypeDef,
+    PutGroupConfigurationInputRequestTypeDef,
 )
 
 
-def get_structure() -> AccountSettingsTypeDef:
+def get_value() -> AccountSettingsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-resource-groups-1.28.15.post1/mypy_boto3_resource_groups.egg-info/SOURCES.txt` & `mypy-boto3-resource-groups-1.28.16/mypy_boto3_resource_groups.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-resource-groups-1.28.15.post1/setup.py` & `mypy-boto3-resource-groups-1.28.16/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-resource-groups",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_resource_groups"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ResourceGroups 1.28.15 service generated with"
-        " mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.ResourceGroups 1.28.16 service generated with"
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
-    keywords="boto3 resource-groups type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 resource-groups type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_resource_groups": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_groups/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

