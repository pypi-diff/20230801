# Comparing `tmp/mypy-boto3-omics-1.28.16.tar.gz` & `tmp/mypy-boto3-omics-1.28.16.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-omics-1.28.16.tar", last modified: Mon Jul 31 19:32:48 2023, max compression
+gzip compressed data, was "mypy-boto3-omics-1.28.16.post1.tar", last modified: Tue Aug  1 11:37:27 2023, max compression
```

## Comparing `mypy-boto3-omics-1.28.16.tar` & `mypy-boto3-omics-1.28.16.post1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:32:48.066182 mypy-boto3-omics-1.28.16/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-31 19:32:20.000000 mypy-boto3-omics-1.28.16/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    29048 2023-07-31 19:32:48.066182 mypy-boto3-omics-1.28.16/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    27569 2023-07-31 19:32:20.000000 mypy-boto3-omics-1.28.16/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:32:48.058182 mypy-boto3-omics-1.28.16/mypy_boto3_omics/
--rw-r--r--   0 runner    (1001) docker     (123)     7505 2023-07-31 19:32:20.000000 mypy-boto3-omics-1.28.16/mypy_boto3_omics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7504 2023-07-31 19:32:20.000000 mypy-boto3-omics-1.28.16/mypy_boto3_omics/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-31 19:32:20.000000 mypy-boto3-omics-1.28.16/mypy_boto3_omics/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    61486 2023-07-31 19:32:20.000000 mypy-boto3-omics-1.28.16/mypy_boto3_omics/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    61374 2023-07-31 19:32:20.000000 mypy-boto3-omics-1.28.16/mypy_boto3_omics/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15919 2023-07-31 19:32:21.000000 mypy-boto3-omics-1.28.16/mypy_boto3_omics/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    15917 2023-07-31 19:32:21.000000 mypy-boto3-omics-1.28.16/mypy_boto3_omics/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    21971 2023-07-31 19:32:20.000000 mypy-boto3-omics-1.28.16/mypy_boto3_omics/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    21951 2023-07-31 19:32:20.000000 mypy-boto3-omics-1.28.16/mypy_boto3_omics/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 19:32:20.000000 mypy-boto3-omics-1.28.16/mypy_boto3_omics/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    98062 2023-07-31 19:32:23.000000 mypy-boto3-omics-1.28.16/mypy_boto3_omics/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    97906 2023-07-31 19:32:22.000000 mypy-boto3-omics-1.28.16/mypy_boto3_omics/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-31 19:32:20.000000 mypy-boto3-omics-1.28.16/mypy_boto3_omics/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    15098 2023-07-31 19:32:20.000000 mypy-boto3-omics-1.28.16/mypy_boto3_omics/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)    15082 2023-07-31 19:32:20.000000 mypy-boto3-omics-1.28.16/mypy_boto3_omics/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:32:48.066182 mypy-boto3-omics-1.28.16/mypy_boto3_omics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    29048 2023-07-31 19:32:47.000000 mypy-boto3-omics-1.28.16/mypy_boto3_omics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-31 19:32:47.000000 mypy-boto3-omics-1.28.16/mypy_boto3_omics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 19:32:47.000000 mypy-boto3-omics-1.28.16/mypy_boto3_omics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 19:32:47.000000 mypy-boto3-omics-1.28.16/mypy_boto3_omics.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-31 19:32:47.000000 mypy-boto3-omics-1.28.16/mypy_boto3_omics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-31 19:32:47.000000 mypy-boto3-omics-1.28.16/mypy_boto3_omics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 19:32:48.066182 mypy-boto3-omics-1.28.16/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-31 19:32:19.000000 mypy-boto3-omics-1.28.16/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:27.588804 mypy-boto3-omics-1.28.16.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:25:21.000000 mypy-boto3-omics-1.28.16.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    29119 2023-08-01 11:37:27.588804 mypy-boto3-omics-1.28.16.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    27637 2023-08-01 11:25:21.000000 mypy-boto3-omics-1.28.16.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:27.584804 mypy-boto3-omics-1.28.16.post1/mypy_boto3_omics/
+-rw-r--r--   0 runner    (1001) docker     (123)     7505 2023-08-01 11:25:21.000000 mypy-boto3-omics-1.28.16.post1/mypy_boto3_omics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7504 2023-08-01 11:25:21.000000 mypy-boto3-omics-1.28.16.post1/mypy_boto3_omics/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-08-01 11:25:21.000000 mypy-boto3-omics-1.28.16.post1/mypy_boto3_omics/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61333 2023-08-01 11:25:22.000000 mypy-boto3-omics-1.28.16.post1/mypy_boto3_omics/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61221 2023-08-01 11:25:21.000000 mypy-boto3-omics-1.28.16.post1/mypy_boto3_omics/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15919 2023-08-01 11:25:22.000000 mypy-boto3-omics-1.28.16.post1/mypy_boto3_omics/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15917 2023-08-01 11:25:22.000000 mypy-boto3-omics-1.28.16.post1/mypy_boto3_omics/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    21971 2023-08-01 11:25:22.000000 mypy-boto3-omics-1.28.16.post1/mypy_boto3_omics/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21951 2023-08-01 11:25:22.000000 mypy-boto3-omics-1.28.16.post1/mypy_boto3_omics/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:25:21.000000 mypy-boto3-omics-1.28.16.post1/mypy_boto3_omics/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    98180 2023-08-01 11:25:25.000000 mypy-boto3-omics-1.28.16.post1/mypy_boto3_omics/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    98024 2023-08-01 11:25:24.000000 mypy-boto3-omics-1.28.16.post1/mypy_boto3_omics/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-01 11:25:21.000000 mypy-boto3-omics-1.28.16.post1/mypy_boto3_omics/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15098 2023-08-01 11:25:22.000000 mypy-boto3-omics-1.28.16.post1/mypy_boto3_omics/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15082 2023-08-01 11:25:22.000000 mypy-boto3-omics-1.28.16.post1/mypy_boto3_omics/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:27.588804 mypy-boto3-omics-1.28.16.post1/mypy_boto3_omics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    29119 2023-08-01 11:37:27.000000 mypy-boto3-omics-1.28.16.post1/mypy_boto3_omics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-08-01 11:37:27.000000 mypy-boto3-omics-1.28.16.post1/mypy_boto3_omics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:27.000000 mypy-boto3-omics-1.28.16.post1/mypy_boto3_omics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:27.000000 mypy-boto3-omics-1.28.16.post1/mypy_boto3_omics.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:27.000000 mypy-boto3-omics-1.28.16.post1/mypy_boto3_omics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-01 11:37:27.000000 mypy-boto3-omics-1.28.16.post1/mypy_boto3_omics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:27.588804 mypy-boto3-omics-1.28.16.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-08-01 11:25:21.000000 mypy-boto3-omics-1.28.16.post1/setup.py
```

### Comparing `mypy-boto3-omics-1.28.16/LICENSE` & `mypy-boto3-omics-1.28.16.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-omics-1.28.16/PKG-INFO` & `mypy-boto3-omics-1.28.16.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-omics
-Version: 1.28.16
-Summary: Type annotations for boto3.Omics 1.28.16 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16.post1
+Summary: Type annotations for boto3.Omics 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 omics type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 omics type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -47,15 +47,15 @@
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
 [mypy-boto3-omics docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/).
 
 See how it helps to find and fix potential bugs:
 
@@ -75,15 +75,15 @@
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Waiters annotations](#waiters-annotations)
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
@@ -499,35 +499,36 @@
 )
 
 
 def check_value(value: AcceleratorsType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_omics.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_omics.type_defs import (
     AbortMultipartReadSetUploadRequestRequestTypeDef,
-    ActivateReadSetFilterTypeDef,
+    TimestampTypeDef,
     ActivateReadSetJobItemTypeDef,
     ActivateReadSetSourceItemTypeDef,
     AnnotationImportItemDetailTypeDef,
     AnnotationImportItemSourceTypeDef,
     AnnotationImportJobItemTypeDef,
     ReferenceItemTypeDef,
     SseConfigTypeDef,
     BatchDeleteReadSetRequestRequestTypeDef,
     ReadSetBatchErrorTypeDef,
     ResponseMetadataTypeDef,
+    BlobTypeDef,
     CancelAnnotationImportRequestRequestTypeDef,
     CancelRunRequestRequestTypeDef,
     CancelVariantImportRequestRequestTypeDef,
     CompleteReadSetUploadPartListItemTypeDef,
     CreateMultipartReadSetUploadRequestRequestTypeDef,
     CreateRunGroupRequestRequestTypeDef,
     WorkflowParameterTypeDef,
@@ -536,15 +537,14 @@
     DeleteReferenceStoreRequestRequestTypeDef,
     DeleteRunGroupRequestRequestTypeDef,
     DeleteRunRequestRequestTypeDef,
     DeleteSequenceStoreRequestRequestTypeDef,
     DeleteVariantStoreRequestRequestTypeDef,
     DeleteWorkflowRequestRequestTypeDef,
     ExportReadSetDetailTypeDef,
-    ExportReadSetFilterTypeDef,
     ExportReadSetJobDetailTypeDef,
     ExportReadSetTypeDef,
     FileInformationTypeDef,
     VcfOptionsTypeDef,
     WaiterConfigTypeDef,
     GetAnnotationImportRequestRequestTypeDef,
     GetAnnotationStoreRequestRequestTypeDef,
@@ -563,37 +563,30 @@
     GetRunRequestRequestTypeDef,
     GetRunTaskRequestRequestTypeDef,
     GetSequenceStoreRequestRequestTypeDef,
     GetVariantImportRequestRequestTypeDef,
     VariantImportItemDetailTypeDef,
     GetVariantStoreRequestRequestTypeDef,
     GetWorkflowRequestRequestTypeDef,
-    ImportReadSetFilterTypeDef,
     ImportReadSetJobItemTypeDef,
     SourceFilesTypeDef,
-    ImportReferenceFilterTypeDef,
     ImportReferenceJobItemTypeDef,
     ListAnnotationImportJobsFilterTypeDef,
     PaginatorConfigTypeDef,
     ListAnnotationStoresFilterTypeDef,
     ListMultipartReadSetUploadsRequestRequestTypeDef,
     MultipartReadSetUploadListItemTypeDef,
-    ReadSetUploadPartListFilterTypeDef,
     ReadSetUploadPartListItemTypeDef,
-    ReadSetFilterTypeDef,
-    ReferenceStoreFilterTypeDef,
-    ReferenceFilterTypeDef,
     ReferenceListItemTypeDef,
     ListRunGroupsRequestRequestTypeDef,
     RunGroupListItemTypeDef,
     ListRunTasksRequestRequestTypeDef,
     TaskListItemTypeDef,
     ListRunsRequestRequestTypeDef,
     RunListItemTypeDef,
-    SequenceStoreFilterTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListVariantImportJobsFilterTypeDef,
     VariantImportJobItemTypeDef,
     ListVariantStoresFilterTypeDef,
     ListWorkflowsRequestRequestTypeDef,
     WorkflowListItemTypeDef,
     ReadOptionsTypeDef,
@@ -605,16 +598,23 @@
     TsvStoreOptionsTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAnnotationStoreRequestRequestTypeDef,
     UpdateRunGroupRequestRequestTypeDef,
     UpdateVariantStoreRequestRequestTypeDef,
     UpdateWorkflowRequestRequestTypeDef,
-    UploadReadSetPartRequestRequestTypeDef,
-    ListReadSetActivationJobsRequestRequestTypeDef,
+    ActivateReadSetFilterTypeDef,
+    ExportReadSetFilterTypeDef,
+    ImportReadSetFilterTypeDef,
+    ImportReferenceFilterTypeDef,
+    ReadSetFilterTypeDef,
+    ReadSetUploadPartListFilterTypeDef,
+    ReferenceFilterTypeDef,
+    ReferenceStoreFilterTypeDef,
+    SequenceStoreFilterTypeDef,
     AnnotationStoreItemTypeDef,
     CreateReferenceStoreRequestRequestTypeDef,
     CreateSequenceStoreRequestRequestTypeDef,
     CreateVariantStoreRequestRequestTypeDef,
     ReferenceStoreDetailTypeDef,
     SequenceStoreDetailTypeDef,
     VariantStoreItemTypeDef,
@@ -646,19 +646,19 @@
     StartReadSetExportJobResponseTypeDef,
     StartReadSetImportJobResponseTypeDef,
     StartReferenceImportJobResponseTypeDef,
     StartRunResponseTypeDef,
     StartVariantImportResponseTypeDef,
     UpdateVariantStoreResponseTypeDef,
     UploadReadSetPartResponseTypeDef,
+    UploadReadSetPartRequestRequestTypeDef,
     CompleteMultipartReadSetUploadRequestRequestTypeDef,
     CreateWorkflowRequestRequestTypeDef,
     GetWorkflowResponseTypeDef,
     GetReadSetExportJobResponseTypeDef,
-    ListReadSetExportJobsRequestRequestTypeDef,
     ListReadSetExportJobsResponseTypeDef,
     StartReadSetExportJobRequestRequestTypeDef,
     ReadSetFilesTypeDef,
     ReferenceFilesTypeDef,
     GetAnnotationImportRequestAnnotationImportJobCreatedWaitTypeDef,
     GetAnnotationStoreRequestAnnotationStoreCreatedWaitTypeDef,
     GetAnnotationStoreRequestAnnotationStoreDeletedWaitTypeDef,
@@ -673,81 +673,84 @@
     GetVariantImportRequestVariantImportJobCreatedWaitTypeDef,
     GetVariantStoreRequestVariantStoreCreatedWaitTypeDef,
     GetVariantStoreRequestVariantStoreDeletedWaitTypeDef,
     GetWorkflowRequestWorkflowActiveWaitTypeDef,
     ReadSetListItemTypeDef,
     GetReferenceImportJobResponseTypeDef,
     GetVariantImportResponseTypeDef,
-    ListReadSetImportJobsRequestRequestTypeDef,
     ListReadSetImportJobsResponseTypeDef,
     ImportReadSetSourceItemTypeDef,
     StartReadSetImportJobSourceItemTypeDef,
-    ListReferenceImportJobsRequestRequestTypeDef,
     ListReferenceImportJobsResponseTypeDef,
     ListAnnotationImportJobsRequestRequestTypeDef,
     ListAnnotationImportJobsRequestListAnnotationImportJobsPaginateTypeDef,
     ListMultipartReadSetUploadsRequestListMultipartReadSetUploadsPaginateTypeDef,
-    ListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef,
-    ListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef,
-    ListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef,
-    ListReferenceImportJobsRequestListReferenceImportJobsPaginateTypeDef,
     ListRunGroupsRequestListRunGroupsPaginateTypeDef,
     ListRunTasksRequestListRunTasksPaginateTypeDef,
     ListRunsRequestListRunsPaginateTypeDef,
     ListWorkflowsRequestListWorkflowsPaginateTypeDef,
     ListAnnotationStoresRequestListAnnotationStoresPaginateTypeDef,
     ListAnnotationStoresRequestRequestTypeDef,
     ListMultipartReadSetUploadsResponseTypeDef,
-    ListReadSetUploadPartsRequestListReadSetUploadPartsPaginateTypeDef,
-    ListReadSetUploadPartsRequestRequestTypeDef,
     ListReadSetUploadPartsResponseTypeDef,
-    ListReadSetsRequestListReadSetsPaginateTypeDef,
-    ListReadSetsRequestRequestTypeDef,
-    ListReferenceStoresRequestListReferenceStoresPaginateTypeDef,
-    ListReferenceStoresRequestRequestTypeDef,
-    ListReferencesRequestListReferencesPaginateTypeDef,
-    ListReferencesRequestRequestTypeDef,
     ListReferencesResponseTypeDef,
     ListRunGroupsResponseTypeDef,
     ListRunTasksResponseTypeDef,
     ListRunsResponseTypeDef,
-    ListSequenceStoresRequestListSequenceStoresPaginateTypeDef,
-    ListSequenceStoresRequestRequestTypeDef,
     ListVariantImportJobsRequestListVariantImportJobsPaginateTypeDef,
     ListVariantImportJobsRequestRequestTypeDef,
     ListVariantImportJobsResponseTypeDef,
     ListVariantStoresRequestListVariantStoresPaginateTypeDef,
     ListVariantStoresRequestRequestTypeDef,
     ListWorkflowsResponseTypeDef,
     TsvOptionsTypeDef,
     StartReadSetActivationJobRequestRequestTypeDef,
     StartReferenceImportJobRequestRequestTypeDef,
     StartVariantImportRequestRequestTypeDef,
     StoreOptionsOutputTypeDef,
     StoreOptionsTypeDef,
+    ListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef,
+    ListReadSetActivationJobsRequestRequestTypeDef,
+    ListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef,
+    ListReadSetExportJobsRequestRequestTypeDef,
+    ListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef,
+    ListReadSetImportJobsRequestRequestTypeDef,
+    ListReferenceImportJobsRequestListReferenceImportJobsPaginateTypeDef,
+    ListReferenceImportJobsRequestRequestTypeDef,
+    ListReadSetsRequestListReadSetsPaginateTypeDef,
+    ListReadSetsRequestRequestTypeDef,
+    ListReadSetUploadPartsRequestListReadSetUploadPartsPaginateTypeDef,
+    ListReadSetUploadPartsRequestRequestTypeDef,
+    ListReferencesRequestListReferencesPaginateTypeDef,
+    ListReferencesRequestRequestTypeDef,
+    ListReferenceStoresRequestListReferenceStoresPaginateTypeDef,
+    ListReferenceStoresRequestRequestTypeDef,
+    ListSequenceStoresRequestListSequenceStoresPaginateTypeDef,
+    ListSequenceStoresRequestRequestTypeDef,
     ListAnnotationStoresResponseTypeDef,
     ListReferenceStoresResponseTypeDef,
     ListSequenceStoresResponseTypeDef,
     ListVariantStoresResponseTypeDef,
     GetReadSetMetadataResponseTypeDef,
     GetReferenceMetadataResponseTypeDef,
     ListReadSetsResponseTypeDef,
     GetReadSetImportJobResponseTypeDef,
     StartReadSetImportJobRequestRequestTypeDef,
     FormatOptionsTypeDef,
     CreateAnnotationStoreResponseTypeDef,
     GetAnnotationStoreResponseTypeDef,
     UpdateAnnotationStoreResponseTypeDef,
     CreateAnnotationStoreRequestRequestTypeDef,
+    StoreOptionsUnionTypeDef,
     GetAnnotationImportResponseTypeDef,
     StartAnnotationImportRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AbortMultipartReadSetUploadRequestRequestTypeDef:
+def get_value() -> AbortMultipartReadSetUploadRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-omics-1.28.16/README.md` & `mypy-boto3-omics-1.28.16.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
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
 [mypy-boto3-omics docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/).
 
 See how it helps to find and fix potential bugs:
 
@@ -43,15 +43,15 @@
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Waiters annotations](#waiters-annotations)
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
@@ -467,35 +467,36 @@
 )
 
 
 def check_value(value: AcceleratorsType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_omics.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_omics.type_defs import (
     AbortMultipartReadSetUploadRequestRequestTypeDef,
-    ActivateReadSetFilterTypeDef,
+    TimestampTypeDef,
     ActivateReadSetJobItemTypeDef,
     ActivateReadSetSourceItemTypeDef,
     AnnotationImportItemDetailTypeDef,
     AnnotationImportItemSourceTypeDef,
     AnnotationImportJobItemTypeDef,
     ReferenceItemTypeDef,
     SseConfigTypeDef,
     BatchDeleteReadSetRequestRequestTypeDef,
     ReadSetBatchErrorTypeDef,
     ResponseMetadataTypeDef,
+    BlobTypeDef,
     CancelAnnotationImportRequestRequestTypeDef,
     CancelRunRequestRequestTypeDef,
     CancelVariantImportRequestRequestTypeDef,
     CompleteReadSetUploadPartListItemTypeDef,
     CreateMultipartReadSetUploadRequestRequestTypeDef,
     CreateRunGroupRequestRequestTypeDef,
     WorkflowParameterTypeDef,
@@ -504,15 +505,14 @@
     DeleteReferenceStoreRequestRequestTypeDef,
     DeleteRunGroupRequestRequestTypeDef,
     DeleteRunRequestRequestTypeDef,
     DeleteSequenceStoreRequestRequestTypeDef,
     DeleteVariantStoreRequestRequestTypeDef,
     DeleteWorkflowRequestRequestTypeDef,
     ExportReadSetDetailTypeDef,
-    ExportReadSetFilterTypeDef,
     ExportReadSetJobDetailTypeDef,
     ExportReadSetTypeDef,
     FileInformationTypeDef,
     VcfOptionsTypeDef,
     WaiterConfigTypeDef,
     GetAnnotationImportRequestRequestTypeDef,
     GetAnnotationStoreRequestRequestTypeDef,
@@ -531,37 +531,30 @@
     GetRunRequestRequestTypeDef,
     GetRunTaskRequestRequestTypeDef,
     GetSequenceStoreRequestRequestTypeDef,
     GetVariantImportRequestRequestTypeDef,
     VariantImportItemDetailTypeDef,
     GetVariantStoreRequestRequestTypeDef,
     GetWorkflowRequestRequestTypeDef,
-    ImportReadSetFilterTypeDef,
     ImportReadSetJobItemTypeDef,
     SourceFilesTypeDef,
-    ImportReferenceFilterTypeDef,
     ImportReferenceJobItemTypeDef,
     ListAnnotationImportJobsFilterTypeDef,
     PaginatorConfigTypeDef,
     ListAnnotationStoresFilterTypeDef,
     ListMultipartReadSetUploadsRequestRequestTypeDef,
     MultipartReadSetUploadListItemTypeDef,
-    ReadSetUploadPartListFilterTypeDef,
     ReadSetUploadPartListItemTypeDef,
-    ReadSetFilterTypeDef,
-    ReferenceStoreFilterTypeDef,
-    ReferenceFilterTypeDef,
     ReferenceListItemTypeDef,
     ListRunGroupsRequestRequestTypeDef,
     RunGroupListItemTypeDef,
     ListRunTasksRequestRequestTypeDef,
     TaskListItemTypeDef,
     ListRunsRequestRequestTypeDef,
     RunListItemTypeDef,
-    SequenceStoreFilterTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListVariantImportJobsFilterTypeDef,
     VariantImportJobItemTypeDef,
     ListVariantStoresFilterTypeDef,
     ListWorkflowsRequestRequestTypeDef,
     WorkflowListItemTypeDef,
     ReadOptionsTypeDef,
@@ -573,16 +566,23 @@
     TsvStoreOptionsTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAnnotationStoreRequestRequestTypeDef,
     UpdateRunGroupRequestRequestTypeDef,
     UpdateVariantStoreRequestRequestTypeDef,
     UpdateWorkflowRequestRequestTypeDef,
-    UploadReadSetPartRequestRequestTypeDef,
-    ListReadSetActivationJobsRequestRequestTypeDef,
+    ActivateReadSetFilterTypeDef,
+    ExportReadSetFilterTypeDef,
+    ImportReadSetFilterTypeDef,
+    ImportReferenceFilterTypeDef,
+    ReadSetFilterTypeDef,
+    ReadSetUploadPartListFilterTypeDef,
+    ReferenceFilterTypeDef,
+    ReferenceStoreFilterTypeDef,
+    SequenceStoreFilterTypeDef,
     AnnotationStoreItemTypeDef,
     CreateReferenceStoreRequestRequestTypeDef,
     CreateSequenceStoreRequestRequestTypeDef,
     CreateVariantStoreRequestRequestTypeDef,
     ReferenceStoreDetailTypeDef,
     SequenceStoreDetailTypeDef,
     VariantStoreItemTypeDef,
@@ -614,19 +614,19 @@
     StartReadSetExportJobResponseTypeDef,
     StartReadSetImportJobResponseTypeDef,
     StartReferenceImportJobResponseTypeDef,
     StartRunResponseTypeDef,
     StartVariantImportResponseTypeDef,
     UpdateVariantStoreResponseTypeDef,
     UploadReadSetPartResponseTypeDef,
+    UploadReadSetPartRequestRequestTypeDef,
     CompleteMultipartReadSetUploadRequestRequestTypeDef,
     CreateWorkflowRequestRequestTypeDef,
     GetWorkflowResponseTypeDef,
     GetReadSetExportJobResponseTypeDef,
-    ListReadSetExportJobsRequestRequestTypeDef,
     ListReadSetExportJobsResponseTypeDef,
     StartReadSetExportJobRequestRequestTypeDef,
     ReadSetFilesTypeDef,
     ReferenceFilesTypeDef,
     GetAnnotationImportRequestAnnotationImportJobCreatedWaitTypeDef,
     GetAnnotationStoreRequestAnnotationStoreCreatedWaitTypeDef,
     GetAnnotationStoreRequestAnnotationStoreDeletedWaitTypeDef,
@@ -641,81 +641,84 @@
     GetVariantImportRequestVariantImportJobCreatedWaitTypeDef,
     GetVariantStoreRequestVariantStoreCreatedWaitTypeDef,
     GetVariantStoreRequestVariantStoreDeletedWaitTypeDef,
     GetWorkflowRequestWorkflowActiveWaitTypeDef,
     ReadSetListItemTypeDef,
     GetReferenceImportJobResponseTypeDef,
     GetVariantImportResponseTypeDef,
-    ListReadSetImportJobsRequestRequestTypeDef,
     ListReadSetImportJobsResponseTypeDef,
     ImportReadSetSourceItemTypeDef,
     StartReadSetImportJobSourceItemTypeDef,
-    ListReferenceImportJobsRequestRequestTypeDef,
     ListReferenceImportJobsResponseTypeDef,
     ListAnnotationImportJobsRequestRequestTypeDef,
     ListAnnotationImportJobsRequestListAnnotationImportJobsPaginateTypeDef,
     ListMultipartReadSetUploadsRequestListMultipartReadSetUploadsPaginateTypeDef,
-    ListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef,
-    ListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef,
-    ListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef,
-    ListReferenceImportJobsRequestListReferenceImportJobsPaginateTypeDef,
     ListRunGroupsRequestListRunGroupsPaginateTypeDef,
     ListRunTasksRequestListRunTasksPaginateTypeDef,
     ListRunsRequestListRunsPaginateTypeDef,
     ListWorkflowsRequestListWorkflowsPaginateTypeDef,
     ListAnnotationStoresRequestListAnnotationStoresPaginateTypeDef,
     ListAnnotationStoresRequestRequestTypeDef,
     ListMultipartReadSetUploadsResponseTypeDef,
-    ListReadSetUploadPartsRequestListReadSetUploadPartsPaginateTypeDef,
-    ListReadSetUploadPartsRequestRequestTypeDef,
     ListReadSetUploadPartsResponseTypeDef,
-    ListReadSetsRequestListReadSetsPaginateTypeDef,
-    ListReadSetsRequestRequestTypeDef,
-    ListReferenceStoresRequestListReferenceStoresPaginateTypeDef,
-    ListReferenceStoresRequestRequestTypeDef,
-    ListReferencesRequestListReferencesPaginateTypeDef,
-    ListReferencesRequestRequestTypeDef,
     ListReferencesResponseTypeDef,
     ListRunGroupsResponseTypeDef,
     ListRunTasksResponseTypeDef,
     ListRunsResponseTypeDef,
-    ListSequenceStoresRequestListSequenceStoresPaginateTypeDef,
-    ListSequenceStoresRequestRequestTypeDef,
     ListVariantImportJobsRequestListVariantImportJobsPaginateTypeDef,
     ListVariantImportJobsRequestRequestTypeDef,
     ListVariantImportJobsResponseTypeDef,
     ListVariantStoresRequestListVariantStoresPaginateTypeDef,
     ListVariantStoresRequestRequestTypeDef,
     ListWorkflowsResponseTypeDef,
     TsvOptionsTypeDef,
     StartReadSetActivationJobRequestRequestTypeDef,
     StartReferenceImportJobRequestRequestTypeDef,
     StartVariantImportRequestRequestTypeDef,
     StoreOptionsOutputTypeDef,
     StoreOptionsTypeDef,
+    ListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef,
+    ListReadSetActivationJobsRequestRequestTypeDef,
+    ListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef,
+    ListReadSetExportJobsRequestRequestTypeDef,
+    ListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef,
+    ListReadSetImportJobsRequestRequestTypeDef,
+    ListReferenceImportJobsRequestListReferenceImportJobsPaginateTypeDef,
+    ListReferenceImportJobsRequestRequestTypeDef,
+    ListReadSetsRequestListReadSetsPaginateTypeDef,
+    ListReadSetsRequestRequestTypeDef,
+    ListReadSetUploadPartsRequestListReadSetUploadPartsPaginateTypeDef,
+    ListReadSetUploadPartsRequestRequestTypeDef,
+    ListReferencesRequestListReferencesPaginateTypeDef,
+    ListReferencesRequestRequestTypeDef,
+    ListReferenceStoresRequestListReferenceStoresPaginateTypeDef,
+    ListReferenceStoresRequestRequestTypeDef,
+    ListSequenceStoresRequestListSequenceStoresPaginateTypeDef,
+    ListSequenceStoresRequestRequestTypeDef,
     ListAnnotationStoresResponseTypeDef,
     ListReferenceStoresResponseTypeDef,
     ListSequenceStoresResponseTypeDef,
     ListVariantStoresResponseTypeDef,
     GetReadSetMetadataResponseTypeDef,
     GetReferenceMetadataResponseTypeDef,
     ListReadSetsResponseTypeDef,
     GetReadSetImportJobResponseTypeDef,
     StartReadSetImportJobRequestRequestTypeDef,
     FormatOptionsTypeDef,
     CreateAnnotationStoreResponseTypeDef,
     GetAnnotationStoreResponseTypeDef,
     UpdateAnnotationStoreResponseTypeDef,
     CreateAnnotationStoreRequestRequestTypeDef,
+    StoreOptionsUnionTypeDef,
     GetAnnotationImportResponseTypeDef,
     StartAnnotationImportRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AbortMultipartReadSetUploadRequestRequestTypeDef:
+def get_value() -> AbortMultipartReadSetUploadRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-omics-1.28.16/mypy_boto3_omics/__init__.py` & `mypy-boto3-omics-1.28.16.post1/mypy_boto3_omics/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-omics-1.28.16/mypy_boto3_omics/__init__.pyi` & `mypy-boto3-omics-1.28.16.post1/mypy_boto3_omics/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-omics-1.28.16/mypy_boto3_omics/__main__.py` & `mypy-boto3-omics-1.28.16.post1/mypy_boto3_omics/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Omics 1.28.16\nVersion:         1.28.16\nBuilder version:"
-        " 7.16.2\nDocs:           "
+        "Type annotations for boto3.Omics 1.28.16\nVersion:         1.28.16.post1\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.16")
+    print("1.28.16.post1")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-omics-1.28.16/mypy_boto3_omics/client.py` & `mypy-boto3-omics-1.28.16.post1/mypy_boto3_omics/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,18 +10,17 @@
     from mypy_boto3_omics.client import OmicsClient
 
     session = Session()
     client: OmicsClient = session.client("omics")
     ```
 """
 import sys
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
-from botocore.response import StreamingBody
 
 from .literals import (
     FileTypeType,
     ReadSetFileType,
     ReadSetPartSourceType,
     ReferenceFileType,
     RunLogLevelType,
@@ -51,14 +50,15 @@
     ListVariantStoresPaginator,
     ListWorkflowsPaginator,
 )
 from .type_defs import (
     ActivateReadSetFilterTypeDef,
     AnnotationImportItemSourceTypeDef,
     BatchDeleteReadSetResponseTypeDef,
+    BlobTypeDef,
     CompleteMultipartReadSetUploadResponseTypeDef,
     CompleteReadSetUploadPartListItemTypeDef,
     CreateAnnotationStoreResponseTypeDef,
     CreateMultipartReadSetUploadResponseTypeDef,
     CreateReferenceStoreResponseTypeDef,
     CreateRunGroupResponseTypeDef,
     CreateSequenceStoreResponseTypeDef,
@@ -126,16 +126,15 @@
     StartReadSetExportJobResponseTypeDef,
     StartReadSetImportJobResponseTypeDef,
     StartReadSetImportJobSourceItemTypeDef,
     StartReferenceImportJobResponseTypeDef,
     StartReferenceImportJobSourceItemTypeDef,
     StartRunResponseTypeDef,
     StartVariantImportResponseTypeDef,
-    StoreOptionsOutputTypeDef,
-    StoreOptionsTypeDef,
+    StoreOptionsUnionTypeDef,
     UpdateAnnotationStoreResponseTypeDef,
     UpdateVariantStoreResponseTypeDef,
     UploadReadSetPartResponseTypeDef,
     VariantImportItemSourceTypeDef,
     WorkflowParameterTypeDef,
 )
 from .waiter import (
@@ -283,15 +282,15 @@
         *,
         storeFormat: StoreFormatType,
         reference: ReferenceItemTypeDef = ...,
         name: str = ...,
         description: str = ...,
         tags: Mapping[str, str] = ...,
         sseConfig: SseConfigTypeDef = ...,
-        storeOptions: Union[StoreOptionsTypeDef, StoreOptionsOutputTypeDef] = ...
+        storeOptions: StoreOptionsUnionTypeDef = ...
     ) -> CreateAnnotationStoreResponseTypeDef:
         """
         Creates an annotation store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.create_annotation_store)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/client/#create_annotation_store)
         """
@@ -387,15 +386,15 @@
     def create_workflow(
         self,
         *,
         requestId: str,
         name: str = ...,
         description: str = ...,
         engine: WorkflowEngineType = ...,
-        definitionZip: Union[str, bytes, IO[Any], StreamingBody] = ...,
+        definitionZip: BlobTypeDef = ...,
         definitionUri: str = ...,
         main: str = ...,
         parameterTemplate: Mapping[str, WorkflowParameterTypeDef] = ...,
         storageCapacity: int = ...,
         tags: Mapping[str, str] = ...,
         accelerators: Literal["GPU"] = ...
     ) -> CreateWorkflowResponseTypeDef:
@@ -1115,15 +1114,15 @@
     def upload_read_set_part(
         self,
         *,
         sequenceStoreId: str,
         uploadId: str,
         partSource: ReadSetPartSourceType,
         partNumber: int,
-        payload: Union[str, bytes, IO[Any], StreamingBody]
+        payload: BlobTypeDef
     ) -> UploadReadSetPartResponseTypeDef:
         """
         This operation uploads a specific part of a read set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.upload_read_set_part)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/client/#upload_read_set_part)
         """
```

### Comparing `mypy-boto3-omics-1.28.16/mypy_boto3_omics/client.pyi` & `mypy-boto3-omics-1.28.16.post1/mypy_boto3_omics/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,18 +10,17 @@
     from mypy_boto3_omics.client import OmicsClient
 
     session = Session()
     client: OmicsClient = session.client("omics")
     ```
 """
 import sys
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
-from botocore.response import StreamingBody
 
 from .literals import (
     FileTypeType,
     ReadSetFileType,
     ReadSetPartSourceType,
     ReferenceFileType,
     RunLogLevelType,
@@ -51,14 +50,15 @@
     ListVariantStoresPaginator,
     ListWorkflowsPaginator,
 )
 from .type_defs import (
     ActivateReadSetFilterTypeDef,
     AnnotationImportItemSourceTypeDef,
     BatchDeleteReadSetResponseTypeDef,
+    BlobTypeDef,
     CompleteMultipartReadSetUploadResponseTypeDef,
     CompleteReadSetUploadPartListItemTypeDef,
     CreateAnnotationStoreResponseTypeDef,
     CreateMultipartReadSetUploadResponseTypeDef,
     CreateReferenceStoreResponseTypeDef,
     CreateRunGroupResponseTypeDef,
     CreateSequenceStoreResponseTypeDef,
@@ -126,16 +126,15 @@
     StartReadSetExportJobResponseTypeDef,
     StartReadSetImportJobResponseTypeDef,
     StartReadSetImportJobSourceItemTypeDef,
     StartReferenceImportJobResponseTypeDef,
     StartReferenceImportJobSourceItemTypeDef,
     StartRunResponseTypeDef,
     StartVariantImportResponseTypeDef,
-    StoreOptionsOutputTypeDef,
-    StoreOptionsTypeDef,
+    StoreOptionsUnionTypeDef,
     UpdateAnnotationStoreResponseTypeDef,
     UpdateVariantStoreResponseTypeDef,
     UploadReadSetPartResponseTypeDef,
     VariantImportItemSourceTypeDef,
     WorkflowParameterTypeDef,
 )
 from .waiter import (
@@ -270,15 +269,15 @@
         *,
         storeFormat: StoreFormatType,
         reference: ReferenceItemTypeDef = ...,
         name: str = ...,
         description: str = ...,
         tags: Mapping[str, str] = ...,
         sseConfig: SseConfigTypeDef = ...,
-        storeOptions: Union[StoreOptionsTypeDef, StoreOptionsOutputTypeDef] = ...
+        storeOptions: StoreOptionsUnionTypeDef = ...
     ) -> CreateAnnotationStoreResponseTypeDef:
         """
         Creates an annotation store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.create_annotation_store)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/client/#create_annotation_store)
         """
@@ -368,15 +367,15 @@
     def create_workflow(
         self,
         *,
         requestId: str,
         name: str = ...,
         description: str = ...,
         engine: WorkflowEngineType = ...,
-        definitionZip: Union[str, bytes, IO[Any], StreamingBody] = ...,
+        definitionZip: BlobTypeDef = ...,
         definitionUri: str = ...,
         main: str = ...,
         parameterTemplate: Mapping[str, WorkflowParameterTypeDef] = ...,
         storageCapacity: int = ...,
         tags: Mapping[str, str] = ...,
         accelerators: Literal["GPU"] = ...
     ) -> CreateWorkflowResponseTypeDef:
@@ -1036,15 +1035,15 @@
     def upload_read_set_part(
         self,
         *,
         sequenceStoreId: str,
         uploadId: str,
         partSource: ReadSetPartSourceType,
         partNumber: int,
-        payload: Union[str, bytes, IO[Any], StreamingBody]
+        payload: BlobTypeDef
     ) -> UploadReadSetPartResponseTypeDef:
         """
         This operation uploads a specific part of a read set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.upload_read_set_part)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/client/#upload_read_set_part)
         """
```

### Comparing `mypy-boto3-omics-1.28.16/mypy_boto3_omics/literals.py` & `mypy-boto3-omics-1.28.16.post1/mypy_boto3_omics/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-omics-1.28.16/mypy_boto3_omics/literals.pyi` & `mypy-boto3-omics-1.28.16.post1/mypy_boto3_omics/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-omics-1.28.16/mypy_boto3_omics/paginator.py` & `mypy-boto3-omics-1.28.16.post1/mypy_boto3_omics/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-omics-1.28.16/mypy_boto3_omics/paginator.pyi` & `mypy-boto3-omics-1.28.16.post1/mypy_boto3_omics/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-omics-1.28.16/mypy_boto3_omics/type_defs.py` & `mypy-boto3-omics-1.28.16.post1/mypy_boto3_omics/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_omics.type_defs import AbortMultipartReadSetUploadRequestRequestTypeDef
 
-    data: AbortMultipartReadSetUploadRequestRequestTypeDef = {...}
+    data: AbortMultipartReadSetUploadRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -55,25 +55,26 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AbortMultipartReadSetUploadRequestRequestTypeDef",
-    "ActivateReadSetFilterTypeDef",
+    "TimestampTypeDef",
     "ActivateReadSetJobItemTypeDef",
     "ActivateReadSetSourceItemTypeDef",
     "AnnotationImportItemDetailTypeDef",
     "AnnotationImportItemSourceTypeDef",
     "AnnotationImportJobItemTypeDef",
     "ReferenceItemTypeDef",
     "SseConfigTypeDef",
     "BatchDeleteReadSetRequestRequestTypeDef",
     "ReadSetBatchErrorTypeDef",
     "ResponseMetadataTypeDef",
+    "BlobTypeDef",
     "CancelAnnotationImportRequestRequestTypeDef",
     "CancelRunRequestRequestTypeDef",
     "CancelVariantImportRequestRequestTypeDef",
     "CompleteReadSetUploadPartListItemTypeDef",
     "CreateMultipartReadSetUploadRequestRequestTypeDef",
     "CreateRunGroupRequestRequestTypeDef",
     "WorkflowParameterTypeDef",
@@ -82,15 +83,14 @@
     "DeleteReferenceStoreRequestRequestTypeDef",
     "DeleteRunGroupRequestRequestTypeDef",
     "DeleteRunRequestRequestTypeDef",
     "DeleteSequenceStoreRequestRequestTypeDef",
     "DeleteVariantStoreRequestRequestTypeDef",
     "DeleteWorkflowRequestRequestTypeDef",
     "ExportReadSetDetailTypeDef",
-    "ExportReadSetFilterTypeDef",
     "ExportReadSetJobDetailTypeDef",
     "ExportReadSetTypeDef",
     "FileInformationTypeDef",
     "VcfOptionsTypeDef",
     "WaiterConfigTypeDef",
     "GetAnnotationImportRequestRequestTypeDef",
     "GetAnnotationStoreRequestRequestTypeDef",
@@ -109,37 +109,30 @@
     "GetRunRequestRequestTypeDef",
     "GetRunTaskRequestRequestTypeDef",
     "GetSequenceStoreRequestRequestTypeDef",
     "GetVariantImportRequestRequestTypeDef",
     "VariantImportItemDetailTypeDef",
     "GetVariantStoreRequestRequestTypeDef",
     "GetWorkflowRequestRequestTypeDef",
-    "ImportReadSetFilterTypeDef",
     "ImportReadSetJobItemTypeDef",
     "SourceFilesTypeDef",
-    "ImportReferenceFilterTypeDef",
     "ImportReferenceJobItemTypeDef",
     "ListAnnotationImportJobsFilterTypeDef",
     "PaginatorConfigTypeDef",
     "ListAnnotationStoresFilterTypeDef",
     "ListMultipartReadSetUploadsRequestRequestTypeDef",
     "MultipartReadSetUploadListItemTypeDef",
-    "ReadSetUploadPartListFilterTypeDef",
     "ReadSetUploadPartListItemTypeDef",
-    "ReadSetFilterTypeDef",
-    "ReferenceStoreFilterTypeDef",
-    "ReferenceFilterTypeDef",
     "ReferenceListItemTypeDef",
     "ListRunGroupsRequestRequestTypeDef",
     "RunGroupListItemTypeDef",
     "ListRunTasksRequestRequestTypeDef",
     "TaskListItemTypeDef",
     "ListRunsRequestRequestTypeDef",
     "RunListItemTypeDef",
-    "SequenceStoreFilterTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListVariantImportJobsFilterTypeDef",
     "VariantImportJobItemTypeDef",
     "ListVariantStoresFilterTypeDef",
     "ListWorkflowsRequestRequestTypeDef",
     "WorkflowListItemTypeDef",
     "ReadOptionsTypeDef",
@@ -151,16 +144,23 @@
     "TsvStoreOptionsTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAnnotationStoreRequestRequestTypeDef",
     "UpdateRunGroupRequestRequestTypeDef",
     "UpdateVariantStoreRequestRequestTypeDef",
     "UpdateWorkflowRequestRequestTypeDef",
-    "UploadReadSetPartRequestRequestTypeDef",
-    "ListReadSetActivationJobsRequestRequestTypeDef",
+    "ActivateReadSetFilterTypeDef",
+    "ExportReadSetFilterTypeDef",
+    "ImportReadSetFilterTypeDef",
+    "ImportReferenceFilterTypeDef",
+    "ReadSetFilterTypeDef",
+    "ReadSetUploadPartListFilterTypeDef",
+    "ReferenceFilterTypeDef",
+    "ReferenceStoreFilterTypeDef",
+    "SequenceStoreFilterTypeDef",
     "AnnotationStoreItemTypeDef",
     "CreateReferenceStoreRequestRequestTypeDef",
     "CreateSequenceStoreRequestRequestTypeDef",
     "CreateVariantStoreRequestRequestTypeDef",
     "ReferenceStoreDetailTypeDef",
     "SequenceStoreDetailTypeDef",
     "VariantStoreItemTypeDef",
@@ -192,19 +192,19 @@
     "StartReadSetExportJobResponseTypeDef",
     "StartReadSetImportJobResponseTypeDef",
     "StartReferenceImportJobResponseTypeDef",
     "StartRunResponseTypeDef",
     "StartVariantImportResponseTypeDef",
     "UpdateVariantStoreResponseTypeDef",
     "UploadReadSetPartResponseTypeDef",
+    "UploadReadSetPartRequestRequestTypeDef",
     "CompleteMultipartReadSetUploadRequestRequestTypeDef",
     "CreateWorkflowRequestRequestTypeDef",
     "GetWorkflowResponseTypeDef",
     "GetReadSetExportJobResponseTypeDef",
-    "ListReadSetExportJobsRequestRequestTypeDef",
     "ListReadSetExportJobsResponseTypeDef",
     "StartReadSetExportJobRequestRequestTypeDef",
     "ReadSetFilesTypeDef",
     "ReferenceFilesTypeDef",
     "GetAnnotationImportRequestAnnotationImportJobCreatedWaitTypeDef",
     "GetAnnotationStoreRequestAnnotationStoreCreatedWaitTypeDef",
     "GetAnnotationStoreRequestAnnotationStoreDeletedWaitTypeDef",
@@ -219,97 +219,91 @@
     "GetVariantImportRequestVariantImportJobCreatedWaitTypeDef",
     "GetVariantStoreRequestVariantStoreCreatedWaitTypeDef",
     "GetVariantStoreRequestVariantStoreDeletedWaitTypeDef",
     "GetWorkflowRequestWorkflowActiveWaitTypeDef",
     "ReadSetListItemTypeDef",
     "GetReferenceImportJobResponseTypeDef",
     "GetVariantImportResponseTypeDef",
-    "ListReadSetImportJobsRequestRequestTypeDef",
     "ListReadSetImportJobsResponseTypeDef",
     "ImportReadSetSourceItemTypeDef",
     "StartReadSetImportJobSourceItemTypeDef",
-    "ListReferenceImportJobsRequestRequestTypeDef",
     "ListReferenceImportJobsResponseTypeDef",
     "ListAnnotationImportJobsRequestRequestTypeDef",
     "ListAnnotationImportJobsRequestListAnnotationImportJobsPaginateTypeDef",
     "ListMultipartReadSetUploadsRequestListMultipartReadSetUploadsPaginateTypeDef",
-    "ListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef",
-    "ListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef",
-    "ListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef",
-    "ListReferenceImportJobsRequestListReferenceImportJobsPaginateTypeDef",
     "ListRunGroupsRequestListRunGroupsPaginateTypeDef",
     "ListRunTasksRequestListRunTasksPaginateTypeDef",
     "ListRunsRequestListRunsPaginateTypeDef",
     "ListWorkflowsRequestListWorkflowsPaginateTypeDef",
     "ListAnnotationStoresRequestListAnnotationStoresPaginateTypeDef",
     "ListAnnotationStoresRequestRequestTypeDef",
     "ListMultipartReadSetUploadsResponseTypeDef",
-    "ListReadSetUploadPartsRequestListReadSetUploadPartsPaginateTypeDef",
-    "ListReadSetUploadPartsRequestRequestTypeDef",
     "ListReadSetUploadPartsResponseTypeDef",
-    "ListReadSetsRequestListReadSetsPaginateTypeDef",
-    "ListReadSetsRequestRequestTypeDef",
-    "ListReferenceStoresRequestListReferenceStoresPaginateTypeDef",
-    "ListReferenceStoresRequestRequestTypeDef",
-    "ListReferencesRequestListReferencesPaginateTypeDef",
-    "ListReferencesRequestRequestTypeDef",
     "ListReferencesResponseTypeDef",
     "ListRunGroupsResponseTypeDef",
     "ListRunTasksResponseTypeDef",
     "ListRunsResponseTypeDef",
-    "ListSequenceStoresRequestListSequenceStoresPaginateTypeDef",
-    "ListSequenceStoresRequestRequestTypeDef",
     "ListVariantImportJobsRequestListVariantImportJobsPaginateTypeDef",
     "ListVariantImportJobsRequestRequestTypeDef",
     "ListVariantImportJobsResponseTypeDef",
     "ListVariantStoresRequestListVariantStoresPaginateTypeDef",
     "ListVariantStoresRequestRequestTypeDef",
     "ListWorkflowsResponseTypeDef",
     "TsvOptionsTypeDef",
     "StartReadSetActivationJobRequestRequestTypeDef",
     "StartReferenceImportJobRequestRequestTypeDef",
     "StartVariantImportRequestRequestTypeDef",
     "StoreOptionsOutputTypeDef",
     "StoreOptionsTypeDef",
+    "ListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef",
+    "ListReadSetActivationJobsRequestRequestTypeDef",
+    "ListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef",
+    "ListReadSetExportJobsRequestRequestTypeDef",
+    "ListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef",
+    "ListReadSetImportJobsRequestRequestTypeDef",
+    "ListReferenceImportJobsRequestListReferenceImportJobsPaginateTypeDef",
+    "ListReferenceImportJobsRequestRequestTypeDef",
+    "ListReadSetsRequestListReadSetsPaginateTypeDef",
+    "ListReadSetsRequestRequestTypeDef",
+    "ListReadSetUploadPartsRequestListReadSetUploadPartsPaginateTypeDef",
+    "ListReadSetUploadPartsRequestRequestTypeDef",
+    "ListReferencesRequestListReferencesPaginateTypeDef",
+    "ListReferencesRequestRequestTypeDef",
+    "ListReferenceStoresRequestListReferenceStoresPaginateTypeDef",
+    "ListReferenceStoresRequestRequestTypeDef",
+    "ListSequenceStoresRequestListSequenceStoresPaginateTypeDef",
+    "ListSequenceStoresRequestRequestTypeDef",
     "ListAnnotationStoresResponseTypeDef",
     "ListReferenceStoresResponseTypeDef",
     "ListSequenceStoresResponseTypeDef",
     "ListVariantStoresResponseTypeDef",
     "GetReadSetMetadataResponseTypeDef",
     "GetReferenceMetadataResponseTypeDef",
     "ListReadSetsResponseTypeDef",
     "GetReadSetImportJobResponseTypeDef",
     "StartReadSetImportJobRequestRequestTypeDef",
     "FormatOptionsTypeDef",
     "CreateAnnotationStoreResponseTypeDef",
     "GetAnnotationStoreResponseTypeDef",
     "UpdateAnnotationStoreResponseTypeDef",
     "CreateAnnotationStoreRequestRequestTypeDef",
+    "StoreOptionsUnionTypeDef",
     "GetAnnotationImportResponseTypeDef",
     "StartAnnotationImportRequestRequestTypeDef",
 )
 
 AbortMultipartReadSetUploadRequestRequestTypeDef = TypedDict(
     "AbortMultipartReadSetUploadRequestRequestTypeDef",
     {
         "sequenceStoreId": str,
         "uploadId": str,
     },
 )
 
-ActivateReadSetFilterTypeDef = TypedDict(
-    "ActivateReadSetFilterTypeDef",
-    {
-        "status": ReadSetActivationJobStatusType,
-        "createdAfter": Union[datetime, str],
-        "createdBefore": Union[datetime, str],
-    },
-    total=False,
-)
-
+TimestampTypeDef = Union[datetime, str]
 _RequiredActivateReadSetJobItemTypeDef = TypedDict(
     "_RequiredActivateReadSetJobItemTypeDef",
     {
         "id": str,
         "sequenceStoreId": str,
         "status": ReadSetActivationJobStatusType,
         "creationTime": datetime,
@@ -446,14 +440,15 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 CancelAnnotationImportRequestRequestTypeDef = TypedDict(
     "CancelAnnotationImportRequestRequestTypeDef",
     {
         "jobId": str,
     },
 )
 
@@ -650,24 +645,14 @@
 
 class ExportReadSetDetailTypeDef(
     _RequiredExportReadSetDetailTypeDef, _OptionalExportReadSetDetailTypeDef
 ):
     pass
 
 
-ExportReadSetFilterTypeDef = TypedDict(
-    "ExportReadSetFilterTypeDef",
-    {
-        "status": ReadSetExportJobStatusType,
-        "createdAfter": Union[datetime, str],
-        "createdBefore": Union[datetime, str],
-    },
-    total=False,
-)
-
 _RequiredExportReadSetJobDetailTypeDef = TypedDict(
     "_RequiredExportReadSetJobDetailTypeDef",
     {
         "id": str,
         "sequenceStoreId": str,
         "destination": str,
         "status": ReadSetExportJobStatusType,
@@ -973,24 +958,14 @@
 
 class GetWorkflowRequestRequestTypeDef(
     _RequiredGetWorkflowRequestRequestTypeDef, _OptionalGetWorkflowRequestRequestTypeDef
 ):
     pass
 
 
-ImportReadSetFilterTypeDef = TypedDict(
-    "ImportReadSetFilterTypeDef",
-    {
-        "status": ReadSetImportJobStatusType,
-        "createdAfter": Union[datetime, str],
-        "createdBefore": Union[datetime, str],
-    },
-    total=False,
-)
-
 _RequiredImportReadSetJobItemTypeDef = TypedDict(
     "_RequiredImportReadSetJobItemTypeDef",
     {
         "id": str,
         "sequenceStoreId": str,
         "roleArn": str,
         "status": ReadSetImportJobStatusType,
@@ -1027,24 +1002,14 @@
 )
 
 
 class SourceFilesTypeDef(_RequiredSourceFilesTypeDef, _OptionalSourceFilesTypeDef):
     pass
 
 
-ImportReferenceFilterTypeDef = TypedDict(
-    "ImportReferenceFilterTypeDef",
-    {
-        "status": ReferenceImportJobStatusType,
-        "createdAfter": Union[datetime, str],
-        "createdBefore": Union[datetime, str],
-    },
-    total=False,
-)
-
 _RequiredImportReferenceJobItemTypeDef = TypedDict(
     "_RequiredImportReferenceJobItemTypeDef",
     {
         "id": str,
         "referenceStoreId": str,
         "roleArn": str,
         "status": ReferenceImportJobStatusType,
@@ -1142,23 +1107,14 @@
 
 class MultipartReadSetUploadListItemTypeDef(
     _RequiredMultipartReadSetUploadListItemTypeDef, _OptionalMultipartReadSetUploadListItemTypeDef
 ):
     pass
 
 
-ReadSetUploadPartListFilterTypeDef = TypedDict(
-    "ReadSetUploadPartListFilterTypeDef",
-    {
-        "createdAfter": Union[datetime, str],
-        "createdBefore": Union[datetime, str],
-    },
-    total=False,
-)
-
 _RequiredReadSetUploadPartListItemTypeDef = TypedDict(
     "_RequiredReadSetUploadPartListItemTypeDef",
     {
         "partNumber": int,
         "partSize": int,
         "partSource": ReadSetPartSourceType,
         "checksum": str,
@@ -1176,51 +1132,14 @@
 
 class ReadSetUploadPartListItemTypeDef(
     _RequiredReadSetUploadPartListItemTypeDef, _OptionalReadSetUploadPartListItemTypeDef
 ):
     pass
 
 
-ReadSetFilterTypeDef = TypedDict(
-    "ReadSetFilterTypeDef",
-    {
-        "name": str,
-        "status": ReadSetStatusType,
-        "referenceArn": str,
-        "createdAfter": Union[datetime, str],
-        "createdBefore": Union[datetime, str],
-        "sampleId": str,
-        "subjectId": str,
-        "generatedFrom": str,
-        "creationType": CreationTypeType,
-    },
-    total=False,
-)
-
-ReferenceStoreFilterTypeDef = TypedDict(
-    "ReferenceStoreFilterTypeDef",
-    {
-        "name": str,
-        "createdAfter": Union[datetime, str],
-        "createdBefore": Union[datetime, str],
-    },
-    total=False,
-)
-
-ReferenceFilterTypeDef = TypedDict(
-    "ReferenceFilterTypeDef",
-    {
-        "name": str,
-        "md5": str,
-        "createdAfter": Union[datetime, str],
-        "createdBefore": Union[datetime, str],
-    },
-    total=False,
-)
-
 _RequiredReferenceListItemTypeDef = TypedDict(
     "_RequiredReferenceListItemTypeDef",
     {
         "id": str,
         "arn": str,
         "referenceStoreId": str,
         "md5": str,
@@ -1334,24 +1253,14 @@
         "creationTime": datetime,
         "startTime": datetime,
         "stopTime": datetime,
     },
     total=False,
 )
 
-SequenceStoreFilterTypeDef = TypedDict(
-    "SequenceStoreFilterTypeDef",
-    {
-        "name": str,
-        "createdAfter": Union[datetime, str],
-        "createdBefore": Union[datetime, str],
-    },
-    total=False,
-)
-
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
@@ -1635,48 +1544,109 @@
 
 class UpdateWorkflowRequestRequestTypeDef(
     _RequiredUpdateWorkflowRequestRequestTypeDef, _OptionalUpdateWorkflowRequestRequestTypeDef
 ):
     pass
 
 
-UploadReadSetPartRequestRequestTypeDef = TypedDict(
-    "UploadReadSetPartRequestRequestTypeDef",
+ActivateReadSetFilterTypeDef = TypedDict(
+    "ActivateReadSetFilterTypeDef",
     {
-        "sequenceStoreId": str,
-        "uploadId": str,
-        "partSource": ReadSetPartSourceType,
-        "partNumber": int,
-        "payload": Union[str, bytes, IO[Any], StreamingBody],
+        "status": ReadSetActivationJobStatusType,
+        "createdAfter": TimestampTypeDef,
+        "createdBefore": TimestampTypeDef,
     },
+    total=False,
 )
 
-_RequiredListReadSetActivationJobsRequestRequestTypeDef = TypedDict(
-    "_RequiredListReadSetActivationJobsRequestRequestTypeDef",
+ExportReadSetFilterTypeDef = TypedDict(
+    "ExportReadSetFilterTypeDef",
     {
-        "sequenceStoreId": str,
+        "status": ReadSetExportJobStatusType,
+        "createdAfter": TimestampTypeDef,
+        "createdBefore": TimestampTypeDef,
     },
+    total=False,
 )
-_OptionalListReadSetActivationJobsRequestRequestTypeDef = TypedDict(
-    "_OptionalListReadSetActivationJobsRequestRequestTypeDef",
+
+ImportReadSetFilterTypeDef = TypedDict(
+    "ImportReadSetFilterTypeDef",
     {
-        "maxResults": int,
-        "nextToken": str,
-        "filter": ActivateReadSetFilterTypeDef,
+        "status": ReadSetImportJobStatusType,
+        "createdAfter": TimestampTypeDef,
+        "createdBefore": TimestampTypeDef,
     },
     total=False,
 )
 
+ImportReferenceFilterTypeDef = TypedDict(
+    "ImportReferenceFilterTypeDef",
+    {
+        "status": ReferenceImportJobStatusType,
+        "createdAfter": TimestampTypeDef,
+        "createdBefore": TimestampTypeDef,
+    },
+    total=False,
+)
 
-class ListReadSetActivationJobsRequestRequestTypeDef(
-    _RequiredListReadSetActivationJobsRequestRequestTypeDef,
-    _OptionalListReadSetActivationJobsRequestRequestTypeDef,
-):
-    pass
+ReadSetFilterTypeDef = TypedDict(
+    "ReadSetFilterTypeDef",
+    {
+        "name": str,
+        "status": ReadSetStatusType,
+        "referenceArn": str,
+        "createdAfter": TimestampTypeDef,
+        "createdBefore": TimestampTypeDef,
+        "sampleId": str,
+        "subjectId": str,
+        "generatedFrom": str,
+        "creationType": CreationTypeType,
+    },
+    total=False,
+)
 
+ReadSetUploadPartListFilterTypeDef = TypedDict(
+    "ReadSetUploadPartListFilterTypeDef",
+    {
+        "createdAfter": TimestampTypeDef,
+        "createdBefore": TimestampTypeDef,
+    },
+    total=False,
+)
+
+ReferenceFilterTypeDef = TypedDict(
+    "ReferenceFilterTypeDef",
+    {
+        "name": str,
+        "md5": str,
+        "createdAfter": TimestampTypeDef,
+        "createdBefore": TimestampTypeDef,
+    },
+    total=False,
+)
+
+ReferenceStoreFilterTypeDef = TypedDict(
+    "ReferenceStoreFilterTypeDef",
+    {
+        "name": str,
+        "createdAfter": TimestampTypeDef,
+        "createdBefore": TimestampTypeDef,
+    },
+    total=False,
+)
+
+SequenceStoreFilterTypeDef = TypedDict(
+    "SequenceStoreFilterTypeDef",
+    {
+        "name": str,
+        "createdAfter": TimestampTypeDef,
+        "createdBefore": TimestampTypeDef,
+    },
+    total=False,
+)
 
 AnnotationStoreItemTypeDef = TypedDict(
     "AnnotationStoreItemTypeDef",
     {
         "id": str,
         "reference": ReferenceItemTypeDef,
         "status": StoreStatusType,
@@ -2212,14 +2182,25 @@
     "UploadReadSetPartResponseTypeDef",
     {
         "checksum": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+UploadReadSetPartRequestRequestTypeDef = TypedDict(
+    "UploadReadSetPartRequestRequestTypeDef",
+    {
+        "sequenceStoreId": str,
+        "uploadId": str,
+        "partSource": ReadSetPartSourceType,
+        "partNumber": int,
+        "payload": BlobTypeDef,
+    },
+)
+
 CompleteMultipartReadSetUploadRequestRequestTypeDef = TypedDict(
     "CompleteMultipartReadSetUploadRequestRequestTypeDef",
     {
         "sequenceStoreId": str,
         "uploadId": str,
         "parts": Sequence[CompleteReadSetUploadPartListItemTypeDef],
     },
@@ -2233,15 +2214,15 @@
 )
 _OptionalCreateWorkflowRequestRequestTypeDef = TypedDict(
     "_OptionalCreateWorkflowRequestRequestTypeDef",
     {
         "name": str,
         "description": str,
         "engine": WorkflowEngineType,
-        "definitionZip": Union[str, bytes, IO[Any], StreamingBody],
+        "definitionZip": BlobTypeDef,
         "definitionUri": str,
         "main": str,
         "parameterTemplate": Mapping[str, WorkflowParameterTypeDef],
         "storageCapacity": int,
         "tags": Mapping[str, str],
         "accelerators": Literal["GPU"],
     },
@@ -2290,38 +2271,14 @@
         "creationTime": datetime,
         "completionTime": datetime,
         "readSets": List[ExportReadSetDetailTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredListReadSetExportJobsRequestRequestTypeDef = TypedDict(
-    "_RequiredListReadSetExportJobsRequestRequestTypeDef",
-    {
-        "sequenceStoreId": str,
-    },
-)
-_OptionalListReadSetExportJobsRequestRequestTypeDef = TypedDict(
-    "_OptionalListReadSetExportJobsRequestRequestTypeDef",
-    {
-        "maxResults": int,
-        "nextToken": str,
-        "filter": ExportReadSetFilterTypeDef,
-    },
-    total=False,
-)
-
-
-class ListReadSetExportJobsRequestRequestTypeDef(
-    _RequiredListReadSetExportJobsRequestRequestTypeDef,
-    _OptionalListReadSetExportJobsRequestRequestTypeDef,
-):
-    pass
-
-
 ListReadSetExportJobsResponseTypeDef = TypedDict(
     "ListReadSetExportJobsResponseTypeDef",
     {
         "nextToken": str,
         "exportJobs": List[ExportReadSetJobDetailTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2769,38 +2726,14 @@
         "items": List[VariantImportItemDetailTypeDef],
         "runLeftNormalization": bool,
         "annotationFields": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredListReadSetImportJobsRequestRequestTypeDef = TypedDict(
-    "_RequiredListReadSetImportJobsRequestRequestTypeDef",
-    {
-        "sequenceStoreId": str,
-    },
-)
-_OptionalListReadSetImportJobsRequestRequestTypeDef = TypedDict(
-    "_OptionalListReadSetImportJobsRequestRequestTypeDef",
-    {
-        "maxResults": int,
-        "nextToken": str,
-        "filter": ImportReadSetFilterTypeDef,
-    },
-    total=False,
-)
-
-
-class ListReadSetImportJobsRequestRequestTypeDef(
-    _RequiredListReadSetImportJobsRequestRequestTypeDef,
-    _OptionalListReadSetImportJobsRequestRequestTypeDef,
-):
-    pass
-
-
 ListReadSetImportJobsResponseTypeDef = TypedDict(
     "ListReadSetImportJobsResponseTypeDef",
     {
         "nextToken": str,
         "importJobs": List[ImportReadSetJobItemTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2860,38 +2793,14 @@
 
 class StartReadSetImportJobSourceItemTypeDef(
     _RequiredStartReadSetImportJobSourceItemTypeDef, _OptionalStartReadSetImportJobSourceItemTypeDef
 ):
     pass
 
 
-_RequiredListReferenceImportJobsRequestRequestTypeDef = TypedDict(
-    "_RequiredListReferenceImportJobsRequestRequestTypeDef",
-    {
-        "referenceStoreId": str,
-    },
-)
-_OptionalListReferenceImportJobsRequestRequestTypeDef = TypedDict(
-    "_OptionalListReferenceImportJobsRequestRequestTypeDef",
-    {
-        "maxResults": int,
-        "nextToken": str,
-        "filter": ImportReferenceFilterTypeDef,
-    },
-    total=False,
-)
-
-
-class ListReferenceImportJobsRequestRequestTypeDef(
-    _RequiredListReferenceImportJobsRequestRequestTypeDef,
-    _OptionalListReferenceImportJobsRequestRequestTypeDef,
-):
-    pass
-
-
 ListReferenceImportJobsResponseTypeDef = TypedDict(
     "ListReferenceImportJobsResponseTypeDef",
     {
         "nextToken": str,
         "importJobs": List[ImportReferenceJobItemTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2936,106 +2845,14 @@
 class ListMultipartReadSetUploadsRequestListMultipartReadSetUploadsPaginateTypeDef(
     _RequiredListMultipartReadSetUploadsRequestListMultipartReadSetUploadsPaginateTypeDef,
     _OptionalListMultipartReadSetUploadsRequestListMultipartReadSetUploadsPaginateTypeDef,
 ):
     pass
 
 
-_RequiredListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef = TypedDict(
-    "_RequiredListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef",
-    {
-        "sequenceStoreId": str,
-    },
-)
-_OptionalListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef = TypedDict(
-    "_OptionalListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef",
-    {
-        "filter": ActivateReadSetFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef(
-    _RequiredListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef,
-    _OptionalListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef = TypedDict(
-    "_RequiredListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef",
-    {
-        "sequenceStoreId": str,
-    },
-)
-_OptionalListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef = TypedDict(
-    "_OptionalListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef",
-    {
-        "filter": ExportReadSetFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef(
-    _RequiredListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef,
-    _OptionalListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef = TypedDict(
-    "_RequiredListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef",
-    {
-        "sequenceStoreId": str,
-    },
-)
-_OptionalListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef = TypedDict(
-    "_OptionalListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef",
-    {
-        "filter": ImportReadSetFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef(
-    _RequiredListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef,
-    _OptionalListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListReferenceImportJobsRequestListReferenceImportJobsPaginateTypeDef = TypedDict(
-    "_RequiredListReferenceImportJobsRequestListReferenceImportJobsPaginateTypeDef",
-    {
-        "referenceStoreId": str,
-    },
-)
-_OptionalListReferenceImportJobsRequestListReferenceImportJobsPaginateTypeDef = TypedDict(
-    "_OptionalListReferenceImportJobsRequestListReferenceImportJobsPaginateTypeDef",
-    {
-        "filter": ImportReferenceFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListReferenceImportJobsRequestListReferenceImportJobsPaginateTypeDef(
-    _RequiredListReferenceImportJobsRequestListReferenceImportJobsPaginateTypeDef,
-    _OptionalListReferenceImportJobsRequestListReferenceImportJobsPaginateTypeDef,
-):
-    pass
-
-
 ListRunGroupsRequestListRunGroupsPaginateTypeDef = TypedDict(
     "ListRunGroupsRequestListRunGroupsPaginateTypeDef",
     {
         "name": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -3111,392 +2928,580 @@
     {
         "nextToken": str,
         "uploads": List[MultipartReadSetUploadListItemTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredListReadSetUploadPartsRequestListReadSetUploadPartsPaginateTypeDef = TypedDict(
-    "_RequiredListReadSetUploadPartsRequestListReadSetUploadPartsPaginateTypeDef",
+ListReadSetUploadPartsResponseTypeDef = TypedDict(
+    "ListReadSetUploadPartsResponseTypeDef",
     {
-        "sequenceStoreId": str,
-        "uploadId": str,
-        "partSource": ReadSetPartSourceType,
+        "nextToken": str,
+        "parts": List[ReadSetUploadPartListItemTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalListReadSetUploadPartsRequestListReadSetUploadPartsPaginateTypeDef = TypedDict(
-    "_OptionalListReadSetUploadPartsRequestListReadSetUploadPartsPaginateTypeDef",
+
+ListReferencesResponseTypeDef = TypedDict(
+    "ListReferencesResponseTypeDef",
     {
-        "filter": ReadSetUploadPartListFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "nextToken": str,
+        "references": List[ReferenceListItemTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
+ListRunGroupsResponseTypeDef = TypedDict(
+    "ListRunGroupsResponseTypeDef",
+    {
+        "items": List[RunGroupListItemTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class ListReadSetUploadPartsRequestListReadSetUploadPartsPaginateTypeDef(
-    _RequiredListReadSetUploadPartsRequestListReadSetUploadPartsPaginateTypeDef,
-    _OptionalListReadSetUploadPartsRequestListReadSetUploadPartsPaginateTypeDef,
-):
-    pass
+ListRunTasksResponseTypeDef = TypedDict(
+    "ListRunTasksResponseTypeDef",
+    {
+        "items": List[TaskListItemTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
+ListRunsResponseTypeDef = TypedDict(
+    "ListRunsResponseTypeDef",
+    {
+        "items": List[RunListItemTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-_RequiredListReadSetUploadPartsRequestRequestTypeDef = TypedDict(
-    "_RequiredListReadSetUploadPartsRequestRequestTypeDef",
+ListVariantImportJobsRequestListVariantImportJobsPaginateTypeDef = TypedDict(
+    "ListVariantImportJobsRequestListVariantImportJobsPaginateTypeDef",
     {
-        "sequenceStoreId": str,
-        "uploadId": str,
-        "partSource": ReadSetPartSourceType,
+        "ids": Sequence[str],
+        "filter": ListVariantImportJobsFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
-_OptionalListReadSetUploadPartsRequestRequestTypeDef = TypedDict(
-    "_OptionalListReadSetUploadPartsRequestRequestTypeDef",
+
+ListVariantImportJobsRequestRequestTypeDef = TypedDict(
+    "ListVariantImportJobsRequestRequestTypeDef",
     {
         "maxResults": int,
+        "ids": Sequence[str],
         "nextToken": str,
-        "filter": ReadSetUploadPartListFilterTypeDef,
+        "filter": ListVariantImportJobsFilterTypeDef,
     },
     total=False,
 )
 
+ListVariantImportJobsResponseTypeDef = TypedDict(
+    "ListVariantImportJobsResponseTypeDef",
+    {
+        "variantImportJobs": List[VariantImportJobItemTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class ListReadSetUploadPartsRequestRequestTypeDef(
-    _RequiredListReadSetUploadPartsRequestRequestTypeDef,
-    _OptionalListReadSetUploadPartsRequestRequestTypeDef,
-):
-    pass
+ListVariantStoresRequestListVariantStoresPaginateTypeDef = TypedDict(
+    "ListVariantStoresRequestListVariantStoresPaginateTypeDef",
+    {
+        "ids": Sequence[str],
+        "filter": ListVariantStoresFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
 
+ListVariantStoresRequestRequestTypeDef = TypedDict(
+    "ListVariantStoresRequestRequestTypeDef",
+    {
+        "maxResults": int,
+        "ids": Sequence[str],
+        "nextToken": str,
+        "filter": ListVariantStoresFilterTypeDef,
+    },
+    total=False,
+)
 
-ListReadSetUploadPartsResponseTypeDef = TypedDict(
-    "ListReadSetUploadPartsResponseTypeDef",
+ListWorkflowsResponseTypeDef = TypedDict(
+    "ListWorkflowsResponseTypeDef",
     {
+        "items": List[WorkflowListItemTypeDef],
         "nextToken": str,
-        "parts": List[ReadSetUploadPartListItemTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredListReadSetsRequestListReadSetsPaginateTypeDef = TypedDict(
-    "_RequiredListReadSetsRequestListReadSetsPaginateTypeDef",
+TsvOptionsTypeDef = TypedDict(
+    "TsvOptionsTypeDef",
+    {
+        "readOptions": ReadOptionsTypeDef,
+    },
+    total=False,
+)
+
+_RequiredStartReadSetActivationJobRequestRequestTypeDef = TypedDict(
+    "_RequiredStartReadSetActivationJobRequestRequestTypeDef",
     {
         "sequenceStoreId": str,
+        "sources": Sequence[StartReadSetActivationJobSourceItemTypeDef],
     },
 )
-_OptionalListReadSetsRequestListReadSetsPaginateTypeDef = TypedDict(
-    "_OptionalListReadSetsRequestListReadSetsPaginateTypeDef",
+_OptionalStartReadSetActivationJobRequestRequestTypeDef = TypedDict(
+    "_OptionalStartReadSetActivationJobRequestRequestTypeDef",
     {
-        "filter": ReadSetFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "clientToken": str,
     },
     total=False,
 )
 
 
-class ListReadSetsRequestListReadSetsPaginateTypeDef(
-    _RequiredListReadSetsRequestListReadSetsPaginateTypeDef,
-    _OptionalListReadSetsRequestListReadSetsPaginateTypeDef,
+class StartReadSetActivationJobRequestRequestTypeDef(
+    _RequiredStartReadSetActivationJobRequestRequestTypeDef,
+    _OptionalStartReadSetActivationJobRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredListReadSetsRequestRequestTypeDef = TypedDict(
-    "_RequiredListReadSetsRequestRequestTypeDef",
+_RequiredStartReferenceImportJobRequestRequestTypeDef = TypedDict(
+    "_RequiredStartReferenceImportJobRequestRequestTypeDef",
     {
-        "sequenceStoreId": str,
+        "referenceStoreId": str,
+        "roleArn": str,
+        "sources": Sequence[StartReferenceImportJobSourceItemTypeDef],
     },
 )
-_OptionalListReadSetsRequestRequestTypeDef = TypedDict(
-    "_OptionalListReadSetsRequestRequestTypeDef",
+_OptionalStartReferenceImportJobRequestRequestTypeDef = TypedDict(
+    "_OptionalStartReferenceImportJobRequestRequestTypeDef",
     {
-        "maxResults": int,
-        "nextToken": str,
-        "filter": ReadSetFilterTypeDef,
+        "clientToken": str,
     },
     total=False,
 )
 
 
-class ListReadSetsRequestRequestTypeDef(
-    _RequiredListReadSetsRequestRequestTypeDef, _OptionalListReadSetsRequestRequestTypeDef
+class StartReferenceImportJobRequestRequestTypeDef(
+    _RequiredStartReferenceImportJobRequestRequestTypeDef,
+    _OptionalStartReferenceImportJobRequestRequestTypeDef,
 ):
     pass
 
 
-ListReferenceStoresRequestListReferenceStoresPaginateTypeDef = TypedDict(
-    "ListReferenceStoresRequestListReferenceStoresPaginateTypeDef",
+_RequiredStartVariantImportRequestRequestTypeDef = TypedDict(
+    "_RequiredStartVariantImportRequestRequestTypeDef",
     {
-        "filter": ReferenceStoreFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "destinationName": str,
+        "roleArn": str,
+        "items": Sequence[VariantImportItemSourceTypeDef],
+    },
+)
+_OptionalStartVariantImportRequestRequestTypeDef = TypedDict(
+    "_OptionalStartVariantImportRequestRequestTypeDef",
+    {
+        "runLeftNormalization": bool,
+        "annotationFields": Mapping[str, str],
     },
     total=False,
 )
 
-ListReferenceStoresRequestRequestTypeDef = TypedDict(
-    "ListReferenceStoresRequestRequestTypeDef",
+
+class StartVariantImportRequestRequestTypeDef(
+    _RequiredStartVariantImportRequestRequestTypeDef,
+    _OptionalStartVariantImportRequestRequestTypeDef,
+):
+    pass
+
+
+StoreOptionsOutputTypeDef = TypedDict(
+    "StoreOptionsOutputTypeDef",
     {
-        "maxResults": int,
-        "nextToken": str,
-        "filter": ReferenceStoreFilterTypeDef,
+        "tsvStoreOptions": TsvStoreOptionsOutputTypeDef,
     },
     total=False,
 )
 
-_RequiredListReferencesRequestListReferencesPaginateTypeDef = TypedDict(
-    "_RequiredListReferencesRequestListReferencesPaginateTypeDef",
+StoreOptionsTypeDef = TypedDict(
+    "StoreOptionsTypeDef",
     {
-        "referenceStoreId": str,
+        "tsvStoreOptions": TsvStoreOptionsTypeDef,
     },
+    total=False,
 )
-_OptionalListReferencesRequestListReferencesPaginateTypeDef = TypedDict(
-    "_OptionalListReferencesRequestListReferencesPaginateTypeDef",
+
+_RequiredListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef = TypedDict(
+    "_RequiredListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef",
     {
-        "filter": ReferenceFilterTypeDef,
+        "sequenceStoreId": str,
+    },
+)
+_OptionalListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef = TypedDict(
+    "_OptionalListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef",
+    {
+        "filter": ActivateReadSetFilterTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
-class ListReferencesRequestListReferencesPaginateTypeDef(
-    _RequiredListReferencesRequestListReferencesPaginateTypeDef,
-    _OptionalListReferencesRequestListReferencesPaginateTypeDef,
+class ListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef(
+    _RequiredListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef,
+    _OptionalListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef,
 ):
     pass
 
 
-_RequiredListReferencesRequestRequestTypeDef = TypedDict(
-    "_RequiredListReferencesRequestRequestTypeDef",
+_RequiredListReadSetActivationJobsRequestRequestTypeDef = TypedDict(
+    "_RequiredListReadSetActivationJobsRequestRequestTypeDef",
     {
-        "referenceStoreId": str,
+        "sequenceStoreId": str,
     },
 )
-_OptionalListReferencesRequestRequestTypeDef = TypedDict(
-    "_OptionalListReferencesRequestRequestTypeDef",
+_OptionalListReadSetActivationJobsRequestRequestTypeDef = TypedDict(
+    "_OptionalListReadSetActivationJobsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
-        "filter": ReferenceFilterTypeDef,
+        "filter": ActivateReadSetFilterTypeDef,
     },
     total=False,
 )
 
 
-class ListReferencesRequestRequestTypeDef(
-    _RequiredListReferencesRequestRequestTypeDef, _OptionalListReferencesRequestRequestTypeDef
+class ListReadSetActivationJobsRequestRequestTypeDef(
+    _RequiredListReadSetActivationJobsRequestRequestTypeDef,
+    _OptionalListReadSetActivationJobsRequestRequestTypeDef,
 ):
     pass
 
 
-ListReferencesResponseTypeDef = TypedDict(
-    "ListReferencesResponseTypeDef",
+_RequiredListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef = TypedDict(
+    "_RequiredListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef",
     {
-        "nextToken": str,
-        "references": List[ReferenceListItemTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "sequenceStoreId": str,
     },
 )
-
-ListRunGroupsResponseTypeDef = TypedDict(
-    "ListRunGroupsResponseTypeDef",
+_OptionalListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef = TypedDict(
+    "_OptionalListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef",
     {
-        "items": List[RunGroupListItemTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "filter": ExportReadSetFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-ListRunTasksResponseTypeDef = TypedDict(
-    "ListRunTasksResponseTypeDef",
+
+class ListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef(
+    _RequiredListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef,
+    _OptionalListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListReadSetExportJobsRequestRequestTypeDef = TypedDict(
+    "_RequiredListReadSetExportJobsRequestRequestTypeDef",
     {
-        "items": List[TaskListItemTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "sequenceStoreId": str,
     },
 )
-
-ListRunsResponseTypeDef = TypedDict(
-    "ListRunsResponseTypeDef",
+_OptionalListReadSetExportJobsRequestRequestTypeDef = TypedDict(
+    "_OptionalListReadSetExportJobsRequestRequestTypeDef",
     {
-        "items": List[RunListItemTypeDef],
+        "maxResults": int,
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "filter": ExportReadSetFilterTypeDef,
     },
+    total=False,
 )
 
-ListSequenceStoresRequestListSequenceStoresPaginateTypeDef = TypedDict(
-    "ListSequenceStoresRequestListSequenceStoresPaginateTypeDef",
+
+class ListReadSetExportJobsRequestRequestTypeDef(
+    _RequiredListReadSetExportJobsRequestRequestTypeDef,
+    _OptionalListReadSetExportJobsRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef = TypedDict(
+    "_RequiredListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef",
     {
-        "filter": SequenceStoreFilterTypeDef,
+        "sequenceStoreId": str,
+    },
+)
+_OptionalListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef = TypedDict(
+    "_OptionalListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef",
+    {
+        "filter": ImportReadSetFilterTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListSequenceStoresRequestRequestTypeDef = TypedDict(
-    "ListSequenceStoresRequestRequestTypeDef",
+
+class ListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef(
+    _RequiredListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef,
+    _OptionalListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListReadSetImportJobsRequestRequestTypeDef = TypedDict(
+    "_RequiredListReadSetImportJobsRequestRequestTypeDef",
+    {
+        "sequenceStoreId": str,
+    },
+)
+_OptionalListReadSetImportJobsRequestRequestTypeDef = TypedDict(
+    "_OptionalListReadSetImportJobsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
-        "filter": SequenceStoreFilterTypeDef,
+        "filter": ImportReadSetFilterTypeDef,
     },
     total=False,
 )
 
-ListVariantImportJobsRequestListVariantImportJobsPaginateTypeDef = TypedDict(
-    "ListVariantImportJobsRequestListVariantImportJobsPaginateTypeDef",
+
+class ListReadSetImportJobsRequestRequestTypeDef(
+    _RequiredListReadSetImportJobsRequestRequestTypeDef,
+    _OptionalListReadSetImportJobsRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredListReferenceImportJobsRequestListReferenceImportJobsPaginateTypeDef = TypedDict(
+    "_RequiredListReferenceImportJobsRequestListReferenceImportJobsPaginateTypeDef",
     {
-        "ids": Sequence[str],
-        "filter": ListVariantImportJobsFilterTypeDef,
+        "referenceStoreId": str,
+    },
+)
+_OptionalListReferenceImportJobsRequestListReferenceImportJobsPaginateTypeDef = TypedDict(
+    "_OptionalListReferenceImportJobsRequestListReferenceImportJobsPaginateTypeDef",
+    {
+        "filter": ImportReferenceFilterTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListVariantImportJobsRequestRequestTypeDef = TypedDict(
-    "ListVariantImportJobsRequestRequestTypeDef",
+
+class ListReferenceImportJobsRequestListReferenceImportJobsPaginateTypeDef(
+    _RequiredListReferenceImportJobsRequestListReferenceImportJobsPaginateTypeDef,
+    _OptionalListReferenceImportJobsRequestListReferenceImportJobsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListReferenceImportJobsRequestRequestTypeDef = TypedDict(
+    "_RequiredListReferenceImportJobsRequestRequestTypeDef",
+    {
+        "referenceStoreId": str,
+    },
+)
+_OptionalListReferenceImportJobsRequestRequestTypeDef = TypedDict(
+    "_OptionalListReferenceImportJobsRequestRequestTypeDef",
     {
         "maxResults": int,
-        "ids": Sequence[str],
         "nextToken": str,
-        "filter": ListVariantImportJobsFilterTypeDef,
+        "filter": ImportReferenceFilterTypeDef,
     },
     total=False,
 )
 
-ListVariantImportJobsResponseTypeDef = TypedDict(
-    "ListVariantImportJobsResponseTypeDef",
+
+class ListReferenceImportJobsRequestRequestTypeDef(
+    _RequiredListReferenceImportJobsRequestRequestTypeDef,
+    _OptionalListReferenceImportJobsRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredListReadSetsRequestListReadSetsPaginateTypeDef = TypedDict(
+    "_RequiredListReadSetsRequestListReadSetsPaginateTypeDef",
     {
-        "variantImportJobs": List[VariantImportJobItemTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "sequenceStoreId": str,
     },
 )
-
-ListVariantStoresRequestListVariantStoresPaginateTypeDef = TypedDict(
-    "ListVariantStoresRequestListVariantStoresPaginateTypeDef",
+_OptionalListReadSetsRequestListReadSetsPaginateTypeDef = TypedDict(
+    "_OptionalListReadSetsRequestListReadSetsPaginateTypeDef",
     {
-        "ids": Sequence[str],
-        "filter": ListVariantStoresFilterTypeDef,
+        "filter": ReadSetFilterTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListVariantStoresRequestRequestTypeDef = TypedDict(
-    "ListVariantStoresRequestRequestTypeDef",
+
+class ListReadSetsRequestListReadSetsPaginateTypeDef(
+    _RequiredListReadSetsRequestListReadSetsPaginateTypeDef,
+    _OptionalListReadSetsRequestListReadSetsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListReadSetsRequestRequestTypeDef = TypedDict(
+    "_RequiredListReadSetsRequestRequestTypeDef",
+    {
+        "sequenceStoreId": str,
+    },
+)
+_OptionalListReadSetsRequestRequestTypeDef = TypedDict(
+    "_OptionalListReadSetsRequestRequestTypeDef",
     {
         "maxResults": int,
-        "ids": Sequence[str],
         "nextToken": str,
-        "filter": ListVariantStoresFilterTypeDef,
+        "filter": ReadSetFilterTypeDef,
     },
     total=False,
 )
 
-ListWorkflowsResponseTypeDef = TypedDict(
-    "ListWorkflowsResponseTypeDef",
+
+class ListReadSetsRequestRequestTypeDef(
+    _RequiredListReadSetsRequestRequestTypeDef, _OptionalListReadSetsRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredListReadSetUploadPartsRequestListReadSetUploadPartsPaginateTypeDef = TypedDict(
+    "_RequiredListReadSetUploadPartsRequestListReadSetUploadPartsPaginateTypeDef",
     {
-        "items": List[WorkflowListItemTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "sequenceStoreId": str,
+        "uploadId": str,
+        "partSource": ReadSetPartSourceType,
     },
 )
-
-TsvOptionsTypeDef = TypedDict(
-    "TsvOptionsTypeDef",
+_OptionalListReadSetUploadPartsRequestListReadSetUploadPartsPaginateTypeDef = TypedDict(
+    "_OptionalListReadSetUploadPartsRequestListReadSetUploadPartsPaginateTypeDef",
     {
-        "readOptions": ReadOptionsTypeDef,
+        "filter": ReadSetUploadPartListFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-_RequiredStartReadSetActivationJobRequestRequestTypeDef = TypedDict(
-    "_RequiredStartReadSetActivationJobRequestRequestTypeDef",
+
+class ListReadSetUploadPartsRequestListReadSetUploadPartsPaginateTypeDef(
+    _RequiredListReadSetUploadPartsRequestListReadSetUploadPartsPaginateTypeDef,
+    _OptionalListReadSetUploadPartsRequestListReadSetUploadPartsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListReadSetUploadPartsRequestRequestTypeDef = TypedDict(
+    "_RequiredListReadSetUploadPartsRequestRequestTypeDef",
     {
         "sequenceStoreId": str,
-        "sources": Sequence[StartReadSetActivationJobSourceItemTypeDef],
+        "uploadId": str,
+        "partSource": ReadSetPartSourceType,
     },
 )
-_OptionalStartReadSetActivationJobRequestRequestTypeDef = TypedDict(
-    "_OptionalStartReadSetActivationJobRequestRequestTypeDef",
+_OptionalListReadSetUploadPartsRequestRequestTypeDef = TypedDict(
+    "_OptionalListReadSetUploadPartsRequestRequestTypeDef",
     {
-        "clientToken": str,
+        "maxResults": int,
+        "nextToken": str,
+        "filter": ReadSetUploadPartListFilterTypeDef,
     },
     total=False,
 )
 
 
-class StartReadSetActivationJobRequestRequestTypeDef(
-    _RequiredStartReadSetActivationJobRequestRequestTypeDef,
-    _OptionalStartReadSetActivationJobRequestRequestTypeDef,
+class ListReadSetUploadPartsRequestRequestTypeDef(
+    _RequiredListReadSetUploadPartsRequestRequestTypeDef,
+    _OptionalListReadSetUploadPartsRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredStartReferenceImportJobRequestRequestTypeDef = TypedDict(
-    "_RequiredStartReferenceImportJobRequestRequestTypeDef",
+_RequiredListReferencesRequestListReferencesPaginateTypeDef = TypedDict(
+    "_RequiredListReferencesRequestListReferencesPaginateTypeDef",
     {
         "referenceStoreId": str,
-        "roleArn": str,
-        "sources": Sequence[StartReferenceImportJobSourceItemTypeDef],
     },
 )
-_OptionalStartReferenceImportJobRequestRequestTypeDef = TypedDict(
-    "_OptionalStartReferenceImportJobRequestRequestTypeDef",
+_OptionalListReferencesRequestListReferencesPaginateTypeDef = TypedDict(
+    "_OptionalListReferencesRequestListReferencesPaginateTypeDef",
     {
-        "clientToken": str,
+        "filter": ReferenceFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
-class StartReferenceImportJobRequestRequestTypeDef(
-    _RequiredStartReferenceImportJobRequestRequestTypeDef,
-    _OptionalStartReferenceImportJobRequestRequestTypeDef,
+class ListReferencesRequestListReferencesPaginateTypeDef(
+    _RequiredListReferencesRequestListReferencesPaginateTypeDef,
+    _OptionalListReferencesRequestListReferencesPaginateTypeDef,
 ):
     pass
 
 
-_RequiredStartVariantImportRequestRequestTypeDef = TypedDict(
-    "_RequiredStartVariantImportRequestRequestTypeDef",
+_RequiredListReferencesRequestRequestTypeDef = TypedDict(
+    "_RequiredListReferencesRequestRequestTypeDef",
     {
-        "destinationName": str,
-        "roleArn": str,
-        "items": Sequence[VariantImportItemSourceTypeDef],
+        "referenceStoreId": str,
     },
 )
-_OptionalStartVariantImportRequestRequestTypeDef = TypedDict(
-    "_OptionalStartVariantImportRequestRequestTypeDef",
+_OptionalListReferencesRequestRequestTypeDef = TypedDict(
+    "_OptionalListReferencesRequestRequestTypeDef",
     {
-        "runLeftNormalization": bool,
-        "annotationFields": Mapping[str, str],
+        "maxResults": int,
+        "nextToken": str,
+        "filter": ReferenceFilterTypeDef,
     },
     total=False,
 )
 
 
-class StartVariantImportRequestRequestTypeDef(
-    _RequiredStartVariantImportRequestRequestTypeDef,
-    _OptionalStartVariantImportRequestRequestTypeDef,
+class ListReferencesRequestRequestTypeDef(
+    _RequiredListReferencesRequestRequestTypeDef, _OptionalListReferencesRequestRequestTypeDef
 ):
     pass
 
 
-StoreOptionsOutputTypeDef = TypedDict(
-    "StoreOptionsOutputTypeDef",
+ListReferenceStoresRequestListReferenceStoresPaginateTypeDef = TypedDict(
+    "ListReferenceStoresRequestListReferenceStoresPaginateTypeDef",
     {
-        "tsvStoreOptions": TsvStoreOptionsOutputTypeDef,
+        "filter": ReferenceStoreFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-StoreOptionsTypeDef = TypedDict(
-    "StoreOptionsTypeDef",
+ListReferenceStoresRequestRequestTypeDef = TypedDict(
+    "ListReferenceStoresRequestRequestTypeDef",
     {
-        "tsvStoreOptions": TsvStoreOptionsTypeDef,
+        "maxResults": int,
+        "nextToken": str,
+        "filter": ReferenceStoreFilterTypeDef,
+    },
+    total=False,
+)
+
+ListSequenceStoresRequestListSequenceStoresPaginateTypeDef = TypedDict(
+    "ListSequenceStoresRequestListSequenceStoresPaginateTypeDef",
+    {
+        "filter": SequenceStoreFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListSequenceStoresRequestRequestTypeDef = TypedDict(
+    "ListSequenceStoresRequestRequestTypeDef",
+    {
+        "maxResults": int,
+        "nextToken": str,
+        "filter": SequenceStoreFilterTypeDef,
     },
     total=False,
 )
 
 ListAnnotationStoresResponseTypeDef = TypedDict(
     "ListAnnotationStoresResponseTypeDef",
     {
@@ -3703,14 +3708,15 @@
 class CreateAnnotationStoreRequestRequestTypeDef(
     _RequiredCreateAnnotationStoreRequestRequestTypeDef,
     _OptionalCreateAnnotationStoreRequestRequestTypeDef,
 ):
     pass
 
 
+StoreOptionsUnionTypeDef = Union[StoreOptionsTypeDef, StoreOptionsOutputTypeDef]
 GetAnnotationImportResponseTypeDef = TypedDict(
     "GetAnnotationImportResponseTypeDef",
     {
         "id": str,
         "destinationName": str,
         "roleArn": str,
         "status": JobStatusType,
```

### Comparing `mypy-boto3-omics-1.28.16/mypy_boto3_omics/type_defs.pyi` & `mypy-boto3-omics-1.28.16.post1/mypy_boto3_omics/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_omics.type_defs import AbortMultipartReadSetUploadRequestRequestTypeDef
 
-    data: AbortMultipartReadSetUploadRequestRequestTypeDef = {...}
+    data: AbortMultipartReadSetUploadRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -54,25 +54,26 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AbortMultipartReadSetUploadRequestRequestTypeDef",
-    "ActivateReadSetFilterTypeDef",
+    "TimestampTypeDef",
     "ActivateReadSetJobItemTypeDef",
     "ActivateReadSetSourceItemTypeDef",
     "AnnotationImportItemDetailTypeDef",
     "AnnotationImportItemSourceTypeDef",
     "AnnotationImportJobItemTypeDef",
     "ReferenceItemTypeDef",
     "SseConfigTypeDef",
     "BatchDeleteReadSetRequestRequestTypeDef",
     "ReadSetBatchErrorTypeDef",
     "ResponseMetadataTypeDef",
+    "BlobTypeDef",
     "CancelAnnotationImportRequestRequestTypeDef",
     "CancelRunRequestRequestTypeDef",
     "CancelVariantImportRequestRequestTypeDef",
     "CompleteReadSetUploadPartListItemTypeDef",
     "CreateMultipartReadSetUploadRequestRequestTypeDef",
     "CreateRunGroupRequestRequestTypeDef",
     "WorkflowParameterTypeDef",
@@ -81,15 +82,14 @@
     "DeleteReferenceStoreRequestRequestTypeDef",
     "DeleteRunGroupRequestRequestTypeDef",
     "DeleteRunRequestRequestTypeDef",
     "DeleteSequenceStoreRequestRequestTypeDef",
     "DeleteVariantStoreRequestRequestTypeDef",
     "DeleteWorkflowRequestRequestTypeDef",
     "ExportReadSetDetailTypeDef",
-    "ExportReadSetFilterTypeDef",
     "ExportReadSetJobDetailTypeDef",
     "ExportReadSetTypeDef",
     "FileInformationTypeDef",
     "VcfOptionsTypeDef",
     "WaiterConfigTypeDef",
     "GetAnnotationImportRequestRequestTypeDef",
     "GetAnnotationStoreRequestRequestTypeDef",
@@ -108,37 +108,30 @@
     "GetRunRequestRequestTypeDef",
     "GetRunTaskRequestRequestTypeDef",
     "GetSequenceStoreRequestRequestTypeDef",
     "GetVariantImportRequestRequestTypeDef",
     "VariantImportItemDetailTypeDef",
     "GetVariantStoreRequestRequestTypeDef",
     "GetWorkflowRequestRequestTypeDef",
-    "ImportReadSetFilterTypeDef",
     "ImportReadSetJobItemTypeDef",
     "SourceFilesTypeDef",
-    "ImportReferenceFilterTypeDef",
     "ImportReferenceJobItemTypeDef",
     "ListAnnotationImportJobsFilterTypeDef",
     "PaginatorConfigTypeDef",
     "ListAnnotationStoresFilterTypeDef",
     "ListMultipartReadSetUploadsRequestRequestTypeDef",
     "MultipartReadSetUploadListItemTypeDef",
-    "ReadSetUploadPartListFilterTypeDef",
     "ReadSetUploadPartListItemTypeDef",
-    "ReadSetFilterTypeDef",
-    "ReferenceStoreFilterTypeDef",
-    "ReferenceFilterTypeDef",
     "ReferenceListItemTypeDef",
     "ListRunGroupsRequestRequestTypeDef",
     "RunGroupListItemTypeDef",
     "ListRunTasksRequestRequestTypeDef",
     "TaskListItemTypeDef",
     "ListRunsRequestRequestTypeDef",
     "RunListItemTypeDef",
-    "SequenceStoreFilterTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListVariantImportJobsFilterTypeDef",
     "VariantImportJobItemTypeDef",
     "ListVariantStoresFilterTypeDef",
     "ListWorkflowsRequestRequestTypeDef",
     "WorkflowListItemTypeDef",
     "ReadOptionsTypeDef",
@@ -150,16 +143,23 @@
     "TsvStoreOptionsTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAnnotationStoreRequestRequestTypeDef",
     "UpdateRunGroupRequestRequestTypeDef",
     "UpdateVariantStoreRequestRequestTypeDef",
     "UpdateWorkflowRequestRequestTypeDef",
-    "UploadReadSetPartRequestRequestTypeDef",
-    "ListReadSetActivationJobsRequestRequestTypeDef",
+    "ActivateReadSetFilterTypeDef",
+    "ExportReadSetFilterTypeDef",
+    "ImportReadSetFilterTypeDef",
+    "ImportReferenceFilterTypeDef",
+    "ReadSetFilterTypeDef",
+    "ReadSetUploadPartListFilterTypeDef",
+    "ReferenceFilterTypeDef",
+    "ReferenceStoreFilterTypeDef",
+    "SequenceStoreFilterTypeDef",
     "AnnotationStoreItemTypeDef",
     "CreateReferenceStoreRequestRequestTypeDef",
     "CreateSequenceStoreRequestRequestTypeDef",
     "CreateVariantStoreRequestRequestTypeDef",
     "ReferenceStoreDetailTypeDef",
     "SequenceStoreDetailTypeDef",
     "VariantStoreItemTypeDef",
@@ -191,19 +191,19 @@
     "StartReadSetExportJobResponseTypeDef",
     "StartReadSetImportJobResponseTypeDef",
     "StartReferenceImportJobResponseTypeDef",
     "StartRunResponseTypeDef",
     "StartVariantImportResponseTypeDef",
     "UpdateVariantStoreResponseTypeDef",
     "UploadReadSetPartResponseTypeDef",
+    "UploadReadSetPartRequestRequestTypeDef",
     "CompleteMultipartReadSetUploadRequestRequestTypeDef",
     "CreateWorkflowRequestRequestTypeDef",
     "GetWorkflowResponseTypeDef",
     "GetReadSetExportJobResponseTypeDef",
-    "ListReadSetExportJobsRequestRequestTypeDef",
     "ListReadSetExportJobsResponseTypeDef",
     "StartReadSetExportJobRequestRequestTypeDef",
     "ReadSetFilesTypeDef",
     "ReferenceFilesTypeDef",
     "GetAnnotationImportRequestAnnotationImportJobCreatedWaitTypeDef",
     "GetAnnotationStoreRequestAnnotationStoreCreatedWaitTypeDef",
     "GetAnnotationStoreRequestAnnotationStoreDeletedWaitTypeDef",
@@ -218,97 +218,91 @@
     "GetVariantImportRequestVariantImportJobCreatedWaitTypeDef",
     "GetVariantStoreRequestVariantStoreCreatedWaitTypeDef",
     "GetVariantStoreRequestVariantStoreDeletedWaitTypeDef",
     "GetWorkflowRequestWorkflowActiveWaitTypeDef",
     "ReadSetListItemTypeDef",
     "GetReferenceImportJobResponseTypeDef",
     "GetVariantImportResponseTypeDef",
-    "ListReadSetImportJobsRequestRequestTypeDef",
     "ListReadSetImportJobsResponseTypeDef",
     "ImportReadSetSourceItemTypeDef",
     "StartReadSetImportJobSourceItemTypeDef",
-    "ListReferenceImportJobsRequestRequestTypeDef",
     "ListReferenceImportJobsResponseTypeDef",
     "ListAnnotationImportJobsRequestRequestTypeDef",
     "ListAnnotationImportJobsRequestListAnnotationImportJobsPaginateTypeDef",
     "ListMultipartReadSetUploadsRequestListMultipartReadSetUploadsPaginateTypeDef",
-    "ListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef",
-    "ListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef",
-    "ListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef",
-    "ListReferenceImportJobsRequestListReferenceImportJobsPaginateTypeDef",
     "ListRunGroupsRequestListRunGroupsPaginateTypeDef",
     "ListRunTasksRequestListRunTasksPaginateTypeDef",
     "ListRunsRequestListRunsPaginateTypeDef",
     "ListWorkflowsRequestListWorkflowsPaginateTypeDef",
     "ListAnnotationStoresRequestListAnnotationStoresPaginateTypeDef",
     "ListAnnotationStoresRequestRequestTypeDef",
     "ListMultipartReadSetUploadsResponseTypeDef",
-    "ListReadSetUploadPartsRequestListReadSetUploadPartsPaginateTypeDef",
-    "ListReadSetUploadPartsRequestRequestTypeDef",
     "ListReadSetUploadPartsResponseTypeDef",
-    "ListReadSetsRequestListReadSetsPaginateTypeDef",
-    "ListReadSetsRequestRequestTypeDef",
-    "ListReferenceStoresRequestListReferenceStoresPaginateTypeDef",
-    "ListReferenceStoresRequestRequestTypeDef",
-    "ListReferencesRequestListReferencesPaginateTypeDef",
-    "ListReferencesRequestRequestTypeDef",
     "ListReferencesResponseTypeDef",
     "ListRunGroupsResponseTypeDef",
     "ListRunTasksResponseTypeDef",
     "ListRunsResponseTypeDef",
-    "ListSequenceStoresRequestListSequenceStoresPaginateTypeDef",
-    "ListSequenceStoresRequestRequestTypeDef",
     "ListVariantImportJobsRequestListVariantImportJobsPaginateTypeDef",
     "ListVariantImportJobsRequestRequestTypeDef",
     "ListVariantImportJobsResponseTypeDef",
     "ListVariantStoresRequestListVariantStoresPaginateTypeDef",
     "ListVariantStoresRequestRequestTypeDef",
     "ListWorkflowsResponseTypeDef",
     "TsvOptionsTypeDef",
     "StartReadSetActivationJobRequestRequestTypeDef",
     "StartReferenceImportJobRequestRequestTypeDef",
     "StartVariantImportRequestRequestTypeDef",
     "StoreOptionsOutputTypeDef",
     "StoreOptionsTypeDef",
+    "ListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef",
+    "ListReadSetActivationJobsRequestRequestTypeDef",
+    "ListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef",
+    "ListReadSetExportJobsRequestRequestTypeDef",
+    "ListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef",
+    "ListReadSetImportJobsRequestRequestTypeDef",
+    "ListReferenceImportJobsRequestListReferenceImportJobsPaginateTypeDef",
+    "ListReferenceImportJobsRequestRequestTypeDef",
+    "ListReadSetsRequestListReadSetsPaginateTypeDef",
+    "ListReadSetsRequestRequestTypeDef",
+    "ListReadSetUploadPartsRequestListReadSetUploadPartsPaginateTypeDef",
+    "ListReadSetUploadPartsRequestRequestTypeDef",
+    "ListReferencesRequestListReferencesPaginateTypeDef",
+    "ListReferencesRequestRequestTypeDef",
+    "ListReferenceStoresRequestListReferenceStoresPaginateTypeDef",
+    "ListReferenceStoresRequestRequestTypeDef",
+    "ListSequenceStoresRequestListSequenceStoresPaginateTypeDef",
+    "ListSequenceStoresRequestRequestTypeDef",
     "ListAnnotationStoresResponseTypeDef",
     "ListReferenceStoresResponseTypeDef",
     "ListSequenceStoresResponseTypeDef",
     "ListVariantStoresResponseTypeDef",
     "GetReadSetMetadataResponseTypeDef",
     "GetReferenceMetadataResponseTypeDef",
     "ListReadSetsResponseTypeDef",
     "GetReadSetImportJobResponseTypeDef",
     "StartReadSetImportJobRequestRequestTypeDef",
     "FormatOptionsTypeDef",
     "CreateAnnotationStoreResponseTypeDef",
     "GetAnnotationStoreResponseTypeDef",
     "UpdateAnnotationStoreResponseTypeDef",
     "CreateAnnotationStoreRequestRequestTypeDef",
+    "StoreOptionsUnionTypeDef",
     "GetAnnotationImportResponseTypeDef",
     "StartAnnotationImportRequestRequestTypeDef",
 )
 
 AbortMultipartReadSetUploadRequestRequestTypeDef = TypedDict(
     "AbortMultipartReadSetUploadRequestRequestTypeDef",
     {
         "sequenceStoreId": str,
         "uploadId": str,
     },
 )
 
-ActivateReadSetFilterTypeDef = TypedDict(
-    "ActivateReadSetFilterTypeDef",
-    {
-        "status": ReadSetActivationJobStatusType,
-        "createdAfter": Union[datetime, str],
-        "createdBefore": Union[datetime, str],
-    },
-    total=False,
-)
-
+TimestampTypeDef = Union[datetime, str]
 _RequiredActivateReadSetJobItemTypeDef = TypedDict(
     "_RequiredActivateReadSetJobItemTypeDef",
     {
         "id": str,
         "sequenceStoreId": str,
         "status": ReadSetActivationJobStatusType,
         "creationTime": datetime,
@@ -437,14 +431,15 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 CancelAnnotationImportRequestRequestTypeDef = TypedDict(
     "CancelAnnotationImportRequestRequestTypeDef",
     {
         "jobId": str,
     },
 )
 
@@ -631,24 +626,14 @@
 )
 
 class ExportReadSetDetailTypeDef(
     _RequiredExportReadSetDetailTypeDef, _OptionalExportReadSetDetailTypeDef
 ):
     pass
 
-ExportReadSetFilterTypeDef = TypedDict(
-    "ExportReadSetFilterTypeDef",
-    {
-        "status": ReadSetExportJobStatusType,
-        "createdAfter": Union[datetime, str],
-        "createdBefore": Union[datetime, str],
-    },
-    total=False,
-)
-
 _RequiredExportReadSetJobDetailTypeDef = TypedDict(
     "_RequiredExportReadSetJobDetailTypeDef",
     {
         "id": str,
         "sequenceStoreId": str,
         "destination": str,
         "status": ReadSetExportJobStatusType,
@@ -940,24 +925,14 @@
 )
 
 class GetWorkflowRequestRequestTypeDef(
     _RequiredGetWorkflowRequestRequestTypeDef, _OptionalGetWorkflowRequestRequestTypeDef
 ):
     pass
 
-ImportReadSetFilterTypeDef = TypedDict(
-    "ImportReadSetFilterTypeDef",
-    {
-        "status": ReadSetImportJobStatusType,
-        "createdAfter": Union[datetime, str],
-        "createdBefore": Union[datetime, str],
-    },
-    total=False,
-)
-
 _RequiredImportReadSetJobItemTypeDef = TypedDict(
     "_RequiredImportReadSetJobItemTypeDef",
     {
         "id": str,
         "sequenceStoreId": str,
         "roleArn": str,
         "status": ReadSetImportJobStatusType,
@@ -990,24 +965,14 @@
     },
     total=False,
 )
 
 class SourceFilesTypeDef(_RequiredSourceFilesTypeDef, _OptionalSourceFilesTypeDef):
     pass
 
-ImportReferenceFilterTypeDef = TypedDict(
-    "ImportReferenceFilterTypeDef",
-    {
-        "status": ReferenceImportJobStatusType,
-        "createdAfter": Union[datetime, str],
-        "createdBefore": Union[datetime, str],
-    },
-    total=False,
-)
-
 _RequiredImportReferenceJobItemTypeDef = TypedDict(
     "_RequiredImportReferenceJobItemTypeDef",
     {
         "id": str,
         "referenceStoreId": str,
         "roleArn": str,
         "status": ReferenceImportJobStatusType,
@@ -1099,23 +1064,14 @@
 )
 
 class MultipartReadSetUploadListItemTypeDef(
     _RequiredMultipartReadSetUploadListItemTypeDef, _OptionalMultipartReadSetUploadListItemTypeDef
 ):
     pass
 
-ReadSetUploadPartListFilterTypeDef = TypedDict(
-    "ReadSetUploadPartListFilterTypeDef",
-    {
-        "createdAfter": Union[datetime, str],
-        "createdBefore": Union[datetime, str],
-    },
-    total=False,
-)
-
 _RequiredReadSetUploadPartListItemTypeDef = TypedDict(
     "_RequiredReadSetUploadPartListItemTypeDef",
     {
         "partNumber": int,
         "partSize": int,
         "partSource": ReadSetPartSourceType,
         "checksum": str,
@@ -1131,51 +1087,14 @@
 )
 
 class ReadSetUploadPartListItemTypeDef(
     _RequiredReadSetUploadPartListItemTypeDef, _OptionalReadSetUploadPartListItemTypeDef
 ):
     pass
 
-ReadSetFilterTypeDef = TypedDict(
-    "ReadSetFilterTypeDef",
-    {
-        "name": str,
-        "status": ReadSetStatusType,
-        "referenceArn": str,
-        "createdAfter": Union[datetime, str],
-        "createdBefore": Union[datetime, str],
-        "sampleId": str,
-        "subjectId": str,
-        "generatedFrom": str,
-        "creationType": CreationTypeType,
-    },
-    total=False,
-)
-
-ReferenceStoreFilterTypeDef = TypedDict(
-    "ReferenceStoreFilterTypeDef",
-    {
-        "name": str,
-        "createdAfter": Union[datetime, str],
-        "createdBefore": Union[datetime, str],
-    },
-    total=False,
-)
-
-ReferenceFilterTypeDef = TypedDict(
-    "ReferenceFilterTypeDef",
-    {
-        "name": str,
-        "md5": str,
-        "createdAfter": Union[datetime, str],
-        "createdBefore": Union[datetime, str],
-    },
-    total=False,
-)
-
 _RequiredReferenceListItemTypeDef = TypedDict(
     "_RequiredReferenceListItemTypeDef",
     {
         "id": str,
         "arn": str,
         "referenceStoreId": str,
         "md5": str,
@@ -1285,24 +1204,14 @@
         "creationTime": datetime,
         "startTime": datetime,
         "stopTime": datetime,
     },
     total=False,
 )
 
-SequenceStoreFilterTypeDef = TypedDict(
-    "SequenceStoreFilterTypeDef",
-    {
-        "name": str,
-        "createdAfter": Union[datetime, str],
-        "createdBefore": Union[datetime, str],
-    },
-    total=False,
-)
-
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
@@ -1572,46 +1481,109 @@
 )
 
 class UpdateWorkflowRequestRequestTypeDef(
     _RequiredUpdateWorkflowRequestRequestTypeDef, _OptionalUpdateWorkflowRequestRequestTypeDef
 ):
     pass
 
-UploadReadSetPartRequestRequestTypeDef = TypedDict(
-    "UploadReadSetPartRequestRequestTypeDef",
+ActivateReadSetFilterTypeDef = TypedDict(
+    "ActivateReadSetFilterTypeDef",
     {
-        "sequenceStoreId": str,
-        "uploadId": str,
-        "partSource": ReadSetPartSourceType,
-        "partNumber": int,
-        "payload": Union[str, bytes, IO[Any], StreamingBody],
+        "status": ReadSetActivationJobStatusType,
+        "createdAfter": TimestampTypeDef,
+        "createdBefore": TimestampTypeDef,
     },
+    total=False,
 )
 
-_RequiredListReadSetActivationJobsRequestRequestTypeDef = TypedDict(
-    "_RequiredListReadSetActivationJobsRequestRequestTypeDef",
+ExportReadSetFilterTypeDef = TypedDict(
+    "ExportReadSetFilterTypeDef",
     {
-        "sequenceStoreId": str,
+        "status": ReadSetExportJobStatusType,
+        "createdAfter": TimestampTypeDef,
+        "createdBefore": TimestampTypeDef,
     },
+    total=False,
 )
-_OptionalListReadSetActivationJobsRequestRequestTypeDef = TypedDict(
-    "_OptionalListReadSetActivationJobsRequestRequestTypeDef",
+
+ImportReadSetFilterTypeDef = TypedDict(
+    "ImportReadSetFilterTypeDef",
     {
-        "maxResults": int,
-        "nextToken": str,
-        "filter": ActivateReadSetFilterTypeDef,
+        "status": ReadSetImportJobStatusType,
+        "createdAfter": TimestampTypeDef,
+        "createdBefore": TimestampTypeDef,
     },
     total=False,
 )
 
-class ListReadSetActivationJobsRequestRequestTypeDef(
-    _RequiredListReadSetActivationJobsRequestRequestTypeDef,
-    _OptionalListReadSetActivationJobsRequestRequestTypeDef,
-):
-    pass
+ImportReferenceFilterTypeDef = TypedDict(
+    "ImportReferenceFilterTypeDef",
+    {
+        "status": ReferenceImportJobStatusType,
+        "createdAfter": TimestampTypeDef,
+        "createdBefore": TimestampTypeDef,
+    },
+    total=False,
+)
+
+ReadSetFilterTypeDef = TypedDict(
+    "ReadSetFilterTypeDef",
+    {
+        "name": str,
+        "status": ReadSetStatusType,
+        "referenceArn": str,
+        "createdAfter": TimestampTypeDef,
+        "createdBefore": TimestampTypeDef,
+        "sampleId": str,
+        "subjectId": str,
+        "generatedFrom": str,
+        "creationType": CreationTypeType,
+    },
+    total=False,
+)
+
+ReadSetUploadPartListFilterTypeDef = TypedDict(
+    "ReadSetUploadPartListFilterTypeDef",
+    {
+        "createdAfter": TimestampTypeDef,
+        "createdBefore": TimestampTypeDef,
+    },
+    total=False,
+)
+
+ReferenceFilterTypeDef = TypedDict(
+    "ReferenceFilterTypeDef",
+    {
+        "name": str,
+        "md5": str,
+        "createdAfter": TimestampTypeDef,
+        "createdBefore": TimestampTypeDef,
+    },
+    total=False,
+)
+
+ReferenceStoreFilterTypeDef = TypedDict(
+    "ReferenceStoreFilterTypeDef",
+    {
+        "name": str,
+        "createdAfter": TimestampTypeDef,
+        "createdBefore": TimestampTypeDef,
+    },
+    total=False,
+)
+
+SequenceStoreFilterTypeDef = TypedDict(
+    "SequenceStoreFilterTypeDef",
+    {
+        "name": str,
+        "createdAfter": TimestampTypeDef,
+        "createdBefore": TimestampTypeDef,
+    },
+    total=False,
+)
 
 AnnotationStoreItemTypeDef = TypedDict(
     "AnnotationStoreItemTypeDef",
     {
         "id": str,
         "reference": ReferenceItemTypeDef,
         "status": StoreStatusType,
@@ -2137,14 +2109,25 @@
     "UploadReadSetPartResponseTypeDef",
     {
         "checksum": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+UploadReadSetPartRequestRequestTypeDef = TypedDict(
+    "UploadReadSetPartRequestRequestTypeDef",
+    {
+        "sequenceStoreId": str,
+        "uploadId": str,
+        "partSource": ReadSetPartSourceType,
+        "partNumber": int,
+        "payload": BlobTypeDef,
+    },
+)
+
 CompleteMultipartReadSetUploadRequestRequestTypeDef = TypedDict(
     "CompleteMultipartReadSetUploadRequestRequestTypeDef",
     {
         "sequenceStoreId": str,
         "uploadId": str,
         "parts": Sequence[CompleteReadSetUploadPartListItemTypeDef],
     },
@@ -2158,15 +2141,15 @@
 )
 _OptionalCreateWorkflowRequestRequestTypeDef = TypedDict(
     "_OptionalCreateWorkflowRequestRequestTypeDef",
     {
         "name": str,
         "description": str,
         "engine": WorkflowEngineType,
-        "definitionZip": Union[str, bytes, IO[Any], StreamingBody],
+        "definitionZip": BlobTypeDef,
         "definitionUri": str,
         "main": str,
         "parameterTemplate": Mapping[str, WorkflowParameterTypeDef],
         "storageCapacity": int,
         "tags": Mapping[str, str],
         "accelerators": Literal["GPU"],
     },
@@ -2213,36 +2196,14 @@
         "creationTime": datetime,
         "completionTime": datetime,
         "readSets": List[ExportReadSetDetailTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredListReadSetExportJobsRequestRequestTypeDef = TypedDict(
-    "_RequiredListReadSetExportJobsRequestRequestTypeDef",
-    {
-        "sequenceStoreId": str,
-    },
-)
-_OptionalListReadSetExportJobsRequestRequestTypeDef = TypedDict(
-    "_OptionalListReadSetExportJobsRequestRequestTypeDef",
-    {
-        "maxResults": int,
-        "nextToken": str,
-        "filter": ExportReadSetFilterTypeDef,
-    },
-    total=False,
-)
-
-class ListReadSetExportJobsRequestRequestTypeDef(
-    _RequiredListReadSetExportJobsRequestRequestTypeDef,
-    _OptionalListReadSetExportJobsRequestRequestTypeDef,
-):
-    pass
-
 ListReadSetExportJobsResponseTypeDef = TypedDict(
     "ListReadSetExportJobsResponseTypeDef",
     {
         "nextToken": str,
         "exportJobs": List[ExportReadSetJobDetailTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2656,36 +2617,14 @@
         "items": List[VariantImportItemDetailTypeDef],
         "runLeftNormalization": bool,
         "annotationFields": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredListReadSetImportJobsRequestRequestTypeDef = TypedDict(
-    "_RequiredListReadSetImportJobsRequestRequestTypeDef",
-    {
-        "sequenceStoreId": str,
-    },
-)
-_OptionalListReadSetImportJobsRequestRequestTypeDef = TypedDict(
-    "_OptionalListReadSetImportJobsRequestRequestTypeDef",
-    {
-        "maxResults": int,
-        "nextToken": str,
-        "filter": ImportReadSetFilterTypeDef,
-    },
-    total=False,
-)
-
-class ListReadSetImportJobsRequestRequestTypeDef(
-    _RequiredListReadSetImportJobsRequestRequestTypeDef,
-    _OptionalListReadSetImportJobsRequestRequestTypeDef,
-):
-    pass
-
 ListReadSetImportJobsResponseTypeDef = TypedDict(
     "ListReadSetImportJobsResponseTypeDef",
     {
         "nextToken": str,
         "importJobs": List[ImportReadSetJobItemTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2741,36 +2680,14 @@
 )
 
 class StartReadSetImportJobSourceItemTypeDef(
     _RequiredStartReadSetImportJobSourceItemTypeDef, _OptionalStartReadSetImportJobSourceItemTypeDef
 ):
     pass
 
-_RequiredListReferenceImportJobsRequestRequestTypeDef = TypedDict(
-    "_RequiredListReferenceImportJobsRequestRequestTypeDef",
-    {
-        "referenceStoreId": str,
-    },
-)
-_OptionalListReferenceImportJobsRequestRequestTypeDef = TypedDict(
-    "_OptionalListReferenceImportJobsRequestRequestTypeDef",
-    {
-        "maxResults": int,
-        "nextToken": str,
-        "filter": ImportReferenceFilterTypeDef,
-    },
-    total=False,
-)
-
-class ListReferenceImportJobsRequestRequestTypeDef(
-    _RequiredListReferenceImportJobsRequestRequestTypeDef,
-    _OptionalListReferenceImportJobsRequestRequestTypeDef,
-):
-    pass
-
 ListReferenceImportJobsResponseTypeDef = TypedDict(
     "ListReferenceImportJobsResponseTypeDef",
     {
         "nextToken": str,
         "importJobs": List[ImportReferenceJobItemTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2813,98 +2730,14 @@
 
 class ListMultipartReadSetUploadsRequestListMultipartReadSetUploadsPaginateTypeDef(
     _RequiredListMultipartReadSetUploadsRequestListMultipartReadSetUploadsPaginateTypeDef,
     _OptionalListMultipartReadSetUploadsRequestListMultipartReadSetUploadsPaginateTypeDef,
 ):
     pass
 
-_RequiredListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef = TypedDict(
-    "_RequiredListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef",
-    {
-        "sequenceStoreId": str,
-    },
-)
-_OptionalListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef = TypedDict(
-    "_OptionalListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef",
-    {
-        "filter": ActivateReadSetFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef(
-    _RequiredListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef,
-    _OptionalListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef,
-):
-    pass
-
-_RequiredListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef = TypedDict(
-    "_RequiredListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef",
-    {
-        "sequenceStoreId": str,
-    },
-)
-_OptionalListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef = TypedDict(
-    "_OptionalListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef",
-    {
-        "filter": ExportReadSetFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef(
-    _RequiredListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef,
-    _OptionalListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef,
-):
-    pass
-
-_RequiredListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef = TypedDict(
-    "_RequiredListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef",
-    {
-        "sequenceStoreId": str,
-    },
-)
-_OptionalListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef = TypedDict(
-    "_OptionalListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef",
-    {
-        "filter": ImportReadSetFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef(
-    _RequiredListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef,
-    _OptionalListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef,
-):
-    pass
-
-_RequiredListReferenceImportJobsRequestListReferenceImportJobsPaginateTypeDef = TypedDict(
-    "_RequiredListReferenceImportJobsRequestListReferenceImportJobsPaginateTypeDef",
-    {
-        "referenceStoreId": str,
-    },
-)
-_OptionalListReferenceImportJobsRequestListReferenceImportJobsPaginateTypeDef = TypedDict(
-    "_OptionalListReferenceImportJobsRequestListReferenceImportJobsPaginateTypeDef",
-    {
-        "filter": ImportReferenceFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListReferenceImportJobsRequestListReferenceImportJobsPaginateTypeDef(
-    _RequiredListReferenceImportJobsRequestListReferenceImportJobsPaginateTypeDef,
-    _OptionalListReferenceImportJobsRequestListReferenceImportJobsPaginateTypeDef,
-):
-    pass
-
 ListRunGroupsRequestListRunGroupsPaginateTypeDef = TypedDict(
     "ListRunGroupsRequestListRunGroupsPaginateTypeDef",
     {
         "name": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -2978,173 +2811,23 @@
     {
         "nextToken": str,
         "uploads": List[MultipartReadSetUploadListItemTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredListReadSetUploadPartsRequestListReadSetUploadPartsPaginateTypeDef = TypedDict(
-    "_RequiredListReadSetUploadPartsRequestListReadSetUploadPartsPaginateTypeDef",
-    {
-        "sequenceStoreId": str,
-        "uploadId": str,
-        "partSource": ReadSetPartSourceType,
-    },
-)
-_OptionalListReadSetUploadPartsRequestListReadSetUploadPartsPaginateTypeDef = TypedDict(
-    "_OptionalListReadSetUploadPartsRequestListReadSetUploadPartsPaginateTypeDef",
-    {
-        "filter": ReadSetUploadPartListFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListReadSetUploadPartsRequestListReadSetUploadPartsPaginateTypeDef(
-    _RequiredListReadSetUploadPartsRequestListReadSetUploadPartsPaginateTypeDef,
-    _OptionalListReadSetUploadPartsRequestListReadSetUploadPartsPaginateTypeDef,
-):
-    pass
-
-_RequiredListReadSetUploadPartsRequestRequestTypeDef = TypedDict(
-    "_RequiredListReadSetUploadPartsRequestRequestTypeDef",
-    {
-        "sequenceStoreId": str,
-        "uploadId": str,
-        "partSource": ReadSetPartSourceType,
-    },
-)
-_OptionalListReadSetUploadPartsRequestRequestTypeDef = TypedDict(
-    "_OptionalListReadSetUploadPartsRequestRequestTypeDef",
-    {
-        "maxResults": int,
-        "nextToken": str,
-        "filter": ReadSetUploadPartListFilterTypeDef,
-    },
-    total=False,
-)
-
-class ListReadSetUploadPartsRequestRequestTypeDef(
-    _RequiredListReadSetUploadPartsRequestRequestTypeDef,
-    _OptionalListReadSetUploadPartsRequestRequestTypeDef,
-):
-    pass
-
 ListReadSetUploadPartsResponseTypeDef = TypedDict(
     "ListReadSetUploadPartsResponseTypeDef",
     {
         "nextToken": str,
         "parts": List[ReadSetUploadPartListItemTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredListReadSetsRequestListReadSetsPaginateTypeDef = TypedDict(
-    "_RequiredListReadSetsRequestListReadSetsPaginateTypeDef",
-    {
-        "sequenceStoreId": str,
-    },
-)
-_OptionalListReadSetsRequestListReadSetsPaginateTypeDef = TypedDict(
-    "_OptionalListReadSetsRequestListReadSetsPaginateTypeDef",
-    {
-        "filter": ReadSetFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListReadSetsRequestListReadSetsPaginateTypeDef(
-    _RequiredListReadSetsRequestListReadSetsPaginateTypeDef,
-    _OptionalListReadSetsRequestListReadSetsPaginateTypeDef,
-):
-    pass
-
-_RequiredListReadSetsRequestRequestTypeDef = TypedDict(
-    "_RequiredListReadSetsRequestRequestTypeDef",
-    {
-        "sequenceStoreId": str,
-    },
-)
-_OptionalListReadSetsRequestRequestTypeDef = TypedDict(
-    "_OptionalListReadSetsRequestRequestTypeDef",
-    {
-        "maxResults": int,
-        "nextToken": str,
-        "filter": ReadSetFilterTypeDef,
-    },
-    total=False,
-)
-
-class ListReadSetsRequestRequestTypeDef(
-    _RequiredListReadSetsRequestRequestTypeDef, _OptionalListReadSetsRequestRequestTypeDef
-):
-    pass
-
-ListReferenceStoresRequestListReferenceStoresPaginateTypeDef = TypedDict(
-    "ListReferenceStoresRequestListReferenceStoresPaginateTypeDef",
-    {
-        "filter": ReferenceStoreFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListReferenceStoresRequestRequestTypeDef = TypedDict(
-    "ListReferenceStoresRequestRequestTypeDef",
-    {
-        "maxResults": int,
-        "nextToken": str,
-        "filter": ReferenceStoreFilterTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListReferencesRequestListReferencesPaginateTypeDef = TypedDict(
-    "_RequiredListReferencesRequestListReferencesPaginateTypeDef",
-    {
-        "referenceStoreId": str,
-    },
-)
-_OptionalListReferencesRequestListReferencesPaginateTypeDef = TypedDict(
-    "_OptionalListReferencesRequestListReferencesPaginateTypeDef",
-    {
-        "filter": ReferenceFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListReferencesRequestListReferencesPaginateTypeDef(
-    _RequiredListReferencesRequestListReferencesPaginateTypeDef,
-    _OptionalListReferencesRequestListReferencesPaginateTypeDef,
-):
-    pass
-
-_RequiredListReferencesRequestRequestTypeDef = TypedDict(
-    "_RequiredListReferencesRequestRequestTypeDef",
-    {
-        "referenceStoreId": str,
-    },
-)
-_OptionalListReferencesRequestRequestTypeDef = TypedDict(
-    "_OptionalListReferencesRequestRequestTypeDef",
-    {
-        "maxResults": int,
-        "nextToken": str,
-        "filter": ReferenceFilterTypeDef,
-    },
-    total=False,
-)
-
-class ListReferencesRequestRequestTypeDef(
-    _RequiredListReferencesRequestRequestTypeDef, _OptionalListReferencesRequestRequestTypeDef
-):
-    pass
-
 ListReferencesResponseTypeDef = TypedDict(
     "ListReferencesResponseTypeDef",
     {
         "nextToken": str,
         "references": List[ReferenceListItemTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -3173,33 +2856,14 @@
     {
         "items": List[RunListItemTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListSequenceStoresRequestListSequenceStoresPaginateTypeDef = TypedDict(
-    "ListSequenceStoresRequestListSequenceStoresPaginateTypeDef",
-    {
-        "filter": SequenceStoreFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListSequenceStoresRequestRequestTypeDef = TypedDict(
-    "ListSequenceStoresRequestRequestTypeDef",
-    {
-        "maxResults": int,
-        "nextToken": str,
-        "filter": SequenceStoreFilterTypeDef,
-    },
-    total=False,
-)
-
 ListVariantImportJobsRequestListVariantImportJobsPaginateTypeDef = TypedDict(
     "ListVariantImportJobsRequestListVariantImportJobsPaginateTypeDef",
     {
         "ids": Sequence[str],
         "filter": ListVariantImportJobsFilterTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
@@ -3342,14 +3006,355 @@
     "StoreOptionsTypeDef",
     {
         "tsvStoreOptions": TsvStoreOptionsTypeDef,
     },
     total=False,
 )
 
+_RequiredListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef = TypedDict(
+    "_RequiredListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef",
+    {
+        "sequenceStoreId": str,
+    },
+)
+_OptionalListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef = TypedDict(
+    "_OptionalListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef",
+    {
+        "filter": ActivateReadSetFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef(
+    _RequiredListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef,
+    _OptionalListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef,
+):
+    pass
+
+_RequiredListReadSetActivationJobsRequestRequestTypeDef = TypedDict(
+    "_RequiredListReadSetActivationJobsRequestRequestTypeDef",
+    {
+        "sequenceStoreId": str,
+    },
+)
+_OptionalListReadSetActivationJobsRequestRequestTypeDef = TypedDict(
+    "_OptionalListReadSetActivationJobsRequestRequestTypeDef",
+    {
+        "maxResults": int,
+        "nextToken": str,
+        "filter": ActivateReadSetFilterTypeDef,
+    },
+    total=False,
+)
+
+class ListReadSetActivationJobsRequestRequestTypeDef(
+    _RequiredListReadSetActivationJobsRequestRequestTypeDef,
+    _OptionalListReadSetActivationJobsRequestRequestTypeDef,
+):
+    pass
+
+_RequiredListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef = TypedDict(
+    "_RequiredListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef",
+    {
+        "sequenceStoreId": str,
+    },
+)
+_OptionalListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef = TypedDict(
+    "_OptionalListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef",
+    {
+        "filter": ExportReadSetFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef(
+    _RequiredListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef,
+    _OptionalListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef,
+):
+    pass
+
+_RequiredListReadSetExportJobsRequestRequestTypeDef = TypedDict(
+    "_RequiredListReadSetExportJobsRequestRequestTypeDef",
+    {
+        "sequenceStoreId": str,
+    },
+)
+_OptionalListReadSetExportJobsRequestRequestTypeDef = TypedDict(
+    "_OptionalListReadSetExportJobsRequestRequestTypeDef",
+    {
+        "maxResults": int,
+        "nextToken": str,
+        "filter": ExportReadSetFilterTypeDef,
+    },
+    total=False,
+)
+
+class ListReadSetExportJobsRequestRequestTypeDef(
+    _RequiredListReadSetExportJobsRequestRequestTypeDef,
+    _OptionalListReadSetExportJobsRequestRequestTypeDef,
+):
+    pass
+
+_RequiredListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef = TypedDict(
+    "_RequiredListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef",
+    {
+        "sequenceStoreId": str,
+    },
+)
+_OptionalListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef = TypedDict(
+    "_OptionalListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef",
+    {
+        "filter": ImportReadSetFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef(
+    _RequiredListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef,
+    _OptionalListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef,
+):
+    pass
+
+_RequiredListReadSetImportJobsRequestRequestTypeDef = TypedDict(
+    "_RequiredListReadSetImportJobsRequestRequestTypeDef",
+    {
+        "sequenceStoreId": str,
+    },
+)
+_OptionalListReadSetImportJobsRequestRequestTypeDef = TypedDict(
+    "_OptionalListReadSetImportJobsRequestRequestTypeDef",
+    {
+        "maxResults": int,
+        "nextToken": str,
+        "filter": ImportReadSetFilterTypeDef,
+    },
+    total=False,
+)
+
+class ListReadSetImportJobsRequestRequestTypeDef(
+    _RequiredListReadSetImportJobsRequestRequestTypeDef,
+    _OptionalListReadSetImportJobsRequestRequestTypeDef,
+):
+    pass
+
+_RequiredListReferenceImportJobsRequestListReferenceImportJobsPaginateTypeDef = TypedDict(
+    "_RequiredListReferenceImportJobsRequestListReferenceImportJobsPaginateTypeDef",
+    {
+        "referenceStoreId": str,
+    },
+)
+_OptionalListReferenceImportJobsRequestListReferenceImportJobsPaginateTypeDef = TypedDict(
+    "_OptionalListReferenceImportJobsRequestListReferenceImportJobsPaginateTypeDef",
+    {
+        "filter": ImportReferenceFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListReferenceImportJobsRequestListReferenceImportJobsPaginateTypeDef(
+    _RequiredListReferenceImportJobsRequestListReferenceImportJobsPaginateTypeDef,
+    _OptionalListReferenceImportJobsRequestListReferenceImportJobsPaginateTypeDef,
+):
+    pass
+
+_RequiredListReferenceImportJobsRequestRequestTypeDef = TypedDict(
+    "_RequiredListReferenceImportJobsRequestRequestTypeDef",
+    {
+        "referenceStoreId": str,
+    },
+)
+_OptionalListReferenceImportJobsRequestRequestTypeDef = TypedDict(
+    "_OptionalListReferenceImportJobsRequestRequestTypeDef",
+    {
+        "maxResults": int,
+        "nextToken": str,
+        "filter": ImportReferenceFilterTypeDef,
+    },
+    total=False,
+)
+
+class ListReferenceImportJobsRequestRequestTypeDef(
+    _RequiredListReferenceImportJobsRequestRequestTypeDef,
+    _OptionalListReferenceImportJobsRequestRequestTypeDef,
+):
+    pass
+
+_RequiredListReadSetsRequestListReadSetsPaginateTypeDef = TypedDict(
+    "_RequiredListReadSetsRequestListReadSetsPaginateTypeDef",
+    {
+        "sequenceStoreId": str,
+    },
+)
+_OptionalListReadSetsRequestListReadSetsPaginateTypeDef = TypedDict(
+    "_OptionalListReadSetsRequestListReadSetsPaginateTypeDef",
+    {
+        "filter": ReadSetFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListReadSetsRequestListReadSetsPaginateTypeDef(
+    _RequiredListReadSetsRequestListReadSetsPaginateTypeDef,
+    _OptionalListReadSetsRequestListReadSetsPaginateTypeDef,
+):
+    pass
+
+_RequiredListReadSetsRequestRequestTypeDef = TypedDict(
+    "_RequiredListReadSetsRequestRequestTypeDef",
+    {
+        "sequenceStoreId": str,
+    },
+)
+_OptionalListReadSetsRequestRequestTypeDef = TypedDict(
+    "_OptionalListReadSetsRequestRequestTypeDef",
+    {
+        "maxResults": int,
+        "nextToken": str,
+        "filter": ReadSetFilterTypeDef,
+    },
+    total=False,
+)
+
+class ListReadSetsRequestRequestTypeDef(
+    _RequiredListReadSetsRequestRequestTypeDef, _OptionalListReadSetsRequestRequestTypeDef
+):
+    pass
+
+_RequiredListReadSetUploadPartsRequestListReadSetUploadPartsPaginateTypeDef = TypedDict(
+    "_RequiredListReadSetUploadPartsRequestListReadSetUploadPartsPaginateTypeDef",
+    {
+        "sequenceStoreId": str,
+        "uploadId": str,
+        "partSource": ReadSetPartSourceType,
+    },
+)
+_OptionalListReadSetUploadPartsRequestListReadSetUploadPartsPaginateTypeDef = TypedDict(
+    "_OptionalListReadSetUploadPartsRequestListReadSetUploadPartsPaginateTypeDef",
+    {
+        "filter": ReadSetUploadPartListFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListReadSetUploadPartsRequestListReadSetUploadPartsPaginateTypeDef(
+    _RequiredListReadSetUploadPartsRequestListReadSetUploadPartsPaginateTypeDef,
+    _OptionalListReadSetUploadPartsRequestListReadSetUploadPartsPaginateTypeDef,
+):
+    pass
+
+_RequiredListReadSetUploadPartsRequestRequestTypeDef = TypedDict(
+    "_RequiredListReadSetUploadPartsRequestRequestTypeDef",
+    {
+        "sequenceStoreId": str,
+        "uploadId": str,
+        "partSource": ReadSetPartSourceType,
+    },
+)
+_OptionalListReadSetUploadPartsRequestRequestTypeDef = TypedDict(
+    "_OptionalListReadSetUploadPartsRequestRequestTypeDef",
+    {
+        "maxResults": int,
+        "nextToken": str,
+        "filter": ReadSetUploadPartListFilterTypeDef,
+    },
+    total=False,
+)
+
+class ListReadSetUploadPartsRequestRequestTypeDef(
+    _RequiredListReadSetUploadPartsRequestRequestTypeDef,
+    _OptionalListReadSetUploadPartsRequestRequestTypeDef,
+):
+    pass
+
+_RequiredListReferencesRequestListReferencesPaginateTypeDef = TypedDict(
+    "_RequiredListReferencesRequestListReferencesPaginateTypeDef",
+    {
+        "referenceStoreId": str,
+    },
+)
+_OptionalListReferencesRequestListReferencesPaginateTypeDef = TypedDict(
+    "_OptionalListReferencesRequestListReferencesPaginateTypeDef",
+    {
+        "filter": ReferenceFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListReferencesRequestListReferencesPaginateTypeDef(
+    _RequiredListReferencesRequestListReferencesPaginateTypeDef,
+    _OptionalListReferencesRequestListReferencesPaginateTypeDef,
+):
+    pass
+
+_RequiredListReferencesRequestRequestTypeDef = TypedDict(
+    "_RequiredListReferencesRequestRequestTypeDef",
+    {
+        "referenceStoreId": str,
+    },
+)
+_OptionalListReferencesRequestRequestTypeDef = TypedDict(
+    "_OptionalListReferencesRequestRequestTypeDef",
+    {
+        "maxResults": int,
+        "nextToken": str,
+        "filter": ReferenceFilterTypeDef,
+    },
+    total=False,
+)
+
+class ListReferencesRequestRequestTypeDef(
+    _RequiredListReferencesRequestRequestTypeDef, _OptionalListReferencesRequestRequestTypeDef
+):
+    pass
+
+ListReferenceStoresRequestListReferenceStoresPaginateTypeDef = TypedDict(
+    "ListReferenceStoresRequestListReferenceStoresPaginateTypeDef",
+    {
+        "filter": ReferenceStoreFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListReferenceStoresRequestRequestTypeDef = TypedDict(
+    "ListReferenceStoresRequestRequestTypeDef",
+    {
+        "maxResults": int,
+        "nextToken": str,
+        "filter": ReferenceStoreFilterTypeDef,
+    },
+    total=False,
+)
+
+ListSequenceStoresRequestListSequenceStoresPaginateTypeDef = TypedDict(
+    "ListSequenceStoresRequestListSequenceStoresPaginateTypeDef",
+    {
+        "filter": SequenceStoreFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListSequenceStoresRequestRequestTypeDef = TypedDict(
+    "ListSequenceStoresRequestRequestTypeDef",
+    {
+        "maxResults": int,
+        "nextToken": str,
+        "filter": SequenceStoreFilterTypeDef,
+    },
+    total=False,
+)
+
 ListAnnotationStoresResponseTypeDef = TypedDict(
     "ListAnnotationStoresResponseTypeDef",
     {
         "annotationStores": List[AnnotationStoreItemTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -3548,14 +3553,15 @@
 
 class CreateAnnotationStoreRequestRequestTypeDef(
     _RequiredCreateAnnotationStoreRequestRequestTypeDef,
     _OptionalCreateAnnotationStoreRequestRequestTypeDef,
 ):
     pass
 
+StoreOptionsUnionTypeDef = Union[StoreOptionsTypeDef, StoreOptionsOutputTypeDef]
 GetAnnotationImportResponseTypeDef = TypedDict(
     "GetAnnotationImportResponseTypeDef",
     {
         "id": str,
         "destinationName": str,
         "roleArn": str,
         "status": JobStatusType,
```

### Comparing `mypy-boto3-omics-1.28.16/mypy_boto3_omics/waiter.py` & `mypy-boto3-omics-1.28.16.post1/mypy_boto3_omics/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-omics-1.28.16/mypy_boto3_omics/waiter.pyi` & `mypy-boto3-omics-1.28.16.post1/mypy_boto3_omics/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-omics-1.28.16/mypy_boto3_omics.egg-info/PKG-INFO` & `mypy-boto3-omics-1.28.16.post1/mypy_boto3_omics.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-omics
-Version: 1.28.16
-Summary: Type annotations for boto3.Omics 1.28.16 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16.post1
+Summary: Type annotations for boto3.Omics 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 omics type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 omics type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -47,15 +47,15 @@
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
 [mypy-boto3-omics docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/).
 
 See how it helps to find and fix potential bugs:
 
@@ -75,15 +75,15 @@
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Waiters annotations](#waiters-annotations)
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
@@ -499,35 +499,36 @@
 )
 
 
 def check_value(value: AcceleratorsType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_omics.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_omics.type_defs import (
     AbortMultipartReadSetUploadRequestRequestTypeDef,
-    ActivateReadSetFilterTypeDef,
+    TimestampTypeDef,
     ActivateReadSetJobItemTypeDef,
     ActivateReadSetSourceItemTypeDef,
     AnnotationImportItemDetailTypeDef,
     AnnotationImportItemSourceTypeDef,
     AnnotationImportJobItemTypeDef,
     ReferenceItemTypeDef,
     SseConfigTypeDef,
     BatchDeleteReadSetRequestRequestTypeDef,
     ReadSetBatchErrorTypeDef,
     ResponseMetadataTypeDef,
+    BlobTypeDef,
     CancelAnnotationImportRequestRequestTypeDef,
     CancelRunRequestRequestTypeDef,
     CancelVariantImportRequestRequestTypeDef,
     CompleteReadSetUploadPartListItemTypeDef,
     CreateMultipartReadSetUploadRequestRequestTypeDef,
     CreateRunGroupRequestRequestTypeDef,
     WorkflowParameterTypeDef,
@@ -536,15 +537,14 @@
     DeleteReferenceStoreRequestRequestTypeDef,
     DeleteRunGroupRequestRequestTypeDef,
     DeleteRunRequestRequestTypeDef,
     DeleteSequenceStoreRequestRequestTypeDef,
     DeleteVariantStoreRequestRequestTypeDef,
     DeleteWorkflowRequestRequestTypeDef,
     ExportReadSetDetailTypeDef,
-    ExportReadSetFilterTypeDef,
     ExportReadSetJobDetailTypeDef,
     ExportReadSetTypeDef,
     FileInformationTypeDef,
     VcfOptionsTypeDef,
     WaiterConfigTypeDef,
     GetAnnotationImportRequestRequestTypeDef,
     GetAnnotationStoreRequestRequestTypeDef,
@@ -563,37 +563,30 @@
     GetRunRequestRequestTypeDef,
     GetRunTaskRequestRequestTypeDef,
     GetSequenceStoreRequestRequestTypeDef,
     GetVariantImportRequestRequestTypeDef,
     VariantImportItemDetailTypeDef,
     GetVariantStoreRequestRequestTypeDef,
     GetWorkflowRequestRequestTypeDef,
-    ImportReadSetFilterTypeDef,
     ImportReadSetJobItemTypeDef,
     SourceFilesTypeDef,
-    ImportReferenceFilterTypeDef,
     ImportReferenceJobItemTypeDef,
     ListAnnotationImportJobsFilterTypeDef,
     PaginatorConfigTypeDef,
     ListAnnotationStoresFilterTypeDef,
     ListMultipartReadSetUploadsRequestRequestTypeDef,
     MultipartReadSetUploadListItemTypeDef,
-    ReadSetUploadPartListFilterTypeDef,
     ReadSetUploadPartListItemTypeDef,
-    ReadSetFilterTypeDef,
-    ReferenceStoreFilterTypeDef,
-    ReferenceFilterTypeDef,
     ReferenceListItemTypeDef,
     ListRunGroupsRequestRequestTypeDef,
     RunGroupListItemTypeDef,
     ListRunTasksRequestRequestTypeDef,
     TaskListItemTypeDef,
     ListRunsRequestRequestTypeDef,
     RunListItemTypeDef,
-    SequenceStoreFilterTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListVariantImportJobsFilterTypeDef,
     VariantImportJobItemTypeDef,
     ListVariantStoresFilterTypeDef,
     ListWorkflowsRequestRequestTypeDef,
     WorkflowListItemTypeDef,
     ReadOptionsTypeDef,
@@ -605,16 +598,23 @@
     TsvStoreOptionsTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAnnotationStoreRequestRequestTypeDef,
     UpdateRunGroupRequestRequestTypeDef,
     UpdateVariantStoreRequestRequestTypeDef,
     UpdateWorkflowRequestRequestTypeDef,
-    UploadReadSetPartRequestRequestTypeDef,
-    ListReadSetActivationJobsRequestRequestTypeDef,
+    ActivateReadSetFilterTypeDef,
+    ExportReadSetFilterTypeDef,
+    ImportReadSetFilterTypeDef,
+    ImportReferenceFilterTypeDef,
+    ReadSetFilterTypeDef,
+    ReadSetUploadPartListFilterTypeDef,
+    ReferenceFilterTypeDef,
+    ReferenceStoreFilterTypeDef,
+    SequenceStoreFilterTypeDef,
     AnnotationStoreItemTypeDef,
     CreateReferenceStoreRequestRequestTypeDef,
     CreateSequenceStoreRequestRequestTypeDef,
     CreateVariantStoreRequestRequestTypeDef,
     ReferenceStoreDetailTypeDef,
     SequenceStoreDetailTypeDef,
     VariantStoreItemTypeDef,
@@ -646,19 +646,19 @@
     StartReadSetExportJobResponseTypeDef,
     StartReadSetImportJobResponseTypeDef,
     StartReferenceImportJobResponseTypeDef,
     StartRunResponseTypeDef,
     StartVariantImportResponseTypeDef,
     UpdateVariantStoreResponseTypeDef,
     UploadReadSetPartResponseTypeDef,
+    UploadReadSetPartRequestRequestTypeDef,
     CompleteMultipartReadSetUploadRequestRequestTypeDef,
     CreateWorkflowRequestRequestTypeDef,
     GetWorkflowResponseTypeDef,
     GetReadSetExportJobResponseTypeDef,
-    ListReadSetExportJobsRequestRequestTypeDef,
     ListReadSetExportJobsResponseTypeDef,
     StartReadSetExportJobRequestRequestTypeDef,
     ReadSetFilesTypeDef,
     ReferenceFilesTypeDef,
     GetAnnotationImportRequestAnnotationImportJobCreatedWaitTypeDef,
     GetAnnotationStoreRequestAnnotationStoreCreatedWaitTypeDef,
     GetAnnotationStoreRequestAnnotationStoreDeletedWaitTypeDef,
@@ -673,81 +673,84 @@
     GetVariantImportRequestVariantImportJobCreatedWaitTypeDef,
     GetVariantStoreRequestVariantStoreCreatedWaitTypeDef,
     GetVariantStoreRequestVariantStoreDeletedWaitTypeDef,
     GetWorkflowRequestWorkflowActiveWaitTypeDef,
     ReadSetListItemTypeDef,
     GetReferenceImportJobResponseTypeDef,
     GetVariantImportResponseTypeDef,
-    ListReadSetImportJobsRequestRequestTypeDef,
     ListReadSetImportJobsResponseTypeDef,
     ImportReadSetSourceItemTypeDef,
     StartReadSetImportJobSourceItemTypeDef,
-    ListReferenceImportJobsRequestRequestTypeDef,
     ListReferenceImportJobsResponseTypeDef,
     ListAnnotationImportJobsRequestRequestTypeDef,
     ListAnnotationImportJobsRequestListAnnotationImportJobsPaginateTypeDef,
     ListMultipartReadSetUploadsRequestListMultipartReadSetUploadsPaginateTypeDef,
-    ListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef,
-    ListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef,
-    ListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef,
-    ListReferenceImportJobsRequestListReferenceImportJobsPaginateTypeDef,
     ListRunGroupsRequestListRunGroupsPaginateTypeDef,
     ListRunTasksRequestListRunTasksPaginateTypeDef,
     ListRunsRequestListRunsPaginateTypeDef,
     ListWorkflowsRequestListWorkflowsPaginateTypeDef,
     ListAnnotationStoresRequestListAnnotationStoresPaginateTypeDef,
     ListAnnotationStoresRequestRequestTypeDef,
     ListMultipartReadSetUploadsResponseTypeDef,
-    ListReadSetUploadPartsRequestListReadSetUploadPartsPaginateTypeDef,
-    ListReadSetUploadPartsRequestRequestTypeDef,
     ListReadSetUploadPartsResponseTypeDef,
-    ListReadSetsRequestListReadSetsPaginateTypeDef,
-    ListReadSetsRequestRequestTypeDef,
-    ListReferenceStoresRequestListReferenceStoresPaginateTypeDef,
-    ListReferenceStoresRequestRequestTypeDef,
-    ListReferencesRequestListReferencesPaginateTypeDef,
-    ListReferencesRequestRequestTypeDef,
     ListReferencesResponseTypeDef,
     ListRunGroupsResponseTypeDef,
     ListRunTasksResponseTypeDef,
     ListRunsResponseTypeDef,
-    ListSequenceStoresRequestListSequenceStoresPaginateTypeDef,
-    ListSequenceStoresRequestRequestTypeDef,
     ListVariantImportJobsRequestListVariantImportJobsPaginateTypeDef,
     ListVariantImportJobsRequestRequestTypeDef,
     ListVariantImportJobsResponseTypeDef,
     ListVariantStoresRequestListVariantStoresPaginateTypeDef,
     ListVariantStoresRequestRequestTypeDef,
     ListWorkflowsResponseTypeDef,
     TsvOptionsTypeDef,
     StartReadSetActivationJobRequestRequestTypeDef,
     StartReferenceImportJobRequestRequestTypeDef,
     StartVariantImportRequestRequestTypeDef,
     StoreOptionsOutputTypeDef,
     StoreOptionsTypeDef,
+    ListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef,
+    ListReadSetActivationJobsRequestRequestTypeDef,
+    ListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef,
+    ListReadSetExportJobsRequestRequestTypeDef,
+    ListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef,
+    ListReadSetImportJobsRequestRequestTypeDef,
+    ListReferenceImportJobsRequestListReferenceImportJobsPaginateTypeDef,
+    ListReferenceImportJobsRequestRequestTypeDef,
+    ListReadSetsRequestListReadSetsPaginateTypeDef,
+    ListReadSetsRequestRequestTypeDef,
+    ListReadSetUploadPartsRequestListReadSetUploadPartsPaginateTypeDef,
+    ListReadSetUploadPartsRequestRequestTypeDef,
+    ListReferencesRequestListReferencesPaginateTypeDef,
+    ListReferencesRequestRequestTypeDef,
+    ListReferenceStoresRequestListReferenceStoresPaginateTypeDef,
+    ListReferenceStoresRequestRequestTypeDef,
+    ListSequenceStoresRequestListSequenceStoresPaginateTypeDef,
+    ListSequenceStoresRequestRequestTypeDef,
     ListAnnotationStoresResponseTypeDef,
     ListReferenceStoresResponseTypeDef,
     ListSequenceStoresResponseTypeDef,
     ListVariantStoresResponseTypeDef,
     GetReadSetMetadataResponseTypeDef,
     GetReferenceMetadataResponseTypeDef,
     ListReadSetsResponseTypeDef,
     GetReadSetImportJobResponseTypeDef,
     StartReadSetImportJobRequestRequestTypeDef,
     FormatOptionsTypeDef,
     CreateAnnotationStoreResponseTypeDef,
     GetAnnotationStoreResponseTypeDef,
     UpdateAnnotationStoreResponseTypeDef,
     CreateAnnotationStoreRequestRequestTypeDef,
+    StoreOptionsUnionTypeDef,
     GetAnnotationImportResponseTypeDef,
     StartAnnotationImportRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AbortMultipartReadSetUploadRequestRequestTypeDef:
+def get_value() -> AbortMultipartReadSetUploadRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-omics-1.28.16/mypy_boto3_omics.egg-info/SOURCES.txt` & `mypy-boto3-omics-1.28.16.post1/mypy_boto3_omics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-omics-1.28.16/setup.py` & `mypy-boto3-omics-1.28.16.post1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-omics",
-    version="1.28.16",
+    version="1.28.16.post1",
     packages=["mypy_boto3_omics"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Omics 1.28.16 service generated with mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.Omics 1.28.16 service generated with mypy-boto3-builder 7.17.1"
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
-    keywords="boto3 omics type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 omics type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_omics": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

