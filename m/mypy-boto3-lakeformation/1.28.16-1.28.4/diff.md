# Comparing `tmp/mypy-boto3-lakeformation-1.28.16.tar.gz` & `tmp/mypy-boto3-lakeformation-1.28.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-lakeformation-1.28.16.tar", last modified: Tue Aug  1 11:37:10 2023, max compression
+gzip compressed data, was "mypy-boto3-lakeformation-1.28.4.tar", last modified: Tue Jul 18 01:01:41 2023, max compression
```

## Comparing `mypy-boto3-lakeformation-1.28.16.tar` & `mypy-boto3-lakeformation-1.28.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:10.164844 mypy-boto3-lakeformation-1.28.16/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:21:54.000000 mypy-boto3-lakeformation-1.28.16/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19463 2023-08-01 11:37:10.160844 mypy-boto3-lakeformation-1.28.16/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17955 2023-08-01 11:21:54.000000 mypy-boto3-lakeformation-1.28.16/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:10.160844 mypy-boto3-lakeformation-1.28.16/mypy_boto3_lakeformation/
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-08-01 11:21:54.000000 mypy-boto3-lakeformation-1.28.16/mypy_boto3_lakeformation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-08-01 11:21:54.000000 mypy-boto3-lakeformation-1.28.16/mypy_boto3_lakeformation/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-08-01 11:21:54.000000 mypy-boto3-lakeformation-1.28.16/mypy_boto3_lakeformation/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37294 2023-08-01 11:21:54.000000 mypy-boto3-lakeformation-1.28.16/mypy_boto3_lakeformation/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    37235 2023-08-01 11:21:54.000000 mypy-boto3-lakeformation-1.28.16/mypy_boto3_lakeformation/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10499 2023-08-01 11:21:54.000000 mypy-boto3-lakeformation-1.28.16/mypy_boto3_lakeformation/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10497 2023-08-01 11:21:54.000000 mypy-boto3-lakeformation-1.28.16/mypy_boto3_lakeformation/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6773 2023-08-01 11:21:54.000000 mypy-boto3-lakeformation-1.28.16/mypy_boto3_lakeformation/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-08-01 11:21:54.000000 mypy-boto3-lakeformation-1.28.16/mypy_boto3_lakeformation/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:21:54.000000 mypy-boto3-lakeformation-1.28.16/mypy_boto3_lakeformation/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    55466 2023-08-01 11:21:56.000000 mypy-boto3-lakeformation-1.28.16/mypy_boto3_lakeformation/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    55368 2023-08-01 11:21:55.000000 mypy-boto3-lakeformation-1.28.16/mypy_boto3_lakeformation/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:21:54.000000 mypy-boto3-lakeformation-1.28.16/mypy_boto3_lakeformation/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:10.160844 mypy-boto3-lakeformation-1.28.16/mypy_boto3_lakeformation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19463 2023-08-01 11:37:09.000000 mypy-boto3-lakeformation-1.28.16/mypy_boto3_lakeformation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-08-01 11:37:09.000000 mypy-boto3-lakeformation-1.28.16/mypy_boto3_lakeformation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:09.000000 mypy-boto3-lakeformation-1.28.16/mypy_boto3_lakeformation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:09.000000 mypy-boto3-lakeformation-1.28.16/mypy_boto3_lakeformation.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:09.000000 mypy-boto3-lakeformation-1.28.16/mypy_boto3_lakeformation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-01 11:37:09.000000 mypy-boto3-lakeformation-1.28.16/mypy_boto3_lakeformation.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:10.164844 mypy-boto3-lakeformation-1.28.16/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-08-01 11:21:54.000000 mypy-boto3-lakeformation-1.28.16/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:01:41.969310 mypy-boto3-lakeformation-1.28.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-18 01:01:30.000000 mypy-boto3-lakeformation-1.28.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19383 2023-07-18 01:01:41.969310 mypy-boto3-lakeformation-1.28.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17874 2023-07-18 01:01:30.000000 mypy-boto3-lakeformation-1.28.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:01:41.969310 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-18 01:01:30.000000 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-07-18 01:01:30.000000 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-18 01:01:30.000000 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37102 2023-07-18 01:01:30.000000 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37043 2023-07-18 01:01:30.000000 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10421 2023-07-18 01:01:30.000000 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10419 2023-07-18 01:01:30.000000 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-07-18 01:01:30.000000 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-07-18 01:01:30.000000 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 01:01:30.000000 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    53022 2023-07-18 01:01:31.000000 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52937 2023-07-18 01:01:31.000000 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-18 01:01:30.000000 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:01:41.969310 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19383 2023-07-18 01:01:41.000000 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-18 01:01:41.000000 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 01:01:41.000000 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 01:01:41.000000 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-18 01:01:41.000000 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-18 01:01:41.000000 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 01:01:41.969310 mypy-boto3-lakeformation-1.28.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-07-18 01:01:29.000000 mypy-boto3-lakeformation-1.28.4/setup.py
```

### Comparing `mypy-boto3-lakeformation-1.28.16/LICENSE` & `mypy-boto3-lakeformation-1.28.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lakeformation-1.28.16/PKG-INFO` & `mypy-boto3-lakeformation-1.28.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-lakeformation
-Version: 1.28.16
-Summary: Type annotations for boto3.LakeFormation 1.28.16 service generated with mypy-boto3-builder 7.17.1
+Version: 1.28.4
+Summary: Type annotations for boto3.LakeFormation 1.28.4 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 lakeformation type-annotations botocore mypy typeshed autocomplete
+Keywords: boto3 lakeformation type-annotations boto3-stubs mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-lakeformation"></a>
 
 # mypy-boto3-lakeformation
 
 [![PyPI - mypy-boto3-lakeformation](https://img.shields.io/pypi/v/mypy-boto3-lakeformation.svg?color=blue)](https://pypi.org/project/mypy-boto3-lakeformation)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lakeformation.svg?color=blue)](https://pypi.org/project/mypy-boto3-lakeformation)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-lakeformation)](https://pepy.tech/project/mypy-boto3-lakeformation)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-lakeformation?color=blue)](https://pypistats.org/packages/mypy-boto3-lakeformation)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LakeFormation 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation)
+[boto3.LakeFormation 1.28.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.17.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-lakeformation docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/).
 
 See how it helps to find and fix potential bugs:
 
@@ -74,15 +74,15 @@
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Literals](#literals)
-    - [Type definitions](#type-definitions)
+    - [Typed dictionaries](#typed-dictionaries)
   - [How it works](#how-it-works)
   - [What's new](#what's-new)
     - [Implemented features](#implemented-features)
     - [Latest changes](#latest-changes)
   - [Versioning](#versioning)
   - [Thank you](#thank-you)
   - [Documentation](#documentation)
@@ -342,39 +342,44 @@
 )
 
 
 def check_value(value: ComparisonOperatorType) -> bool:
     ...
 ```
 
-<a id="type-definitions"></a>
+<a id="typed-dictionaries"></a>
 
-### Type definitions
+### Typed dictionaries
 
 `mypy_boto3_lakeformation.type_defs` module contains structures and shapes
-assembled to typed dictionaries and unions for additional type checking.
+assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_lakeformation.type_defs import (
+    LFTagPairTypeDef,
     ResponseMetadataTypeDef,
     AddObjectInputTypeDef,
     AssumeDecoratedRoleWithSAMLRequestRequestTypeDef,
     AuditContextTypeDef,
     ErrorDetailTypeDef,
+    DataLakePrincipalOutputTypeDef,
     DataLakePrincipalTypeDef,
     CancelTransactionRequestRequestTypeDef,
     LFTagPairOutputTypeDef,
     ColumnWildcardOutputTypeDef,
     ColumnWildcardTypeDef,
     CommitTransactionRequestRequestTypeDef,
     CreateLFTagRequestRequestTypeDef,
     RowFilterOutputTypeDef,
+    DataCellsFilterResourceOutputTypeDef,
     DataCellsFilterResourceTypeDef,
     RowFilterTypeDef,
+    DataLocationResourceOutputTypeDef,
     DataLocationResourceTypeDef,
+    DatabaseResourceOutputTypeDef,
     DatabaseResourceTypeDef,
     DeleteDataCellsFilterRequestRequestTypeDef,
     DeleteLFTagRequestRequestTypeDef,
     DeleteObjectInputTypeDef,
     VirtualObjectTypeDef,
     DeregisterResourceRequestRequestTypeDef,
     DescribeResourceRequestRequestTypeDef,
@@ -388,31 +393,31 @@
     GetDataCellsFilterRequestRequestTypeDef,
     GetDataLakeSettingsRequestRequestTypeDef,
     GetEffectivePermissionsForPathRequestRequestTypeDef,
     GetLFTagRequestRequestTypeDef,
     GetQueryStateRequestRequestTypeDef,
     GetQueryStatisticsRequestRequestTypeDef,
     PlanningStatisticsTypeDef,
-    TimestampTypeDef,
+    GetTableObjectsRequestRequestTypeDef,
     PartitionValueListTypeDef,
     GetWorkUnitResultsRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     GetWorkUnitsRequestRequestTypeDef,
     WorkUnitRangeTypeDef,
     LFTagKeyResourceOutputTypeDef,
     LFTagKeyResourceTypeDef,
     LFTagOutputTypeDef,
-    LFTagPairTypeDef,
     LFTagTypeDef,
     TableResourceTypeDef,
     ListLFTagsRequestRequestTypeDef,
     ListTableStorageOptimizersRequestRequestTypeDef,
     StorageOptimizerTypeDef,
     ListTransactionsRequestRequestTypeDef,
     TableObjectTypeDef,
+    QueryPlanningContextTypeDef,
     RegisterResourceRequestRequestTypeDef,
     TableResourceOutputTypeDef,
     StartTransactionRequestRequestTypeDef,
     UpdateLFTagRequestRequestTypeDef,
     UpdateResourceRequestRequestTypeDef,
     UpdateTableStorageOptimizerRequestRequestTypeDef,
     AssumeDecoratedRoleWithSAMLResponseTypeDef,
@@ -440,76 +445,67 @@
     DeleteObjectsOnCancelRequestRequestTypeDef,
     DescribeResourceResponseTypeDef,
     ListResourcesResponseTypeDef,
     DescribeTransactionResponseTypeDef,
     ListTransactionsResponseTypeDef,
     ListResourcesRequestRequestTypeDef,
     GetQueryStatisticsResponseTypeDef,
-    GetTableObjectsRequestRequestTypeDef,
-    QueryPlanningContextTypeDef,
     GetTemporaryGluePartitionCredentialsRequestRequestTypeDef,
     GetWorkUnitsRequestGetWorkUnitsPaginateTypeDef,
     ListLFTagsRequestListLFTagsPaginateTypeDef,
     GetWorkUnitsResponseTypeDef,
     LFTagPolicyResourceOutputTypeDef,
-    LFTagPairUnionTypeDef,
     LFTagPolicyResourceTypeDef,
-    LFTagUnionTypeDef,
+    SearchDatabasesByLFTagsRequestRequestTypeDef,
+    SearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef,
+    SearchTablesByLFTagsRequestRequestTypeDef,
+    SearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef,
     ListDataCellsFilterRequestListDataCellsFilterPaginateTypeDef,
     ListDataCellsFilterRequestRequestTypeDef,
     ListTableStorageOptimizersResponseTypeDef,
     PartitionObjectsTypeDef,
-    TableResourceUnionTypeDef,
+    StartQueryPlanningRequestRequestTypeDef,
     DataLakeSettingsOutputTypeDef,
     DataLakeSettingsTypeDef,
     GetResourceLFTagsResponseTypeDef,
     TaggedTableTypeDef,
     AddLFTagsToResourceResponseTypeDef,
     RemoveLFTagsFromResourceResponseTypeDef,
     GetDataCellsFilterResponseTypeDef,
     ListDataCellsFilterResponseTypeDef,
     CreateDataCellsFilterRequestRequestTypeDef,
-    DataCellsFilterUnionTypeDef,
     UpdateDataCellsFilterRequestRequestTypeDef,
     SearchDatabasesByLFTagsResponseTypeDef,
     UpdateTableObjectsRequestRequestTypeDef,
-    StartQueryPlanningRequestRequestTypeDef,
     ResourceOutputTypeDef,
     ResourceTypeDef,
-    SearchDatabasesByLFTagsRequestRequestTypeDef,
-    SearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef,
-    SearchTablesByLFTagsRequestRequestTypeDef,
-    SearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef,
     GetTableObjectsResponseTypeDef,
     GetDataLakeSettingsResponseTypeDef,
-    DataLakeSettingsUnionTypeDef,
     PutDataLakeSettingsRequestRequestTypeDef,
     SearchTablesByLFTagsResponseTypeDef,
     BatchPermissionsRequestEntryOutputTypeDef,
     PrincipalResourcePermissionsTypeDef,
     AddLFTagsToResourceRequestRequestTypeDef,
     BatchPermissionsRequestEntryTypeDef,
     GetResourceLFTagsRequestRequestTypeDef,
     GrantPermissionsRequestRequestTypeDef,
     ListPermissionsRequestRequestTypeDef,
     RemoveLFTagsFromResourceRequestRequestTypeDef,
-    ResourceUnionTypeDef,
     RevokePermissionsRequestRequestTypeDef,
     BatchPermissionsFailureEntryTypeDef,
     GetEffectivePermissionsForPathResponseTypeDef,
     ListPermissionsResponseTypeDef,
-    BatchPermissionsRequestEntryUnionTypeDef,
-    BatchGrantPermissionsResponseTypeDef,
-    BatchRevokePermissionsResponseTypeDef,
     BatchGrantPermissionsRequestRequestTypeDef,
     BatchRevokePermissionsRequestRequestTypeDef,
+    BatchGrantPermissionsResponseTypeDef,
+    BatchRevokePermissionsResponseTypeDef,
 )
 
 
-def get_value() -> ResponseMetadataTypeDef:
+def get_structure() -> LFTagPairTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-lakeformation-1.28.16/README.md` & `mypy-boto3-lakeformation-1.28.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-lakeformation"></a>
 
 # mypy-boto3-lakeformation
 
 [![PyPI - mypy-boto3-lakeformation](https://img.shields.io/pypi/v/mypy-boto3-lakeformation.svg?color=blue)](https://pypi.org/project/mypy-boto3-lakeformation)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lakeformation.svg?color=blue)](https://pypi.org/project/mypy-boto3-lakeformation)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-lakeformation)](https://pepy.tech/project/mypy-boto3-lakeformation)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-lakeformation?color=blue)](https://pypistats.org/packages/mypy-boto3-lakeformation)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LakeFormation 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation)
+[boto3.LakeFormation 1.28.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.17.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-lakeformation docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/).
 
 See how it helps to find and fix potential bugs:
 
@@ -42,15 +42,15 @@
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Literals](#literals)
-    - [Type definitions](#type-definitions)
+    - [Typed dictionaries](#typed-dictionaries)
   - [How it works](#how-it-works)
   - [What's new](#what's-new)
     - [Implemented features](#implemented-features)
     - [Latest changes](#latest-changes)
   - [Versioning](#versioning)
   - [Thank you](#thank-you)
   - [Documentation](#documentation)
@@ -310,39 +310,44 @@
 )
 
 
 def check_value(value: ComparisonOperatorType) -> bool:
     ...
 ```
 
-<a id="type-definitions"></a>
+<a id="typed-dictionaries"></a>
 
-### Type definitions
+### Typed dictionaries
 
 `mypy_boto3_lakeformation.type_defs` module contains structures and shapes
-assembled to typed dictionaries and unions for additional type checking.
+assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_lakeformation.type_defs import (
+    LFTagPairTypeDef,
     ResponseMetadataTypeDef,
     AddObjectInputTypeDef,
     AssumeDecoratedRoleWithSAMLRequestRequestTypeDef,
     AuditContextTypeDef,
     ErrorDetailTypeDef,
+    DataLakePrincipalOutputTypeDef,
     DataLakePrincipalTypeDef,
     CancelTransactionRequestRequestTypeDef,
     LFTagPairOutputTypeDef,
     ColumnWildcardOutputTypeDef,
     ColumnWildcardTypeDef,
     CommitTransactionRequestRequestTypeDef,
     CreateLFTagRequestRequestTypeDef,
     RowFilterOutputTypeDef,
+    DataCellsFilterResourceOutputTypeDef,
     DataCellsFilterResourceTypeDef,
     RowFilterTypeDef,
+    DataLocationResourceOutputTypeDef,
     DataLocationResourceTypeDef,
+    DatabaseResourceOutputTypeDef,
     DatabaseResourceTypeDef,
     DeleteDataCellsFilterRequestRequestTypeDef,
     DeleteLFTagRequestRequestTypeDef,
     DeleteObjectInputTypeDef,
     VirtualObjectTypeDef,
     DeregisterResourceRequestRequestTypeDef,
     DescribeResourceRequestRequestTypeDef,
@@ -356,31 +361,31 @@
     GetDataCellsFilterRequestRequestTypeDef,
     GetDataLakeSettingsRequestRequestTypeDef,
     GetEffectivePermissionsForPathRequestRequestTypeDef,
     GetLFTagRequestRequestTypeDef,
     GetQueryStateRequestRequestTypeDef,
     GetQueryStatisticsRequestRequestTypeDef,
     PlanningStatisticsTypeDef,
-    TimestampTypeDef,
+    GetTableObjectsRequestRequestTypeDef,
     PartitionValueListTypeDef,
     GetWorkUnitResultsRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     GetWorkUnitsRequestRequestTypeDef,
     WorkUnitRangeTypeDef,
     LFTagKeyResourceOutputTypeDef,
     LFTagKeyResourceTypeDef,
     LFTagOutputTypeDef,
-    LFTagPairTypeDef,
     LFTagTypeDef,
     TableResourceTypeDef,
     ListLFTagsRequestRequestTypeDef,
     ListTableStorageOptimizersRequestRequestTypeDef,
     StorageOptimizerTypeDef,
     ListTransactionsRequestRequestTypeDef,
     TableObjectTypeDef,
+    QueryPlanningContextTypeDef,
     RegisterResourceRequestRequestTypeDef,
     TableResourceOutputTypeDef,
     StartTransactionRequestRequestTypeDef,
     UpdateLFTagRequestRequestTypeDef,
     UpdateResourceRequestRequestTypeDef,
     UpdateTableStorageOptimizerRequestRequestTypeDef,
     AssumeDecoratedRoleWithSAMLResponseTypeDef,
@@ -408,76 +413,67 @@
     DeleteObjectsOnCancelRequestRequestTypeDef,
     DescribeResourceResponseTypeDef,
     ListResourcesResponseTypeDef,
     DescribeTransactionResponseTypeDef,
     ListTransactionsResponseTypeDef,
     ListResourcesRequestRequestTypeDef,
     GetQueryStatisticsResponseTypeDef,
-    GetTableObjectsRequestRequestTypeDef,
-    QueryPlanningContextTypeDef,
     GetTemporaryGluePartitionCredentialsRequestRequestTypeDef,
     GetWorkUnitsRequestGetWorkUnitsPaginateTypeDef,
     ListLFTagsRequestListLFTagsPaginateTypeDef,
     GetWorkUnitsResponseTypeDef,
     LFTagPolicyResourceOutputTypeDef,
-    LFTagPairUnionTypeDef,
     LFTagPolicyResourceTypeDef,
-    LFTagUnionTypeDef,
+    SearchDatabasesByLFTagsRequestRequestTypeDef,
+    SearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef,
+    SearchTablesByLFTagsRequestRequestTypeDef,
+    SearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef,
     ListDataCellsFilterRequestListDataCellsFilterPaginateTypeDef,
     ListDataCellsFilterRequestRequestTypeDef,
     ListTableStorageOptimizersResponseTypeDef,
     PartitionObjectsTypeDef,
-    TableResourceUnionTypeDef,
+    StartQueryPlanningRequestRequestTypeDef,
     DataLakeSettingsOutputTypeDef,
     DataLakeSettingsTypeDef,
     GetResourceLFTagsResponseTypeDef,
     TaggedTableTypeDef,
     AddLFTagsToResourceResponseTypeDef,
     RemoveLFTagsFromResourceResponseTypeDef,
     GetDataCellsFilterResponseTypeDef,
     ListDataCellsFilterResponseTypeDef,
     CreateDataCellsFilterRequestRequestTypeDef,
-    DataCellsFilterUnionTypeDef,
     UpdateDataCellsFilterRequestRequestTypeDef,
     SearchDatabasesByLFTagsResponseTypeDef,
     UpdateTableObjectsRequestRequestTypeDef,
-    StartQueryPlanningRequestRequestTypeDef,
     ResourceOutputTypeDef,
     ResourceTypeDef,
-    SearchDatabasesByLFTagsRequestRequestTypeDef,
-    SearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef,
-    SearchTablesByLFTagsRequestRequestTypeDef,
-    SearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef,
     GetTableObjectsResponseTypeDef,
     GetDataLakeSettingsResponseTypeDef,
-    DataLakeSettingsUnionTypeDef,
     PutDataLakeSettingsRequestRequestTypeDef,
     SearchTablesByLFTagsResponseTypeDef,
     BatchPermissionsRequestEntryOutputTypeDef,
     PrincipalResourcePermissionsTypeDef,
     AddLFTagsToResourceRequestRequestTypeDef,
     BatchPermissionsRequestEntryTypeDef,
     GetResourceLFTagsRequestRequestTypeDef,
     GrantPermissionsRequestRequestTypeDef,
     ListPermissionsRequestRequestTypeDef,
     RemoveLFTagsFromResourceRequestRequestTypeDef,
-    ResourceUnionTypeDef,
     RevokePermissionsRequestRequestTypeDef,
     BatchPermissionsFailureEntryTypeDef,
     GetEffectivePermissionsForPathResponseTypeDef,
     ListPermissionsResponseTypeDef,
-    BatchPermissionsRequestEntryUnionTypeDef,
-    BatchGrantPermissionsResponseTypeDef,
-    BatchRevokePermissionsResponseTypeDef,
     BatchGrantPermissionsRequestRequestTypeDef,
     BatchRevokePermissionsRequestRequestTypeDef,
+    BatchGrantPermissionsResponseTypeDef,
+    BatchRevokePermissionsResponseTypeDef,
 )
 
 
-def get_value() -> ResponseMetadataTypeDef:
+def get_structure() -> LFTagPairTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-lakeformation-1.28.16/mypy_boto3_lakeformation/__init__.py` & `mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lakeformation-1.28.16/mypy_boto3_lakeformation/__init__.pyi` & `mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lakeformation-1.28.16/mypy_boto3_lakeformation/client.py` & `mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,16 @@
     from mypy_boto3_lakeformation.client import LakeFormationClient
 
     session = Session()
     client: LakeFormationClient = session.client("lakeformation")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from datetime import datetime
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     DataLakeResourceTypeType,
     OptimizerTypeType,
     PermissionType,
@@ -35,20 +36,20 @@
     SearchTablesByLFTagsPaginator,
 )
 from .type_defs import (
     AddLFTagsToResourceResponseTypeDef,
     AssumeDecoratedRoleWithSAMLResponseTypeDef,
     AuditContextTypeDef,
     BatchGrantPermissionsResponseTypeDef,
-    BatchPermissionsRequestEntryUnionTypeDef,
+    BatchPermissionsRequestEntryTypeDef,
     BatchRevokePermissionsResponseTypeDef,
     CommitTransactionResponseTypeDef,
-    DataCellsFilterUnionTypeDef,
+    DataCellsFilterTypeDef,
     DataLakePrincipalTypeDef,
-    DataLakeSettingsUnionTypeDef,
+    DataLakeSettingsTypeDef,
     DescribeResourceResponseTypeDef,
     DescribeTransactionResponseTypeDef,
     FilterConditionTypeDef,
     GetDataCellsFilterResponseTypeDef,
     GetDataLakeSettingsResponseTypeDef,
     GetEffectivePermissionsForPathResponseTypeDef,
     GetLFTagResponseTypeDef,
@@ -56,32 +57,31 @@
     GetQueryStatisticsResponseTypeDef,
     GetResourceLFTagsResponseTypeDef,
     GetTableObjectsResponseTypeDef,
     GetTemporaryGluePartitionCredentialsResponseTypeDef,
     GetTemporaryGlueTableCredentialsResponseTypeDef,
     GetWorkUnitResultsResponseTypeDef,
     GetWorkUnitsResponseTypeDef,
-    LFTagPairUnionTypeDef,
-    LFTagUnionTypeDef,
+    LFTagPairTypeDef,
+    LFTagTypeDef,
     ListDataCellsFilterResponseTypeDef,
     ListLFTagsResponseTypeDef,
     ListPermissionsResponseTypeDef,
     ListResourcesResponseTypeDef,
     ListTableStorageOptimizersResponseTypeDef,
     ListTransactionsResponseTypeDef,
     PartitionValueListTypeDef,
     QueryPlanningContextTypeDef,
     RemoveLFTagsFromResourceResponseTypeDef,
-    ResourceUnionTypeDef,
+    ResourceTypeDef,
     SearchDatabasesByLFTagsResponseTypeDef,
     SearchTablesByLFTagsResponseTypeDef,
     StartQueryPlanningResponseTypeDef,
     StartTransactionResponseTypeDef,
-    TableResourceUnionTypeDef,
-    TimestampTypeDef,
+    TableResourceTypeDef,
     UpdateTableStorageOptimizerResponseTypeDef,
     VirtualObjectTypeDef,
     WriteOperationTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
@@ -136,19 +136,15 @@
         LakeFormationClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#exceptions)
         """
 
     def add_lf_tags_to_resource(
-        self,
-        *,
-        Resource: ResourceUnionTypeDef,
-        LFTags: Sequence[LFTagPairUnionTypeDef],
-        CatalogId: str = ...
+        self, *, Resource: ResourceTypeDef, LFTags: Sequence[LFTagPairTypeDef], CatalogId: str = ...
     ) -> AddLFTagsToResourceResponseTypeDef:
         """
         Attaches one or more LF-tags to an existing resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.add_lf_tags_to_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#add_lf_tags_to_resource)
         """
@@ -161,25 +157,25 @@
         the SAML assertion included in the request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.assume_decorated_role_with_saml)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#assume_decorated_role_with_saml)
         """
 
     def batch_grant_permissions(
-        self, *, Entries: Sequence[BatchPermissionsRequestEntryUnionTypeDef], CatalogId: str = ...
+        self, *, Entries: Sequence[BatchPermissionsRequestEntryTypeDef], CatalogId: str = ...
     ) -> BatchGrantPermissionsResponseTypeDef:
         """
         Batch operation to grant permissions to the principal.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.batch_grant_permissions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#batch_grant_permissions)
         """
 
     def batch_revoke_permissions(
-        self, *, Entries: Sequence[BatchPermissionsRequestEntryUnionTypeDef], CatalogId: str = ...
+        self, *, Entries: Sequence[BatchPermissionsRequestEntryTypeDef], CatalogId: str = ...
     ) -> BatchRevokePermissionsResponseTypeDef:
         """
         Batch operation to revoke permissions from the principal.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.batch_revoke_permissions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#batch_revoke_permissions)
         """
@@ -212,15 +208,15 @@
         """
         Attempts to commit the specified transaction.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.commit_transaction)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#commit_transaction)
         """
 
-    def create_data_cells_filter(self, *, TableData: DataCellsFilterUnionTypeDef) -> Dict[str, Any]:
+    def create_data_cells_filter(self, *, TableData: DataCellsFilterTypeDef) -> Dict[str, Any]:
         """
         Creates a data cell filter to allow one to grant access to certain columns on
         certain rows.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.create_data_cells_filter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#create_data_cells_filter)
         """
@@ -375,19 +371,15 @@
         Retrieves statistics on the planning and execution of a query.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.get_query_statistics)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#get_query_statistics)
         """
 
     def get_resource_lf_tags(
-        self,
-        *,
-        Resource: ResourceUnionTypeDef,
-        CatalogId: str = ...,
-        ShowAssignedLFTags: bool = ...
+        self, *, Resource: ResourceTypeDef, CatalogId: str = ..., ShowAssignedLFTags: bool = ...
     ) -> GetResourceLFTagsResponseTypeDef:
         """
         Returns the LF-tags applied to a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.get_resource_lf_tags)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#get_resource_lf_tags)
         """
@@ -395,15 +387,15 @@
     def get_table_objects(
         self,
         *,
         DatabaseName: str,
         TableName: str,
         CatalogId: str = ...,
         TransactionId: str = ...,
-        QueryAsOfTime: TimestampTypeDef = ...,
+        QueryAsOfTime: Union[datetime, str] = ...,
         PartitionPredicate: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> GetTableObjectsResponseTypeDef:
         """
         Returns the set of Amazon S3 objects that make up the specified governed table.
 
@@ -466,29 +458,29 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#get_work_units)
         """
 
     def grant_permissions(
         self,
         *,
         Principal: DataLakePrincipalTypeDef,
-        Resource: ResourceUnionTypeDef,
+        Resource: ResourceTypeDef,
         Permissions: Sequence[PermissionType],
         CatalogId: str = ...,
         PermissionsWithGrantOption: Sequence[PermissionType] = ...
     ) -> Dict[str, Any]:
         """
         Grants permissions to the principal to access metadata in the Data Catalog and
         data organized in underlying data storage such as Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.grant_permissions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#grant_permissions)
         """
 
     def list_data_cells_filter(
-        self, *, Table: TableResourceUnionTypeDef = ..., NextToken: str = ..., MaxResults: int = ...
+        self, *, Table: TableResourceTypeDef = ..., NextToken: str = ..., MaxResults: int = ...
     ) -> ListDataCellsFilterResponseTypeDef:
         """
         Lists all the data cell filters on a table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.list_data_cells_filter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#list_data_cells_filter)
         """
@@ -510,15 +502,15 @@
 
     def list_permissions(
         self,
         *,
         CatalogId: str = ...,
         Principal: DataLakePrincipalTypeDef = ...,
         ResourceType: DataLakeResourceTypeType = ...,
-        Resource: ResourceUnionTypeDef = ...,
+        Resource: ResourceTypeDef = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
         IncludeRelated: str = ...
     ) -> ListPermissionsResponseTypeDef:
         """
         Returns a list of the principal permissions on the resource, filtered by the
         permissions of the caller.
@@ -571,15 +563,15 @@
         Returns metadata about transactions and their status.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.list_transactions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#list_transactions)
         """
 
     def put_data_lake_settings(
-        self, *, DataLakeSettings: DataLakeSettingsUnionTypeDef, CatalogId: str = ...
+        self, *, DataLakeSettings: DataLakeSettingsTypeDef, CatalogId: str = ...
     ) -> Dict[str, Any]:
         """
         Sets the list of data lake administrators who have admin privileges on all
         resources managed by Lake Formation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.put_data_lake_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#put_data_lake_settings)
@@ -597,32 +589,28 @@
         Registers the resource as managed by the Data Catalog.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.register_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#register_resource)
         """
 
     def remove_lf_tags_from_resource(
-        self,
-        *,
-        Resource: ResourceUnionTypeDef,
-        LFTags: Sequence[LFTagPairUnionTypeDef],
-        CatalogId: str = ...
+        self, *, Resource: ResourceTypeDef, LFTags: Sequence[LFTagPairTypeDef], CatalogId: str = ...
     ) -> RemoveLFTagsFromResourceResponseTypeDef:
         """
         Removes an LF-tag from the resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.remove_lf_tags_from_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#remove_lf_tags_from_resource)
         """
 
     def revoke_permissions(
         self,
         *,
         Principal: DataLakePrincipalTypeDef,
-        Resource: ResourceUnionTypeDef,
+        Resource: ResourceTypeDef,
         Permissions: Sequence[PermissionType],
         CatalogId: str = ...,
         PermissionsWithGrantOption: Sequence[PermissionType] = ...
     ) -> Dict[str, Any]:
         """
         Revokes permissions to the principal to access metadata in the Data Catalog and
         data organized in underlying data storage such as Amazon S3.
@@ -630,30 +618,30 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.revoke_permissions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#revoke_permissions)
         """
 
     def search_databases_by_lf_tags(
         self,
         *,
-        Expression: Sequence[LFTagUnionTypeDef],
+        Expression: Sequence[LFTagTypeDef],
         NextToken: str = ...,
         MaxResults: int = ...,
         CatalogId: str = ...
     ) -> SearchDatabasesByLFTagsResponseTypeDef:
         """
         This operation allows a search on `DATABASE` resources by `TagCondition`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.search_databases_by_lf_tags)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#search_databases_by_lf_tags)
         """
 
     def search_tables_by_lf_tags(
         self,
         *,
-        Expression: Sequence[LFTagUnionTypeDef],
+        Expression: Sequence[LFTagTypeDef],
         NextToken: str = ...,
         MaxResults: int = ...,
         CatalogId: str = ...
     ) -> SearchTablesByLFTagsResponseTypeDef:
         """
         This operation allows a search on `TABLE` resources by `LFTag`s.
 
@@ -677,15 +665,15 @@
         """
         Starts a new transaction and returns its transaction ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.start_transaction)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#start_transaction)
         """
 
-    def update_data_cells_filter(self, *, TableData: DataCellsFilterUnionTypeDef) -> Dict[str, Any]:
+    def update_data_cells_filter(self, *, TableData: DataCellsFilterTypeDef) -> Dict[str, Any]:
         """
         Updates a data cell filter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.update_data_cells_filter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#update_data_cells_filter)
         """
```

### Comparing `mypy-boto3-lakeformation-1.28.16/mypy_boto3_lakeformation/client.pyi` & `mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,16 @@
     from mypy_boto3_lakeformation.client import LakeFormationClient
 
     session = Session()
     client: LakeFormationClient = session.client("lakeformation")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from datetime import datetime
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     DataLakeResourceTypeType,
     OptimizerTypeType,
     PermissionType,
@@ -35,20 +36,20 @@
     SearchTablesByLFTagsPaginator,
 )
 from .type_defs import (
     AddLFTagsToResourceResponseTypeDef,
     AssumeDecoratedRoleWithSAMLResponseTypeDef,
     AuditContextTypeDef,
     BatchGrantPermissionsResponseTypeDef,
-    BatchPermissionsRequestEntryUnionTypeDef,
+    BatchPermissionsRequestEntryTypeDef,
     BatchRevokePermissionsResponseTypeDef,
     CommitTransactionResponseTypeDef,
-    DataCellsFilterUnionTypeDef,
+    DataCellsFilterTypeDef,
     DataLakePrincipalTypeDef,
-    DataLakeSettingsUnionTypeDef,
+    DataLakeSettingsTypeDef,
     DescribeResourceResponseTypeDef,
     DescribeTransactionResponseTypeDef,
     FilterConditionTypeDef,
     GetDataCellsFilterResponseTypeDef,
     GetDataLakeSettingsResponseTypeDef,
     GetEffectivePermissionsForPathResponseTypeDef,
     GetLFTagResponseTypeDef,
@@ -56,32 +57,31 @@
     GetQueryStatisticsResponseTypeDef,
     GetResourceLFTagsResponseTypeDef,
     GetTableObjectsResponseTypeDef,
     GetTemporaryGluePartitionCredentialsResponseTypeDef,
     GetTemporaryGlueTableCredentialsResponseTypeDef,
     GetWorkUnitResultsResponseTypeDef,
     GetWorkUnitsResponseTypeDef,
-    LFTagPairUnionTypeDef,
-    LFTagUnionTypeDef,
+    LFTagPairTypeDef,
+    LFTagTypeDef,
     ListDataCellsFilterResponseTypeDef,
     ListLFTagsResponseTypeDef,
     ListPermissionsResponseTypeDef,
     ListResourcesResponseTypeDef,
     ListTableStorageOptimizersResponseTypeDef,
     ListTransactionsResponseTypeDef,
     PartitionValueListTypeDef,
     QueryPlanningContextTypeDef,
     RemoveLFTagsFromResourceResponseTypeDef,
-    ResourceUnionTypeDef,
+    ResourceTypeDef,
     SearchDatabasesByLFTagsResponseTypeDef,
     SearchTablesByLFTagsResponseTypeDef,
     StartQueryPlanningResponseTypeDef,
     StartTransactionResponseTypeDef,
-    TableResourceUnionTypeDef,
-    TimestampTypeDef,
+    TableResourceTypeDef,
     UpdateTableStorageOptimizerResponseTypeDef,
     VirtualObjectTypeDef,
     WriteOperationTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
@@ -131,19 +131,15 @@
         """
         LakeFormationClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#exceptions)
         """
     def add_lf_tags_to_resource(
-        self,
-        *,
-        Resource: ResourceUnionTypeDef,
-        LFTags: Sequence[LFTagPairUnionTypeDef],
-        CatalogId: str = ...
+        self, *, Resource: ResourceTypeDef, LFTags: Sequence[LFTagPairTypeDef], CatalogId: str = ...
     ) -> AddLFTagsToResourceResponseTypeDef:
         """
         Attaches one or more LF-tags to an existing resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.add_lf_tags_to_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#add_lf_tags_to_resource)
         """
@@ -154,24 +150,24 @@
         Allows a caller to assume an IAM role decorated as the SAML user specified in
         the SAML assertion included in the request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.assume_decorated_role_with_saml)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#assume_decorated_role_with_saml)
         """
     def batch_grant_permissions(
-        self, *, Entries: Sequence[BatchPermissionsRequestEntryUnionTypeDef], CatalogId: str = ...
+        self, *, Entries: Sequence[BatchPermissionsRequestEntryTypeDef], CatalogId: str = ...
     ) -> BatchGrantPermissionsResponseTypeDef:
         """
         Batch operation to grant permissions to the principal.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.batch_grant_permissions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#batch_grant_permissions)
         """
     def batch_revoke_permissions(
-        self, *, Entries: Sequence[BatchPermissionsRequestEntryUnionTypeDef], CatalogId: str = ...
+        self, *, Entries: Sequence[BatchPermissionsRequestEntryTypeDef], CatalogId: str = ...
     ) -> BatchRevokePermissionsResponseTypeDef:
         """
         Batch operation to revoke permissions from the principal.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.batch_revoke_permissions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#batch_revoke_permissions)
         """
@@ -199,15 +195,15 @@
     def commit_transaction(self, *, TransactionId: str) -> CommitTransactionResponseTypeDef:
         """
         Attempts to commit the specified transaction.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.commit_transaction)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#commit_transaction)
         """
-    def create_data_cells_filter(self, *, TableData: DataCellsFilterUnionTypeDef) -> Dict[str, Any]:
+    def create_data_cells_filter(self, *, TableData: DataCellsFilterTypeDef) -> Dict[str, Any]:
         """
         Creates a data cell filter to allow one to grant access to certain columns on
         certain rows.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.create_data_cells_filter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#create_data_cells_filter)
         """
@@ -346,34 +342,30 @@
         """
         Retrieves statistics on the planning and execution of a query.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.get_query_statistics)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#get_query_statistics)
         """
     def get_resource_lf_tags(
-        self,
-        *,
-        Resource: ResourceUnionTypeDef,
-        CatalogId: str = ...,
-        ShowAssignedLFTags: bool = ...
+        self, *, Resource: ResourceTypeDef, CatalogId: str = ..., ShowAssignedLFTags: bool = ...
     ) -> GetResourceLFTagsResponseTypeDef:
         """
         Returns the LF-tags applied to a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.get_resource_lf_tags)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#get_resource_lf_tags)
         """
     def get_table_objects(
         self,
         *,
         DatabaseName: str,
         TableName: str,
         CatalogId: str = ...,
         TransactionId: str = ...,
-        QueryAsOfTime: TimestampTypeDef = ...,
+        QueryAsOfTime: Union[datetime, str] = ...,
         PartitionPredicate: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> GetTableObjectsResponseTypeDef:
         """
         Returns the set of Amazon S3 objects that make up the specified governed table.
 
@@ -431,28 +423,28 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.get_work_units)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#get_work_units)
         """
     def grant_permissions(
         self,
         *,
         Principal: DataLakePrincipalTypeDef,
-        Resource: ResourceUnionTypeDef,
+        Resource: ResourceTypeDef,
         Permissions: Sequence[PermissionType],
         CatalogId: str = ...,
         PermissionsWithGrantOption: Sequence[PermissionType] = ...
     ) -> Dict[str, Any]:
         """
         Grants permissions to the principal to access metadata in the Data Catalog and
         data organized in underlying data storage such as Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.grant_permissions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#grant_permissions)
         """
     def list_data_cells_filter(
-        self, *, Table: TableResourceUnionTypeDef = ..., NextToken: str = ..., MaxResults: int = ...
+        self, *, Table: TableResourceTypeDef = ..., NextToken: str = ..., MaxResults: int = ...
     ) -> ListDataCellsFilterResponseTypeDef:
         """
         Lists all the data cell filters on a table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.list_data_cells_filter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#list_data_cells_filter)
         """
@@ -472,15 +464,15 @@
         """
     def list_permissions(
         self,
         *,
         CatalogId: str = ...,
         Principal: DataLakePrincipalTypeDef = ...,
         ResourceType: DataLakeResourceTypeType = ...,
-        Resource: ResourceUnionTypeDef = ...,
+        Resource: ResourceTypeDef = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
         IncludeRelated: str = ...
     ) -> ListPermissionsResponseTypeDef:
         """
         Returns a list of the principal permissions on the resource, filtered by the
         permissions of the caller.
@@ -529,15 +521,15 @@
         """
         Returns metadata about transactions and their status.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.list_transactions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#list_transactions)
         """
     def put_data_lake_settings(
-        self, *, DataLakeSettings: DataLakeSettingsUnionTypeDef, CatalogId: str = ...
+        self, *, DataLakeSettings: DataLakeSettingsTypeDef, CatalogId: str = ...
     ) -> Dict[str, Any]:
         """
         Sets the list of data lake administrators who have admin privileges on all
         resources managed by Lake Formation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.put_data_lake_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#put_data_lake_settings)
@@ -553,60 +545,56 @@
         """
         Registers the resource as managed by the Data Catalog.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.register_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#register_resource)
         """
     def remove_lf_tags_from_resource(
-        self,
-        *,
-        Resource: ResourceUnionTypeDef,
-        LFTags: Sequence[LFTagPairUnionTypeDef],
-        CatalogId: str = ...
+        self, *, Resource: ResourceTypeDef, LFTags: Sequence[LFTagPairTypeDef], CatalogId: str = ...
     ) -> RemoveLFTagsFromResourceResponseTypeDef:
         """
         Removes an LF-tag from the resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.remove_lf_tags_from_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#remove_lf_tags_from_resource)
         """
     def revoke_permissions(
         self,
         *,
         Principal: DataLakePrincipalTypeDef,
-        Resource: ResourceUnionTypeDef,
+        Resource: ResourceTypeDef,
         Permissions: Sequence[PermissionType],
         CatalogId: str = ...,
         PermissionsWithGrantOption: Sequence[PermissionType] = ...
     ) -> Dict[str, Any]:
         """
         Revokes permissions to the principal to access metadata in the Data Catalog and
         data organized in underlying data storage such as Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.revoke_permissions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#revoke_permissions)
         """
     def search_databases_by_lf_tags(
         self,
         *,
-        Expression: Sequence[LFTagUnionTypeDef],
+        Expression: Sequence[LFTagTypeDef],
         NextToken: str = ...,
         MaxResults: int = ...,
         CatalogId: str = ...
     ) -> SearchDatabasesByLFTagsResponseTypeDef:
         """
         This operation allows a search on `DATABASE` resources by `TagCondition`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.search_databases_by_lf_tags)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#search_databases_by_lf_tags)
         """
     def search_tables_by_lf_tags(
         self,
         *,
-        Expression: Sequence[LFTagUnionTypeDef],
+        Expression: Sequence[LFTagTypeDef],
         NextToken: str = ...,
         MaxResults: int = ...,
         CatalogId: str = ...
     ) -> SearchTablesByLFTagsResponseTypeDef:
         """
         This operation allows a search on `TABLE` resources by `LFTag`s.
 
@@ -627,15 +615,15 @@
     ) -> StartTransactionResponseTypeDef:
         """
         Starts a new transaction and returns its transaction ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.start_transaction)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#start_transaction)
         """
-    def update_data_cells_filter(self, *, TableData: DataCellsFilterUnionTypeDef) -> Dict[str, Any]:
+    def update_data_cells_filter(self, *, TableData: DataCellsFilterTypeDef) -> Dict[str, Any]:
         """
         Updates a data cell filter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.update_data_cells_filter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/client/#update_data_cells_filter)
         """
     def update_lf_tag(
```

### Comparing `mypy-boto3-lakeformation-1.28.16/mypy_boto3_lakeformation/literals.py` & `mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -205,15 +205,14 @@
     "elasticbeanstalk",
     "elastictranscoder",
     "elb",
     "elbv2",
     "emr",
     "emr-containers",
     "emr-serverless",
-    "entityresolution",
     "es",
     "events",
     "evidently",
     "finspace",
     "finspace-data",
     "firehose",
     "fis",
@@ -292,28 +291,26 @@
     "lookoutmetrics",
     "lookoutvision",
     "m2",
     "machinelearning",
     "macie",
     "macie2",
     "managedblockchain",
-    "managedblockchain-query",
     "marketplace-catalog",
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
     "mediapackage-vod",
     "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
-    "medical-imaging",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
     "migration-hub-refactor-spaces",
     "migrationhub-config",
     "migrationhuborchestrator",
```

### Comparing `mypy-boto3-lakeformation-1.28.16/mypy_boto3_lakeformation/literals.pyi` & `mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -203,15 +203,14 @@
     "elasticbeanstalk",
     "elastictranscoder",
     "elb",
     "elbv2",
     "emr",
     "emr-containers",
     "emr-serverless",
-    "entityresolution",
     "es",
     "events",
     "evidently",
     "finspace",
     "finspace-data",
     "firehose",
     "fis",
@@ -290,28 +289,26 @@
     "lookoutmetrics",
     "lookoutvision",
     "m2",
     "machinelearning",
     "macie",
     "macie2",
     "managedblockchain",
-    "managedblockchain-query",
     "marketplace-catalog",
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
     "mediapackage-vod",
     "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
-    "medical-imaging",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
     "migration-hub-refactor-spaces",
     "migrationhub-config",
     "migrationhuborchestrator",
```

### Comparing `mypy-boto3-lakeformation-1.28.16/mypy_boto3_lakeformation/paginator.py` & `mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/paginator.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -30,75 +30,67 @@
 from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import ResourceShareTypeType
 from .type_defs import (
     GetWorkUnitsResponseTypeDef,
-    LFTagUnionTypeDef,
+    LFTagTypeDef,
     ListDataCellsFilterResponseTypeDef,
     ListLFTagsResponseTypeDef,
     PaginatorConfigTypeDef,
     SearchDatabasesByLFTagsResponseTypeDef,
     SearchTablesByLFTagsResponseTypeDef,
-    TableResourceUnionTypeDef,
+    TableResourceTypeDef,
 )
 
 __all__ = (
     "GetWorkUnitsPaginator",
     "ListDataCellsFilterPaginator",
     "ListLFTagsPaginator",
     "SearchDatabasesByLFTagsPaginator",
     "SearchTablesByLFTagsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class GetWorkUnitsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.GetWorkUnits)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/paginators/#getworkunitspaginator)
     """
 
     def paginate(
         self, *, QueryId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetWorkUnitsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.GetWorkUnits.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/paginators/#getworkunitspaginator)
         """
 
-
 class ListDataCellsFilterPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.ListDataCellsFilter)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/paginators/#listdatacellsfilterpaginator)
     """
 
     def paginate(
-        self,
-        *,
-        Table: TableResourceUnionTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, Table: TableResourceTypeDef = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDataCellsFilterResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.ListDataCellsFilter.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/paginators/#listdatacellsfilterpaginator)
         """
 
-
 class ListLFTagsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.ListLFTags)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/paginators/#listlftagspaginator)
     """
 
     def paginate(
@@ -109,44 +101,42 @@
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListLFTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.ListLFTags.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/paginators/#listlftagspaginator)
         """
 
-
 class SearchDatabasesByLFTagsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.SearchDatabasesByLFTags)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/paginators/#searchdatabasesbylftagspaginator)
     """
 
     def paginate(
         self,
         *,
-        Expression: Sequence[LFTagUnionTypeDef],
+        Expression: Sequence[LFTagTypeDef],
         CatalogId: str = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[SearchDatabasesByLFTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.SearchDatabasesByLFTags.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/paginators/#searchdatabasesbylftagspaginator)
         """
 
-
 class SearchTablesByLFTagsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.SearchTablesByLFTags)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/paginators/#searchtablesbylftagspaginator)
     """
 
     def paginate(
         self,
         *,
-        Expression: Sequence[LFTagUnionTypeDef],
+        Expression: Sequence[LFTagTypeDef],
         CatalogId: str = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[SearchTablesByLFTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.SearchTablesByLFTags.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/paginators/#searchtablesbylftagspaginator)
         """
```

### Comparing `mypy-boto3-lakeformation-1.28.16/mypy_boto3_lakeformation/paginator.pyi` & `mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/paginator.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,70 +30,72 @@
 from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import ResourceShareTypeType
 from .type_defs import (
     GetWorkUnitsResponseTypeDef,
-    LFTagUnionTypeDef,
+    LFTagTypeDef,
     ListDataCellsFilterResponseTypeDef,
     ListLFTagsResponseTypeDef,
     PaginatorConfigTypeDef,
     SearchDatabasesByLFTagsResponseTypeDef,
     SearchTablesByLFTagsResponseTypeDef,
-    TableResourceUnionTypeDef,
+    TableResourceTypeDef,
 )
 
 __all__ = (
     "GetWorkUnitsPaginator",
     "ListDataCellsFilterPaginator",
     "ListLFTagsPaginator",
     "SearchDatabasesByLFTagsPaginator",
     "SearchTablesByLFTagsPaginator",
 )
 
+
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class GetWorkUnitsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.GetWorkUnits)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/paginators/#getworkunitspaginator)
     """
 
     def paginate(
         self, *, QueryId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetWorkUnitsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.GetWorkUnits.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/paginators/#getworkunitspaginator)
         """
 
+
 class ListDataCellsFilterPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.ListDataCellsFilter)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/paginators/#listdatacellsfilterpaginator)
     """
 
     def paginate(
-        self,
-        *,
-        Table: TableResourceUnionTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, Table: TableResourceTypeDef = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDataCellsFilterResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.ListDataCellsFilter.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/paginators/#listdatacellsfilterpaginator)
         """
 
+
 class ListLFTagsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.ListLFTags)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/paginators/#listlftagspaginator)
     """
 
     def paginate(
@@ -104,42 +106,44 @@
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListLFTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.ListLFTags.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/paginators/#listlftagspaginator)
         """
 
+
 class SearchDatabasesByLFTagsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.SearchDatabasesByLFTags)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/paginators/#searchdatabasesbylftagspaginator)
     """
 
     def paginate(
         self,
         *,
-        Expression: Sequence[LFTagUnionTypeDef],
+        Expression: Sequence[LFTagTypeDef],
         CatalogId: str = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[SearchDatabasesByLFTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.SearchDatabasesByLFTags.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/paginators/#searchdatabasesbylftagspaginator)
         """
 
+
 class SearchTablesByLFTagsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.SearchTablesByLFTags)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/paginators/#searchtablesbylftagspaginator)
     """
 
     def paginate(
         self,
         *,
-        Expression: Sequence[LFTagUnionTypeDef],
+        Expression: Sequence[LFTagTypeDef],
         CatalogId: str = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[SearchTablesByLFTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.SearchTablesByLFTags.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/paginators/#searchtablesbylftagspaginator)
         """
```

### Comparing `mypy-boto3-lakeformation-1.28.16/mypy_boto3_lakeformation/type_defs.py` & `mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/type_defs.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for lakeformation service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_lakeformation.type_defs import ResponseMetadataTypeDef
+    from mypy_boto3_lakeformation.type_defs import LFTagPairTypeDef
 
-    data: ResponseMetadataTypeDef = ...
+    data: LFTagPairTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -35,30 +35,35 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
+    "LFTagPairTypeDef",
     "ResponseMetadataTypeDef",
     "AddObjectInputTypeDef",
     "AssumeDecoratedRoleWithSAMLRequestRequestTypeDef",
     "AuditContextTypeDef",
     "ErrorDetailTypeDef",
+    "DataLakePrincipalOutputTypeDef",
     "DataLakePrincipalTypeDef",
     "CancelTransactionRequestRequestTypeDef",
     "LFTagPairOutputTypeDef",
     "ColumnWildcardOutputTypeDef",
     "ColumnWildcardTypeDef",
     "CommitTransactionRequestRequestTypeDef",
     "CreateLFTagRequestRequestTypeDef",
     "RowFilterOutputTypeDef",
+    "DataCellsFilterResourceOutputTypeDef",
     "DataCellsFilterResourceTypeDef",
     "RowFilterTypeDef",
+    "DataLocationResourceOutputTypeDef",
     "DataLocationResourceTypeDef",
+    "DatabaseResourceOutputTypeDef",
     "DatabaseResourceTypeDef",
     "DeleteDataCellsFilterRequestRequestTypeDef",
     "DeleteLFTagRequestRequestTypeDef",
     "DeleteObjectInputTypeDef",
     "VirtualObjectTypeDef",
     "DeregisterResourceRequestRequestTypeDef",
     "DescribeResourceRequestRequestTypeDef",
@@ -72,31 +77,31 @@
     "GetDataCellsFilterRequestRequestTypeDef",
     "GetDataLakeSettingsRequestRequestTypeDef",
     "GetEffectivePermissionsForPathRequestRequestTypeDef",
     "GetLFTagRequestRequestTypeDef",
     "GetQueryStateRequestRequestTypeDef",
     "GetQueryStatisticsRequestRequestTypeDef",
     "PlanningStatisticsTypeDef",
-    "TimestampTypeDef",
+    "GetTableObjectsRequestRequestTypeDef",
     "PartitionValueListTypeDef",
     "GetWorkUnitResultsRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "GetWorkUnitsRequestRequestTypeDef",
     "WorkUnitRangeTypeDef",
     "LFTagKeyResourceOutputTypeDef",
     "LFTagKeyResourceTypeDef",
     "LFTagOutputTypeDef",
-    "LFTagPairTypeDef",
     "LFTagTypeDef",
     "TableResourceTypeDef",
     "ListLFTagsRequestRequestTypeDef",
     "ListTableStorageOptimizersRequestRequestTypeDef",
     "StorageOptimizerTypeDef",
     "ListTransactionsRequestRequestTypeDef",
     "TableObjectTypeDef",
+    "QueryPlanningContextTypeDef",
     "RegisterResourceRequestRequestTypeDef",
     "TableResourceOutputTypeDef",
     "StartTransactionRequestRequestTypeDef",
     "UpdateLFTagRequestRequestTypeDef",
     "UpdateResourceRequestRequestTypeDef",
     "UpdateTableStorageOptimizerRequestRequestTypeDef",
     "AssumeDecoratedRoleWithSAMLResponseTypeDef",
@@ -124,74 +129,85 @@
     "DeleteObjectsOnCancelRequestRequestTypeDef",
     "DescribeResourceResponseTypeDef",
     "ListResourcesResponseTypeDef",
     "DescribeTransactionResponseTypeDef",
     "ListTransactionsResponseTypeDef",
     "ListResourcesRequestRequestTypeDef",
     "GetQueryStatisticsResponseTypeDef",
-    "GetTableObjectsRequestRequestTypeDef",
-    "QueryPlanningContextTypeDef",
     "GetTemporaryGluePartitionCredentialsRequestRequestTypeDef",
     "GetWorkUnitsRequestGetWorkUnitsPaginateTypeDef",
     "ListLFTagsRequestListLFTagsPaginateTypeDef",
     "GetWorkUnitsResponseTypeDef",
     "LFTagPolicyResourceOutputTypeDef",
-    "LFTagPairUnionTypeDef",
     "LFTagPolicyResourceTypeDef",
-    "LFTagUnionTypeDef",
+    "SearchDatabasesByLFTagsRequestRequestTypeDef",
+    "SearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef",
+    "SearchTablesByLFTagsRequestRequestTypeDef",
+    "SearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef",
     "ListDataCellsFilterRequestListDataCellsFilterPaginateTypeDef",
     "ListDataCellsFilterRequestRequestTypeDef",
     "ListTableStorageOptimizersResponseTypeDef",
     "PartitionObjectsTypeDef",
-    "TableResourceUnionTypeDef",
+    "StartQueryPlanningRequestRequestTypeDef",
     "DataLakeSettingsOutputTypeDef",
     "DataLakeSettingsTypeDef",
     "GetResourceLFTagsResponseTypeDef",
     "TaggedTableTypeDef",
     "AddLFTagsToResourceResponseTypeDef",
     "RemoveLFTagsFromResourceResponseTypeDef",
     "GetDataCellsFilterResponseTypeDef",
     "ListDataCellsFilterResponseTypeDef",
     "CreateDataCellsFilterRequestRequestTypeDef",
-    "DataCellsFilterUnionTypeDef",
     "UpdateDataCellsFilterRequestRequestTypeDef",
     "SearchDatabasesByLFTagsResponseTypeDef",
     "UpdateTableObjectsRequestRequestTypeDef",
-    "StartQueryPlanningRequestRequestTypeDef",
     "ResourceOutputTypeDef",
     "ResourceTypeDef",
-    "SearchDatabasesByLFTagsRequestRequestTypeDef",
-    "SearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef",
-    "SearchTablesByLFTagsRequestRequestTypeDef",
-    "SearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef",
     "GetTableObjectsResponseTypeDef",
     "GetDataLakeSettingsResponseTypeDef",
-    "DataLakeSettingsUnionTypeDef",
     "PutDataLakeSettingsRequestRequestTypeDef",
     "SearchTablesByLFTagsResponseTypeDef",
     "BatchPermissionsRequestEntryOutputTypeDef",
     "PrincipalResourcePermissionsTypeDef",
     "AddLFTagsToResourceRequestRequestTypeDef",
     "BatchPermissionsRequestEntryTypeDef",
     "GetResourceLFTagsRequestRequestTypeDef",
     "GrantPermissionsRequestRequestTypeDef",
     "ListPermissionsRequestRequestTypeDef",
     "RemoveLFTagsFromResourceRequestRequestTypeDef",
-    "ResourceUnionTypeDef",
     "RevokePermissionsRequestRequestTypeDef",
     "BatchPermissionsFailureEntryTypeDef",
     "GetEffectivePermissionsForPathResponseTypeDef",
     "ListPermissionsResponseTypeDef",
-    "BatchPermissionsRequestEntryUnionTypeDef",
-    "BatchGrantPermissionsResponseTypeDef",
-    "BatchRevokePermissionsResponseTypeDef",
     "BatchGrantPermissionsRequestRequestTypeDef",
     "BatchRevokePermissionsRequestRequestTypeDef",
+    "BatchGrantPermissionsResponseTypeDef",
+    "BatchRevokePermissionsResponseTypeDef",
+)
+
+_RequiredLFTagPairTypeDef = TypedDict(
+    "_RequiredLFTagPairTypeDef",
+    {
+        "TagKey": str,
+        "TagValues": Sequence[str],
+    },
+)
+_OptionalLFTagPairTypeDef = TypedDict(
+    "_OptionalLFTagPairTypeDef",
+    {
+        "CatalogId": str,
+    },
+    total=False,
 )
 
+
+class LFTagPairTypeDef(_RequiredLFTagPairTypeDef, _OptionalLFTagPairTypeDef):
+    pass
+
+
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -254,15 +270,21 @@
 
 ErrorDetailTypeDef = TypedDict(
     "ErrorDetailTypeDef",
     {
         "ErrorCode": str,
         "ErrorMessage": str,
     },
-    total=False,
+)
+
+DataLakePrincipalOutputTypeDef = TypedDict(
+    "DataLakePrincipalOutputTypeDef",
+    {
+        "DataLakePrincipalIdentifier": str,
+    },
 )
 
 DataLakePrincipalTypeDef = TypedDict(
     "DataLakePrincipalTypeDef",
     {
         "DataLakePrincipalIdentifier": str,
     },
@@ -272,40 +294,28 @@
 CancelTransactionRequestRequestTypeDef = TypedDict(
     "CancelTransactionRequestRequestTypeDef",
     {
         "TransactionId": str,
     },
 )
 
-_RequiredLFTagPairOutputTypeDef = TypedDict(
-    "_RequiredLFTagPairOutputTypeDef",
+LFTagPairOutputTypeDef = TypedDict(
+    "LFTagPairOutputTypeDef",
     {
+        "CatalogId": str,
         "TagKey": str,
         "TagValues": List[str],
     },
 )
-_OptionalLFTagPairOutputTypeDef = TypedDict(
-    "_OptionalLFTagPairOutputTypeDef",
-    {
-        "CatalogId": str,
-    },
-    total=False,
-)
-
-
-class LFTagPairOutputTypeDef(_RequiredLFTagPairOutputTypeDef, _OptionalLFTagPairOutputTypeDef):
-    pass
-
 
 ColumnWildcardOutputTypeDef = TypedDict(
     "ColumnWildcardOutputTypeDef",
     {
         "ExcludedColumnNames": List[str],
     },
-    total=False,
 )
 
 ColumnWildcardTypeDef = TypedDict(
     "ColumnWildcardTypeDef",
     {
         "ExcludedColumnNames": Sequence[str],
     },
@@ -343,15 +353,24 @@
 
 RowFilterOutputTypeDef = TypedDict(
     "RowFilterOutputTypeDef",
     {
         "FilterExpression": str,
         "AllRowsWildcard": Dict[str, Any],
     },
-    total=False,
+)
+
+DataCellsFilterResourceOutputTypeDef = TypedDict(
+    "DataCellsFilterResourceOutputTypeDef",
+    {
+        "TableCatalogId": str,
+        "DatabaseName": str,
+        "TableName": str,
+        "Name": str,
+    },
 )
 
 DataCellsFilterResourceTypeDef = TypedDict(
     "DataCellsFilterResourceTypeDef",
     {
         "TableCatalogId": str,
         "DatabaseName": str,
@@ -366,14 +385,22 @@
     {
         "FilterExpression": str,
         "AllRowsWildcard": Mapping[str, Any],
     },
     total=False,
 )
 
+DataLocationResourceOutputTypeDef = TypedDict(
+    "DataLocationResourceOutputTypeDef",
+    {
+        "CatalogId": str,
+        "ResourceArn": str,
+    },
+)
+
 _RequiredDataLocationResourceTypeDef = TypedDict(
     "_RequiredDataLocationResourceTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalDataLocationResourceTypeDef = TypedDict(
@@ -387,14 +414,22 @@
 
 class DataLocationResourceTypeDef(
     _RequiredDataLocationResourceTypeDef, _OptionalDataLocationResourceTypeDef
 ):
     pass
 
 
+DatabaseResourceOutputTypeDef = TypedDict(
+    "DatabaseResourceOutputTypeDef",
+    {
+        "CatalogId": str,
+        "Name": str,
+    },
+)
+
 _RequiredDatabaseResourceTypeDef = TypedDict(
     "_RequiredDatabaseResourceTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalDatabaseResourceTypeDef = TypedDict(
@@ -501,15 +536,14 @@
     "ResourceInfoTypeDef",
     {
         "ResourceArn": str,
         "RoleArn": str,
         "LastModified": datetime,
         "WithFederation": bool,
     },
-    total=False,
 )
 
 DescribeTransactionRequestRequestTypeDef = TypedDict(
     "DescribeTransactionRequestRequestTypeDef",
     {
         "TransactionId": str,
     },
@@ -519,33 +553,30 @@
     "TransactionDescriptionTypeDef",
     {
         "TransactionId": str,
         "TransactionStatus": TransactionStatusType,
         "TransactionStartTime": datetime,
         "TransactionEndTime": datetime,
     },
-    total=False,
 )
 
 DetailsMapTypeDef = TypedDict(
     "DetailsMapTypeDef",
     {
         "ResourceShare": List[str],
     },
-    total=False,
 )
 
 ExecutionStatisticsTypeDef = TypedDict(
     "ExecutionStatisticsTypeDef",
     {
         "AverageExecutionTimeMillis": int,
         "DataScannedBytes": int,
         "WorkUnitsExecutedCount": int,
     },
-    total=False,
 )
 
 ExtendTransactionRequestRequestTypeDef = TypedDict(
     "ExtendTransactionRequestRequestTypeDef",
     {
         "TransactionId": str,
     },
@@ -643,18 +674,43 @@
     "PlanningStatisticsTypeDef",
     {
         "EstimatedDataToScanBytes": int,
         "PlanningTimeMillis": int,
         "QueueTimeMillis": int,
         "WorkUnitsGeneratedCount": int,
     },
+)
+
+_RequiredGetTableObjectsRequestRequestTypeDef = TypedDict(
+    "_RequiredGetTableObjectsRequestRequestTypeDef",
+    {
+        "DatabaseName": str,
+        "TableName": str,
+    },
+)
+_OptionalGetTableObjectsRequestRequestTypeDef = TypedDict(
+    "_OptionalGetTableObjectsRequestRequestTypeDef",
+    {
+        "CatalogId": str,
+        "TransactionId": str,
+        "QueryAsOfTime": Union[datetime, str],
+        "PartitionPredicate": str,
+        "MaxResults": int,
+        "NextToken": str,
+    },
     total=False,
 )
 
-TimestampTypeDef = Union[datetime, str]
+
+class GetTableObjectsRequestRequestTypeDef(
+    _RequiredGetTableObjectsRequestRequestTypeDef, _OptionalGetTableObjectsRequestRequestTypeDef
+):
+    pass
+
+
 PartitionValueListTypeDef = TypedDict(
     "PartitionValueListTypeDef",
     {
         "Values": Sequence[str],
     },
 )
 
@@ -704,35 +760,22 @@
     {
         "WorkUnitIdMax": int,
         "WorkUnitIdMin": int,
         "WorkUnitToken": str,
     },
 )
 
-_RequiredLFTagKeyResourceOutputTypeDef = TypedDict(
-    "_RequiredLFTagKeyResourceOutputTypeDef",
+LFTagKeyResourceOutputTypeDef = TypedDict(
+    "LFTagKeyResourceOutputTypeDef",
     {
+        "CatalogId": str,
         "TagKey": str,
         "TagValues": List[str],
     },
 )
-_OptionalLFTagKeyResourceOutputTypeDef = TypedDict(
-    "_OptionalLFTagKeyResourceOutputTypeDef",
-    {
-        "CatalogId": str,
-    },
-    total=False,
-)
-
-
-class LFTagKeyResourceOutputTypeDef(
-    _RequiredLFTagKeyResourceOutputTypeDef, _OptionalLFTagKeyResourceOutputTypeDef
-):
-    pass
-
 
 _RequiredLFTagKeyResourceTypeDef = TypedDict(
     "_RequiredLFTagKeyResourceTypeDef",
     {
         "TagKey": str,
         "TagValues": Sequence[str],
     },
@@ -754,34 +797,14 @@
     "LFTagOutputTypeDef",
     {
         "TagKey": str,
         "TagValues": List[str],
     },
 )
 
-_RequiredLFTagPairTypeDef = TypedDict(
-    "_RequiredLFTagPairTypeDef",
-    {
-        "TagKey": str,
-        "TagValues": Sequence[str],
-    },
-)
-_OptionalLFTagPairTypeDef = TypedDict(
-    "_OptionalLFTagPairTypeDef",
-    {
-        "CatalogId": str,
-    },
-    total=False,
-)
-
-
-class LFTagPairTypeDef(_RequiredLFTagPairTypeDef, _OptionalLFTagPairTypeDef):
-    pass
-
-
 LFTagTypeDef = TypedDict(
     "LFTagTypeDef",
     {
         "TagKey": str,
         "TagValues": Sequence[str],
     },
 )
@@ -849,15 +872,14 @@
     {
         "StorageOptimizerType": OptimizerTypeType,
         "Config": Dict[str, str],
         "ErrorMessage": str,
         "Warnings": str,
         "LastRunDetails": str,
     },
-    total=False,
 )
 
 ListTransactionsRequestRequestTypeDef = TypedDict(
     "ListTransactionsRequestRequestTypeDef",
     {
         "CatalogId": str,
         "StatusFilter": TransactionStatusFilterType,
@@ -870,17 +892,40 @@
 TableObjectTypeDef = TypedDict(
     "TableObjectTypeDef",
     {
         "Uri": str,
         "ETag": str,
         "Size": int,
     },
+)
+
+_RequiredQueryPlanningContextTypeDef = TypedDict(
+    "_RequiredQueryPlanningContextTypeDef",
+    {
+        "DatabaseName": str,
+    },
+)
+_OptionalQueryPlanningContextTypeDef = TypedDict(
+    "_OptionalQueryPlanningContextTypeDef",
+    {
+        "CatalogId": str,
+        "QueryAsOfTime": Union[datetime, str],
+        "QueryParameters": Mapping[str, str],
+        "TransactionId": str,
+    },
     total=False,
 )
 
+
+class QueryPlanningContextTypeDef(
+    _RequiredQueryPlanningContextTypeDef, _OptionalQueryPlanningContextTypeDef
+):
+    pass
+
+
 _RequiredRegisterResourceRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalRegisterResourceRequestRequestTypeDef = TypedDict(
@@ -896,37 +941,24 @@
 
 class RegisterResourceRequestRequestTypeDef(
     _RequiredRegisterResourceRequestRequestTypeDef, _OptionalRegisterResourceRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredTableResourceOutputTypeDef = TypedDict(
-    "_RequiredTableResourceOutputTypeDef",
-    {
-        "DatabaseName": str,
-    },
-)
-_OptionalTableResourceOutputTypeDef = TypedDict(
-    "_OptionalTableResourceOutputTypeDef",
+TableResourceOutputTypeDef = TypedDict(
+    "TableResourceOutputTypeDef",
     {
         "CatalogId": str,
+        "DatabaseName": str,
         "Name": str,
         "TableWildcard": Dict[str, Any],
     },
-    total=False,
 )
 
-
-class TableResourceOutputTypeDef(
-    _RequiredTableResourceOutputTypeDef, _OptionalTableResourceOutputTypeDef
-):
-    pass
-
-
 StartTransactionRequestRequestTypeDef = TypedDict(
     "StartTransactionRequestRequestTypeDef",
     {
         "TransactionType": TransactionTypeType,
     },
     total=False,
 )
@@ -1116,18 +1148,17 @@
 ):
     pass
 
 
 PrincipalPermissionsOutputTypeDef = TypedDict(
     "PrincipalPermissionsOutputTypeDef",
     {
-        "Principal": DataLakePrincipalTypeDef,
+        "Principal": DataLakePrincipalOutputTypeDef,
         "Permissions": List[PermissionType],
     },
-    total=False,
 )
 
 PrincipalPermissionsTypeDef = TypedDict(
     "PrincipalPermissionsTypeDef",
     {
         "Principal": DataLakePrincipalTypeDef,
         "Permissions": Sequence[PermissionType],
@@ -1137,59 +1168,44 @@
 
 ColumnLFTagTypeDef = TypedDict(
     "ColumnLFTagTypeDef",
     {
         "Name": str,
         "LFTags": List[LFTagPairOutputTypeDef],
     },
-    total=False,
 )
 
 LFTagErrorTypeDef = TypedDict(
     "LFTagErrorTypeDef",
     {
         "LFTag": LFTagPairOutputTypeDef,
         "Error": ErrorDetailTypeDef,
     },
-    total=False,
 )
 
 ListLFTagsResponseTypeDef = TypedDict(
     "ListLFTagsResponseTypeDef",
     {
         "LFTags": List[LFTagPairOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredTableWithColumnsResourceOutputTypeDef = TypedDict(
-    "_RequiredTableWithColumnsResourceOutputTypeDef",
+TableWithColumnsResourceOutputTypeDef = TypedDict(
+    "TableWithColumnsResourceOutputTypeDef",
     {
+        "CatalogId": str,
         "DatabaseName": str,
         "Name": str,
-    },
-)
-_OptionalTableWithColumnsResourceOutputTypeDef = TypedDict(
-    "_OptionalTableWithColumnsResourceOutputTypeDef",
-    {
-        "CatalogId": str,
         "ColumnNames": List[str],
         "ColumnWildcard": ColumnWildcardOutputTypeDef,
     },
-    total=False,
 )
 
-
-class TableWithColumnsResourceOutputTypeDef(
-    _RequiredTableWithColumnsResourceOutputTypeDef, _OptionalTableWithColumnsResourceOutputTypeDef
-):
-    pass
-
-
 _RequiredTableWithColumnsResourceTypeDef = TypedDict(
     "_RequiredTableWithColumnsResourceTypeDef",
     {
         "DatabaseName": str,
         "Name": str,
     },
 )
@@ -1206,41 +1222,28 @@
 
 class TableWithColumnsResourceTypeDef(
     _RequiredTableWithColumnsResourceTypeDef, _OptionalTableWithColumnsResourceTypeDef
 ):
     pass
 
 
-_RequiredDataCellsFilterOutputTypeDef = TypedDict(
-    "_RequiredDataCellsFilterOutputTypeDef",
+DataCellsFilterOutputTypeDef = TypedDict(
+    "DataCellsFilterOutputTypeDef",
     {
         "TableCatalogId": str,
         "DatabaseName": str,
         "TableName": str,
         "Name": str,
-    },
-)
-_OptionalDataCellsFilterOutputTypeDef = TypedDict(
-    "_OptionalDataCellsFilterOutputTypeDef",
-    {
         "RowFilter": RowFilterOutputTypeDef,
         "ColumnNames": List[str],
         "ColumnWildcard": ColumnWildcardOutputTypeDef,
         "VersionId": str,
     },
-    total=False,
 )
 
-
-class DataCellsFilterOutputTypeDef(
-    _RequiredDataCellsFilterOutputTypeDef, _OptionalDataCellsFilterOutputTypeDef
-):
-    pass
-
-
 _RequiredDataCellsFilterTypeDef = TypedDict(
     "_RequiredDataCellsFilterTypeDef",
     {
         "TableCatalogId": str,
         "DatabaseName": str,
         "TableName": str,
         "Name": str,
@@ -1261,18 +1264,17 @@
 class DataCellsFilterTypeDef(_RequiredDataCellsFilterTypeDef, _OptionalDataCellsFilterTypeDef):
     pass
 
 
 TaggedDatabaseTypeDef = TypedDict(
     "TaggedDatabaseTypeDef",
     {
-        "Database": DatabaseResourceTypeDef,
+        "Database": DatabaseResourceOutputTypeDef,
         "LFTags": List[LFTagPairOutputTypeDef],
     },
-    total=False,
 )
 
 WriteOperationTypeDef = TypedDict(
     "WriteOperationTypeDef",
     {
         "AddObject": AddObjectInputTypeDef,
         "DeleteObject": DeleteObjectInputTypeDef,
@@ -1355,65 +1357,14 @@
         "ExecutionStatistics": ExecutionStatisticsTypeDef,
         "PlanningStatistics": PlanningStatisticsTypeDef,
         "QuerySubmissionTime": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredGetTableObjectsRequestRequestTypeDef = TypedDict(
-    "_RequiredGetTableObjectsRequestRequestTypeDef",
-    {
-        "DatabaseName": str,
-        "TableName": str,
-    },
-)
-_OptionalGetTableObjectsRequestRequestTypeDef = TypedDict(
-    "_OptionalGetTableObjectsRequestRequestTypeDef",
-    {
-        "CatalogId": str,
-        "TransactionId": str,
-        "QueryAsOfTime": TimestampTypeDef,
-        "PartitionPredicate": str,
-        "MaxResults": int,
-        "NextToken": str,
-    },
-    total=False,
-)
-
-
-class GetTableObjectsRequestRequestTypeDef(
-    _RequiredGetTableObjectsRequestRequestTypeDef, _OptionalGetTableObjectsRequestRequestTypeDef
-):
-    pass
-
-
-_RequiredQueryPlanningContextTypeDef = TypedDict(
-    "_RequiredQueryPlanningContextTypeDef",
-    {
-        "DatabaseName": str,
-    },
-)
-_OptionalQueryPlanningContextTypeDef = TypedDict(
-    "_OptionalQueryPlanningContextTypeDef",
-    {
-        "CatalogId": str,
-        "QueryAsOfTime": TimestampTypeDef,
-        "QueryParameters": Mapping[str, str],
-        "TransactionId": str,
-    },
-    total=False,
-)
-
-
-class QueryPlanningContextTypeDef(
-    _RequiredQueryPlanningContextTypeDef, _OptionalQueryPlanningContextTypeDef
-):
-    pass
-
-
 _RequiredGetTemporaryGluePartitionCredentialsRequestRequestTypeDef = TypedDict(
     "_RequiredGetTemporaryGluePartitionCredentialsRequestRequestTypeDef",
     {
         "TableArn": str,
         "Partition": PartitionValueListTypeDef,
     },
 )
@@ -1474,60 +1425,139 @@
         "NextToken": str,
         "QueryId": str,
         "WorkUnitRanges": List[WorkUnitRangeTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredLFTagPolicyResourceOutputTypeDef = TypedDict(
-    "_RequiredLFTagPolicyResourceOutputTypeDef",
+LFTagPolicyResourceOutputTypeDef = TypedDict(
+    "LFTagPolicyResourceOutputTypeDef",
     {
+        "CatalogId": str,
         "ResourceType": ResourceTypeType,
         "Expression": List[LFTagOutputTypeDef],
     },
 )
-_OptionalLFTagPolicyResourceOutputTypeDef = TypedDict(
-    "_OptionalLFTagPolicyResourceOutputTypeDef",
+
+_RequiredLFTagPolicyResourceTypeDef = TypedDict(
+    "_RequiredLFTagPolicyResourceTypeDef",
+    {
+        "ResourceType": ResourceTypeType,
+        "Expression": Sequence[LFTagTypeDef],
+    },
+)
+_OptionalLFTagPolicyResourceTypeDef = TypedDict(
+    "_OptionalLFTagPolicyResourceTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
 
-class LFTagPolicyResourceOutputTypeDef(
-    _RequiredLFTagPolicyResourceOutputTypeDef, _OptionalLFTagPolicyResourceOutputTypeDef
+class LFTagPolicyResourceTypeDef(
+    _RequiredLFTagPolicyResourceTypeDef, _OptionalLFTagPolicyResourceTypeDef
 ):
     pass
 
 
-LFTagPairUnionTypeDef = Union[LFTagPairTypeDef, LFTagPairOutputTypeDef]
-_RequiredLFTagPolicyResourceTypeDef = TypedDict(
-    "_RequiredLFTagPolicyResourceTypeDef",
+_RequiredSearchDatabasesByLFTagsRequestRequestTypeDef = TypedDict(
+    "_RequiredSearchDatabasesByLFTagsRequestRequestTypeDef",
     {
-        "ResourceType": ResourceTypeType,
         "Expression": Sequence[LFTagTypeDef],
     },
 )
-_OptionalLFTagPolicyResourceTypeDef = TypedDict(
-    "_OptionalLFTagPolicyResourceTypeDef",
+_OptionalSearchDatabasesByLFTagsRequestRequestTypeDef = TypedDict(
+    "_OptionalSearchDatabasesByLFTagsRequestRequestTypeDef",
     {
+        "NextToken": str,
+        "MaxResults": int,
         "CatalogId": str,
     },
     total=False,
 )
 
 
-class LFTagPolicyResourceTypeDef(
-    _RequiredLFTagPolicyResourceTypeDef, _OptionalLFTagPolicyResourceTypeDef
+class SearchDatabasesByLFTagsRequestRequestTypeDef(
+    _RequiredSearchDatabasesByLFTagsRequestRequestTypeDef,
+    _OptionalSearchDatabasesByLFTagsRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredSearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef = TypedDict(
+    "_RequiredSearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef",
+    {
+        "Expression": Sequence[LFTagTypeDef],
+    },
+)
+_OptionalSearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef = TypedDict(
+    "_OptionalSearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef",
+    {
+        "CatalogId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class SearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef(
+    _RequiredSearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef,
+    _OptionalSearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredSearchTablesByLFTagsRequestRequestTypeDef = TypedDict(
+    "_RequiredSearchTablesByLFTagsRequestRequestTypeDef",
+    {
+        "Expression": Sequence[LFTagTypeDef],
+    },
+)
+_OptionalSearchTablesByLFTagsRequestRequestTypeDef = TypedDict(
+    "_OptionalSearchTablesByLFTagsRequestRequestTypeDef",
+    {
+        "NextToken": str,
+        "MaxResults": int,
+        "CatalogId": str,
+    },
+    total=False,
+)
+
+
+class SearchTablesByLFTagsRequestRequestTypeDef(
+    _RequiredSearchTablesByLFTagsRequestRequestTypeDef,
+    _OptionalSearchTablesByLFTagsRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredSearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef = TypedDict(
+    "_RequiredSearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef",
+    {
+        "Expression": Sequence[LFTagTypeDef],
+    },
+)
+_OptionalSearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef = TypedDict(
+    "_OptionalSearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef",
+    {
+        "CatalogId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class SearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef(
+    _RequiredSearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef,
+    _OptionalSearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef,
 ):
     pass
 
 
-LFTagUnionTypeDef = Union[LFTagTypeDef, LFTagOutputTypeDef]
 ListDataCellsFilterRequestListDataCellsFilterPaginateTypeDef = TypedDict(
     "ListDataCellsFilterRequestListDataCellsFilterPaginateTypeDef",
     {
         "Table": TableResourceTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -1554,33 +1584,38 @@
 
 PartitionObjectsTypeDef = TypedDict(
     "PartitionObjectsTypeDef",
     {
         "PartitionValues": List[str],
         "Objects": List[TableObjectTypeDef],
     },
-    total=False,
 )
 
-TableResourceUnionTypeDef = Union[TableResourceTypeDef, TableResourceOutputTypeDef]
+StartQueryPlanningRequestRequestTypeDef = TypedDict(
+    "StartQueryPlanningRequestRequestTypeDef",
+    {
+        "QueryPlanningContext": QueryPlanningContextTypeDef,
+        "QueryString": str,
+    },
+)
+
 DataLakeSettingsOutputTypeDef = TypedDict(
     "DataLakeSettingsOutputTypeDef",
     {
-        "DataLakeAdmins": List[DataLakePrincipalTypeDef],
-        "ReadOnlyAdmins": List[DataLakePrincipalTypeDef],
+        "DataLakeAdmins": List[DataLakePrincipalOutputTypeDef],
+        "ReadOnlyAdmins": List[DataLakePrincipalOutputTypeDef],
         "CreateDatabaseDefaultPermissions": List[PrincipalPermissionsOutputTypeDef],
         "CreateTableDefaultPermissions": List[PrincipalPermissionsOutputTypeDef],
         "Parameters": Dict[str, str],
         "TrustedResourceOwners": List[str],
         "AllowExternalDataFiltering": bool,
         "AllowFullTableExternalDataAccess": bool,
-        "ExternalDataFilteringAllowList": List[DataLakePrincipalTypeDef],
+        "ExternalDataFilteringAllowList": List[DataLakePrincipalOutputTypeDef],
         "AuthorizedSessionTagValueList": List[str],
     },
-    total=False,
 )
 
 DataLakeSettingsTypeDef = TypedDict(
     "DataLakeSettingsTypeDef",
     {
         "DataLakeAdmins": Sequence[DataLakePrincipalTypeDef],
         "ReadOnlyAdmins": Sequence[DataLakePrincipalTypeDef],
@@ -1610,15 +1645,14 @@
     "TaggedTableTypeDef",
     {
         "Table": TableResourceOutputTypeDef,
         "LFTagOnDatabase": List[LFTagPairOutputTypeDef],
         "LFTagsOnTable": List[LFTagPairOutputTypeDef],
         "LFTagsOnColumns": List[ColumnLFTagTypeDef],
     },
-    total=False,
 )
 
 AddLFTagsToResourceResponseTypeDef = TypedDict(
     "AddLFTagsToResourceResponseTypeDef",
     {
         "Failures": List[LFTagErrorTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1653,15 +1687,14 @@
 CreateDataCellsFilterRequestRequestTypeDef = TypedDict(
     "CreateDataCellsFilterRequestRequestTypeDef",
     {
         "TableData": DataCellsFilterTypeDef,
     },
 )
 
-DataCellsFilterUnionTypeDef = Union[DataCellsFilterTypeDef, DataCellsFilterOutputTypeDef]
 UpdateDataCellsFilterRequestRequestTypeDef = TypedDict(
     "UpdateDataCellsFilterRequestRequestTypeDef",
     {
         "TableData": DataCellsFilterTypeDef,
     },
 )
 
@@ -1695,35 +1728,26 @@
 class UpdateTableObjectsRequestRequestTypeDef(
     _RequiredUpdateTableObjectsRequestRequestTypeDef,
     _OptionalUpdateTableObjectsRequestRequestTypeDef,
 ):
     pass
 
 
-StartQueryPlanningRequestRequestTypeDef = TypedDict(
-    "StartQueryPlanningRequestRequestTypeDef",
-    {
-        "QueryPlanningContext": QueryPlanningContextTypeDef,
-        "QueryString": str,
-    },
-)
-
 ResourceOutputTypeDef = TypedDict(
     "ResourceOutputTypeDef",
     {
         "Catalog": Dict[str, Any],
-        "Database": DatabaseResourceTypeDef,
+        "Database": DatabaseResourceOutputTypeDef,
         "Table": TableResourceOutputTypeDef,
         "TableWithColumns": TableWithColumnsResourceOutputTypeDef,
-        "DataLocation": DataLocationResourceTypeDef,
-        "DataCellsFilter": DataCellsFilterResourceTypeDef,
+        "DataLocation": DataLocationResourceOutputTypeDef,
+        "DataCellsFilter": DataCellsFilterResourceOutputTypeDef,
         "LFTag": LFTagKeyResourceOutputTypeDef,
         "LFTagPolicy": LFTagPolicyResourceOutputTypeDef,
     },
-    total=False,
 )
 
 ResourceTypeDef = TypedDict(
     "ResourceTypeDef",
     {
         "Catalog": Mapping[str, Any],
         "Database": DatabaseResourceTypeDef,
@@ -1733,108 +1757,14 @@
         "DataCellsFilter": DataCellsFilterResourceTypeDef,
         "LFTag": LFTagKeyResourceTypeDef,
         "LFTagPolicy": LFTagPolicyResourceTypeDef,
     },
     total=False,
 )
 
-_RequiredSearchDatabasesByLFTagsRequestRequestTypeDef = TypedDict(
-    "_RequiredSearchDatabasesByLFTagsRequestRequestTypeDef",
-    {
-        "Expression": Sequence[LFTagUnionTypeDef],
-    },
-)
-_OptionalSearchDatabasesByLFTagsRequestRequestTypeDef = TypedDict(
-    "_OptionalSearchDatabasesByLFTagsRequestRequestTypeDef",
-    {
-        "NextToken": str,
-        "MaxResults": int,
-        "CatalogId": str,
-    },
-    total=False,
-)
-
-
-class SearchDatabasesByLFTagsRequestRequestTypeDef(
-    _RequiredSearchDatabasesByLFTagsRequestRequestTypeDef,
-    _OptionalSearchDatabasesByLFTagsRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredSearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef = TypedDict(
-    "_RequiredSearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef",
-    {
-        "Expression": Sequence[LFTagUnionTypeDef],
-    },
-)
-_OptionalSearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef = TypedDict(
-    "_OptionalSearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef",
-    {
-        "CatalogId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class SearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef(
-    _RequiredSearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef,
-    _OptionalSearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredSearchTablesByLFTagsRequestRequestTypeDef = TypedDict(
-    "_RequiredSearchTablesByLFTagsRequestRequestTypeDef",
-    {
-        "Expression": Sequence[LFTagUnionTypeDef],
-    },
-)
-_OptionalSearchTablesByLFTagsRequestRequestTypeDef = TypedDict(
-    "_OptionalSearchTablesByLFTagsRequestRequestTypeDef",
-    {
-        "NextToken": str,
-        "MaxResults": int,
-        "CatalogId": str,
-    },
-    total=False,
-)
-
-
-class SearchTablesByLFTagsRequestRequestTypeDef(
-    _RequiredSearchTablesByLFTagsRequestRequestTypeDef,
-    _OptionalSearchTablesByLFTagsRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredSearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef = TypedDict(
-    "_RequiredSearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef",
-    {
-        "Expression": Sequence[LFTagUnionTypeDef],
-    },
-)
-_OptionalSearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef = TypedDict(
-    "_OptionalSearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef",
-    {
-        "CatalogId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class SearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef(
-    _RequiredSearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef,
-    _OptionalSearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef,
-):
-    pass
-
-
 GetTableObjectsResponseTypeDef = TypedDict(
     "GetTableObjectsResponseTypeDef",
     {
         "Objects": List[PartitionObjectsTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1844,15 +1774,14 @@
     "GetDataLakeSettingsResponseTypeDef",
     {
         "DataLakeSettings": DataLakeSettingsOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DataLakeSettingsUnionTypeDef = Union[DataLakeSettingsTypeDef, DataLakeSettingsOutputTypeDef]
 _RequiredPutDataLakeSettingsRequestRequestTypeDef = TypedDict(
     "_RequiredPutDataLakeSettingsRequestRequestTypeDef",
     {
         "DataLakeSettings": DataLakeSettingsTypeDef,
     },
 )
 _OptionalPutDataLakeSettingsRequestRequestTypeDef = TypedDict(
@@ -1876,56 +1805,41 @@
     {
         "NextToken": str,
         "TableList": List[TaggedTableTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredBatchPermissionsRequestEntryOutputTypeDef = TypedDict(
-    "_RequiredBatchPermissionsRequestEntryOutputTypeDef",
+BatchPermissionsRequestEntryOutputTypeDef = TypedDict(
+    "BatchPermissionsRequestEntryOutputTypeDef",
     {
         "Id": str,
-    },
-)
-_OptionalBatchPermissionsRequestEntryOutputTypeDef = TypedDict(
-    "_OptionalBatchPermissionsRequestEntryOutputTypeDef",
-    {
-        "Principal": DataLakePrincipalTypeDef,
+        "Principal": DataLakePrincipalOutputTypeDef,
         "Resource": ResourceOutputTypeDef,
         "Permissions": List[PermissionType],
         "PermissionsWithGrantOption": List[PermissionType],
     },
-    total=False,
 )
 
-
-class BatchPermissionsRequestEntryOutputTypeDef(
-    _RequiredBatchPermissionsRequestEntryOutputTypeDef,
-    _OptionalBatchPermissionsRequestEntryOutputTypeDef,
-):
-    pass
-
-
 PrincipalResourcePermissionsTypeDef = TypedDict(
     "PrincipalResourcePermissionsTypeDef",
     {
-        "Principal": DataLakePrincipalTypeDef,
+        "Principal": DataLakePrincipalOutputTypeDef,
         "Resource": ResourceOutputTypeDef,
         "Permissions": List[PermissionType],
         "PermissionsWithGrantOption": List[PermissionType],
         "AdditionalDetails": DetailsMapTypeDef,
     },
-    total=False,
 )
 
 _RequiredAddLFTagsToResourceRequestRequestTypeDef = TypedDict(
     "_RequiredAddLFTagsToResourceRequestRequestTypeDef",
     {
         "Resource": ResourceTypeDef,
-        "LFTags": Sequence[LFTagPairUnionTypeDef],
+        "LFTags": Sequence[LFTagPairTypeDef],
     },
 )
 _OptionalAddLFTagsToResourceRequestRequestTypeDef = TypedDict(
     "_OptionalAddLFTagsToResourceRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
@@ -2024,15 +1938,15 @@
     total=False,
 )
 
 _RequiredRemoveLFTagsFromResourceRequestRequestTypeDef = TypedDict(
     "_RequiredRemoveLFTagsFromResourceRequestRequestTypeDef",
     {
         "Resource": ResourceTypeDef,
-        "LFTags": Sequence[LFTagPairUnionTypeDef],
+        "LFTags": Sequence[LFTagPairTypeDef],
     },
 )
 _OptionalRemoveLFTagsFromResourceRequestRequestTypeDef = TypedDict(
     "_OptionalRemoveLFTagsFromResourceRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
@@ -2043,15 +1957,14 @@
 class RemoveLFTagsFromResourceRequestRequestTypeDef(
     _RequiredRemoveLFTagsFromResourceRequestRequestTypeDef,
     _OptionalRemoveLFTagsFromResourceRequestRequestTypeDef,
 ):
     pass
 
 
-ResourceUnionTypeDef = Union[ResourceTypeDef, ResourceOutputTypeDef]
 _RequiredRevokePermissionsRequestRequestTypeDef = TypedDict(
     "_RequiredRevokePermissionsRequestRequestTypeDef",
     {
         "Principal": DataLakePrincipalTypeDef,
         "Resource": ResourceTypeDef,
         "Permissions": Sequence[PermissionType],
     },
@@ -2074,15 +1987,14 @@
 
 BatchPermissionsFailureEntryTypeDef = TypedDict(
     "BatchPermissionsFailureEntryTypeDef",
     {
         "RequestEntry": BatchPermissionsRequestEntryOutputTypeDef,
         "Error": ErrorDetailTypeDef,
     },
-    total=False,
 )
 
 GetEffectivePermissionsForPathResponseTypeDef = TypedDict(
     "GetEffectivePermissionsForPathResponseTypeDef",
     {
         "Permissions": List[PrincipalResourcePermissionsTypeDef],
         "NextToken": str,
@@ -2095,37 +2007,18 @@
     {
         "PrincipalResourcePermissions": List[PrincipalResourcePermissionsTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BatchPermissionsRequestEntryUnionTypeDef = Union[
-    BatchPermissionsRequestEntryTypeDef, BatchPermissionsRequestEntryOutputTypeDef
-]
-BatchGrantPermissionsResponseTypeDef = TypedDict(
-    "BatchGrantPermissionsResponseTypeDef",
-    {
-        "Failures": List[BatchPermissionsFailureEntryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-BatchRevokePermissionsResponseTypeDef = TypedDict(
-    "BatchRevokePermissionsResponseTypeDef",
-    {
-        "Failures": List[BatchPermissionsFailureEntryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredBatchGrantPermissionsRequestRequestTypeDef = TypedDict(
     "_RequiredBatchGrantPermissionsRequestRequestTypeDef",
     {
-        "Entries": Sequence[BatchPermissionsRequestEntryUnionTypeDef],
+        "Entries": Sequence[BatchPermissionsRequestEntryTypeDef],
     },
 )
 _OptionalBatchGrantPermissionsRequestRequestTypeDef = TypedDict(
     "_OptionalBatchGrantPermissionsRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
@@ -2139,15 +2032,15 @@
 ):
     pass
 
 
 _RequiredBatchRevokePermissionsRequestRequestTypeDef = TypedDict(
     "_RequiredBatchRevokePermissionsRequestRequestTypeDef",
     {
-        "Entries": Sequence[BatchPermissionsRequestEntryUnionTypeDef],
+        "Entries": Sequence[BatchPermissionsRequestEntryTypeDef],
     },
 )
 _OptionalBatchRevokePermissionsRequestRequestTypeDef = TypedDict(
     "_OptionalBatchRevokePermissionsRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
@@ -2156,7 +2049,24 @@
 
 
 class BatchRevokePermissionsRequestRequestTypeDef(
     _RequiredBatchRevokePermissionsRequestRequestTypeDef,
     _OptionalBatchRevokePermissionsRequestRequestTypeDef,
 ):
     pass
+
+
+BatchGrantPermissionsResponseTypeDef = TypedDict(
+    "BatchGrantPermissionsResponseTypeDef",
+    {
+        "Failures": List[BatchPermissionsFailureEntryTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+BatchRevokePermissionsResponseTypeDef = TypedDict(
+    "BatchRevokePermissionsResponseTypeDef",
+    {
+        "Failures": List[BatchPermissionsFailureEntryTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
```

### Comparing `mypy-boto3-lakeformation-1.28.16/mypy_boto3_lakeformation/type_defs.pyi` & `mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for lakeformation service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_lakeformation.type_defs import ResponseMetadataTypeDef
+    from mypy_boto3_lakeformation.type_defs import LFTagPairTypeDef
 
-    data: ResponseMetadataTypeDef = ...
+    data: LFTagPairTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -34,30 +34,35 @@
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
+    "LFTagPairTypeDef",
     "ResponseMetadataTypeDef",
     "AddObjectInputTypeDef",
     "AssumeDecoratedRoleWithSAMLRequestRequestTypeDef",
     "AuditContextTypeDef",
     "ErrorDetailTypeDef",
+    "DataLakePrincipalOutputTypeDef",
     "DataLakePrincipalTypeDef",
     "CancelTransactionRequestRequestTypeDef",
     "LFTagPairOutputTypeDef",
     "ColumnWildcardOutputTypeDef",
     "ColumnWildcardTypeDef",
     "CommitTransactionRequestRequestTypeDef",
     "CreateLFTagRequestRequestTypeDef",
     "RowFilterOutputTypeDef",
+    "DataCellsFilterResourceOutputTypeDef",
     "DataCellsFilterResourceTypeDef",
     "RowFilterTypeDef",
+    "DataLocationResourceOutputTypeDef",
     "DataLocationResourceTypeDef",
+    "DatabaseResourceOutputTypeDef",
     "DatabaseResourceTypeDef",
     "DeleteDataCellsFilterRequestRequestTypeDef",
     "DeleteLFTagRequestRequestTypeDef",
     "DeleteObjectInputTypeDef",
     "VirtualObjectTypeDef",
     "DeregisterResourceRequestRequestTypeDef",
     "DescribeResourceRequestRequestTypeDef",
@@ -71,31 +76,31 @@
     "GetDataCellsFilterRequestRequestTypeDef",
     "GetDataLakeSettingsRequestRequestTypeDef",
     "GetEffectivePermissionsForPathRequestRequestTypeDef",
     "GetLFTagRequestRequestTypeDef",
     "GetQueryStateRequestRequestTypeDef",
     "GetQueryStatisticsRequestRequestTypeDef",
     "PlanningStatisticsTypeDef",
-    "TimestampTypeDef",
+    "GetTableObjectsRequestRequestTypeDef",
     "PartitionValueListTypeDef",
     "GetWorkUnitResultsRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "GetWorkUnitsRequestRequestTypeDef",
     "WorkUnitRangeTypeDef",
     "LFTagKeyResourceOutputTypeDef",
     "LFTagKeyResourceTypeDef",
     "LFTagOutputTypeDef",
-    "LFTagPairTypeDef",
     "LFTagTypeDef",
     "TableResourceTypeDef",
     "ListLFTagsRequestRequestTypeDef",
     "ListTableStorageOptimizersRequestRequestTypeDef",
     "StorageOptimizerTypeDef",
     "ListTransactionsRequestRequestTypeDef",
     "TableObjectTypeDef",
+    "QueryPlanningContextTypeDef",
     "RegisterResourceRequestRequestTypeDef",
     "TableResourceOutputTypeDef",
     "StartTransactionRequestRequestTypeDef",
     "UpdateLFTagRequestRequestTypeDef",
     "UpdateResourceRequestRequestTypeDef",
     "UpdateTableStorageOptimizerRequestRequestTypeDef",
     "AssumeDecoratedRoleWithSAMLResponseTypeDef",
@@ -123,74 +128,83 @@
     "DeleteObjectsOnCancelRequestRequestTypeDef",
     "DescribeResourceResponseTypeDef",
     "ListResourcesResponseTypeDef",
     "DescribeTransactionResponseTypeDef",
     "ListTransactionsResponseTypeDef",
     "ListResourcesRequestRequestTypeDef",
     "GetQueryStatisticsResponseTypeDef",
-    "GetTableObjectsRequestRequestTypeDef",
-    "QueryPlanningContextTypeDef",
     "GetTemporaryGluePartitionCredentialsRequestRequestTypeDef",
     "GetWorkUnitsRequestGetWorkUnitsPaginateTypeDef",
     "ListLFTagsRequestListLFTagsPaginateTypeDef",
     "GetWorkUnitsResponseTypeDef",
     "LFTagPolicyResourceOutputTypeDef",
-    "LFTagPairUnionTypeDef",
     "LFTagPolicyResourceTypeDef",
-    "LFTagUnionTypeDef",
+    "SearchDatabasesByLFTagsRequestRequestTypeDef",
+    "SearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef",
+    "SearchTablesByLFTagsRequestRequestTypeDef",
+    "SearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef",
     "ListDataCellsFilterRequestListDataCellsFilterPaginateTypeDef",
     "ListDataCellsFilterRequestRequestTypeDef",
     "ListTableStorageOptimizersResponseTypeDef",
     "PartitionObjectsTypeDef",
-    "TableResourceUnionTypeDef",
+    "StartQueryPlanningRequestRequestTypeDef",
     "DataLakeSettingsOutputTypeDef",
     "DataLakeSettingsTypeDef",
     "GetResourceLFTagsResponseTypeDef",
     "TaggedTableTypeDef",
     "AddLFTagsToResourceResponseTypeDef",
     "RemoveLFTagsFromResourceResponseTypeDef",
     "GetDataCellsFilterResponseTypeDef",
     "ListDataCellsFilterResponseTypeDef",
     "CreateDataCellsFilterRequestRequestTypeDef",
-    "DataCellsFilterUnionTypeDef",
     "UpdateDataCellsFilterRequestRequestTypeDef",
     "SearchDatabasesByLFTagsResponseTypeDef",
     "UpdateTableObjectsRequestRequestTypeDef",
-    "StartQueryPlanningRequestRequestTypeDef",
     "ResourceOutputTypeDef",
     "ResourceTypeDef",
-    "SearchDatabasesByLFTagsRequestRequestTypeDef",
-    "SearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef",
-    "SearchTablesByLFTagsRequestRequestTypeDef",
-    "SearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef",
     "GetTableObjectsResponseTypeDef",
     "GetDataLakeSettingsResponseTypeDef",
-    "DataLakeSettingsUnionTypeDef",
     "PutDataLakeSettingsRequestRequestTypeDef",
     "SearchTablesByLFTagsResponseTypeDef",
     "BatchPermissionsRequestEntryOutputTypeDef",
     "PrincipalResourcePermissionsTypeDef",
     "AddLFTagsToResourceRequestRequestTypeDef",
     "BatchPermissionsRequestEntryTypeDef",
     "GetResourceLFTagsRequestRequestTypeDef",
     "GrantPermissionsRequestRequestTypeDef",
     "ListPermissionsRequestRequestTypeDef",
     "RemoveLFTagsFromResourceRequestRequestTypeDef",
-    "ResourceUnionTypeDef",
     "RevokePermissionsRequestRequestTypeDef",
     "BatchPermissionsFailureEntryTypeDef",
     "GetEffectivePermissionsForPathResponseTypeDef",
     "ListPermissionsResponseTypeDef",
-    "BatchPermissionsRequestEntryUnionTypeDef",
-    "BatchGrantPermissionsResponseTypeDef",
-    "BatchRevokePermissionsResponseTypeDef",
     "BatchGrantPermissionsRequestRequestTypeDef",
     "BatchRevokePermissionsRequestRequestTypeDef",
+    "BatchGrantPermissionsResponseTypeDef",
+    "BatchRevokePermissionsResponseTypeDef",
+)
+
+_RequiredLFTagPairTypeDef = TypedDict(
+    "_RequiredLFTagPairTypeDef",
+    {
+        "TagKey": str,
+        "TagValues": Sequence[str],
+    },
+)
+_OptionalLFTagPairTypeDef = TypedDict(
+    "_OptionalLFTagPairTypeDef",
+    {
+        "CatalogId": str,
+    },
+    total=False,
 )
 
+class LFTagPairTypeDef(_RequiredLFTagPairTypeDef, _OptionalLFTagPairTypeDef):
+    pass
+
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -249,15 +263,21 @@
 
 ErrorDetailTypeDef = TypedDict(
     "ErrorDetailTypeDef",
     {
         "ErrorCode": str,
         "ErrorMessage": str,
     },
-    total=False,
+)
+
+DataLakePrincipalOutputTypeDef = TypedDict(
+    "DataLakePrincipalOutputTypeDef",
+    {
+        "DataLakePrincipalIdentifier": str,
+    },
 )
 
 DataLakePrincipalTypeDef = TypedDict(
     "DataLakePrincipalTypeDef",
     {
         "DataLakePrincipalIdentifier": str,
     },
@@ -267,38 +287,28 @@
 CancelTransactionRequestRequestTypeDef = TypedDict(
     "CancelTransactionRequestRequestTypeDef",
     {
         "TransactionId": str,
     },
 )
 
-_RequiredLFTagPairOutputTypeDef = TypedDict(
-    "_RequiredLFTagPairOutputTypeDef",
+LFTagPairOutputTypeDef = TypedDict(
+    "LFTagPairOutputTypeDef",
     {
+        "CatalogId": str,
         "TagKey": str,
         "TagValues": List[str],
     },
 )
-_OptionalLFTagPairOutputTypeDef = TypedDict(
-    "_OptionalLFTagPairOutputTypeDef",
-    {
-        "CatalogId": str,
-    },
-    total=False,
-)
-
-class LFTagPairOutputTypeDef(_RequiredLFTagPairOutputTypeDef, _OptionalLFTagPairOutputTypeDef):
-    pass
 
 ColumnWildcardOutputTypeDef = TypedDict(
     "ColumnWildcardOutputTypeDef",
     {
         "ExcludedColumnNames": List[str],
     },
-    total=False,
 )
 
 ColumnWildcardTypeDef = TypedDict(
     "ColumnWildcardTypeDef",
     {
         "ExcludedColumnNames": Sequence[str],
     },
@@ -334,15 +344,24 @@
 
 RowFilterOutputTypeDef = TypedDict(
     "RowFilterOutputTypeDef",
     {
         "FilterExpression": str,
         "AllRowsWildcard": Dict[str, Any],
     },
-    total=False,
+)
+
+DataCellsFilterResourceOutputTypeDef = TypedDict(
+    "DataCellsFilterResourceOutputTypeDef",
+    {
+        "TableCatalogId": str,
+        "DatabaseName": str,
+        "TableName": str,
+        "Name": str,
+    },
 )
 
 DataCellsFilterResourceTypeDef = TypedDict(
     "DataCellsFilterResourceTypeDef",
     {
         "TableCatalogId": str,
         "DatabaseName": str,
@@ -357,14 +376,22 @@
     {
         "FilterExpression": str,
         "AllRowsWildcard": Mapping[str, Any],
     },
     total=False,
 )
 
+DataLocationResourceOutputTypeDef = TypedDict(
+    "DataLocationResourceOutputTypeDef",
+    {
+        "CatalogId": str,
+        "ResourceArn": str,
+    },
+)
+
 _RequiredDataLocationResourceTypeDef = TypedDict(
     "_RequiredDataLocationResourceTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalDataLocationResourceTypeDef = TypedDict(
@@ -376,14 +403,22 @@
 )
 
 class DataLocationResourceTypeDef(
     _RequiredDataLocationResourceTypeDef, _OptionalDataLocationResourceTypeDef
 ):
     pass
 
+DatabaseResourceOutputTypeDef = TypedDict(
+    "DatabaseResourceOutputTypeDef",
+    {
+        "CatalogId": str,
+        "Name": str,
+    },
+)
+
 _RequiredDatabaseResourceTypeDef = TypedDict(
     "_RequiredDatabaseResourceTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalDatabaseResourceTypeDef = TypedDict(
@@ -482,15 +517,14 @@
     "ResourceInfoTypeDef",
     {
         "ResourceArn": str,
         "RoleArn": str,
         "LastModified": datetime,
         "WithFederation": bool,
     },
-    total=False,
 )
 
 DescribeTransactionRequestRequestTypeDef = TypedDict(
     "DescribeTransactionRequestRequestTypeDef",
     {
         "TransactionId": str,
     },
@@ -500,33 +534,30 @@
     "TransactionDescriptionTypeDef",
     {
         "TransactionId": str,
         "TransactionStatus": TransactionStatusType,
         "TransactionStartTime": datetime,
         "TransactionEndTime": datetime,
     },
-    total=False,
 )
 
 DetailsMapTypeDef = TypedDict(
     "DetailsMapTypeDef",
     {
         "ResourceShare": List[str],
     },
-    total=False,
 )
 
 ExecutionStatisticsTypeDef = TypedDict(
     "ExecutionStatisticsTypeDef",
     {
         "AverageExecutionTimeMillis": int,
         "DataScannedBytes": int,
         "WorkUnitsExecutedCount": int,
     },
-    total=False,
 )
 
 ExtendTransactionRequestRequestTypeDef = TypedDict(
     "ExtendTransactionRequestRequestTypeDef",
     {
         "TransactionId": str,
     },
@@ -620,18 +651,41 @@
     "PlanningStatisticsTypeDef",
     {
         "EstimatedDataToScanBytes": int,
         "PlanningTimeMillis": int,
         "QueueTimeMillis": int,
         "WorkUnitsGeneratedCount": int,
     },
+)
+
+_RequiredGetTableObjectsRequestRequestTypeDef = TypedDict(
+    "_RequiredGetTableObjectsRequestRequestTypeDef",
+    {
+        "DatabaseName": str,
+        "TableName": str,
+    },
+)
+_OptionalGetTableObjectsRequestRequestTypeDef = TypedDict(
+    "_OptionalGetTableObjectsRequestRequestTypeDef",
+    {
+        "CatalogId": str,
+        "TransactionId": str,
+        "QueryAsOfTime": Union[datetime, str],
+        "PartitionPredicate": str,
+        "MaxResults": int,
+        "NextToken": str,
+    },
     total=False,
 )
 
-TimestampTypeDef = Union[datetime, str]
+class GetTableObjectsRequestRequestTypeDef(
+    _RequiredGetTableObjectsRequestRequestTypeDef, _OptionalGetTableObjectsRequestRequestTypeDef
+):
+    pass
+
 PartitionValueListTypeDef = TypedDict(
     "PartitionValueListTypeDef",
     {
         "Values": Sequence[str],
     },
 )
 
@@ -679,33 +733,22 @@
     {
         "WorkUnitIdMax": int,
         "WorkUnitIdMin": int,
         "WorkUnitToken": str,
     },
 )
 
-_RequiredLFTagKeyResourceOutputTypeDef = TypedDict(
-    "_RequiredLFTagKeyResourceOutputTypeDef",
+LFTagKeyResourceOutputTypeDef = TypedDict(
+    "LFTagKeyResourceOutputTypeDef",
     {
+        "CatalogId": str,
         "TagKey": str,
         "TagValues": List[str],
     },
 )
-_OptionalLFTagKeyResourceOutputTypeDef = TypedDict(
-    "_OptionalLFTagKeyResourceOutputTypeDef",
-    {
-        "CatalogId": str,
-    },
-    total=False,
-)
-
-class LFTagKeyResourceOutputTypeDef(
-    _RequiredLFTagKeyResourceOutputTypeDef, _OptionalLFTagKeyResourceOutputTypeDef
-):
-    pass
 
 _RequiredLFTagKeyResourceTypeDef = TypedDict(
     "_RequiredLFTagKeyResourceTypeDef",
     {
         "TagKey": str,
         "TagValues": Sequence[str],
     },
@@ -725,32 +768,14 @@
     "LFTagOutputTypeDef",
     {
         "TagKey": str,
         "TagValues": List[str],
     },
 )
 
-_RequiredLFTagPairTypeDef = TypedDict(
-    "_RequiredLFTagPairTypeDef",
-    {
-        "TagKey": str,
-        "TagValues": Sequence[str],
-    },
-)
-_OptionalLFTagPairTypeDef = TypedDict(
-    "_OptionalLFTagPairTypeDef",
-    {
-        "CatalogId": str,
-    },
-    total=False,
-)
-
-class LFTagPairTypeDef(_RequiredLFTagPairTypeDef, _OptionalLFTagPairTypeDef):
-    pass
-
 LFTagTypeDef = TypedDict(
     "LFTagTypeDef",
     {
         "TagKey": str,
         "TagValues": Sequence[str],
     },
 )
@@ -814,15 +839,14 @@
     {
         "StorageOptimizerType": OptimizerTypeType,
         "Config": Dict[str, str],
         "ErrorMessage": str,
         "Warnings": str,
         "LastRunDetails": str,
     },
-    total=False,
 )
 
 ListTransactionsRequestRequestTypeDef = TypedDict(
     "ListTransactionsRequestRequestTypeDef",
     {
         "CatalogId": str,
         "StatusFilter": TransactionStatusFilterType,
@@ -835,17 +859,38 @@
 TableObjectTypeDef = TypedDict(
     "TableObjectTypeDef",
     {
         "Uri": str,
         "ETag": str,
         "Size": int,
     },
+)
+
+_RequiredQueryPlanningContextTypeDef = TypedDict(
+    "_RequiredQueryPlanningContextTypeDef",
+    {
+        "DatabaseName": str,
+    },
+)
+_OptionalQueryPlanningContextTypeDef = TypedDict(
+    "_OptionalQueryPlanningContextTypeDef",
+    {
+        "CatalogId": str,
+        "QueryAsOfTime": Union[datetime, str],
+        "QueryParameters": Mapping[str, str],
+        "TransactionId": str,
+    },
     total=False,
 )
 
+class QueryPlanningContextTypeDef(
+    _RequiredQueryPlanningContextTypeDef, _OptionalQueryPlanningContextTypeDef
+):
+    pass
+
 _RequiredRegisterResourceRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalRegisterResourceRequestRequestTypeDef = TypedDict(
@@ -859,35 +904,24 @@
 )
 
 class RegisterResourceRequestRequestTypeDef(
     _RequiredRegisterResourceRequestRequestTypeDef, _OptionalRegisterResourceRequestRequestTypeDef
 ):
     pass
 
-_RequiredTableResourceOutputTypeDef = TypedDict(
-    "_RequiredTableResourceOutputTypeDef",
-    {
-        "DatabaseName": str,
-    },
-)
-_OptionalTableResourceOutputTypeDef = TypedDict(
-    "_OptionalTableResourceOutputTypeDef",
+TableResourceOutputTypeDef = TypedDict(
+    "TableResourceOutputTypeDef",
     {
         "CatalogId": str,
+        "DatabaseName": str,
         "Name": str,
         "TableWildcard": Dict[str, Any],
     },
-    total=False,
 )
 
-class TableResourceOutputTypeDef(
-    _RequiredTableResourceOutputTypeDef, _OptionalTableResourceOutputTypeDef
-):
-    pass
-
 StartTransactionRequestRequestTypeDef = TypedDict(
     "StartTransactionRequestRequestTypeDef",
     {
         "TransactionType": TransactionTypeType,
     },
     total=False,
 )
@@ -1069,18 +1103,17 @@
     _OptionalGetTemporaryGlueTableCredentialsRequestRequestTypeDef,
 ):
     pass
 
 PrincipalPermissionsOutputTypeDef = TypedDict(
     "PrincipalPermissionsOutputTypeDef",
     {
-        "Principal": DataLakePrincipalTypeDef,
+        "Principal": DataLakePrincipalOutputTypeDef,
         "Permissions": List[PermissionType],
     },
-    total=False,
 )
 
 PrincipalPermissionsTypeDef = TypedDict(
     "PrincipalPermissionsTypeDef",
     {
         "Principal": DataLakePrincipalTypeDef,
         "Permissions": Sequence[PermissionType],
@@ -1090,57 +1123,44 @@
 
 ColumnLFTagTypeDef = TypedDict(
     "ColumnLFTagTypeDef",
     {
         "Name": str,
         "LFTags": List[LFTagPairOutputTypeDef],
     },
-    total=False,
 )
 
 LFTagErrorTypeDef = TypedDict(
     "LFTagErrorTypeDef",
     {
         "LFTag": LFTagPairOutputTypeDef,
         "Error": ErrorDetailTypeDef,
     },
-    total=False,
 )
 
 ListLFTagsResponseTypeDef = TypedDict(
     "ListLFTagsResponseTypeDef",
     {
         "LFTags": List[LFTagPairOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredTableWithColumnsResourceOutputTypeDef = TypedDict(
-    "_RequiredTableWithColumnsResourceOutputTypeDef",
+TableWithColumnsResourceOutputTypeDef = TypedDict(
+    "TableWithColumnsResourceOutputTypeDef",
     {
+        "CatalogId": str,
         "DatabaseName": str,
         "Name": str,
-    },
-)
-_OptionalTableWithColumnsResourceOutputTypeDef = TypedDict(
-    "_OptionalTableWithColumnsResourceOutputTypeDef",
-    {
-        "CatalogId": str,
         "ColumnNames": List[str],
         "ColumnWildcard": ColumnWildcardOutputTypeDef,
     },
-    total=False,
 )
 
-class TableWithColumnsResourceOutputTypeDef(
-    _RequiredTableWithColumnsResourceOutputTypeDef, _OptionalTableWithColumnsResourceOutputTypeDef
-):
-    pass
-
 _RequiredTableWithColumnsResourceTypeDef = TypedDict(
     "_RequiredTableWithColumnsResourceTypeDef",
     {
         "DatabaseName": str,
         "Name": str,
     },
 )
@@ -1155,39 +1175,28 @@
 )
 
 class TableWithColumnsResourceTypeDef(
     _RequiredTableWithColumnsResourceTypeDef, _OptionalTableWithColumnsResourceTypeDef
 ):
     pass
 
-_RequiredDataCellsFilterOutputTypeDef = TypedDict(
-    "_RequiredDataCellsFilterOutputTypeDef",
+DataCellsFilterOutputTypeDef = TypedDict(
+    "DataCellsFilterOutputTypeDef",
     {
         "TableCatalogId": str,
         "DatabaseName": str,
         "TableName": str,
         "Name": str,
-    },
-)
-_OptionalDataCellsFilterOutputTypeDef = TypedDict(
-    "_OptionalDataCellsFilterOutputTypeDef",
-    {
         "RowFilter": RowFilterOutputTypeDef,
         "ColumnNames": List[str],
         "ColumnWildcard": ColumnWildcardOutputTypeDef,
         "VersionId": str,
     },
-    total=False,
 )
 
-class DataCellsFilterOutputTypeDef(
-    _RequiredDataCellsFilterOutputTypeDef, _OptionalDataCellsFilterOutputTypeDef
-):
-    pass
-
 _RequiredDataCellsFilterTypeDef = TypedDict(
     "_RequiredDataCellsFilterTypeDef",
     {
         "TableCatalogId": str,
         "DatabaseName": str,
         "TableName": str,
         "Name": str,
@@ -1206,18 +1215,17 @@
 
 class DataCellsFilterTypeDef(_RequiredDataCellsFilterTypeDef, _OptionalDataCellsFilterTypeDef):
     pass
 
 TaggedDatabaseTypeDef = TypedDict(
     "TaggedDatabaseTypeDef",
     {
-        "Database": DatabaseResourceTypeDef,
+        "Database": DatabaseResourceOutputTypeDef,
         "LFTags": List[LFTagPairOutputTypeDef],
     },
-    total=False,
 )
 
 WriteOperationTypeDef = TypedDict(
     "WriteOperationTypeDef",
     {
         "AddObject": AddObjectInputTypeDef,
         "DeleteObject": DeleteObjectInputTypeDef,
@@ -1298,61 +1306,14 @@
         "ExecutionStatistics": ExecutionStatisticsTypeDef,
         "PlanningStatistics": PlanningStatisticsTypeDef,
         "QuerySubmissionTime": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredGetTableObjectsRequestRequestTypeDef = TypedDict(
-    "_RequiredGetTableObjectsRequestRequestTypeDef",
-    {
-        "DatabaseName": str,
-        "TableName": str,
-    },
-)
-_OptionalGetTableObjectsRequestRequestTypeDef = TypedDict(
-    "_OptionalGetTableObjectsRequestRequestTypeDef",
-    {
-        "CatalogId": str,
-        "TransactionId": str,
-        "QueryAsOfTime": TimestampTypeDef,
-        "PartitionPredicate": str,
-        "MaxResults": int,
-        "NextToken": str,
-    },
-    total=False,
-)
-
-class GetTableObjectsRequestRequestTypeDef(
-    _RequiredGetTableObjectsRequestRequestTypeDef, _OptionalGetTableObjectsRequestRequestTypeDef
-):
-    pass
-
-_RequiredQueryPlanningContextTypeDef = TypedDict(
-    "_RequiredQueryPlanningContextTypeDef",
-    {
-        "DatabaseName": str,
-    },
-)
-_OptionalQueryPlanningContextTypeDef = TypedDict(
-    "_OptionalQueryPlanningContextTypeDef",
-    {
-        "CatalogId": str,
-        "QueryAsOfTime": TimestampTypeDef,
-        "QueryParameters": Mapping[str, str],
-        "TransactionId": str,
-    },
-    total=False,
-)
-
-class QueryPlanningContextTypeDef(
-    _RequiredQueryPlanningContextTypeDef, _OptionalQueryPlanningContextTypeDef
-):
-    pass
-
 _RequiredGetTemporaryGluePartitionCredentialsRequestRequestTypeDef = TypedDict(
     "_RequiredGetTemporaryGluePartitionCredentialsRequestRequestTypeDef",
     {
         "TableArn": str,
         "Partition": PartitionValueListTypeDef,
     },
 )
@@ -1409,56 +1370,129 @@
         "NextToken": str,
         "QueryId": str,
         "WorkUnitRanges": List[WorkUnitRangeTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredLFTagPolicyResourceOutputTypeDef = TypedDict(
-    "_RequiredLFTagPolicyResourceOutputTypeDef",
+LFTagPolicyResourceOutputTypeDef = TypedDict(
+    "LFTagPolicyResourceOutputTypeDef",
     {
+        "CatalogId": str,
         "ResourceType": ResourceTypeType,
         "Expression": List[LFTagOutputTypeDef],
     },
 )
-_OptionalLFTagPolicyResourceOutputTypeDef = TypedDict(
-    "_OptionalLFTagPolicyResourceOutputTypeDef",
+
+_RequiredLFTagPolicyResourceTypeDef = TypedDict(
+    "_RequiredLFTagPolicyResourceTypeDef",
+    {
+        "ResourceType": ResourceTypeType,
+        "Expression": Sequence[LFTagTypeDef],
+    },
+)
+_OptionalLFTagPolicyResourceTypeDef = TypedDict(
+    "_OptionalLFTagPolicyResourceTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
-class LFTagPolicyResourceOutputTypeDef(
-    _RequiredLFTagPolicyResourceOutputTypeDef, _OptionalLFTagPolicyResourceOutputTypeDef
+class LFTagPolicyResourceTypeDef(
+    _RequiredLFTagPolicyResourceTypeDef, _OptionalLFTagPolicyResourceTypeDef
 ):
     pass
 
-LFTagPairUnionTypeDef = Union[LFTagPairTypeDef, LFTagPairOutputTypeDef]
-_RequiredLFTagPolicyResourceTypeDef = TypedDict(
-    "_RequiredLFTagPolicyResourceTypeDef",
+_RequiredSearchDatabasesByLFTagsRequestRequestTypeDef = TypedDict(
+    "_RequiredSearchDatabasesByLFTagsRequestRequestTypeDef",
     {
-        "ResourceType": ResourceTypeType,
         "Expression": Sequence[LFTagTypeDef],
     },
 )
-_OptionalLFTagPolicyResourceTypeDef = TypedDict(
-    "_OptionalLFTagPolicyResourceTypeDef",
+_OptionalSearchDatabasesByLFTagsRequestRequestTypeDef = TypedDict(
+    "_OptionalSearchDatabasesByLFTagsRequestRequestTypeDef",
     {
+        "NextToken": str,
+        "MaxResults": int,
         "CatalogId": str,
     },
     total=False,
 )
 
-class LFTagPolicyResourceTypeDef(
-    _RequiredLFTagPolicyResourceTypeDef, _OptionalLFTagPolicyResourceTypeDef
+class SearchDatabasesByLFTagsRequestRequestTypeDef(
+    _RequiredSearchDatabasesByLFTagsRequestRequestTypeDef,
+    _OptionalSearchDatabasesByLFTagsRequestRequestTypeDef,
+):
+    pass
+
+_RequiredSearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef = TypedDict(
+    "_RequiredSearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef",
+    {
+        "Expression": Sequence[LFTagTypeDef],
+    },
+)
+_OptionalSearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef = TypedDict(
+    "_OptionalSearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef",
+    {
+        "CatalogId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class SearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef(
+    _RequiredSearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef,
+    _OptionalSearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef,
+):
+    pass
+
+_RequiredSearchTablesByLFTagsRequestRequestTypeDef = TypedDict(
+    "_RequiredSearchTablesByLFTagsRequestRequestTypeDef",
+    {
+        "Expression": Sequence[LFTagTypeDef],
+    },
+)
+_OptionalSearchTablesByLFTagsRequestRequestTypeDef = TypedDict(
+    "_OptionalSearchTablesByLFTagsRequestRequestTypeDef",
+    {
+        "NextToken": str,
+        "MaxResults": int,
+        "CatalogId": str,
+    },
+    total=False,
+)
+
+class SearchTablesByLFTagsRequestRequestTypeDef(
+    _RequiredSearchTablesByLFTagsRequestRequestTypeDef,
+    _OptionalSearchTablesByLFTagsRequestRequestTypeDef,
+):
+    pass
+
+_RequiredSearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef = TypedDict(
+    "_RequiredSearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef",
+    {
+        "Expression": Sequence[LFTagTypeDef],
+    },
+)
+_OptionalSearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef = TypedDict(
+    "_OptionalSearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef",
+    {
+        "CatalogId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class SearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef(
+    _RequiredSearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef,
+    _OptionalSearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef,
 ):
     pass
 
-LFTagUnionTypeDef = Union[LFTagTypeDef, LFTagOutputTypeDef]
 ListDataCellsFilterRequestListDataCellsFilterPaginateTypeDef = TypedDict(
     "ListDataCellsFilterRequestListDataCellsFilterPaginateTypeDef",
     {
         "Table": TableResourceTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -1485,33 +1519,38 @@
 
 PartitionObjectsTypeDef = TypedDict(
     "PartitionObjectsTypeDef",
     {
         "PartitionValues": List[str],
         "Objects": List[TableObjectTypeDef],
     },
-    total=False,
 )
 
-TableResourceUnionTypeDef = Union[TableResourceTypeDef, TableResourceOutputTypeDef]
+StartQueryPlanningRequestRequestTypeDef = TypedDict(
+    "StartQueryPlanningRequestRequestTypeDef",
+    {
+        "QueryPlanningContext": QueryPlanningContextTypeDef,
+        "QueryString": str,
+    },
+)
+
 DataLakeSettingsOutputTypeDef = TypedDict(
     "DataLakeSettingsOutputTypeDef",
     {
-        "DataLakeAdmins": List[DataLakePrincipalTypeDef],
-        "ReadOnlyAdmins": List[DataLakePrincipalTypeDef],
+        "DataLakeAdmins": List[DataLakePrincipalOutputTypeDef],
+        "ReadOnlyAdmins": List[DataLakePrincipalOutputTypeDef],
         "CreateDatabaseDefaultPermissions": List[PrincipalPermissionsOutputTypeDef],
         "CreateTableDefaultPermissions": List[PrincipalPermissionsOutputTypeDef],
         "Parameters": Dict[str, str],
         "TrustedResourceOwners": List[str],
         "AllowExternalDataFiltering": bool,
         "AllowFullTableExternalDataAccess": bool,
-        "ExternalDataFilteringAllowList": List[DataLakePrincipalTypeDef],
+        "ExternalDataFilteringAllowList": List[DataLakePrincipalOutputTypeDef],
         "AuthorizedSessionTagValueList": List[str],
     },
-    total=False,
 )
 
 DataLakeSettingsTypeDef = TypedDict(
     "DataLakeSettingsTypeDef",
     {
         "DataLakeAdmins": Sequence[DataLakePrincipalTypeDef],
         "ReadOnlyAdmins": Sequence[DataLakePrincipalTypeDef],
@@ -1541,15 +1580,14 @@
     "TaggedTableTypeDef",
     {
         "Table": TableResourceOutputTypeDef,
         "LFTagOnDatabase": List[LFTagPairOutputTypeDef],
         "LFTagsOnTable": List[LFTagPairOutputTypeDef],
         "LFTagsOnColumns": List[ColumnLFTagTypeDef],
     },
-    total=False,
 )
 
 AddLFTagsToResourceResponseTypeDef = TypedDict(
     "AddLFTagsToResourceResponseTypeDef",
     {
         "Failures": List[LFTagErrorTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1584,15 +1622,14 @@
 CreateDataCellsFilterRequestRequestTypeDef = TypedDict(
     "CreateDataCellsFilterRequestRequestTypeDef",
     {
         "TableData": DataCellsFilterTypeDef,
     },
 )
 
-DataCellsFilterUnionTypeDef = Union[DataCellsFilterTypeDef, DataCellsFilterOutputTypeDef]
 UpdateDataCellsFilterRequestRequestTypeDef = TypedDict(
     "UpdateDataCellsFilterRequestRequestTypeDef",
     {
         "TableData": DataCellsFilterTypeDef,
     },
 )
 
@@ -1624,35 +1661,26 @@
 
 class UpdateTableObjectsRequestRequestTypeDef(
     _RequiredUpdateTableObjectsRequestRequestTypeDef,
     _OptionalUpdateTableObjectsRequestRequestTypeDef,
 ):
     pass
 
-StartQueryPlanningRequestRequestTypeDef = TypedDict(
-    "StartQueryPlanningRequestRequestTypeDef",
-    {
-        "QueryPlanningContext": QueryPlanningContextTypeDef,
-        "QueryString": str,
-    },
-)
-
 ResourceOutputTypeDef = TypedDict(
     "ResourceOutputTypeDef",
     {
         "Catalog": Dict[str, Any],
-        "Database": DatabaseResourceTypeDef,
+        "Database": DatabaseResourceOutputTypeDef,
         "Table": TableResourceOutputTypeDef,
         "TableWithColumns": TableWithColumnsResourceOutputTypeDef,
-        "DataLocation": DataLocationResourceTypeDef,
-        "DataCellsFilter": DataCellsFilterResourceTypeDef,
+        "DataLocation": DataLocationResourceOutputTypeDef,
+        "DataCellsFilter": DataCellsFilterResourceOutputTypeDef,
         "LFTag": LFTagKeyResourceOutputTypeDef,
         "LFTagPolicy": LFTagPolicyResourceOutputTypeDef,
     },
-    total=False,
 )
 
 ResourceTypeDef = TypedDict(
     "ResourceTypeDef",
     {
         "Catalog": Mapping[str, Any],
         "Database": DatabaseResourceTypeDef,
@@ -1662,100 +1690,14 @@
         "DataCellsFilter": DataCellsFilterResourceTypeDef,
         "LFTag": LFTagKeyResourceTypeDef,
         "LFTagPolicy": LFTagPolicyResourceTypeDef,
     },
     total=False,
 )
 
-_RequiredSearchDatabasesByLFTagsRequestRequestTypeDef = TypedDict(
-    "_RequiredSearchDatabasesByLFTagsRequestRequestTypeDef",
-    {
-        "Expression": Sequence[LFTagUnionTypeDef],
-    },
-)
-_OptionalSearchDatabasesByLFTagsRequestRequestTypeDef = TypedDict(
-    "_OptionalSearchDatabasesByLFTagsRequestRequestTypeDef",
-    {
-        "NextToken": str,
-        "MaxResults": int,
-        "CatalogId": str,
-    },
-    total=False,
-)
-
-class SearchDatabasesByLFTagsRequestRequestTypeDef(
-    _RequiredSearchDatabasesByLFTagsRequestRequestTypeDef,
-    _OptionalSearchDatabasesByLFTagsRequestRequestTypeDef,
-):
-    pass
-
-_RequiredSearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef = TypedDict(
-    "_RequiredSearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef",
-    {
-        "Expression": Sequence[LFTagUnionTypeDef],
-    },
-)
-_OptionalSearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef = TypedDict(
-    "_OptionalSearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef",
-    {
-        "CatalogId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class SearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef(
-    _RequiredSearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef,
-    _OptionalSearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef,
-):
-    pass
-
-_RequiredSearchTablesByLFTagsRequestRequestTypeDef = TypedDict(
-    "_RequiredSearchTablesByLFTagsRequestRequestTypeDef",
-    {
-        "Expression": Sequence[LFTagUnionTypeDef],
-    },
-)
-_OptionalSearchTablesByLFTagsRequestRequestTypeDef = TypedDict(
-    "_OptionalSearchTablesByLFTagsRequestRequestTypeDef",
-    {
-        "NextToken": str,
-        "MaxResults": int,
-        "CatalogId": str,
-    },
-    total=False,
-)
-
-class SearchTablesByLFTagsRequestRequestTypeDef(
-    _RequiredSearchTablesByLFTagsRequestRequestTypeDef,
-    _OptionalSearchTablesByLFTagsRequestRequestTypeDef,
-):
-    pass
-
-_RequiredSearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef = TypedDict(
-    "_RequiredSearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef",
-    {
-        "Expression": Sequence[LFTagUnionTypeDef],
-    },
-)
-_OptionalSearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef = TypedDict(
-    "_OptionalSearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef",
-    {
-        "CatalogId": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class SearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef(
-    _RequiredSearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef,
-    _OptionalSearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef,
-):
-    pass
-
 GetTableObjectsResponseTypeDef = TypedDict(
     "GetTableObjectsResponseTypeDef",
     {
         "Objects": List[PartitionObjectsTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1765,15 +1707,14 @@
     "GetDataLakeSettingsResponseTypeDef",
     {
         "DataLakeSettings": DataLakeSettingsOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DataLakeSettingsUnionTypeDef = Union[DataLakeSettingsTypeDef, DataLakeSettingsOutputTypeDef]
 _RequiredPutDataLakeSettingsRequestRequestTypeDef = TypedDict(
     "_RequiredPutDataLakeSettingsRequestRequestTypeDef",
     {
         "DataLakeSettings": DataLakeSettingsTypeDef,
     },
 )
 _OptionalPutDataLakeSettingsRequestRequestTypeDef = TypedDict(
@@ -1795,54 +1736,41 @@
     {
         "NextToken": str,
         "TableList": List[TaggedTableTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredBatchPermissionsRequestEntryOutputTypeDef = TypedDict(
-    "_RequiredBatchPermissionsRequestEntryOutputTypeDef",
+BatchPermissionsRequestEntryOutputTypeDef = TypedDict(
+    "BatchPermissionsRequestEntryOutputTypeDef",
     {
         "Id": str,
-    },
-)
-_OptionalBatchPermissionsRequestEntryOutputTypeDef = TypedDict(
-    "_OptionalBatchPermissionsRequestEntryOutputTypeDef",
-    {
-        "Principal": DataLakePrincipalTypeDef,
+        "Principal": DataLakePrincipalOutputTypeDef,
         "Resource": ResourceOutputTypeDef,
         "Permissions": List[PermissionType],
         "PermissionsWithGrantOption": List[PermissionType],
     },
-    total=False,
 )
 
-class BatchPermissionsRequestEntryOutputTypeDef(
-    _RequiredBatchPermissionsRequestEntryOutputTypeDef,
-    _OptionalBatchPermissionsRequestEntryOutputTypeDef,
-):
-    pass
-
 PrincipalResourcePermissionsTypeDef = TypedDict(
     "PrincipalResourcePermissionsTypeDef",
     {
-        "Principal": DataLakePrincipalTypeDef,
+        "Principal": DataLakePrincipalOutputTypeDef,
         "Resource": ResourceOutputTypeDef,
         "Permissions": List[PermissionType],
         "PermissionsWithGrantOption": List[PermissionType],
         "AdditionalDetails": DetailsMapTypeDef,
     },
-    total=False,
 )
 
 _RequiredAddLFTagsToResourceRequestRequestTypeDef = TypedDict(
     "_RequiredAddLFTagsToResourceRequestRequestTypeDef",
     {
         "Resource": ResourceTypeDef,
-        "LFTags": Sequence[LFTagPairUnionTypeDef],
+        "LFTags": Sequence[LFTagPairTypeDef],
     },
 )
 _OptionalAddLFTagsToResourceRequestRequestTypeDef = TypedDict(
     "_OptionalAddLFTagsToResourceRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
@@ -1933,15 +1861,15 @@
     total=False,
 )
 
 _RequiredRemoveLFTagsFromResourceRequestRequestTypeDef = TypedDict(
     "_RequiredRemoveLFTagsFromResourceRequestRequestTypeDef",
     {
         "Resource": ResourceTypeDef,
-        "LFTags": Sequence[LFTagPairUnionTypeDef],
+        "LFTags": Sequence[LFTagPairTypeDef],
     },
 )
 _OptionalRemoveLFTagsFromResourceRequestRequestTypeDef = TypedDict(
     "_OptionalRemoveLFTagsFromResourceRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
@@ -1950,15 +1878,14 @@
 
 class RemoveLFTagsFromResourceRequestRequestTypeDef(
     _RequiredRemoveLFTagsFromResourceRequestRequestTypeDef,
     _OptionalRemoveLFTagsFromResourceRequestRequestTypeDef,
 ):
     pass
 
-ResourceUnionTypeDef = Union[ResourceTypeDef, ResourceOutputTypeDef]
 _RequiredRevokePermissionsRequestRequestTypeDef = TypedDict(
     "_RequiredRevokePermissionsRequestRequestTypeDef",
     {
         "Principal": DataLakePrincipalTypeDef,
         "Resource": ResourceTypeDef,
         "Permissions": Sequence[PermissionType],
     },
@@ -1979,15 +1906,14 @@
 
 BatchPermissionsFailureEntryTypeDef = TypedDict(
     "BatchPermissionsFailureEntryTypeDef",
     {
         "RequestEntry": BatchPermissionsRequestEntryOutputTypeDef,
         "Error": ErrorDetailTypeDef,
     },
-    total=False,
 )
 
 GetEffectivePermissionsForPathResponseTypeDef = TypedDict(
     "GetEffectivePermissionsForPathResponseTypeDef",
     {
         "Permissions": List[PrincipalResourcePermissionsTypeDef],
         "NextToken": str,
@@ -2000,37 +1926,18 @@
     {
         "PrincipalResourcePermissions": List[PrincipalResourcePermissionsTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BatchPermissionsRequestEntryUnionTypeDef = Union[
-    BatchPermissionsRequestEntryTypeDef, BatchPermissionsRequestEntryOutputTypeDef
-]
-BatchGrantPermissionsResponseTypeDef = TypedDict(
-    "BatchGrantPermissionsResponseTypeDef",
-    {
-        "Failures": List[BatchPermissionsFailureEntryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-BatchRevokePermissionsResponseTypeDef = TypedDict(
-    "BatchRevokePermissionsResponseTypeDef",
-    {
-        "Failures": List[BatchPermissionsFailureEntryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredBatchGrantPermissionsRequestRequestTypeDef = TypedDict(
     "_RequiredBatchGrantPermissionsRequestRequestTypeDef",
     {
-        "Entries": Sequence[BatchPermissionsRequestEntryUnionTypeDef],
+        "Entries": Sequence[BatchPermissionsRequestEntryTypeDef],
     },
 )
 _OptionalBatchGrantPermissionsRequestRequestTypeDef = TypedDict(
     "_OptionalBatchGrantPermissionsRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
@@ -2042,15 +1949,15 @@
     _OptionalBatchGrantPermissionsRequestRequestTypeDef,
 ):
     pass
 
 _RequiredBatchRevokePermissionsRequestRequestTypeDef = TypedDict(
     "_RequiredBatchRevokePermissionsRequestRequestTypeDef",
     {
-        "Entries": Sequence[BatchPermissionsRequestEntryUnionTypeDef],
+        "Entries": Sequence[BatchPermissionsRequestEntryTypeDef],
     },
 )
 _OptionalBatchRevokePermissionsRequestRequestTypeDef = TypedDict(
     "_OptionalBatchRevokePermissionsRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
@@ -2058,7 +1965,23 @@
 )
 
 class BatchRevokePermissionsRequestRequestTypeDef(
     _RequiredBatchRevokePermissionsRequestRequestTypeDef,
     _OptionalBatchRevokePermissionsRequestRequestTypeDef,
 ):
     pass
+
+BatchGrantPermissionsResponseTypeDef = TypedDict(
+    "BatchGrantPermissionsResponseTypeDef",
+    {
+        "Failures": List[BatchPermissionsFailureEntryTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+BatchRevokePermissionsResponseTypeDef = TypedDict(
+    "BatchRevokePermissionsResponseTypeDef",
+    {
+        "Failures": List[BatchPermissionsFailureEntryTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
```

### Comparing `mypy-boto3-lakeformation-1.28.16/mypy_boto3_lakeformation.egg-info/PKG-INFO` & `mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-lakeformation
-Version: 1.28.16
-Summary: Type annotations for boto3.LakeFormation 1.28.16 service generated with mypy-boto3-builder 7.17.1
+Version: 1.28.4
+Summary: Type annotations for boto3.LakeFormation 1.28.4 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 lakeformation type-annotations botocore mypy typeshed autocomplete
+Keywords: boto3 lakeformation type-annotations boto3-stubs mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-lakeformation"></a>
 
 # mypy-boto3-lakeformation
 
 [![PyPI - mypy-boto3-lakeformation](https://img.shields.io/pypi/v/mypy-boto3-lakeformation.svg?color=blue)](https://pypi.org/project/mypy-boto3-lakeformation)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lakeformation.svg?color=blue)](https://pypi.org/project/mypy-boto3-lakeformation)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-lakeformation)](https://pepy.tech/project/mypy-boto3-lakeformation)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-lakeformation?color=blue)](https://pypistats.org/packages/mypy-boto3-lakeformation)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LakeFormation 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation)
+[boto3.LakeFormation 1.28.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.17.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-lakeformation docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/).
 
 See how it helps to find and fix potential bugs:
 
@@ -74,15 +74,15 @@
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Literals](#literals)
-    - [Type definitions](#type-definitions)
+    - [Typed dictionaries](#typed-dictionaries)
   - [How it works](#how-it-works)
   - [What's new](#what's-new)
     - [Implemented features](#implemented-features)
     - [Latest changes](#latest-changes)
   - [Versioning](#versioning)
   - [Thank you](#thank-you)
   - [Documentation](#documentation)
@@ -342,39 +342,44 @@
 )
 
 
 def check_value(value: ComparisonOperatorType) -> bool:
     ...
 ```
 
-<a id="type-definitions"></a>
+<a id="typed-dictionaries"></a>
 
-### Type definitions
+### Typed dictionaries
 
 `mypy_boto3_lakeformation.type_defs` module contains structures and shapes
-assembled to typed dictionaries and unions for additional type checking.
+assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_lakeformation.type_defs import (
+    LFTagPairTypeDef,
     ResponseMetadataTypeDef,
     AddObjectInputTypeDef,
     AssumeDecoratedRoleWithSAMLRequestRequestTypeDef,
     AuditContextTypeDef,
     ErrorDetailTypeDef,
+    DataLakePrincipalOutputTypeDef,
     DataLakePrincipalTypeDef,
     CancelTransactionRequestRequestTypeDef,
     LFTagPairOutputTypeDef,
     ColumnWildcardOutputTypeDef,
     ColumnWildcardTypeDef,
     CommitTransactionRequestRequestTypeDef,
     CreateLFTagRequestRequestTypeDef,
     RowFilterOutputTypeDef,
+    DataCellsFilterResourceOutputTypeDef,
     DataCellsFilterResourceTypeDef,
     RowFilterTypeDef,
+    DataLocationResourceOutputTypeDef,
     DataLocationResourceTypeDef,
+    DatabaseResourceOutputTypeDef,
     DatabaseResourceTypeDef,
     DeleteDataCellsFilterRequestRequestTypeDef,
     DeleteLFTagRequestRequestTypeDef,
     DeleteObjectInputTypeDef,
     VirtualObjectTypeDef,
     DeregisterResourceRequestRequestTypeDef,
     DescribeResourceRequestRequestTypeDef,
@@ -388,31 +393,31 @@
     GetDataCellsFilterRequestRequestTypeDef,
     GetDataLakeSettingsRequestRequestTypeDef,
     GetEffectivePermissionsForPathRequestRequestTypeDef,
     GetLFTagRequestRequestTypeDef,
     GetQueryStateRequestRequestTypeDef,
     GetQueryStatisticsRequestRequestTypeDef,
     PlanningStatisticsTypeDef,
-    TimestampTypeDef,
+    GetTableObjectsRequestRequestTypeDef,
     PartitionValueListTypeDef,
     GetWorkUnitResultsRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     GetWorkUnitsRequestRequestTypeDef,
     WorkUnitRangeTypeDef,
     LFTagKeyResourceOutputTypeDef,
     LFTagKeyResourceTypeDef,
     LFTagOutputTypeDef,
-    LFTagPairTypeDef,
     LFTagTypeDef,
     TableResourceTypeDef,
     ListLFTagsRequestRequestTypeDef,
     ListTableStorageOptimizersRequestRequestTypeDef,
     StorageOptimizerTypeDef,
     ListTransactionsRequestRequestTypeDef,
     TableObjectTypeDef,
+    QueryPlanningContextTypeDef,
     RegisterResourceRequestRequestTypeDef,
     TableResourceOutputTypeDef,
     StartTransactionRequestRequestTypeDef,
     UpdateLFTagRequestRequestTypeDef,
     UpdateResourceRequestRequestTypeDef,
     UpdateTableStorageOptimizerRequestRequestTypeDef,
     AssumeDecoratedRoleWithSAMLResponseTypeDef,
@@ -440,76 +445,67 @@
     DeleteObjectsOnCancelRequestRequestTypeDef,
     DescribeResourceResponseTypeDef,
     ListResourcesResponseTypeDef,
     DescribeTransactionResponseTypeDef,
     ListTransactionsResponseTypeDef,
     ListResourcesRequestRequestTypeDef,
     GetQueryStatisticsResponseTypeDef,
-    GetTableObjectsRequestRequestTypeDef,
-    QueryPlanningContextTypeDef,
     GetTemporaryGluePartitionCredentialsRequestRequestTypeDef,
     GetWorkUnitsRequestGetWorkUnitsPaginateTypeDef,
     ListLFTagsRequestListLFTagsPaginateTypeDef,
     GetWorkUnitsResponseTypeDef,
     LFTagPolicyResourceOutputTypeDef,
-    LFTagPairUnionTypeDef,
     LFTagPolicyResourceTypeDef,
-    LFTagUnionTypeDef,
+    SearchDatabasesByLFTagsRequestRequestTypeDef,
+    SearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef,
+    SearchTablesByLFTagsRequestRequestTypeDef,
+    SearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef,
     ListDataCellsFilterRequestListDataCellsFilterPaginateTypeDef,
     ListDataCellsFilterRequestRequestTypeDef,
     ListTableStorageOptimizersResponseTypeDef,
     PartitionObjectsTypeDef,
-    TableResourceUnionTypeDef,
+    StartQueryPlanningRequestRequestTypeDef,
     DataLakeSettingsOutputTypeDef,
     DataLakeSettingsTypeDef,
     GetResourceLFTagsResponseTypeDef,
     TaggedTableTypeDef,
     AddLFTagsToResourceResponseTypeDef,
     RemoveLFTagsFromResourceResponseTypeDef,
     GetDataCellsFilterResponseTypeDef,
     ListDataCellsFilterResponseTypeDef,
     CreateDataCellsFilterRequestRequestTypeDef,
-    DataCellsFilterUnionTypeDef,
     UpdateDataCellsFilterRequestRequestTypeDef,
     SearchDatabasesByLFTagsResponseTypeDef,
     UpdateTableObjectsRequestRequestTypeDef,
-    StartQueryPlanningRequestRequestTypeDef,
     ResourceOutputTypeDef,
     ResourceTypeDef,
-    SearchDatabasesByLFTagsRequestRequestTypeDef,
-    SearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef,
-    SearchTablesByLFTagsRequestRequestTypeDef,
-    SearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef,
     GetTableObjectsResponseTypeDef,
     GetDataLakeSettingsResponseTypeDef,
-    DataLakeSettingsUnionTypeDef,
     PutDataLakeSettingsRequestRequestTypeDef,
     SearchTablesByLFTagsResponseTypeDef,
     BatchPermissionsRequestEntryOutputTypeDef,
     PrincipalResourcePermissionsTypeDef,
     AddLFTagsToResourceRequestRequestTypeDef,
     BatchPermissionsRequestEntryTypeDef,
     GetResourceLFTagsRequestRequestTypeDef,
     GrantPermissionsRequestRequestTypeDef,
     ListPermissionsRequestRequestTypeDef,
     RemoveLFTagsFromResourceRequestRequestTypeDef,
-    ResourceUnionTypeDef,
     RevokePermissionsRequestRequestTypeDef,
     BatchPermissionsFailureEntryTypeDef,
     GetEffectivePermissionsForPathResponseTypeDef,
     ListPermissionsResponseTypeDef,
-    BatchPermissionsRequestEntryUnionTypeDef,
-    BatchGrantPermissionsResponseTypeDef,
-    BatchRevokePermissionsResponseTypeDef,
     BatchGrantPermissionsRequestRequestTypeDef,
     BatchRevokePermissionsRequestRequestTypeDef,
+    BatchGrantPermissionsResponseTypeDef,
+    BatchRevokePermissionsResponseTypeDef,
 )
 
 
-def get_value() -> ResponseMetadataTypeDef:
+def get_structure() -> LFTagPairTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-lakeformation-1.28.16/mypy_boto3_lakeformation.egg-info/SOURCES.txt` & `mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lakeformation-1.28.16/setup.py` & `mypy-boto3-lakeformation-1.28.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-lakeformation",
-    version="1.28.16",
+    version="1.28.4",
     packages=["mypy_boto3_lakeformation"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.LakeFormation 1.28.16 service generated with mypy-boto3-builder"
-        " 7.17.1"
+        "Type annotations for boto3.LakeFormation 1.28.4 service generated with mypy-boto3-builder"
+        " 7.15.1"
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
-    keywords="boto3 lakeformation type-annotations botocore mypy typeshed autocomplete",
+    keywords="boto3 lakeformation type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_lakeformation": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

