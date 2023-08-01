# Comparing `tmp/mypy-boto3-m2-1.28.16.tar.gz` & `tmp/mypy-boto3-m2-1.28.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-m2-1.28.16.tar", last modified: Tue Aug  1 11:37:15 2023, max compression
+gzip compressed data, was "mypy-boto3-m2-1.28.5.tar", last modified: Tue Jul 18 19:32:41 2023, max compression
```

## Comparing `mypy-boto3-m2-1.28.16.tar` & `mypy-boto3-m2-1.28.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:14.980834 mypy-boto3-m2-1.28.16/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:23:07.000000 mypy-boto3-m2-1.28.16/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18526 2023-08-01 11:37:14.980834 mypy-boto3-m2-1.28.16/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17042 2023-08-01 11:23:07.000000 mypy-boto3-m2-1.28.16/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:14.980834 mypy-boto3-m2-1.28.16/mypy_boto3_m2/
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-08-01 11:23:07.000000 mypy-boto3-m2-1.28.16/mypy_boto3_m2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-08-01 11:23:07.000000 mypy-boto3-m2-1.28.16/mypy_boto3_m2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-08-01 11:23:07.000000 mypy-boto3-m2-1.28.16/mypy_boto3_m2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27887 2023-08-01 11:23:08.000000 mypy-boto3-m2-1.28.16/mypy_boto3_m2/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    27838 2023-08-01 11:23:08.000000 mypy-boto3-m2-1.28.16/mypy_boto3_m2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10435 2023-08-01 11:23:10.000000 mypy-boto3-m2-1.28.16/mypy_boto3_m2/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10433 2023-08-01 11:23:10.000000 mypy-boto3-m2-1.28.16/mypy_boto3_m2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-08-01 11:23:10.000000 mypy-boto3-m2-1.28.16/mypy_boto3_m2/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11330 2023-08-01 11:23:10.000000 mypy-boto3-m2-1.28.16/mypy_boto3_m2/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:23:07.000000 mypy-boto3-m2-1.28.16/mypy_boto3_m2/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    42542 2023-08-01 11:23:12.000000 mypy-boto3-m2-1.28.16/mypy_boto3_m2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    42474 2023-08-01 11:23:11.000000 mypy-boto3-m2-1.28.16/mypy_boto3_m2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:23:07.000000 mypy-boto3-m2-1.28.16/mypy_boto3_m2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:14.980834 mypy-boto3-m2-1.28.16/mypy_boto3_m2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18526 2023-08-01 11:37:14.000000 mypy-boto3-m2-1.28.16/mypy_boto3_m2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-08-01 11:37:14.000000 mypy-boto3-m2-1.28.16/mypy_boto3_m2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:14.000000 mypy-boto3-m2-1.28.16/mypy_boto3_m2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:14.000000 mypy-boto3-m2-1.28.16/mypy_boto3_m2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:14.000000 mypy-boto3-m2-1.28.16/mypy_boto3_m2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-01 11:37:14.000000 mypy-boto3-m2-1.28.16/mypy_boto3_m2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:14.984834 mypy-boto3-m2-1.28.16/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-08-01 11:23:07.000000 mypy-boto3-m2-1.28.16/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:32:41.746719 mypy-boto3-m2-1.28.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-18 19:32:25.000000 mypy-boto3-m2-1.28.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18872 2023-07-18 19:32:41.746719 mypy-boto3-m2-1.28.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17387 2023-07-18 19:32:25.000000 mypy-boto3-m2-1.28.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:32:41.746719 mypy-boto3-m2-1.28.5/mypy_boto3_m2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-07-18 19:32:25.000000 mypy-boto3-m2-1.28.5/mypy_boto3_m2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-07-18 19:32:25.000000 mypy-boto3-m2-1.28.5/mypy_boto3_m2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-18 19:32:25.000000 mypy-boto3-m2-1.28.5/mypy_boto3_m2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27910 2023-07-18 19:32:25.000000 mypy-boto3-m2-1.28.5/mypy_boto3_m2/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27861 2023-07-18 19:32:25.000000 mypy-boto3-m2-1.28.5/mypy_boto3_m2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10357 2023-07-18 19:32:26.000000 mypy-boto3-m2-1.28.5/mypy_boto3_m2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10355 2023-07-18 19:32:26.000000 mypy-boto3-m2-1.28.5/mypy_boto3_m2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11382 2023-07-18 19:32:26.000000 mypy-boto3-m2-1.28.5/mypy_boto3_m2/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11371 2023-07-18 19:32:25.000000 mypy-boto3-m2-1.28.5/mypy_boto3_m2/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 19:32:25.000000 mypy-boto3-m2-1.28.5/mypy_boto3_m2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    42524 2023-07-18 19:32:27.000000 mypy-boto3-m2-1.28.5/mypy_boto3_m2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42470 2023-07-18 19:32:26.000000 mypy-boto3-m2-1.28.5/mypy_boto3_m2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-18 19:32:25.000000 mypy-boto3-m2-1.28.5/mypy_boto3_m2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:32:41.746719 mypy-boto3-m2-1.28.5/mypy_boto3_m2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18872 2023-07-18 19:32:41.000000 mypy-boto3-m2-1.28.5/mypy_boto3_m2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-18 19:32:41.000000 mypy-boto3-m2-1.28.5/mypy_boto3_m2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 19:32:41.000000 mypy-boto3-m2-1.28.5/mypy_boto3_m2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 19:32:41.000000 mypy-boto3-m2-1.28.5/mypy_boto3_m2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-18 19:32:41.000000 mypy-boto3-m2-1.28.5/mypy_boto3_m2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-18 19:32:41.000000 mypy-boto3-m2-1.28.5/mypy_boto3_m2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 19:32:41.746719 mypy-boto3-m2-1.28.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-07-18 19:32:24.000000 mypy-boto3-m2-1.28.5/setup.py
```

### Comparing `mypy-boto3-m2-1.28.16/LICENSE` & `mypy-boto3-m2-1.28.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-m2-1.28.16/PKG-INFO` & `mypy-boto3-m2-1.28.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-m2
-Version: 1.28.16
-Summary: Type annotations for boto3.MainframeModernization 1.28.16 service generated with mypy-boto3-builder 7.17.1
+Version: 1.28.5
+Summary: Type annotations for boto3.MainframeModernization 1.28.5 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 m2 type-annotations botocore mypy typeshed autocomplete
+Keywords: boto3 m2 type-annotations boto3-stubs mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-m2"></a>
 
 # mypy-boto3-m2
 
 [![PyPI - mypy-boto3-m2](https://img.shields.io/pypi/v/mypy-boto3-m2.svg?color=blue)](https://pypi.org/project/mypy-boto3-m2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-m2.svg?color=blue)](https://pypi.org/project/mypy-boto3-m2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-m2)](https://pepy.tech/project/mypy-boto3-m2)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-m2?color=blue)](https://pypistats.org/packages/mypy-boto3-m2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MainframeModernization 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization)
+[boto3.MainframeModernization 1.28.5](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization)
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
 [mypy-boto3-m2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/).
 
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
@@ -353,35 +353,41 @@
 )
 
 
 def check_value(value: ApplicationDeploymentLifecycleType) -> bool:
     ...
 ```
 
-<a id="type-definitions"></a>
+<a id="typed-dictionaries"></a>
 
-### Type definitions
+### Typed dictionaries
 
 `mypy_boto3_m2.type_defs` module contains structures and shapes assembled to
-typed dictionaries and unions for additional type checking.
+typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_m2.type_defs import (
+    AlternateKeyOutputTypeDef,
     AlternateKeyTypeDef,
     ApplicationSummaryTypeDef,
     ApplicationVersionSummaryTypeDef,
     FileBatchJobDefinitionTypeDef,
     ScriptBatchJobDefinitionTypeDef,
+    FileBatchJobIdentifierOutputTypeDef,
+    ScriptBatchJobIdentifierOutputTypeDef,
     FileBatchJobIdentifierTypeDef,
     ScriptBatchJobIdentifierTypeDef,
     CancelBatchJobExecutionRequestRequestTypeDef,
     DefinitionTypeDef,
-    ResponseMetadataTypeDef,
+    CreateApplicationResponseTypeDef,
+    CreateDataSetImportTaskResponseTypeDef,
     CreateDeploymentRequestRequestTypeDef,
+    CreateDeploymentResponseTypeDef,
     HighAvailabilityConfigTypeDef,
+    CreateEnvironmentResponseTypeDef,
     ExternalLocationTypeDef,
     DataSetImportSummaryTypeDef,
     DataSetSummaryTypeDef,
     RecordLengthTypeDef,
     GdgDetailAttributesTypeDef,
     PoDetailAttributesTypeDef,
     PsDetailAttributesTypeDef,
@@ -389,101 +395,103 @@
     PoAttributesTypeDef,
     PsAttributesTypeDef,
     DeleteApplicationFromEnvironmentRequestRequestTypeDef,
     DeleteApplicationRequestRequestTypeDef,
     DeleteEnvironmentRequestRequestTypeDef,
     DeployedVersionSummaryTypeDef,
     DeploymentSummaryTypeDef,
+    EfsStorageConfigurationOutputTypeDef,
     EfsStorageConfigurationTypeDef,
     EngineVersionsSummaryTypeDef,
     EnvironmentSummaryTypeDef,
+    FsxStorageConfigurationOutputTypeDef,
     FsxStorageConfigurationTypeDef,
     GetApplicationRequestRequestTypeDef,
     LogGroupSummaryTypeDef,
     GetApplicationVersionRequestRequestTypeDef,
+    GetApplicationVersionResponseTypeDef,
     GetBatchJobExecutionRequestRequestTypeDef,
     GetDataSetDetailsRequestRequestTypeDef,
     GetDataSetImportTaskRequestRequestTypeDef,
     GetDeploymentRequestRequestTypeDef,
+    GetDeploymentResponseTypeDef,
     GetEnvironmentRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    HighAvailabilityConfigOutputTypeDef,
+    GetSignedBluinsightsUrlResponseTypeDef,
+    ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef,
     ListApplicationVersionsRequestRequestTypeDef,
+    ListApplicationsRequestListApplicationsPaginateTypeDef,
     ListApplicationsRequestRequestTypeDef,
+    ListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef,
     ListBatchJobDefinitionsRequestRequestTypeDef,
-    TimestampTypeDef,
+    ListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef,
+    ListBatchJobExecutionsRequestRequestTypeDef,
+    ListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef,
     ListDataSetImportHistoryRequestRequestTypeDef,
+    ListDataSetsRequestListDataSetsPaginateTypeDef,
     ListDataSetsRequestRequestTypeDef,
+    ListDeploymentsRequestListDeploymentsPaginateTypeDef,
     ListDeploymentsRequestRequestTypeDef,
+    ListEngineVersionsRequestListEngineVersionsPaginateTypeDef,
     ListEngineVersionsRequestRequestTypeDef,
+    ListEnvironmentsRequestListEnvironmentsPaginateTypeDef,
     ListEnvironmentsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     MaintenanceScheduleTypeDef,
+    PaginatorConfigTypeDef,
+    PrimaryKeyOutputTypeDef,
     PrimaryKeyTypeDef,
+    ResponseMetadataTypeDef,
     StartApplicationRequestRequestTypeDef,
+    StartBatchJobResponseTypeDef,
     StopApplicationRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    UpdateApplicationResponseTypeDef,
     UpdateEnvironmentRequestRequestTypeDef,
+    UpdateEnvironmentResponseTypeDef,
+    ListApplicationsResponseTypeDef,
+    ListApplicationVersionsResponseTypeDef,
     BatchJobDefinitionTypeDef,
+    BatchJobIdentifierOutputTypeDef,
     BatchJobIdentifierTypeDef,
     CreateApplicationRequestRequestTypeDef,
     UpdateApplicationRequestRequestTypeDef,
-    CreateApplicationResponseTypeDef,
-    CreateDataSetImportTaskResponseTypeDef,
-    CreateDeploymentResponseTypeDef,
-    CreateEnvironmentResponseTypeDef,
-    GetApplicationVersionResponseTypeDef,
-    GetDeploymentResponseTypeDef,
-    GetSignedBluinsightsUrlResponseTypeDef,
-    ListApplicationVersionsResponseTypeDef,
-    ListApplicationsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    StartBatchJobResponseTypeDef,
-    UpdateApplicationResponseTypeDef,
-    UpdateEnvironmentResponseTypeDef,
     DataSetImportTaskTypeDef,
     GetDataSetImportTaskResponseTypeDef,
     ListDataSetsResponseTypeDef,
     ListDeploymentsResponseTypeDef,
     ListEngineVersionsResponseTypeDef,
     ListEnvironmentsResponseTypeDef,
+    StorageConfigurationOutputTypeDef,
     StorageConfigurationTypeDef,
     GetApplicationResponseTypeDef,
-    ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef,
-    ListApplicationsRequestListApplicationsPaginateTypeDef,
-    ListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef,
-    ListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef,
-    ListDataSetsRequestListDataSetsPaginateTypeDef,
-    ListDeploymentsRequestListDeploymentsPaginateTypeDef,
-    ListEngineVersionsRequestListEngineVersionsPaginateTypeDef,
-    ListEnvironmentsRequestListEnvironmentsPaginateTypeDef,
-    ListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef,
-    ListBatchJobExecutionsRequestRequestTypeDef,
     PendingMaintenanceTypeDef,
-    VsamAttributesTypeDef,
     VsamDetailAttributesTypeDef,
+    VsamAttributesTypeDef,
     ListBatchJobDefinitionsResponseTypeDef,
     BatchJobExecutionSummaryTypeDef,
     GetBatchJobExecutionResponseTypeDef,
     StartBatchJobRequestRequestTypeDef,
     ListDataSetImportHistoryResponseTypeDef,
     CreateEnvironmentRequestRequestTypeDef,
     GetEnvironmentResponseTypeDef,
-    DatasetOrgAttributesTypeDef,
     DatasetDetailOrgAttributesTypeDef,
+    DatasetOrgAttributesTypeDef,
     ListBatchJobExecutionsResponseTypeDef,
-    DataSetTypeDef,
     GetDataSetDetailsResponseTypeDef,
+    DataSetTypeDef,
     DataSetImportItemTypeDef,
     DataSetImportConfigTypeDef,
     CreateDataSetImportTaskRequestRequestTypeDef,
 )
 
 
-def get_value() -> AlternateKeyTypeDef:
+def get_structure() -> AlternateKeyOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-m2-1.28.16/README.md` & `mypy-boto3-m2-1.28.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-m2"></a>
 
 # mypy-boto3-m2
 
 [![PyPI - mypy-boto3-m2](https://img.shields.io/pypi/v/mypy-boto3-m2.svg?color=blue)](https://pypi.org/project/mypy-boto3-m2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-m2.svg?color=blue)](https://pypi.org/project/mypy-boto3-m2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-m2)](https://pepy.tech/project/mypy-boto3-m2)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-m2?color=blue)](https://pypistats.org/packages/mypy-boto3-m2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MainframeModernization 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization)
+[boto3.MainframeModernization 1.28.5](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization)
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
 [mypy-boto3-m2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/).
 
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
@@ -321,35 +321,41 @@
 )
 
 
 def check_value(value: ApplicationDeploymentLifecycleType) -> bool:
     ...
 ```
 
-<a id="type-definitions"></a>
+<a id="typed-dictionaries"></a>
 
-### Type definitions
+### Typed dictionaries
 
 `mypy_boto3_m2.type_defs` module contains structures and shapes assembled to
-typed dictionaries and unions for additional type checking.
+typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_m2.type_defs import (
+    AlternateKeyOutputTypeDef,
     AlternateKeyTypeDef,
     ApplicationSummaryTypeDef,
     ApplicationVersionSummaryTypeDef,
     FileBatchJobDefinitionTypeDef,
     ScriptBatchJobDefinitionTypeDef,
+    FileBatchJobIdentifierOutputTypeDef,
+    ScriptBatchJobIdentifierOutputTypeDef,
     FileBatchJobIdentifierTypeDef,
     ScriptBatchJobIdentifierTypeDef,
     CancelBatchJobExecutionRequestRequestTypeDef,
     DefinitionTypeDef,
-    ResponseMetadataTypeDef,
+    CreateApplicationResponseTypeDef,
+    CreateDataSetImportTaskResponseTypeDef,
     CreateDeploymentRequestRequestTypeDef,
+    CreateDeploymentResponseTypeDef,
     HighAvailabilityConfigTypeDef,
+    CreateEnvironmentResponseTypeDef,
     ExternalLocationTypeDef,
     DataSetImportSummaryTypeDef,
     DataSetSummaryTypeDef,
     RecordLengthTypeDef,
     GdgDetailAttributesTypeDef,
     PoDetailAttributesTypeDef,
     PsDetailAttributesTypeDef,
@@ -357,101 +363,103 @@
     PoAttributesTypeDef,
     PsAttributesTypeDef,
     DeleteApplicationFromEnvironmentRequestRequestTypeDef,
     DeleteApplicationRequestRequestTypeDef,
     DeleteEnvironmentRequestRequestTypeDef,
     DeployedVersionSummaryTypeDef,
     DeploymentSummaryTypeDef,
+    EfsStorageConfigurationOutputTypeDef,
     EfsStorageConfigurationTypeDef,
     EngineVersionsSummaryTypeDef,
     EnvironmentSummaryTypeDef,
+    FsxStorageConfigurationOutputTypeDef,
     FsxStorageConfigurationTypeDef,
     GetApplicationRequestRequestTypeDef,
     LogGroupSummaryTypeDef,
     GetApplicationVersionRequestRequestTypeDef,
+    GetApplicationVersionResponseTypeDef,
     GetBatchJobExecutionRequestRequestTypeDef,
     GetDataSetDetailsRequestRequestTypeDef,
     GetDataSetImportTaskRequestRequestTypeDef,
     GetDeploymentRequestRequestTypeDef,
+    GetDeploymentResponseTypeDef,
     GetEnvironmentRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    HighAvailabilityConfigOutputTypeDef,
+    GetSignedBluinsightsUrlResponseTypeDef,
+    ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef,
     ListApplicationVersionsRequestRequestTypeDef,
+    ListApplicationsRequestListApplicationsPaginateTypeDef,
     ListApplicationsRequestRequestTypeDef,
+    ListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef,
     ListBatchJobDefinitionsRequestRequestTypeDef,
-    TimestampTypeDef,
+    ListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef,
+    ListBatchJobExecutionsRequestRequestTypeDef,
+    ListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef,
     ListDataSetImportHistoryRequestRequestTypeDef,
+    ListDataSetsRequestListDataSetsPaginateTypeDef,
     ListDataSetsRequestRequestTypeDef,
+    ListDeploymentsRequestListDeploymentsPaginateTypeDef,
     ListDeploymentsRequestRequestTypeDef,
+    ListEngineVersionsRequestListEngineVersionsPaginateTypeDef,
     ListEngineVersionsRequestRequestTypeDef,
+    ListEnvironmentsRequestListEnvironmentsPaginateTypeDef,
     ListEnvironmentsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     MaintenanceScheduleTypeDef,
+    PaginatorConfigTypeDef,
+    PrimaryKeyOutputTypeDef,
     PrimaryKeyTypeDef,
+    ResponseMetadataTypeDef,
     StartApplicationRequestRequestTypeDef,
+    StartBatchJobResponseTypeDef,
     StopApplicationRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    UpdateApplicationResponseTypeDef,
     UpdateEnvironmentRequestRequestTypeDef,
+    UpdateEnvironmentResponseTypeDef,
+    ListApplicationsResponseTypeDef,
+    ListApplicationVersionsResponseTypeDef,
     BatchJobDefinitionTypeDef,
+    BatchJobIdentifierOutputTypeDef,
     BatchJobIdentifierTypeDef,
     CreateApplicationRequestRequestTypeDef,
     UpdateApplicationRequestRequestTypeDef,
-    CreateApplicationResponseTypeDef,
-    CreateDataSetImportTaskResponseTypeDef,
-    CreateDeploymentResponseTypeDef,
-    CreateEnvironmentResponseTypeDef,
-    GetApplicationVersionResponseTypeDef,
-    GetDeploymentResponseTypeDef,
-    GetSignedBluinsightsUrlResponseTypeDef,
-    ListApplicationVersionsResponseTypeDef,
-    ListApplicationsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    StartBatchJobResponseTypeDef,
-    UpdateApplicationResponseTypeDef,
-    UpdateEnvironmentResponseTypeDef,
     DataSetImportTaskTypeDef,
     GetDataSetImportTaskResponseTypeDef,
     ListDataSetsResponseTypeDef,
     ListDeploymentsResponseTypeDef,
     ListEngineVersionsResponseTypeDef,
     ListEnvironmentsResponseTypeDef,
+    StorageConfigurationOutputTypeDef,
     StorageConfigurationTypeDef,
     GetApplicationResponseTypeDef,
-    ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef,
-    ListApplicationsRequestListApplicationsPaginateTypeDef,
-    ListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef,
-    ListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef,
-    ListDataSetsRequestListDataSetsPaginateTypeDef,
-    ListDeploymentsRequestListDeploymentsPaginateTypeDef,
-    ListEngineVersionsRequestListEngineVersionsPaginateTypeDef,
-    ListEnvironmentsRequestListEnvironmentsPaginateTypeDef,
-    ListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef,
-    ListBatchJobExecutionsRequestRequestTypeDef,
     PendingMaintenanceTypeDef,
-    VsamAttributesTypeDef,
     VsamDetailAttributesTypeDef,
+    VsamAttributesTypeDef,
     ListBatchJobDefinitionsResponseTypeDef,
     BatchJobExecutionSummaryTypeDef,
     GetBatchJobExecutionResponseTypeDef,
     StartBatchJobRequestRequestTypeDef,
     ListDataSetImportHistoryResponseTypeDef,
     CreateEnvironmentRequestRequestTypeDef,
     GetEnvironmentResponseTypeDef,
-    DatasetOrgAttributesTypeDef,
     DatasetDetailOrgAttributesTypeDef,
+    DatasetOrgAttributesTypeDef,
     ListBatchJobExecutionsResponseTypeDef,
-    DataSetTypeDef,
     GetDataSetDetailsResponseTypeDef,
+    DataSetTypeDef,
     DataSetImportItemTypeDef,
     DataSetImportConfigTypeDef,
     CreateDataSetImportTaskRequestRequestTypeDef,
 )
 
 
-def get_value() -> AlternateKeyTypeDef:
+def get_structure() -> AlternateKeyOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-m2-1.28.16/mypy_boto3_m2/__init__.py` & `mypy-boto3-m2-1.28.5/mypy_boto3_m2/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-m2-1.28.16/mypy_boto3_m2/__init__.pyi` & `mypy-boto3-m2-1.28.5/mypy_boto3_m2/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-m2-1.28.16/mypy_boto3_m2/__main__.py` & `mypy-boto3-m2-1.28.5/mypy_boto3_m2/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.MainframeModernization 1.28.16\nVersion:        "
-        " 1.28.16\nBuilder version: 7.17.1\nDocs:           "
+        "Type annotations for boto3.MainframeModernization 1.28.5\nVersion:         1.28.5\nBuilder"
+        " version: 7.15.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.16")
+    print("1.28.5")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-m2-1.28.16/mypy_boto3_m2/client.py` & `mypy-boto3-m2-1.28.5/mypy_boto3_m2/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,16 @@
     from mypy_boto3_m2.client import MainframeModernizationClient
 
     session = Session()
     client: MainframeModernizationClient = session.client("m2")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from datetime import datetime
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import BatchJobExecutionStatusType, EngineTypeType
 from .paginator import (
     ListApplicationsPaginator,
     ListApplicationVersionsPaginator,
@@ -55,15 +56,14 @@
     ListDataSetsResponseTypeDef,
     ListDeploymentsResponseTypeDef,
     ListEngineVersionsResponseTypeDef,
     ListEnvironmentsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     StartBatchJobResponseTypeDef,
     StorageConfigurationTypeDef,
-    TimestampTypeDef,
     UpdateApplicationResponseTypeDef,
     UpdateEnvironmentResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -363,16 +363,16 @@
         self,
         *,
         applicationId: str,
         executionIds: Sequence[str] = ...,
         jobName: str = ...,
         maxResults: int = ...,
         nextToken: str = ...,
-        startedAfter: TimestampTypeDef = ...,
-        startedBefore: TimestampTypeDef = ...,
+        startedAfter: Union[datetime, str] = ...,
+        startedBefore: Union[datetime, str] = ...,
         status: BatchJobExecutionStatusType = ...
     ) -> ListBatchJobExecutionsResponseTypeDef:
         """
         Lists historical, current, and scheduled batch job executions for a specific
         application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.list_batch_job_executions)
```

### Comparing `mypy-boto3-m2-1.28.16/mypy_boto3_m2/client.pyi` & `mypy-boto3-m2-1.28.5/mypy_boto3_m2/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,16 @@
     from mypy_boto3_m2.client import MainframeModernizationClient
 
     session = Session()
     client: MainframeModernizationClient = session.client("m2")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from datetime import datetime
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import BatchJobExecutionStatusType, EngineTypeType
 from .paginator import (
     ListApplicationsPaginator,
     ListApplicationVersionsPaginator,
@@ -55,15 +56,14 @@
     ListDataSetsResponseTypeDef,
     ListDeploymentsResponseTypeDef,
     ListEngineVersionsResponseTypeDef,
     ListEnvironmentsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     StartBatchJobResponseTypeDef,
     StorageConfigurationTypeDef,
-    TimestampTypeDef,
     UpdateApplicationResponseTypeDef,
     UpdateEnvironmentResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -336,16 +336,16 @@
         self,
         *,
         applicationId: str,
         executionIds: Sequence[str] = ...,
         jobName: str = ...,
         maxResults: int = ...,
         nextToken: str = ...,
-        startedAfter: TimestampTypeDef = ...,
-        startedBefore: TimestampTypeDef = ...,
+        startedAfter: Union[datetime, str] = ...,
+        startedBefore: Union[datetime, str] = ...,
         status: BatchJobExecutionStatusType = ...
     ) -> ListBatchJobExecutionsResponseTypeDef:
         """
         Lists historical, current, and scheduled batch job executions for a specific
         application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.list_batch_job_executions)
```

### Comparing `mypy-boto3-m2-1.28.16/mypy_boto3_m2/literals.py` & `mypy-boto3-m2-1.28.5/mypy_boto3_m2/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -202,15 +202,14 @@
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
@@ -289,28 +288,26 @@
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

### Comparing `mypy-boto3-m2-1.28.16/mypy_boto3_m2/literals.pyi` & `mypy-boto3-m2-1.28.5/mypy_boto3_m2/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -200,15 +200,14 @@
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
@@ -287,28 +286,26 @@
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

### Comparing `mypy-boto3-m2-1.28.16/mypy_boto3_m2/paginator.py` & `mypy-boto3-m2-1.28.5/mypy_boto3_m2/paginator.py`

 * *Files 7% similar despite different names*

```diff
@@ -31,15 +31,16 @@
     list_data_set_import_history_paginator: ListDataSetImportHistoryPaginator = client.get_paginator("list_data_set_import_history")
     list_data_sets_paginator: ListDataSetsPaginator = client.get_paginator("list_data_sets")
     list_deployments_paginator: ListDeploymentsPaginator = client.get_paginator("list_deployments")
     list_engine_versions_paginator: ListEngineVersionsPaginator = client.get_paginator("list_engine_versions")
     list_environments_paginator: ListEnvironmentsPaginator = client.get_paginator("list_environments")
     ```
 """
-from typing import Generic, Iterator, Sequence, TypeVar
+from datetime import datetime
+from typing import Generic, Iterator, Sequence, TypeVar, Union
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import BatchJobExecutionStatusType, EngineTypeType
 from .type_defs import (
     ListApplicationsResponseTypeDef,
     ListApplicationVersionsResponseTypeDef,
@@ -47,15 +48,14 @@
     ListBatchJobExecutionsResponseTypeDef,
     ListDataSetImportHistoryResponseTypeDef,
     ListDataSetsResponseTypeDef,
     ListDeploymentsResponseTypeDef,
     ListEngineVersionsResponseTypeDef,
     ListEnvironmentsResponseTypeDef,
     PaginatorConfigTypeDef,
-    TimestampTypeDef,
 )
 
 __all__ = (
     "ListApplicationVersionsPaginator",
     "ListApplicationsPaginator",
     "ListBatchJobDefinitionsPaginator",
     "ListBatchJobExecutionsPaginator",
@@ -80,15 +80,15 @@
 class ListApplicationVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListApplicationVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/paginators/#listapplicationversionspaginator)
     """
 
     def paginate(
-        self, *, applicationId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, applicationId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListApplicationVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListApplicationVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/paginators/#listapplicationversionspaginator)
         """
 
 
@@ -99,15 +99,15 @@
     """
 
     def paginate(
         self,
         *,
         environmentId: str = ...,
         names: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListApplicationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListApplications.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/paginators/#listapplicationspaginator)
         """
 
 
@@ -118,15 +118,15 @@
     """
 
     def paginate(
         self,
         *,
         applicationId: str,
         prefix: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListBatchJobDefinitionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListBatchJobDefinitions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/paginators/#listbatchjobdefinitionspaginator)
         """
 
 
@@ -138,33 +138,33 @@
 
     def paginate(
         self,
         *,
         applicationId: str,
         executionIds: Sequence[str] = ...,
         jobName: str = ...,
-        startedAfter: TimestampTypeDef = ...,
-        startedBefore: TimestampTypeDef = ...,
+        startedAfter: Union[datetime, str] = ...,
+        startedBefore: Union[datetime, str] = ...,
         status: BatchJobExecutionStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListBatchJobExecutionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListBatchJobExecutions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/paginators/#listbatchjobexecutionspaginator)
         """
 
 
 class ListDataSetImportHistoryPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListDataSetImportHistory)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/paginators/#listdatasetimporthistorypaginator)
     """
 
     def paginate(
-        self, *, applicationId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, applicationId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDataSetImportHistoryResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListDataSetImportHistory.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/paginators/#listdatasetimporthistorypaginator)
         """
 
 
@@ -175,45 +175,45 @@
     """
 
     def paginate(
         self,
         *,
         applicationId: str,
         prefix: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDataSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListDataSets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/paginators/#listdatasetspaginator)
         """
 
 
 class ListDeploymentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListDeployments)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/paginators/#listdeploymentspaginator)
     """
 
     def paginate(
-        self, *, applicationId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, applicationId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDeploymentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListDeployments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/paginators/#listdeploymentspaginator)
         """
 
 
 class ListEngineVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListEngineVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/paginators/#listengineversionspaginator)
     """
 
     def paginate(
-        self, *, engineType: EngineTypeType = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, engineType: EngineTypeType = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListEngineVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListEngineVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/paginators/#listengineversionspaginator)
         """
 
 
@@ -224,13 +224,13 @@
     """
 
     def paginate(
         self,
         *,
         engineType: EngineTypeType = ...,
         names: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListEnvironmentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListEnvironments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/paginators/#listenvironmentspaginator)
         """
```

### Comparing `mypy-boto3-m2-1.28.16/mypy_boto3_m2/paginator.pyi` & `mypy-boto3-m2-1.28.5/mypy_boto3_m2/paginator.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -31,15 +31,16 @@
     list_data_set_import_history_paginator: ListDataSetImportHistoryPaginator = client.get_paginator("list_data_set_import_history")
     list_data_sets_paginator: ListDataSetsPaginator = client.get_paginator("list_data_sets")
     list_deployments_paginator: ListDeploymentsPaginator = client.get_paginator("list_deployments")
     list_engine_versions_paginator: ListEngineVersionsPaginator = client.get_paginator("list_engine_versions")
     list_environments_paginator: ListEnvironmentsPaginator = client.get_paginator("list_environments")
     ```
 """
-from typing import Generic, Iterator, Sequence, TypeVar
+from datetime import datetime
+from typing import Generic, Iterator, Sequence, TypeVar, Union
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import BatchJobExecutionStatusType, EngineTypeType
 from .type_defs import (
     ListApplicationsResponseTypeDef,
     ListApplicationVersionsResponseTypeDef,
@@ -47,15 +48,14 @@
     ListBatchJobExecutionsResponseTypeDef,
     ListDataSetImportHistoryResponseTypeDef,
     ListDataSetsResponseTypeDef,
     ListDeploymentsResponseTypeDef,
     ListEngineVersionsResponseTypeDef,
     ListEnvironmentsResponseTypeDef,
     PaginatorConfigTypeDef,
-    TimestampTypeDef,
 )
 
 __all__ = (
     "ListApplicationVersionsPaginator",
     "ListApplicationsPaginator",
     "ListBatchJobDefinitionsPaginator",
     "ListBatchJobExecutionsPaginator",
@@ -77,15 +77,15 @@
 class ListApplicationVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListApplicationVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/paginators/#listapplicationversionspaginator)
     """
 
     def paginate(
-        self, *, applicationId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, applicationId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListApplicationVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListApplicationVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/paginators/#listapplicationversionspaginator)
         """
 
 class ListApplicationsPaginator(Paginator):
@@ -95,15 +95,15 @@
     """
 
     def paginate(
         self,
         *,
         environmentId: str = ...,
         names: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListApplicationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListApplications.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/paginators/#listapplicationspaginator)
         """
 
 class ListBatchJobDefinitionsPaginator(Paginator):
@@ -113,15 +113,15 @@
     """
 
     def paginate(
         self,
         *,
         applicationId: str,
         prefix: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListBatchJobDefinitionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListBatchJobDefinitions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/paginators/#listbatchjobdefinitionspaginator)
         """
 
 class ListBatchJobExecutionsPaginator(Paginator):
@@ -132,32 +132,32 @@
 
     def paginate(
         self,
         *,
         applicationId: str,
         executionIds: Sequence[str] = ...,
         jobName: str = ...,
-        startedAfter: TimestampTypeDef = ...,
-        startedBefore: TimestampTypeDef = ...,
+        startedAfter: Union[datetime, str] = ...,
+        startedBefore: Union[datetime, str] = ...,
         status: BatchJobExecutionStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListBatchJobExecutionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListBatchJobExecutions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/paginators/#listbatchjobexecutionspaginator)
         """
 
 class ListDataSetImportHistoryPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListDataSetImportHistory)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/paginators/#listdatasetimporthistorypaginator)
     """
 
     def paginate(
-        self, *, applicationId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, applicationId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDataSetImportHistoryResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListDataSetImportHistory.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/paginators/#listdatasetimporthistorypaginator)
         """
 
 class ListDataSetsPaginator(Paginator):
@@ -167,43 +167,43 @@
     """
 
     def paginate(
         self,
         *,
         applicationId: str,
         prefix: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDataSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListDataSets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/paginators/#listdatasetspaginator)
         """
 
 class ListDeploymentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListDeployments)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/paginators/#listdeploymentspaginator)
     """
 
     def paginate(
-        self, *, applicationId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, applicationId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDeploymentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListDeployments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/paginators/#listdeploymentspaginator)
         """
 
 class ListEngineVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListEngineVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/paginators/#listengineversionspaginator)
     """
 
     def paginate(
-        self, *, engineType: EngineTypeType = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, engineType: EngineTypeType = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListEngineVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListEngineVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/paginators/#listengineversionspaginator)
         """
 
 class ListEnvironmentsPaginator(Paginator):
@@ -213,13 +213,13 @@
     """
 
     def paginate(
         self,
         *,
         engineType: EngineTypeType = ...,
         names: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListEnvironmentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListEnvironments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/paginators/#listenvironmentspaginator)
         """
```

### Comparing `mypy-boto3-m2-1.28.16/mypy_boto3_m2/type_defs.py` & `mypy-boto3-m2-1.28.5/mypy_boto3_m2/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for m2 service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_m2.type_defs import AlternateKeyTypeDef
+    from mypy_boto3_m2.type_defs import AlternateKeyOutputTypeDef
 
-    data: AlternateKeyTypeDef = ...
+    data: AlternateKeyOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -30,26 +30,32 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
+    "AlternateKeyOutputTypeDef",
     "AlternateKeyTypeDef",
     "ApplicationSummaryTypeDef",
     "ApplicationVersionSummaryTypeDef",
     "FileBatchJobDefinitionTypeDef",
     "ScriptBatchJobDefinitionTypeDef",
+    "FileBatchJobIdentifierOutputTypeDef",
+    "ScriptBatchJobIdentifierOutputTypeDef",
     "FileBatchJobIdentifierTypeDef",
     "ScriptBatchJobIdentifierTypeDef",
     "CancelBatchJobExecutionRequestRequestTypeDef",
     "DefinitionTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateApplicationResponseTypeDef",
+    "CreateDataSetImportTaskResponseTypeDef",
     "CreateDeploymentRequestRequestTypeDef",
+    "CreateDeploymentResponseTypeDef",
     "HighAvailabilityConfigTypeDef",
+    "CreateEnvironmentResponseTypeDef",
     "ExternalLocationTypeDef",
     "DataSetImportSummaryTypeDef",
     "DataSetSummaryTypeDef",
     "RecordLengthTypeDef",
     "GdgDetailAttributesTypeDef",
     "PoDetailAttributesTypeDef",
     "PsDetailAttributesTypeDef",
@@ -57,99 +63,111 @@
     "PoAttributesTypeDef",
     "PsAttributesTypeDef",
     "DeleteApplicationFromEnvironmentRequestRequestTypeDef",
     "DeleteApplicationRequestRequestTypeDef",
     "DeleteEnvironmentRequestRequestTypeDef",
     "DeployedVersionSummaryTypeDef",
     "DeploymentSummaryTypeDef",
+    "EfsStorageConfigurationOutputTypeDef",
     "EfsStorageConfigurationTypeDef",
     "EngineVersionsSummaryTypeDef",
     "EnvironmentSummaryTypeDef",
+    "FsxStorageConfigurationOutputTypeDef",
     "FsxStorageConfigurationTypeDef",
     "GetApplicationRequestRequestTypeDef",
     "LogGroupSummaryTypeDef",
     "GetApplicationVersionRequestRequestTypeDef",
+    "GetApplicationVersionResponseTypeDef",
     "GetBatchJobExecutionRequestRequestTypeDef",
     "GetDataSetDetailsRequestRequestTypeDef",
     "GetDataSetImportTaskRequestRequestTypeDef",
     "GetDeploymentRequestRequestTypeDef",
+    "GetDeploymentResponseTypeDef",
     "GetEnvironmentRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "HighAvailabilityConfigOutputTypeDef",
+    "GetSignedBluinsightsUrlResponseTypeDef",
+    "ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef",
     "ListApplicationVersionsRequestRequestTypeDef",
+    "ListApplicationsRequestListApplicationsPaginateTypeDef",
     "ListApplicationsRequestRequestTypeDef",
+    "ListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef",
     "ListBatchJobDefinitionsRequestRequestTypeDef",
-    "TimestampTypeDef",
+    "ListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef",
+    "ListBatchJobExecutionsRequestRequestTypeDef",
+    "ListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef",
     "ListDataSetImportHistoryRequestRequestTypeDef",
+    "ListDataSetsRequestListDataSetsPaginateTypeDef",
     "ListDataSetsRequestRequestTypeDef",
+    "ListDeploymentsRequestListDeploymentsPaginateTypeDef",
     "ListDeploymentsRequestRequestTypeDef",
+    "ListEngineVersionsRequestListEngineVersionsPaginateTypeDef",
     "ListEngineVersionsRequestRequestTypeDef",
+    "ListEnvironmentsRequestListEnvironmentsPaginateTypeDef",
     "ListEnvironmentsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "MaintenanceScheduleTypeDef",
+    "PaginatorConfigTypeDef",
+    "PrimaryKeyOutputTypeDef",
     "PrimaryKeyTypeDef",
+    "ResponseMetadataTypeDef",
     "StartApplicationRequestRequestTypeDef",
+    "StartBatchJobResponseTypeDef",
     "StopApplicationRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "UpdateApplicationResponseTypeDef",
     "UpdateEnvironmentRequestRequestTypeDef",
+    "UpdateEnvironmentResponseTypeDef",
+    "ListApplicationsResponseTypeDef",
+    "ListApplicationVersionsResponseTypeDef",
     "BatchJobDefinitionTypeDef",
+    "BatchJobIdentifierOutputTypeDef",
     "BatchJobIdentifierTypeDef",
     "CreateApplicationRequestRequestTypeDef",
     "UpdateApplicationRequestRequestTypeDef",
-    "CreateApplicationResponseTypeDef",
-    "CreateDataSetImportTaskResponseTypeDef",
-    "CreateDeploymentResponseTypeDef",
-    "CreateEnvironmentResponseTypeDef",
-    "GetApplicationVersionResponseTypeDef",
-    "GetDeploymentResponseTypeDef",
-    "GetSignedBluinsightsUrlResponseTypeDef",
-    "ListApplicationVersionsResponseTypeDef",
-    "ListApplicationsResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "StartBatchJobResponseTypeDef",
-    "UpdateApplicationResponseTypeDef",
-    "UpdateEnvironmentResponseTypeDef",
     "DataSetImportTaskTypeDef",
     "GetDataSetImportTaskResponseTypeDef",
     "ListDataSetsResponseTypeDef",
     "ListDeploymentsResponseTypeDef",
     "ListEngineVersionsResponseTypeDef",
     "ListEnvironmentsResponseTypeDef",
+    "StorageConfigurationOutputTypeDef",
     "StorageConfigurationTypeDef",
     "GetApplicationResponseTypeDef",
-    "ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef",
-    "ListApplicationsRequestListApplicationsPaginateTypeDef",
-    "ListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef",
-    "ListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef",
-    "ListDataSetsRequestListDataSetsPaginateTypeDef",
-    "ListDeploymentsRequestListDeploymentsPaginateTypeDef",
-    "ListEngineVersionsRequestListEngineVersionsPaginateTypeDef",
-    "ListEnvironmentsRequestListEnvironmentsPaginateTypeDef",
-    "ListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef",
-    "ListBatchJobExecutionsRequestRequestTypeDef",
     "PendingMaintenanceTypeDef",
-    "VsamAttributesTypeDef",
     "VsamDetailAttributesTypeDef",
+    "VsamAttributesTypeDef",
     "ListBatchJobDefinitionsResponseTypeDef",
     "BatchJobExecutionSummaryTypeDef",
     "GetBatchJobExecutionResponseTypeDef",
     "StartBatchJobRequestRequestTypeDef",
     "ListDataSetImportHistoryResponseTypeDef",
     "CreateEnvironmentRequestRequestTypeDef",
     "GetEnvironmentResponseTypeDef",
-    "DatasetOrgAttributesTypeDef",
     "DatasetDetailOrgAttributesTypeDef",
+    "DatasetOrgAttributesTypeDef",
     "ListBatchJobExecutionsResponseTypeDef",
-    "DataSetTypeDef",
     "GetDataSetDetailsResponseTypeDef",
+    "DataSetTypeDef",
     "DataSetImportItemTypeDef",
     "DataSetImportConfigTypeDef",
     "CreateDataSetImportTaskRequestRequestTypeDef",
 )
 
+AlternateKeyOutputTypeDef = TypedDict(
+    "AlternateKeyOutputTypeDef",
+    {
+        "allowDuplicates": bool,
+        "length": int,
+        "name": str,
+        "offset": int,
+    },
+)
+
 _RequiredAlternateKeyTypeDef = TypedDict(
     "_RequiredAlternateKeyTypeDef",
     {
         "length": int,
         "offset": int,
     },
 )
@@ -163,92 +181,68 @@
 )
 
 
 class AlternateKeyTypeDef(_RequiredAlternateKeyTypeDef, _OptionalAlternateKeyTypeDef):
     pass
 
 
-_RequiredApplicationSummaryTypeDef = TypedDict(
-    "_RequiredApplicationSummaryTypeDef",
+ApplicationSummaryTypeDef = TypedDict(
+    "ApplicationSummaryTypeDef",
     {
         "applicationArn": str,
         "applicationId": str,
         "applicationVersion": int,
         "creationTime": datetime,
-        "engineType": EngineTypeType,
-        "name": str,
-        "status": ApplicationLifecycleType,
-    },
-)
-_OptionalApplicationSummaryTypeDef = TypedDict(
-    "_OptionalApplicationSummaryTypeDef",
-    {
         "deploymentStatus": ApplicationDeploymentLifecycleType,
         "description": str,
+        "engineType": EngineTypeType,
         "environmentId": str,
         "lastStartTime": datetime,
+        "name": str,
         "roleArn": str,
+        "status": ApplicationLifecycleType,
         "versionStatus": ApplicationVersionLifecycleType,
     },
-    total=False,
 )
 
-
-class ApplicationSummaryTypeDef(
-    _RequiredApplicationSummaryTypeDef, _OptionalApplicationSummaryTypeDef
-):
-    pass
-
-
-_RequiredApplicationVersionSummaryTypeDef = TypedDict(
-    "_RequiredApplicationVersionSummaryTypeDef",
+ApplicationVersionSummaryTypeDef = TypedDict(
+    "ApplicationVersionSummaryTypeDef",
     {
         "applicationVersion": int,
         "creationTime": datetime,
         "status": ApplicationVersionLifecycleType,
+        "statusReason": str,
     },
 )
-_OptionalApplicationVersionSummaryTypeDef = TypedDict(
-    "_OptionalApplicationVersionSummaryTypeDef",
+
+FileBatchJobDefinitionTypeDef = TypedDict(
+    "FileBatchJobDefinitionTypeDef",
     {
-        "statusReason": str,
+        "fileName": str,
+        "folderPath": str,
     },
-    total=False,
 )
 
-
-class ApplicationVersionSummaryTypeDef(
-    _RequiredApplicationVersionSummaryTypeDef, _OptionalApplicationVersionSummaryTypeDef
-):
-    pass
-
-
-_RequiredFileBatchJobDefinitionTypeDef = TypedDict(
-    "_RequiredFileBatchJobDefinitionTypeDef",
+ScriptBatchJobDefinitionTypeDef = TypedDict(
+    "ScriptBatchJobDefinitionTypeDef",
     {
-        "fileName": str,
+        "scriptName": str,
     },
 )
-_OptionalFileBatchJobDefinitionTypeDef = TypedDict(
-    "_OptionalFileBatchJobDefinitionTypeDef",
+
+FileBatchJobIdentifierOutputTypeDef = TypedDict(
+    "FileBatchJobIdentifierOutputTypeDef",
     {
+        "fileName": str,
         "folderPath": str,
     },
-    total=False,
 )
 
-
-class FileBatchJobDefinitionTypeDef(
-    _RequiredFileBatchJobDefinitionTypeDef, _OptionalFileBatchJobDefinitionTypeDef
-):
-    pass
-
-
-ScriptBatchJobDefinitionTypeDef = TypedDict(
-    "ScriptBatchJobDefinitionTypeDef",
+ScriptBatchJobIdentifierOutputTypeDef = TypedDict(
+    "ScriptBatchJobIdentifierOutputTypeDef",
     {
         "scriptName": str,
     },
 )
 
 _RequiredFileBatchJobIdentifierTypeDef = TypedDict(
     "_RequiredFileBatchJobIdentifierTypeDef",
@@ -291,22 +285,29 @@
     {
         "content": str,
         "s3Location": str,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateApplicationResponseTypeDef = TypedDict(
+    "CreateApplicationResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "applicationArn": str,
+        "applicationId": str,
+        "applicationVersion": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateDataSetImportTaskResponseTypeDef = TypedDict(
+    "CreateDataSetImportTaskResponseTypeDef",
+    {
+        "taskId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateDeploymentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDeploymentRequestRequestTypeDef",
     {
         "applicationId": str,
@@ -325,21 +326,37 @@
 
 class CreateDeploymentRequestRequestTypeDef(
     _RequiredCreateDeploymentRequestRequestTypeDef, _OptionalCreateDeploymentRequestRequestTypeDef
 ):
     pass
 
 
+CreateDeploymentResponseTypeDef = TypedDict(
+    "CreateDeploymentResponseTypeDef",
+    {
+        "deploymentId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 HighAvailabilityConfigTypeDef = TypedDict(
     "HighAvailabilityConfigTypeDef",
     {
         "desiredCapacity": int,
     },
 )
 
+CreateEnvironmentResponseTypeDef = TypedDict(
+    "CreateEnvironmentResponseTypeDef",
+    {
+        "environmentId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ExternalLocationTypeDef = TypedDict(
     "ExternalLocationTypeDef",
     {
         "s3Location": str,
     },
     total=False,
 )
@@ -351,52 +368,40 @@
         "inProgress": int,
         "pending": int,
         "succeeded": int,
         "total": int,
     },
 )
 
-_RequiredDataSetSummaryTypeDef = TypedDict(
-    "_RequiredDataSetSummaryTypeDef",
-    {
-        "dataSetName": str,
-    },
-)
-_OptionalDataSetSummaryTypeDef = TypedDict(
-    "_OptionalDataSetSummaryTypeDef",
+DataSetSummaryTypeDef = TypedDict(
+    "DataSetSummaryTypeDef",
     {
         "creationTime": datetime,
+        "dataSetName": str,
         "dataSetOrg": str,
         "format": str,
         "lastReferencedTime": datetime,
         "lastUpdatedTime": datetime,
     },
-    total=False,
 )
 
-
-class DataSetSummaryTypeDef(_RequiredDataSetSummaryTypeDef, _OptionalDataSetSummaryTypeDef):
-    pass
-
-
 RecordLengthTypeDef = TypedDict(
     "RecordLengthTypeDef",
     {
         "max": int,
         "min": int,
     },
 )
 
 GdgDetailAttributesTypeDef = TypedDict(
     "GdgDetailAttributesTypeDef",
     {
         "limit": int,
         "rollDisposition": str,
     },
-    total=False,
 )
 
 PoDetailAttributesTypeDef = TypedDict(
     "PoDetailAttributesTypeDef",
     {
         "encoding": str,
         "format": str,
@@ -477,62 +482,44 @@
 DeleteEnvironmentRequestRequestTypeDef = TypedDict(
     "DeleteEnvironmentRequestRequestTypeDef",
     {
         "environmentId": str,
     },
 )
 
-_RequiredDeployedVersionSummaryTypeDef = TypedDict(
-    "_RequiredDeployedVersionSummaryTypeDef",
+DeployedVersionSummaryTypeDef = TypedDict(
+    "DeployedVersionSummaryTypeDef",
     {
         "applicationVersion": int,
         "status": DeploymentLifecycleType,
-    },
-)
-_OptionalDeployedVersionSummaryTypeDef = TypedDict(
-    "_OptionalDeployedVersionSummaryTypeDef",
-    {
         "statusReason": str,
     },
-    total=False,
 )
 
-
-class DeployedVersionSummaryTypeDef(
-    _RequiredDeployedVersionSummaryTypeDef, _OptionalDeployedVersionSummaryTypeDef
-):
-    pass
-
-
-_RequiredDeploymentSummaryTypeDef = TypedDict(
-    "_RequiredDeploymentSummaryTypeDef",
+DeploymentSummaryTypeDef = TypedDict(
+    "DeploymentSummaryTypeDef",
     {
         "applicationId": str,
         "applicationVersion": int,
         "creationTime": datetime,
         "deploymentId": str,
         "environmentId": str,
         "status": DeploymentLifecycleType,
+        "statusReason": str,
     },
 )
-_OptionalDeploymentSummaryTypeDef = TypedDict(
-    "_OptionalDeploymentSummaryTypeDef",
+
+EfsStorageConfigurationOutputTypeDef = TypedDict(
+    "EfsStorageConfigurationOutputTypeDef",
     {
-        "statusReason": str,
+        "fileSystemId": str,
+        "mountPoint": str,
     },
-    total=False,
 )
 
-
-class DeploymentSummaryTypeDef(
-    _RequiredDeploymentSummaryTypeDef, _OptionalDeploymentSummaryTypeDef
-):
-    pass
-
-
 EfsStorageConfigurationTypeDef = TypedDict(
     "EfsStorageConfigurationTypeDef",
     {
         "fileSystemId": str,
         "mountPoint": str,
     },
 )
@@ -555,14 +542,22 @@
         "environmentId": str,
         "instanceType": str,
         "name": str,
         "status": EnvironmentLifecycleType,
     },
 )
 
+FsxStorageConfigurationOutputTypeDef = TypedDict(
+    "FsxStorageConfigurationOutputTypeDef",
+    {
+        "fileSystemId": str,
+        "mountPoint": str,
+    },
+)
+
 FsxStorageConfigurationTypeDef = TypedDict(
     "FsxStorageConfigurationTypeDef",
     {
         "fileSystemId": str,
         "mountPoint": str,
     },
 )
@@ -586,14 +581,28 @@
     "GetApplicationVersionRequestRequestTypeDef",
     {
         "applicationId": str,
         "applicationVersion": int,
     },
 )
 
+GetApplicationVersionResponseTypeDef = TypedDict(
+    "GetApplicationVersionResponseTypeDef",
+    {
+        "applicationVersion": int,
+        "creationTime": datetime,
+        "definitionContent": str,
+        "description": str,
+        "name": str,
+        "status": ApplicationVersionLifecycleType,
+        "statusReason": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetBatchJobExecutionRequestRequestTypeDef = TypedDict(
     "GetBatchJobExecutionRequestRequestTypeDef",
     {
         "applicationId": str,
         "executionId": str,
     },
 )
@@ -618,31 +627,72 @@
     "GetDeploymentRequestRequestTypeDef",
     {
         "applicationId": str,
         "deploymentId": str,
     },
 )
 
+GetDeploymentResponseTypeDef = TypedDict(
+    "GetDeploymentResponseTypeDef",
+    {
+        "applicationId": str,
+        "applicationVersion": int,
+        "creationTime": datetime,
+        "deploymentId": str,
+        "environmentId": str,
+        "status": DeploymentLifecycleType,
+        "statusReason": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetEnvironmentRequestRequestTypeDef = TypedDict(
     "GetEnvironmentRequestRequestTypeDef",
     {
         "environmentId": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+HighAvailabilityConfigOutputTypeDef = TypedDict(
+    "HighAvailabilityConfigOutputTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "desiredCapacity": int,
+    },
+)
+
+GetSignedBluinsightsUrlResponseTypeDef = TypedDict(
+    "GetSignedBluinsightsUrlResponseTypeDef",
+    {
+        "signedBiUrl": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef",
+    {
+        "applicationId": str,
+    },
+)
+_OptionalListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
+class ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef(
+    _RequiredListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef,
+    _OptionalListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListApplicationVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListApplicationVersionsRequestRequestTypeDef",
     {
         "applicationId": str,
     },
 )
 _OptionalListApplicationVersionsRequestRequestTypeDef = TypedDict(
@@ -658,25 +708,58 @@
 class ListApplicationVersionsRequestRequestTypeDef(
     _RequiredListApplicationVersionsRequestRequestTypeDef,
     _OptionalListApplicationVersionsRequestRequestTypeDef,
 ):
     pass
 
 
+ListApplicationsRequestListApplicationsPaginateTypeDef = TypedDict(
+    "ListApplicationsRequestListApplicationsPaginateTypeDef",
+    {
+        "environmentId": str,
+        "names": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListApplicationsRequestRequestTypeDef = TypedDict(
     "ListApplicationsRequestRequestTypeDef",
     {
         "environmentId": str,
         "maxResults": int,
         "names": Sequence[str],
         "nextToken": str,
     },
     total=False,
 )
 
+_RequiredListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef = TypedDict(
+    "_RequiredListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef",
+    {
+        "applicationId": str,
+    },
+)
+_OptionalListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef = TypedDict(
+    "_OptionalListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef",
+    {
+        "prefix": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef(
+    _RequiredListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef,
+    _OptionalListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListBatchJobDefinitionsRequestRequestTypeDef = TypedDict(
     "_RequiredListBatchJobDefinitionsRequestRequestTypeDef",
     {
         "applicationId": str,
     },
 )
 _OptionalListBatchJobDefinitionsRequestRequestTypeDef = TypedDict(
@@ -693,15 +776,91 @@
 class ListBatchJobDefinitionsRequestRequestTypeDef(
     _RequiredListBatchJobDefinitionsRequestRequestTypeDef,
     _OptionalListBatchJobDefinitionsRequestRequestTypeDef,
 ):
     pass
 
 
-TimestampTypeDef = Union[datetime, str]
+_RequiredListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef = TypedDict(
+    "_RequiredListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef",
+    {
+        "applicationId": str,
+    },
+)
+_OptionalListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef = TypedDict(
+    "_OptionalListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef",
+    {
+        "executionIds": Sequence[str],
+        "jobName": str,
+        "startedAfter": Union[datetime, str],
+        "startedBefore": Union[datetime, str],
+        "status": BatchJobExecutionStatusType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef(
+    _RequiredListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef,
+    _OptionalListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListBatchJobExecutionsRequestRequestTypeDef = TypedDict(
+    "_RequiredListBatchJobExecutionsRequestRequestTypeDef",
+    {
+        "applicationId": str,
+    },
+)
+_OptionalListBatchJobExecutionsRequestRequestTypeDef = TypedDict(
+    "_OptionalListBatchJobExecutionsRequestRequestTypeDef",
+    {
+        "executionIds": Sequence[str],
+        "jobName": str,
+        "maxResults": int,
+        "nextToken": str,
+        "startedAfter": Union[datetime, str],
+        "startedBefore": Union[datetime, str],
+        "status": BatchJobExecutionStatusType,
+    },
+    total=False,
+)
+
+
+class ListBatchJobExecutionsRequestRequestTypeDef(
+    _RequiredListBatchJobExecutionsRequestRequestTypeDef,
+    _OptionalListBatchJobExecutionsRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef = TypedDict(
+    "_RequiredListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef",
+    {
+        "applicationId": str,
+    },
+)
+_OptionalListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef = TypedDict(
+    "_OptionalListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef(
+    _RequiredListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef,
+    _OptionalListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListDataSetImportHistoryRequestRequestTypeDef = TypedDict(
     "_RequiredListDataSetImportHistoryRequestRequestTypeDef",
     {
         "applicationId": str,
     },
 )
 _OptionalListDataSetImportHistoryRequestRequestTypeDef = TypedDict(
@@ -717,14 +876,37 @@
 class ListDataSetImportHistoryRequestRequestTypeDef(
     _RequiredListDataSetImportHistoryRequestRequestTypeDef,
     _OptionalListDataSetImportHistoryRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredListDataSetsRequestListDataSetsPaginateTypeDef = TypedDict(
+    "_RequiredListDataSetsRequestListDataSetsPaginateTypeDef",
+    {
+        "applicationId": str,
+    },
+)
+_OptionalListDataSetsRequestListDataSetsPaginateTypeDef = TypedDict(
+    "_OptionalListDataSetsRequestListDataSetsPaginateTypeDef",
+    {
+        "prefix": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListDataSetsRequestListDataSetsPaginateTypeDef(
+    _RequiredListDataSetsRequestListDataSetsPaginateTypeDef,
+    _OptionalListDataSetsRequestListDataSetsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListDataSetsRequestRequestTypeDef = TypedDict(
     "_RequiredListDataSetsRequestRequestTypeDef",
     {
         "applicationId": str,
     },
 )
 _OptionalListDataSetsRequestRequestTypeDef = TypedDict(
@@ -740,14 +922,36 @@
 
 class ListDataSetsRequestRequestTypeDef(
     _RequiredListDataSetsRequestRequestTypeDef, _OptionalListDataSetsRequestRequestTypeDef
 ):
     pass
 
 
+_RequiredListDeploymentsRequestListDeploymentsPaginateTypeDef = TypedDict(
+    "_RequiredListDeploymentsRequestListDeploymentsPaginateTypeDef",
+    {
+        "applicationId": str,
+    },
+)
+_OptionalListDeploymentsRequestListDeploymentsPaginateTypeDef = TypedDict(
+    "_OptionalListDeploymentsRequestListDeploymentsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListDeploymentsRequestListDeploymentsPaginateTypeDef(
+    _RequiredListDeploymentsRequestListDeploymentsPaginateTypeDef,
+    _OptionalListDeploymentsRequestListDeploymentsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListDeploymentsRequestRequestTypeDef = TypedDict(
     "_RequiredListDeploymentsRequestRequestTypeDef",
     {
         "applicationId": str,
     },
 )
 _OptionalListDeploymentsRequestRequestTypeDef = TypedDict(
@@ -762,24 +966,43 @@
 
 class ListDeploymentsRequestRequestTypeDef(
     _RequiredListDeploymentsRequestRequestTypeDef, _OptionalListDeploymentsRequestRequestTypeDef
 ):
     pass
 
 
+ListEngineVersionsRequestListEngineVersionsPaginateTypeDef = TypedDict(
+    "ListEngineVersionsRequestListEngineVersionsPaginateTypeDef",
+    {
+        "engineType": EngineTypeType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListEngineVersionsRequestRequestTypeDef = TypedDict(
     "ListEngineVersionsRequestRequestTypeDef",
     {
         "engineType": EngineTypeType,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+ListEnvironmentsRequestListEnvironmentsPaginateTypeDef = TypedDict(
+    "ListEnvironmentsRequestListEnvironmentsPaginateTypeDef",
+    {
+        "engineType": EngineTypeType,
+        "names": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListEnvironmentsRequestRequestTypeDef = TypedDict(
     "ListEnvironmentsRequestRequestTypeDef",
     {
         "engineType": EngineTypeType,
         "maxResults": int,
         "names": Sequence[str],
         "nextToken": str,
@@ -790,23 +1013,49 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 MaintenanceScheduleTypeDef = TypedDict(
     "MaintenanceScheduleTypeDef",
     {
         "endTime": datetime,
         "startTime": datetime,
     },
+)
+
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
+    {
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
+    },
     total=False,
 )
 
+PrimaryKeyOutputTypeDef = TypedDict(
+    "PrimaryKeyOutputTypeDef",
+    {
+        "length": int,
+        "name": str,
+        "offset": int,
+    },
+)
+
 _RequiredPrimaryKeyTypeDef = TypedDict(
     "_RequiredPrimaryKeyTypeDef",
     {
         "length": int,
         "offset": int,
     },
 )
@@ -819,21 +1068,40 @@
 )
 
 
 class PrimaryKeyTypeDef(_RequiredPrimaryKeyTypeDef, _OptionalPrimaryKeyTypeDef):
     pass
 
 
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
+    {
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
 StartApplicationRequestRequestTypeDef = TypedDict(
     "StartApplicationRequestRequestTypeDef",
     {
         "applicationId": str,
     },
 )
 
+StartBatchJobResponseTypeDef = TypedDict(
+    "StartBatchJobResponseTypeDef",
+    {
+        "executionId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredStopApplicationRequestRequestTypeDef = TypedDict(
     "_RequiredStopApplicationRequestRequestTypeDef",
     {
         "applicationId": str,
     },
 )
 _OptionalStopApplicationRequestRequestTypeDef = TypedDict(
@@ -863,14 +1131,22 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
+UpdateApplicationResponseTypeDef = TypedDict(
+    "UpdateApplicationResponseTypeDef",
+    {
+        "applicationVersion": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpdateEnvironmentRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateEnvironmentRequestRequestTypeDef",
     {
         "environmentId": str,
     },
 )
 _OptionalUpdateEnvironmentRequestRequestTypeDef = TypedDict(
@@ -888,21 +1164,54 @@
 
 class UpdateEnvironmentRequestRequestTypeDef(
     _RequiredUpdateEnvironmentRequestRequestTypeDef, _OptionalUpdateEnvironmentRequestRequestTypeDef
 ):
     pass
 
 
+UpdateEnvironmentResponseTypeDef = TypedDict(
+    "UpdateEnvironmentResponseTypeDef",
+    {
+        "environmentId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListApplicationsResponseTypeDef = TypedDict(
+    "ListApplicationsResponseTypeDef",
+    {
+        "applications": List[ApplicationSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListApplicationVersionsResponseTypeDef = TypedDict(
+    "ListApplicationVersionsResponseTypeDef",
+    {
+        "applicationVersions": List[ApplicationVersionSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 BatchJobDefinitionTypeDef = TypedDict(
     "BatchJobDefinitionTypeDef",
     {
         "fileBatchJobDefinition": FileBatchJobDefinitionTypeDef,
         "scriptBatchJobDefinition": ScriptBatchJobDefinitionTypeDef,
     },
-    total=False,
+)
+
+BatchJobIdentifierOutputTypeDef = TypedDict(
+    "BatchJobIdentifierOutputTypeDef",
+    {
+        "fileBatchJobIdentifier": FileBatchJobIdentifierOutputTypeDef,
+        "scriptBatchJobIdentifier": ScriptBatchJobIdentifierOutputTypeDef,
+    },
 )
 
 BatchJobIdentifierTypeDef = TypedDict(
     "BatchJobIdentifierTypeDef",
     {
         "fileBatchJobIdentifier": FileBatchJobIdentifierTypeDef,
         "scriptBatchJobIdentifier": ScriptBatchJobIdentifierTypeDef,
@@ -956,134 +1265,14 @@
 
 class UpdateApplicationRequestRequestTypeDef(
     _RequiredUpdateApplicationRequestRequestTypeDef, _OptionalUpdateApplicationRequestRequestTypeDef
 ):
     pass
 
 
-CreateApplicationResponseTypeDef = TypedDict(
-    "CreateApplicationResponseTypeDef",
-    {
-        "applicationArn": str,
-        "applicationId": str,
-        "applicationVersion": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateDataSetImportTaskResponseTypeDef = TypedDict(
-    "CreateDataSetImportTaskResponseTypeDef",
-    {
-        "taskId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateDeploymentResponseTypeDef = TypedDict(
-    "CreateDeploymentResponseTypeDef",
-    {
-        "deploymentId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateEnvironmentResponseTypeDef = TypedDict(
-    "CreateEnvironmentResponseTypeDef",
-    {
-        "environmentId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetApplicationVersionResponseTypeDef = TypedDict(
-    "GetApplicationVersionResponseTypeDef",
-    {
-        "applicationVersion": int,
-        "creationTime": datetime,
-        "definitionContent": str,
-        "description": str,
-        "name": str,
-        "status": ApplicationVersionLifecycleType,
-        "statusReason": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetDeploymentResponseTypeDef = TypedDict(
-    "GetDeploymentResponseTypeDef",
-    {
-        "applicationId": str,
-        "applicationVersion": int,
-        "creationTime": datetime,
-        "deploymentId": str,
-        "environmentId": str,
-        "status": DeploymentLifecycleType,
-        "statusReason": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetSignedBluinsightsUrlResponseTypeDef = TypedDict(
-    "GetSignedBluinsightsUrlResponseTypeDef",
-    {
-        "signedBiUrl": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListApplicationVersionsResponseTypeDef = TypedDict(
-    "ListApplicationVersionsResponseTypeDef",
-    {
-        "applicationVersions": List[ApplicationVersionSummaryTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListApplicationsResponseTypeDef = TypedDict(
-    "ListApplicationsResponseTypeDef",
-    {
-        "applications": List[ApplicationSummaryTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartBatchJobResponseTypeDef = TypedDict(
-    "StartBatchJobResponseTypeDef",
-    {
-        "executionId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateApplicationResponseTypeDef = TypedDict(
-    "UpdateApplicationResponseTypeDef",
-    {
-        "applicationVersion": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateEnvironmentResponseTypeDef = TypedDict(
-    "UpdateEnvironmentResponseTypeDef",
-    {
-        "environmentId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 DataSetImportTaskTypeDef = TypedDict(
     "DataSetImportTaskTypeDef",
     {
         "status": DataSetTaskLifecycleType,
         "summary": DataSetImportSummaryTypeDef,
         "taskId": str,
     },
@@ -1091,51 +1280,59 @@
 
 GetDataSetImportTaskResponseTypeDef = TypedDict(
     "GetDataSetImportTaskResponseTypeDef",
     {
         "status": DataSetTaskLifecycleType,
         "summary": DataSetImportSummaryTypeDef,
         "taskId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDataSetsResponseTypeDef = TypedDict(
     "ListDataSetsResponseTypeDef",
     {
         "dataSets": List[DataSetSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDeploymentsResponseTypeDef = TypedDict(
     "ListDeploymentsResponseTypeDef",
     {
         "deployments": List[DeploymentSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListEngineVersionsResponseTypeDef = TypedDict(
     "ListEngineVersionsResponseTypeDef",
     {
         "engineVersions": List[EngineVersionsSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListEnvironmentsResponseTypeDef = TypedDict(
     "ListEnvironmentsResponseTypeDef",
     {
         "environments": List[EnvironmentSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+StorageConfigurationOutputTypeDef = TypedDict(
+    "StorageConfigurationOutputTypeDef",
+    {
+        "efs": EfsStorageConfigurationOutputTypeDef,
+        "fsx": FsxStorageConfigurationOutputTypeDef,
     },
 )
 
 StorageConfigurationTypeDef = TypedDict(
     "StorageConfigurationTypeDef",
     {
         "efs": EfsStorageConfigurationTypeDef,
@@ -1163,221 +1360,36 @@
         "logGroups": List[LogGroupSummaryTypeDef],
         "name": str,
         "roleArn": str,
         "status": ApplicationLifecycleType,
         "statusReason": str,
         "tags": Dict[str, str],
         "targetGroupArns": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef",
-    {
-        "applicationId": str,
-    },
-)
-_OptionalListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef(
-    _RequiredListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef,
-    _OptionalListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef,
-):
-    pass
-
-
-ListApplicationsRequestListApplicationsPaginateTypeDef = TypedDict(
-    "ListApplicationsRequestListApplicationsPaginateTypeDef",
-    {
-        "environmentId": str,
-        "names": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef = TypedDict(
-    "_RequiredListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef",
-    {
-        "applicationId": str,
-    },
-)
-_OptionalListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef = TypedDict(
-    "_OptionalListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef",
-    {
-        "prefix": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-
-class ListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef(
-    _RequiredListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef,
-    _OptionalListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef = TypedDict(
-    "_RequiredListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef",
-    {
-        "applicationId": str,
-    },
-)
-_OptionalListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef = TypedDict(
-    "_OptionalListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef(
-    _RequiredListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef,
-    _OptionalListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListDataSetsRequestListDataSetsPaginateTypeDef = TypedDict(
-    "_RequiredListDataSetsRequestListDataSetsPaginateTypeDef",
-    {
-        "applicationId": str,
-    },
-)
-_OptionalListDataSetsRequestListDataSetsPaginateTypeDef = TypedDict(
-    "_OptionalListDataSetsRequestListDataSetsPaginateTypeDef",
-    {
-        "prefix": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListDataSetsRequestListDataSetsPaginateTypeDef(
-    _RequiredListDataSetsRequestListDataSetsPaginateTypeDef,
-    _OptionalListDataSetsRequestListDataSetsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListDeploymentsRequestListDeploymentsPaginateTypeDef = TypedDict(
-    "_RequiredListDeploymentsRequestListDeploymentsPaginateTypeDef",
-    {
-        "applicationId": str,
-    },
-)
-_OptionalListDeploymentsRequestListDeploymentsPaginateTypeDef = TypedDict(
-    "_OptionalListDeploymentsRequestListDeploymentsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListDeploymentsRequestListDeploymentsPaginateTypeDef(
-    _RequiredListDeploymentsRequestListDeploymentsPaginateTypeDef,
-    _OptionalListDeploymentsRequestListDeploymentsPaginateTypeDef,
-):
-    pass
-
-
-ListEngineVersionsRequestListEngineVersionsPaginateTypeDef = TypedDict(
-    "ListEngineVersionsRequestListEngineVersionsPaginateTypeDef",
-    {
-        "engineType": EngineTypeType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListEnvironmentsRequestListEnvironmentsPaginateTypeDef = TypedDict(
-    "ListEnvironmentsRequestListEnvironmentsPaginateTypeDef",
-    {
-        "engineType": EngineTypeType,
-        "names": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef = TypedDict(
-    "_RequiredListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef",
-    {
-        "applicationId": str,
-    },
-)
-_OptionalListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef = TypedDict(
-    "_OptionalListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef",
-    {
-        "executionIds": Sequence[str],
-        "jobName": str,
-        "startedAfter": TimestampTypeDef,
-        "startedBefore": TimestampTypeDef,
-        "status": BatchJobExecutionStatusType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef(
-    _RequiredListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef,
-    _OptionalListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListBatchJobExecutionsRequestRequestTypeDef = TypedDict(
-    "_RequiredListBatchJobExecutionsRequestRequestTypeDef",
-    {
-        "applicationId": str,
-    },
-)
-_OptionalListBatchJobExecutionsRequestRequestTypeDef = TypedDict(
-    "_OptionalListBatchJobExecutionsRequestRequestTypeDef",
-    {
-        "executionIds": Sequence[str],
-        "jobName": str,
-        "maxResults": int,
-        "nextToken": str,
-        "startedAfter": TimestampTypeDef,
-        "startedBefore": TimestampTypeDef,
-        "status": BatchJobExecutionStatusType,
-    },
-    total=False,
-)
-
-
-class ListBatchJobExecutionsRequestRequestTypeDef(
-    _RequiredListBatchJobExecutionsRequestRequestTypeDef,
-    _OptionalListBatchJobExecutionsRequestRequestTypeDef,
-):
-    pass
-
-
 PendingMaintenanceTypeDef = TypedDict(
     "PendingMaintenanceTypeDef",
     {
         "engineVersion": str,
         "schedule": MaintenanceScheduleTypeDef,
     },
-    total=False,
+)
+
+VsamDetailAttributesTypeDef = TypedDict(
+    "VsamDetailAttributesTypeDef",
+    {
+        "alternateKeys": List[AlternateKeyOutputTypeDef],
+        "cacheAtStartup": bool,
+        "compressed": bool,
+        "encoding": str,
+        "primaryKey": PrimaryKeyOutputTypeDef,
+        "recordFormat": str,
+    },
 )
 
 _RequiredVsamAttributesTypeDef = TypedDict(
     "_RequiredVsamAttributesTypeDef",
     {
         "format": str,
     },
@@ -1394,81 +1406,55 @@
 )
 
 
 class VsamAttributesTypeDef(_RequiredVsamAttributesTypeDef, _OptionalVsamAttributesTypeDef):
     pass
 
 
-VsamDetailAttributesTypeDef = TypedDict(
-    "VsamDetailAttributesTypeDef",
-    {
-        "alternateKeys": List[AlternateKeyTypeDef],
-        "cacheAtStartup": bool,
-        "compressed": bool,
-        "encoding": str,
-        "primaryKey": PrimaryKeyTypeDef,
-        "recordFormat": str,
-    },
-    total=False,
-)
-
 ListBatchJobDefinitionsResponseTypeDef = TypedDict(
     "ListBatchJobDefinitionsResponseTypeDef",
     {
         "batchJobDefinitions": List[BatchJobDefinitionTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredBatchJobExecutionSummaryTypeDef = TypedDict(
-    "_RequiredBatchJobExecutionSummaryTypeDef",
+BatchJobExecutionSummaryTypeDef = TypedDict(
+    "BatchJobExecutionSummaryTypeDef",
     {
         "applicationId": str,
-        "executionId": str,
-        "startTime": datetime,
-        "status": BatchJobExecutionStatusType,
-    },
-)
-_OptionalBatchJobExecutionSummaryTypeDef = TypedDict(
-    "_OptionalBatchJobExecutionSummaryTypeDef",
-    {
-        "batchJobIdentifier": BatchJobIdentifierTypeDef,
+        "batchJobIdentifier": BatchJobIdentifierOutputTypeDef,
         "endTime": datetime,
+        "executionId": str,
         "jobId": str,
         "jobName": str,
         "jobType": BatchJobTypeType,
         "returnCode": str,
+        "startTime": datetime,
+        "status": BatchJobExecutionStatusType,
     },
-    total=False,
 )
 
-
-class BatchJobExecutionSummaryTypeDef(
-    _RequiredBatchJobExecutionSummaryTypeDef, _OptionalBatchJobExecutionSummaryTypeDef
-):
-    pass
-
-
 GetBatchJobExecutionResponseTypeDef = TypedDict(
     "GetBatchJobExecutionResponseTypeDef",
     {
         "applicationId": str,
-        "batchJobIdentifier": BatchJobIdentifierTypeDef,
+        "batchJobIdentifier": BatchJobIdentifierOutputTypeDef,
         "endTime": datetime,
         "executionId": str,
         "jobId": str,
         "jobName": str,
         "jobType": BatchJobTypeType,
         "jobUser": str,
         "returnCode": str,
         "startTime": datetime,
         "status": BatchJobExecutionStatusType,
         "statusReason": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredStartBatchJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartBatchJobRequestRequestTypeDef",
     {
         "applicationId": str,
@@ -1491,15 +1477,15 @@
 
 
 ListDataSetImportHistoryResponseTypeDef = TypedDict(
     "ListDataSetImportHistoryResponseTypeDef",
     {
         "dataSetImportTasks": List[DataSetImportTaskTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateEnvironmentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateEnvironmentRequestRequestTypeDef",
     {
         "engineType": EngineTypeType,
@@ -1538,61 +1524,75 @@
         "actualCapacity": int,
         "creationTime": datetime,
         "description": str,
         "engineType": EngineTypeType,
         "engineVersion": str,
         "environmentArn": str,
         "environmentId": str,
-        "highAvailabilityConfig": HighAvailabilityConfigTypeDef,
+        "highAvailabilityConfig": HighAvailabilityConfigOutputTypeDef,
         "instanceType": str,
         "kmsKeyId": str,
         "loadBalancerArn": str,
         "name": str,
         "pendingMaintenance": PendingMaintenanceTypeDef,
         "preferredMaintenanceWindow": str,
         "publiclyAccessible": bool,
         "securityGroupIds": List[str],
         "status": EnvironmentLifecycleType,
         "statusReason": str,
-        "storageConfigurations": List[StorageConfigurationTypeDef],
+        "storageConfigurations": List[StorageConfigurationOutputTypeDef],
         "subnetIds": List[str],
         "tags": Dict[str, str],
         "vpcId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DatasetOrgAttributesTypeDef = TypedDict(
-    "DatasetOrgAttributesTypeDef",
-    {
-        "gdg": GdgAttributesTypeDef,
-        "po": PoAttributesTypeDef,
-        "ps": PsAttributesTypeDef,
-        "vsam": VsamAttributesTypeDef,
-    },
-    total=False,
-)
-
 DatasetDetailOrgAttributesTypeDef = TypedDict(
     "DatasetDetailOrgAttributesTypeDef",
     {
         "gdg": GdgDetailAttributesTypeDef,
         "po": PoDetailAttributesTypeDef,
         "ps": PsDetailAttributesTypeDef,
         "vsam": VsamDetailAttributesTypeDef,
     },
+)
+
+DatasetOrgAttributesTypeDef = TypedDict(
+    "DatasetOrgAttributesTypeDef",
+    {
+        "gdg": GdgAttributesTypeDef,
+        "po": PoAttributesTypeDef,
+        "ps": PsAttributesTypeDef,
+        "vsam": VsamAttributesTypeDef,
+    },
     total=False,
 )
 
 ListBatchJobExecutionsResponseTypeDef = TypedDict(
     "ListBatchJobExecutionsResponseTypeDef",
     {
         "batchJobExecutions": List[BatchJobExecutionSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetDataSetDetailsResponseTypeDef = TypedDict(
+    "GetDataSetDetailsResponseTypeDef",
+    {
+        "blocksize": int,
+        "creationTime": datetime,
+        "dataSetName": str,
+        "dataSetOrg": DatasetDetailOrgAttributesTypeDef,
+        "lastReferencedTime": datetime,
+        "lastUpdatedTime": datetime,
+        "location": str,
+        "recordLength": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredDataSetTypeDef = TypedDict(
     "_RequiredDataSetTypeDef",
     {
         "datasetName": str,
@@ -1610,29 +1610,14 @@
 )
 
 
 class DataSetTypeDef(_RequiredDataSetTypeDef, _OptionalDataSetTypeDef):
     pass
 
 
-GetDataSetDetailsResponseTypeDef = TypedDict(
-    "GetDataSetDetailsResponseTypeDef",
-    {
-        "blocksize": int,
-        "creationTime": datetime,
-        "dataSetName": str,
-        "dataSetOrg": DatasetDetailOrgAttributesTypeDef,
-        "lastReferencedTime": datetime,
-        "lastUpdatedTime": datetime,
-        "location": str,
-        "recordLength": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 DataSetImportItemTypeDef = TypedDict(
     "DataSetImportItemTypeDef",
     {
         "dataSet": DataSetTypeDef,
         "externalLocation": ExternalLocationTypeDef,
     },
 )
```

### Comparing `mypy-boto3-m2-1.28.16/mypy_boto3_m2/type_defs.pyi` & `mypy-boto3-m2-1.28.5/mypy_boto3_m2/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for m2 service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_m2.type_defs import AlternateKeyTypeDef
+    from mypy_boto3_m2.type_defs import AlternateKeyOutputTypeDef
 
-    data: AlternateKeyTypeDef = ...
+    data: AlternateKeyOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -29,26 +29,32 @@
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
+    "AlternateKeyOutputTypeDef",
     "AlternateKeyTypeDef",
     "ApplicationSummaryTypeDef",
     "ApplicationVersionSummaryTypeDef",
     "FileBatchJobDefinitionTypeDef",
     "ScriptBatchJobDefinitionTypeDef",
+    "FileBatchJobIdentifierOutputTypeDef",
+    "ScriptBatchJobIdentifierOutputTypeDef",
     "FileBatchJobIdentifierTypeDef",
     "ScriptBatchJobIdentifierTypeDef",
     "CancelBatchJobExecutionRequestRequestTypeDef",
     "DefinitionTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateApplicationResponseTypeDef",
+    "CreateDataSetImportTaskResponseTypeDef",
     "CreateDeploymentRequestRequestTypeDef",
+    "CreateDeploymentResponseTypeDef",
     "HighAvailabilityConfigTypeDef",
+    "CreateEnvironmentResponseTypeDef",
     "ExternalLocationTypeDef",
     "DataSetImportSummaryTypeDef",
     "DataSetSummaryTypeDef",
     "RecordLengthTypeDef",
     "GdgDetailAttributesTypeDef",
     "PoDetailAttributesTypeDef",
     "PsDetailAttributesTypeDef",
@@ -56,99 +62,111 @@
     "PoAttributesTypeDef",
     "PsAttributesTypeDef",
     "DeleteApplicationFromEnvironmentRequestRequestTypeDef",
     "DeleteApplicationRequestRequestTypeDef",
     "DeleteEnvironmentRequestRequestTypeDef",
     "DeployedVersionSummaryTypeDef",
     "DeploymentSummaryTypeDef",
+    "EfsStorageConfigurationOutputTypeDef",
     "EfsStorageConfigurationTypeDef",
     "EngineVersionsSummaryTypeDef",
     "EnvironmentSummaryTypeDef",
+    "FsxStorageConfigurationOutputTypeDef",
     "FsxStorageConfigurationTypeDef",
     "GetApplicationRequestRequestTypeDef",
     "LogGroupSummaryTypeDef",
     "GetApplicationVersionRequestRequestTypeDef",
+    "GetApplicationVersionResponseTypeDef",
     "GetBatchJobExecutionRequestRequestTypeDef",
     "GetDataSetDetailsRequestRequestTypeDef",
     "GetDataSetImportTaskRequestRequestTypeDef",
     "GetDeploymentRequestRequestTypeDef",
+    "GetDeploymentResponseTypeDef",
     "GetEnvironmentRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "HighAvailabilityConfigOutputTypeDef",
+    "GetSignedBluinsightsUrlResponseTypeDef",
+    "ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef",
     "ListApplicationVersionsRequestRequestTypeDef",
+    "ListApplicationsRequestListApplicationsPaginateTypeDef",
     "ListApplicationsRequestRequestTypeDef",
+    "ListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef",
     "ListBatchJobDefinitionsRequestRequestTypeDef",
-    "TimestampTypeDef",
+    "ListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef",
+    "ListBatchJobExecutionsRequestRequestTypeDef",
+    "ListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef",
     "ListDataSetImportHistoryRequestRequestTypeDef",
+    "ListDataSetsRequestListDataSetsPaginateTypeDef",
     "ListDataSetsRequestRequestTypeDef",
+    "ListDeploymentsRequestListDeploymentsPaginateTypeDef",
     "ListDeploymentsRequestRequestTypeDef",
+    "ListEngineVersionsRequestListEngineVersionsPaginateTypeDef",
     "ListEngineVersionsRequestRequestTypeDef",
+    "ListEnvironmentsRequestListEnvironmentsPaginateTypeDef",
     "ListEnvironmentsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "MaintenanceScheduleTypeDef",
+    "PaginatorConfigTypeDef",
+    "PrimaryKeyOutputTypeDef",
     "PrimaryKeyTypeDef",
+    "ResponseMetadataTypeDef",
     "StartApplicationRequestRequestTypeDef",
+    "StartBatchJobResponseTypeDef",
     "StopApplicationRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "UpdateApplicationResponseTypeDef",
     "UpdateEnvironmentRequestRequestTypeDef",
+    "UpdateEnvironmentResponseTypeDef",
+    "ListApplicationsResponseTypeDef",
+    "ListApplicationVersionsResponseTypeDef",
     "BatchJobDefinitionTypeDef",
+    "BatchJobIdentifierOutputTypeDef",
     "BatchJobIdentifierTypeDef",
     "CreateApplicationRequestRequestTypeDef",
     "UpdateApplicationRequestRequestTypeDef",
-    "CreateApplicationResponseTypeDef",
-    "CreateDataSetImportTaskResponseTypeDef",
-    "CreateDeploymentResponseTypeDef",
-    "CreateEnvironmentResponseTypeDef",
-    "GetApplicationVersionResponseTypeDef",
-    "GetDeploymentResponseTypeDef",
-    "GetSignedBluinsightsUrlResponseTypeDef",
-    "ListApplicationVersionsResponseTypeDef",
-    "ListApplicationsResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "StartBatchJobResponseTypeDef",
-    "UpdateApplicationResponseTypeDef",
-    "UpdateEnvironmentResponseTypeDef",
     "DataSetImportTaskTypeDef",
     "GetDataSetImportTaskResponseTypeDef",
     "ListDataSetsResponseTypeDef",
     "ListDeploymentsResponseTypeDef",
     "ListEngineVersionsResponseTypeDef",
     "ListEnvironmentsResponseTypeDef",
+    "StorageConfigurationOutputTypeDef",
     "StorageConfigurationTypeDef",
     "GetApplicationResponseTypeDef",
-    "ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef",
-    "ListApplicationsRequestListApplicationsPaginateTypeDef",
-    "ListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef",
-    "ListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef",
-    "ListDataSetsRequestListDataSetsPaginateTypeDef",
-    "ListDeploymentsRequestListDeploymentsPaginateTypeDef",
-    "ListEngineVersionsRequestListEngineVersionsPaginateTypeDef",
-    "ListEnvironmentsRequestListEnvironmentsPaginateTypeDef",
-    "ListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef",
-    "ListBatchJobExecutionsRequestRequestTypeDef",
     "PendingMaintenanceTypeDef",
-    "VsamAttributesTypeDef",
     "VsamDetailAttributesTypeDef",
+    "VsamAttributesTypeDef",
     "ListBatchJobDefinitionsResponseTypeDef",
     "BatchJobExecutionSummaryTypeDef",
     "GetBatchJobExecutionResponseTypeDef",
     "StartBatchJobRequestRequestTypeDef",
     "ListDataSetImportHistoryResponseTypeDef",
     "CreateEnvironmentRequestRequestTypeDef",
     "GetEnvironmentResponseTypeDef",
-    "DatasetOrgAttributesTypeDef",
     "DatasetDetailOrgAttributesTypeDef",
+    "DatasetOrgAttributesTypeDef",
     "ListBatchJobExecutionsResponseTypeDef",
-    "DataSetTypeDef",
     "GetDataSetDetailsResponseTypeDef",
+    "DataSetTypeDef",
     "DataSetImportItemTypeDef",
     "DataSetImportConfigTypeDef",
     "CreateDataSetImportTaskRequestRequestTypeDef",
 )
 
+AlternateKeyOutputTypeDef = TypedDict(
+    "AlternateKeyOutputTypeDef",
+    {
+        "allowDuplicates": bool,
+        "length": int,
+        "name": str,
+        "offset": int,
+    },
+)
+
 _RequiredAlternateKeyTypeDef = TypedDict(
     "_RequiredAlternateKeyTypeDef",
     {
         "length": int,
         "offset": int,
     },
 )
@@ -160,86 +178,68 @@
     },
     total=False,
 )
 
 class AlternateKeyTypeDef(_RequiredAlternateKeyTypeDef, _OptionalAlternateKeyTypeDef):
     pass
 
-_RequiredApplicationSummaryTypeDef = TypedDict(
-    "_RequiredApplicationSummaryTypeDef",
+ApplicationSummaryTypeDef = TypedDict(
+    "ApplicationSummaryTypeDef",
     {
         "applicationArn": str,
         "applicationId": str,
         "applicationVersion": int,
         "creationTime": datetime,
-        "engineType": EngineTypeType,
-        "name": str,
-        "status": ApplicationLifecycleType,
-    },
-)
-_OptionalApplicationSummaryTypeDef = TypedDict(
-    "_OptionalApplicationSummaryTypeDef",
-    {
         "deploymentStatus": ApplicationDeploymentLifecycleType,
         "description": str,
+        "engineType": EngineTypeType,
         "environmentId": str,
         "lastStartTime": datetime,
+        "name": str,
         "roleArn": str,
+        "status": ApplicationLifecycleType,
         "versionStatus": ApplicationVersionLifecycleType,
     },
-    total=False,
 )
 
-class ApplicationSummaryTypeDef(
-    _RequiredApplicationSummaryTypeDef, _OptionalApplicationSummaryTypeDef
-):
-    pass
-
-_RequiredApplicationVersionSummaryTypeDef = TypedDict(
-    "_RequiredApplicationVersionSummaryTypeDef",
+ApplicationVersionSummaryTypeDef = TypedDict(
+    "ApplicationVersionSummaryTypeDef",
     {
         "applicationVersion": int,
         "creationTime": datetime,
         "status": ApplicationVersionLifecycleType,
+        "statusReason": str,
     },
 )
-_OptionalApplicationVersionSummaryTypeDef = TypedDict(
-    "_OptionalApplicationVersionSummaryTypeDef",
+
+FileBatchJobDefinitionTypeDef = TypedDict(
+    "FileBatchJobDefinitionTypeDef",
     {
-        "statusReason": str,
+        "fileName": str,
+        "folderPath": str,
     },
-    total=False,
 )
 
-class ApplicationVersionSummaryTypeDef(
-    _RequiredApplicationVersionSummaryTypeDef, _OptionalApplicationVersionSummaryTypeDef
-):
-    pass
-
-_RequiredFileBatchJobDefinitionTypeDef = TypedDict(
-    "_RequiredFileBatchJobDefinitionTypeDef",
+ScriptBatchJobDefinitionTypeDef = TypedDict(
+    "ScriptBatchJobDefinitionTypeDef",
     {
-        "fileName": str,
+        "scriptName": str,
     },
 )
-_OptionalFileBatchJobDefinitionTypeDef = TypedDict(
-    "_OptionalFileBatchJobDefinitionTypeDef",
+
+FileBatchJobIdentifierOutputTypeDef = TypedDict(
+    "FileBatchJobIdentifierOutputTypeDef",
     {
+        "fileName": str,
         "folderPath": str,
     },
-    total=False,
 )
 
-class FileBatchJobDefinitionTypeDef(
-    _RequiredFileBatchJobDefinitionTypeDef, _OptionalFileBatchJobDefinitionTypeDef
-):
-    pass
-
-ScriptBatchJobDefinitionTypeDef = TypedDict(
-    "ScriptBatchJobDefinitionTypeDef",
+ScriptBatchJobIdentifierOutputTypeDef = TypedDict(
+    "ScriptBatchJobIdentifierOutputTypeDef",
     {
         "scriptName": str,
     },
 )
 
 _RequiredFileBatchJobIdentifierTypeDef = TypedDict(
     "_RequiredFileBatchJobIdentifierTypeDef",
@@ -280,22 +280,29 @@
     {
         "content": str,
         "s3Location": str,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateApplicationResponseTypeDef = TypedDict(
+    "CreateApplicationResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "applicationArn": str,
+        "applicationId": str,
+        "applicationVersion": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateDataSetImportTaskResponseTypeDef = TypedDict(
+    "CreateDataSetImportTaskResponseTypeDef",
+    {
+        "taskId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateDeploymentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDeploymentRequestRequestTypeDef",
     {
         "applicationId": str,
@@ -312,21 +319,37 @@
 )
 
 class CreateDeploymentRequestRequestTypeDef(
     _RequiredCreateDeploymentRequestRequestTypeDef, _OptionalCreateDeploymentRequestRequestTypeDef
 ):
     pass
 
+CreateDeploymentResponseTypeDef = TypedDict(
+    "CreateDeploymentResponseTypeDef",
+    {
+        "deploymentId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 HighAvailabilityConfigTypeDef = TypedDict(
     "HighAvailabilityConfigTypeDef",
     {
         "desiredCapacity": int,
     },
 )
 
+CreateEnvironmentResponseTypeDef = TypedDict(
+    "CreateEnvironmentResponseTypeDef",
+    {
+        "environmentId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ExternalLocationTypeDef = TypedDict(
     "ExternalLocationTypeDef",
     {
         "s3Location": str,
     },
     total=False,
 )
@@ -338,50 +361,40 @@
         "inProgress": int,
         "pending": int,
         "succeeded": int,
         "total": int,
     },
 )
 
-_RequiredDataSetSummaryTypeDef = TypedDict(
-    "_RequiredDataSetSummaryTypeDef",
-    {
-        "dataSetName": str,
-    },
-)
-_OptionalDataSetSummaryTypeDef = TypedDict(
-    "_OptionalDataSetSummaryTypeDef",
+DataSetSummaryTypeDef = TypedDict(
+    "DataSetSummaryTypeDef",
     {
         "creationTime": datetime,
+        "dataSetName": str,
         "dataSetOrg": str,
         "format": str,
         "lastReferencedTime": datetime,
         "lastUpdatedTime": datetime,
     },
-    total=False,
 )
 
-class DataSetSummaryTypeDef(_RequiredDataSetSummaryTypeDef, _OptionalDataSetSummaryTypeDef):
-    pass
-
 RecordLengthTypeDef = TypedDict(
     "RecordLengthTypeDef",
     {
         "max": int,
         "min": int,
     },
 )
 
 GdgDetailAttributesTypeDef = TypedDict(
     "GdgDetailAttributesTypeDef",
     {
         "limit": int,
         "rollDisposition": str,
     },
-    total=False,
 )
 
 PoDetailAttributesTypeDef = TypedDict(
     "PoDetailAttributesTypeDef",
     {
         "encoding": str,
         "format": str,
@@ -458,58 +471,44 @@
 DeleteEnvironmentRequestRequestTypeDef = TypedDict(
     "DeleteEnvironmentRequestRequestTypeDef",
     {
         "environmentId": str,
     },
 )
 
-_RequiredDeployedVersionSummaryTypeDef = TypedDict(
-    "_RequiredDeployedVersionSummaryTypeDef",
+DeployedVersionSummaryTypeDef = TypedDict(
+    "DeployedVersionSummaryTypeDef",
     {
         "applicationVersion": int,
         "status": DeploymentLifecycleType,
-    },
-)
-_OptionalDeployedVersionSummaryTypeDef = TypedDict(
-    "_OptionalDeployedVersionSummaryTypeDef",
-    {
         "statusReason": str,
     },
-    total=False,
 )
 
-class DeployedVersionSummaryTypeDef(
-    _RequiredDeployedVersionSummaryTypeDef, _OptionalDeployedVersionSummaryTypeDef
-):
-    pass
-
-_RequiredDeploymentSummaryTypeDef = TypedDict(
-    "_RequiredDeploymentSummaryTypeDef",
+DeploymentSummaryTypeDef = TypedDict(
+    "DeploymentSummaryTypeDef",
     {
         "applicationId": str,
         "applicationVersion": int,
         "creationTime": datetime,
         "deploymentId": str,
         "environmentId": str,
         "status": DeploymentLifecycleType,
+        "statusReason": str,
     },
 )
-_OptionalDeploymentSummaryTypeDef = TypedDict(
-    "_OptionalDeploymentSummaryTypeDef",
+
+EfsStorageConfigurationOutputTypeDef = TypedDict(
+    "EfsStorageConfigurationOutputTypeDef",
     {
-        "statusReason": str,
+        "fileSystemId": str,
+        "mountPoint": str,
     },
-    total=False,
 )
 
-class DeploymentSummaryTypeDef(
-    _RequiredDeploymentSummaryTypeDef, _OptionalDeploymentSummaryTypeDef
-):
-    pass
-
 EfsStorageConfigurationTypeDef = TypedDict(
     "EfsStorageConfigurationTypeDef",
     {
         "fileSystemId": str,
         "mountPoint": str,
     },
 )
@@ -532,14 +531,22 @@
         "environmentId": str,
         "instanceType": str,
         "name": str,
         "status": EnvironmentLifecycleType,
     },
 )
 
+FsxStorageConfigurationOutputTypeDef = TypedDict(
+    "FsxStorageConfigurationOutputTypeDef",
+    {
+        "fileSystemId": str,
+        "mountPoint": str,
+    },
+)
+
 FsxStorageConfigurationTypeDef = TypedDict(
     "FsxStorageConfigurationTypeDef",
     {
         "fileSystemId": str,
         "mountPoint": str,
     },
 )
@@ -563,14 +570,28 @@
     "GetApplicationVersionRequestRequestTypeDef",
     {
         "applicationId": str,
         "applicationVersion": int,
     },
 )
 
+GetApplicationVersionResponseTypeDef = TypedDict(
+    "GetApplicationVersionResponseTypeDef",
+    {
+        "applicationVersion": int,
+        "creationTime": datetime,
+        "definitionContent": str,
+        "description": str,
+        "name": str,
+        "status": ApplicationVersionLifecycleType,
+        "statusReason": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetBatchJobExecutionRequestRequestTypeDef = TypedDict(
     "GetBatchJobExecutionRequestRequestTypeDef",
     {
         "applicationId": str,
         "executionId": str,
     },
 )
@@ -595,31 +616,70 @@
     "GetDeploymentRequestRequestTypeDef",
     {
         "applicationId": str,
         "deploymentId": str,
     },
 )
 
+GetDeploymentResponseTypeDef = TypedDict(
+    "GetDeploymentResponseTypeDef",
+    {
+        "applicationId": str,
+        "applicationVersion": int,
+        "creationTime": datetime,
+        "deploymentId": str,
+        "environmentId": str,
+        "status": DeploymentLifecycleType,
+        "statusReason": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetEnvironmentRequestRequestTypeDef = TypedDict(
     "GetEnvironmentRequestRequestTypeDef",
     {
         "environmentId": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+HighAvailabilityConfigOutputTypeDef = TypedDict(
+    "HighAvailabilityConfigOutputTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "desiredCapacity": int,
+    },
+)
+
+GetSignedBluinsightsUrlResponseTypeDef = TypedDict(
+    "GetSignedBluinsightsUrlResponseTypeDef",
+    {
+        "signedBiUrl": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef",
+    {
+        "applicationId": str,
+    },
+)
+_OptionalListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+class ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef(
+    _RequiredListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef,
+    _OptionalListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef,
+):
+    pass
+
 _RequiredListApplicationVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListApplicationVersionsRequestRequestTypeDef",
     {
         "applicationId": str,
     },
 )
 _OptionalListApplicationVersionsRequestRequestTypeDef = TypedDict(
@@ -633,25 +693,56 @@
 
 class ListApplicationVersionsRequestRequestTypeDef(
     _RequiredListApplicationVersionsRequestRequestTypeDef,
     _OptionalListApplicationVersionsRequestRequestTypeDef,
 ):
     pass
 
+ListApplicationsRequestListApplicationsPaginateTypeDef = TypedDict(
+    "ListApplicationsRequestListApplicationsPaginateTypeDef",
+    {
+        "environmentId": str,
+        "names": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListApplicationsRequestRequestTypeDef = TypedDict(
     "ListApplicationsRequestRequestTypeDef",
     {
         "environmentId": str,
         "maxResults": int,
         "names": Sequence[str],
         "nextToken": str,
     },
     total=False,
 )
 
+_RequiredListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef = TypedDict(
+    "_RequiredListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef",
+    {
+        "applicationId": str,
+    },
+)
+_OptionalListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef = TypedDict(
+    "_OptionalListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef",
+    {
+        "prefix": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef(
+    _RequiredListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef,
+    _OptionalListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef,
+):
+    pass
+
 _RequiredListBatchJobDefinitionsRequestRequestTypeDef = TypedDict(
     "_RequiredListBatchJobDefinitionsRequestRequestTypeDef",
     {
         "applicationId": str,
     },
 )
 _OptionalListBatchJobDefinitionsRequestRequestTypeDef = TypedDict(
@@ -666,15 +757,85 @@
 
 class ListBatchJobDefinitionsRequestRequestTypeDef(
     _RequiredListBatchJobDefinitionsRequestRequestTypeDef,
     _OptionalListBatchJobDefinitionsRequestRequestTypeDef,
 ):
     pass
 
-TimestampTypeDef = Union[datetime, str]
+_RequiredListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef = TypedDict(
+    "_RequiredListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef",
+    {
+        "applicationId": str,
+    },
+)
+_OptionalListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef = TypedDict(
+    "_OptionalListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef",
+    {
+        "executionIds": Sequence[str],
+        "jobName": str,
+        "startedAfter": Union[datetime, str],
+        "startedBefore": Union[datetime, str],
+        "status": BatchJobExecutionStatusType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef(
+    _RequiredListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef,
+    _OptionalListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef,
+):
+    pass
+
+_RequiredListBatchJobExecutionsRequestRequestTypeDef = TypedDict(
+    "_RequiredListBatchJobExecutionsRequestRequestTypeDef",
+    {
+        "applicationId": str,
+    },
+)
+_OptionalListBatchJobExecutionsRequestRequestTypeDef = TypedDict(
+    "_OptionalListBatchJobExecutionsRequestRequestTypeDef",
+    {
+        "executionIds": Sequence[str],
+        "jobName": str,
+        "maxResults": int,
+        "nextToken": str,
+        "startedAfter": Union[datetime, str],
+        "startedBefore": Union[datetime, str],
+        "status": BatchJobExecutionStatusType,
+    },
+    total=False,
+)
+
+class ListBatchJobExecutionsRequestRequestTypeDef(
+    _RequiredListBatchJobExecutionsRequestRequestTypeDef,
+    _OptionalListBatchJobExecutionsRequestRequestTypeDef,
+):
+    pass
+
+_RequiredListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef = TypedDict(
+    "_RequiredListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef",
+    {
+        "applicationId": str,
+    },
+)
+_OptionalListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef = TypedDict(
+    "_OptionalListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef(
+    _RequiredListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef,
+    _OptionalListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef,
+):
+    pass
+
 _RequiredListDataSetImportHistoryRequestRequestTypeDef = TypedDict(
     "_RequiredListDataSetImportHistoryRequestRequestTypeDef",
     {
         "applicationId": str,
     },
 )
 _OptionalListDataSetImportHistoryRequestRequestTypeDef = TypedDict(
@@ -688,14 +849,35 @@
 
 class ListDataSetImportHistoryRequestRequestTypeDef(
     _RequiredListDataSetImportHistoryRequestRequestTypeDef,
     _OptionalListDataSetImportHistoryRequestRequestTypeDef,
 ):
     pass
 
+_RequiredListDataSetsRequestListDataSetsPaginateTypeDef = TypedDict(
+    "_RequiredListDataSetsRequestListDataSetsPaginateTypeDef",
+    {
+        "applicationId": str,
+    },
+)
+_OptionalListDataSetsRequestListDataSetsPaginateTypeDef = TypedDict(
+    "_OptionalListDataSetsRequestListDataSetsPaginateTypeDef",
+    {
+        "prefix": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListDataSetsRequestListDataSetsPaginateTypeDef(
+    _RequiredListDataSetsRequestListDataSetsPaginateTypeDef,
+    _OptionalListDataSetsRequestListDataSetsPaginateTypeDef,
+):
+    pass
+
 _RequiredListDataSetsRequestRequestTypeDef = TypedDict(
     "_RequiredListDataSetsRequestRequestTypeDef",
     {
         "applicationId": str,
     },
 )
 _OptionalListDataSetsRequestRequestTypeDef = TypedDict(
@@ -709,14 +891,34 @@
 )
 
 class ListDataSetsRequestRequestTypeDef(
     _RequiredListDataSetsRequestRequestTypeDef, _OptionalListDataSetsRequestRequestTypeDef
 ):
     pass
 
+_RequiredListDeploymentsRequestListDeploymentsPaginateTypeDef = TypedDict(
+    "_RequiredListDeploymentsRequestListDeploymentsPaginateTypeDef",
+    {
+        "applicationId": str,
+    },
+)
+_OptionalListDeploymentsRequestListDeploymentsPaginateTypeDef = TypedDict(
+    "_OptionalListDeploymentsRequestListDeploymentsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListDeploymentsRequestListDeploymentsPaginateTypeDef(
+    _RequiredListDeploymentsRequestListDeploymentsPaginateTypeDef,
+    _OptionalListDeploymentsRequestListDeploymentsPaginateTypeDef,
+):
+    pass
+
 _RequiredListDeploymentsRequestRequestTypeDef = TypedDict(
     "_RequiredListDeploymentsRequestRequestTypeDef",
     {
         "applicationId": str,
     },
 )
 _OptionalListDeploymentsRequestRequestTypeDef = TypedDict(
@@ -729,24 +931,43 @@
 )
 
 class ListDeploymentsRequestRequestTypeDef(
     _RequiredListDeploymentsRequestRequestTypeDef, _OptionalListDeploymentsRequestRequestTypeDef
 ):
     pass
 
+ListEngineVersionsRequestListEngineVersionsPaginateTypeDef = TypedDict(
+    "ListEngineVersionsRequestListEngineVersionsPaginateTypeDef",
+    {
+        "engineType": EngineTypeType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListEngineVersionsRequestRequestTypeDef = TypedDict(
     "ListEngineVersionsRequestRequestTypeDef",
     {
         "engineType": EngineTypeType,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+ListEnvironmentsRequestListEnvironmentsPaginateTypeDef = TypedDict(
+    "ListEnvironmentsRequestListEnvironmentsPaginateTypeDef",
+    {
+        "engineType": EngineTypeType,
+        "names": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListEnvironmentsRequestRequestTypeDef = TypedDict(
     "ListEnvironmentsRequestRequestTypeDef",
     {
         "engineType": EngineTypeType,
         "maxResults": int,
         "names": Sequence[str],
         "nextToken": str,
@@ -757,23 +978,49 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 MaintenanceScheduleTypeDef = TypedDict(
     "MaintenanceScheduleTypeDef",
     {
         "endTime": datetime,
         "startTime": datetime,
     },
+)
+
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
+    {
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
+    },
     total=False,
 )
 
+PrimaryKeyOutputTypeDef = TypedDict(
+    "PrimaryKeyOutputTypeDef",
+    {
+        "length": int,
+        "name": str,
+        "offset": int,
+    },
+)
+
 _RequiredPrimaryKeyTypeDef = TypedDict(
     "_RequiredPrimaryKeyTypeDef",
     {
         "length": int,
         "offset": int,
     },
 )
@@ -784,21 +1031,40 @@
     },
     total=False,
 )
 
 class PrimaryKeyTypeDef(_RequiredPrimaryKeyTypeDef, _OptionalPrimaryKeyTypeDef):
     pass
 
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
+    {
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
 StartApplicationRequestRequestTypeDef = TypedDict(
     "StartApplicationRequestRequestTypeDef",
     {
         "applicationId": str,
     },
 )
 
+StartBatchJobResponseTypeDef = TypedDict(
+    "StartBatchJobResponseTypeDef",
+    {
+        "executionId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredStopApplicationRequestRequestTypeDef = TypedDict(
     "_RequiredStopApplicationRequestRequestTypeDef",
     {
         "applicationId": str,
     },
 )
 _OptionalStopApplicationRequestRequestTypeDef = TypedDict(
@@ -826,14 +1092,22 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
+UpdateApplicationResponseTypeDef = TypedDict(
+    "UpdateApplicationResponseTypeDef",
+    {
+        "applicationVersion": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredUpdateEnvironmentRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateEnvironmentRequestRequestTypeDef",
     {
         "environmentId": str,
     },
 )
 _OptionalUpdateEnvironmentRequestRequestTypeDef = TypedDict(
@@ -849,21 +1123,54 @@
 )
 
 class UpdateEnvironmentRequestRequestTypeDef(
     _RequiredUpdateEnvironmentRequestRequestTypeDef, _OptionalUpdateEnvironmentRequestRequestTypeDef
 ):
     pass
 
+UpdateEnvironmentResponseTypeDef = TypedDict(
+    "UpdateEnvironmentResponseTypeDef",
+    {
+        "environmentId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListApplicationsResponseTypeDef = TypedDict(
+    "ListApplicationsResponseTypeDef",
+    {
+        "applications": List[ApplicationSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListApplicationVersionsResponseTypeDef = TypedDict(
+    "ListApplicationVersionsResponseTypeDef",
+    {
+        "applicationVersions": List[ApplicationVersionSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 BatchJobDefinitionTypeDef = TypedDict(
     "BatchJobDefinitionTypeDef",
     {
         "fileBatchJobDefinition": FileBatchJobDefinitionTypeDef,
         "scriptBatchJobDefinition": ScriptBatchJobDefinitionTypeDef,
     },
-    total=False,
+)
+
+BatchJobIdentifierOutputTypeDef = TypedDict(
+    "BatchJobIdentifierOutputTypeDef",
+    {
+        "fileBatchJobIdentifier": FileBatchJobIdentifierOutputTypeDef,
+        "scriptBatchJobIdentifier": ScriptBatchJobIdentifierOutputTypeDef,
+    },
 )
 
 BatchJobIdentifierTypeDef = TypedDict(
     "BatchJobIdentifierTypeDef",
     {
         "fileBatchJobIdentifier": FileBatchJobIdentifierTypeDef,
         "scriptBatchJobIdentifier": ScriptBatchJobIdentifierTypeDef,
@@ -913,134 +1220,14 @@
 )
 
 class UpdateApplicationRequestRequestTypeDef(
     _RequiredUpdateApplicationRequestRequestTypeDef, _OptionalUpdateApplicationRequestRequestTypeDef
 ):
     pass
 
-CreateApplicationResponseTypeDef = TypedDict(
-    "CreateApplicationResponseTypeDef",
-    {
-        "applicationArn": str,
-        "applicationId": str,
-        "applicationVersion": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateDataSetImportTaskResponseTypeDef = TypedDict(
-    "CreateDataSetImportTaskResponseTypeDef",
-    {
-        "taskId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateDeploymentResponseTypeDef = TypedDict(
-    "CreateDeploymentResponseTypeDef",
-    {
-        "deploymentId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateEnvironmentResponseTypeDef = TypedDict(
-    "CreateEnvironmentResponseTypeDef",
-    {
-        "environmentId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetApplicationVersionResponseTypeDef = TypedDict(
-    "GetApplicationVersionResponseTypeDef",
-    {
-        "applicationVersion": int,
-        "creationTime": datetime,
-        "definitionContent": str,
-        "description": str,
-        "name": str,
-        "status": ApplicationVersionLifecycleType,
-        "statusReason": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetDeploymentResponseTypeDef = TypedDict(
-    "GetDeploymentResponseTypeDef",
-    {
-        "applicationId": str,
-        "applicationVersion": int,
-        "creationTime": datetime,
-        "deploymentId": str,
-        "environmentId": str,
-        "status": DeploymentLifecycleType,
-        "statusReason": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetSignedBluinsightsUrlResponseTypeDef = TypedDict(
-    "GetSignedBluinsightsUrlResponseTypeDef",
-    {
-        "signedBiUrl": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListApplicationVersionsResponseTypeDef = TypedDict(
-    "ListApplicationVersionsResponseTypeDef",
-    {
-        "applicationVersions": List[ApplicationVersionSummaryTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListApplicationsResponseTypeDef = TypedDict(
-    "ListApplicationsResponseTypeDef",
-    {
-        "applications": List[ApplicationSummaryTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartBatchJobResponseTypeDef = TypedDict(
-    "StartBatchJobResponseTypeDef",
-    {
-        "executionId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateApplicationResponseTypeDef = TypedDict(
-    "UpdateApplicationResponseTypeDef",
-    {
-        "applicationVersion": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateEnvironmentResponseTypeDef = TypedDict(
-    "UpdateEnvironmentResponseTypeDef",
-    {
-        "environmentId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 DataSetImportTaskTypeDef = TypedDict(
     "DataSetImportTaskTypeDef",
     {
         "status": DataSetTaskLifecycleType,
         "summary": DataSetImportSummaryTypeDef,
         "taskId": str,
     },
@@ -1048,51 +1235,59 @@
 
 GetDataSetImportTaskResponseTypeDef = TypedDict(
     "GetDataSetImportTaskResponseTypeDef",
     {
         "status": DataSetTaskLifecycleType,
         "summary": DataSetImportSummaryTypeDef,
         "taskId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDataSetsResponseTypeDef = TypedDict(
     "ListDataSetsResponseTypeDef",
     {
         "dataSets": List[DataSetSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDeploymentsResponseTypeDef = TypedDict(
     "ListDeploymentsResponseTypeDef",
     {
         "deployments": List[DeploymentSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListEngineVersionsResponseTypeDef = TypedDict(
     "ListEngineVersionsResponseTypeDef",
     {
         "engineVersions": List[EngineVersionsSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListEnvironmentsResponseTypeDef = TypedDict(
     "ListEnvironmentsResponseTypeDef",
     {
         "environments": List[EnvironmentSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+StorageConfigurationOutputTypeDef = TypedDict(
+    "StorageConfigurationOutputTypeDef",
+    {
+        "efs": EfsStorageConfigurationOutputTypeDef,
+        "fsx": FsxStorageConfigurationOutputTypeDef,
     },
 )
 
 StorageConfigurationTypeDef = TypedDict(
     "StorageConfigurationTypeDef",
     {
         "efs": EfsStorageConfigurationTypeDef,
@@ -1120,207 +1315,36 @@
         "logGroups": List[LogGroupSummaryTypeDef],
         "name": str,
         "roleArn": str,
         "status": ApplicationLifecycleType,
         "statusReason": str,
         "tags": Dict[str, str],
         "targetGroupArns": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef",
-    {
-        "applicationId": str,
-    },
-)
-_OptionalListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef(
-    _RequiredListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef,
-    _OptionalListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef,
-):
-    pass
-
-ListApplicationsRequestListApplicationsPaginateTypeDef = TypedDict(
-    "ListApplicationsRequestListApplicationsPaginateTypeDef",
-    {
-        "environmentId": str,
-        "names": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef = TypedDict(
-    "_RequiredListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef",
-    {
-        "applicationId": str,
-    },
-)
-_OptionalListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef = TypedDict(
-    "_OptionalListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef",
-    {
-        "prefix": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef(
-    _RequiredListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef,
-    _OptionalListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef,
-):
-    pass
-
-_RequiredListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef = TypedDict(
-    "_RequiredListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef",
-    {
-        "applicationId": str,
-    },
-)
-_OptionalListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef = TypedDict(
-    "_OptionalListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef(
-    _RequiredListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef,
-    _OptionalListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef,
-):
-    pass
-
-_RequiredListDataSetsRequestListDataSetsPaginateTypeDef = TypedDict(
-    "_RequiredListDataSetsRequestListDataSetsPaginateTypeDef",
-    {
-        "applicationId": str,
-    },
-)
-_OptionalListDataSetsRequestListDataSetsPaginateTypeDef = TypedDict(
-    "_OptionalListDataSetsRequestListDataSetsPaginateTypeDef",
-    {
-        "prefix": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListDataSetsRequestListDataSetsPaginateTypeDef(
-    _RequiredListDataSetsRequestListDataSetsPaginateTypeDef,
-    _OptionalListDataSetsRequestListDataSetsPaginateTypeDef,
-):
-    pass
-
-_RequiredListDeploymentsRequestListDeploymentsPaginateTypeDef = TypedDict(
-    "_RequiredListDeploymentsRequestListDeploymentsPaginateTypeDef",
-    {
-        "applicationId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
-_OptionalListDeploymentsRequestListDeploymentsPaginateTypeDef = TypedDict(
-    "_OptionalListDeploymentsRequestListDeploymentsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListDeploymentsRequestListDeploymentsPaginateTypeDef(
-    _RequiredListDeploymentsRequestListDeploymentsPaginateTypeDef,
-    _OptionalListDeploymentsRequestListDeploymentsPaginateTypeDef,
-):
-    pass
-
-ListEngineVersionsRequestListEngineVersionsPaginateTypeDef = TypedDict(
-    "ListEngineVersionsRequestListEngineVersionsPaginateTypeDef",
-    {
-        "engineType": EngineTypeType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListEnvironmentsRequestListEnvironmentsPaginateTypeDef = TypedDict(
-    "ListEnvironmentsRequestListEnvironmentsPaginateTypeDef",
-    {
-        "engineType": EngineTypeType,
-        "names": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef = TypedDict(
-    "_RequiredListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef",
-    {
-        "applicationId": str,
-    },
-)
-_OptionalListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef = TypedDict(
-    "_OptionalListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef",
-    {
-        "executionIds": Sequence[str],
-        "jobName": str,
-        "startedAfter": TimestampTypeDef,
-        "startedBefore": TimestampTypeDef,
-        "status": BatchJobExecutionStatusType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef(
-    _RequiredListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef,
-    _OptionalListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef,
-):
-    pass
-
-_RequiredListBatchJobExecutionsRequestRequestTypeDef = TypedDict(
-    "_RequiredListBatchJobExecutionsRequestRequestTypeDef",
-    {
-        "applicationId": str,
-    },
-)
-_OptionalListBatchJobExecutionsRequestRequestTypeDef = TypedDict(
-    "_OptionalListBatchJobExecutionsRequestRequestTypeDef",
-    {
-        "executionIds": Sequence[str],
-        "jobName": str,
-        "maxResults": int,
-        "nextToken": str,
-        "startedAfter": TimestampTypeDef,
-        "startedBefore": TimestampTypeDef,
-        "status": BatchJobExecutionStatusType,
-    },
-    total=False,
-)
-
-class ListBatchJobExecutionsRequestRequestTypeDef(
-    _RequiredListBatchJobExecutionsRequestRequestTypeDef,
-    _OptionalListBatchJobExecutionsRequestRequestTypeDef,
-):
-    pass
 
 PendingMaintenanceTypeDef = TypedDict(
     "PendingMaintenanceTypeDef",
     {
         "engineVersion": str,
         "schedule": MaintenanceScheduleTypeDef,
     },
-    total=False,
+)
+
+VsamDetailAttributesTypeDef = TypedDict(
+    "VsamDetailAttributesTypeDef",
+    {
+        "alternateKeys": List[AlternateKeyOutputTypeDef],
+        "cacheAtStartup": bool,
+        "compressed": bool,
+        "encoding": str,
+        "primaryKey": PrimaryKeyOutputTypeDef,
+        "recordFormat": str,
+    },
 )
 
 _RequiredVsamAttributesTypeDef = TypedDict(
     "_RequiredVsamAttributesTypeDef",
     {
         "format": str,
     },
@@ -1335,79 +1359,55 @@
     },
     total=False,
 )
 
 class VsamAttributesTypeDef(_RequiredVsamAttributesTypeDef, _OptionalVsamAttributesTypeDef):
     pass
 
-VsamDetailAttributesTypeDef = TypedDict(
-    "VsamDetailAttributesTypeDef",
-    {
-        "alternateKeys": List[AlternateKeyTypeDef],
-        "cacheAtStartup": bool,
-        "compressed": bool,
-        "encoding": str,
-        "primaryKey": PrimaryKeyTypeDef,
-        "recordFormat": str,
-    },
-    total=False,
-)
-
 ListBatchJobDefinitionsResponseTypeDef = TypedDict(
     "ListBatchJobDefinitionsResponseTypeDef",
     {
         "batchJobDefinitions": List[BatchJobDefinitionTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredBatchJobExecutionSummaryTypeDef = TypedDict(
-    "_RequiredBatchJobExecutionSummaryTypeDef",
+BatchJobExecutionSummaryTypeDef = TypedDict(
+    "BatchJobExecutionSummaryTypeDef",
     {
         "applicationId": str,
-        "executionId": str,
-        "startTime": datetime,
-        "status": BatchJobExecutionStatusType,
-    },
-)
-_OptionalBatchJobExecutionSummaryTypeDef = TypedDict(
-    "_OptionalBatchJobExecutionSummaryTypeDef",
-    {
-        "batchJobIdentifier": BatchJobIdentifierTypeDef,
+        "batchJobIdentifier": BatchJobIdentifierOutputTypeDef,
         "endTime": datetime,
+        "executionId": str,
         "jobId": str,
         "jobName": str,
         "jobType": BatchJobTypeType,
         "returnCode": str,
+        "startTime": datetime,
+        "status": BatchJobExecutionStatusType,
     },
-    total=False,
 )
 
-class BatchJobExecutionSummaryTypeDef(
-    _RequiredBatchJobExecutionSummaryTypeDef, _OptionalBatchJobExecutionSummaryTypeDef
-):
-    pass
-
 GetBatchJobExecutionResponseTypeDef = TypedDict(
     "GetBatchJobExecutionResponseTypeDef",
     {
         "applicationId": str,
-        "batchJobIdentifier": BatchJobIdentifierTypeDef,
+        "batchJobIdentifier": BatchJobIdentifierOutputTypeDef,
         "endTime": datetime,
         "executionId": str,
         "jobId": str,
         "jobName": str,
         "jobType": BatchJobTypeType,
         "jobUser": str,
         "returnCode": str,
         "startTime": datetime,
         "status": BatchJobExecutionStatusType,
         "statusReason": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredStartBatchJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartBatchJobRequestRequestTypeDef",
     {
         "applicationId": str,
@@ -1428,15 +1428,15 @@
     pass
 
 ListDataSetImportHistoryResponseTypeDef = TypedDict(
     "ListDataSetImportHistoryResponseTypeDef",
     {
         "dataSetImportTasks": List[DataSetImportTaskTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateEnvironmentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateEnvironmentRequestRequestTypeDef",
     {
         "engineType": EngineTypeType,
@@ -1473,61 +1473,75 @@
         "actualCapacity": int,
         "creationTime": datetime,
         "description": str,
         "engineType": EngineTypeType,
         "engineVersion": str,
         "environmentArn": str,
         "environmentId": str,
-        "highAvailabilityConfig": HighAvailabilityConfigTypeDef,
+        "highAvailabilityConfig": HighAvailabilityConfigOutputTypeDef,
         "instanceType": str,
         "kmsKeyId": str,
         "loadBalancerArn": str,
         "name": str,
         "pendingMaintenance": PendingMaintenanceTypeDef,
         "preferredMaintenanceWindow": str,
         "publiclyAccessible": bool,
         "securityGroupIds": List[str],
         "status": EnvironmentLifecycleType,
         "statusReason": str,
-        "storageConfigurations": List[StorageConfigurationTypeDef],
+        "storageConfigurations": List[StorageConfigurationOutputTypeDef],
         "subnetIds": List[str],
         "tags": Dict[str, str],
         "vpcId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DatasetOrgAttributesTypeDef = TypedDict(
-    "DatasetOrgAttributesTypeDef",
-    {
-        "gdg": GdgAttributesTypeDef,
-        "po": PoAttributesTypeDef,
-        "ps": PsAttributesTypeDef,
-        "vsam": VsamAttributesTypeDef,
-    },
-    total=False,
-)
-
 DatasetDetailOrgAttributesTypeDef = TypedDict(
     "DatasetDetailOrgAttributesTypeDef",
     {
         "gdg": GdgDetailAttributesTypeDef,
         "po": PoDetailAttributesTypeDef,
         "ps": PsDetailAttributesTypeDef,
         "vsam": VsamDetailAttributesTypeDef,
     },
+)
+
+DatasetOrgAttributesTypeDef = TypedDict(
+    "DatasetOrgAttributesTypeDef",
+    {
+        "gdg": GdgAttributesTypeDef,
+        "po": PoAttributesTypeDef,
+        "ps": PsAttributesTypeDef,
+        "vsam": VsamAttributesTypeDef,
+    },
     total=False,
 )
 
 ListBatchJobExecutionsResponseTypeDef = TypedDict(
     "ListBatchJobExecutionsResponseTypeDef",
     {
         "batchJobExecutions": List[BatchJobExecutionSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetDataSetDetailsResponseTypeDef = TypedDict(
+    "GetDataSetDetailsResponseTypeDef",
+    {
+        "blocksize": int,
+        "creationTime": datetime,
+        "dataSetName": str,
+        "dataSetOrg": DatasetDetailOrgAttributesTypeDef,
+        "lastReferencedTime": datetime,
+        "lastUpdatedTime": datetime,
+        "location": str,
+        "recordLength": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredDataSetTypeDef = TypedDict(
     "_RequiredDataSetTypeDef",
     {
         "datasetName": str,
@@ -1543,29 +1557,14 @@
     },
     total=False,
 )
 
 class DataSetTypeDef(_RequiredDataSetTypeDef, _OptionalDataSetTypeDef):
     pass
 
-GetDataSetDetailsResponseTypeDef = TypedDict(
-    "GetDataSetDetailsResponseTypeDef",
-    {
-        "blocksize": int,
-        "creationTime": datetime,
-        "dataSetName": str,
-        "dataSetOrg": DatasetDetailOrgAttributesTypeDef,
-        "lastReferencedTime": datetime,
-        "lastUpdatedTime": datetime,
-        "location": str,
-        "recordLength": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 DataSetImportItemTypeDef = TypedDict(
     "DataSetImportItemTypeDef",
     {
         "dataSet": DataSetTypeDef,
         "externalLocation": ExternalLocationTypeDef,
     },
 )
```

### Comparing `mypy-boto3-m2-1.28.16/mypy_boto3_m2.egg-info/PKG-INFO` & `mypy-boto3-m2-1.28.5/mypy_boto3_m2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-m2
-Version: 1.28.16
-Summary: Type annotations for boto3.MainframeModernization 1.28.16 service generated with mypy-boto3-builder 7.17.1
+Version: 1.28.5
+Summary: Type annotations for boto3.MainframeModernization 1.28.5 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 m2 type-annotations botocore mypy typeshed autocomplete
+Keywords: boto3 m2 type-annotations boto3-stubs mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-m2"></a>
 
 # mypy-boto3-m2
 
 [![PyPI - mypy-boto3-m2](https://img.shields.io/pypi/v/mypy-boto3-m2.svg?color=blue)](https://pypi.org/project/mypy-boto3-m2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-m2.svg?color=blue)](https://pypi.org/project/mypy-boto3-m2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-m2)](https://pepy.tech/project/mypy-boto3-m2)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-m2?color=blue)](https://pypistats.org/packages/mypy-boto3-m2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MainframeModernization 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization)
+[boto3.MainframeModernization 1.28.5](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization)
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
 [mypy-boto3-m2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/).
 
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
@@ -353,35 +353,41 @@
 )
 
 
 def check_value(value: ApplicationDeploymentLifecycleType) -> bool:
     ...
 ```
 
-<a id="type-definitions"></a>
+<a id="typed-dictionaries"></a>
 
-### Type definitions
+### Typed dictionaries
 
 `mypy_boto3_m2.type_defs` module contains structures and shapes assembled to
-typed dictionaries and unions for additional type checking.
+typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_m2.type_defs import (
+    AlternateKeyOutputTypeDef,
     AlternateKeyTypeDef,
     ApplicationSummaryTypeDef,
     ApplicationVersionSummaryTypeDef,
     FileBatchJobDefinitionTypeDef,
     ScriptBatchJobDefinitionTypeDef,
+    FileBatchJobIdentifierOutputTypeDef,
+    ScriptBatchJobIdentifierOutputTypeDef,
     FileBatchJobIdentifierTypeDef,
     ScriptBatchJobIdentifierTypeDef,
     CancelBatchJobExecutionRequestRequestTypeDef,
     DefinitionTypeDef,
-    ResponseMetadataTypeDef,
+    CreateApplicationResponseTypeDef,
+    CreateDataSetImportTaskResponseTypeDef,
     CreateDeploymentRequestRequestTypeDef,
+    CreateDeploymentResponseTypeDef,
     HighAvailabilityConfigTypeDef,
+    CreateEnvironmentResponseTypeDef,
     ExternalLocationTypeDef,
     DataSetImportSummaryTypeDef,
     DataSetSummaryTypeDef,
     RecordLengthTypeDef,
     GdgDetailAttributesTypeDef,
     PoDetailAttributesTypeDef,
     PsDetailAttributesTypeDef,
@@ -389,101 +395,103 @@
     PoAttributesTypeDef,
     PsAttributesTypeDef,
     DeleteApplicationFromEnvironmentRequestRequestTypeDef,
     DeleteApplicationRequestRequestTypeDef,
     DeleteEnvironmentRequestRequestTypeDef,
     DeployedVersionSummaryTypeDef,
     DeploymentSummaryTypeDef,
+    EfsStorageConfigurationOutputTypeDef,
     EfsStorageConfigurationTypeDef,
     EngineVersionsSummaryTypeDef,
     EnvironmentSummaryTypeDef,
+    FsxStorageConfigurationOutputTypeDef,
     FsxStorageConfigurationTypeDef,
     GetApplicationRequestRequestTypeDef,
     LogGroupSummaryTypeDef,
     GetApplicationVersionRequestRequestTypeDef,
+    GetApplicationVersionResponseTypeDef,
     GetBatchJobExecutionRequestRequestTypeDef,
     GetDataSetDetailsRequestRequestTypeDef,
     GetDataSetImportTaskRequestRequestTypeDef,
     GetDeploymentRequestRequestTypeDef,
+    GetDeploymentResponseTypeDef,
     GetEnvironmentRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    HighAvailabilityConfigOutputTypeDef,
+    GetSignedBluinsightsUrlResponseTypeDef,
+    ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef,
     ListApplicationVersionsRequestRequestTypeDef,
+    ListApplicationsRequestListApplicationsPaginateTypeDef,
     ListApplicationsRequestRequestTypeDef,
+    ListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef,
     ListBatchJobDefinitionsRequestRequestTypeDef,
-    TimestampTypeDef,
+    ListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef,
+    ListBatchJobExecutionsRequestRequestTypeDef,
+    ListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef,
     ListDataSetImportHistoryRequestRequestTypeDef,
+    ListDataSetsRequestListDataSetsPaginateTypeDef,
     ListDataSetsRequestRequestTypeDef,
+    ListDeploymentsRequestListDeploymentsPaginateTypeDef,
     ListDeploymentsRequestRequestTypeDef,
+    ListEngineVersionsRequestListEngineVersionsPaginateTypeDef,
     ListEngineVersionsRequestRequestTypeDef,
+    ListEnvironmentsRequestListEnvironmentsPaginateTypeDef,
     ListEnvironmentsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     MaintenanceScheduleTypeDef,
+    PaginatorConfigTypeDef,
+    PrimaryKeyOutputTypeDef,
     PrimaryKeyTypeDef,
+    ResponseMetadataTypeDef,
     StartApplicationRequestRequestTypeDef,
+    StartBatchJobResponseTypeDef,
     StopApplicationRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    UpdateApplicationResponseTypeDef,
     UpdateEnvironmentRequestRequestTypeDef,
+    UpdateEnvironmentResponseTypeDef,
+    ListApplicationsResponseTypeDef,
+    ListApplicationVersionsResponseTypeDef,
     BatchJobDefinitionTypeDef,
+    BatchJobIdentifierOutputTypeDef,
     BatchJobIdentifierTypeDef,
     CreateApplicationRequestRequestTypeDef,
     UpdateApplicationRequestRequestTypeDef,
-    CreateApplicationResponseTypeDef,
-    CreateDataSetImportTaskResponseTypeDef,
-    CreateDeploymentResponseTypeDef,
-    CreateEnvironmentResponseTypeDef,
-    GetApplicationVersionResponseTypeDef,
-    GetDeploymentResponseTypeDef,
-    GetSignedBluinsightsUrlResponseTypeDef,
-    ListApplicationVersionsResponseTypeDef,
-    ListApplicationsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    StartBatchJobResponseTypeDef,
-    UpdateApplicationResponseTypeDef,
-    UpdateEnvironmentResponseTypeDef,
     DataSetImportTaskTypeDef,
     GetDataSetImportTaskResponseTypeDef,
     ListDataSetsResponseTypeDef,
     ListDeploymentsResponseTypeDef,
     ListEngineVersionsResponseTypeDef,
     ListEnvironmentsResponseTypeDef,
+    StorageConfigurationOutputTypeDef,
     StorageConfigurationTypeDef,
     GetApplicationResponseTypeDef,
-    ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef,
-    ListApplicationsRequestListApplicationsPaginateTypeDef,
-    ListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef,
-    ListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef,
-    ListDataSetsRequestListDataSetsPaginateTypeDef,
-    ListDeploymentsRequestListDeploymentsPaginateTypeDef,
-    ListEngineVersionsRequestListEngineVersionsPaginateTypeDef,
-    ListEnvironmentsRequestListEnvironmentsPaginateTypeDef,
-    ListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef,
-    ListBatchJobExecutionsRequestRequestTypeDef,
     PendingMaintenanceTypeDef,
-    VsamAttributesTypeDef,
     VsamDetailAttributesTypeDef,
+    VsamAttributesTypeDef,
     ListBatchJobDefinitionsResponseTypeDef,
     BatchJobExecutionSummaryTypeDef,
     GetBatchJobExecutionResponseTypeDef,
     StartBatchJobRequestRequestTypeDef,
     ListDataSetImportHistoryResponseTypeDef,
     CreateEnvironmentRequestRequestTypeDef,
     GetEnvironmentResponseTypeDef,
-    DatasetOrgAttributesTypeDef,
     DatasetDetailOrgAttributesTypeDef,
+    DatasetOrgAttributesTypeDef,
     ListBatchJobExecutionsResponseTypeDef,
-    DataSetTypeDef,
     GetDataSetDetailsResponseTypeDef,
+    DataSetTypeDef,
     DataSetImportItemTypeDef,
     DataSetImportConfigTypeDef,
     CreateDataSetImportTaskRequestRequestTypeDef,
 )
 
 
-def get_value() -> AlternateKeyTypeDef:
+def get_structure() -> AlternateKeyOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-m2-1.28.16/mypy_boto3_m2.egg-info/SOURCES.txt` & `mypy-boto3-m2-1.28.5/mypy_boto3_m2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-m2-1.28.16/setup.py` & `mypy-boto3-m2-1.28.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-m2",
-    version="1.28.16",
+    version="1.28.5",
     packages=["mypy_boto3_m2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.MainframeModernization 1.28.16 service generated with"
-        " mypy-boto3-builder 7.17.1"
+        "Type annotations for boto3.MainframeModernization 1.28.5 service generated with"
+        " mypy-boto3-builder 7.15.1"
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
-    keywords="boto3 m2 type-annotations botocore mypy typeshed autocomplete",
+    keywords="boto3 m2 type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_m2": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

