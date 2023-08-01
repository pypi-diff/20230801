# Comparing `tmp/mypy-boto3-clouddirectory-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-clouddirectory-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-clouddirectory-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:41 2023, max compression
+gzip compressed data, was "mypy-boto3-clouddirectory-1.28.16.tar", last modified: Tue Aug  1 11:36:22 2023, max compression
```

## Comparing `mypy-boto3-clouddirectory-1.28.15.post1.tar` & `mypy-boto3-clouddirectory-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:41.477050 mypy-boto3-clouddirectory-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:39:45.000000 mypy-boto3-clouddirectory-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    26164 2023-07-29 10:02:41.469050 mypy-boto3-clouddirectory-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    24643 2023-07-29 09:39:45.000000 mypy-boto3-clouddirectory-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:41.465050 mypy-boto3-clouddirectory-1.28.15.post1/mypy_boto3_clouddirectory/
--rw-r--r--   0 runner    (1001) docker     (123)     4770 2023-07-29 09:39:45.000000 mypy-boto3-clouddirectory-1.28.15.post1/mypy_boto3_clouddirectory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-07-29 09:39:45.000000 mypy-boto3-clouddirectory-1.28.15.post1/mypy_boto3_clouddirectory/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-29 09:39:45.000000 mypy-boto3-clouddirectory-1.28.15.post1/mypy_boto3_clouddirectory/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    57281 2023-07-29 09:39:46.000000 mypy-boto3-clouddirectory-1.28.15.post1/mypy_boto3_clouddirectory/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    57189 2023-07-29 09:39:46.000000 mypy-boto3-clouddirectory-1.28.15.post1/mypy_boto3_clouddirectory/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11952 2023-07-29 09:39:46.000000 mypy-boto3-clouddirectory-1.28.15.post1/mypy_boto3_clouddirectory/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11950 2023-07-29 09:39:46.000000 mypy-boto3-clouddirectory-1.28.15.post1/mypy_boto3_clouddirectory/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    24350 2023-07-29 09:39:46.000000 mypy-boto3-clouddirectory-1.28.15.post1/mypy_boto3_clouddirectory/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    24329 2023-07-29 09:39:46.000000 mypy-boto3-clouddirectory-1.28.15.post1/mypy_boto3_clouddirectory/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:39:45.000000 mypy-boto3-clouddirectory-1.28.15.post1/mypy_boto3_clouddirectory/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    90060 2023-07-29 09:39:50.000000 mypy-boto3-clouddirectory-1.28.15.post1/mypy_boto3_clouddirectory/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    89927 2023-07-29 09:39:48.000000 mypy-boto3-clouddirectory-1.28.15.post1/mypy_boto3_clouddirectory/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:39:45.000000 mypy-boto3-clouddirectory-1.28.15.post1/mypy_boto3_clouddirectory/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:41.469050 mypy-boto3-clouddirectory-1.28.15.post1/mypy_boto3_clouddirectory.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    26164 2023-07-29 10:02:41.000000 mypy-boto3-clouddirectory-1.28.15.post1/mypy_boto3_clouddirectory.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-29 10:02:41.000000 mypy-boto3-clouddirectory-1.28.15.post1/mypy_boto3_clouddirectory.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:41.000000 mypy-boto3-clouddirectory-1.28.15.post1/mypy_boto3_clouddirectory.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:41.000000 mypy-boto3-clouddirectory-1.28.15.post1/mypy_boto3_clouddirectory.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:41.000000 mypy-boto3-clouddirectory-1.28.15.post1/mypy_boto3_clouddirectory.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-29 10:02:41.000000 mypy-boto3-clouddirectory-1.28.15.post1/mypy_boto3_clouddirectory.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:41.477050 mypy-boto3-clouddirectory-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-07-29 09:39:45.000000 mypy-boto3-clouddirectory-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:22.208934 mypy-boto3-clouddirectory-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:12:18.000000 mypy-boto3-clouddirectory-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    26338 2023-08-01 11:36:22.208934 mypy-boto3-clouddirectory-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    24826 2023-08-01 11:12:18.000000 mypy-boto3-clouddirectory-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:22.204934 mypy-boto3-clouddirectory-1.28.16/mypy_boto3_clouddirectory/
+-rw-r--r--   0 runner    (1001) docker     (123)     4770 2023-08-01 11:12:18.000000 mypy-boto3-clouddirectory-1.28.16/mypy_boto3_clouddirectory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-08-01 11:12:18.000000 mypy-boto3-clouddirectory-1.28.16/mypy_boto3_clouddirectory/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-08-01 11:12:18.000000 mypy-boto3-clouddirectory-1.28.16/mypy_boto3_clouddirectory/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56807 2023-08-01 11:12:19.000000 mypy-boto3-clouddirectory-1.28.16/mypy_boto3_clouddirectory/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56715 2023-08-01 11:12:18.000000 mypy-boto3-clouddirectory-1.28.16/mypy_boto3_clouddirectory/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11952 2023-08-01 11:12:20.000000 mypy-boto3-clouddirectory-1.28.16/mypy_boto3_clouddirectory/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11950 2023-08-01 11:12:20.000000 mypy-boto3-clouddirectory-1.28.16/mypy_boto3_clouddirectory/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    24350 2023-08-01 11:12:20.000000 mypy-boto3-clouddirectory-1.28.16/mypy_boto3_clouddirectory/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24329 2023-08-01 11:12:20.000000 mypy-boto3-clouddirectory-1.28.16/mypy_boto3_clouddirectory/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:12:18.000000 mypy-boto3-clouddirectory-1.28.16/mypy_boto3_clouddirectory/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    90517 2023-08-01 11:12:22.000000 mypy-boto3-clouddirectory-1.28.16/mypy_boto3_clouddirectory/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    90385 2023-08-01 11:12:21.000000 mypy-boto3-clouddirectory-1.28.16/mypy_boto3_clouddirectory/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:12:18.000000 mypy-boto3-clouddirectory-1.28.16/mypy_boto3_clouddirectory/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:22.208934 mypy-boto3-clouddirectory-1.28.16/mypy_boto3_clouddirectory.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    26338 2023-08-01 11:36:21.000000 mypy-boto3-clouddirectory-1.28.16/mypy_boto3_clouddirectory.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-08-01 11:36:22.000000 mypy-boto3-clouddirectory-1.28.16/mypy_boto3_clouddirectory.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:21.000000 mypy-boto3-clouddirectory-1.28.16/mypy_boto3_clouddirectory.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:21.000000 mypy-boto3-clouddirectory-1.28.16/mypy_boto3_clouddirectory.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:21.000000 mypy-boto3-clouddirectory-1.28.16/mypy_boto3_clouddirectory.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-01 11:36:21.000000 mypy-boto3-clouddirectory-1.28.16/mypy_boto3_clouddirectory.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:22.208934 mypy-boto3-clouddirectory-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-08-01 11:12:18.000000 mypy-boto3-clouddirectory-1.28.16/setup.py
```

### Comparing `mypy-boto3-clouddirectory-1.28.15.post1/LICENSE` & `mypy-boto3-clouddirectory-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-clouddirectory-1.28.15.post1/PKG-INFO` & `mypy-boto3-clouddirectory-1.28.16/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-clouddirectory
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.CloudDirectory 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.CloudDirectory 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 clouddirectory type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 clouddirectory type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-clouddirectory.svg?color=blue)](https://pypi.org/project/mypy-boto3-clouddirectory)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-clouddirectory)](https://pepy.tech/project/mypy-boto3-clouddirectory)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudDirectory 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory)
+[boto3.CloudDirectory 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory)
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
 [mypy-boto3-clouddirectory docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/).
 
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
@@ -407,44 +407,44 @@
 )
 
 
 def check_value(value: BatchReadExceptionTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_clouddirectory.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_clouddirectory.type_defs import (
     ObjectReferenceTypeDef,
     SchemaFacetTypeDef,
     ApplySchemaRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     TypedLinkSchemaAndFacetNameTypeDef,
     AttributeKeyTypeDef,
     TypedAttributeValueOutputTypeDef,
-    TypedAttributeValueTypeDef,
     BatchAttachObjectResponseTypeDef,
     BatchAttachToIndexResponseTypeDef,
     BatchCreateIndexResponseTypeDef,
     BatchCreateObjectResponseTypeDef,
     BatchDetachFromIndexResponseTypeDef,
     BatchDetachObjectResponseTypeDef,
     BatchListObjectChildrenResponseTypeDef,
     PathToObjectIdentifiersTypeDef,
     ObjectIdentifierAndLinkNameTupleTypeDef,
     BatchListObjectPoliciesResponseTypeDef,
     BatchListPolicyAttachmentsResponseTypeDef,
     BatchReadExceptionTypeDef,
     BatchUpdateObjectAttributesResponseTypeDef,
+    BlobTypeDef,
     CreateDirectoryRequestRequestTypeDef,
     CreateSchemaRequestRequestTypeDef,
     DeleteDirectoryRequestRequestTypeDef,
     DeleteFacetRequestRequestTypeDef,
     DeleteSchemaRequestRequestTypeDef,
     DeleteTypedLinkFacetRequestRequestTypeDef,
     DirectoryTypeDef,
@@ -470,14 +470,15 @@
     ListTagsForResourceRequestRequestTypeDef,
     TagTypeDef,
     ListTypedLinkFacetAttributesRequestRequestTypeDef,
     ListTypedLinkFacetNamesRequestRequestTypeDef,
     PolicyAttachmentTypeDef,
     PublishSchemaRequestRequestTypeDef,
     PutSchemaFromJsonRequestRequestTypeDef,
+    TimestampTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateSchemaRequestRequestTypeDef,
     UpgradeAppliedSchemaRequestRequestTypeDef,
     UpgradePublishedSchemaRequestRequestTypeDef,
     AttachObjectRequestRequestTypeDef,
     AttachPolicyRequestRequestTypeDef,
     AttachToIndexRequestRequestTypeDef,
@@ -548,29 +549,22 @@
     UpdateSchemaResponseTypeDef,
     UpgradeAppliedSchemaResponseTypeDef,
     UpgradePublishedSchemaResponseTypeDef,
     BatchCreateIndexTypeDef,
     CreateIndexRequestRequestTypeDef,
     AttributeKeyAndValueOutputTypeDef,
     AttributeNameAndValueOutputTypeDef,
-    AttributeKeyAndValueTypeDef,
-    AttributeNameAndValueTypeDef,
-    LinkAttributeActionTypeDef,
-    ObjectAttributeActionTypeDef,
-    TypedAttributeValueRangeTypeDef,
     BatchListObjectParentPathsResponseTypeDef,
     ListObjectParentPathsResponseTypeDef,
     BatchListObjectParentsResponseTypeDef,
     ListObjectParentsResponseTypeDef,
     GetDirectoryResponseTypeDef,
     ListDirectoriesResponseTypeDef,
     FacetAttributeDefinitionOutputTypeDef,
     TypedLinkAttributeDefinitionOutputTypeDef,
-    FacetAttributeDefinitionTypeDef,
-    TypedLinkAttributeDefinitionTypeDef,
     GetFacetResponseTypeDef,
     ListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef,
     ListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef,
     ListDevelopmentSchemaArnsRequestListDevelopmentSchemaArnsPaginateTypeDef,
     ListDirectoriesRequestListDirectoriesPaginateTypeDef,
     ListFacetAttributesRequestListFacetAttributesPaginateTypeDef,
     ListFacetNamesRequestListFacetNamesPaginateTypeDef,
@@ -583,86 +577,98 @@
     ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef,
     ListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef,
     LookupPolicyRequestLookupPolicyPaginateTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     PolicyToPathTypeDef,
+    TypedAttributeValueTypeDef,
     BatchGetLinkAttributesResponseTypeDef,
     BatchGetObjectAttributesResponseTypeDef,
     BatchListObjectAttributesResponseTypeDef,
     GetLinkAttributesResponseTypeDef,
     GetObjectAttributesResponseTypeDef,
     IndexAttachmentTypeDef,
     ListObjectAttributesResponseTypeDef,
     TypedLinkSpecifierOutputTypeDef,
-    AddFacetToObjectRequestRequestTypeDef,
-    BatchAddFacetToObjectTypeDef,
-    BatchCreateObjectTypeDef,
-    CreateObjectRequestRequestTypeDef,
-    AttachTypedLinkRequestRequestTypeDef,
-    BatchAttachTypedLinkTypeDef,
-    TypedLinkSpecifierTypeDef,
-    LinkAttributeUpdateTypeDef,
-    ObjectAttributeUpdateTypeDef,
-    ObjectAttributeRangeTypeDef,
-    TypedLinkAttributeRangeTypeDef,
     FacetAttributeOutputTypeDef,
     ListTypedLinkFacetAttributesResponseTypeDef,
-    FacetAttributeTypeDef,
-    TypedLinkFacetAttributeUpdateTypeDef,
-    TypedLinkFacetTypeDef,
     BatchLookupPolicyResponseTypeDef,
     LookupPolicyResponseTypeDef,
+    AttributeKeyAndValueTypeDef,
+    AttributeNameAndValueTypeDef,
+    FacetAttributeDefinitionTypeDef,
+    LinkAttributeActionTypeDef,
+    ObjectAttributeActionTypeDef,
+    TypedAttributeValueRangeTypeDef,
+    TypedLinkAttributeDefinitionTypeDef,
     BatchListAttachedIndicesResponseTypeDef,
     BatchListIndexResponseTypeDef,
     ListAttachedIndicesResponseTypeDef,
     ListIndexResponseTypeDef,
     AttachTypedLinkResponseTypeDef,
     BatchAttachTypedLinkResponseTypeDef,
     BatchListIncomingTypedLinksResponseTypeDef,
     BatchListOutgoingTypedLinksResponseTypeDef,
     ListIncomingTypedLinksResponseTypeDef,
     ListOutgoingTypedLinksResponseTypeDef,
+    ListFacetAttributesResponseTypeDef,
+    AttributeKeyAndValueUnionTypeDef,
+    BatchAddFacetToObjectTypeDef,
+    BatchCreateObjectTypeDef,
+    AttributeNameAndValueUnionTypeDef,
+    BatchAttachTypedLinkTypeDef,
+    TypedLinkSpecifierTypeDef,
+    FacetAttributeTypeDef,
+    LinkAttributeUpdateTypeDef,
+    ObjectAttributeUpdateTypeDef,
+    ObjectAttributeRangeTypeDef,
+    TypedLinkAttributeRangeTypeDef,
+    TypedLinkFacetAttributeUpdateTypeDef,
+    TypedLinkFacetTypeDef,
+    BatchWriteOperationResponseTypeDef,
+    BatchReadSuccessfulResponseTypeDef,
+    AddFacetToObjectRequestRequestTypeDef,
+    CreateObjectRequestRequestTypeDef,
+    AttachTypedLinkRequestRequestTypeDef,
     BatchDetachTypedLinkTypeDef,
     BatchGetLinkAttributesTypeDef,
     DetachTypedLinkRequestRequestTypeDef,
     GetLinkAttributesRequestRequestTypeDef,
+    TypedLinkSpecifierUnionTypeDef,
+    FacetAttributeUnionTypeDef,
+    FacetAttributeUpdateTypeDef,
     BatchUpdateLinkAttributesTypeDef,
     UpdateLinkAttributesRequestRequestTypeDef,
     BatchUpdateObjectAttributesTypeDef,
     UpdateObjectAttributesRequestRequestTypeDef,
     BatchListIndexTypeDef,
     ListIndexRequestListIndexPaginateTypeDef,
     ListIndexRequestRequestTypeDef,
     BatchListIncomingTypedLinksTypeDef,
     BatchListOutgoingTypedLinksTypeDef,
     ListIncomingTypedLinksRequestListIncomingTypedLinksPaginateTypeDef,
     ListIncomingTypedLinksRequestRequestTypeDef,
     ListOutgoingTypedLinksRequestListOutgoingTypedLinksPaginateTypeDef,
     ListOutgoingTypedLinksRequestRequestTypeDef,
-    ListFacetAttributesResponseTypeDef,
-    CreateFacetRequestRequestTypeDef,
-    FacetAttributeUpdateTypeDef,
     UpdateTypedLinkFacetRequestRequestTypeDef,
     CreateTypedLinkFacetRequestRequestTypeDef,
-    BatchWriteOperationResponseTypeDef,
-    BatchReadSuccessfulResponseTypeDef,
-    BatchWriteOperationTypeDef,
-    BatchReadOperationTypeDef,
-    UpdateFacetRequestRequestTypeDef,
     BatchWriteResponseTypeDef,
     BatchReadOperationResponseTypeDef,
+    CreateFacetRequestRequestTypeDef,
+    UpdateFacetRequestRequestTypeDef,
+    BatchWriteOperationTypeDef,
+    BatchReadOperationTypeDef,
+    BatchReadResponseTypeDef,
     BatchWriteRequestRequestTypeDef,
     BatchReadRequestRequestTypeDef,
-    BatchReadResponseTypeDef,
 )
 
 
-def get_structure() -> ObjectReferenceTypeDef:
+def get_value() -> ObjectReferenceTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-clouddirectory-1.28.15.post1/README.md` & `mypy-boto3-clouddirectory-1.28.16/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-clouddirectory.svg?color=blue)](https://pypi.org/project/mypy-boto3-clouddirectory)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-clouddirectory)](https://pepy.tech/project/mypy-boto3-clouddirectory)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudDirectory 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory)
+[boto3.CloudDirectory 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory)
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
 [mypy-boto3-clouddirectory docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/).
 
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
@@ -375,44 +375,44 @@
 )
 
 
 def check_value(value: BatchReadExceptionTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_clouddirectory.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_clouddirectory.type_defs import (
     ObjectReferenceTypeDef,
     SchemaFacetTypeDef,
     ApplySchemaRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     TypedLinkSchemaAndFacetNameTypeDef,
     AttributeKeyTypeDef,
     TypedAttributeValueOutputTypeDef,
-    TypedAttributeValueTypeDef,
     BatchAttachObjectResponseTypeDef,
     BatchAttachToIndexResponseTypeDef,
     BatchCreateIndexResponseTypeDef,
     BatchCreateObjectResponseTypeDef,
     BatchDetachFromIndexResponseTypeDef,
     BatchDetachObjectResponseTypeDef,
     BatchListObjectChildrenResponseTypeDef,
     PathToObjectIdentifiersTypeDef,
     ObjectIdentifierAndLinkNameTupleTypeDef,
     BatchListObjectPoliciesResponseTypeDef,
     BatchListPolicyAttachmentsResponseTypeDef,
     BatchReadExceptionTypeDef,
     BatchUpdateObjectAttributesResponseTypeDef,
+    BlobTypeDef,
     CreateDirectoryRequestRequestTypeDef,
     CreateSchemaRequestRequestTypeDef,
     DeleteDirectoryRequestRequestTypeDef,
     DeleteFacetRequestRequestTypeDef,
     DeleteSchemaRequestRequestTypeDef,
     DeleteTypedLinkFacetRequestRequestTypeDef,
     DirectoryTypeDef,
@@ -438,14 +438,15 @@
     ListTagsForResourceRequestRequestTypeDef,
     TagTypeDef,
     ListTypedLinkFacetAttributesRequestRequestTypeDef,
     ListTypedLinkFacetNamesRequestRequestTypeDef,
     PolicyAttachmentTypeDef,
     PublishSchemaRequestRequestTypeDef,
     PutSchemaFromJsonRequestRequestTypeDef,
+    TimestampTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateSchemaRequestRequestTypeDef,
     UpgradeAppliedSchemaRequestRequestTypeDef,
     UpgradePublishedSchemaRequestRequestTypeDef,
     AttachObjectRequestRequestTypeDef,
     AttachPolicyRequestRequestTypeDef,
     AttachToIndexRequestRequestTypeDef,
@@ -516,29 +517,22 @@
     UpdateSchemaResponseTypeDef,
     UpgradeAppliedSchemaResponseTypeDef,
     UpgradePublishedSchemaResponseTypeDef,
     BatchCreateIndexTypeDef,
     CreateIndexRequestRequestTypeDef,
     AttributeKeyAndValueOutputTypeDef,
     AttributeNameAndValueOutputTypeDef,
-    AttributeKeyAndValueTypeDef,
-    AttributeNameAndValueTypeDef,
-    LinkAttributeActionTypeDef,
-    ObjectAttributeActionTypeDef,
-    TypedAttributeValueRangeTypeDef,
     BatchListObjectParentPathsResponseTypeDef,
     ListObjectParentPathsResponseTypeDef,
     BatchListObjectParentsResponseTypeDef,
     ListObjectParentsResponseTypeDef,
     GetDirectoryResponseTypeDef,
     ListDirectoriesResponseTypeDef,
     FacetAttributeDefinitionOutputTypeDef,
     TypedLinkAttributeDefinitionOutputTypeDef,
-    FacetAttributeDefinitionTypeDef,
-    TypedLinkAttributeDefinitionTypeDef,
     GetFacetResponseTypeDef,
     ListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef,
     ListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef,
     ListDevelopmentSchemaArnsRequestListDevelopmentSchemaArnsPaginateTypeDef,
     ListDirectoriesRequestListDirectoriesPaginateTypeDef,
     ListFacetAttributesRequestListFacetAttributesPaginateTypeDef,
     ListFacetNamesRequestListFacetNamesPaginateTypeDef,
@@ -551,86 +545,98 @@
     ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef,
     ListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef,
     LookupPolicyRequestLookupPolicyPaginateTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     PolicyToPathTypeDef,
+    TypedAttributeValueTypeDef,
     BatchGetLinkAttributesResponseTypeDef,
     BatchGetObjectAttributesResponseTypeDef,
     BatchListObjectAttributesResponseTypeDef,
     GetLinkAttributesResponseTypeDef,
     GetObjectAttributesResponseTypeDef,
     IndexAttachmentTypeDef,
     ListObjectAttributesResponseTypeDef,
     TypedLinkSpecifierOutputTypeDef,
-    AddFacetToObjectRequestRequestTypeDef,
-    BatchAddFacetToObjectTypeDef,
-    BatchCreateObjectTypeDef,
-    CreateObjectRequestRequestTypeDef,
-    AttachTypedLinkRequestRequestTypeDef,
-    BatchAttachTypedLinkTypeDef,
-    TypedLinkSpecifierTypeDef,
-    LinkAttributeUpdateTypeDef,
-    ObjectAttributeUpdateTypeDef,
-    ObjectAttributeRangeTypeDef,
-    TypedLinkAttributeRangeTypeDef,
     FacetAttributeOutputTypeDef,
     ListTypedLinkFacetAttributesResponseTypeDef,
-    FacetAttributeTypeDef,
-    TypedLinkFacetAttributeUpdateTypeDef,
-    TypedLinkFacetTypeDef,
     BatchLookupPolicyResponseTypeDef,
     LookupPolicyResponseTypeDef,
+    AttributeKeyAndValueTypeDef,
+    AttributeNameAndValueTypeDef,
+    FacetAttributeDefinitionTypeDef,
+    LinkAttributeActionTypeDef,
+    ObjectAttributeActionTypeDef,
+    TypedAttributeValueRangeTypeDef,
+    TypedLinkAttributeDefinitionTypeDef,
     BatchListAttachedIndicesResponseTypeDef,
     BatchListIndexResponseTypeDef,
     ListAttachedIndicesResponseTypeDef,
     ListIndexResponseTypeDef,
     AttachTypedLinkResponseTypeDef,
     BatchAttachTypedLinkResponseTypeDef,
     BatchListIncomingTypedLinksResponseTypeDef,
     BatchListOutgoingTypedLinksResponseTypeDef,
     ListIncomingTypedLinksResponseTypeDef,
     ListOutgoingTypedLinksResponseTypeDef,
+    ListFacetAttributesResponseTypeDef,
+    AttributeKeyAndValueUnionTypeDef,
+    BatchAddFacetToObjectTypeDef,
+    BatchCreateObjectTypeDef,
+    AttributeNameAndValueUnionTypeDef,
+    BatchAttachTypedLinkTypeDef,
+    TypedLinkSpecifierTypeDef,
+    FacetAttributeTypeDef,
+    LinkAttributeUpdateTypeDef,
+    ObjectAttributeUpdateTypeDef,
+    ObjectAttributeRangeTypeDef,
+    TypedLinkAttributeRangeTypeDef,
+    TypedLinkFacetAttributeUpdateTypeDef,
+    TypedLinkFacetTypeDef,
+    BatchWriteOperationResponseTypeDef,
+    BatchReadSuccessfulResponseTypeDef,
+    AddFacetToObjectRequestRequestTypeDef,
+    CreateObjectRequestRequestTypeDef,
+    AttachTypedLinkRequestRequestTypeDef,
     BatchDetachTypedLinkTypeDef,
     BatchGetLinkAttributesTypeDef,
     DetachTypedLinkRequestRequestTypeDef,
     GetLinkAttributesRequestRequestTypeDef,
+    TypedLinkSpecifierUnionTypeDef,
+    FacetAttributeUnionTypeDef,
+    FacetAttributeUpdateTypeDef,
     BatchUpdateLinkAttributesTypeDef,
     UpdateLinkAttributesRequestRequestTypeDef,
     BatchUpdateObjectAttributesTypeDef,
     UpdateObjectAttributesRequestRequestTypeDef,
     BatchListIndexTypeDef,
     ListIndexRequestListIndexPaginateTypeDef,
     ListIndexRequestRequestTypeDef,
     BatchListIncomingTypedLinksTypeDef,
     BatchListOutgoingTypedLinksTypeDef,
     ListIncomingTypedLinksRequestListIncomingTypedLinksPaginateTypeDef,
     ListIncomingTypedLinksRequestRequestTypeDef,
     ListOutgoingTypedLinksRequestListOutgoingTypedLinksPaginateTypeDef,
     ListOutgoingTypedLinksRequestRequestTypeDef,
-    ListFacetAttributesResponseTypeDef,
-    CreateFacetRequestRequestTypeDef,
-    FacetAttributeUpdateTypeDef,
     UpdateTypedLinkFacetRequestRequestTypeDef,
     CreateTypedLinkFacetRequestRequestTypeDef,
-    BatchWriteOperationResponseTypeDef,
-    BatchReadSuccessfulResponseTypeDef,
-    BatchWriteOperationTypeDef,
-    BatchReadOperationTypeDef,
-    UpdateFacetRequestRequestTypeDef,
     BatchWriteResponseTypeDef,
     BatchReadOperationResponseTypeDef,
+    CreateFacetRequestRequestTypeDef,
+    UpdateFacetRequestRequestTypeDef,
+    BatchWriteOperationTypeDef,
+    BatchReadOperationTypeDef,
+    BatchReadResponseTypeDef,
     BatchWriteRequestRequestTypeDef,
     BatchReadRequestRequestTypeDef,
-    BatchReadResponseTypeDef,
 )
 
 
-def get_structure() -> ObjectReferenceTypeDef:
+def get_value() -> ObjectReferenceTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-clouddirectory-1.28.15.post1/mypy_boto3_clouddirectory/__init__.py` & `mypy-boto3-clouddirectory-1.28.16/mypy_boto3_clouddirectory/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-clouddirectory-1.28.15.post1/mypy_boto3_clouddirectory/__init__.pyi` & `mypy-boto3-clouddirectory-1.28.16/mypy_boto3_clouddirectory/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-clouddirectory-1.28.15.post1/mypy_boto3_clouddirectory/__main__.py` & `mypy-boto3-clouddirectory-1.28.16/mypy_boto3_clouddirectory/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CloudDirectory 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.CloudDirectory 1.28.16\nVersion:         1.28.16\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory\nOther"
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

### Comparing `mypy-boto3-clouddirectory-1.28.15.post1/mypy_boto3_clouddirectory/client.py` & `mypy-boto3-clouddirectory-1.28.16/mypy_boto3_clouddirectory/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_clouddirectory.client import CloudDirectoryClient
 
     session = Session()
     client: CloudDirectoryClient = session.client("clouddirectory")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import ConsistencyLevelType, DirectoryStateType, FacetStyleType, ObjectTypeType
 from .paginator import (
     ListAppliedSchemaArnsPaginator,
     ListAttachedIndicesPaginator,
@@ -41,19 +41,17 @@
     LookupPolicyPaginator,
 )
 from .type_defs import (
     ApplySchemaResponseTypeDef,
     AttachObjectResponseTypeDef,
     AttachToIndexResponseTypeDef,
     AttachTypedLinkResponseTypeDef,
-    AttributeKeyAndValueOutputTypeDef,
-    AttributeKeyAndValueTypeDef,
+    AttributeKeyAndValueUnionTypeDef,
     AttributeKeyTypeDef,
-    AttributeNameAndValueOutputTypeDef,
-    AttributeNameAndValueTypeDef,
+    AttributeNameAndValueUnionTypeDef,
     BatchReadOperationTypeDef,
     BatchReadResponseTypeDef,
     BatchWriteOperationTypeDef,
     BatchWriteResponseTypeDef,
     CreateDirectoryResponseTypeDef,
     CreateIndexResponseTypeDef,
     CreateObjectResponseTypeDef,
@@ -61,16 +59,15 @@
     DeleteDirectoryResponseTypeDef,
     DeleteSchemaResponseTypeDef,
     DetachFromIndexResponseTypeDef,
     DetachObjectResponseTypeDef,
     DisableDirectoryResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     EnableDirectoryResponseTypeDef,
-    FacetAttributeOutputTypeDef,
-    FacetAttributeTypeDef,
+    FacetAttributeUnionTypeDef,
     FacetAttributeUpdateTypeDef,
     GetAppliedSchemaVersionResponseTypeDef,
     GetDirectoryResponseTypeDef,
     GetFacetResponseTypeDef,
     GetLinkAttributesResponseTypeDef,
     GetObjectAttributesResponseTypeDef,
     GetObjectInformationResponseTypeDef,
@@ -105,16 +102,15 @@
     PutSchemaFromJsonResponseTypeDef,
     SchemaFacetTypeDef,
     TagTypeDef,
     TypedLinkAttributeRangeTypeDef,
     TypedLinkFacetAttributeUpdateTypeDef,
     TypedLinkFacetTypeDef,
     TypedLinkSchemaAndFacetNameTypeDef,
-    TypedLinkSpecifierOutputTypeDef,
-    TypedLinkSpecifierTypeDef,
+    TypedLinkSpecifierUnionTypeDef,
     UpdateObjectAttributesResponseTypeDef,
     UpdateSchemaResponseTypeDef,
     UpgradeAppliedSchemaResponseTypeDef,
     UpgradePublishedSchemaResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
@@ -192,17 +188,15 @@
 
     def add_facet_to_object(
         self,
         *,
         DirectoryArn: str,
         SchemaFacet: SchemaFacetTypeDef,
         ObjectReference: ObjectReferenceTypeDef,
-        ObjectAttributeList: Sequence[
-            Union[AttributeKeyAndValueTypeDef, AttributeKeyAndValueOutputTypeDef]
-        ] = ...
+        ObjectAttributeList: Sequence[AttributeKeyAndValueUnionTypeDef] = ...
     ) -> Dict[str, Any]:
         """
         Adds a new  Facet to an object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.add_facet_to_object)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/client/#add_facet_to_object)
         """
@@ -264,17 +258,15 @@
     def attach_typed_link(
         self,
         *,
         DirectoryArn: str,
         SourceObjectReference: ObjectReferenceTypeDef,
         TargetObjectReference: ObjectReferenceTypeDef,
         TypedLinkFacet: TypedLinkSchemaAndFacetNameTypeDef,
-        Attributes: Sequence[
-            Union[AttributeNameAndValueTypeDef, AttributeNameAndValueOutputTypeDef]
-        ]
+        Attributes: Sequence[AttributeNameAndValueUnionTypeDef]
     ) -> AttachTypedLinkResponseTypeDef:
         """
         Attaches a typed link to a specified source and target object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.attach_typed_link)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/client/#attach_typed_link)
         """
@@ -328,15 +320,15 @@
         """
 
     def create_facet(
         self,
         *,
         SchemaArn: str,
         Name: str,
-        Attributes: Sequence[Union[FacetAttributeTypeDef, FacetAttributeOutputTypeDef]] = ...,
+        Attributes: Sequence[FacetAttributeUnionTypeDef] = ...,
         ObjectType: ObjectTypeType = ...,
         FacetStyle: FacetStyleType = ...
     ) -> Dict[str, Any]:
         """
         Creates a new  Facet in a schema.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.create_facet)
@@ -360,17 +352,15 @@
         """
 
     def create_object(
         self,
         *,
         DirectoryArn: str,
         SchemaFacets: Sequence[SchemaFacetTypeDef],
-        ObjectAttributeList: Sequence[
-            Union[AttributeKeyAndValueTypeDef, AttributeKeyAndValueOutputTypeDef]
-        ] = ...,
+        ObjectAttributeList: Sequence[AttributeKeyAndValueUnionTypeDef] = ...,
         ParentReference: ObjectReferenceTypeDef = ...,
         LinkName: str = ...
     ) -> CreateObjectResponseTypeDef:
         """
         Creates an object in a  Directory.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.create_object)
@@ -472,18 +462,15 @@
         Detaches a policy from an object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.detach_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/client/#detach_policy)
         """
 
     def detach_typed_link(
-        self,
-        *,
-        DirectoryArn: str,
-        TypedLinkSpecifier: Union[TypedLinkSpecifierTypeDef, TypedLinkSpecifierOutputTypeDef]
+        self, *, DirectoryArn: str, TypedLinkSpecifier: TypedLinkSpecifierUnionTypeDef
     ) -> EmptyResponseMetadataTypeDef:
         """
         Detaches a typed link from a specified source and target object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.detach_typed_link)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/client/#detach_typed_link)
         """
@@ -545,15 +532,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/client/#get_facet)
         """
 
     def get_link_attributes(
         self,
         *,
         DirectoryArn: str,
-        TypedLinkSpecifier: Union[TypedLinkSpecifierTypeDef, TypedLinkSpecifierOutputTypeDef],
+        TypedLinkSpecifier: TypedLinkSpecifierUnionTypeDef,
         AttributeNames: Sequence[str],
         ConsistencyLevel: ConsistencyLevelType = ...
     ) -> GetLinkAttributesResponseTypeDef:
         """
         Retrieves attributes that are associated with a typed link.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.get_link_attributes)
@@ -966,15 +953,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/client/#update_facet)
         """
 
     def update_link_attributes(
         self,
         *,
         DirectoryArn: str,
-        TypedLinkSpecifier: Union[TypedLinkSpecifierTypeDef, TypedLinkSpecifierOutputTypeDef],
+        TypedLinkSpecifier: TypedLinkSpecifierUnionTypeDef,
         AttributeUpdates: Sequence[LinkAttributeUpdateTypeDef]
     ) -> Dict[str, Any]:
         """
         Updates a given typed link’s attributes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.update_link_attributes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/client/#update_link_attributes)
```

### Comparing `mypy-boto3-clouddirectory-1.28.15.post1/mypy_boto3_clouddirectory/client.pyi` & `mypy-boto3-clouddirectory-1.28.16/mypy_boto3_clouddirectory/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_clouddirectory.client import CloudDirectoryClient
 
     session = Session()
     client: CloudDirectoryClient = session.client("clouddirectory")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import ConsistencyLevelType, DirectoryStateType, FacetStyleType, ObjectTypeType
 from .paginator import (
     ListAppliedSchemaArnsPaginator,
     ListAttachedIndicesPaginator,
@@ -41,19 +41,17 @@
     LookupPolicyPaginator,
 )
 from .type_defs import (
     ApplySchemaResponseTypeDef,
     AttachObjectResponseTypeDef,
     AttachToIndexResponseTypeDef,
     AttachTypedLinkResponseTypeDef,
-    AttributeKeyAndValueOutputTypeDef,
-    AttributeKeyAndValueTypeDef,
+    AttributeKeyAndValueUnionTypeDef,
     AttributeKeyTypeDef,
-    AttributeNameAndValueOutputTypeDef,
-    AttributeNameAndValueTypeDef,
+    AttributeNameAndValueUnionTypeDef,
     BatchReadOperationTypeDef,
     BatchReadResponseTypeDef,
     BatchWriteOperationTypeDef,
     BatchWriteResponseTypeDef,
     CreateDirectoryResponseTypeDef,
     CreateIndexResponseTypeDef,
     CreateObjectResponseTypeDef,
@@ -61,16 +59,15 @@
     DeleteDirectoryResponseTypeDef,
     DeleteSchemaResponseTypeDef,
     DetachFromIndexResponseTypeDef,
     DetachObjectResponseTypeDef,
     DisableDirectoryResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     EnableDirectoryResponseTypeDef,
-    FacetAttributeOutputTypeDef,
-    FacetAttributeTypeDef,
+    FacetAttributeUnionTypeDef,
     FacetAttributeUpdateTypeDef,
     GetAppliedSchemaVersionResponseTypeDef,
     GetDirectoryResponseTypeDef,
     GetFacetResponseTypeDef,
     GetLinkAttributesResponseTypeDef,
     GetObjectAttributesResponseTypeDef,
     GetObjectInformationResponseTypeDef,
@@ -105,16 +102,15 @@
     PutSchemaFromJsonResponseTypeDef,
     SchemaFacetTypeDef,
     TagTypeDef,
     TypedLinkAttributeRangeTypeDef,
     TypedLinkFacetAttributeUpdateTypeDef,
     TypedLinkFacetTypeDef,
     TypedLinkSchemaAndFacetNameTypeDef,
-    TypedLinkSpecifierOutputTypeDef,
-    TypedLinkSpecifierTypeDef,
+    TypedLinkSpecifierUnionTypeDef,
     UpdateObjectAttributesResponseTypeDef,
     UpdateSchemaResponseTypeDef,
     UpgradeAppliedSchemaResponseTypeDef,
     UpgradePublishedSchemaResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
@@ -187,17 +183,15 @@
         """
     def add_facet_to_object(
         self,
         *,
         DirectoryArn: str,
         SchemaFacet: SchemaFacetTypeDef,
         ObjectReference: ObjectReferenceTypeDef,
-        ObjectAttributeList: Sequence[
-            Union[AttributeKeyAndValueTypeDef, AttributeKeyAndValueOutputTypeDef]
-        ] = ...
+        ObjectAttributeList: Sequence[AttributeKeyAndValueUnionTypeDef] = ...
     ) -> Dict[str, Any]:
         """
         Adds a new  Facet to an object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.add_facet_to_object)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/client/#add_facet_to_object)
         """
@@ -254,17 +248,15 @@
     def attach_typed_link(
         self,
         *,
         DirectoryArn: str,
         SourceObjectReference: ObjectReferenceTypeDef,
         TargetObjectReference: ObjectReferenceTypeDef,
         TypedLinkFacet: TypedLinkSchemaAndFacetNameTypeDef,
-        Attributes: Sequence[
-            Union[AttributeNameAndValueTypeDef, AttributeNameAndValueOutputTypeDef]
-        ]
+        Attributes: Sequence[AttributeNameAndValueUnionTypeDef]
     ) -> AttachTypedLinkResponseTypeDef:
         """
         Attaches a typed link to a specified source and target object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.attach_typed_link)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/client/#attach_typed_link)
         """
@@ -312,15 +304,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/client/#create_directory)
         """
     def create_facet(
         self,
         *,
         SchemaArn: str,
         Name: str,
-        Attributes: Sequence[Union[FacetAttributeTypeDef, FacetAttributeOutputTypeDef]] = ...,
+        Attributes: Sequence[FacetAttributeUnionTypeDef] = ...,
         ObjectType: ObjectTypeType = ...,
         FacetStyle: FacetStyleType = ...
     ) -> Dict[str, Any]:
         """
         Creates a new  Facet in a schema.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.create_facet)
@@ -342,17 +334,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/client/#create_index)
         """
     def create_object(
         self,
         *,
         DirectoryArn: str,
         SchemaFacets: Sequence[SchemaFacetTypeDef],
-        ObjectAttributeList: Sequence[
-            Union[AttributeKeyAndValueTypeDef, AttributeKeyAndValueOutputTypeDef]
-        ] = ...,
+        ObjectAttributeList: Sequence[AttributeKeyAndValueUnionTypeDef] = ...,
         ParentReference: ObjectReferenceTypeDef = ...,
         LinkName: str = ...
     ) -> CreateObjectResponseTypeDef:
         """
         Creates an object in a  Directory.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.create_object)
@@ -443,18 +433,15 @@
         """
         Detaches a policy from an object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.detach_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/client/#detach_policy)
         """
     def detach_typed_link(
-        self,
-        *,
-        DirectoryArn: str,
-        TypedLinkSpecifier: Union[TypedLinkSpecifierTypeDef, TypedLinkSpecifierOutputTypeDef]
+        self, *, DirectoryArn: str, TypedLinkSpecifier: TypedLinkSpecifierUnionTypeDef
     ) -> EmptyResponseMetadataTypeDef:
         """
         Detaches a typed link from a specified source and target object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.detach_typed_link)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/client/#detach_typed_link)
         """
@@ -509,15 +496,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.get_facet)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/client/#get_facet)
         """
     def get_link_attributes(
         self,
         *,
         DirectoryArn: str,
-        TypedLinkSpecifier: Union[TypedLinkSpecifierTypeDef, TypedLinkSpecifierOutputTypeDef],
+        TypedLinkSpecifier: TypedLinkSpecifierUnionTypeDef,
         AttributeNames: Sequence[str],
         ConsistencyLevel: ConsistencyLevelType = ...
     ) -> GetLinkAttributesResponseTypeDef:
         """
         Retrieves attributes that are associated with a typed link.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.get_link_attributes)
@@ -898,15 +885,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.update_facet)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/client/#update_facet)
         """
     def update_link_attributes(
         self,
         *,
         DirectoryArn: str,
-        TypedLinkSpecifier: Union[TypedLinkSpecifierTypeDef, TypedLinkSpecifierOutputTypeDef],
+        TypedLinkSpecifier: TypedLinkSpecifierUnionTypeDef,
         AttributeUpdates: Sequence[LinkAttributeUpdateTypeDef]
     ) -> Dict[str, Any]:
         """
         Updates a given typed link’s attributes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory.Client.update_link_attributes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/client/#update_link_attributes)
```

### Comparing `mypy-boto3-clouddirectory-1.28.15.post1/mypy_boto3_clouddirectory/literals.py` & `mypy-boto3-clouddirectory-1.28.16/mypy_boto3_clouddirectory/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-clouddirectory-1.28.15.post1/mypy_boto3_clouddirectory/literals.pyi` & `mypy-boto3-clouddirectory-1.28.16/mypy_boto3_clouddirectory/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-clouddirectory-1.28.15.post1/mypy_boto3_clouddirectory/paginator.py` & `mypy-boto3-clouddirectory-1.28.16/mypy_boto3_clouddirectory/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-clouddirectory-1.28.15.post1/mypy_boto3_clouddirectory/paginator.pyi` & `mypy-boto3-clouddirectory-1.28.16/mypy_boto3_clouddirectory/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-clouddirectory-1.28.15.post1/mypy_boto3_clouddirectory/type_defs.py` & `mypy-boto3-clouddirectory-1.28.16/mypy_boto3_clouddirectory/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_clouddirectory.type_defs import ObjectReferenceTypeDef
 
-    data: ObjectReferenceTypeDef = {...}
+    data: ObjectReferenceTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -40,28 +40,28 @@
     "ObjectReferenceTypeDef",
     "SchemaFacetTypeDef",
     "ApplySchemaRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "TypedLinkSchemaAndFacetNameTypeDef",
     "AttributeKeyTypeDef",
     "TypedAttributeValueOutputTypeDef",
-    "TypedAttributeValueTypeDef",
     "BatchAttachObjectResponseTypeDef",
     "BatchAttachToIndexResponseTypeDef",
     "BatchCreateIndexResponseTypeDef",
     "BatchCreateObjectResponseTypeDef",
     "BatchDetachFromIndexResponseTypeDef",
     "BatchDetachObjectResponseTypeDef",
     "BatchListObjectChildrenResponseTypeDef",
     "PathToObjectIdentifiersTypeDef",
     "ObjectIdentifierAndLinkNameTupleTypeDef",
     "BatchListObjectPoliciesResponseTypeDef",
     "BatchListPolicyAttachmentsResponseTypeDef",
     "BatchReadExceptionTypeDef",
     "BatchUpdateObjectAttributesResponseTypeDef",
+    "BlobTypeDef",
     "CreateDirectoryRequestRequestTypeDef",
     "CreateSchemaRequestRequestTypeDef",
     "DeleteDirectoryRequestRequestTypeDef",
     "DeleteFacetRequestRequestTypeDef",
     "DeleteSchemaRequestRequestTypeDef",
     "DeleteTypedLinkFacetRequestRequestTypeDef",
     "DirectoryTypeDef",
@@ -87,14 +87,15 @@
     "ListTagsForResourceRequestRequestTypeDef",
     "TagTypeDef",
     "ListTypedLinkFacetAttributesRequestRequestTypeDef",
     "ListTypedLinkFacetNamesRequestRequestTypeDef",
     "PolicyAttachmentTypeDef",
     "PublishSchemaRequestRequestTypeDef",
     "PutSchemaFromJsonRequestRequestTypeDef",
+    "TimestampTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateSchemaRequestRequestTypeDef",
     "UpgradeAppliedSchemaRequestRequestTypeDef",
     "UpgradePublishedSchemaRequestRequestTypeDef",
     "AttachObjectRequestRequestTypeDef",
     "AttachPolicyRequestRequestTypeDef",
     "AttachToIndexRequestRequestTypeDef",
@@ -165,29 +166,22 @@
     "UpdateSchemaResponseTypeDef",
     "UpgradeAppliedSchemaResponseTypeDef",
     "UpgradePublishedSchemaResponseTypeDef",
     "BatchCreateIndexTypeDef",
     "CreateIndexRequestRequestTypeDef",
     "AttributeKeyAndValueOutputTypeDef",
     "AttributeNameAndValueOutputTypeDef",
-    "AttributeKeyAndValueTypeDef",
-    "AttributeNameAndValueTypeDef",
-    "LinkAttributeActionTypeDef",
-    "ObjectAttributeActionTypeDef",
-    "TypedAttributeValueRangeTypeDef",
     "BatchListObjectParentPathsResponseTypeDef",
     "ListObjectParentPathsResponseTypeDef",
     "BatchListObjectParentsResponseTypeDef",
     "ListObjectParentsResponseTypeDef",
     "GetDirectoryResponseTypeDef",
     "ListDirectoriesResponseTypeDef",
     "FacetAttributeDefinitionOutputTypeDef",
     "TypedLinkAttributeDefinitionOutputTypeDef",
-    "FacetAttributeDefinitionTypeDef",
-    "TypedLinkAttributeDefinitionTypeDef",
     "GetFacetResponseTypeDef",
     "ListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef",
     "ListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef",
     "ListDevelopmentSchemaArnsRequestListDevelopmentSchemaArnsPaginateTypeDef",
     "ListDirectoriesRequestListDirectoriesPaginateTypeDef",
     "ListFacetAttributesRequestListFacetAttributesPaginateTypeDef",
     "ListFacetNamesRequestListFacetNamesPaginateTypeDef",
@@ -200,82 +194,94 @@
     "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef",
     "ListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef",
     "LookupPolicyRequestLookupPolicyPaginateTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "PolicyToPathTypeDef",
+    "TypedAttributeValueTypeDef",
     "BatchGetLinkAttributesResponseTypeDef",
     "BatchGetObjectAttributesResponseTypeDef",
     "BatchListObjectAttributesResponseTypeDef",
     "GetLinkAttributesResponseTypeDef",
     "GetObjectAttributesResponseTypeDef",
     "IndexAttachmentTypeDef",
     "ListObjectAttributesResponseTypeDef",
     "TypedLinkSpecifierOutputTypeDef",
-    "AddFacetToObjectRequestRequestTypeDef",
-    "BatchAddFacetToObjectTypeDef",
-    "BatchCreateObjectTypeDef",
-    "CreateObjectRequestRequestTypeDef",
-    "AttachTypedLinkRequestRequestTypeDef",
-    "BatchAttachTypedLinkTypeDef",
-    "TypedLinkSpecifierTypeDef",
-    "LinkAttributeUpdateTypeDef",
-    "ObjectAttributeUpdateTypeDef",
-    "ObjectAttributeRangeTypeDef",
-    "TypedLinkAttributeRangeTypeDef",
     "FacetAttributeOutputTypeDef",
     "ListTypedLinkFacetAttributesResponseTypeDef",
-    "FacetAttributeTypeDef",
-    "TypedLinkFacetAttributeUpdateTypeDef",
-    "TypedLinkFacetTypeDef",
     "BatchLookupPolicyResponseTypeDef",
     "LookupPolicyResponseTypeDef",
+    "AttributeKeyAndValueTypeDef",
+    "AttributeNameAndValueTypeDef",
+    "FacetAttributeDefinitionTypeDef",
+    "LinkAttributeActionTypeDef",
+    "ObjectAttributeActionTypeDef",
+    "TypedAttributeValueRangeTypeDef",
+    "TypedLinkAttributeDefinitionTypeDef",
     "BatchListAttachedIndicesResponseTypeDef",
     "BatchListIndexResponseTypeDef",
     "ListAttachedIndicesResponseTypeDef",
     "ListIndexResponseTypeDef",
     "AttachTypedLinkResponseTypeDef",
     "BatchAttachTypedLinkResponseTypeDef",
     "BatchListIncomingTypedLinksResponseTypeDef",
     "BatchListOutgoingTypedLinksResponseTypeDef",
     "ListIncomingTypedLinksResponseTypeDef",
     "ListOutgoingTypedLinksResponseTypeDef",
+    "ListFacetAttributesResponseTypeDef",
+    "AttributeKeyAndValueUnionTypeDef",
+    "BatchAddFacetToObjectTypeDef",
+    "BatchCreateObjectTypeDef",
+    "AttributeNameAndValueUnionTypeDef",
+    "BatchAttachTypedLinkTypeDef",
+    "TypedLinkSpecifierTypeDef",
+    "FacetAttributeTypeDef",
+    "LinkAttributeUpdateTypeDef",
+    "ObjectAttributeUpdateTypeDef",
+    "ObjectAttributeRangeTypeDef",
+    "TypedLinkAttributeRangeTypeDef",
+    "TypedLinkFacetAttributeUpdateTypeDef",
+    "TypedLinkFacetTypeDef",
+    "BatchWriteOperationResponseTypeDef",
+    "BatchReadSuccessfulResponseTypeDef",
+    "AddFacetToObjectRequestRequestTypeDef",
+    "CreateObjectRequestRequestTypeDef",
+    "AttachTypedLinkRequestRequestTypeDef",
     "BatchDetachTypedLinkTypeDef",
     "BatchGetLinkAttributesTypeDef",
     "DetachTypedLinkRequestRequestTypeDef",
     "GetLinkAttributesRequestRequestTypeDef",
+    "TypedLinkSpecifierUnionTypeDef",
+    "FacetAttributeUnionTypeDef",
+    "FacetAttributeUpdateTypeDef",
     "BatchUpdateLinkAttributesTypeDef",
     "UpdateLinkAttributesRequestRequestTypeDef",
     "BatchUpdateObjectAttributesTypeDef",
     "UpdateObjectAttributesRequestRequestTypeDef",
     "BatchListIndexTypeDef",
     "ListIndexRequestListIndexPaginateTypeDef",
     "ListIndexRequestRequestTypeDef",
     "BatchListIncomingTypedLinksTypeDef",
     "BatchListOutgoingTypedLinksTypeDef",
     "ListIncomingTypedLinksRequestListIncomingTypedLinksPaginateTypeDef",
     "ListIncomingTypedLinksRequestRequestTypeDef",
     "ListOutgoingTypedLinksRequestListOutgoingTypedLinksPaginateTypeDef",
     "ListOutgoingTypedLinksRequestRequestTypeDef",
-    "ListFacetAttributesResponseTypeDef",
-    "CreateFacetRequestRequestTypeDef",
-    "FacetAttributeUpdateTypeDef",
     "UpdateTypedLinkFacetRequestRequestTypeDef",
     "CreateTypedLinkFacetRequestRequestTypeDef",
-    "BatchWriteOperationResponseTypeDef",
-    "BatchReadSuccessfulResponseTypeDef",
-    "BatchWriteOperationTypeDef",
-    "BatchReadOperationTypeDef",
-    "UpdateFacetRequestRequestTypeDef",
     "BatchWriteResponseTypeDef",
     "BatchReadOperationResponseTypeDef",
+    "CreateFacetRequestRequestTypeDef",
+    "UpdateFacetRequestRequestTypeDef",
+    "BatchWriteOperationTypeDef",
+    "BatchReadOperationTypeDef",
+    "BatchReadResponseTypeDef",
     "BatchWriteRequestRequestTypeDef",
     "BatchReadRequestRequestTypeDef",
-    "BatchReadResponseTypeDef",
 )
 
 ObjectReferenceTypeDef = TypedDict(
     "ObjectReferenceTypeDef",
     {
         "Selector": str,
     },
@@ -335,26 +341,14 @@
         "BooleanValue": bool,
         "NumberValue": str,
         "DatetimeValue": datetime,
     },
     total=False,
 )
 
-TypedAttributeValueTypeDef = TypedDict(
-    "TypedAttributeValueTypeDef",
-    {
-        "StringValue": str,
-        "BinaryValue": Union[str, bytes, IO[Any], StreamingBody],
-        "BooleanValue": bool,
-        "NumberValue": str,
-        "DatetimeValue": Union[datetime, str],
-    },
-    total=False,
-)
-
 BatchAttachObjectResponseTypeDef = TypedDict(
     "BatchAttachObjectResponseTypeDef",
     {
         "attachedObjectIdentifier": str,
     },
     total=False,
 )
@@ -457,14 +451,15 @@
     "BatchUpdateObjectAttributesResponseTypeDef",
     {
         "ObjectIdentifier": str,
     },
     total=False,
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 CreateDirectoryRequestRequestTypeDef = TypedDict(
     "CreateDirectoryRequestRequestTypeDef",
     {
         "Name": str,
         "SchemaArn": str,
     },
 )
@@ -839,14 +834,15 @@
     "PutSchemaFromJsonRequestRequestTypeDef",
     {
         "SchemaArn": str,
         "Document": str,
     },
 )
 
+TimestampTypeDef = Union[datetime, str]
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -1841,71 +1837,14 @@
     "AttributeNameAndValueOutputTypeDef",
     {
         "AttributeName": str,
         "Value": TypedAttributeValueOutputTypeDef,
     },
 )
 
-AttributeKeyAndValueTypeDef = TypedDict(
-    "AttributeKeyAndValueTypeDef",
-    {
-        "Key": AttributeKeyTypeDef,
-        "Value": TypedAttributeValueTypeDef,
-    },
-)
-
-AttributeNameAndValueTypeDef = TypedDict(
-    "AttributeNameAndValueTypeDef",
-    {
-        "AttributeName": str,
-        "Value": TypedAttributeValueTypeDef,
-    },
-)
-
-LinkAttributeActionTypeDef = TypedDict(
-    "LinkAttributeActionTypeDef",
-    {
-        "AttributeActionType": UpdateActionTypeType,
-        "AttributeUpdateValue": TypedAttributeValueTypeDef,
-    },
-    total=False,
-)
-
-ObjectAttributeActionTypeDef = TypedDict(
-    "ObjectAttributeActionTypeDef",
-    {
-        "ObjectAttributeActionType": UpdateActionTypeType,
-        "ObjectAttributeUpdateValue": TypedAttributeValueTypeDef,
-    },
-    total=False,
-)
-
-_RequiredTypedAttributeValueRangeTypeDef = TypedDict(
-    "_RequiredTypedAttributeValueRangeTypeDef",
-    {
-        "StartMode": RangeModeType,
-        "EndMode": RangeModeType,
-    },
-)
-_OptionalTypedAttributeValueRangeTypeDef = TypedDict(
-    "_OptionalTypedAttributeValueRangeTypeDef",
-    {
-        "StartValue": TypedAttributeValueTypeDef,
-        "EndValue": TypedAttributeValueTypeDef,
-    },
-    total=False,
-)
-
-
-class TypedAttributeValueRangeTypeDef(
-    _RequiredTypedAttributeValueRangeTypeDef, _OptionalTypedAttributeValueRangeTypeDef
-):
-    pass
-
-
 BatchListObjectParentPathsResponseTypeDef = TypedDict(
     "BatchListObjectParentPathsResponseTypeDef",
     {
         "PathToObjectIdentifiersList": List[PathToObjectIdentifiersTypeDef],
         "NextToken": str,
     },
     total=False,
@@ -2001,62 +1940,14 @@
 class TypedLinkAttributeDefinitionOutputTypeDef(
     _RequiredTypedLinkAttributeDefinitionOutputTypeDef,
     _OptionalTypedLinkAttributeDefinitionOutputTypeDef,
 ):
     pass
 
 
-_RequiredFacetAttributeDefinitionTypeDef = TypedDict(
-    "_RequiredFacetAttributeDefinitionTypeDef",
-    {
-        "Type": FacetAttributeTypeType,
-    },
-)
-_OptionalFacetAttributeDefinitionTypeDef = TypedDict(
-    "_OptionalFacetAttributeDefinitionTypeDef",
-    {
-        "DefaultValue": TypedAttributeValueTypeDef,
-        "IsImmutable": bool,
-        "Rules": Mapping[str, RuleTypeDef],
-    },
-    total=False,
-)
-
-
-class FacetAttributeDefinitionTypeDef(
-    _RequiredFacetAttributeDefinitionTypeDef, _OptionalFacetAttributeDefinitionTypeDef
-):
-    pass
-
-
-_RequiredTypedLinkAttributeDefinitionTypeDef = TypedDict(
-    "_RequiredTypedLinkAttributeDefinitionTypeDef",
-    {
-        "Name": str,
-        "Type": FacetAttributeTypeType,
-        "RequiredBehavior": RequiredAttributeBehaviorType,
-    },
-)
-_OptionalTypedLinkAttributeDefinitionTypeDef = TypedDict(
-    "_OptionalTypedLinkAttributeDefinitionTypeDef",
-    {
-        "DefaultValue": TypedAttributeValueTypeDef,
-        "IsImmutable": bool,
-        "Rules": Mapping[str, RuleTypeDef],
-    },
-    total=False,
-)
-
-
-class TypedLinkAttributeDefinitionTypeDef(
-    _RequiredTypedLinkAttributeDefinitionTypeDef, _OptionalTypedLinkAttributeDefinitionTypeDef
-):
-    pass
-
-
 GetFacetResponseTypeDef = TypedDict(
     "GetFacetResponseTypeDef",
     {
         "Facet": FacetTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2396,14 +2287,26 @@
     {
         "Path": str,
         "Policies": List[PolicyAttachmentTypeDef],
     },
     total=False,
 )
 
+TypedAttributeValueTypeDef = TypedDict(
+    "TypedAttributeValueTypeDef",
+    {
+        "StringValue": str,
+        "BinaryValue": BlobTypeDef,
+        "BooleanValue": bool,
+        "NumberValue": str,
+        "DatetimeValue": TimestampTypeDef,
+    },
+    total=False,
+)
+
 BatchGetLinkAttributesResponseTypeDef = TypedDict(
     "BatchGetLinkAttributesResponseTypeDef",
     {
         "Attributes": List[AttributeKeyAndValueOutputTypeDef],
     },
     total=False,
 )
@@ -2465,208 +2368,322 @@
         "TypedLinkFacet": TypedLinkSchemaAndFacetNameTypeDef,
         "SourceObjectReference": ObjectReferenceTypeDef,
         "TargetObjectReference": ObjectReferenceTypeDef,
         "IdentityAttributeValues": List[AttributeNameAndValueOutputTypeDef],
     },
 )
 
-_RequiredAddFacetToObjectRequestRequestTypeDef = TypedDict(
-    "_RequiredAddFacetToObjectRequestRequestTypeDef",
+_RequiredFacetAttributeOutputTypeDef = TypedDict(
+    "_RequiredFacetAttributeOutputTypeDef",
     {
-        "DirectoryArn": str,
-        "SchemaFacet": SchemaFacetTypeDef,
-        "ObjectReference": ObjectReferenceTypeDef,
+        "Name": str,
     },
 )
-_OptionalAddFacetToObjectRequestRequestTypeDef = TypedDict(
-    "_OptionalAddFacetToObjectRequestRequestTypeDef",
+_OptionalFacetAttributeOutputTypeDef = TypedDict(
+    "_OptionalFacetAttributeOutputTypeDef",
     {
-        "ObjectAttributeList": Sequence[
-            Union[AttributeKeyAndValueTypeDef, AttributeKeyAndValueOutputTypeDef]
-        ],
+        "AttributeDefinition": FacetAttributeDefinitionOutputTypeDef,
+        "AttributeReference": FacetAttributeReferenceTypeDef,
+        "RequiredBehavior": RequiredAttributeBehaviorType,
     },
     total=False,
 )
 
 
-class AddFacetToObjectRequestRequestTypeDef(
-    _RequiredAddFacetToObjectRequestRequestTypeDef, _OptionalAddFacetToObjectRequestRequestTypeDef
+class FacetAttributeOutputTypeDef(
+    _RequiredFacetAttributeOutputTypeDef, _OptionalFacetAttributeOutputTypeDef
 ):
     pass
 
 
-BatchAddFacetToObjectTypeDef = TypedDict(
-    "BatchAddFacetToObjectTypeDef",
+ListTypedLinkFacetAttributesResponseTypeDef = TypedDict(
+    "ListTypedLinkFacetAttributesResponseTypeDef",
     {
-        "SchemaFacet": SchemaFacetTypeDef,
-        "ObjectAttributeList": Sequence[AttributeKeyAndValueTypeDef],
-        "ObjectReference": ObjectReferenceTypeDef,
+        "Attributes": List[TypedLinkAttributeDefinitionOutputTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredBatchCreateObjectTypeDef = TypedDict(
-    "_RequiredBatchCreateObjectTypeDef",
+BatchLookupPolicyResponseTypeDef = TypedDict(
+    "BatchLookupPolicyResponseTypeDef",
     {
-        "SchemaFacet": Sequence[SchemaFacetTypeDef],
-        "ObjectAttributeList": Sequence[AttributeKeyAndValueTypeDef],
+        "PolicyToPathList": List[PolicyToPathTypeDef],
+        "NextToken": str,
     },
+    total=False,
 )
-_OptionalBatchCreateObjectTypeDef = TypedDict(
-    "_OptionalBatchCreateObjectTypeDef",
+
+LookupPolicyResponseTypeDef = TypedDict(
+    "LookupPolicyResponseTypeDef",
     {
-        "ParentReference": ObjectReferenceTypeDef,
-        "LinkName": str,
-        "BatchReferenceName": str,
+        "PolicyToPathList": List[PolicyToPathTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AttributeKeyAndValueTypeDef = TypedDict(
+    "AttributeKeyAndValueTypeDef",
+    {
+        "Key": AttributeKeyTypeDef,
+        "Value": TypedAttributeValueTypeDef,
+    },
+)
+
+AttributeNameAndValueTypeDef = TypedDict(
+    "AttributeNameAndValueTypeDef",
+    {
+        "AttributeName": str,
+        "Value": TypedAttributeValueTypeDef,
+    },
+)
+
+_RequiredFacetAttributeDefinitionTypeDef = TypedDict(
+    "_RequiredFacetAttributeDefinitionTypeDef",
+    {
+        "Type": FacetAttributeTypeType,
+    },
+)
+_OptionalFacetAttributeDefinitionTypeDef = TypedDict(
+    "_OptionalFacetAttributeDefinitionTypeDef",
+    {
+        "DefaultValue": TypedAttributeValueTypeDef,
+        "IsImmutable": bool,
+        "Rules": Mapping[str, RuleTypeDef],
     },
     total=False,
 )
 
 
-class BatchCreateObjectTypeDef(
-    _RequiredBatchCreateObjectTypeDef, _OptionalBatchCreateObjectTypeDef
+class FacetAttributeDefinitionTypeDef(
+    _RequiredFacetAttributeDefinitionTypeDef, _OptionalFacetAttributeDefinitionTypeDef
 ):
     pass
 
 
-_RequiredCreateObjectRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateObjectRequestRequestTypeDef",
+LinkAttributeActionTypeDef = TypedDict(
+    "LinkAttributeActionTypeDef",
     {
-        "DirectoryArn": str,
-        "SchemaFacets": Sequence[SchemaFacetTypeDef],
+        "AttributeActionType": UpdateActionTypeType,
+        "AttributeUpdateValue": TypedAttributeValueTypeDef,
     },
+    total=False,
 )
-_OptionalCreateObjectRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateObjectRequestRequestTypeDef",
+
+ObjectAttributeActionTypeDef = TypedDict(
+    "ObjectAttributeActionTypeDef",
     {
-        "ObjectAttributeList": Sequence[
-            Union[AttributeKeyAndValueTypeDef, AttributeKeyAndValueOutputTypeDef]
-        ],
-        "ParentReference": ObjectReferenceTypeDef,
-        "LinkName": str,
+        "ObjectAttributeActionType": UpdateActionTypeType,
+        "ObjectAttributeUpdateValue": TypedAttributeValueTypeDef,
     },
     total=False,
 )
 
+_RequiredTypedAttributeValueRangeTypeDef = TypedDict(
+    "_RequiredTypedAttributeValueRangeTypeDef",
+    {
+        "StartMode": RangeModeType,
+        "EndMode": RangeModeType,
+    },
+)
+_OptionalTypedAttributeValueRangeTypeDef = TypedDict(
+    "_OptionalTypedAttributeValueRangeTypeDef",
+    {
+        "StartValue": TypedAttributeValueTypeDef,
+        "EndValue": TypedAttributeValueTypeDef,
+    },
+    total=False,
+)
 
-class CreateObjectRequestRequestTypeDef(
-    _RequiredCreateObjectRequestRequestTypeDef, _OptionalCreateObjectRequestRequestTypeDef
+
+class TypedAttributeValueRangeTypeDef(
+    _RequiredTypedAttributeValueRangeTypeDef, _OptionalTypedAttributeValueRangeTypeDef
 ):
     pass
 
 
-AttachTypedLinkRequestRequestTypeDef = TypedDict(
-    "AttachTypedLinkRequestRequestTypeDef",
+_RequiredTypedLinkAttributeDefinitionTypeDef = TypedDict(
+    "_RequiredTypedLinkAttributeDefinitionTypeDef",
     {
-        "DirectoryArn": str,
-        "SourceObjectReference": ObjectReferenceTypeDef,
-        "TargetObjectReference": ObjectReferenceTypeDef,
-        "TypedLinkFacet": TypedLinkSchemaAndFacetNameTypeDef,
-        "Attributes": Sequence[
-            Union[AttributeNameAndValueTypeDef, AttributeNameAndValueOutputTypeDef]
-        ],
+        "Name": str,
+        "Type": FacetAttributeTypeType,
+        "RequiredBehavior": RequiredAttributeBehaviorType,
     },
 )
-
-BatchAttachTypedLinkTypeDef = TypedDict(
-    "BatchAttachTypedLinkTypeDef",
+_OptionalTypedLinkAttributeDefinitionTypeDef = TypedDict(
+    "_OptionalTypedLinkAttributeDefinitionTypeDef",
     {
-        "SourceObjectReference": ObjectReferenceTypeDef,
-        "TargetObjectReference": ObjectReferenceTypeDef,
-        "TypedLinkFacet": TypedLinkSchemaAndFacetNameTypeDef,
-        "Attributes": Sequence[AttributeNameAndValueTypeDef],
+        "DefaultValue": TypedAttributeValueTypeDef,
+        "IsImmutable": bool,
+        "Rules": Mapping[str, RuleTypeDef],
     },
+    total=False,
 )
 
-TypedLinkSpecifierTypeDef = TypedDict(
-    "TypedLinkSpecifierTypeDef",
+
+class TypedLinkAttributeDefinitionTypeDef(
+    _RequiredTypedLinkAttributeDefinitionTypeDef, _OptionalTypedLinkAttributeDefinitionTypeDef
+):
+    pass
+
+
+BatchListAttachedIndicesResponseTypeDef = TypedDict(
+    "BatchListAttachedIndicesResponseTypeDef",
     {
-        "TypedLinkFacet": TypedLinkSchemaAndFacetNameTypeDef,
-        "SourceObjectReference": ObjectReferenceTypeDef,
-        "TargetObjectReference": ObjectReferenceTypeDef,
-        "IdentityAttributeValues": Sequence[AttributeNameAndValueTypeDef],
+        "IndexAttachments": List[IndexAttachmentTypeDef],
+        "NextToken": str,
     },
+    total=False,
 )
 
-LinkAttributeUpdateTypeDef = TypedDict(
-    "LinkAttributeUpdateTypeDef",
+BatchListIndexResponseTypeDef = TypedDict(
+    "BatchListIndexResponseTypeDef",
     {
-        "AttributeKey": AttributeKeyTypeDef,
-        "AttributeAction": LinkAttributeActionTypeDef,
+        "IndexAttachments": List[IndexAttachmentTypeDef],
+        "NextToken": str,
     },
     total=False,
 )
 
-ObjectAttributeUpdateTypeDef = TypedDict(
-    "ObjectAttributeUpdateTypeDef",
+ListAttachedIndicesResponseTypeDef = TypedDict(
+    "ListAttachedIndicesResponseTypeDef",
     {
-        "ObjectAttributeKey": AttributeKeyTypeDef,
-        "ObjectAttributeAction": ObjectAttributeActionTypeDef,
+        "IndexAttachments": List[IndexAttachmentTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-ObjectAttributeRangeTypeDef = TypedDict(
-    "ObjectAttributeRangeTypeDef",
+ListIndexResponseTypeDef = TypedDict(
+    "ListIndexResponseTypeDef",
     {
-        "AttributeKey": AttributeKeyTypeDef,
-        "Range": TypedAttributeValueRangeTypeDef,
+        "IndexAttachments": List[IndexAttachmentTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AttachTypedLinkResponseTypeDef = TypedDict(
+    "AttachTypedLinkResponseTypeDef",
+    {
+        "TypedLinkSpecifier": TypedLinkSpecifierOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+BatchAttachTypedLinkResponseTypeDef = TypedDict(
+    "BatchAttachTypedLinkResponseTypeDef",
+    {
+        "TypedLinkSpecifier": TypedLinkSpecifierOutputTypeDef,
     },
     total=False,
 )
 
-_RequiredTypedLinkAttributeRangeTypeDef = TypedDict(
-    "_RequiredTypedLinkAttributeRangeTypeDef",
+BatchListIncomingTypedLinksResponseTypeDef = TypedDict(
+    "BatchListIncomingTypedLinksResponseTypeDef",
     {
-        "Range": TypedAttributeValueRangeTypeDef,
+        "LinkSpecifiers": List[TypedLinkSpecifierOutputTypeDef],
+        "NextToken": str,
     },
+    total=False,
 )
-_OptionalTypedLinkAttributeRangeTypeDef = TypedDict(
-    "_OptionalTypedLinkAttributeRangeTypeDef",
+
+BatchListOutgoingTypedLinksResponseTypeDef = TypedDict(
+    "BatchListOutgoingTypedLinksResponseTypeDef",
     {
-        "AttributeName": str,
+        "TypedLinkSpecifiers": List[TypedLinkSpecifierOutputTypeDef],
+        "NextToken": str,
     },
     total=False,
 )
 
+ListIncomingTypedLinksResponseTypeDef = TypedDict(
+    "ListIncomingTypedLinksResponseTypeDef",
+    {
+        "LinkSpecifiers": List[TypedLinkSpecifierOutputTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class TypedLinkAttributeRangeTypeDef(
-    _RequiredTypedLinkAttributeRangeTypeDef, _OptionalTypedLinkAttributeRangeTypeDef
-):
-    pass
+ListOutgoingTypedLinksResponseTypeDef = TypedDict(
+    "ListOutgoingTypedLinksResponseTypeDef",
+    {
+        "TypedLinkSpecifiers": List[TypedLinkSpecifierOutputTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
+ListFacetAttributesResponseTypeDef = TypedDict(
+    "ListFacetAttributesResponseTypeDef",
+    {
+        "Attributes": List[FacetAttributeOutputTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-_RequiredFacetAttributeOutputTypeDef = TypedDict(
-    "_RequiredFacetAttributeOutputTypeDef",
+AttributeKeyAndValueUnionTypeDef = Union[
+    AttributeKeyAndValueTypeDef, AttributeKeyAndValueOutputTypeDef
+]
+BatchAddFacetToObjectTypeDef = TypedDict(
+    "BatchAddFacetToObjectTypeDef",
     {
-        "Name": str,
+        "SchemaFacet": SchemaFacetTypeDef,
+        "ObjectAttributeList": Sequence[AttributeKeyAndValueTypeDef],
+        "ObjectReference": ObjectReferenceTypeDef,
     },
 )
-_OptionalFacetAttributeOutputTypeDef = TypedDict(
-    "_OptionalFacetAttributeOutputTypeDef",
+
+_RequiredBatchCreateObjectTypeDef = TypedDict(
+    "_RequiredBatchCreateObjectTypeDef",
     {
-        "AttributeDefinition": FacetAttributeDefinitionOutputTypeDef,
-        "AttributeReference": FacetAttributeReferenceTypeDef,
-        "RequiredBehavior": RequiredAttributeBehaviorType,
+        "SchemaFacet": Sequence[SchemaFacetTypeDef],
+        "ObjectAttributeList": Sequence[AttributeKeyAndValueTypeDef],
+    },
+)
+_OptionalBatchCreateObjectTypeDef = TypedDict(
+    "_OptionalBatchCreateObjectTypeDef",
+    {
+        "ParentReference": ObjectReferenceTypeDef,
+        "LinkName": str,
+        "BatchReferenceName": str,
     },
     total=False,
 )
 
 
-class FacetAttributeOutputTypeDef(
-    _RequiredFacetAttributeOutputTypeDef, _OptionalFacetAttributeOutputTypeDef
+class BatchCreateObjectTypeDef(
+    _RequiredBatchCreateObjectTypeDef, _OptionalBatchCreateObjectTypeDef
 ):
     pass
 
 
-ListTypedLinkFacetAttributesResponseTypeDef = TypedDict(
-    "ListTypedLinkFacetAttributesResponseTypeDef",
+AttributeNameAndValueUnionTypeDef = Union[
+    AttributeNameAndValueTypeDef, AttributeNameAndValueOutputTypeDef
+]
+BatchAttachTypedLinkTypeDef = TypedDict(
+    "BatchAttachTypedLinkTypeDef",
     {
-        "Attributes": List[TypedLinkAttributeDefinitionOutputTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "SourceObjectReference": ObjectReferenceTypeDef,
+        "TargetObjectReference": ObjectReferenceTypeDef,
+        "TypedLinkFacet": TypedLinkSchemaAndFacetNameTypeDef,
+        "Attributes": Sequence[AttributeNameAndValueTypeDef],
+    },
+)
+
+TypedLinkSpecifierTypeDef = TypedDict(
+    "TypedLinkSpecifierTypeDef",
+    {
+        "TypedLinkFacet": TypedLinkSchemaAndFacetNameTypeDef,
+        "SourceObjectReference": ObjectReferenceTypeDef,
+        "TargetObjectReference": ObjectReferenceTypeDef,
+        "IdentityAttributeValues": Sequence[AttributeNameAndValueTypeDef],
     },
 )
 
 _RequiredFacetAttributeTypeDef = TypedDict(
     "_RequiredFacetAttributeTypeDef",
     {
         "Name": str,
@@ -2683,134 +2700,177 @@
 )
 
 
 class FacetAttributeTypeDef(_RequiredFacetAttributeTypeDef, _OptionalFacetAttributeTypeDef):
     pass
 
 
-TypedLinkFacetAttributeUpdateTypeDef = TypedDict(
-    "TypedLinkFacetAttributeUpdateTypeDef",
+LinkAttributeUpdateTypeDef = TypedDict(
+    "LinkAttributeUpdateTypeDef",
     {
-        "Attribute": TypedLinkAttributeDefinitionTypeDef,
-        "Action": UpdateActionTypeType,
+        "AttributeKey": AttributeKeyTypeDef,
+        "AttributeAction": LinkAttributeActionTypeDef,
     },
+    total=False,
 )
 
-TypedLinkFacetTypeDef = TypedDict(
-    "TypedLinkFacetTypeDef",
+ObjectAttributeUpdateTypeDef = TypedDict(
+    "ObjectAttributeUpdateTypeDef",
     {
-        "Name": str,
-        "Attributes": Sequence[TypedLinkAttributeDefinitionTypeDef],
-        "IdentityAttributeOrder": Sequence[str],
+        "ObjectAttributeKey": AttributeKeyTypeDef,
+        "ObjectAttributeAction": ObjectAttributeActionTypeDef,
     },
+    total=False,
 )
 
-BatchLookupPolicyResponseTypeDef = TypedDict(
-    "BatchLookupPolicyResponseTypeDef",
+ObjectAttributeRangeTypeDef = TypedDict(
+    "ObjectAttributeRangeTypeDef",
     {
-        "PolicyToPathList": List[PolicyToPathTypeDef],
-        "NextToken": str,
+        "AttributeKey": AttributeKeyTypeDef,
+        "Range": TypedAttributeValueRangeTypeDef,
     },
     total=False,
 )
 
-LookupPolicyResponseTypeDef = TypedDict(
-    "LookupPolicyResponseTypeDef",
+_RequiredTypedLinkAttributeRangeTypeDef = TypedDict(
+    "_RequiredTypedLinkAttributeRangeTypeDef",
     {
-        "PolicyToPathList": List[PolicyToPathTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Range": TypedAttributeValueRangeTypeDef,
     },
 )
-
-BatchListAttachedIndicesResponseTypeDef = TypedDict(
-    "BatchListAttachedIndicesResponseTypeDef",
+_OptionalTypedLinkAttributeRangeTypeDef = TypedDict(
+    "_OptionalTypedLinkAttributeRangeTypeDef",
     {
-        "IndexAttachments": List[IndexAttachmentTypeDef],
-        "NextToken": str,
+        "AttributeName": str,
     },
     total=False,
 )
 
-BatchListIndexResponseTypeDef = TypedDict(
-    "BatchListIndexResponseTypeDef",
+
+class TypedLinkAttributeRangeTypeDef(
+    _RequiredTypedLinkAttributeRangeTypeDef, _OptionalTypedLinkAttributeRangeTypeDef
+):
+    pass
+
+
+TypedLinkFacetAttributeUpdateTypeDef = TypedDict(
+    "TypedLinkFacetAttributeUpdateTypeDef",
     {
-        "IndexAttachments": List[IndexAttachmentTypeDef],
-        "NextToken": str,
+        "Attribute": TypedLinkAttributeDefinitionTypeDef,
+        "Action": UpdateActionTypeType,
     },
-    total=False,
 )
 
-ListAttachedIndicesResponseTypeDef = TypedDict(
-    "ListAttachedIndicesResponseTypeDef",
+TypedLinkFacetTypeDef = TypedDict(
+    "TypedLinkFacetTypeDef",
     {
-        "IndexAttachments": List[IndexAttachmentTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Name": str,
+        "Attributes": Sequence[TypedLinkAttributeDefinitionTypeDef],
+        "IdentityAttributeOrder": Sequence[str],
     },
 )
 
-ListIndexResponseTypeDef = TypedDict(
-    "ListIndexResponseTypeDef",
+BatchWriteOperationResponseTypeDef = TypedDict(
+    "BatchWriteOperationResponseTypeDef",
     {
-        "IndexAttachments": List[IndexAttachmentTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "CreateObject": BatchCreateObjectResponseTypeDef,
+        "AttachObject": BatchAttachObjectResponseTypeDef,
+        "DetachObject": BatchDetachObjectResponseTypeDef,
+        "UpdateObjectAttributes": BatchUpdateObjectAttributesResponseTypeDef,
+        "DeleteObject": Dict[str, Any],
+        "AddFacetToObject": Dict[str, Any],
+        "RemoveFacetFromObject": Dict[str, Any],
+        "AttachPolicy": Dict[str, Any],
+        "DetachPolicy": Dict[str, Any],
+        "CreateIndex": BatchCreateIndexResponseTypeDef,
+        "AttachToIndex": BatchAttachToIndexResponseTypeDef,
+        "DetachFromIndex": BatchDetachFromIndexResponseTypeDef,
+        "AttachTypedLink": BatchAttachTypedLinkResponseTypeDef,
+        "DetachTypedLink": Dict[str, Any],
+        "UpdateLinkAttributes": Dict[str, Any],
     },
+    total=False,
 )
 
-AttachTypedLinkResponseTypeDef = TypedDict(
-    "AttachTypedLinkResponseTypeDef",
+BatchReadSuccessfulResponseTypeDef = TypedDict(
+    "BatchReadSuccessfulResponseTypeDef",
     {
-        "TypedLinkSpecifier": TypedLinkSpecifierOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ListObjectAttributes": BatchListObjectAttributesResponseTypeDef,
+        "ListObjectChildren": BatchListObjectChildrenResponseTypeDef,
+        "GetObjectInformation": BatchGetObjectInformationResponseTypeDef,
+        "GetObjectAttributes": BatchGetObjectAttributesResponseTypeDef,
+        "ListAttachedIndices": BatchListAttachedIndicesResponseTypeDef,
+        "ListObjectParentPaths": BatchListObjectParentPathsResponseTypeDef,
+        "ListObjectPolicies": BatchListObjectPoliciesResponseTypeDef,
+        "ListPolicyAttachments": BatchListPolicyAttachmentsResponseTypeDef,
+        "LookupPolicy": BatchLookupPolicyResponseTypeDef,
+        "ListIndex": BatchListIndexResponseTypeDef,
+        "ListOutgoingTypedLinks": BatchListOutgoingTypedLinksResponseTypeDef,
+        "ListIncomingTypedLinks": BatchListIncomingTypedLinksResponseTypeDef,
+        "GetLinkAttributes": BatchGetLinkAttributesResponseTypeDef,
+        "ListObjectParents": BatchListObjectParentsResponseTypeDef,
     },
+    total=False,
 )
 
-BatchAttachTypedLinkResponseTypeDef = TypedDict(
-    "BatchAttachTypedLinkResponseTypeDef",
+_RequiredAddFacetToObjectRequestRequestTypeDef = TypedDict(
+    "_RequiredAddFacetToObjectRequestRequestTypeDef",
     {
-        "TypedLinkSpecifier": TypedLinkSpecifierOutputTypeDef,
+        "DirectoryArn": str,
+        "SchemaFacet": SchemaFacetTypeDef,
+        "ObjectReference": ObjectReferenceTypeDef,
     },
-    total=False,
 )
-
-BatchListIncomingTypedLinksResponseTypeDef = TypedDict(
-    "BatchListIncomingTypedLinksResponseTypeDef",
+_OptionalAddFacetToObjectRequestRequestTypeDef = TypedDict(
+    "_OptionalAddFacetToObjectRequestRequestTypeDef",
     {
-        "LinkSpecifiers": List[TypedLinkSpecifierOutputTypeDef],
-        "NextToken": str,
+        "ObjectAttributeList": Sequence[AttributeKeyAndValueUnionTypeDef],
     },
     total=False,
 )
 
-BatchListOutgoingTypedLinksResponseTypeDef = TypedDict(
-    "BatchListOutgoingTypedLinksResponseTypeDef",
+
+class AddFacetToObjectRequestRequestTypeDef(
+    _RequiredAddFacetToObjectRequestRequestTypeDef, _OptionalAddFacetToObjectRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredCreateObjectRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateObjectRequestRequestTypeDef",
     {
-        "TypedLinkSpecifiers": List[TypedLinkSpecifierOutputTypeDef],
-        "NextToken": str,
+        "DirectoryArn": str,
+        "SchemaFacets": Sequence[SchemaFacetTypeDef],
     },
-    total=False,
 )
-
-ListIncomingTypedLinksResponseTypeDef = TypedDict(
-    "ListIncomingTypedLinksResponseTypeDef",
+_OptionalCreateObjectRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateObjectRequestRequestTypeDef",
     {
-        "LinkSpecifiers": List[TypedLinkSpecifierOutputTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ObjectAttributeList": Sequence[AttributeKeyAndValueUnionTypeDef],
+        "ParentReference": ObjectReferenceTypeDef,
+        "LinkName": str,
     },
+    total=False,
 )
 
-ListOutgoingTypedLinksResponseTypeDef = TypedDict(
-    "ListOutgoingTypedLinksResponseTypeDef",
+
+class CreateObjectRequestRequestTypeDef(
+    _RequiredCreateObjectRequestRequestTypeDef, _OptionalCreateObjectRequestRequestTypeDef
+):
+    pass
+
+
+AttachTypedLinkRequestRequestTypeDef = TypedDict(
+    "AttachTypedLinkRequestRequestTypeDef",
     {
-        "TypedLinkSpecifiers": List[TypedLinkSpecifierOutputTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "DirectoryArn": str,
+        "SourceObjectReference": ObjectReferenceTypeDef,
+        "TargetObjectReference": ObjectReferenceTypeDef,
+        "TypedLinkFacet": TypedLinkSchemaAndFacetNameTypeDef,
+        "Attributes": Sequence[AttributeNameAndValueUnionTypeDef],
     },
 )
 
 BatchDetachTypedLinkTypeDef = TypedDict(
     "BatchDetachTypedLinkTypeDef",
     {
         "TypedLinkSpecifier": TypedLinkSpecifierTypeDef,
@@ -2852,14 +2912,25 @@
 
 class GetLinkAttributesRequestRequestTypeDef(
     _RequiredGetLinkAttributesRequestRequestTypeDef, _OptionalGetLinkAttributesRequestRequestTypeDef
 ):
     pass
 
 
+TypedLinkSpecifierUnionTypeDef = Union[TypedLinkSpecifierTypeDef, TypedLinkSpecifierOutputTypeDef]
+FacetAttributeUnionTypeDef = Union[FacetAttributeTypeDef, FacetAttributeOutputTypeDef]
+FacetAttributeUpdateTypeDef = TypedDict(
+    "FacetAttributeUpdateTypeDef",
+    {
+        "Attribute": FacetAttributeTypeDef,
+        "Action": UpdateActionTypeType,
+    },
+    total=False,
+)
+
 BatchUpdateLinkAttributesTypeDef = TypedDict(
     "BatchUpdateLinkAttributesTypeDef",
     {
         "TypedLinkSpecifier": TypedLinkSpecifierTypeDef,
         "AttributeUpdates": Sequence[LinkAttributeUpdateTypeDef],
     },
 )
@@ -3111,116 +3182,95 @@
 class ListOutgoingTypedLinksRequestRequestTypeDef(
     _RequiredListOutgoingTypedLinksRequestRequestTypeDef,
     _OptionalListOutgoingTypedLinksRequestRequestTypeDef,
 ):
     pass
 
 
-ListFacetAttributesResponseTypeDef = TypedDict(
-    "ListFacetAttributesResponseTypeDef",
+UpdateTypedLinkFacetRequestRequestTypeDef = TypedDict(
+    "UpdateTypedLinkFacetRequestRequestTypeDef",
     {
-        "Attributes": List[FacetAttributeOutputTypeDef],
-        "NextToken": str,
+        "SchemaArn": str,
+        "Name": str,
+        "AttributeUpdates": Sequence[TypedLinkFacetAttributeUpdateTypeDef],
+        "IdentityAttributeOrder": Sequence[str],
+    },
+)
+
+CreateTypedLinkFacetRequestRequestTypeDef = TypedDict(
+    "CreateTypedLinkFacetRequestRequestTypeDef",
+    {
+        "SchemaArn": str,
+        "Facet": TypedLinkFacetTypeDef,
+    },
+)
+
+BatchWriteResponseTypeDef = TypedDict(
+    "BatchWriteResponseTypeDef",
+    {
+        "Responses": List[BatchWriteOperationResponseTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+BatchReadOperationResponseTypeDef = TypedDict(
+    "BatchReadOperationResponseTypeDef",
+    {
+        "SuccessfulResponse": BatchReadSuccessfulResponseTypeDef,
+        "ExceptionResponse": BatchReadExceptionTypeDef,
+    },
+    total=False,
+)
+
 _RequiredCreateFacetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFacetRequestRequestTypeDef",
     {
         "SchemaArn": str,
         "Name": str,
     },
 )
 _OptionalCreateFacetRequestRequestTypeDef = TypedDict(
     "_OptionalCreateFacetRequestRequestTypeDef",
     {
-        "Attributes": Sequence[Union[FacetAttributeTypeDef, FacetAttributeOutputTypeDef]],
+        "Attributes": Sequence[FacetAttributeUnionTypeDef],
         "ObjectType": ObjectTypeType,
         "FacetStyle": FacetStyleType,
     },
     total=False,
 )
 
 
 class CreateFacetRequestRequestTypeDef(
     _RequiredCreateFacetRequestRequestTypeDef, _OptionalCreateFacetRequestRequestTypeDef
 ):
     pass
 
 
-FacetAttributeUpdateTypeDef = TypedDict(
-    "FacetAttributeUpdateTypeDef",
-    {
-        "Attribute": FacetAttributeTypeDef,
-        "Action": UpdateActionTypeType,
-    },
-    total=False,
-)
-
-UpdateTypedLinkFacetRequestRequestTypeDef = TypedDict(
-    "UpdateTypedLinkFacetRequestRequestTypeDef",
+_RequiredUpdateFacetRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateFacetRequestRequestTypeDef",
     {
         "SchemaArn": str,
         "Name": str,
-        "AttributeUpdates": Sequence[TypedLinkFacetAttributeUpdateTypeDef],
-        "IdentityAttributeOrder": Sequence[str],
     },
 )
-
-CreateTypedLinkFacetRequestRequestTypeDef = TypedDict(
-    "CreateTypedLinkFacetRequestRequestTypeDef",
-    {
-        "SchemaArn": str,
-        "Facet": TypedLinkFacetTypeDef,
-    },
-)
-
-BatchWriteOperationResponseTypeDef = TypedDict(
-    "BatchWriteOperationResponseTypeDef",
+_OptionalUpdateFacetRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateFacetRequestRequestTypeDef",
     {
-        "CreateObject": BatchCreateObjectResponseTypeDef,
-        "AttachObject": BatchAttachObjectResponseTypeDef,
-        "DetachObject": BatchDetachObjectResponseTypeDef,
-        "UpdateObjectAttributes": BatchUpdateObjectAttributesResponseTypeDef,
-        "DeleteObject": Dict[str, Any],
-        "AddFacetToObject": Dict[str, Any],
-        "RemoveFacetFromObject": Dict[str, Any],
-        "AttachPolicy": Dict[str, Any],
-        "DetachPolicy": Dict[str, Any],
-        "CreateIndex": BatchCreateIndexResponseTypeDef,
-        "AttachToIndex": BatchAttachToIndexResponseTypeDef,
-        "DetachFromIndex": BatchDetachFromIndexResponseTypeDef,
-        "AttachTypedLink": BatchAttachTypedLinkResponseTypeDef,
-        "DetachTypedLink": Dict[str, Any],
-        "UpdateLinkAttributes": Dict[str, Any],
+        "AttributeUpdates": Sequence[FacetAttributeUpdateTypeDef],
+        "ObjectType": ObjectTypeType,
     },
     total=False,
 )
 
-BatchReadSuccessfulResponseTypeDef = TypedDict(
-    "BatchReadSuccessfulResponseTypeDef",
-    {
-        "ListObjectAttributes": BatchListObjectAttributesResponseTypeDef,
-        "ListObjectChildren": BatchListObjectChildrenResponseTypeDef,
-        "GetObjectInformation": BatchGetObjectInformationResponseTypeDef,
-        "GetObjectAttributes": BatchGetObjectAttributesResponseTypeDef,
-        "ListAttachedIndices": BatchListAttachedIndicesResponseTypeDef,
-        "ListObjectParentPaths": BatchListObjectParentPathsResponseTypeDef,
-        "ListObjectPolicies": BatchListObjectPoliciesResponseTypeDef,
-        "ListPolicyAttachments": BatchListPolicyAttachmentsResponseTypeDef,
-        "LookupPolicy": BatchLookupPolicyResponseTypeDef,
-        "ListIndex": BatchListIndexResponseTypeDef,
-        "ListOutgoingTypedLinks": BatchListOutgoingTypedLinksResponseTypeDef,
-        "ListIncomingTypedLinks": BatchListIncomingTypedLinksResponseTypeDef,
-        "GetLinkAttributes": BatchGetLinkAttributesResponseTypeDef,
-        "ListObjectParents": BatchListObjectParentsResponseTypeDef,
-    },
-    total=False,
-)
+
+class UpdateFacetRequestRequestTypeDef(
+    _RequiredUpdateFacetRequestRequestTypeDef, _OptionalUpdateFacetRequestRequestTypeDef
+):
+    pass
+
 
 BatchWriteOperationTypeDef = TypedDict(
     "BatchWriteOperationTypeDef",
     {
         "CreateObject": BatchCreateObjectTypeDef,
         "AttachObject": BatchAttachObjectTypeDef,
         "DetachObject": BatchDetachObjectTypeDef,
@@ -3257,54 +3307,22 @@
         "ListOutgoingTypedLinks": BatchListOutgoingTypedLinksTypeDef,
         "ListIncomingTypedLinks": BatchListIncomingTypedLinksTypeDef,
         "GetLinkAttributes": BatchGetLinkAttributesTypeDef,
     },
     total=False,
 )
 
-_RequiredUpdateFacetRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateFacetRequestRequestTypeDef",
-    {
-        "SchemaArn": str,
-        "Name": str,
-    },
-)
-_OptionalUpdateFacetRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateFacetRequestRequestTypeDef",
-    {
-        "AttributeUpdates": Sequence[FacetAttributeUpdateTypeDef],
-        "ObjectType": ObjectTypeType,
-    },
-    total=False,
-)
-
-
-class UpdateFacetRequestRequestTypeDef(
-    _RequiredUpdateFacetRequestRequestTypeDef, _OptionalUpdateFacetRequestRequestTypeDef
-):
-    pass
-
-
-BatchWriteResponseTypeDef = TypedDict(
-    "BatchWriteResponseTypeDef",
+BatchReadResponseTypeDef = TypedDict(
+    "BatchReadResponseTypeDef",
     {
-        "Responses": List[BatchWriteOperationResponseTypeDef],
+        "Responses": List[BatchReadOperationResponseTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BatchReadOperationResponseTypeDef = TypedDict(
-    "BatchReadOperationResponseTypeDef",
-    {
-        "SuccessfulResponse": BatchReadSuccessfulResponseTypeDef,
-        "ExceptionResponse": BatchReadExceptionTypeDef,
-    },
-    total=False,
-)
-
 BatchWriteRequestRequestTypeDef = TypedDict(
     "BatchWriteRequestRequestTypeDef",
     {
         "DirectoryArn": str,
         "Operations": Sequence[BatchWriteOperationTypeDef],
     },
 )
@@ -3325,16 +3343,7 @@
 )
 
 
 class BatchReadRequestRequestTypeDef(
     _RequiredBatchReadRequestRequestTypeDef, _OptionalBatchReadRequestRequestTypeDef
 ):
     pass
-
-
-BatchReadResponseTypeDef = TypedDict(
-    "BatchReadResponseTypeDef",
-    {
-        "Responses": List[BatchReadOperationResponseTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
```

### Comparing `mypy-boto3-clouddirectory-1.28.15.post1/mypy_boto3_clouddirectory/type_defs.pyi` & `mypy-boto3-clouddirectory-1.28.16/mypy_boto3_clouddirectory/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_clouddirectory.type_defs import ObjectReferenceTypeDef
 
-    data: ObjectReferenceTypeDef = {...}
+    data: ObjectReferenceTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -39,28 +39,28 @@
     "ObjectReferenceTypeDef",
     "SchemaFacetTypeDef",
     "ApplySchemaRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "TypedLinkSchemaAndFacetNameTypeDef",
     "AttributeKeyTypeDef",
     "TypedAttributeValueOutputTypeDef",
-    "TypedAttributeValueTypeDef",
     "BatchAttachObjectResponseTypeDef",
     "BatchAttachToIndexResponseTypeDef",
     "BatchCreateIndexResponseTypeDef",
     "BatchCreateObjectResponseTypeDef",
     "BatchDetachFromIndexResponseTypeDef",
     "BatchDetachObjectResponseTypeDef",
     "BatchListObjectChildrenResponseTypeDef",
     "PathToObjectIdentifiersTypeDef",
     "ObjectIdentifierAndLinkNameTupleTypeDef",
     "BatchListObjectPoliciesResponseTypeDef",
     "BatchListPolicyAttachmentsResponseTypeDef",
     "BatchReadExceptionTypeDef",
     "BatchUpdateObjectAttributesResponseTypeDef",
+    "BlobTypeDef",
     "CreateDirectoryRequestRequestTypeDef",
     "CreateSchemaRequestRequestTypeDef",
     "DeleteDirectoryRequestRequestTypeDef",
     "DeleteFacetRequestRequestTypeDef",
     "DeleteSchemaRequestRequestTypeDef",
     "DeleteTypedLinkFacetRequestRequestTypeDef",
     "DirectoryTypeDef",
@@ -86,14 +86,15 @@
     "ListTagsForResourceRequestRequestTypeDef",
     "TagTypeDef",
     "ListTypedLinkFacetAttributesRequestRequestTypeDef",
     "ListTypedLinkFacetNamesRequestRequestTypeDef",
     "PolicyAttachmentTypeDef",
     "PublishSchemaRequestRequestTypeDef",
     "PutSchemaFromJsonRequestRequestTypeDef",
+    "TimestampTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateSchemaRequestRequestTypeDef",
     "UpgradeAppliedSchemaRequestRequestTypeDef",
     "UpgradePublishedSchemaRequestRequestTypeDef",
     "AttachObjectRequestRequestTypeDef",
     "AttachPolicyRequestRequestTypeDef",
     "AttachToIndexRequestRequestTypeDef",
@@ -164,29 +165,22 @@
     "UpdateSchemaResponseTypeDef",
     "UpgradeAppliedSchemaResponseTypeDef",
     "UpgradePublishedSchemaResponseTypeDef",
     "BatchCreateIndexTypeDef",
     "CreateIndexRequestRequestTypeDef",
     "AttributeKeyAndValueOutputTypeDef",
     "AttributeNameAndValueOutputTypeDef",
-    "AttributeKeyAndValueTypeDef",
-    "AttributeNameAndValueTypeDef",
-    "LinkAttributeActionTypeDef",
-    "ObjectAttributeActionTypeDef",
-    "TypedAttributeValueRangeTypeDef",
     "BatchListObjectParentPathsResponseTypeDef",
     "ListObjectParentPathsResponseTypeDef",
     "BatchListObjectParentsResponseTypeDef",
     "ListObjectParentsResponseTypeDef",
     "GetDirectoryResponseTypeDef",
     "ListDirectoriesResponseTypeDef",
     "FacetAttributeDefinitionOutputTypeDef",
     "TypedLinkAttributeDefinitionOutputTypeDef",
-    "FacetAttributeDefinitionTypeDef",
-    "TypedLinkAttributeDefinitionTypeDef",
     "GetFacetResponseTypeDef",
     "ListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef",
     "ListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef",
     "ListDevelopmentSchemaArnsRequestListDevelopmentSchemaArnsPaginateTypeDef",
     "ListDirectoriesRequestListDirectoriesPaginateTypeDef",
     "ListFacetAttributesRequestListFacetAttributesPaginateTypeDef",
     "ListFacetNamesRequestListFacetNamesPaginateTypeDef",
@@ -199,82 +193,94 @@
     "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef",
     "ListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef",
     "LookupPolicyRequestLookupPolicyPaginateTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "PolicyToPathTypeDef",
+    "TypedAttributeValueTypeDef",
     "BatchGetLinkAttributesResponseTypeDef",
     "BatchGetObjectAttributesResponseTypeDef",
     "BatchListObjectAttributesResponseTypeDef",
     "GetLinkAttributesResponseTypeDef",
     "GetObjectAttributesResponseTypeDef",
     "IndexAttachmentTypeDef",
     "ListObjectAttributesResponseTypeDef",
     "TypedLinkSpecifierOutputTypeDef",
-    "AddFacetToObjectRequestRequestTypeDef",
-    "BatchAddFacetToObjectTypeDef",
-    "BatchCreateObjectTypeDef",
-    "CreateObjectRequestRequestTypeDef",
-    "AttachTypedLinkRequestRequestTypeDef",
-    "BatchAttachTypedLinkTypeDef",
-    "TypedLinkSpecifierTypeDef",
-    "LinkAttributeUpdateTypeDef",
-    "ObjectAttributeUpdateTypeDef",
-    "ObjectAttributeRangeTypeDef",
-    "TypedLinkAttributeRangeTypeDef",
     "FacetAttributeOutputTypeDef",
     "ListTypedLinkFacetAttributesResponseTypeDef",
-    "FacetAttributeTypeDef",
-    "TypedLinkFacetAttributeUpdateTypeDef",
-    "TypedLinkFacetTypeDef",
     "BatchLookupPolicyResponseTypeDef",
     "LookupPolicyResponseTypeDef",
+    "AttributeKeyAndValueTypeDef",
+    "AttributeNameAndValueTypeDef",
+    "FacetAttributeDefinitionTypeDef",
+    "LinkAttributeActionTypeDef",
+    "ObjectAttributeActionTypeDef",
+    "TypedAttributeValueRangeTypeDef",
+    "TypedLinkAttributeDefinitionTypeDef",
     "BatchListAttachedIndicesResponseTypeDef",
     "BatchListIndexResponseTypeDef",
     "ListAttachedIndicesResponseTypeDef",
     "ListIndexResponseTypeDef",
     "AttachTypedLinkResponseTypeDef",
     "BatchAttachTypedLinkResponseTypeDef",
     "BatchListIncomingTypedLinksResponseTypeDef",
     "BatchListOutgoingTypedLinksResponseTypeDef",
     "ListIncomingTypedLinksResponseTypeDef",
     "ListOutgoingTypedLinksResponseTypeDef",
+    "ListFacetAttributesResponseTypeDef",
+    "AttributeKeyAndValueUnionTypeDef",
+    "BatchAddFacetToObjectTypeDef",
+    "BatchCreateObjectTypeDef",
+    "AttributeNameAndValueUnionTypeDef",
+    "BatchAttachTypedLinkTypeDef",
+    "TypedLinkSpecifierTypeDef",
+    "FacetAttributeTypeDef",
+    "LinkAttributeUpdateTypeDef",
+    "ObjectAttributeUpdateTypeDef",
+    "ObjectAttributeRangeTypeDef",
+    "TypedLinkAttributeRangeTypeDef",
+    "TypedLinkFacetAttributeUpdateTypeDef",
+    "TypedLinkFacetTypeDef",
+    "BatchWriteOperationResponseTypeDef",
+    "BatchReadSuccessfulResponseTypeDef",
+    "AddFacetToObjectRequestRequestTypeDef",
+    "CreateObjectRequestRequestTypeDef",
+    "AttachTypedLinkRequestRequestTypeDef",
     "BatchDetachTypedLinkTypeDef",
     "BatchGetLinkAttributesTypeDef",
     "DetachTypedLinkRequestRequestTypeDef",
     "GetLinkAttributesRequestRequestTypeDef",
+    "TypedLinkSpecifierUnionTypeDef",
+    "FacetAttributeUnionTypeDef",
+    "FacetAttributeUpdateTypeDef",
     "BatchUpdateLinkAttributesTypeDef",
     "UpdateLinkAttributesRequestRequestTypeDef",
     "BatchUpdateObjectAttributesTypeDef",
     "UpdateObjectAttributesRequestRequestTypeDef",
     "BatchListIndexTypeDef",
     "ListIndexRequestListIndexPaginateTypeDef",
     "ListIndexRequestRequestTypeDef",
     "BatchListIncomingTypedLinksTypeDef",
     "BatchListOutgoingTypedLinksTypeDef",
     "ListIncomingTypedLinksRequestListIncomingTypedLinksPaginateTypeDef",
     "ListIncomingTypedLinksRequestRequestTypeDef",
     "ListOutgoingTypedLinksRequestListOutgoingTypedLinksPaginateTypeDef",
     "ListOutgoingTypedLinksRequestRequestTypeDef",
-    "ListFacetAttributesResponseTypeDef",
-    "CreateFacetRequestRequestTypeDef",
-    "FacetAttributeUpdateTypeDef",
     "UpdateTypedLinkFacetRequestRequestTypeDef",
     "CreateTypedLinkFacetRequestRequestTypeDef",
-    "BatchWriteOperationResponseTypeDef",
-    "BatchReadSuccessfulResponseTypeDef",
-    "BatchWriteOperationTypeDef",
-    "BatchReadOperationTypeDef",
-    "UpdateFacetRequestRequestTypeDef",
     "BatchWriteResponseTypeDef",
     "BatchReadOperationResponseTypeDef",
+    "CreateFacetRequestRequestTypeDef",
+    "UpdateFacetRequestRequestTypeDef",
+    "BatchWriteOperationTypeDef",
+    "BatchReadOperationTypeDef",
+    "BatchReadResponseTypeDef",
     "BatchWriteRequestRequestTypeDef",
     "BatchReadRequestRequestTypeDef",
-    "BatchReadResponseTypeDef",
 )
 
 ObjectReferenceTypeDef = TypedDict(
     "ObjectReferenceTypeDef",
     {
         "Selector": str,
     },
@@ -334,26 +340,14 @@
         "BooleanValue": bool,
         "NumberValue": str,
         "DatetimeValue": datetime,
     },
     total=False,
 )
 
-TypedAttributeValueTypeDef = TypedDict(
-    "TypedAttributeValueTypeDef",
-    {
-        "StringValue": str,
-        "BinaryValue": Union[str, bytes, IO[Any], StreamingBody],
-        "BooleanValue": bool,
-        "NumberValue": str,
-        "DatetimeValue": Union[datetime, str],
-    },
-    total=False,
-)
-
 BatchAttachObjectResponseTypeDef = TypedDict(
     "BatchAttachObjectResponseTypeDef",
     {
         "attachedObjectIdentifier": str,
     },
     total=False,
 )
@@ -456,14 +450,15 @@
     "BatchUpdateObjectAttributesResponseTypeDef",
     {
         "ObjectIdentifier": str,
     },
     total=False,
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 CreateDirectoryRequestRequestTypeDef = TypedDict(
     "CreateDirectoryRequestRequestTypeDef",
     {
         "Name": str,
         "SchemaArn": str,
     },
 )
@@ -824,14 +819,15 @@
     "PutSchemaFromJsonRequestRequestTypeDef",
     {
         "SchemaArn": str,
         "Document": str,
     },
 )
 
+TimestampTypeDef = Union[datetime, str]
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -1780,69 +1776,14 @@
     "AttributeNameAndValueOutputTypeDef",
     {
         "AttributeName": str,
         "Value": TypedAttributeValueOutputTypeDef,
     },
 )
 
-AttributeKeyAndValueTypeDef = TypedDict(
-    "AttributeKeyAndValueTypeDef",
-    {
-        "Key": AttributeKeyTypeDef,
-        "Value": TypedAttributeValueTypeDef,
-    },
-)
-
-AttributeNameAndValueTypeDef = TypedDict(
-    "AttributeNameAndValueTypeDef",
-    {
-        "AttributeName": str,
-        "Value": TypedAttributeValueTypeDef,
-    },
-)
-
-LinkAttributeActionTypeDef = TypedDict(
-    "LinkAttributeActionTypeDef",
-    {
-        "AttributeActionType": UpdateActionTypeType,
-        "AttributeUpdateValue": TypedAttributeValueTypeDef,
-    },
-    total=False,
-)
-
-ObjectAttributeActionTypeDef = TypedDict(
-    "ObjectAttributeActionTypeDef",
-    {
-        "ObjectAttributeActionType": UpdateActionTypeType,
-        "ObjectAttributeUpdateValue": TypedAttributeValueTypeDef,
-    },
-    total=False,
-)
-
-_RequiredTypedAttributeValueRangeTypeDef = TypedDict(
-    "_RequiredTypedAttributeValueRangeTypeDef",
-    {
-        "StartMode": RangeModeType,
-        "EndMode": RangeModeType,
-    },
-)
-_OptionalTypedAttributeValueRangeTypeDef = TypedDict(
-    "_OptionalTypedAttributeValueRangeTypeDef",
-    {
-        "StartValue": TypedAttributeValueTypeDef,
-        "EndValue": TypedAttributeValueTypeDef,
-    },
-    total=False,
-)
-
-class TypedAttributeValueRangeTypeDef(
-    _RequiredTypedAttributeValueRangeTypeDef, _OptionalTypedAttributeValueRangeTypeDef
-):
-    pass
-
 BatchListObjectParentPathsResponseTypeDef = TypedDict(
     "BatchListObjectParentPathsResponseTypeDef",
     {
         "PathToObjectIdentifiersList": List[PathToObjectIdentifiersTypeDef],
         "NextToken": str,
     },
     total=False,
@@ -1934,58 +1875,14 @@
 
 class TypedLinkAttributeDefinitionOutputTypeDef(
     _RequiredTypedLinkAttributeDefinitionOutputTypeDef,
     _OptionalTypedLinkAttributeDefinitionOutputTypeDef,
 ):
     pass
 
-_RequiredFacetAttributeDefinitionTypeDef = TypedDict(
-    "_RequiredFacetAttributeDefinitionTypeDef",
-    {
-        "Type": FacetAttributeTypeType,
-    },
-)
-_OptionalFacetAttributeDefinitionTypeDef = TypedDict(
-    "_OptionalFacetAttributeDefinitionTypeDef",
-    {
-        "DefaultValue": TypedAttributeValueTypeDef,
-        "IsImmutable": bool,
-        "Rules": Mapping[str, RuleTypeDef],
-    },
-    total=False,
-)
-
-class FacetAttributeDefinitionTypeDef(
-    _RequiredFacetAttributeDefinitionTypeDef, _OptionalFacetAttributeDefinitionTypeDef
-):
-    pass
-
-_RequiredTypedLinkAttributeDefinitionTypeDef = TypedDict(
-    "_RequiredTypedLinkAttributeDefinitionTypeDef",
-    {
-        "Name": str,
-        "Type": FacetAttributeTypeType,
-        "RequiredBehavior": RequiredAttributeBehaviorType,
-    },
-)
-_OptionalTypedLinkAttributeDefinitionTypeDef = TypedDict(
-    "_OptionalTypedLinkAttributeDefinitionTypeDef",
-    {
-        "DefaultValue": TypedAttributeValueTypeDef,
-        "IsImmutable": bool,
-        "Rules": Mapping[str, RuleTypeDef],
-    },
-    total=False,
-)
-
-class TypedLinkAttributeDefinitionTypeDef(
-    _RequiredTypedLinkAttributeDefinitionTypeDef, _OptionalTypedLinkAttributeDefinitionTypeDef
-):
-    pass
-
 GetFacetResponseTypeDef = TypedDict(
     "GetFacetResponseTypeDef",
     {
         "Facet": FacetTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2301,14 +2198,26 @@
     {
         "Path": str,
         "Policies": List[PolicyAttachmentTypeDef],
     },
     total=False,
 )
 
+TypedAttributeValueTypeDef = TypedDict(
+    "TypedAttributeValueTypeDef",
+    {
+        "StringValue": str,
+        "BinaryValue": BlobTypeDef,
+        "BooleanValue": bool,
+        "NumberValue": str,
+        "DatetimeValue": TimestampTypeDef,
+    },
+    total=False,
+)
+
 BatchGetLinkAttributesResponseTypeDef = TypedDict(
     "BatchGetLinkAttributesResponseTypeDef",
     {
         "Attributes": List[AttributeKeyAndValueOutputTypeDef],
     },
     total=False,
 )
@@ -2370,198 +2279,312 @@
         "TypedLinkFacet": TypedLinkSchemaAndFacetNameTypeDef,
         "SourceObjectReference": ObjectReferenceTypeDef,
         "TargetObjectReference": ObjectReferenceTypeDef,
         "IdentityAttributeValues": List[AttributeNameAndValueOutputTypeDef],
     },
 )
 
-_RequiredAddFacetToObjectRequestRequestTypeDef = TypedDict(
-    "_RequiredAddFacetToObjectRequestRequestTypeDef",
+_RequiredFacetAttributeOutputTypeDef = TypedDict(
+    "_RequiredFacetAttributeOutputTypeDef",
     {
-        "DirectoryArn": str,
-        "SchemaFacet": SchemaFacetTypeDef,
-        "ObjectReference": ObjectReferenceTypeDef,
+        "Name": str,
     },
 )
-_OptionalAddFacetToObjectRequestRequestTypeDef = TypedDict(
-    "_OptionalAddFacetToObjectRequestRequestTypeDef",
+_OptionalFacetAttributeOutputTypeDef = TypedDict(
+    "_OptionalFacetAttributeOutputTypeDef",
     {
-        "ObjectAttributeList": Sequence[
-            Union[AttributeKeyAndValueTypeDef, AttributeKeyAndValueOutputTypeDef]
-        ],
+        "AttributeDefinition": FacetAttributeDefinitionOutputTypeDef,
+        "AttributeReference": FacetAttributeReferenceTypeDef,
+        "RequiredBehavior": RequiredAttributeBehaviorType,
     },
     total=False,
 )
 
-class AddFacetToObjectRequestRequestTypeDef(
-    _RequiredAddFacetToObjectRequestRequestTypeDef, _OptionalAddFacetToObjectRequestRequestTypeDef
+class FacetAttributeOutputTypeDef(
+    _RequiredFacetAttributeOutputTypeDef, _OptionalFacetAttributeOutputTypeDef
 ):
     pass
 
-BatchAddFacetToObjectTypeDef = TypedDict(
-    "BatchAddFacetToObjectTypeDef",
+ListTypedLinkFacetAttributesResponseTypeDef = TypedDict(
+    "ListTypedLinkFacetAttributesResponseTypeDef",
     {
-        "SchemaFacet": SchemaFacetTypeDef,
-        "ObjectAttributeList": Sequence[AttributeKeyAndValueTypeDef],
-        "ObjectReference": ObjectReferenceTypeDef,
+        "Attributes": List[TypedLinkAttributeDefinitionOutputTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredBatchCreateObjectTypeDef = TypedDict(
-    "_RequiredBatchCreateObjectTypeDef",
+BatchLookupPolicyResponseTypeDef = TypedDict(
+    "BatchLookupPolicyResponseTypeDef",
     {
-        "SchemaFacet": Sequence[SchemaFacetTypeDef],
-        "ObjectAttributeList": Sequence[AttributeKeyAndValueTypeDef],
+        "PolicyToPathList": List[PolicyToPathTypeDef],
+        "NextToken": str,
     },
+    total=False,
 )
-_OptionalBatchCreateObjectTypeDef = TypedDict(
-    "_OptionalBatchCreateObjectTypeDef",
+
+LookupPolicyResponseTypeDef = TypedDict(
+    "LookupPolicyResponseTypeDef",
     {
-        "ParentReference": ObjectReferenceTypeDef,
-        "LinkName": str,
-        "BatchReferenceName": str,
+        "PolicyToPathList": List[PolicyToPathTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AttributeKeyAndValueTypeDef = TypedDict(
+    "AttributeKeyAndValueTypeDef",
+    {
+        "Key": AttributeKeyTypeDef,
+        "Value": TypedAttributeValueTypeDef,
+    },
+)
+
+AttributeNameAndValueTypeDef = TypedDict(
+    "AttributeNameAndValueTypeDef",
+    {
+        "AttributeName": str,
+        "Value": TypedAttributeValueTypeDef,
+    },
+)
+
+_RequiredFacetAttributeDefinitionTypeDef = TypedDict(
+    "_RequiredFacetAttributeDefinitionTypeDef",
+    {
+        "Type": FacetAttributeTypeType,
+    },
+)
+_OptionalFacetAttributeDefinitionTypeDef = TypedDict(
+    "_OptionalFacetAttributeDefinitionTypeDef",
+    {
+        "DefaultValue": TypedAttributeValueTypeDef,
+        "IsImmutable": bool,
+        "Rules": Mapping[str, RuleTypeDef],
     },
     total=False,
 )
 
-class BatchCreateObjectTypeDef(
-    _RequiredBatchCreateObjectTypeDef, _OptionalBatchCreateObjectTypeDef
+class FacetAttributeDefinitionTypeDef(
+    _RequiredFacetAttributeDefinitionTypeDef, _OptionalFacetAttributeDefinitionTypeDef
 ):
     pass
 
-_RequiredCreateObjectRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateObjectRequestRequestTypeDef",
+LinkAttributeActionTypeDef = TypedDict(
+    "LinkAttributeActionTypeDef",
     {
-        "DirectoryArn": str,
-        "SchemaFacets": Sequence[SchemaFacetTypeDef],
+        "AttributeActionType": UpdateActionTypeType,
+        "AttributeUpdateValue": TypedAttributeValueTypeDef,
     },
+    total=False,
 )
-_OptionalCreateObjectRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateObjectRequestRequestTypeDef",
+
+ObjectAttributeActionTypeDef = TypedDict(
+    "ObjectAttributeActionTypeDef",
     {
-        "ObjectAttributeList": Sequence[
-            Union[AttributeKeyAndValueTypeDef, AttributeKeyAndValueOutputTypeDef]
-        ],
-        "ParentReference": ObjectReferenceTypeDef,
-        "LinkName": str,
+        "ObjectAttributeActionType": UpdateActionTypeType,
+        "ObjectAttributeUpdateValue": TypedAttributeValueTypeDef,
     },
     total=False,
 )
 
-class CreateObjectRequestRequestTypeDef(
-    _RequiredCreateObjectRequestRequestTypeDef, _OptionalCreateObjectRequestRequestTypeDef
+_RequiredTypedAttributeValueRangeTypeDef = TypedDict(
+    "_RequiredTypedAttributeValueRangeTypeDef",
+    {
+        "StartMode": RangeModeType,
+        "EndMode": RangeModeType,
+    },
+)
+_OptionalTypedAttributeValueRangeTypeDef = TypedDict(
+    "_OptionalTypedAttributeValueRangeTypeDef",
+    {
+        "StartValue": TypedAttributeValueTypeDef,
+        "EndValue": TypedAttributeValueTypeDef,
+    },
+    total=False,
+)
+
+class TypedAttributeValueRangeTypeDef(
+    _RequiredTypedAttributeValueRangeTypeDef, _OptionalTypedAttributeValueRangeTypeDef
 ):
     pass
 
-AttachTypedLinkRequestRequestTypeDef = TypedDict(
-    "AttachTypedLinkRequestRequestTypeDef",
+_RequiredTypedLinkAttributeDefinitionTypeDef = TypedDict(
+    "_RequiredTypedLinkAttributeDefinitionTypeDef",
     {
-        "DirectoryArn": str,
-        "SourceObjectReference": ObjectReferenceTypeDef,
-        "TargetObjectReference": ObjectReferenceTypeDef,
-        "TypedLinkFacet": TypedLinkSchemaAndFacetNameTypeDef,
-        "Attributes": Sequence[
-            Union[AttributeNameAndValueTypeDef, AttributeNameAndValueOutputTypeDef]
-        ],
+        "Name": str,
+        "Type": FacetAttributeTypeType,
+        "RequiredBehavior": RequiredAttributeBehaviorType,
     },
 )
+_OptionalTypedLinkAttributeDefinitionTypeDef = TypedDict(
+    "_OptionalTypedLinkAttributeDefinitionTypeDef",
+    {
+        "DefaultValue": TypedAttributeValueTypeDef,
+        "IsImmutable": bool,
+        "Rules": Mapping[str, RuleTypeDef],
+    },
+    total=False,
+)
 
-BatchAttachTypedLinkTypeDef = TypedDict(
-    "BatchAttachTypedLinkTypeDef",
+class TypedLinkAttributeDefinitionTypeDef(
+    _RequiredTypedLinkAttributeDefinitionTypeDef, _OptionalTypedLinkAttributeDefinitionTypeDef
+):
+    pass
+
+BatchListAttachedIndicesResponseTypeDef = TypedDict(
+    "BatchListAttachedIndicesResponseTypeDef",
     {
-        "SourceObjectReference": ObjectReferenceTypeDef,
-        "TargetObjectReference": ObjectReferenceTypeDef,
-        "TypedLinkFacet": TypedLinkSchemaAndFacetNameTypeDef,
-        "Attributes": Sequence[AttributeNameAndValueTypeDef],
+        "IndexAttachments": List[IndexAttachmentTypeDef],
+        "NextToken": str,
     },
+    total=False,
 )
 
-TypedLinkSpecifierTypeDef = TypedDict(
-    "TypedLinkSpecifierTypeDef",
+BatchListIndexResponseTypeDef = TypedDict(
+    "BatchListIndexResponseTypeDef",
     {
-        "TypedLinkFacet": TypedLinkSchemaAndFacetNameTypeDef,
-        "SourceObjectReference": ObjectReferenceTypeDef,
-        "TargetObjectReference": ObjectReferenceTypeDef,
-        "IdentityAttributeValues": Sequence[AttributeNameAndValueTypeDef],
+        "IndexAttachments": List[IndexAttachmentTypeDef],
+        "NextToken": str,
     },
+    total=False,
 )
 
-LinkAttributeUpdateTypeDef = TypedDict(
-    "LinkAttributeUpdateTypeDef",
+ListAttachedIndicesResponseTypeDef = TypedDict(
+    "ListAttachedIndicesResponseTypeDef",
     {
-        "AttributeKey": AttributeKeyTypeDef,
-        "AttributeAction": LinkAttributeActionTypeDef,
+        "IndexAttachments": List[IndexAttachmentTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListIndexResponseTypeDef = TypedDict(
+    "ListIndexResponseTypeDef",
+    {
+        "IndexAttachments": List[IndexAttachmentTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AttachTypedLinkResponseTypeDef = TypedDict(
+    "AttachTypedLinkResponseTypeDef",
+    {
+        "TypedLinkSpecifier": TypedLinkSpecifierOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+BatchAttachTypedLinkResponseTypeDef = TypedDict(
+    "BatchAttachTypedLinkResponseTypeDef",
+    {
+        "TypedLinkSpecifier": TypedLinkSpecifierOutputTypeDef,
     },
     total=False,
 )
 
-ObjectAttributeUpdateTypeDef = TypedDict(
-    "ObjectAttributeUpdateTypeDef",
+BatchListIncomingTypedLinksResponseTypeDef = TypedDict(
+    "BatchListIncomingTypedLinksResponseTypeDef",
     {
-        "ObjectAttributeKey": AttributeKeyTypeDef,
-        "ObjectAttributeAction": ObjectAttributeActionTypeDef,
+        "LinkSpecifiers": List[TypedLinkSpecifierOutputTypeDef],
+        "NextToken": str,
     },
     total=False,
 )
 
-ObjectAttributeRangeTypeDef = TypedDict(
-    "ObjectAttributeRangeTypeDef",
+BatchListOutgoingTypedLinksResponseTypeDef = TypedDict(
+    "BatchListOutgoingTypedLinksResponseTypeDef",
     {
-        "AttributeKey": AttributeKeyTypeDef,
-        "Range": TypedAttributeValueRangeTypeDef,
+        "TypedLinkSpecifiers": List[TypedLinkSpecifierOutputTypeDef],
+        "NextToken": str,
     },
     total=False,
 )
 
-_RequiredTypedLinkAttributeRangeTypeDef = TypedDict(
-    "_RequiredTypedLinkAttributeRangeTypeDef",
+ListIncomingTypedLinksResponseTypeDef = TypedDict(
+    "ListIncomingTypedLinksResponseTypeDef",
     {
-        "Range": TypedAttributeValueRangeTypeDef,
+        "LinkSpecifiers": List[TypedLinkSpecifierOutputTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalTypedLinkAttributeRangeTypeDef = TypedDict(
-    "_OptionalTypedLinkAttributeRangeTypeDef",
+
+ListOutgoingTypedLinksResponseTypeDef = TypedDict(
+    "ListOutgoingTypedLinksResponseTypeDef",
     {
-        "AttributeName": str,
+        "TypedLinkSpecifiers": List[TypedLinkSpecifierOutputTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class TypedLinkAttributeRangeTypeDef(
-    _RequiredTypedLinkAttributeRangeTypeDef, _OptionalTypedLinkAttributeRangeTypeDef
-):
-    pass
+ListFacetAttributesResponseTypeDef = TypedDict(
+    "ListFacetAttributesResponseTypeDef",
+    {
+        "Attributes": List[FacetAttributeOutputTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-_RequiredFacetAttributeOutputTypeDef = TypedDict(
-    "_RequiredFacetAttributeOutputTypeDef",
+AttributeKeyAndValueUnionTypeDef = Union[
+    AttributeKeyAndValueTypeDef, AttributeKeyAndValueOutputTypeDef
+]
+BatchAddFacetToObjectTypeDef = TypedDict(
+    "BatchAddFacetToObjectTypeDef",
     {
-        "Name": str,
+        "SchemaFacet": SchemaFacetTypeDef,
+        "ObjectAttributeList": Sequence[AttributeKeyAndValueTypeDef],
+        "ObjectReference": ObjectReferenceTypeDef,
     },
 )
-_OptionalFacetAttributeOutputTypeDef = TypedDict(
-    "_OptionalFacetAttributeOutputTypeDef",
+
+_RequiredBatchCreateObjectTypeDef = TypedDict(
+    "_RequiredBatchCreateObjectTypeDef",
     {
-        "AttributeDefinition": FacetAttributeDefinitionOutputTypeDef,
-        "AttributeReference": FacetAttributeReferenceTypeDef,
-        "RequiredBehavior": RequiredAttributeBehaviorType,
+        "SchemaFacet": Sequence[SchemaFacetTypeDef],
+        "ObjectAttributeList": Sequence[AttributeKeyAndValueTypeDef],
+    },
+)
+_OptionalBatchCreateObjectTypeDef = TypedDict(
+    "_OptionalBatchCreateObjectTypeDef",
+    {
+        "ParentReference": ObjectReferenceTypeDef,
+        "LinkName": str,
+        "BatchReferenceName": str,
     },
     total=False,
 )
 
-class FacetAttributeOutputTypeDef(
-    _RequiredFacetAttributeOutputTypeDef, _OptionalFacetAttributeOutputTypeDef
+class BatchCreateObjectTypeDef(
+    _RequiredBatchCreateObjectTypeDef, _OptionalBatchCreateObjectTypeDef
 ):
     pass
 
-ListTypedLinkFacetAttributesResponseTypeDef = TypedDict(
-    "ListTypedLinkFacetAttributesResponseTypeDef",
+AttributeNameAndValueUnionTypeDef = Union[
+    AttributeNameAndValueTypeDef, AttributeNameAndValueOutputTypeDef
+]
+BatchAttachTypedLinkTypeDef = TypedDict(
+    "BatchAttachTypedLinkTypeDef",
     {
-        "Attributes": List[TypedLinkAttributeDefinitionOutputTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "SourceObjectReference": ObjectReferenceTypeDef,
+        "TargetObjectReference": ObjectReferenceTypeDef,
+        "TypedLinkFacet": TypedLinkSchemaAndFacetNameTypeDef,
+        "Attributes": Sequence[AttributeNameAndValueTypeDef],
+    },
+)
+
+TypedLinkSpecifierTypeDef = TypedDict(
+    "TypedLinkSpecifierTypeDef",
+    {
+        "TypedLinkFacet": TypedLinkSchemaAndFacetNameTypeDef,
+        "SourceObjectReference": ObjectReferenceTypeDef,
+        "TargetObjectReference": ObjectReferenceTypeDef,
+        "IdentityAttributeValues": Sequence[AttributeNameAndValueTypeDef],
     },
 )
 
 _RequiredFacetAttributeTypeDef = TypedDict(
     "_RequiredFacetAttributeTypeDef",
     {
         "Name": str,
@@ -2576,134 +2599,171 @@
     },
     total=False,
 )
 
 class FacetAttributeTypeDef(_RequiredFacetAttributeTypeDef, _OptionalFacetAttributeTypeDef):
     pass
 
-TypedLinkFacetAttributeUpdateTypeDef = TypedDict(
-    "TypedLinkFacetAttributeUpdateTypeDef",
+LinkAttributeUpdateTypeDef = TypedDict(
+    "LinkAttributeUpdateTypeDef",
     {
-        "Attribute": TypedLinkAttributeDefinitionTypeDef,
-        "Action": UpdateActionTypeType,
+        "AttributeKey": AttributeKeyTypeDef,
+        "AttributeAction": LinkAttributeActionTypeDef,
     },
+    total=False,
 )
 
-TypedLinkFacetTypeDef = TypedDict(
-    "TypedLinkFacetTypeDef",
+ObjectAttributeUpdateTypeDef = TypedDict(
+    "ObjectAttributeUpdateTypeDef",
     {
-        "Name": str,
-        "Attributes": Sequence[TypedLinkAttributeDefinitionTypeDef],
-        "IdentityAttributeOrder": Sequence[str],
+        "ObjectAttributeKey": AttributeKeyTypeDef,
+        "ObjectAttributeAction": ObjectAttributeActionTypeDef,
     },
+    total=False,
 )
 
-BatchLookupPolicyResponseTypeDef = TypedDict(
-    "BatchLookupPolicyResponseTypeDef",
+ObjectAttributeRangeTypeDef = TypedDict(
+    "ObjectAttributeRangeTypeDef",
     {
-        "PolicyToPathList": List[PolicyToPathTypeDef],
-        "NextToken": str,
+        "AttributeKey": AttributeKeyTypeDef,
+        "Range": TypedAttributeValueRangeTypeDef,
     },
     total=False,
 )
 
-LookupPolicyResponseTypeDef = TypedDict(
-    "LookupPolicyResponseTypeDef",
+_RequiredTypedLinkAttributeRangeTypeDef = TypedDict(
+    "_RequiredTypedLinkAttributeRangeTypeDef",
     {
-        "PolicyToPathList": List[PolicyToPathTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Range": TypedAttributeValueRangeTypeDef,
     },
 )
-
-BatchListAttachedIndicesResponseTypeDef = TypedDict(
-    "BatchListAttachedIndicesResponseTypeDef",
+_OptionalTypedLinkAttributeRangeTypeDef = TypedDict(
+    "_OptionalTypedLinkAttributeRangeTypeDef",
     {
-        "IndexAttachments": List[IndexAttachmentTypeDef],
-        "NextToken": str,
+        "AttributeName": str,
     },
     total=False,
 )
 
-BatchListIndexResponseTypeDef = TypedDict(
-    "BatchListIndexResponseTypeDef",
+class TypedLinkAttributeRangeTypeDef(
+    _RequiredTypedLinkAttributeRangeTypeDef, _OptionalTypedLinkAttributeRangeTypeDef
+):
+    pass
+
+TypedLinkFacetAttributeUpdateTypeDef = TypedDict(
+    "TypedLinkFacetAttributeUpdateTypeDef",
     {
-        "IndexAttachments": List[IndexAttachmentTypeDef],
-        "NextToken": str,
+        "Attribute": TypedLinkAttributeDefinitionTypeDef,
+        "Action": UpdateActionTypeType,
     },
-    total=False,
 )
 
-ListAttachedIndicesResponseTypeDef = TypedDict(
-    "ListAttachedIndicesResponseTypeDef",
+TypedLinkFacetTypeDef = TypedDict(
+    "TypedLinkFacetTypeDef",
     {
-        "IndexAttachments": List[IndexAttachmentTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Name": str,
+        "Attributes": Sequence[TypedLinkAttributeDefinitionTypeDef],
+        "IdentityAttributeOrder": Sequence[str],
     },
 )
 
-ListIndexResponseTypeDef = TypedDict(
-    "ListIndexResponseTypeDef",
+BatchWriteOperationResponseTypeDef = TypedDict(
+    "BatchWriteOperationResponseTypeDef",
     {
-        "IndexAttachments": List[IndexAttachmentTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "CreateObject": BatchCreateObjectResponseTypeDef,
+        "AttachObject": BatchAttachObjectResponseTypeDef,
+        "DetachObject": BatchDetachObjectResponseTypeDef,
+        "UpdateObjectAttributes": BatchUpdateObjectAttributesResponseTypeDef,
+        "DeleteObject": Dict[str, Any],
+        "AddFacetToObject": Dict[str, Any],
+        "RemoveFacetFromObject": Dict[str, Any],
+        "AttachPolicy": Dict[str, Any],
+        "DetachPolicy": Dict[str, Any],
+        "CreateIndex": BatchCreateIndexResponseTypeDef,
+        "AttachToIndex": BatchAttachToIndexResponseTypeDef,
+        "DetachFromIndex": BatchDetachFromIndexResponseTypeDef,
+        "AttachTypedLink": BatchAttachTypedLinkResponseTypeDef,
+        "DetachTypedLink": Dict[str, Any],
+        "UpdateLinkAttributes": Dict[str, Any],
     },
+    total=False,
 )
 
-AttachTypedLinkResponseTypeDef = TypedDict(
-    "AttachTypedLinkResponseTypeDef",
+BatchReadSuccessfulResponseTypeDef = TypedDict(
+    "BatchReadSuccessfulResponseTypeDef",
     {
-        "TypedLinkSpecifier": TypedLinkSpecifierOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ListObjectAttributes": BatchListObjectAttributesResponseTypeDef,
+        "ListObjectChildren": BatchListObjectChildrenResponseTypeDef,
+        "GetObjectInformation": BatchGetObjectInformationResponseTypeDef,
+        "GetObjectAttributes": BatchGetObjectAttributesResponseTypeDef,
+        "ListAttachedIndices": BatchListAttachedIndicesResponseTypeDef,
+        "ListObjectParentPaths": BatchListObjectParentPathsResponseTypeDef,
+        "ListObjectPolicies": BatchListObjectPoliciesResponseTypeDef,
+        "ListPolicyAttachments": BatchListPolicyAttachmentsResponseTypeDef,
+        "LookupPolicy": BatchLookupPolicyResponseTypeDef,
+        "ListIndex": BatchListIndexResponseTypeDef,
+        "ListOutgoingTypedLinks": BatchListOutgoingTypedLinksResponseTypeDef,
+        "ListIncomingTypedLinks": BatchListIncomingTypedLinksResponseTypeDef,
+        "GetLinkAttributes": BatchGetLinkAttributesResponseTypeDef,
+        "ListObjectParents": BatchListObjectParentsResponseTypeDef,
     },
+    total=False,
 )
 
-BatchAttachTypedLinkResponseTypeDef = TypedDict(
-    "BatchAttachTypedLinkResponseTypeDef",
+_RequiredAddFacetToObjectRequestRequestTypeDef = TypedDict(
+    "_RequiredAddFacetToObjectRequestRequestTypeDef",
     {
-        "TypedLinkSpecifier": TypedLinkSpecifierOutputTypeDef,
+        "DirectoryArn": str,
+        "SchemaFacet": SchemaFacetTypeDef,
+        "ObjectReference": ObjectReferenceTypeDef,
     },
-    total=False,
 )
-
-BatchListIncomingTypedLinksResponseTypeDef = TypedDict(
-    "BatchListIncomingTypedLinksResponseTypeDef",
+_OptionalAddFacetToObjectRequestRequestTypeDef = TypedDict(
+    "_OptionalAddFacetToObjectRequestRequestTypeDef",
     {
-        "LinkSpecifiers": List[TypedLinkSpecifierOutputTypeDef],
-        "NextToken": str,
+        "ObjectAttributeList": Sequence[AttributeKeyAndValueUnionTypeDef],
     },
     total=False,
 )
 
-BatchListOutgoingTypedLinksResponseTypeDef = TypedDict(
-    "BatchListOutgoingTypedLinksResponseTypeDef",
+class AddFacetToObjectRequestRequestTypeDef(
+    _RequiredAddFacetToObjectRequestRequestTypeDef, _OptionalAddFacetToObjectRequestRequestTypeDef
+):
+    pass
+
+_RequiredCreateObjectRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateObjectRequestRequestTypeDef",
     {
-        "TypedLinkSpecifiers": List[TypedLinkSpecifierOutputTypeDef],
-        "NextToken": str,
+        "DirectoryArn": str,
+        "SchemaFacets": Sequence[SchemaFacetTypeDef],
     },
-    total=False,
 )
-
-ListIncomingTypedLinksResponseTypeDef = TypedDict(
-    "ListIncomingTypedLinksResponseTypeDef",
+_OptionalCreateObjectRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateObjectRequestRequestTypeDef",
     {
-        "LinkSpecifiers": List[TypedLinkSpecifierOutputTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ObjectAttributeList": Sequence[AttributeKeyAndValueUnionTypeDef],
+        "ParentReference": ObjectReferenceTypeDef,
+        "LinkName": str,
     },
+    total=False,
 )
 
-ListOutgoingTypedLinksResponseTypeDef = TypedDict(
-    "ListOutgoingTypedLinksResponseTypeDef",
+class CreateObjectRequestRequestTypeDef(
+    _RequiredCreateObjectRequestRequestTypeDef, _OptionalCreateObjectRequestRequestTypeDef
+):
+    pass
+
+AttachTypedLinkRequestRequestTypeDef = TypedDict(
+    "AttachTypedLinkRequestRequestTypeDef",
     {
-        "TypedLinkSpecifiers": List[TypedLinkSpecifierOutputTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "DirectoryArn": str,
+        "SourceObjectReference": ObjectReferenceTypeDef,
+        "TargetObjectReference": ObjectReferenceTypeDef,
+        "TypedLinkFacet": TypedLinkSchemaAndFacetNameTypeDef,
+        "Attributes": Sequence[AttributeNameAndValueUnionTypeDef],
     },
 )
 
 BatchDetachTypedLinkTypeDef = TypedDict(
     "BatchDetachTypedLinkTypeDef",
     {
         "TypedLinkSpecifier": TypedLinkSpecifierTypeDef,
@@ -2743,14 +2803,25 @@
 )
 
 class GetLinkAttributesRequestRequestTypeDef(
     _RequiredGetLinkAttributesRequestRequestTypeDef, _OptionalGetLinkAttributesRequestRequestTypeDef
 ):
     pass
 
+TypedLinkSpecifierUnionTypeDef = Union[TypedLinkSpecifierTypeDef, TypedLinkSpecifierOutputTypeDef]
+FacetAttributeUnionTypeDef = Union[FacetAttributeTypeDef, FacetAttributeOutputTypeDef]
+FacetAttributeUpdateTypeDef = TypedDict(
+    "FacetAttributeUpdateTypeDef",
+    {
+        "Attribute": FacetAttributeTypeDef,
+        "Action": UpdateActionTypeType,
+    },
+    total=False,
+)
+
 BatchUpdateLinkAttributesTypeDef = TypedDict(
     "BatchUpdateLinkAttributesTypeDef",
     {
         "TypedLinkSpecifier": TypedLinkSpecifierTypeDef,
         "AttributeUpdates": Sequence[LinkAttributeUpdateTypeDef],
     },
 )
@@ -2984,114 +3055,91 @@
 
 class ListOutgoingTypedLinksRequestRequestTypeDef(
     _RequiredListOutgoingTypedLinksRequestRequestTypeDef,
     _OptionalListOutgoingTypedLinksRequestRequestTypeDef,
 ):
     pass
 
-ListFacetAttributesResponseTypeDef = TypedDict(
-    "ListFacetAttributesResponseTypeDef",
+UpdateTypedLinkFacetRequestRequestTypeDef = TypedDict(
+    "UpdateTypedLinkFacetRequestRequestTypeDef",
     {
-        "Attributes": List[FacetAttributeOutputTypeDef],
-        "NextToken": str,
+        "SchemaArn": str,
+        "Name": str,
+        "AttributeUpdates": Sequence[TypedLinkFacetAttributeUpdateTypeDef],
+        "IdentityAttributeOrder": Sequence[str],
+    },
+)
+
+CreateTypedLinkFacetRequestRequestTypeDef = TypedDict(
+    "CreateTypedLinkFacetRequestRequestTypeDef",
+    {
+        "SchemaArn": str,
+        "Facet": TypedLinkFacetTypeDef,
+    },
+)
+
+BatchWriteResponseTypeDef = TypedDict(
+    "BatchWriteResponseTypeDef",
+    {
+        "Responses": List[BatchWriteOperationResponseTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+BatchReadOperationResponseTypeDef = TypedDict(
+    "BatchReadOperationResponseTypeDef",
+    {
+        "SuccessfulResponse": BatchReadSuccessfulResponseTypeDef,
+        "ExceptionResponse": BatchReadExceptionTypeDef,
+    },
+    total=False,
+)
+
 _RequiredCreateFacetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFacetRequestRequestTypeDef",
     {
         "SchemaArn": str,
         "Name": str,
     },
 )
 _OptionalCreateFacetRequestRequestTypeDef = TypedDict(
     "_OptionalCreateFacetRequestRequestTypeDef",
     {
-        "Attributes": Sequence[Union[FacetAttributeTypeDef, FacetAttributeOutputTypeDef]],
+        "Attributes": Sequence[FacetAttributeUnionTypeDef],
         "ObjectType": ObjectTypeType,
         "FacetStyle": FacetStyleType,
     },
     total=False,
 )
 
 class CreateFacetRequestRequestTypeDef(
     _RequiredCreateFacetRequestRequestTypeDef, _OptionalCreateFacetRequestRequestTypeDef
 ):
     pass
 
-FacetAttributeUpdateTypeDef = TypedDict(
-    "FacetAttributeUpdateTypeDef",
-    {
-        "Attribute": FacetAttributeTypeDef,
-        "Action": UpdateActionTypeType,
-    },
-    total=False,
-)
-
-UpdateTypedLinkFacetRequestRequestTypeDef = TypedDict(
-    "UpdateTypedLinkFacetRequestRequestTypeDef",
+_RequiredUpdateFacetRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateFacetRequestRequestTypeDef",
     {
         "SchemaArn": str,
         "Name": str,
-        "AttributeUpdates": Sequence[TypedLinkFacetAttributeUpdateTypeDef],
-        "IdentityAttributeOrder": Sequence[str],
     },
 )
-
-CreateTypedLinkFacetRequestRequestTypeDef = TypedDict(
-    "CreateTypedLinkFacetRequestRequestTypeDef",
-    {
-        "SchemaArn": str,
-        "Facet": TypedLinkFacetTypeDef,
-    },
-)
-
-BatchWriteOperationResponseTypeDef = TypedDict(
-    "BatchWriteOperationResponseTypeDef",
+_OptionalUpdateFacetRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateFacetRequestRequestTypeDef",
     {
-        "CreateObject": BatchCreateObjectResponseTypeDef,
-        "AttachObject": BatchAttachObjectResponseTypeDef,
-        "DetachObject": BatchDetachObjectResponseTypeDef,
-        "UpdateObjectAttributes": BatchUpdateObjectAttributesResponseTypeDef,
-        "DeleteObject": Dict[str, Any],
-        "AddFacetToObject": Dict[str, Any],
-        "RemoveFacetFromObject": Dict[str, Any],
-        "AttachPolicy": Dict[str, Any],
-        "DetachPolicy": Dict[str, Any],
-        "CreateIndex": BatchCreateIndexResponseTypeDef,
-        "AttachToIndex": BatchAttachToIndexResponseTypeDef,
-        "DetachFromIndex": BatchDetachFromIndexResponseTypeDef,
-        "AttachTypedLink": BatchAttachTypedLinkResponseTypeDef,
-        "DetachTypedLink": Dict[str, Any],
-        "UpdateLinkAttributes": Dict[str, Any],
+        "AttributeUpdates": Sequence[FacetAttributeUpdateTypeDef],
+        "ObjectType": ObjectTypeType,
     },
     total=False,
 )
 
-BatchReadSuccessfulResponseTypeDef = TypedDict(
-    "BatchReadSuccessfulResponseTypeDef",
-    {
-        "ListObjectAttributes": BatchListObjectAttributesResponseTypeDef,
-        "ListObjectChildren": BatchListObjectChildrenResponseTypeDef,
-        "GetObjectInformation": BatchGetObjectInformationResponseTypeDef,
-        "GetObjectAttributes": BatchGetObjectAttributesResponseTypeDef,
-        "ListAttachedIndices": BatchListAttachedIndicesResponseTypeDef,
-        "ListObjectParentPaths": BatchListObjectParentPathsResponseTypeDef,
-        "ListObjectPolicies": BatchListObjectPoliciesResponseTypeDef,
-        "ListPolicyAttachments": BatchListPolicyAttachmentsResponseTypeDef,
-        "LookupPolicy": BatchLookupPolicyResponseTypeDef,
-        "ListIndex": BatchListIndexResponseTypeDef,
-        "ListOutgoingTypedLinks": BatchListOutgoingTypedLinksResponseTypeDef,
-        "ListIncomingTypedLinks": BatchListIncomingTypedLinksResponseTypeDef,
-        "GetLinkAttributes": BatchGetLinkAttributesResponseTypeDef,
-        "ListObjectParents": BatchListObjectParentsResponseTypeDef,
-    },
-    total=False,
-)
+class UpdateFacetRequestRequestTypeDef(
+    _RequiredUpdateFacetRequestRequestTypeDef, _OptionalUpdateFacetRequestRequestTypeDef
+):
+    pass
 
 BatchWriteOperationTypeDef = TypedDict(
     "BatchWriteOperationTypeDef",
     {
         "CreateObject": BatchCreateObjectTypeDef,
         "AttachObject": BatchAttachObjectTypeDef,
         "DetachObject": BatchDetachObjectTypeDef,
@@ -3128,52 +3176,22 @@
         "ListOutgoingTypedLinks": BatchListOutgoingTypedLinksTypeDef,
         "ListIncomingTypedLinks": BatchListIncomingTypedLinksTypeDef,
         "GetLinkAttributes": BatchGetLinkAttributesTypeDef,
     },
     total=False,
 )
 
-_RequiredUpdateFacetRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateFacetRequestRequestTypeDef",
-    {
-        "SchemaArn": str,
-        "Name": str,
-    },
-)
-_OptionalUpdateFacetRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateFacetRequestRequestTypeDef",
-    {
-        "AttributeUpdates": Sequence[FacetAttributeUpdateTypeDef],
-        "ObjectType": ObjectTypeType,
-    },
-    total=False,
-)
-
-class UpdateFacetRequestRequestTypeDef(
-    _RequiredUpdateFacetRequestRequestTypeDef, _OptionalUpdateFacetRequestRequestTypeDef
-):
-    pass
-
-BatchWriteResponseTypeDef = TypedDict(
-    "BatchWriteResponseTypeDef",
+BatchReadResponseTypeDef = TypedDict(
+    "BatchReadResponseTypeDef",
     {
-        "Responses": List[BatchWriteOperationResponseTypeDef],
+        "Responses": List[BatchReadOperationResponseTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BatchReadOperationResponseTypeDef = TypedDict(
-    "BatchReadOperationResponseTypeDef",
-    {
-        "SuccessfulResponse": BatchReadSuccessfulResponseTypeDef,
-        "ExceptionResponse": BatchReadExceptionTypeDef,
-    },
-    total=False,
-)
-
 BatchWriteRequestRequestTypeDef = TypedDict(
     "BatchWriteRequestRequestTypeDef",
     {
         "DirectoryArn": str,
         "Operations": Sequence[BatchWriteOperationTypeDef],
     },
 )
@@ -3193,15 +3211,7 @@
     total=False,
 )
 
 class BatchReadRequestRequestTypeDef(
     _RequiredBatchReadRequestRequestTypeDef, _OptionalBatchReadRequestRequestTypeDef
 ):
     pass
-
-BatchReadResponseTypeDef = TypedDict(
-    "BatchReadResponseTypeDef",
-    {
-        "Responses": List[BatchReadOperationResponseTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
```

### Comparing `mypy-boto3-clouddirectory-1.28.15.post1/mypy_boto3_clouddirectory.egg-info/PKG-INFO` & `mypy-boto3-clouddirectory-1.28.16/mypy_boto3_clouddirectory.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-clouddirectory
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.CloudDirectory 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.CloudDirectory 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 clouddirectory type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 clouddirectory type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-clouddirectory.svg?color=blue)](https://pypi.org/project/mypy-boto3-clouddirectory)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-clouddirectory)](https://pepy.tech/project/mypy-boto3-clouddirectory)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudDirectory 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory)
+[boto3.CloudDirectory 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory)
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
 [mypy-boto3-clouddirectory docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/).
 
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
@@ -407,44 +407,44 @@
 )
 
 
 def check_value(value: BatchReadExceptionTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_clouddirectory.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_clouddirectory.type_defs import (
     ObjectReferenceTypeDef,
     SchemaFacetTypeDef,
     ApplySchemaRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     TypedLinkSchemaAndFacetNameTypeDef,
     AttributeKeyTypeDef,
     TypedAttributeValueOutputTypeDef,
-    TypedAttributeValueTypeDef,
     BatchAttachObjectResponseTypeDef,
     BatchAttachToIndexResponseTypeDef,
     BatchCreateIndexResponseTypeDef,
     BatchCreateObjectResponseTypeDef,
     BatchDetachFromIndexResponseTypeDef,
     BatchDetachObjectResponseTypeDef,
     BatchListObjectChildrenResponseTypeDef,
     PathToObjectIdentifiersTypeDef,
     ObjectIdentifierAndLinkNameTupleTypeDef,
     BatchListObjectPoliciesResponseTypeDef,
     BatchListPolicyAttachmentsResponseTypeDef,
     BatchReadExceptionTypeDef,
     BatchUpdateObjectAttributesResponseTypeDef,
+    BlobTypeDef,
     CreateDirectoryRequestRequestTypeDef,
     CreateSchemaRequestRequestTypeDef,
     DeleteDirectoryRequestRequestTypeDef,
     DeleteFacetRequestRequestTypeDef,
     DeleteSchemaRequestRequestTypeDef,
     DeleteTypedLinkFacetRequestRequestTypeDef,
     DirectoryTypeDef,
@@ -470,14 +470,15 @@
     ListTagsForResourceRequestRequestTypeDef,
     TagTypeDef,
     ListTypedLinkFacetAttributesRequestRequestTypeDef,
     ListTypedLinkFacetNamesRequestRequestTypeDef,
     PolicyAttachmentTypeDef,
     PublishSchemaRequestRequestTypeDef,
     PutSchemaFromJsonRequestRequestTypeDef,
+    TimestampTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateSchemaRequestRequestTypeDef,
     UpgradeAppliedSchemaRequestRequestTypeDef,
     UpgradePublishedSchemaRequestRequestTypeDef,
     AttachObjectRequestRequestTypeDef,
     AttachPolicyRequestRequestTypeDef,
     AttachToIndexRequestRequestTypeDef,
@@ -548,29 +549,22 @@
     UpdateSchemaResponseTypeDef,
     UpgradeAppliedSchemaResponseTypeDef,
     UpgradePublishedSchemaResponseTypeDef,
     BatchCreateIndexTypeDef,
     CreateIndexRequestRequestTypeDef,
     AttributeKeyAndValueOutputTypeDef,
     AttributeNameAndValueOutputTypeDef,
-    AttributeKeyAndValueTypeDef,
-    AttributeNameAndValueTypeDef,
-    LinkAttributeActionTypeDef,
-    ObjectAttributeActionTypeDef,
-    TypedAttributeValueRangeTypeDef,
     BatchListObjectParentPathsResponseTypeDef,
     ListObjectParentPathsResponseTypeDef,
     BatchListObjectParentsResponseTypeDef,
     ListObjectParentsResponseTypeDef,
     GetDirectoryResponseTypeDef,
     ListDirectoriesResponseTypeDef,
     FacetAttributeDefinitionOutputTypeDef,
     TypedLinkAttributeDefinitionOutputTypeDef,
-    FacetAttributeDefinitionTypeDef,
-    TypedLinkAttributeDefinitionTypeDef,
     GetFacetResponseTypeDef,
     ListAppliedSchemaArnsRequestListAppliedSchemaArnsPaginateTypeDef,
     ListAttachedIndicesRequestListAttachedIndicesPaginateTypeDef,
     ListDevelopmentSchemaArnsRequestListDevelopmentSchemaArnsPaginateTypeDef,
     ListDirectoriesRequestListDirectoriesPaginateTypeDef,
     ListFacetAttributesRequestListFacetAttributesPaginateTypeDef,
     ListFacetNamesRequestListFacetNamesPaginateTypeDef,
@@ -583,86 +577,98 @@
     ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef,
     ListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef,
     LookupPolicyRequestLookupPolicyPaginateTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     PolicyToPathTypeDef,
+    TypedAttributeValueTypeDef,
     BatchGetLinkAttributesResponseTypeDef,
     BatchGetObjectAttributesResponseTypeDef,
     BatchListObjectAttributesResponseTypeDef,
     GetLinkAttributesResponseTypeDef,
     GetObjectAttributesResponseTypeDef,
     IndexAttachmentTypeDef,
     ListObjectAttributesResponseTypeDef,
     TypedLinkSpecifierOutputTypeDef,
-    AddFacetToObjectRequestRequestTypeDef,
-    BatchAddFacetToObjectTypeDef,
-    BatchCreateObjectTypeDef,
-    CreateObjectRequestRequestTypeDef,
-    AttachTypedLinkRequestRequestTypeDef,
-    BatchAttachTypedLinkTypeDef,
-    TypedLinkSpecifierTypeDef,
-    LinkAttributeUpdateTypeDef,
-    ObjectAttributeUpdateTypeDef,
-    ObjectAttributeRangeTypeDef,
-    TypedLinkAttributeRangeTypeDef,
     FacetAttributeOutputTypeDef,
     ListTypedLinkFacetAttributesResponseTypeDef,
-    FacetAttributeTypeDef,
-    TypedLinkFacetAttributeUpdateTypeDef,
-    TypedLinkFacetTypeDef,
     BatchLookupPolicyResponseTypeDef,
     LookupPolicyResponseTypeDef,
+    AttributeKeyAndValueTypeDef,
+    AttributeNameAndValueTypeDef,
+    FacetAttributeDefinitionTypeDef,
+    LinkAttributeActionTypeDef,
+    ObjectAttributeActionTypeDef,
+    TypedAttributeValueRangeTypeDef,
+    TypedLinkAttributeDefinitionTypeDef,
     BatchListAttachedIndicesResponseTypeDef,
     BatchListIndexResponseTypeDef,
     ListAttachedIndicesResponseTypeDef,
     ListIndexResponseTypeDef,
     AttachTypedLinkResponseTypeDef,
     BatchAttachTypedLinkResponseTypeDef,
     BatchListIncomingTypedLinksResponseTypeDef,
     BatchListOutgoingTypedLinksResponseTypeDef,
     ListIncomingTypedLinksResponseTypeDef,
     ListOutgoingTypedLinksResponseTypeDef,
+    ListFacetAttributesResponseTypeDef,
+    AttributeKeyAndValueUnionTypeDef,
+    BatchAddFacetToObjectTypeDef,
+    BatchCreateObjectTypeDef,
+    AttributeNameAndValueUnionTypeDef,
+    BatchAttachTypedLinkTypeDef,
+    TypedLinkSpecifierTypeDef,
+    FacetAttributeTypeDef,
+    LinkAttributeUpdateTypeDef,
+    ObjectAttributeUpdateTypeDef,
+    ObjectAttributeRangeTypeDef,
+    TypedLinkAttributeRangeTypeDef,
+    TypedLinkFacetAttributeUpdateTypeDef,
+    TypedLinkFacetTypeDef,
+    BatchWriteOperationResponseTypeDef,
+    BatchReadSuccessfulResponseTypeDef,
+    AddFacetToObjectRequestRequestTypeDef,
+    CreateObjectRequestRequestTypeDef,
+    AttachTypedLinkRequestRequestTypeDef,
     BatchDetachTypedLinkTypeDef,
     BatchGetLinkAttributesTypeDef,
     DetachTypedLinkRequestRequestTypeDef,
     GetLinkAttributesRequestRequestTypeDef,
+    TypedLinkSpecifierUnionTypeDef,
+    FacetAttributeUnionTypeDef,
+    FacetAttributeUpdateTypeDef,
     BatchUpdateLinkAttributesTypeDef,
     UpdateLinkAttributesRequestRequestTypeDef,
     BatchUpdateObjectAttributesTypeDef,
     UpdateObjectAttributesRequestRequestTypeDef,
     BatchListIndexTypeDef,
     ListIndexRequestListIndexPaginateTypeDef,
     ListIndexRequestRequestTypeDef,
     BatchListIncomingTypedLinksTypeDef,
     BatchListOutgoingTypedLinksTypeDef,
     ListIncomingTypedLinksRequestListIncomingTypedLinksPaginateTypeDef,
     ListIncomingTypedLinksRequestRequestTypeDef,
     ListOutgoingTypedLinksRequestListOutgoingTypedLinksPaginateTypeDef,
     ListOutgoingTypedLinksRequestRequestTypeDef,
-    ListFacetAttributesResponseTypeDef,
-    CreateFacetRequestRequestTypeDef,
-    FacetAttributeUpdateTypeDef,
     UpdateTypedLinkFacetRequestRequestTypeDef,
     CreateTypedLinkFacetRequestRequestTypeDef,
-    BatchWriteOperationResponseTypeDef,
-    BatchReadSuccessfulResponseTypeDef,
-    BatchWriteOperationTypeDef,
-    BatchReadOperationTypeDef,
-    UpdateFacetRequestRequestTypeDef,
     BatchWriteResponseTypeDef,
     BatchReadOperationResponseTypeDef,
+    CreateFacetRequestRequestTypeDef,
+    UpdateFacetRequestRequestTypeDef,
+    BatchWriteOperationTypeDef,
+    BatchReadOperationTypeDef,
+    BatchReadResponseTypeDef,
     BatchWriteRequestRequestTypeDef,
     BatchReadRequestRequestTypeDef,
-    BatchReadResponseTypeDef,
 )
 
 
-def get_structure() -> ObjectReferenceTypeDef:
+def get_value() -> ObjectReferenceTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-clouddirectory-1.28.15.post1/mypy_boto3_clouddirectory.egg-info/SOURCES.txt` & `mypy-boto3-clouddirectory-1.28.16/mypy_boto3_clouddirectory.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-clouddirectory-1.28.15.post1/setup.py` & `mypy-boto3-clouddirectory-1.28.16/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-clouddirectory",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_clouddirectory"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CloudDirectory 1.28.15 service generated with"
-        " mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.CloudDirectory 1.28.16 service generated with"
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
-    keywords="boto3 clouddirectory type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 clouddirectory type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_clouddirectory": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

