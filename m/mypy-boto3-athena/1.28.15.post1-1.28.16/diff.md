# Comparing `tmp/mypy-boto3-athena-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-athena-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-athena-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:34 2023, max compression
+gzip compressed data, was "mypy-boto3-athena-1.28.16.tar", last modified: Tue Aug  1 11:36:15 2023, max compression
```

## Comparing `mypy-boto3-athena-1.28.15.post1.tar` & `mypy-boto3-athena-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:34.381021 mypy-boto3-athena-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:38:38.000000 mypy-boto3-athena-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20983 2023-07-29 10:02:34.377021 mypy-boto3-athena-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19494 2023-07-29 09:38:38.000000 mypy-boto3-athena-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:34.373021 mypy-boto3-athena-1.28.15.post1/mypy_boto3_athena/
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-07-29 09:38:38.000000 mypy-boto3-athena-1.28.15.post1/mypy_boto3_athena/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-07-29 09:38:38.000000 mypy-boto3-athena-1.28.15.post1/mypy_boto3_athena/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-29 09:38:38.000000 mypy-boto3-athena-1.28.15.post1/mypy_boto3_athena/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    46302 2023-07-29 09:38:38.000000 mypy-boto3-athena-1.28.15.post1/mypy_boto3_athena/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    46220 2023-07-29 09:38:38.000000 mypy-boto3-athena-1.28.15.post1/mypy_boto3_athena/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10516 2023-07-29 09:38:39.000000 mypy-boto3-athena-1.28.15.post1/mypy_boto3_athena/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10514 2023-07-29 09:38:39.000000 mypy-boto3-athena-1.28.15.post1/mypy_boto3_athena/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8255 2023-07-29 09:38:38.000000 mypy-boto3-athena-1.28.15.post1/mypy_boto3_athena/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8246 2023-07-29 09:38:38.000000 mypy-boto3-athena-1.28.15.post1/mypy_boto3_athena/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:38:38.000000 mypy-boto3-athena-1.28.15.post1/mypy_boto3_athena/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    63618 2023-07-29 09:38:42.000000 mypy-boto3-athena-1.28.15.post1/mypy_boto3_athena/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    63527 2023-07-29 09:38:41.000000 mypy-boto3-athena-1.28.15.post1/mypy_boto3_athena/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:38:38.000000 mypy-boto3-athena-1.28.15.post1/mypy_boto3_athena/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:34.377021 mypy-boto3-athena-1.28.15.post1/mypy_boto3_athena.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20983 2023-07-29 10:02:34.000000 mypy-boto3-athena-1.28.15.post1/mypy_boto3_athena.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-29 10:02:34.000000 mypy-boto3-athena-1.28.15.post1/mypy_boto3_athena.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:34.000000 mypy-boto3-athena-1.28.15.post1/mypy_boto3_athena.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:34.000000 mypy-boto3-athena-1.28.15.post1/mypy_boto3_athena.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:34.000000 mypy-boto3-athena-1.28.15.post1/mypy_boto3_athena.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-29 10:02:34.000000 mypy-boto3-athena-1.28.15.post1/mypy_boto3_athena.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:34.381021 mypy-boto3-athena-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-29 09:38:38.000000 mypy-boto3-athena-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:15.252945 mypy-boto3-athena-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:11:10.000000 mypy-boto3-athena-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21046 2023-08-01 11:36:15.244945 mypy-boto3-athena-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19566 2023-08-01 11:11:10.000000 mypy-boto3-athena-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:15.236945 mypy-boto3-athena-1.28.16/mypy_boto3_athena/
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-08-01 11:11:10.000000 mypy-boto3-athena-1.28.16/mypy_boto3_athena/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-08-01 11:11:10.000000 mypy-boto3-athena-1.28.16/mypy_boto3_athena/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-08-01 11:11:10.000000 mypy-boto3-athena-1.28.16/mypy_boto3_athena/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46137 2023-08-01 11:11:11.000000 mypy-boto3-athena-1.28.16/mypy_boto3_athena/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46055 2023-08-01 11:11:10.000000 mypy-boto3-athena-1.28.16/mypy_boto3_athena/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10516 2023-08-01 11:11:11.000000 mypy-boto3-athena-1.28.16/mypy_boto3_athena/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10514 2023-08-01 11:11:11.000000 mypy-boto3-athena-1.28.16/mypy_boto3_athena/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8255 2023-08-01 11:11:11.000000 mypy-boto3-athena-1.28.16/mypy_boto3_athena/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8246 2023-08-01 11:11:11.000000 mypy-boto3-athena-1.28.16/mypy_boto3_athena/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:11:10.000000 mypy-boto3-athena-1.28.16/mypy_boto3_athena/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    63843 2023-08-01 11:11:13.000000 mypy-boto3-athena-1.28.16/mypy_boto3_athena/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63752 2023-08-01 11:11:12.000000 mypy-boto3-athena-1.28.16/mypy_boto3_athena/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:11:10.000000 mypy-boto3-athena-1.28.16/mypy_boto3_athena/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:15.244945 mypy-boto3-athena-1.28.16/mypy_boto3_athena.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21046 2023-08-01 11:36:14.000000 mypy-boto3-athena-1.28.16/mypy_boto3_athena.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-08-01 11:36:15.000000 mypy-boto3-athena-1.28.16/mypy_boto3_athena.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:14.000000 mypy-boto3-athena-1.28.16/mypy_boto3_athena.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:14.000000 mypy-boto3-athena-1.28.16/mypy_boto3_athena.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:14.000000 mypy-boto3-athena-1.28.16/mypy_boto3_athena.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-01 11:36:14.000000 mypy-boto3-athena-1.28.16/mypy_boto3_athena.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:15.252945 mypy-boto3-athena-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-08-01 11:11:10.000000 mypy-boto3-athena-1.28.16/setup.py
```

### Comparing `mypy-boto3-athena-1.28.15.post1/LICENSE` & `mypy-boto3-athena-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-athena-1.28.15.post1/PKG-INFO` & `mypy-boto3-athena-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-athena
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.Athena 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.Athena 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 athena type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 athena type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-athena.svg?color=blue)](https://pypi.org/project/mypy-boto3-athena)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-athena)](https://pepy.tech/project/mypy-boto3-athena)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Athena 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena)
+[boto3.Athena 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena)
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
 [mypy-boto3-athena docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/).
 
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
 
 
 def check_value(value: CalculationExecutionStateType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_athena.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_athena.type_defs import (
     AclConfigurationTypeDef,
     ApplicationDPUSizesTypeDef,
     AthenaErrorTypeDef,
     BatchGetNamedQueryInputRequestTypeDef,
@@ -483,29 +483,30 @@
     BatchGetPreparedStatementOutputTypeDef,
     StartCalculationExecutionRequestRequestTypeDef,
     CalculationSummaryTypeDef,
     GetCalculationExecutionResponseTypeDef,
     GetCalculationExecutionStatusResponseTypeDef,
     CapacityReservationTypeDef,
     CapacityAssignmentConfigurationTypeDef,
-    PutCapacityAssignmentConfigurationInputRequestTypeDef,
+    CapacityAssignmentUnionTypeDef,
     ResultSetMetadataTypeDef,
     TableMetadataTypeDef,
     CreateCapacityReservationInputRequestTypeDef,
     CreateDataCatalogInputRequestTypeDef,
     ListTagsForResourceOutputTypeDef,
     TagResourceInputRequestTypeDef,
     ListDataCatalogsOutputTypeDef,
     GetDataCatalogOutputTypeDef,
     GetDatabaseOutputTypeDef,
     ListDatabasesOutputTypeDef,
     RowTypeDef,
     ResultConfigurationTypeDef,
     ResultConfigurationUpdatesTypeDef,
     SessionConfigurationTypeDef,
+    EngineConfigurationUnionTypeDef,
     StartSessionRequestRequestTypeDef,
     ListEngineVersionsOutputTypeDef,
     WorkGroupSummaryTypeDef,
     ListExecutorsResponseTypeDef,
     ExportNotebookOutputTypeDef,
     GetNotebookMetadataOutputTypeDef,
     ListNotebookMetadataOutputTypeDef,
@@ -524,14 +525,15 @@
     QueryExecutionStatisticsTypeDef,
     QueryRuntimeStatisticsTypeDef,
     ResultReuseConfigurationTypeDef,
     ListCalculationExecutionsResponseTypeDef,
     GetCapacityReservationOutputTypeDef,
     ListCapacityReservationsOutputTypeDef,
     GetCapacityAssignmentConfigurationOutputTypeDef,
+    PutCapacityAssignmentConfigurationInputRequestTypeDef,
     GetTableMetadataOutputTypeDef,
     ListTableMetadataOutputTypeDef,
     ResultSetTypeDef,
     WorkGroupConfigurationTypeDef,
     WorkGroupConfigurationUpdatesTypeDef,
     GetSessionResponseTypeDef,
     ListWorkGroupsOutputTypeDef,
@@ -545,15 +547,15 @@
     UpdateWorkGroupInputRequestTypeDef,
     BatchGetQueryExecutionOutputTypeDef,
     GetQueryExecutionOutputTypeDef,
     GetWorkGroupOutputTypeDef,
 )
 
 
-def get_structure() -> AclConfigurationTypeDef:
+def get_value() -> AclConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-athena-1.28.15.post1/README.md` & `mypy-boto3-athena-1.28.16/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-athena.svg?color=blue)](https://pypi.org/project/mypy-boto3-athena)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-athena)](https://pepy.tech/project/mypy-boto3-athena)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Athena 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena)
+[boto3.Athena 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena)
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
 [mypy-boto3-athena docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/).
 
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
 
 
 def check_value(value: CalculationExecutionStateType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_athena.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_athena.type_defs import (
     AclConfigurationTypeDef,
     ApplicationDPUSizesTypeDef,
     AthenaErrorTypeDef,
     BatchGetNamedQueryInputRequestTypeDef,
@@ -451,29 +451,30 @@
     BatchGetPreparedStatementOutputTypeDef,
     StartCalculationExecutionRequestRequestTypeDef,
     CalculationSummaryTypeDef,
     GetCalculationExecutionResponseTypeDef,
     GetCalculationExecutionStatusResponseTypeDef,
     CapacityReservationTypeDef,
     CapacityAssignmentConfigurationTypeDef,
-    PutCapacityAssignmentConfigurationInputRequestTypeDef,
+    CapacityAssignmentUnionTypeDef,
     ResultSetMetadataTypeDef,
     TableMetadataTypeDef,
     CreateCapacityReservationInputRequestTypeDef,
     CreateDataCatalogInputRequestTypeDef,
     ListTagsForResourceOutputTypeDef,
     TagResourceInputRequestTypeDef,
     ListDataCatalogsOutputTypeDef,
     GetDataCatalogOutputTypeDef,
     GetDatabaseOutputTypeDef,
     ListDatabasesOutputTypeDef,
     RowTypeDef,
     ResultConfigurationTypeDef,
     ResultConfigurationUpdatesTypeDef,
     SessionConfigurationTypeDef,
+    EngineConfigurationUnionTypeDef,
     StartSessionRequestRequestTypeDef,
     ListEngineVersionsOutputTypeDef,
     WorkGroupSummaryTypeDef,
     ListExecutorsResponseTypeDef,
     ExportNotebookOutputTypeDef,
     GetNotebookMetadataOutputTypeDef,
     ListNotebookMetadataOutputTypeDef,
@@ -492,14 +493,15 @@
     QueryExecutionStatisticsTypeDef,
     QueryRuntimeStatisticsTypeDef,
     ResultReuseConfigurationTypeDef,
     ListCalculationExecutionsResponseTypeDef,
     GetCapacityReservationOutputTypeDef,
     ListCapacityReservationsOutputTypeDef,
     GetCapacityAssignmentConfigurationOutputTypeDef,
+    PutCapacityAssignmentConfigurationInputRequestTypeDef,
     GetTableMetadataOutputTypeDef,
     ListTableMetadataOutputTypeDef,
     ResultSetTypeDef,
     WorkGroupConfigurationTypeDef,
     WorkGroupConfigurationUpdatesTypeDef,
     GetSessionResponseTypeDef,
     ListWorkGroupsOutputTypeDef,
@@ -513,15 +515,15 @@
     UpdateWorkGroupInputRequestTypeDef,
     BatchGetQueryExecutionOutputTypeDef,
     GetQueryExecutionOutputTypeDef,
     GetWorkGroupOutputTypeDef,
 )
 
 
-def get_structure() -> AclConfigurationTypeDef:
+def get_value() -> AclConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-athena-1.28.15.post1/mypy_boto3_athena/__init__.py` & `mypy-boto3-athena-1.28.16/mypy_boto3_athena/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-athena-1.28.15.post1/mypy_boto3_athena/__init__.pyi` & `mypy-boto3-athena-1.28.16/mypy_boto3_athena/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-athena-1.28.15.post1/mypy_boto3_athena/__main__.py` & `mypy-boto3-athena-1.28.16/mypy_boto3_athena/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Athena 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.Athena 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena\nOther"
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

### Comparing `mypy-boto3-athena-1.28.15.post1/mypy_boto3_athena/client.py` & `mypy-boto3-athena-1.28.16/mypy_boto3_athena/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_athena.client import AthenaClient
 
     session = Session()
     client: AthenaClient = session.client("athena")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     CalculationExecutionStateType,
     DataCatalogTypeType,
     ExecutorStateType,
@@ -35,21 +35,19 @@
     ListTagsForResourcePaginator,
 )
 from .type_defs import (
     BatchGetNamedQueryOutputTypeDef,
     BatchGetPreparedStatementOutputTypeDef,
     BatchGetQueryExecutionOutputTypeDef,
     CalculationConfigurationTypeDef,
-    CapacityAssignmentOutputTypeDef,
-    CapacityAssignmentTypeDef,
+    CapacityAssignmentUnionTypeDef,
     CreateNamedQueryOutputTypeDef,
     CreateNotebookOutputTypeDef,
     CreatePresignedNotebookUrlResponseTypeDef,
-    EngineConfigurationOutputTypeDef,
-    EngineConfigurationTypeDef,
+    EngineConfigurationUnionTypeDef,
     ExportNotebookOutputTypeDef,
     FilterDefinitionTypeDef,
     GetCalculationExecutionCodeResponseTypeDef,
     GetCalculationExecutionResponseTypeDef,
     GetCalculationExecutionStatusResponseTypeDef,
     GetCapacityAssignmentConfigurationOutputTypeDef,
     GetCapacityReservationOutputTypeDef,
@@ -726,17 +724,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#list_work_groups)
         """
 
     def put_capacity_assignment_configuration(
         self,
         *,
         CapacityReservationName: str,
-        CapacityAssignments: Sequence[
-            Union[CapacityAssignmentTypeDef, CapacityAssignmentOutputTypeDef]
-        ]
+        CapacityAssignments: Sequence[CapacityAssignmentUnionTypeDef]
     ) -> Dict[str, Any]:
         """
         Puts a new capacity assignment configuration for a specified capacity
         reservation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.put_capacity_assignment_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#put_capacity_assignment_configuration)
@@ -776,15 +772,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#start_query_execution)
         """
 
     def start_session(
         self,
         *,
         WorkGroup: str,
-        EngineConfiguration: Union[EngineConfigurationTypeDef, EngineConfigurationOutputTypeDef],
+        EngineConfiguration: EngineConfigurationUnionTypeDef,
         Description: str = ...,
         NotebookVersion: str = ...,
         SessionIdleTimeoutInMinutes: int = ...,
         ClientRequestToken: str = ...
     ) -> StartSessionResponseTypeDef:
         """
         Creates a session for running calculations within a workgroup.
```

### Comparing `mypy-boto3-athena-1.28.15.post1/mypy_boto3_athena/client.pyi` & `mypy-boto3-athena-1.28.16/mypy_boto3_athena/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_athena.client import AthenaClient
 
     session = Session()
     client: AthenaClient = session.client("athena")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     CalculationExecutionStateType,
     DataCatalogTypeType,
     ExecutorStateType,
@@ -35,21 +35,19 @@
     ListTagsForResourcePaginator,
 )
 from .type_defs import (
     BatchGetNamedQueryOutputTypeDef,
     BatchGetPreparedStatementOutputTypeDef,
     BatchGetQueryExecutionOutputTypeDef,
     CalculationConfigurationTypeDef,
-    CapacityAssignmentOutputTypeDef,
-    CapacityAssignmentTypeDef,
+    CapacityAssignmentUnionTypeDef,
     CreateNamedQueryOutputTypeDef,
     CreateNotebookOutputTypeDef,
     CreatePresignedNotebookUrlResponseTypeDef,
-    EngineConfigurationOutputTypeDef,
-    EngineConfigurationTypeDef,
+    EngineConfigurationUnionTypeDef,
     ExportNotebookOutputTypeDef,
     FilterDefinitionTypeDef,
     GetCalculationExecutionCodeResponseTypeDef,
     GetCalculationExecutionResponseTypeDef,
     GetCalculationExecutionStatusResponseTypeDef,
     GetCapacityAssignmentConfigurationOutputTypeDef,
     GetCapacityReservationOutputTypeDef,
@@ -666,17 +664,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.list_work_groups)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#list_work_groups)
         """
     def put_capacity_assignment_configuration(
         self,
         *,
         CapacityReservationName: str,
-        CapacityAssignments: Sequence[
-            Union[CapacityAssignmentTypeDef, CapacityAssignmentOutputTypeDef]
-        ]
+        CapacityAssignments: Sequence[CapacityAssignmentUnionTypeDef]
     ) -> Dict[str, Any]:
         """
         Puts a new capacity assignment configuration for a specified capacity
         reservation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.put_capacity_assignment_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#put_capacity_assignment_configuration)
@@ -713,15 +709,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.start_query_execution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#start_query_execution)
         """
     def start_session(
         self,
         *,
         WorkGroup: str,
-        EngineConfiguration: Union[EngineConfigurationTypeDef, EngineConfigurationOutputTypeDef],
+        EngineConfiguration: EngineConfigurationUnionTypeDef,
         Description: str = ...,
         NotebookVersion: str = ...,
         SessionIdleTimeoutInMinutes: int = ...,
         ClientRequestToken: str = ...
     ) -> StartSessionResponseTypeDef:
         """
         Creates a session for running calculations within a workgroup.
```

### Comparing `mypy-boto3-athena-1.28.15.post1/mypy_boto3_athena/literals.py` & `mypy-boto3-athena-1.28.16/mypy_boto3_athena/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-athena-1.28.15.post1/mypy_boto3_athena/literals.pyi` & `mypy-boto3-athena-1.28.16/mypy_boto3_athena/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-athena-1.28.15.post1/mypy_boto3_athena/paginator.py` & `mypy-boto3-athena-1.28.16/mypy_boto3_athena/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-athena-1.28.15.post1/mypy_boto3_athena/paginator.pyi` & `mypy-boto3-athena-1.28.16/mypy_boto3_athena/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-athena-1.28.15.post1/mypy_boto3_athena/type_defs.py` & `mypy-boto3-athena-1.28.16/mypy_boto3_athena/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_athena.type_defs import AclConfigurationTypeDef
 
-    data: AclConfigurationTypeDef = {...}
+    data: AclConfigurationTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -162,29 +162,30 @@
     "BatchGetPreparedStatementOutputTypeDef",
     "StartCalculationExecutionRequestRequestTypeDef",
     "CalculationSummaryTypeDef",
     "GetCalculationExecutionResponseTypeDef",
     "GetCalculationExecutionStatusResponseTypeDef",
     "CapacityReservationTypeDef",
     "CapacityAssignmentConfigurationTypeDef",
-    "PutCapacityAssignmentConfigurationInputRequestTypeDef",
+    "CapacityAssignmentUnionTypeDef",
     "ResultSetMetadataTypeDef",
     "TableMetadataTypeDef",
     "CreateCapacityReservationInputRequestTypeDef",
     "CreateDataCatalogInputRequestTypeDef",
     "ListTagsForResourceOutputTypeDef",
     "TagResourceInputRequestTypeDef",
     "ListDataCatalogsOutputTypeDef",
     "GetDataCatalogOutputTypeDef",
     "GetDatabaseOutputTypeDef",
     "ListDatabasesOutputTypeDef",
     "RowTypeDef",
     "ResultConfigurationTypeDef",
     "ResultConfigurationUpdatesTypeDef",
     "SessionConfigurationTypeDef",
+    "EngineConfigurationUnionTypeDef",
     "StartSessionRequestRequestTypeDef",
     "ListEngineVersionsOutputTypeDef",
     "WorkGroupSummaryTypeDef",
     "ListExecutorsResponseTypeDef",
     "ExportNotebookOutputTypeDef",
     "GetNotebookMetadataOutputTypeDef",
     "ListNotebookMetadataOutputTypeDef",
@@ -203,14 +204,15 @@
     "QueryExecutionStatisticsTypeDef",
     "QueryRuntimeStatisticsTypeDef",
     "ResultReuseConfigurationTypeDef",
     "ListCalculationExecutionsResponseTypeDef",
     "GetCapacityReservationOutputTypeDef",
     "ListCapacityReservationsOutputTypeDef",
     "GetCapacityAssignmentConfigurationOutputTypeDef",
+    "PutCapacityAssignmentConfigurationInputRequestTypeDef",
     "GetTableMetadataOutputTypeDef",
     "ListTableMetadataOutputTypeDef",
     "ResultSetTypeDef",
     "WorkGroupConfigurationTypeDef",
     "WorkGroupConfigurationUpdatesTypeDef",
     "GetSessionResponseTypeDef",
     "ListWorkGroupsOutputTypeDef",
@@ -1769,24 +1771,15 @@
     {
         "CapacityReservationName": str,
         "CapacityAssignments": List[CapacityAssignmentOutputTypeDef],
     },
     total=False,
 )
 
-PutCapacityAssignmentConfigurationInputRequestTypeDef = TypedDict(
-    "PutCapacityAssignmentConfigurationInputRequestTypeDef",
-    {
-        "CapacityReservationName": str,
-        "CapacityAssignments": Sequence[
-            Union[CapacityAssignmentTypeDef, CapacityAssignmentOutputTypeDef]
-        ],
-    },
-)
-
+CapacityAssignmentUnionTypeDef = Union[CapacityAssignmentTypeDef, CapacityAssignmentOutputTypeDef]
 ResultSetMetadataTypeDef = TypedDict(
     "ResultSetMetadataTypeDef",
     {
         "ColumnInfo": List[ColumnInfoTypeDef],
     },
     total=False,
 )
@@ -1954,14 +1947,17 @@
         "WorkingDirectory": str,
         "IdleTimeoutSeconds": int,
         "EncryptionConfiguration": EncryptionConfigurationTypeDef,
     },
     total=False,
 )
 
+EngineConfigurationUnionTypeDef = Union[
+    EngineConfigurationTypeDef, EngineConfigurationOutputTypeDef
+]
 _RequiredStartSessionRequestRequestTypeDef = TypedDict(
     "_RequiredStartSessionRequestRequestTypeDef",
     {
         "WorkGroup": str,
         "EngineConfiguration": EngineConfigurationTypeDef,
     },
 )
@@ -2282,14 +2278,22 @@
     "GetCapacityAssignmentConfigurationOutputTypeDef",
     {
         "CapacityAssignmentConfiguration": CapacityAssignmentConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+PutCapacityAssignmentConfigurationInputRequestTypeDef = TypedDict(
+    "PutCapacityAssignmentConfigurationInputRequestTypeDef",
+    {
+        "CapacityReservationName": str,
+        "CapacityAssignments": Sequence[CapacityAssignmentUnionTypeDef],
+    },
+)
+
 GetTableMetadataOutputTypeDef = TypedDict(
     "GetTableMetadataOutputTypeDef",
     {
         "TableMetadata": TableMetadataTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-athena-1.28.15.post1/mypy_boto3_athena/type_defs.pyi` & `mypy-boto3-athena-1.28.16/mypy_boto3_athena/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_athena.type_defs import AclConfigurationTypeDef
 
-    data: AclConfigurationTypeDef = {...}
+    data: AclConfigurationTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -161,29 +161,30 @@
     "BatchGetPreparedStatementOutputTypeDef",
     "StartCalculationExecutionRequestRequestTypeDef",
     "CalculationSummaryTypeDef",
     "GetCalculationExecutionResponseTypeDef",
     "GetCalculationExecutionStatusResponseTypeDef",
     "CapacityReservationTypeDef",
     "CapacityAssignmentConfigurationTypeDef",
-    "PutCapacityAssignmentConfigurationInputRequestTypeDef",
+    "CapacityAssignmentUnionTypeDef",
     "ResultSetMetadataTypeDef",
     "TableMetadataTypeDef",
     "CreateCapacityReservationInputRequestTypeDef",
     "CreateDataCatalogInputRequestTypeDef",
     "ListTagsForResourceOutputTypeDef",
     "TagResourceInputRequestTypeDef",
     "ListDataCatalogsOutputTypeDef",
     "GetDataCatalogOutputTypeDef",
     "GetDatabaseOutputTypeDef",
     "ListDatabasesOutputTypeDef",
     "RowTypeDef",
     "ResultConfigurationTypeDef",
     "ResultConfigurationUpdatesTypeDef",
     "SessionConfigurationTypeDef",
+    "EngineConfigurationUnionTypeDef",
     "StartSessionRequestRequestTypeDef",
     "ListEngineVersionsOutputTypeDef",
     "WorkGroupSummaryTypeDef",
     "ListExecutorsResponseTypeDef",
     "ExportNotebookOutputTypeDef",
     "GetNotebookMetadataOutputTypeDef",
     "ListNotebookMetadataOutputTypeDef",
@@ -202,14 +203,15 @@
     "QueryExecutionStatisticsTypeDef",
     "QueryRuntimeStatisticsTypeDef",
     "ResultReuseConfigurationTypeDef",
     "ListCalculationExecutionsResponseTypeDef",
     "GetCapacityReservationOutputTypeDef",
     "ListCapacityReservationsOutputTypeDef",
     "GetCapacityAssignmentConfigurationOutputTypeDef",
+    "PutCapacityAssignmentConfigurationInputRequestTypeDef",
     "GetTableMetadataOutputTypeDef",
     "ListTableMetadataOutputTypeDef",
     "ResultSetTypeDef",
     "WorkGroupConfigurationTypeDef",
     "WorkGroupConfigurationUpdatesTypeDef",
     "GetSessionResponseTypeDef",
     "ListWorkGroupsOutputTypeDef",
@@ -1704,24 +1706,15 @@
     {
         "CapacityReservationName": str,
         "CapacityAssignments": List[CapacityAssignmentOutputTypeDef],
     },
     total=False,
 )
 
-PutCapacityAssignmentConfigurationInputRequestTypeDef = TypedDict(
-    "PutCapacityAssignmentConfigurationInputRequestTypeDef",
-    {
-        "CapacityReservationName": str,
-        "CapacityAssignments": Sequence[
-            Union[CapacityAssignmentTypeDef, CapacityAssignmentOutputTypeDef]
-        ],
-    },
-)
-
+CapacityAssignmentUnionTypeDef = Union[CapacityAssignmentTypeDef, CapacityAssignmentOutputTypeDef]
 ResultSetMetadataTypeDef = TypedDict(
     "ResultSetMetadataTypeDef",
     {
         "ColumnInfo": List[ColumnInfoTypeDef],
     },
     total=False,
 )
@@ -1883,14 +1876,17 @@
         "WorkingDirectory": str,
         "IdleTimeoutSeconds": int,
         "EncryptionConfiguration": EncryptionConfigurationTypeDef,
     },
     total=False,
 )
 
+EngineConfigurationUnionTypeDef = Union[
+    EngineConfigurationTypeDef, EngineConfigurationOutputTypeDef
+]
 _RequiredStartSessionRequestRequestTypeDef = TypedDict(
     "_RequiredStartSessionRequestRequestTypeDef",
     {
         "WorkGroup": str,
         "EngineConfiguration": EngineConfigurationTypeDef,
     },
 )
@@ -2199,14 +2195,22 @@
     "GetCapacityAssignmentConfigurationOutputTypeDef",
     {
         "CapacityAssignmentConfiguration": CapacityAssignmentConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+PutCapacityAssignmentConfigurationInputRequestTypeDef = TypedDict(
+    "PutCapacityAssignmentConfigurationInputRequestTypeDef",
+    {
+        "CapacityReservationName": str,
+        "CapacityAssignments": Sequence[CapacityAssignmentUnionTypeDef],
+    },
+)
+
 GetTableMetadataOutputTypeDef = TypedDict(
     "GetTableMetadataOutputTypeDef",
     {
         "TableMetadata": TableMetadataTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-athena-1.28.15.post1/mypy_boto3_athena.egg-info/PKG-INFO` & `mypy-boto3-athena-1.28.16/mypy_boto3_athena.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-athena
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.Athena 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.Athena 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 athena type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 athena type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-athena.svg?color=blue)](https://pypi.org/project/mypy-boto3-athena)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-athena)](https://pepy.tech/project/mypy-boto3-athena)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Athena 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena)
+[boto3.Athena 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena)
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
 [mypy-boto3-athena docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/).
 
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
 
 
 def check_value(value: CalculationExecutionStateType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_athena.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_athena.type_defs import (
     AclConfigurationTypeDef,
     ApplicationDPUSizesTypeDef,
     AthenaErrorTypeDef,
     BatchGetNamedQueryInputRequestTypeDef,
@@ -483,29 +483,30 @@
     BatchGetPreparedStatementOutputTypeDef,
     StartCalculationExecutionRequestRequestTypeDef,
     CalculationSummaryTypeDef,
     GetCalculationExecutionResponseTypeDef,
     GetCalculationExecutionStatusResponseTypeDef,
     CapacityReservationTypeDef,
     CapacityAssignmentConfigurationTypeDef,
-    PutCapacityAssignmentConfigurationInputRequestTypeDef,
+    CapacityAssignmentUnionTypeDef,
     ResultSetMetadataTypeDef,
     TableMetadataTypeDef,
     CreateCapacityReservationInputRequestTypeDef,
     CreateDataCatalogInputRequestTypeDef,
     ListTagsForResourceOutputTypeDef,
     TagResourceInputRequestTypeDef,
     ListDataCatalogsOutputTypeDef,
     GetDataCatalogOutputTypeDef,
     GetDatabaseOutputTypeDef,
     ListDatabasesOutputTypeDef,
     RowTypeDef,
     ResultConfigurationTypeDef,
     ResultConfigurationUpdatesTypeDef,
     SessionConfigurationTypeDef,
+    EngineConfigurationUnionTypeDef,
     StartSessionRequestRequestTypeDef,
     ListEngineVersionsOutputTypeDef,
     WorkGroupSummaryTypeDef,
     ListExecutorsResponseTypeDef,
     ExportNotebookOutputTypeDef,
     GetNotebookMetadataOutputTypeDef,
     ListNotebookMetadataOutputTypeDef,
@@ -524,14 +525,15 @@
     QueryExecutionStatisticsTypeDef,
     QueryRuntimeStatisticsTypeDef,
     ResultReuseConfigurationTypeDef,
     ListCalculationExecutionsResponseTypeDef,
     GetCapacityReservationOutputTypeDef,
     ListCapacityReservationsOutputTypeDef,
     GetCapacityAssignmentConfigurationOutputTypeDef,
+    PutCapacityAssignmentConfigurationInputRequestTypeDef,
     GetTableMetadataOutputTypeDef,
     ListTableMetadataOutputTypeDef,
     ResultSetTypeDef,
     WorkGroupConfigurationTypeDef,
     WorkGroupConfigurationUpdatesTypeDef,
     GetSessionResponseTypeDef,
     ListWorkGroupsOutputTypeDef,
@@ -545,15 +547,15 @@
     UpdateWorkGroupInputRequestTypeDef,
     BatchGetQueryExecutionOutputTypeDef,
     GetQueryExecutionOutputTypeDef,
     GetWorkGroupOutputTypeDef,
 )
 
 
-def get_structure() -> AclConfigurationTypeDef:
+def get_value() -> AclConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-athena-1.28.15.post1/mypy_boto3_athena.egg-info/SOURCES.txt` & `mypy-boto3-athena-1.28.16/mypy_boto3_athena.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-athena-1.28.15.post1/setup.py` & `mypy-boto3-athena-1.28.16/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-athena",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_athena"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Athena 1.28.15 service generated with mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.Athena 1.28.16 service generated with mypy-boto3-builder 7.17.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
@@ -33,15 +33,15 @@
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
         "Typing :: Typed",
     ],
-    keywords="boto3 athena type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 athena type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_athena": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

