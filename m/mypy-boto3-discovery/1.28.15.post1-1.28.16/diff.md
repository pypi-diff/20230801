# Comparing `tmp/mypy-boto3-discovery-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-discovery-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-discovery-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:57 2023, max compression
+gzip compressed data, was "mypy-boto3-discovery-1.28.16.tar", last modified: Tue Aug  1 11:36:38 2023, max compression
```

## Comparing `mypy-boto3-discovery-1.28.15.post1.tar` & `mypy-boto3-discovery-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:57.853109 mypy-boto3-discovery-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:42:27.000000 mypy-boto3-discovery-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17092 2023-07-29 10:02:57.845109 mypy-boto3-discovery-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15573 2023-07-29 09:42:27.000000 mypy-boto3-discovery-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:57.837109 mypy-boto3-discovery-1.28.15.post1/mypy_boto3_discovery/
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-07-29 09:42:27.000000 mypy-boto3-discovery-1.28.15.post1/mypy_boto3_discovery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-07-29 09:42:27.000000 mypy-boto3-discovery-1.28.15.post1/mypy_boto3_discovery/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-29 09:42:27.000000 mypy-boto3-discovery-1.28.15.post1/mypy_boto3_discovery/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22908 2023-07-29 09:42:28.000000 mypy-boto3-discovery-1.28.15.post1/mypy_boto3_discovery/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    22870 2023-07-29 09:42:27.000000 mypy-boto3-discovery-1.28.15.post1/mypy_boto3_discovery/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10347 2023-07-29 09:42:28.000000 mypy-boto3-discovery-1.28.15.post1/mypy_boto3_discovery/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10345 2023-07-29 09:42:28.000000 mypy-boto3-discovery-1.28.15.post1/mypy_boto3_discovery/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8295 2023-07-29 09:42:28.000000 mypy-boto3-discovery-1.28.15.post1/mypy_boto3_discovery/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8287 2023-07-29 09:42:28.000000 mypy-boto3-discovery-1.28.15.post1/mypy_boto3_discovery/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:42:27.000000 mypy-boto3-discovery-1.28.15.post1/mypy_boto3_discovery/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    25129 2023-07-29 09:42:29.000000 mypy-boto3-discovery-1.28.15.post1/mypy_boto3_discovery/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    25108 2023-07-29 09:42:28.000000 mypy-boto3-discovery-1.28.15.post1/mypy_boto3_discovery/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:42:27.000000 mypy-boto3-discovery-1.28.15.post1/mypy_boto3_discovery/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:57.845109 mypy-boto3-discovery-1.28.15.post1/mypy_boto3_discovery.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17092 2023-07-29 10:02:57.000000 mypy-boto3-discovery-1.28.15.post1/mypy_boto3_discovery.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-29 10:02:57.000000 mypy-boto3-discovery-1.28.15.post1/mypy_boto3_discovery.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:57.000000 mypy-boto3-discovery-1.28.15.post1/mypy_boto3_discovery.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:57.000000 mypy-boto3-discovery-1.28.15.post1/mypy_boto3_discovery.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:57.000000 mypy-boto3-discovery-1.28.15.post1/mypy_boto3_discovery.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-29 10:02:57.000000 mypy-boto3-discovery-1.28.15.post1/mypy_boto3_discovery.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:57.853109 mypy-boto3-discovery-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-07-29 09:42:27.000000 mypy-boto3-discovery-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:38.500908 mypy-boto3-discovery-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:14:59.000000 mypy-boto3-discovery-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17104 2023-08-01 11:36:38.496908 mypy-boto3-discovery-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15594 2023-08-01 11:14:59.000000 mypy-boto3-discovery-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:38.484908 mypy-boto3-discovery-1.28.16/mypy_boto3_discovery/
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-08-01 11:14:59.000000 mypy-boto3-discovery-1.28.16/mypy_boto3_discovery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-08-01 11:14:59.000000 mypy-boto3-discovery-1.28.16/mypy_boto3_discovery/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-08-01 11:14:59.000000 mypy-boto3-discovery-1.28.16/mypy_boto3_discovery/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22885 2023-08-01 11:15:00.000000 mypy-boto3-discovery-1.28.16/mypy_boto3_discovery/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22847 2023-08-01 11:15:00.000000 mypy-boto3-discovery-1.28.16/mypy_boto3_discovery/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10347 2023-08-01 11:15:00.000000 mypy-boto3-discovery-1.28.16/mypy_boto3_discovery/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10345 2023-08-01 11:15:00.000000 mypy-boto3-discovery-1.28.16/mypy_boto3_discovery/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8295 2023-08-01 11:15:00.000000 mypy-boto3-discovery-1.28.16/mypy_boto3_discovery/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8287 2023-08-01 11:15:00.000000 mypy-boto3-discovery-1.28.16/mypy_boto3_discovery/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:14:59.000000 mypy-boto3-discovery-1.28.16/mypy_boto3_discovery/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    25183 2023-08-01 11:15:01.000000 mypy-boto3-discovery-1.28.16/mypy_boto3_discovery/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25162 2023-08-01 11:15:00.000000 mypy-boto3-discovery-1.28.16/mypy_boto3_discovery/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:14:59.000000 mypy-boto3-discovery-1.28.16/mypy_boto3_discovery/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:38.496908 mypy-boto3-discovery-1.28.16/mypy_boto3_discovery.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17104 2023-08-01 11:36:38.000000 mypy-boto3-discovery-1.28.16/mypy_boto3_discovery.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-08-01 11:36:38.000000 mypy-boto3-discovery-1.28.16/mypy_boto3_discovery.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:38.000000 mypy-boto3-discovery-1.28.16/mypy_boto3_discovery.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:38.000000 mypy-boto3-discovery-1.28.16/mypy_boto3_discovery.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:38.000000 mypy-boto3-discovery-1.28.16/mypy_boto3_discovery.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-01 11:36:38.000000 mypy-boto3-discovery-1.28.16/mypy_boto3_discovery.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:38.500908 mypy-boto3-discovery-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-08-01 11:14:59.000000 mypy-boto3-discovery-1.28.16/setup.py
```

### Comparing `mypy-boto3-discovery-1.28.15.post1/LICENSE` & `mypy-boto3-discovery-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-discovery-1.28.15.post1/PKG-INFO` & `mypy-boto3-discovery-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-discovery
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.ApplicationDiscoveryService 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.ApplicationDiscoveryService 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_discovery/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 discovery type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 discovery type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-discovery.svg?color=blue)](https://pypi.org/project/mypy-boto3-discovery)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_discovery/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-discovery)](https://pepy.tech/project/mypy-boto3-discovery)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ApplicationDiscoveryService 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService)
+[boto3.ApplicationDiscoveryService 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService)
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
 [mypy-boto3-discovery docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_discovery/).
 
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
@@ -349,20 +349,20 @@
 )
 
 
 def check_value(value: AgentStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_discovery.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_discovery.type_defs import (
     AgentConfigurationStatusTypeDef,
     AgentNetworkInfoTypeDef,
     AssociateConfigurationItemsToApplicationRequestRequestTypeDef,
     BatchDeleteImportDataErrorTypeDef,
@@ -390,14 +390,15 @@
     DisassociateConfigurationItemsFromApplicationRequestRequestTypeDef,
     ReservedInstanceOptionsTypeDef,
     UsageMetricBasisTypeDef,
     OrderByElementTypeDef,
     ListServerNeighborsRequestRequestTypeDef,
     NeighborConnectionDetailTypeDef,
     StartDataCollectionByAgentIdsRequestRequestTypeDef,
+    TimestampTypeDef,
     StartImportTaskRequestRequestTypeDef,
     StopContinuousExportRequestRequestTypeDef,
     StopDataCollectionByAgentIdsRequestRequestTypeDef,
     UpdateApplicationRequestRequestTypeDef,
     AgentInfoTypeDef,
     BatchDeleteImportDataResponseTypeDef,
     CreateApplicationResponseTypeDef,
@@ -433,15 +434,15 @@
     ListServerNeighborsResponseTypeDef,
     DescribeAgentsResponseTypeDef,
     ExportPreferencesTypeDef,
     StartExportTaskRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AgentConfigurationStatusTypeDef:
+def get_value() -> AgentConfigurationStatusTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-discovery-1.28.15.post1/README.md` & `mypy-boto3-discovery-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-discovery.svg?color=blue)](https://pypi.org/project/mypy-boto3-discovery)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_discovery/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-discovery)](https://pepy.tech/project/mypy-boto3-discovery)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ApplicationDiscoveryService 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService)
+[boto3.ApplicationDiscoveryService 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService)
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
 [mypy-boto3-discovery docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_discovery/).
 
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
@@ -317,20 +317,20 @@
 )
 
 
 def check_value(value: AgentStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_discovery.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_discovery.type_defs import (
     AgentConfigurationStatusTypeDef,
     AgentNetworkInfoTypeDef,
     AssociateConfigurationItemsToApplicationRequestRequestTypeDef,
     BatchDeleteImportDataErrorTypeDef,
@@ -358,14 +358,15 @@
     DisassociateConfigurationItemsFromApplicationRequestRequestTypeDef,
     ReservedInstanceOptionsTypeDef,
     UsageMetricBasisTypeDef,
     OrderByElementTypeDef,
     ListServerNeighborsRequestRequestTypeDef,
     NeighborConnectionDetailTypeDef,
     StartDataCollectionByAgentIdsRequestRequestTypeDef,
+    TimestampTypeDef,
     StartImportTaskRequestRequestTypeDef,
     StopContinuousExportRequestRequestTypeDef,
     StopDataCollectionByAgentIdsRequestRequestTypeDef,
     UpdateApplicationRequestRequestTypeDef,
     AgentInfoTypeDef,
     BatchDeleteImportDataResponseTypeDef,
     CreateApplicationResponseTypeDef,
@@ -401,15 +402,15 @@
     ListServerNeighborsResponseTypeDef,
     DescribeAgentsResponseTypeDef,
     ExportPreferencesTypeDef,
     StartExportTaskRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AgentConfigurationStatusTypeDef:
+def get_value() -> AgentConfigurationStatusTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-discovery-1.28.15.post1/mypy_boto3_discovery/__init__.py` & `mypy-boto3-discovery-1.28.16/mypy_boto3_discovery/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-discovery-1.28.15.post1/mypy_boto3_discovery/__init__.pyi` & `mypy-boto3-discovery-1.28.16/mypy_boto3_discovery/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-discovery-1.28.15.post1/mypy_boto3_discovery/__main__.py` & `mypy-boto3-discovery-1.28.16/mypy_boto3_discovery/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ApplicationDiscoveryService 1.28.15\nVersion:        "
-        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.ApplicationDiscoveryService 1.28.16\nVersion:        "
+        " 1.28.16\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_discovery//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService\nOther"
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

### Comparing `mypy-boto3-discovery-1.28.15.post1/mypy_boto3_discovery/client.py` & `mypy-boto3-discovery-1.28.16/mypy_boto3_discovery/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from mypy_boto3_discovery.client import ApplicationDiscoveryServiceClient
 
     session = Session()
     client: ApplicationDiscoveryServiceClient = session.client("discovery")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import ConfigurationItemTypeType
 from .paginator import (
     DescribeAgentsPaginator,
     DescribeContinuousExportsPaginator,
@@ -51,14 +50,15 @@
     StartDataCollectionByAgentIdsResponseTypeDef,
     StartExportTaskResponseTypeDef,
     StartImportTaskResponseTypeDef,
     StopContinuousExportResponseTypeDef,
     StopDataCollectionByAgentIdsResponseTypeDef,
     TagFilterTypeDef,
     TagTypeDef,
+    TimestampTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -361,16 +361,16 @@
         """
 
     def start_export_task(
         self,
         *,
         exportDataFormat: Sequence[Literal["CSV"]] = ...,
         filters: Sequence[ExportFilterTypeDef] = ...,
-        startTime: Union[datetime, str] = ...,
-        endTime: Union[datetime, str] = ...,
+        startTime: TimestampTypeDef = ...,
+        endTime: TimestampTypeDef = ...,
         preferences: ExportPreferencesTypeDef = ...
     ) -> StartExportTaskResponseTypeDef:
         """
         Begins the export of a discovered data report to an Amazon S3 bucket managed by
         Amazon Web Services.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService.Client.start_export_task)
```

### Comparing `mypy-boto3-discovery-1.28.15.post1/mypy_boto3_discovery/client.pyi` & `mypy-boto3-discovery-1.28.16/mypy_boto3_discovery/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from mypy_boto3_discovery.client import ApplicationDiscoveryServiceClient
 
     session = Session()
     client: ApplicationDiscoveryServiceClient = session.client("discovery")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import ConfigurationItemTypeType
 from .paginator import (
     DescribeAgentsPaginator,
     DescribeContinuousExportsPaginator,
@@ -51,14 +50,15 @@
     StartDataCollectionByAgentIdsResponseTypeDef,
     StartExportTaskResponseTypeDef,
     StartImportTaskResponseTypeDef,
     StopContinuousExportResponseTypeDef,
     StopDataCollectionByAgentIdsResponseTypeDef,
     TagFilterTypeDef,
     TagTypeDef,
+    TimestampTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -333,16 +333,16 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_discovery/client/#start_data_collection_by_agent_ids)
         """
     def start_export_task(
         self,
         *,
         exportDataFormat: Sequence[Literal["CSV"]] = ...,
         filters: Sequence[ExportFilterTypeDef] = ...,
-        startTime: Union[datetime, str] = ...,
-        endTime: Union[datetime, str] = ...,
+        startTime: TimestampTypeDef = ...,
+        endTime: TimestampTypeDef = ...,
         preferences: ExportPreferencesTypeDef = ...
     ) -> StartExportTaskResponseTypeDef:
         """
         Begins the export of a discovered data report to an Amazon S3 bucket managed by
         Amazon Web Services.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService.Client.start_export_task)
```

### Comparing `mypy-boto3-discovery-1.28.15.post1/mypy_boto3_discovery/literals.py` & `mypy-boto3-discovery-1.28.16/mypy_boto3_discovery/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-discovery-1.28.15.post1/mypy_boto3_discovery/literals.pyi` & `mypy-boto3-discovery-1.28.16/mypy_boto3_discovery/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-discovery-1.28.15.post1/mypy_boto3_discovery/paginator.py` & `mypy-boto3-discovery-1.28.16/mypy_boto3_discovery/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-discovery-1.28.15.post1/mypy_boto3_discovery/paginator.pyi` & `mypy-boto3-discovery-1.28.16/mypy_boto3_discovery/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-discovery-1.28.15.post1/mypy_boto3_discovery/type_defs.py` & `mypy-boto3-discovery-1.28.16/mypy_boto3_discovery/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_discovery/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_discovery.type_defs import AgentConfigurationStatusTypeDef
 
-    data: AgentConfigurationStatusTypeDef = {...}
+    data: AgentConfigurationStatusTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -69,14 +69,15 @@
     "DisassociateConfigurationItemsFromApplicationRequestRequestTypeDef",
     "ReservedInstanceOptionsTypeDef",
     "UsageMetricBasisTypeDef",
     "OrderByElementTypeDef",
     "ListServerNeighborsRequestRequestTypeDef",
     "NeighborConnectionDetailTypeDef",
     "StartDataCollectionByAgentIdsRequestRequestTypeDef",
+    "TimestampTypeDef",
     "StartImportTaskRequestRequestTypeDef",
     "StopContinuousExportRequestRequestTypeDef",
     "StopDataCollectionByAgentIdsRequestRequestTypeDef",
     "UpdateApplicationRequestRequestTypeDef",
     "AgentInfoTypeDef",
     "BatchDeleteImportDataResponseTypeDef",
     "CreateApplicationResponseTypeDef",
@@ -499,14 +500,15 @@
 StartDataCollectionByAgentIdsRequestRequestTypeDef = TypedDict(
     "StartDataCollectionByAgentIdsRequestRequestTypeDef",
     {
         "agentIds": Sequence[str],
     },
 )
 
+TimestampTypeDef = Union[datetime, str]
 _RequiredStartImportTaskRequestRequestTypeDef = TypedDict(
     "_RequiredStartImportTaskRequestRequestTypeDef",
     {
         "name": str,
         "importUrl": str,
     },
 )
@@ -941,13 +943,13 @@
 )
 
 StartExportTaskRequestRequestTypeDef = TypedDict(
     "StartExportTaskRequestRequestTypeDef",
     {
         "exportDataFormat": Sequence[Literal["CSV"]],
         "filters": Sequence[ExportFilterTypeDef],
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
         "preferences": ExportPreferencesTypeDef,
     },
     total=False,
 )
```

### Comparing `mypy-boto3-discovery-1.28.15.post1/mypy_boto3_discovery/type_defs.pyi` & `mypy-boto3-discovery-1.28.16/mypy_boto3_discovery/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_discovery/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_discovery.type_defs import AgentConfigurationStatusTypeDef
 
-    data: AgentConfigurationStatusTypeDef = {...}
+    data: AgentConfigurationStatusTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -68,14 +68,15 @@
     "DisassociateConfigurationItemsFromApplicationRequestRequestTypeDef",
     "ReservedInstanceOptionsTypeDef",
     "UsageMetricBasisTypeDef",
     "OrderByElementTypeDef",
     "ListServerNeighborsRequestRequestTypeDef",
     "NeighborConnectionDetailTypeDef",
     "StartDataCollectionByAgentIdsRequestRequestTypeDef",
+    "TimestampTypeDef",
     "StartImportTaskRequestRequestTypeDef",
     "StopContinuousExportRequestRequestTypeDef",
     "StopDataCollectionByAgentIdsRequestRequestTypeDef",
     "UpdateApplicationRequestRequestTypeDef",
     "AgentInfoTypeDef",
     "BatchDeleteImportDataResponseTypeDef",
     "CreateApplicationResponseTypeDef",
@@ -488,14 +489,15 @@
 StartDataCollectionByAgentIdsRequestRequestTypeDef = TypedDict(
     "StartDataCollectionByAgentIdsRequestRequestTypeDef",
     {
         "agentIds": Sequence[str],
     },
 )
 
+TimestampTypeDef = Union[datetime, str]
 _RequiredStartImportTaskRequestRequestTypeDef = TypedDict(
     "_RequiredStartImportTaskRequestRequestTypeDef",
     {
         "name": str,
         "importUrl": str,
     },
 )
@@ -920,13 +922,13 @@
 )
 
 StartExportTaskRequestRequestTypeDef = TypedDict(
     "StartExportTaskRequestRequestTypeDef",
     {
         "exportDataFormat": Sequence[Literal["CSV"]],
         "filters": Sequence[ExportFilterTypeDef],
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
         "preferences": ExportPreferencesTypeDef,
     },
     total=False,
 )
```

### Comparing `mypy-boto3-discovery-1.28.15.post1/mypy_boto3_discovery.egg-info/PKG-INFO` & `mypy-boto3-discovery-1.28.16/mypy_boto3_discovery.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-discovery
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.ApplicationDiscoveryService 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.ApplicationDiscoveryService 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_discovery/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 discovery type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 discovery type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-discovery.svg?color=blue)](https://pypi.org/project/mypy-boto3-discovery)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_discovery/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-discovery)](https://pepy.tech/project/mypy-boto3-discovery)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ApplicationDiscoveryService 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService)
+[boto3.ApplicationDiscoveryService 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService)
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
 [mypy-boto3-discovery docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_discovery/).
 
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
@@ -349,20 +349,20 @@
 )
 
 
 def check_value(value: AgentStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_discovery.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_discovery.type_defs import (
     AgentConfigurationStatusTypeDef,
     AgentNetworkInfoTypeDef,
     AssociateConfigurationItemsToApplicationRequestRequestTypeDef,
     BatchDeleteImportDataErrorTypeDef,
@@ -390,14 +390,15 @@
     DisassociateConfigurationItemsFromApplicationRequestRequestTypeDef,
     ReservedInstanceOptionsTypeDef,
     UsageMetricBasisTypeDef,
     OrderByElementTypeDef,
     ListServerNeighborsRequestRequestTypeDef,
     NeighborConnectionDetailTypeDef,
     StartDataCollectionByAgentIdsRequestRequestTypeDef,
+    TimestampTypeDef,
     StartImportTaskRequestRequestTypeDef,
     StopContinuousExportRequestRequestTypeDef,
     StopDataCollectionByAgentIdsRequestRequestTypeDef,
     UpdateApplicationRequestRequestTypeDef,
     AgentInfoTypeDef,
     BatchDeleteImportDataResponseTypeDef,
     CreateApplicationResponseTypeDef,
@@ -433,15 +434,15 @@
     ListServerNeighborsResponseTypeDef,
     DescribeAgentsResponseTypeDef,
     ExportPreferencesTypeDef,
     StartExportTaskRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AgentConfigurationStatusTypeDef:
+def get_value() -> AgentConfigurationStatusTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-discovery-1.28.15.post1/mypy_boto3_discovery.egg-info/SOURCES.txt` & `mypy-boto3-discovery-1.28.16/mypy_boto3_discovery.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-discovery-1.28.15.post1/setup.py` & `mypy-boto3-discovery-1.28.16/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-discovery",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_discovery"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ApplicationDiscoveryService 1.28.15 service generated with"
-        " mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.ApplicationDiscoveryService 1.28.16 service generated with"
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
-    keywords="boto3 discovery type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 discovery type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_discovery": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_discovery/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

