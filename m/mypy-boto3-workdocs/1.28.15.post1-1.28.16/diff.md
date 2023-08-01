# Comparing `tmp/mypy-boto3-workdocs-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-workdocs-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-workdocs-1.28.15.post1.tar", last modified: Sat Jul 29 10:04:26 2023, max compression
+gzip compressed data, was "mypy-boto3-workdocs-1.28.16.tar", last modified: Tue Aug  1 11:38:05 2023, max compression
```

## Comparing `mypy-boto3-workdocs-1.28.15.post1.tar` & `mypy-boto3-workdocs-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:26.329459 mypy-boto3-workdocs-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 10:01:40.000000 mypy-boto3-workdocs-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19666 2023-07-29 10:04:26.329459 mypy-boto3-workdocs-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18169 2023-07-29 10:01:40.000000 mypy-boto3-workdocs-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:26.329459 mypy-boto3-workdocs-1.28.15.post1/mypy_boto3_workdocs/
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-07-29 10:01:40.000000 mypy-boto3-workdocs-1.28.15.post1/mypy_boto3_workdocs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-07-29 10:01:40.000000 mypy-boto3-workdocs-1.28.15.post1/mypy_boto3_workdocs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-29 10:01:40.000000 mypy-boto3-workdocs-1.28.15.post1/mypy_boto3_workdocs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38652 2023-07-29 10:01:41.000000 mypy-boto3-workdocs-1.28.15.post1/mypy_boto3_workdocs/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    38591 2023-07-29 10:01:41.000000 mypy-boto3-workdocs-1.28.15.post1/mypy_boto3_workdocs/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13880 2023-07-29 10:01:41.000000 mypy-boto3-workdocs-1.28.15.post1/mypy_boto3_workdocs/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13878 2023-07-29 10:01:41.000000 mypy-boto3-workdocs-1.28.15.post1/mypy_boto3_workdocs/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13859 2023-07-29 10:01:41.000000 mypy-boto3-workdocs-1.28.15.post1/mypy_boto3_workdocs/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13846 2023-07-29 10:01:41.000000 mypy-boto3-workdocs-1.28.15.post1/mypy_boto3_workdocs/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 10:01:40.000000 mypy-boto3-workdocs-1.28.15.post1/mypy_boto3_workdocs/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    50540 2023-07-29 10:01:43.000000 mypy-boto3-workdocs-1.28.15.post1/mypy_boto3_workdocs/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    50449 2023-07-29 10:01:42.000000 mypy-boto3-workdocs-1.28.15.post1/mypy_boto3_workdocs/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 10:01:40.000000 mypy-boto3-workdocs-1.28.15.post1/mypy_boto3_workdocs/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:26.329459 mypy-boto3-workdocs-1.28.15.post1/mypy_boto3_workdocs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19666 2023-07-29 10:04:26.000000 mypy-boto3-workdocs-1.28.15.post1/mypy_boto3_workdocs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-29 10:04:26.000000 mypy-boto3-workdocs-1.28.15.post1/mypy_boto3_workdocs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:26.000000 mypy-boto3-workdocs-1.28.15.post1/mypy_boto3_workdocs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:26.000000 mypy-boto3-workdocs-1.28.15.post1/mypy_boto3_workdocs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:04:26.000000 mypy-boto3-workdocs-1.28.15.post1/mypy_boto3_workdocs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-29 10:04:26.000000 mypy-boto3-workdocs-1.28.15.post1/mypy_boto3_workdocs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:04:26.329459 mypy-boto3-workdocs-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-07-29 10:01:40.000000 mypy-boto3-workdocs-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:38:05.352658 mypy-boto3-workdocs-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:35:21.000000 mypy-boto3-workdocs-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19678 2023-08-01 11:38:05.332658 mypy-boto3-workdocs-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18190 2023-08-01 11:35:21.000000 mypy-boto3-workdocs-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:38:05.328658 mypy-boto3-workdocs-1.28.16/mypy_boto3_workdocs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-08-01 11:35:21.000000 mypy-boto3-workdocs-1.28.16/mypy_boto3_workdocs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-08-01 11:35:21.000000 mypy-boto3-workdocs-1.28.16/mypy_boto3_workdocs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-08-01 11:35:21.000000 mypy-boto3-workdocs-1.28.16/mypy_boto3_workdocs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38621 2023-08-01 11:35:21.000000 mypy-boto3-workdocs-1.28.16/mypy_boto3_workdocs/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38560 2023-08-01 11:35:21.000000 mypy-boto3-workdocs-1.28.16/mypy_boto3_workdocs/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13880 2023-08-01 11:35:22.000000 mypy-boto3-workdocs-1.28.16/mypy_boto3_workdocs/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13878 2023-08-01 11:35:22.000000 mypy-boto3-workdocs-1.28.16/mypy_boto3_workdocs/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13836 2023-08-01 11:35:22.000000 mypy-boto3-workdocs-1.28.16/mypy_boto3_workdocs/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13823 2023-08-01 11:35:22.000000 mypy-boto3-workdocs-1.28.16/mypy_boto3_workdocs/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:35:21.000000 mypy-boto3-workdocs-1.28.16/mypy_boto3_workdocs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    50570 2023-08-01 11:35:23.000000 mypy-boto3-workdocs-1.28.16/mypy_boto3_workdocs/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50479 2023-08-01 11:35:23.000000 mypy-boto3-workdocs-1.28.16/mypy_boto3_workdocs/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:35:21.000000 mypy-boto3-workdocs-1.28.16/mypy_boto3_workdocs/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:38:05.332658 mypy-boto3-workdocs-1.28.16/mypy_boto3_workdocs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19678 2023-08-01 11:38:05.000000 mypy-boto3-workdocs-1.28.16/mypy_boto3_workdocs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-08-01 11:38:05.000000 mypy-boto3-workdocs-1.28.16/mypy_boto3_workdocs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:38:05.000000 mypy-boto3-workdocs-1.28.16/mypy_boto3_workdocs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:38:05.000000 mypy-boto3-workdocs-1.28.16/mypy_boto3_workdocs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:38:05.000000 mypy-boto3-workdocs-1.28.16/mypy_boto3_workdocs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-01 11:38:05.000000 mypy-boto3-workdocs-1.28.16/mypy_boto3_workdocs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:38:05.352658 mypy-boto3-workdocs-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-08-01 11:35:21.000000 mypy-boto3-workdocs-1.28.16/setup.py
```

### Comparing `mypy-boto3-workdocs-1.28.15.post1/LICENSE` & `mypy-boto3-workdocs-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workdocs-1.28.15.post1/PKG-INFO` & `mypy-boto3-workdocs-1.28.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-workdocs
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.WorkDocs 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.WorkDocs 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workdocs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 workdocs type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 workdocs type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-workdocs.svg?color=blue)](https://pypi.org/project/mypy-boto3-workdocs)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workdocs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-workdocs)](https://pepy.tech/project/mypy-boto3-workdocs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WorkDocs 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs)
+[boto3.WorkDocs 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs)
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
 [mypy-boto3-workdocs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workdocs/).
 
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
@@ -386,20 +386,20 @@
 )
 
 
 def check_value(value: ActivityTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_workdocs.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_workdocs.type_defs import (
     AbortDocumentVersionUploadRequestRequestTypeDef,
     ActivateUserRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     UserMetadataTypeDef,
@@ -410,27 +410,26 @@
     CreateCustomMetadataRequestRequestTypeDef,
     CreateFolderRequestRequestTypeDef,
     FolderMetadataTypeDef,
     CreateLabelsRequestRequestTypeDef,
     CreateNotificationSubscriptionRequestRequestTypeDef,
     SubscriptionTypeDef,
     StorageRuleTypeTypeDef,
-    DateRangeTypeTypeDef,
+    TimestampTypeDef,
     DeactivateUserRequestRequestTypeDef,
     DeleteCommentRequestRequestTypeDef,
     DeleteCustomMetadataRequestRequestTypeDef,
     DeleteDocumentRequestRequestTypeDef,
     DeleteDocumentVersionRequestRequestTypeDef,
     DeleteFolderContentsRequestRequestTypeDef,
     DeleteFolderRequestRequestTypeDef,
     DeleteLabelsRequestRequestTypeDef,
     DeleteNotificationSubscriptionRequestRequestTypeDef,
     DeleteUserRequestRequestTypeDef,
     PaginatorConfigTypeDef,
-    DescribeActivitiesRequestRequestTypeDef,
     DescribeCommentsRequestRequestTypeDef,
     DescribeDocumentVersionsRequestRequestTypeDef,
     DocumentVersionMetadataTypeDef,
     DescribeFolderContentsRequestRequestTypeDef,
     DescribeGroupsRequestRequestTypeDef,
     GroupMetadataTypeDef,
     DescribeNotificationSubscriptionsRequestRequestTypeDef,
@@ -442,15 +441,14 @@
     GetCurrentUserRequestRequestTypeDef,
     GetDocumentPathRequestRequestTypeDef,
     GetDocumentRequestRequestTypeDef,
     GetDocumentVersionRequestRequestTypeDef,
     GetFolderPathRequestRequestTypeDef,
     GetFolderRequestRequestTypeDef,
     GetResourcesRequestRequestTypeDef,
-    InitiateDocumentVersionUploadRequestRequestTypeDef,
     UploadMetadataTypeDef,
     PermissionInfoTypeDef,
     RemoveAllResourcePermissionsRequestRequestTypeDef,
     RemoveResourcePermissionRequestRequestTypeDef,
     ResourcePathComponentTypeDef,
     RestoreDocumentVersionsRequestRequestTypeDef,
     SearchSortResultTypeDef,
@@ -465,58 +463,61 @@
     DescribeRootFoldersResponseTypeDef,
     GetFolderResponseTypeDef,
     CreateNotificationSubscriptionResponseTypeDef,
     DescribeNotificationSubscriptionsResponseTypeDef,
     CreateUserRequestRequestTypeDef,
     UpdateUserRequestRequestTypeDef,
     UserStorageMetadataTypeDef,
+    DateRangeTypeTypeDef,
+    DescribeActivitiesRequestRequestTypeDef,
+    InitiateDocumentVersionUploadRequestRequestTypeDef,
     DescribeActivitiesRequestDescribeActivitiesPaginateTypeDef,
     DescribeCommentsRequestDescribeCommentsPaginateTypeDef,
     DescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef,
     DescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef,
     DescribeGroupsRequestDescribeGroupsPaginateTypeDef,
     DescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef,
     DescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef,
     DescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef,
     DescribeUsersRequestDescribeUsersPaginateTypeDef,
     DescribeDocumentVersionsResponseTypeDef,
     DocumentMetadataTypeDef,
     GetDocumentVersionResponseTypeDef,
     DescribeGroupsResponseTypeDef,
     ParticipantsTypeDef,
-    FiltersTypeDef,
     PrincipalTypeDef,
     ResourcePathTypeDef,
     UserTypeDef,
+    FiltersTypeDef,
     DescribeFolderContentsResponseTypeDef,
     GetDocumentResponseTypeDef,
     GetResourcesResponseTypeDef,
     InitiateDocumentVersionUploadResponseTypeDef,
-    SearchResourcesRequestRequestTypeDef,
-    SearchResourcesRequestSearchResourcesPaginateTypeDef,
     DescribeResourcePermissionsResponseTypeDef,
     GetDocumentPathResponseTypeDef,
     GetFolderPathResponseTypeDef,
     ActivateUserResponseTypeDef,
     CommentMetadataTypeDef,
     CommentTypeDef,
     CreateUserResponseTypeDef,
     DescribeUsersResponseTypeDef,
     GetCurrentUserResponseTypeDef,
     UpdateUserResponseTypeDef,
+    SearchResourcesRequestRequestTypeDef,
+    SearchResourcesRequestSearchResourcesPaginateTypeDef,
     ActivityTypeDef,
     ResponseItemTypeDef,
     CreateCommentResponseTypeDef,
     DescribeCommentsResponseTypeDef,
     DescribeActivitiesResponseTypeDef,
     SearchResourcesResponseTypeDef,
 )
 
 
-def get_structure() -> AbortDocumentVersionUploadRequestRequestTypeDef:
+def get_value() -> AbortDocumentVersionUploadRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-workdocs-1.28.15.post1/README.md` & `mypy-boto3-workdocs-1.28.16/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-workdocs.svg?color=blue)](https://pypi.org/project/mypy-boto3-workdocs)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workdocs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-workdocs)](https://pepy.tech/project/mypy-boto3-workdocs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WorkDocs 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs)
+[boto3.WorkDocs 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs)
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
 [mypy-boto3-workdocs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workdocs/).
 
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
@@ -354,20 +354,20 @@
 )
 
 
 def check_value(value: ActivityTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_workdocs.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_workdocs.type_defs import (
     AbortDocumentVersionUploadRequestRequestTypeDef,
     ActivateUserRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     UserMetadataTypeDef,
@@ -378,27 +378,26 @@
     CreateCustomMetadataRequestRequestTypeDef,
     CreateFolderRequestRequestTypeDef,
     FolderMetadataTypeDef,
     CreateLabelsRequestRequestTypeDef,
     CreateNotificationSubscriptionRequestRequestTypeDef,
     SubscriptionTypeDef,
     StorageRuleTypeTypeDef,
-    DateRangeTypeTypeDef,
+    TimestampTypeDef,
     DeactivateUserRequestRequestTypeDef,
     DeleteCommentRequestRequestTypeDef,
     DeleteCustomMetadataRequestRequestTypeDef,
     DeleteDocumentRequestRequestTypeDef,
     DeleteDocumentVersionRequestRequestTypeDef,
     DeleteFolderContentsRequestRequestTypeDef,
     DeleteFolderRequestRequestTypeDef,
     DeleteLabelsRequestRequestTypeDef,
     DeleteNotificationSubscriptionRequestRequestTypeDef,
     DeleteUserRequestRequestTypeDef,
     PaginatorConfigTypeDef,
-    DescribeActivitiesRequestRequestTypeDef,
     DescribeCommentsRequestRequestTypeDef,
     DescribeDocumentVersionsRequestRequestTypeDef,
     DocumentVersionMetadataTypeDef,
     DescribeFolderContentsRequestRequestTypeDef,
     DescribeGroupsRequestRequestTypeDef,
     GroupMetadataTypeDef,
     DescribeNotificationSubscriptionsRequestRequestTypeDef,
@@ -410,15 +409,14 @@
     GetCurrentUserRequestRequestTypeDef,
     GetDocumentPathRequestRequestTypeDef,
     GetDocumentRequestRequestTypeDef,
     GetDocumentVersionRequestRequestTypeDef,
     GetFolderPathRequestRequestTypeDef,
     GetFolderRequestRequestTypeDef,
     GetResourcesRequestRequestTypeDef,
-    InitiateDocumentVersionUploadRequestRequestTypeDef,
     UploadMetadataTypeDef,
     PermissionInfoTypeDef,
     RemoveAllResourcePermissionsRequestRequestTypeDef,
     RemoveResourcePermissionRequestRequestTypeDef,
     ResourcePathComponentTypeDef,
     RestoreDocumentVersionsRequestRequestTypeDef,
     SearchSortResultTypeDef,
@@ -433,58 +431,61 @@
     DescribeRootFoldersResponseTypeDef,
     GetFolderResponseTypeDef,
     CreateNotificationSubscriptionResponseTypeDef,
     DescribeNotificationSubscriptionsResponseTypeDef,
     CreateUserRequestRequestTypeDef,
     UpdateUserRequestRequestTypeDef,
     UserStorageMetadataTypeDef,
+    DateRangeTypeTypeDef,
+    DescribeActivitiesRequestRequestTypeDef,
+    InitiateDocumentVersionUploadRequestRequestTypeDef,
     DescribeActivitiesRequestDescribeActivitiesPaginateTypeDef,
     DescribeCommentsRequestDescribeCommentsPaginateTypeDef,
     DescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef,
     DescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef,
     DescribeGroupsRequestDescribeGroupsPaginateTypeDef,
     DescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef,
     DescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef,
     DescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef,
     DescribeUsersRequestDescribeUsersPaginateTypeDef,
     DescribeDocumentVersionsResponseTypeDef,
     DocumentMetadataTypeDef,
     GetDocumentVersionResponseTypeDef,
     DescribeGroupsResponseTypeDef,
     ParticipantsTypeDef,
-    FiltersTypeDef,
     PrincipalTypeDef,
     ResourcePathTypeDef,
     UserTypeDef,
+    FiltersTypeDef,
     DescribeFolderContentsResponseTypeDef,
     GetDocumentResponseTypeDef,
     GetResourcesResponseTypeDef,
     InitiateDocumentVersionUploadResponseTypeDef,
-    SearchResourcesRequestRequestTypeDef,
-    SearchResourcesRequestSearchResourcesPaginateTypeDef,
     DescribeResourcePermissionsResponseTypeDef,
     GetDocumentPathResponseTypeDef,
     GetFolderPathResponseTypeDef,
     ActivateUserResponseTypeDef,
     CommentMetadataTypeDef,
     CommentTypeDef,
     CreateUserResponseTypeDef,
     DescribeUsersResponseTypeDef,
     GetCurrentUserResponseTypeDef,
     UpdateUserResponseTypeDef,
+    SearchResourcesRequestRequestTypeDef,
+    SearchResourcesRequestSearchResourcesPaginateTypeDef,
     ActivityTypeDef,
     ResponseItemTypeDef,
     CreateCommentResponseTypeDef,
     DescribeCommentsResponseTypeDef,
     DescribeActivitiesResponseTypeDef,
     SearchResourcesResponseTypeDef,
 )
 
 
-def get_structure() -> AbortDocumentVersionUploadRequestRequestTypeDef:
+def get_value() -> AbortDocumentVersionUploadRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-workdocs-1.28.15.post1/mypy_boto3_workdocs/__init__.py` & `mypy-boto3-workdocs-1.28.16/mypy_boto3_workdocs/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workdocs-1.28.15.post1/mypy_boto3_workdocs/__init__.pyi` & `mypy-boto3-workdocs-1.28.16/mypy_boto3_workdocs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workdocs-1.28.15.post1/mypy_boto3_workdocs/__main__.py` & `mypy-boto3-workdocs-1.28.16/mypy_boto3_workdocs/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.WorkDocs 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.WorkDocs 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workdocs//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs\nOther"
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

### Comparing `mypy-boto3-workdocs-1.28.15.post1/mypy_boto3_workdocs/client.py` & `mypy-boto3-workdocs-1.28.16/mypy_boto3_workdocs/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from mypy_boto3_workdocs.client import WorkDocsClient
 
     session = Session()
     client: WorkDocsClient = session.client("workdocs")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     BooleanEnumTypeType,
     CommentVisibilityTypeType,
     FolderContentTypeType,
@@ -73,14 +72,15 @@
     GetResourcesResponseTypeDef,
     InitiateDocumentVersionUploadResponseTypeDef,
     NotificationOptionsTypeDef,
     SearchResourcesResponseTypeDef,
     SearchSortResultTypeDef,
     SharePrincipalTypeDef,
     StorageRuleTypeTypeDef,
+    TimestampTypeDef,
     UpdateUserResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -404,16 +404,16 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workdocs/client/#delete_user)
         """
 
     def describe_activities(
         self,
         *,
         AuthenticationToken: str = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         OrganizationId: str = ...,
         ActivityTypes: str = ...,
         ResourceId: str = ...,
         UserId: str = ...,
         IncludeIndirectActivities: bool = ...,
         Limit: int = ...,
         Marker: str = ...
@@ -663,16 +663,16 @@
 
     def initiate_document_version_upload(
         self,
         *,
         AuthenticationToken: str = ...,
         Id: str = ...,
         Name: str = ...,
-        ContentCreatedTimestamp: Union[datetime, str] = ...,
-        ContentModifiedTimestamp: Union[datetime, str] = ...,
+        ContentCreatedTimestamp: TimestampTypeDef = ...,
+        ContentModifiedTimestamp: TimestampTypeDef = ...,
         ContentType: str = ...,
         DocumentSizeInBytes: int = ...,
         ParentFolderId: str = ...
     ) -> InitiateDocumentVersionUploadResponseTypeDef:
         """
         Creates a new document object and version object.
```

### Comparing `mypy-boto3-workdocs-1.28.15.post1/mypy_boto3_workdocs/client.pyi` & `mypy-boto3-workdocs-1.28.16/mypy_boto3_workdocs/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from mypy_boto3_workdocs.client import WorkDocsClient
 
     session = Session()
     client: WorkDocsClient = session.client("workdocs")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     BooleanEnumTypeType,
     CommentVisibilityTypeType,
     FolderContentTypeType,
@@ -73,14 +72,15 @@
     GetResourcesResponseTypeDef,
     InitiateDocumentVersionUploadResponseTypeDef,
     NotificationOptionsTypeDef,
     SearchResourcesResponseTypeDef,
     SearchSortResultTypeDef,
     SharePrincipalTypeDef,
     StorageRuleTypeTypeDef,
+    TimestampTypeDef,
     UpdateUserResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -378,16 +378,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Client.delete_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workdocs/client/#delete_user)
         """
     def describe_activities(
         self,
         *,
         AuthenticationToken: str = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         OrganizationId: str = ...,
         ActivityTypes: str = ...,
         ResourceId: str = ...,
         UserId: str = ...,
         IncludeIndirectActivities: bool = ...,
         Limit: int = ...,
         Marker: str = ...
@@ -620,16 +620,16 @@
         """
     def initiate_document_version_upload(
         self,
         *,
         AuthenticationToken: str = ...,
         Id: str = ...,
         Name: str = ...,
-        ContentCreatedTimestamp: Union[datetime, str] = ...,
-        ContentModifiedTimestamp: Union[datetime, str] = ...,
+        ContentCreatedTimestamp: TimestampTypeDef = ...,
+        ContentModifiedTimestamp: TimestampTypeDef = ...,
         ContentType: str = ...,
         DocumentSizeInBytes: int = ...,
         ParentFolderId: str = ...
     ) -> InitiateDocumentVersionUploadResponseTypeDef:
         """
         Creates a new document object and version object.
```

### Comparing `mypy-boto3-workdocs-1.28.15.post1/mypy_boto3_workdocs/literals.py` & `mypy-boto3-workdocs-1.28.16/mypy_boto3_workdocs/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workdocs-1.28.15.post1/mypy_boto3_workdocs/literals.pyi` & `mypy-boto3-workdocs-1.28.16/mypy_boto3_workdocs/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workdocs-1.28.15.post1/mypy_boto3_workdocs/paginator.py` & `mypy-boto3-workdocs-1.28.16/mypy_boto3_workdocs/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,16 +34,15 @@
     describe_resource_permissions_paginator: DescribeResourcePermissionsPaginator = client.get_paginator("describe_resource_permissions")
     describe_root_folders_paginator: DescribeRootFoldersPaginator = client.get_paginator("describe_root_folders")
     describe_users_paginator: DescribeUsersPaginator = client.get_paginator("describe_users")
     search_resources_paginator: SearchResourcesPaginator = client.get_paginator("search_resources")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Generic, Iterator, Sequence, TypeVar, Union
+from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import (
     FolderContentTypeType,
     OrderTypeType,
     ResourceSortTypeType,
@@ -61,14 +60,15 @@
     DescribeResourcePermissionsResponseTypeDef,
     DescribeRootFoldersResponseTypeDef,
     DescribeUsersResponseTypeDef,
     FiltersTypeDef,
     PaginatorConfigTypeDef,
     SearchResourcesResponseTypeDef,
     SearchSortResultTypeDef,
+    TimestampTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -103,16 +103,16 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workdocs/paginators/#describeactivitiespaginator)
     """
 
     def paginate(
         self,
         *,
         AuthenticationToken: str = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         OrganizationId: str = ...,
         ActivityTypes: str = ...,
         ResourceId: str = ...,
         UserId: str = ...,
         IncludeIndirectActivities: bool = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeActivitiesResponseTypeDef]:
```

### Comparing `mypy-boto3-workdocs-1.28.15.post1/mypy_boto3_workdocs/paginator.pyi` & `mypy-boto3-workdocs-1.28.16/mypy_boto3_workdocs/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -34,16 +34,15 @@
     describe_resource_permissions_paginator: DescribeResourcePermissionsPaginator = client.get_paginator("describe_resource_permissions")
     describe_root_folders_paginator: DescribeRootFoldersPaginator = client.get_paginator("describe_root_folders")
     describe_users_paginator: DescribeUsersPaginator = client.get_paginator("describe_users")
     search_resources_paginator: SearchResourcesPaginator = client.get_paginator("search_resources")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Generic, Iterator, Sequence, TypeVar, Union
+from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import (
     FolderContentTypeType,
     OrderTypeType,
     ResourceSortTypeType,
@@ -61,14 +60,15 @@
     DescribeResourcePermissionsResponseTypeDef,
     DescribeRootFoldersResponseTypeDef,
     DescribeUsersResponseTypeDef,
     FiltersTypeDef,
     PaginatorConfigTypeDef,
     SearchResourcesResponseTypeDef,
     SearchSortResultTypeDef,
+    TimestampTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -99,16 +99,16 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workdocs/paginators/#describeactivitiespaginator)
     """
 
     def paginate(
         self,
         *,
         AuthenticationToken: str = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         OrganizationId: str = ...,
         ActivityTypes: str = ...,
         ResourceId: str = ...,
         UserId: str = ...,
         IncludeIndirectActivities: bool = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeActivitiesResponseTypeDef]:
```

### Comparing `mypy-boto3-workdocs-1.28.15.post1/mypy_boto3_workdocs/type_defs.py` & `mypy-boto3-workdocs-1.28.16/mypy_boto3_workdocs/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workdocs/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_workdocs.type_defs import AbortDocumentVersionUploadRequestRequestTypeDef
 
-    data: AbortDocumentVersionUploadRequestRequestTypeDef = {...}
+    data: AbortDocumentVersionUploadRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -72,27 +72,26 @@
     "CreateCustomMetadataRequestRequestTypeDef",
     "CreateFolderRequestRequestTypeDef",
     "FolderMetadataTypeDef",
     "CreateLabelsRequestRequestTypeDef",
     "CreateNotificationSubscriptionRequestRequestTypeDef",
     "SubscriptionTypeDef",
     "StorageRuleTypeTypeDef",
-    "DateRangeTypeTypeDef",
+    "TimestampTypeDef",
     "DeactivateUserRequestRequestTypeDef",
     "DeleteCommentRequestRequestTypeDef",
     "DeleteCustomMetadataRequestRequestTypeDef",
     "DeleteDocumentRequestRequestTypeDef",
     "DeleteDocumentVersionRequestRequestTypeDef",
     "DeleteFolderContentsRequestRequestTypeDef",
     "DeleteFolderRequestRequestTypeDef",
     "DeleteLabelsRequestRequestTypeDef",
     "DeleteNotificationSubscriptionRequestRequestTypeDef",
     "DeleteUserRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
-    "DescribeActivitiesRequestRequestTypeDef",
     "DescribeCommentsRequestRequestTypeDef",
     "DescribeDocumentVersionsRequestRequestTypeDef",
     "DocumentVersionMetadataTypeDef",
     "DescribeFolderContentsRequestRequestTypeDef",
     "DescribeGroupsRequestRequestTypeDef",
     "GroupMetadataTypeDef",
     "DescribeNotificationSubscriptionsRequestRequestTypeDef",
@@ -104,15 +103,14 @@
     "GetCurrentUserRequestRequestTypeDef",
     "GetDocumentPathRequestRequestTypeDef",
     "GetDocumentRequestRequestTypeDef",
     "GetDocumentVersionRequestRequestTypeDef",
     "GetFolderPathRequestRequestTypeDef",
     "GetFolderRequestRequestTypeDef",
     "GetResourcesRequestRequestTypeDef",
-    "InitiateDocumentVersionUploadRequestRequestTypeDef",
     "UploadMetadataTypeDef",
     "PermissionInfoTypeDef",
     "RemoveAllResourcePermissionsRequestRequestTypeDef",
     "RemoveResourcePermissionRequestRequestTypeDef",
     "ResourcePathComponentTypeDef",
     "RestoreDocumentVersionsRequestRequestTypeDef",
     "SearchSortResultTypeDef",
@@ -127,48 +125,51 @@
     "DescribeRootFoldersResponseTypeDef",
     "GetFolderResponseTypeDef",
     "CreateNotificationSubscriptionResponseTypeDef",
     "DescribeNotificationSubscriptionsResponseTypeDef",
     "CreateUserRequestRequestTypeDef",
     "UpdateUserRequestRequestTypeDef",
     "UserStorageMetadataTypeDef",
+    "DateRangeTypeTypeDef",
+    "DescribeActivitiesRequestRequestTypeDef",
+    "InitiateDocumentVersionUploadRequestRequestTypeDef",
     "DescribeActivitiesRequestDescribeActivitiesPaginateTypeDef",
     "DescribeCommentsRequestDescribeCommentsPaginateTypeDef",
     "DescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef",
     "DescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef",
     "DescribeGroupsRequestDescribeGroupsPaginateTypeDef",
     "DescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef",
     "DescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef",
     "DescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef",
     "DescribeUsersRequestDescribeUsersPaginateTypeDef",
     "DescribeDocumentVersionsResponseTypeDef",
     "DocumentMetadataTypeDef",
     "GetDocumentVersionResponseTypeDef",
     "DescribeGroupsResponseTypeDef",
     "ParticipantsTypeDef",
-    "FiltersTypeDef",
     "PrincipalTypeDef",
     "ResourcePathTypeDef",
     "UserTypeDef",
+    "FiltersTypeDef",
     "DescribeFolderContentsResponseTypeDef",
     "GetDocumentResponseTypeDef",
     "GetResourcesResponseTypeDef",
     "InitiateDocumentVersionUploadResponseTypeDef",
-    "SearchResourcesRequestRequestTypeDef",
-    "SearchResourcesRequestSearchResourcesPaginateTypeDef",
     "DescribeResourcePermissionsResponseTypeDef",
     "GetDocumentPathResponseTypeDef",
     "GetFolderPathResponseTypeDef",
     "ActivateUserResponseTypeDef",
     "CommentMetadataTypeDef",
     "CommentTypeDef",
     "CreateUserResponseTypeDef",
     "DescribeUsersResponseTypeDef",
     "GetCurrentUserResponseTypeDef",
     "UpdateUserResponseTypeDef",
+    "SearchResourcesRequestRequestTypeDef",
+    "SearchResourcesRequestSearchResourcesPaginateTypeDef",
     "ActivityTypeDef",
     "ResponseItemTypeDef",
     "CreateCommentResponseTypeDef",
     "DescribeCommentsResponseTypeDef",
     "DescribeActivitiesResponseTypeDef",
     "SearchResourcesResponseTypeDef",
 )
@@ -409,23 +410,15 @@
     {
         "StorageAllocatedInBytes": int,
         "StorageType": StorageTypeType,
     },
     total=False,
 )
 
-DateRangeTypeTypeDef = TypedDict(
-    "DateRangeTypeTypeDef",
-    {
-        "StartValue": Union[datetime, str],
-        "EndValue": Union[datetime, str],
-    },
-    total=False,
-)
-
+TimestampTypeDef = Union[datetime, str]
 _RequiredDeactivateUserRequestRequestTypeDef = TypedDict(
     "_RequiredDeactivateUserRequestRequestTypeDef",
     {
         "UserId": str,
     },
 )
 _OptionalDeactivateUserRequestRequestTypeDef = TypedDict(
@@ -637,31 +630,14 @@
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
-DescribeActivitiesRequestRequestTypeDef = TypedDict(
-    "DescribeActivitiesRequestRequestTypeDef",
-    {
-        "AuthenticationToken": str,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "OrganizationId": str,
-        "ActivityTypes": str,
-        "ResourceId": str,
-        "UserId": str,
-        "IncludeIndirectActivities": bool,
-        "Limit": int,
-        "Marker": str,
-    },
-    total=False,
-)
-
 _RequiredDescribeCommentsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeCommentsRequestRequestTypeDef",
     {
         "DocumentId": str,
         "VersionId": str,
     },
 )
@@ -1039,29 +1015,14 @@
         "CollectionType": Literal["SHARED_WITH_ME"],
         "Limit": int,
         "Marker": str,
     },
     total=False,
 )
 
-InitiateDocumentVersionUploadRequestRequestTypeDef = TypedDict(
-    "InitiateDocumentVersionUploadRequestRequestTypeDef",
-    {
-        "AuthenticationToken": str,
-        "Id": str,
-        "Name": str,
-        "ContentCreatedTimestamp": Union[datetime, str],
-        "ContentModifiedTimestamp": Union[datetime, str],
-        "ContentType": str,
-        "DocumentSizeInBytes": int,
-        "ParentFolderId": str,
-    },
-    total=False,
-)
-
 UploadMetadataTypeDef = TypedDict(
     "UploadMetadataTypeDef",
     {
         "UploadUrl": str,
         "SignedHeaders": Dict[str, str],
     },
     total=False,
@@ -1391,20 +1352,61 @@
     {
         "StorageUtilizedInBytes": int,
         "StorageRule": StorageRuleTypeTypeDef,
     },
     total=False,
 )
 
+DateRangeTypeTypeDef = TypedDict(
+    "DateRangeTypeTypeDef",
+    {
+        "StartValue": TimestampTypeDef,
+        "EndValue": TimestampTypeDef,
+    },
+    total=False,
+)
+
+DescribeActivitiesRequestRequestTypeDef = TypedDict(
+    "DescribeActivitiesRequestRequestTypeDef",
+    {
+        "AuthenticationToken": str,
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "OrganizationId": str,
+        "ActivityTypes": str,
+        "ResourceId": str,
+        "UserId": str,
+        "IncludeIndirectActivities": bool,
+        "Limit": int,
+        "Marker": str,
+    },
+    total=False,
+)
+
+InitiateDocumentVersionUploadRequestRequestTypeDef = TypedDict(
+    "InitiateDocumentVersionUploadRequestRequestTypeDef",
+    {
+        "AuthenticationToken": str,
+        "Id": str,
+        "Name": str,
+        "ContentCreatedTimestamp": TimestampTypeDef,
+        "ContentModifiedTimestamp": TimestampTypeDef,
+        "ContentType": str,
+        "DocumentSizeInBytes": int,
+        "ParentFolderId": str,
+    },
+    total=False,
+)
+
 DescribeActivitiesRequestDescribeActivitiesPaginateTypeDef = TypedDict(
     "DescribeActivitiesRequestDescribeActivitiesPaginateTypeDef",
     {
         "AuthenticationToken": str,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
         "OrganizationId": str,
         "ActivityTypes": str,
         "ResourceId": str,
         "UserId": str,
         "IncludeIndirectActivities": bool,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
@@ -1642,31 +1644,14 @@
     {
         "Users": List[UserMetadataTypeDef],
         "Groups": List[GroupMetadataTypeDef],
     },
     total=False,
 )
 
-FiltersTypeDef = TypedDict(
-    "FiltersTypeDef",
-    {
-        "TextLocales": Sequence[LanguageCodeTypeType],
-        "ContentCategories": Sequence[ContentCategoryTypeType],
-        "ResourceTypes": Sequence[SearchResourceTypeType],
-        "Labels": Sequence[str],
-        "Principals": Sequence[SearchPrincipalTypeTypeDef],
-        "AncestorIds": Sequence[str],
-        "SearchCollectionTypes": Sequence[SearchCollectionTypeType],
-        "SizeRange": LongRangeTypeTypeDef,
-        "CreatedRange": DateRangeTypeTypeDef,
-        "ModifiedRange": DateRangeTypeTypeDef,
-    },
-    total=False,
-)
-
 PrincipalTypeDef = TypedDict(
     "PrincipalTypeDef",
     {
         "Id": str,
         "Type": PrincipalTypeType,
         "Roles": List[PermissionInfoTypeDef],
     },
@@ -1699,14 +1684,31 @@
         "TimeZoneId": str,
         "Locale": LocaleTypeType,
         "Storage": UserStorageMetadataTypeDef,
     },
     total=False,
 )
 
+FiltersTypeDef = TypedDict(
+    "FiltersTypeDef",
+    {
+        "TextLocales": Sequence[LanguageCodeTypeType],
+        "ContentCategories": Sequence[ContentCategoryTypeType],
+        "ResourceTypes": Sequence[SearchResourceTypeType],
+        "Labels": Sequence[str],
+        "Principals": Sequence[SearchPrincipalTypeTypeDef],
+        "AncestorIds": Sequence[str],
+        "SearchCollectionTypes": Sequence[SearchCollectionTypeType],
+        "SizeRange": LongRangeTypeTypeDef,
+        "CreatedRange": DateRangeTypeTypeDef,
+        "ModifiedRange": DateRangeTypeTypeDef,
+    },
+    total=False,
+)
+
 DescribeFolderContentsResponseTypeDef = TypedDict(
     "DescribeFolderContentsResponseTypeDef",
     {
         "Folders": List[FolderMetadataTypeDef],
         "Documents": List[DocumentMetadataTypeDef],
         "Marker": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1737,45 +1739,14 @@
     {
         "Metadata": DocumentMetadataTypeDef,
         "UploadMetadata": UploadMetadataTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-SearchResourcesRequestRequestTypeDef = TypedDict(
-    "SearchResourcesRequestRequestTypeDef",
-    {
-        "AuthenticationToken": str,
-        "QueryText": str,
-        "QueryScopes": Sequence[SearchQueryScopeTypeType],
-        "OrganizationId": str,
-        "AdditionalResponseFields": Sequence[Literal["WEBURL"]],
-        "Filters": FiltersTypeDef,
-        "OrderBy": Sequence[SearchSortResultTypeDef],
-        "Limit": int,
-        "Marker": str,
-    },
-    total=False,
-)
-
-SearchResourcesRequestSearchResourcesPaginateTypeDef = TypedDict(
-    "SearchResourcesRequestSearchResourcesPaginateTypeDef",
-    {
-        "AuthenticationToken": str,
-        "QueryText": str,
-        "QueryScopes": Sequence[SearchQueryScopeTypeType],
-        "OrganizationId": str,
-        "AdditionalResponseFields": Sequence[Literal["WEBURL"]],
-        "Filters": FiltersTypeDef,
-        "OrderBy": Sequence[SearchSortResultTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 DescribeResourcePermissionsResponseTypeDef = TypedDict(
     "DescribeResourcePermissionsResponseTypeDef",
     {
         "Principals": List[PrincipalTypeDef],
         "Marker": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1874,14 +1845,45 @@
     "UpdateUserResponseTypeDef",
     {
         "User": UserTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+SearchResourcesRequestRequestTypeDef = TypedDict(
+    "SearchResourcesRequestRequestTypeDef",
+    {
+        "AuthenticationToken": str,
+        "QueryText": str,
+        "QueryScopes": Sequence[SearchQueryScopeTypeType],
+        "OrganizationId": str,
+        "AdditionalResponseFields": Sequence[Literal["WEBURL"]],
+        "Filters": FiltersTypeDef,
+        "OrderBy": Sequence[SearchSortResultTypeDef],
+        "Limit": int,
+        "Marker": str,
+    },
+    total=False,
+)
+
+SearchResourcesRequestSearchResourcesPaginateTypeDef = TypedDict(
+    "SearchResourcesRequestSearchResourcesPaginateTypeDef",
+    {
+        "AuthenticationToken": str,
+        "QueryText": str,
+        "QueryScopes": Sequence[SearchQueryScopeTypeType],
+        "OrganizationId": str,
+        "AdditionalResponseFields": Sequence[Literal["WEBURL"]],
+        "Filters": FiltersTypeDef,
+        "OrderBy": Sequence[SearchSortResultTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 ActivityTypeDef = TypedDict(
     "ActivityTypeDef",
     {
         "Type": ActivityTypeType,
         "TimeStamp": datetime,
         "IsIndirectActivity": bool,
         "OrganizationId": str,
```

### Comparing `mypy-boto3-workdocs-1.28.15.post1/mypy_boto3_workdocs/type_defs.pyi` & `mypy-boto3-workdocs-1.28.16/mypy_boto3_workdocs/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workdocs/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_workdocs.type_defs import AbortDocumentVersionUploadRequestRequestTypeDef
 
-    data: AbortDocumentVersionUploadRequestRequestTypeDef = {...}
+    data: AbortDocumentVersionUploadRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -71,27 +71,26 @@
     "CreateCustomMetadataRequestRequestTypeDef",
     "CreateFolderRequestRequestTypeDef",
     "FolderMetadataTypeDef",
     "CreateLabelsRequestRequestTypeDef",
     "CreateNotificationSubscriptionRequestRequestTypeDef",
     "SubscriptionTypeDef",
     "StorageRuleTypeTypeDef",
-    "DateRangeTypeTypeDef",
+    "TimestampTypeDef",
     "DeactivateUserRequestRequestTypeDef",
     "DeleteCommentRequestRequestTypeDef",
     "DeleteCustomMetadataRequestRequestTypeDef",
     "DeleteDocumentRequestRequestTypeDef",
     "DeleteDocumentVersionRequestRequestTypeDef",
     "DeleteFolderContentsRequestRequestTypeDef",
     "DeleteFolderRequestRequestTypeDef",
     "DeleteLabelsRequestRequestTypeDef",
     "DeleteNotificationSubscriptionRequestRequestTypeDef",
     "DeleteUserRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
-    "DescribeActivitiesRequestRequestTypeDef",
     "DescribeCommentsRequestRequestTypeDef",
     "DescribeDocumentVersionsRequestRequestTypeDef",
     "DocumentVersionMetadataTypeDef",
     "DescribeFolderContentsRequestRequestTypeDef",
     "DescribeGroupsRequestRequestTypeDef",
     "GroupMetadataTypeDef",
     "DescribeNotificationSubscriptionsRequestRequestTypeDef",
@@ -103,15 +102,14 @@
     "GetCurrentUserRequestRequestTypeDef",
     "GetDocumentPathRequestRequestTypeDef",
     "GetDocumentRequestRequestTypeDef",
     "GetDocumentVersionRequestRequestTypeDef",
     "GetFolderPathRequestRequestTypeDef",
     "GetFolderRequestRequestTypeDef",
     "GetResourcesRequestRequestTypeDef",
-    "InitiateDocumentVersionUploadRequestRequestTypeDef",
     "UploadMetadataTypeDef",
     "PermissionInfoTypeDef",
     "RemoveAllResourcePermissionsRequestRequestTypeDef",
     "RemoveResourcePermissionRequestRequestTypeDef",
     "ResourcePathComponentTypeDef",
     "RestoreDocumentVersionsRequestRequestTypeDef",
     "SearchSortResultTypeDef",
@@ -126,48 +124,51 @@
     "DescribeRootFoldersResponseTypeDef",
     "GetFolderResponseTypeDef",
     "CreateNotificationSubscriptionResponseTypeDef",
     "DescribeNotificationSubscriptionsResponseTypeDef",
     "CreateUserRequestRequestTypeDef",
     "UpdateUserRequestRequestTypeDef",
     "UserStorageMetadataTypeDef",
+    "DateRangeTypeTypeDef",
+    "DescribeActivitiesRequestRequestTypeDef",
+    "InitiateDocumentVersionUploadRequestRequestTypeDef",
     "DescribeActivitiesRequestDescribeActivitiesPaginateTypeDef",
     "DescribeCommentsRequestDescribeCommentsPaginateTypeDef",
     "DescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef",
     "DescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef",
     "DescribeGroupsRequestDescribeGroupsPaginateTypeDef",
     "DescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef",
     "DescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef",
     "DescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef",
     "DescribeUsersRequestDescribeUsersPaginateTypeDef",
     "DescribeDocumentVersionsResponseTypeDef",
     "DocumentMetadataTypeDef",
     "GetDocumentVersionResponseTypeDef",
     "DescribeGroupsResponseTypeDef",
     "ParticipantsTypeDef",
-    "FiltersTypeDef",
     "PrincipalTypeDef",
     "ResourcePathTypeDef",
     "UserTypeDef",
+    "FiltersTypeDef",
     "DescribeFolderContentsResponseTypeDef",
     "GetDocumentResponseTypeDef",
     "GetResourcesResponseTypeDef",
     "InitiateDocumentVersionUploadResponseTypeDef",
-    "SearchResourcesRequestRequestTypeDef",
-    "SearchResourcesRequestSearchResourcesPaginateTypeDef",
     "DescribeResourcePermissionsResponseTypeDef",
     "GetDocumentPathResponseTypeDef",
     "GetFolderPathResponseTypeDef",
     "ActivateUserResponseTypeDef",
     "CommentMetadataTypeDef",
     "CommentTypeDef",
     "CreateUserResponseTypeDef",
     "DescribeUsersResponseTypeDef",
     "GetCurrentUserResponseTypeDef",
     "UpdateUserResponseTypeDef",
+    "SearchResourcesRequestRequestTypeDef",
+    "SearchResourcesRequestSearchResourcesPaginateTypeDef",
     "ActivityTypeDef",
     "ResponseItemTypeDef",
     "CreateCommentResponseTypeDef",
     "DescribeCommentsResponseTypeDef",
     "DescribeActivitiesResponseTypeDef",
     "SearchResourcesResponseTypeDef",
 )
@@ -396,23 +397,15 @@
     {
         "StorageAllocatedInBytes": int,
         "StorageType": StorageTypeType,
     },
     total=False,
 )
 
-DateRangeTypeTypeDef = TypedDict(
-    "DateRangeTypeTypeDef",
-    {
-        "StartValue": Union[datetime, str],
-        "EndValue": Union[datetime, str],
-    },
-    total=False,
-)
-
+TimestampTypeDef = Union[datetime, str]
 _RequiredDeactivateUserRequestRequestTypeDef = TypedDict(
     "_RequiredDeactivateUserRequestRequestTypeDef",
     {
         "UserId": str,
     },
 )
 _OptionalDeactivateUserRequestRequestTypeDef = TypedDict(
@@ -606,31 +599,14 @@
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
-DescribeActivitiesRequestRequestTypeDef = TypedDict(
-    "DescribeActivitiesRequestRequestTypeDef",
-    {
-        "AuthenticationToken": str,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "OrganizationId": str,
-        "ActivityTypes": str,
-        "ResourceId": str,
-        "UserId": str,
-        "IncludeIndirectActivities": bool,
-        "Limit": int,
-        "Marker": str,
-    },
-    total=False,
-)
-
 _RequiredDescribeCommentsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeCommentsRequestRequestTypeDef",
     {
         "DocumentId": str,
         "VersionId": str,
     },
 )
@@ -982,29 +958,14 @@
         "CollectionType": Literal["SHARED_WITH_ME"],
         "Limit": int,
         "Marker": str,
     },
     total=False,
 )
 
-InitiateDocumentVersionUploadRequestRequestTypeDef = TypedDict(
-    "InitiateDocumentVersionUploadRequestRequestTypeDef",
-    {
-        "AuthenticationToken": str,
-        "Id": str,
-        "Name": str,
-        "ContentCreatedTimestamp": Union[datetime, str],
-        "ContentModifiedTimestamp": Union[datetime, str],
-        "ContentType": str,
-        "DocumentSizeInBytes": int,
-        "ParentFolderId": str,
-    },
-    total=False,
-)
-
 UploadMetadataTypeDef = TypedDict(
     "UploadMetadataTypeDef",
     {
         "UploadUrl": str,
         "SignedHeaders": Dict[str, str],
     },
     total=False,
@@ -1316,20 +1277,61 @@
     {
         "StorageUtilizedInBytes": int,
         "StorageRule": StorageRuleTypeTypeDef,
     },
     total=False,
 )
 
+DateRangeTypeTypeDef = TypedDict(
+    "DateRangeTypeTypeDef",
+    {
+        "StartValue": TimestampTypeDef,
+        "EndValue": TimestampTypeDef,
+    },
+    total=False,
+)
+
+DescribeActivitiesRequestRequestTypeDef = TypedDict(
+    "DescribeActivitiesRequestRequestTypeDef",
+    {
+        "AuthenticationToken": str,
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "OrganizationId": str,
+        "ActivityTypes": str,
+        "ResourceId": str,
+        "UserId": str,
+        "IncludeIndirectActivities": bool,
+        "Limit": int,
+        "Marker": str,
+    },
+    total=False,
+)
+
+InitiateDocumentVersionUploadRequestRequestTypeDef = TypedDict(
+    "InitiateDocumentVersionUploadRequestRequestTypeDef",
+    {
+        "AuthenticationToken": str,
+        "Id": str,
+        "Name": str,
+        "ContentCreatedTimestamp": TimestampTypeDef,
+        "ContentModifiedTimestamp": TimestampTypeDef,
+        "ContentType": str,
+        "DocumentSizeInBytes": int,
+        "ParentFolderId": str,
+    },
+    total=False,
+)
+
 DescribeActivitiesRequestDescribeActivitiesPaginateTypeDef = TypedDict(
     "DescribeActivitiesRequestDescribeActivitiesPaginateTypeDef",
     {
         "AuthenticationToken": str,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
         "OrganizationId": str,
         "ActivityTypes": str,
         "ResourceId": str,
         "UserId": str,
         "IncludeIndirectActivities": bool,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
@@ -1553,31 +1555,14 @@
     {
         "Users": List[UserMetadataTypeDef],
         "Groups": List[GroupMetadataTypeDef],
     },
     total=False,
 )
 
-FiltersTypeDef = TypedDict(
-    "FiltersTypeDef",
-    {
-        "TextLocales": Sequence[LanguageCodeTypeType],
-        "ContentCategories": Sequence[ContentCategoryTypeType],
-        "ResourceTypes": Sequence[SearchResourceTypeType],
-        "Labels": Sequence[str],
-        "Principals": Sequence[SearchPrincipalTypeTypeDef],
-        "AncestorIds": Sequence[str],
-        "SearchCollectionTypes": Sequence[SearchCollectionTypeType],
-        "SizeRange": LongRangeTypeTypeDef,
-        "CreatedRange": DateRangeTypeTypeDef,
-        "ModifiedRange": DateRangeTypeTypeDef,
-    },
-    total=False,
-)
-
 PrincipalTypeDef = TypedDict(
     "PrincipalTypeDef",
     {
         "Id": str,
         "Type": PrincipalTypeType,
         "Roles": List[PermissionInfoTypeDef],
     },
@@ -1610,14 +1595,31 @@
         "TimeZoneId": str,
         "Locale": LocaleTypeType,
         "Storage": UserStorageMetadataTypeDef,
     },
     total=False,
 )
 
+FiltersTypeDef = TypedDict(
+    "FiltersTypeDef",
+    {
+        "TextLocales": Sequence[LanguageCodeTypeType],
+        "ContentCategories": Sequence[ContentCategoryTypeType],
+        "ResourceTypes": Sequence[SearchResourceTypeType],
+        "Labels": Sequence[str],
+        "Principals": Sequence[SearchPrincipalTypeTypeDef],
+        "AncestorIds": Sequence[str],
+        "SearchCollectionTypes": Sequence[SearchCollectionTypeType],
+        "SizeRange": LongRangeTypeTypeDef,
+        "CreatedRange": DateRangeTypeTypeDef,
+        "ModifiedRange": DateRangeTypeTypeDef,
+    },
+    total=False,
+)
+
 DescribeFolderContentsResponseTypeDef = TypedDict(
     "DescribeFolderContentsResponseTypeDef",
     {
         "Folders": List[FolderMetadataTypeDef],
         "Documents": List[DocumentMetadataTypeDef],
         "Marker": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1648,45 +1650,14 @@
     {
         "Metadata": DocumentMetadataTypeDef,
         "UploadMetadata": UploadMetadataTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-SearchResourcesRequestRequestTypeDef = TypedDict(
-    "SearchResourcesRequestRequestTypeDef",
-    {
-        "AuthenticationToken": str,
-        "QueryText": str,
-        "QueryScopes": Sequence[SearchQueryScopeTypeType],
-        "OrganizationId": str,
-        "AdditionalResponseFields": Sequence[Literal["WEBURL"]],
-        "Filters": FiltersTypeDef,
-        "OrderBy": Sequence[SearchSortResultTypeDef],
-        "Limit": int,
-        "Marker": str,
-    },
-    total=False,
-)
-
-SearchResourcesRequestSearchResourcesPaginateTypeDef = TypedDict(
-    "SearchResourcesRequestSearchResourcesPaginateTypeDef",
-    {
-        "AuthenticationToken": str,
-        "QueryText": str,
-        "QueryScopes": Sequence[SearchQueryScopeTypeType],
-        "OrganizationId": str,
-        "AdditionalResponseFields": Sequence[Literal["WEBURL"]],
-        "Filters": FiltersTypeDef,
-        "OrderBy": Sequence[SearchSortResultTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 DescribeResourcePermissionsResponseTypeDef = TypedDict(
     "DescribeResourcePermissionsResponseTypeDef",
     {
         "Principals": List[PrincipalTypeDef],
         "Marker": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1783,14 +1754,45 @@
     "UpdateUserResponseTypeDef",
     {
         "User": UserTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+SearchResourcesRequestRequestTypeDef = TypedDict(
+    "SearchResourcesRequestRequestTypeDef",
+    {
+        "AuthenticationToken": str,
+        "QueryText": str,
+        "QueryScopes": Sequence[SearchQueryScopeTypeType],
+        "OrganizationId": str,
+        "AdditionalResponseFields": Sequence[Literal["WEBURL"]],
+        "Filters": FiltersTypeDef,
+        "OrderBy": Sequence[SearchSortResultTypeDef],
+        "Limit": int,
+        "Marker": str,
+    },
+    total=False,
+)
+
+SearchResourcesRequestSearchResourcesPaginateTypeDef = TypedDict(
+    "SearchResourcesRequestSearchResourcesPaginateTypeDef",
+    {
+        "AuthenticationToken": str,
+        "QueryText": str,
+        "QueryScopes": Sequence[SearchQueryScopeTypeType],
+        "OrganizationId": str,
+        "AdditionalResponseFields": Sequence[Literal["WEBURL"]],
+        "Filters": FiltersTypeDef,
+        "OrderBy": Sequence[SearchSortResultTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 ActivityTypeDef = TypedDict(
     "ActivityTypeDef",
     {
         "Type": ActivityTypeType,
         "TimeStamp": datetime,
         "IsIndirectActivity": bool,
         "OrganizationId": str,
```

### Comparing `mypy-boto3-workdocs-1.28.15.post1/mypy_boto3_workdocs.egg-info/PKG-INFO` & `mypy-boto3-workdocs-1.28.16/mypy_boto3_workdocs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-workdocs
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.WorkDocs 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.WorkDocs 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workdocs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 workdocs type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 workdocs type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-workdocs.svg?color=blue)](https://pypi.org/project/mypy-boto3-workdocs)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workdocs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-workdocs)](https://pepy.tech/project/mypy-boto3-workdocs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WorkDocs 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs)
+[boto3.WorkDocs 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs)
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
 [mypy-boto3-workdocs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workdocs/).
 
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
@@ -386,20 +386,20 @@
 )
 
 
 def check_value(value: ActivityTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_workdocs.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_workdocs.type_defs import (
     AbortDocumentVersionUploadRequestRequestTypeDef,
     ActivateUserRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     UserMetadataTypeDef,
@@ -410,27 +410,26 @@
     CreateCustomMetadataRequestRequestTypeDef,
     CreateFolderRequestRequestTypeDef,
     FolderMetadataTypeDef,
     CreateLabelsRequestRequestTypeDef,
     CreateNotificationSubscriptionRequestRequestTypeDef,
     SubscriptionTypeDef,
     StorageRuleTypeTypeDef,
-    DateRangeTypeTypeDef,
+    TimestampTypeDef,
     DeactivateUserRequestRequestTypeDef,
     DeleteCommentRequestRequestTypeDef,
     DeleteCustomMetadataRequestRequestTypeDef,
     DeleteDocumentRequestRequestTypeDef,
     DeleteDocumentVersionRequestRequestTypeDef,
     DeleteFolderContentsRequestRequestTypeDef,
     DeleteFolderRequestRequestTypeDef,
     DeleteLabelsRequestRequestTypeDef,
     DeleteNotificationSubscriptionRequestRequestTypeDef,
     DeleteUserRequestRequestTypeDef,
     PaginatorConfigTypeDef,
-    DescribeActivitiesRequestRequestTypeDef,
     DescribeCommentsRequestRequestTypeDef,
     DescribeDocumentVersionsRequestRequestTypeDef,
     DocumentVersionMetadataTypeDef,
     DescribeFolderContentsRequestRequestTypeDef,
     DescribeGroupsRequestRequestTypeDef,
     GroupMetadataTypeDef,
     DescribeNotificationSubscriptionsRequestRequestTypeDef,
@@ -442,15 +441,14 @@
     GetCurrentUserRequestRequestTypeDef,
     GetDocumentPathRequestRequestTypeDef,
     GetDocumentRequestRequestTypeDef,
     GetDocumentVersionRequestRequestTypeDef,
     GetFolderPathRequestRequestTypeDef,
     GetFolderRequestRequestTypeDef,
     GetResourcesRequestRequestTypeDef,
-    InitiateDocumentVersionUploadRequestRequestTypeDef,
     UploadMetadataTypeDef,
     PermissionInfoTypeDef,
     RemoveAllResourcePermissionsRequestRequestTypeDef,
     RemoveResourcePermissionRequestRequestTypeDef,
     ResourcePathComponentTypeDef,
     RestoreDocumentVersionsRequestRequestTypeDef,
     SearchSortResultTypeDef,
@@ -465,58 +463,61 @@
     DescribeRootFoldersResponseTypeDef,
     GetFolderResponseTypeDef,
     CreateNotificationSubscriptionResponseTypeDef,
     DescribeNotificationSubscriptionsResponseTypeDef,
     CreateUserRequestRequestTypeDef,
     UpdateUserRequestRequestTypeDef,
     UserStorageMetadataTypeDef,
+    DateRangeTypeTypeDef,
+    DescribeActivitiesRequestRequestTypeDef,
+    InitiateDocumentVersionUploadRequestRequestTypeDef,
     DescribeActivitiesRequestDescribeActivitiesPaginateTypeDef,
     DescribeCommentsRequestDescribeCommentsPaginateTypeDef,
     DescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef,
     DescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef,
     DescribeGroupsRequestDescribeGroupsPaginateTypeDef,
     DescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef,
     DescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef,
     DescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef,
     DescribeUsersRequestDescribeUsersPaginateTypeDef,
     DescribeDocumentVersionsResponseTypeDef,
     DocumentMetadataTypeDef,
     GetDocumentVersionResponseTypeDef,
     DescribeGroupsResponseTypeDef,
     ParticipantsTypeDef,
-    FiltersTypeDef,
     PrincipalTypeDef,
     ResourcePathTypeDef,
     UserTypeDef,
+    FiltersTypeDef,
     DescribeFolderContentsResponseTypeDef,
     GetDocumentResponseTypeDef,
     GetResourcesResponseTypeDef,
     InitiateDocumentVersionUploadResponseTypeDef,
-    SearchResourcesRequestRequestTypeDef,
-    SearchResourcesRequestSearchResourcesPaginateTypeDef,
     DescribeResourcePermissionsResponseTypeDef,
     GetDocumentPathResponseTypeDef,
     GetFolderPathResponseTypeDef,
     ActivateUserResponseTypeDef,
     CommentMetadataTypeDef,
     CommentTypeDef,
     CreateUserResponseTypeDef,
     DescribeUsersResponseTypeDef,
     GetCurrentUserResponseTypeDef,
     UpdateUserResponseTypeDef,
+    SearchResourcesRequestRequestTypeDef,
+    SearchResourcesRequestSearchResourcesPaginateTypeDef,
     ActivityTypeDef,
     ResponseItemTypeDef,
     CreateCommentResponseTypeDef,
     DescribeCommentsResponseTypeDef,
     DescribeActivitiesResponseTypeDef,
     SearchResourcesResponseTypeDef,
 )
 
 
-def get_structure() -> AbortDocumentVersionUploadRequestRequestTypeDef:
+def get_value() -> AbortDocumentVersionUploadRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-workdocs-1.28.15.post1/mypy_boto3_workdocs.egg-info/SOURCES.txt` & `mypy-boto3-workdocs-1.28.16/mypy_boto3_workdocs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workdocs-1.28.15.post1/setup.py` & `mypy-boto3-workdocs-1.28.16/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-workdocs",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_workdocs"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.WorkDocs 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.2"
+        "Type annotations for boto3.WorkDocs 1.28.16 service generated with mypy-boto3-builder"
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
-    keywords="boto3 workdocs type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 workdocs type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_workdocs": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workdocs/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

