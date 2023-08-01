# Comparing `tmp/mypy-boto3-codecommit-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-codecommit-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-codecommit-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:45 2023, max compression
+gzip compressed data, was "mypy-boto3-codecommit-1.28.16.tar", last modified: Tue Aug  1 11:36:25 2023, max compression
```

## Comparing `mypy-boto3-codecommit-1.28.15.post1.tar` & `mypy-boto3-codecommit-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:45.249064 mypy-boto3-codecommit-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:40:34.000000 mypy-boto3-codecommit-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    22940 2023-07-29 10:02:45.245064 mypy-boto3-codecommit-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21435 2023-07-29 09:40:34.000000 mypy-boto3-codecommit-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:45.245064 mypy-boto3-codecommit-1.28.15.post1/mypy_boto3_codecommit/
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-07-29 09:40:34.000000 mypy-boto3-codecommit-1.28.15.post1/mypy_boto3_codecommit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-29 09:40:34.000000 mypy-boto3-codecommit-1.28.15.post1/mypy_boto3_codecommit/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-29 09:40:34.000000 mypy-boto3-codecommit-1.28.15.post1/mypy_boto3_codecommit/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    71938 2023-07-29 09:40:36.000000 mypy-boto3-codecommit-1.28.15.post1/mypy_boto3_codecommit/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    71847 2023-07-29 09:40:36.000000 mypy-boto3-codecommit-1.28.15.post1/mypy_boto3_codecommit/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10990 2023-07-29 09:40:37.000000 mypy-boto3-codecommit-1.28.15.post1/mypy_boto3_codecommit/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10988 2023-07-29 09:40:37.000000 mypy-boto3-codecommit-1.28.15.post1/mypy_boto3_codecommit/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9450 2023-07-29 09:40:36.000000 mypy-boto3-codecommit-1.28.15.post1/mypy_boto3_codecommit/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9441 2023-07-29 09:40:36.000000 mypy-boto3-codecommit-1.28.15.post1/mypy_boto3_codecommit/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:40:34.000000 mypy-boto3-codecommit-1.28.15.post1/mypy_boto3_codecommit/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    79439 2023-07-29 09:40:39.000000 mypy-boto3-codecommit-1.28.15.post1/mypy_boto3_codecommit/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    79342 2023-07-29 09:40:38.000000 mypy-boto3-codecommit-1.28.15.post1/mypy_boto3_codecommit/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:40:34.000000 mypy-boto3-codecommit-1.28.15.post1/mypy_boto3_codecommit/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:45.245064 mypy-boto3-codecommit-1.28.15.post1/mypy_boto3_codecommit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22940 2023-07-29 10:02:44.000000 mypy-boto3-codecommit-1.28.15.post1/mypy_boto3_codecommit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-29 10:02:45.000000 mypy-boto3-codecommit-1.28.15.post1/mypy_boto3_codecommit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:44.000000 mypy-boto3-codecommit-1.28.15.post1/mypy_boto3_codecommit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:44.000000 mypy-boto3-codecommit-1.28.15.post1/mypy_boto3_codecommit.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:44.000000 mypy-boto3-codecommit-1.28.15.post1/mypy_boto3_codecommit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-29 10:02:44.000000 mypy-boto3-codecommit-1.28.15.post1/mypy_boto3_codecommit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:45.249064 mypy-boto3-codecommit-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-07-29 09:40:34.000000 mypy-boto3-codecommit-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:25.772928 mypy-boto3-codecommit-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:13:08.000000 mypy-boto3-codecommit-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22982 2023-08-01 11:36:25.764928 mypy-boto3-codecommit-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21486 2023-08-01 11:13:08.000000 mypy-boto3-codecommit-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:25.764928 mypy-boto3-codecommit-1.28.16/mypy_boto3_codecommit/
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-08-01 11:13:08.000000 mypy-boto3-codecommit-1.28.16/mypy_boto3_codecommit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-08-01 11:13:08.000000 mypy-boto3-codecommit-1.28.16/mypy_boto3_codecommit/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-08-01 11:13:08.000000 mypy-boto3-codecommit-1.28.16/mypy_boto3_codecommit/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71723 2023-08-01 11:13:08.000000 mypy-boto3-codecommit-1.28.16/mypy_boto3_codecommit/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71632 2023-08-01 11:13:08.000000 mypy-boto3-codecommit-1.28.16/mypy_boto3_codecommit/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10990 2023-08-01 11:13:09.000000 mypy-boto3-codecommit-1.28.16/mypy_boto3_codecommit/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10988 2023-08-01 11:13:09.000000 mypy-boto3-codecommit-1.28.16/mypy_boto3_codecommit/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9450 2023-08-01 11:13:08.000000 mypy-boto3-codecommit-1.28.16/mypy_boto3_codecommit/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9441 2023-08-01 11:13:08.000000 mypy-boto3-codecommit-1.28.16/mypy_boto3_codecommit/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:13:08.000000 mypy-boto3-codecommit-1.28.16/mypy_boto3_codecommit/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    79487 2023-08-01 11:13:12.000000 mypy-boto3-codecommit-1.28.16/mypy_boto3_codecommit/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79390 2023-08-01 11:13:10.000000 mypy-boto3-codecommit-1.28.16/mypy_boto3_codecommit/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:13:08.000000 mypy-boto3-codecommit-1.28.16/mypy_boto3_codecommit/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:25.764928 mypy-boto3-codecommit-1.28.16/mypy_boto3_codecommit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22982 2023-08-01 11:36:25.000000 mypy-boto3-codecommit-1.28.16/mypy_boto3_codecommit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-08-01 11:36:25.000000 mypy-boto3-codecommit-1.28.16/mypy_boto3_codecommit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:25.000000 mypy-boto3-codecommit-1.28.16/mypy_boto3_codecommit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:25.000000 mypy-boto3-codecommit-1.28.16/mypy_boto3_codecommit.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:25.000000 mypy-boto3-codecommit-1.28.16/mypy_boto3_codecommit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-01 11:36:25.000000 mypy-boto3-codecommit-1.28.16/mypy_boto3_codecommit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:25.772928 mypy-boto3-codecommit-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-08-01 11:13:07.000000 mypy-boto3-codecommit-1.28.16/setup.py
```

### Comparing `mypy-boto3-codecommit-1.28.15.post1/LICENSE` & `mypy-boto3-codecommit-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codecommit-1.28.15.post1/PKG-INFO` & `mypy-boto3-codecommit-1.28.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-codecommit
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.CodeCommit 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.CodeCommit 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 codecommit type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 codecommit type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codecommit.svg?color=blue)](https://pypi.org/project/mypy-boto3-codecommit)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codecommit)](https://pepy.tech/project/mypy-boto3-codecommit)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeCommit 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit)
+[boto3.CodeCommit 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit)
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
 [mypy-boto3-codecommit docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit/).
 
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
@@ -350,20 +350,20 @@
 )
 
 
 def check_value(value: ApprovalStateType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_codecommit.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_codecommit.type_defs import (
     ApprovalRuleEventMetadataTypeDef,
     ApprovalRuleOverriddenEventMetadataTypeDef,
     ApprovalRuleTemplateTypeDef,
     OriginApprovalRuleTemplateTypeDef,
@@ -378,25 +378,25 @@
     BatchDisassociateApprovalRuleTemplateFromRepositoriesErrorTypeDef,
     BatchDisassociateApprovalRuleTemplateFromRepositoriesInputRequestTypeDef,
     BatchGetCommitsErrorTypeDef,
     BatchGetCommitsInputRequestTypeDef,
     BatchGetRepositoriesInputRequestTypeDef,
     RepositoryMetadataTypeDef,
     BlobMetadataTypeDef,
+    BlobTypeDef,
     BranchInfoTypeDef,
     CommentTypeDef,
     LocationTypeDef,
     UserInfoTypeDef,
     FileModesTypeDef,
     FileSizesTypeDef,
     IsBinaryFileTypeDef,
     MergeOperationsTypeDef,
     ObjectTypesTypeDef,
     DeleteFileEntryTypeDef,
-    ReplaceContentEntryTypeDef,
     SetFileModeEntryTypeDef,
     CreateApprovalRuleTemplateInputRequestTypeDef,
     CreateBranchInputRequestTypeDef,
     FileMetadataTypeDef,
     CreatePullRequestApprovalRuleInputRequestTypeDef,
     TargetTypeDef,
     CreateRepositoryInputRequestTypeDef,
@@ -451,18 +451,17 @@
     OverridePullRequestApprovalRulesInputRequestTypeDef,
     PostCommentReplyInputRequestTypeDef,
     PullRequestCreatedEventMetadataTypeDef,
     PullRequestSourceReferenceUpdatedEventMetadataTypeDef,
     PullRequestStatusChangedEventMetadataTypeDef,
     PutCommentReactionInputRequestTypeDef,
     SourceFileSpecifierTypeDef,
-    PutFileInputRequestTypeDef,
-    RepositoryTriggerTypeDef,
     ReactionValueFormatsTypeDef,
     RepositoryTriggerExecutionFailureTypeDef,
+    RepositoryTriggerTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateApprovalRuleTemplateContentInputRequestTypeDef,
     UpdateApprovalRuleTemplateDescriptionInputRequestTypeDef,
     UpdateApprovalRuleTemplateNameInputRequestTypeDef,
     UpdateCommentInputRequestTypeDef,
     UpdateDefaultBranchInputRequestTypeDef,
@@ -504,29 +503,30 @@
     UpdateApprovalRuleTemplateDescriptionOutputTypeDef,
     UpdateApprovalRuleTemplateNameOutputTypeDef,
     BatchDisassociateApprovalRuleTemplateFromRepositoriesOutputTypeDef,
     BatchGetRepositoriesOutputTypeDef,
     CreateRepositoryOutputTypeDef,
     GetRepositoryOutputTypeDef,
     DifferenceTypeDef,
+    PutFileInputRequestTypeDef,
+    ReplaceContentEntryTypeDef,
     DeleteBranchOutputTypeDef,
     GetBranchOutputTypeDef,
     DeleteCommentContentOutputTypeDef,
     GetCommentOutputTypeDef,
     PostCommentReplyOutputTypeDef,
     UpdateCommentOutputTypeDef,
     CommentsForComparedCommitTypeDef,
     CommentsForPullRequestTypeDef,
     PostCommentForComparedCommitInputRequestTypeDef,
     PostCommentForComparedCommitOutputTypeDef,
     PostCommentForPullRequestInputRequestTypeDef,
     PostCommentForPullRequestOutputTypeDef,
     CommitTypeDef,
     ConflictMetadataTypeDef,
-    ConflictResolutionTypeDef,
     CreateCommitOutputTypeDef,
     CreatePullRequestInputRequestTypeDef,
     DescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef,
     GetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef,
     GetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef,
     GetDifferencesInputGetDifferencesPaginateTypeDef,
     ListBranchesInputListBranchesPaginateTypeDef,
@@ -536,51 +536,53 @@
     GetFolderOutputTypeDef,
     GetRepositoryTriggersOutputTypeDef,
     ListRepositoriesOutputTypeDef,
     MergeHunkTypeDef,
     PullRequestMergedStateChangedEventMetadataTypeDef,
     PullRequestTargetTypeDef,
     PutFileEntryTypeDef,
-    PutRepositoryTriggersInputRequestTypeDef,
-    TestRepositoryTriggersInputRequestTypeDef,
     ReactionForCommentTypeDef,
     TestRepositoryTriggersOutputTypeDef,
+    RepositoryTriggerUnionTypeDef,
     CreatePullRequestApprovalRuleOutputTypeDef,
     UpdatePullRequestApprovalRuleContentOutputTypeDef,
     GetDifferencesOutputTypeDef,
+    ConflictResolutionTypeDef,
     GetCommentsForComparedCommitOutputTypeDef,
     GetCommentsForPullRequestOutputTypeDef,
     BatchGetCommitsOutputTypeDef,
     GetCommitOutputTypeDef,
     GetMergeConflictsOutputTypeDef,
-    CreateUnreferencedMergeCommitInputRequestTypeDef,
-    MergeBranchesBySquashInputRequestTypeDef,
-    MergeBranchesByThreeWayInputRequestTypeDef,
-    MergePullRequestBySquashInputRequestTypeDef,
-    MergePullRequestByThreeWayInputRequestTypeDef,
     ConflictTypeDef,
     DescribeMergeConflictsOutputTypeDef,
     PullRequestEventTypeDef,
     PullRequestTypeDef,
     CreateCommitInputRequestTypeDef,
     GetCommentReactionsOutputTypeDef,
+    PutRepositoryTriggersInputRequestTypeDef,
+    TestRepositoryTriggersInputRequestTypeDef,
+    CreateUnreferencedMergeCommitInputRequestTypeDef,
+    MergeBranchesBySquashInputRequestTypeDef,
+    MergeBranchesByThreeWayInputRequestTypeDef,
+    MergePullRequestBySquashInputRequestTypeDef,
+    MergePullRequestByThreeWayInputRequestTypeDef,
     BatchDescribeMergeConflictsOutputTypeDef,
     DescribePullRequestEventsOutputTypeDef,
     CreatePullRequestOutputTypeDef,
     GetPullRequestOutputTypeDef,
     MergePullRequestByFastForwardOutputTypeDef,
     MergePullRequestBySquashOutputTypeDef,
     MergePullRequestByThreeWayOutputTypeDef,
     UpdatePullRequestDescriptionOutputTypeDef,
     UpdatePullRequestStatusOutputTypeDef,
     UpdatePullRequestTitleOutputTypeDef,
 )
 
 
-def get_structure() -> ApprovalRuleEventMetadataTypeDef:
+def get_value() -> ApprovalRuleEventMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-codecommit-1.28.15.post1/README.md` & `mypy-boto3-codecommit-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codecommit.svg?color=blue)](https://pypi.org/project/mypy-boto3-codecommit)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codecommit)](https://pepy.tech/project/mypy-boto3-codecommit)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeCommit 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit)
+[boto3.CodeCommit 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit)
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
 [mypy-boto3-codecommit docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit/).
 
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
@@ -318,20 +318,20 @@
 )
 
 
 def check_value(value: ApprovalStateType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_codecommit.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_codecommit.type_defs import (
     ApprovalRuleEventMetadataTypeDef,
     ApprovalRuleOverriddenEventMetadataTypeDef,
     ApprovalRuleTemplateTypeDef,
     OriginApprovalRuleTemplateTypeDef,
@@ -346,25 +346,25 @@
     BatchDisassociateApprovalRuleTemplateFromRepositoriesErrorTypeDef,
     BatchDisassociateApprovalRuleTemplateFromRepositoriesInputRequestTypeDef,
     BatchGetCommitsErrorTypeDef,
     BatchGetCommitsInputRequestTypeDef,
     BatchGetRepositoriesInputRequestTypeDef,
     RepositoryMetadataTypeDef,
     BlobMetadataTypeDef,
+    BlobTypeDef,
     BranchInfoTypeDef,
     CommentTypeDef,
     LocationTypeDef,
     UserInfoTypeDef,
     FileModesTypeDef,
     FileSizesTypeDef,
     IsBinaryFileTypeDef,
     MergeOperationsTypeDef,
     ObjectTypesTypeDef,
     DeleteFileEntryTypeDef,
-    ReplaceContentEntryTypeDef,
     SetFileModeEntryTypeDef,
     CreateApprovalRuleTemplateInputRequestTypeDef,
     CreateBranchInputRequestTypeDef,
     FileMetadataTypeDef,
     CreatePullRequestApprovalRuleInputRequestTypeDef,
     TargetTypeDef,
     CreateRepositoryInputRequestTypeDef,
@@ -419,18 +419,17 @@
     OverridePullRequestApprovalRulesInputRequestTypeDef,
     PostCommentReplyInputRequestTypeDef,
     PullRequestCreatedEventMetadataTypeDef,
     PullRequestSourceReferenceUpdatedEventMetadataTypeDef,
     PullRequestStatusChangedEventMetadataTypeDef,
     PutCommentReactionInputRequestTypeDef,
     SourceFileSpecifierTypeDef,
-    PutFileInputRequestTypeDef,
-    RepositoryTriggerTypeDef,
     ReactionValueFormatsTypeDef,
     RepositoryTriggerExecutionFailureTypeDef,
+    RepositoryTriggerTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateApprovalRuleTemplateContentInputRequestTypeDef,
     UpdateApprovalRuleTemplateDescriptionInputRequestTypeDef,
     UpdateApprovalRuleTemplateNameInputRequestTypeDef,
     UpdateCommentInputRequestTypeDef,
     UpdateDefaultBranchInputRequestTypeDef,
@@ -472,29 +471,30 @@
     UpdateApprovalRuleTemplateDescriptionOutputTypeDef,
     UpdateApprovalRuleTemplateNameOutputTypeDef,
     BatchDisassociateApprovalRuleTemplateFromRepositoriesOutputTypeDef,
     BatchGetRepositoriesOutputTypeDef,
     CreateRepositoryOutputTypeDef,
     GetRepositoryOutputTypeDef,
     DifferenceTypeDef,
+    PutFileInputRequestTypeDef,
+    ReplaceContentEntryTypeDef,
     DeleteBranchOutputTypeDef,
     GetBranchOutputTypeDef,
     DeleteCommentContentOutputTypeDef,
     GetCommentOutputTypeDef,
     PostCommentReplyOutputTypeDef,
     UpdateCommentOutputTypeDef,
     CommentsForComparedCommitTypeDef,
     CommentsForPullRequestTypeDef,
     PostCommentForComparedCommitInputRequestTypeDef,
     PostCommentForComparedCommitOutputTypeDef,
     PostCommentForPullRequestInputRequestTypeDef,
     PostCommentForPullRequestOutputTypeDef,
     CommitTypeDef,
     ConflictMetadataTypeDef,
-    ConflictResolutionTypeDef,
     CreateCommitOutputTypeDef,
     CreatePullRequestInputRequestTypeDef,
     DescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef,
     GetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef,
     GetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef,
     GetDifferencesInputGetDifferencesPaginateTypeDef,
     ListBranchesInputListBranchesPaginateTypeDef,
@@ -504,51 +504,53 @@
     GetFolderOutputTypeDef,
     GetRepositoryTriggersOutputTypeDef,
     ListRepositoriesOutputTypeDef,
     MergeHunkTypeDef,
     PullRequestMergedStateChangedEventMetadataTypeDef,
     PullRequestTargetTypeDef,
     PutFileEntryTypeDef,
-    PutRepositoryTriggersInputRequestTypeDef,
-    TestRepositoryTriggersInputRequestTypeDef,
     ReactionForCommentTypeDef,
     TestRepositoryTriggersOutputTypeDef,
+    RepositoryTriggerUnionTypeDef,
     CreatePullRequestApprovalRuleOutputTypeDef,
     UpdatePullRequestApprovalRuleContentOutputTypeDef,
     GetDifferencesOutputTypeDef,
+    ConflictResolutionTypeDef,
     GetCommentsForComparedCommitOutputTypeDef,
     GetCommentsForPullRequestOutputTypeDef,
     BatchGetCommitsOutputTypeDef,
     GetCommitOutputTypeDef,
     GetMergeConflictsOutputTypeDef,
-    CreateUnreferencedMergeCommitInputRequestTypeDef,
-    MergeBranchesBySquashInputRequestTypeDef,
-    MergeBranchesByThreeWayInputRequestTypeDef,
-    MergePullRequestBySquashInputRequestTypeDef,
-    MergePullRequestByThreeWayInputRequestTypeDef,
     ConflictTypeDef,
     DescribeMergeConflictsOutputTypeDef,
     PullRequestEventTypeDef,
     PullRequestTypeDef,
     CreateCommitInputRequestTypeDef,
     GetCommentReactionsOutputTypeDef,
+    PutRepositoryTriggersInputRequestTypeDef,
+    TestRepositoryTriggersInputRequestTypeDef,
+    CreateUnreferencedMergeCommitInputRequestTypeDef,
+    MergeBranchesBySquashInputRequestTypeDef,
+    MergeBranchesByThreeWayInputRequestTypeDef,
+    MergePullRequestBySquashInputRequestTypeDef,
+    MergePullRequestByThreeWayInputRequestTypeDef,
     BatchDescribeMergeConflictsOutputTypeDef,
     DescribePullRequestEventsOutputTypeDef,
     CreatePullRequestOutputTypeDef,
     GetPullRequestOutputTypeDef,
     MergePullRequestByFastForwardOutputTypeDef,
     MergePullRequestBySquashOutputTypeDef,
     MergePullRequestByThreeWayOutputTypeDef,
     UpdatePullRequestDescriptionOutputTypeDef,
     UpdatePullRequestStatusOutputTypeDef,
     UpdatePullRequestTitleOutputTypeDef,
 )
 
 
-def get_structure() -> ApprovalRuleEventMetadataTypeDef:
+def get_value() -> ApprovalRuleEventMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-codecommit-1.28.15.post1/mypy_boto3_codecommit/__init__.py` & `mypy-boto3-codecommit-1.28.16/mypy_boto3_codecommit/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codecommit-1.28.15.post1/mypy_boto3_codecommit/__init__.pyi` & `mypy-boto3-codecommit-1.28.16/mypy_boto3_codecommit/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codecommit-1.28.15.post1/mypy_boto3_codecommit/__main__.py` & `mypy-boto3-codecommit-1.28.16/mypy_boto3_codecommit/__main__.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CodeCommit 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.CodeCommit 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit\nOther"
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

### Comparing `mypy-boto3-codecommit-1.28.15.post1/mypy_boto3_codecommit/client.py` & `mypy-boto3-codecommit-1.28.16/mypy_boto3_codecommit/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,18 +10,17 @@
     from mypy_boto3_codecommit.client import CodeCommitClient
 
     session = Session()
     client: CodeCommitClient = session.client("codecommit")
     ```
 """
 import sys
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
-from botocore.response import StreamingBody
 
 from .literals import (
     ApprovalStateType,
     ConflictDetailLevelTypeEnumType,
     ConflictResolutionStrategyTypeEnumType,
     FileModeTypeEnumType,
     MergeOptionTypeEnumType,
@@ -42,14 +41,15 @@
 )
 from .type_defs import (
     BatchAssociateApprovalRuleTemplateWithRepositoriesOutputTypeDef,
     BatchDescribeMergeConflictsOutputTypeDef,
     BatchDisassociateApprovalRuleTemplateFromRepositoriesOutputTypeDef,
     BatchGetCommitsOutputTypeDef,
     BatchGetRepositoriesOutputTypeDef,
+    BlobTypeDef,
     ConflictResolutionTypeDef,
     CreateApprovalRuleTemplateOutputTypeDef,
     CreateCommitOutputTypeDef,
     CreatePullRequestApprovalRuleOutputTypeDef,
     CreatePullRequestOutputTypeDef,
     CreateRepositoryOutputTypeDef,
     CreateUnreferencedMergeCommitOutputTypeDef,
@@ -99,16 +99,15 @@
     MergePullRequestByThreeWayOutputTypeDef,
     PostCommentForComparedCommitOutputTypeDef,
     PostCommentForPullRequestOutputTypeDef,
     PostCommentReplyOutputTypeDef,
     PutFileEntryTypeDef,
     PutFileOutputTypeDef,
     PutRepositoryTriggersOutputTypeDef,
-    RepositoryTriggerOutputTypeDef,
-    RepositoryTriggerTypeDef,
+    RepositoryTriggerUnionTypeDef,
     SetFileModeEntryTypeDef,
     TargetTypeDef,
     TestRepositoryTriggersOutputTypeDef,
     UpdateApprovalRuleTemplateContentOutputTypeDef,
     UpdateApprovalRuleTemplateDescriptionOutputTypeDef,
     UpdateApprovalRuleTemplateNameOutputTypeDef,
     UpdateCommentOutputTypeDef,
@@ -1178,15 +1177,15 @@
         """
 
     def put_file(
         self,
         *,
         repositoryName: str,
         branchName: str,
-        fileContent: Union[str, bytes, IO[Any], StreamingBody],
+        fileContent: BlobTypeDef,
         filePath: str,
         fileMode: FileModeTypeEnumType = ...,
         parentCommitId: str = ...,
         commitMessage: str = ...,
         name: str = ...,
         email: str = ...
     ) -> PutFileOutputTypeDef:
@@ -1195,18 +1194,15 @@
         generates a commit for the addition in the specified branch.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Client.put_file)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit/client/#put_file)
         """
 
     def put_repository_triggers(
-        self,
-        *,
-        repositoryName: str,
-        triggers: Sequence[Union[RepositoryTriggerTypeDef, RepositoryTriggerOutputTypeDef]]
+        self, *, repositoryName: str, triggers: Sequence[RepositoryTriggerUnionTypeDef]
     ) -> PutRepositoryTriggersOutputTypeDef:
         """
         Replaces all triggers for a repository.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Client.put_repository_triggers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit/client/#put_repository_triggers)
         """
@@ -1218,18 +1214,15 @@
         Adds or updates tags for a resource in AWS CodeCommit.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit/client/#tag_resource)
         """
 
     def test_repository_triggers(
-        self,
-        *,
-        repositoryName: str,
-        triggers: Sequence[Union[RepositoryTriggerTypeDef, RepositoryTriggerOutputTypeDef]]
+        self, *, repositoryName: str, triggers: Sequence[RepositoryTriggerUnionTypeDef]
     ) -> TestRepositoryTriggersOutputTypeDef:
         """
         Tests the functionality of repository triggers by sending information to the
         trigger target.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Client.test_repository_triggers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit/client/#test_repository_triggers)
```

### Comparing `mypy-boto3-codecommit-1.28.15.post1/mypy_boto3_codecommit/client.pyi` & `mypy-boto3-codecommit-1.28.16/mypy_boto3_codecommit/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,18 +10,17 @@
     from mypy_boto3_codecommit.client import CodeCommitClient
 
     session = Session()
     client: CodeCommitClient = session.client("codecommit")
     ```
 """
 import sys
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
-from botocore.response import StreamingBody
 
 from .literals import (
     ApprovalStateType,
     ConflictDetailLevelTypeEnumType,
     ConflictResolutionStrategyTypeEnumType,
     FileModeTypeEnumType,
     MergeOptionTypeEnumType,
@@ -42,14 +41,15 @@
 )
 from .type_defs import (
     BatchAssociateApprovalRuleTemplateWithRepositoriesOutputTypeDef,
     BatchDescribeMergeConflictsOutputTypeDef,
     BatchDisassociateApprovalRuleTemplateFromRepositoriesOutputTypeDef,
     BatchGetCommitsOutputTypeDef,
     BatchGetRepositoriesOutputTypeDef,
+    BlobTypeDef,
     ConflictResolutionTypeDef,
     CreateApprovalRuleTemplateOutputTypeDef,
     CreateCommitOutputTypeDef,
     CreatePullRequestApprovalRuleOutputTypeDef,
     CreatePullRequestOutputTypeDef,
     CreateRepositoryOutputTypeDef,
     CreateUnreferencedMergeCommitOutputTypeDef,
@@ -99,16 +99,15 @@
     MergePullRequestByThreeWayOutputTypeDef,
     PostCommentForComparedCommitOutputTypeDef,
     PostCommentForPullRequestOutputTypeDef,
     PostCommentReplyOutputTypeDef,
     PutFileEntryTypeDef,
     PutFileOutputTypeDef,
     PutRepositoryTriggersOutputTypeDef,
-    RepositoryTriggerOutputTypeDef,
-    RepositoryTriggerTypeDef,
+    RepositoryTriggerUnionTypeDef,
     SetFileModeEntryTypeDef,
     TargetTypeDef,
     TestRepositoryTriggersOutputTypeDef,
     UpdateApprovalRuleTemplateContentOutputTypeDef,
     UpdateApprovalRuleTemplateDescriptionOutputTypeDef,
     UpdateApprovalRuleTemplateNameOutputTypeDef,
     UpdateCommentOutputTypeDef,
@@ -1110,15 +1109,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit/client/#put_comment_reaction)
         """
     def put_file(
         self,
         *,
         repositoryName: str,
         branchName: str,
-        fileContent: Union[str, bytes, IO[Any], StreamingBody],
+        fileContent: BlobTypeDef,
         filePath: str,
         fileMode: FileModeTypeEnumType = ...,
         parentCommitId: str = ...,
         commitMessage: str = ...,
         name: str = ...,
         email: str = ...
     ) -> PutFileOutputTypeDef:
@@ -1126,18 +1125,15 @@
         Adds or updates a file in a branch in an AWS CodeCommit repository, and
         generates a commit for the addition in the specified branch.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Client.put_file)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit/client/#put_file)
         """
     def put_repository_triggers(
-        self,
-        *,
-        repositoryName: str,
-        triggers: Sequence[Union[RepositoryTriggerTypeDef, RepositoryTriggerOutputTypeDef]]
+        self, *, repositoryName: str, triggers: Sequence[RepositoryTriggerUnionTypeDef]
     ) -> PutRepositoryTriggersOutputTypeDef:
         """
         Replaces all triggers for a repository.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Client.put_repository_triggers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit/client/#put_repository_triggers)
         """
@@ -1147,18 +1143,15 @@
         """
         Adds or updates tags for a resource in AWS CodeCommit.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit/client/#tag_resource)
         """
     def test_repository_triggers(
-        self,
-        *,
-        repositoryName: str,
-        triggers: Sequence[Union[RepositoryTriggerTypeDef, RepositoryTriggerOutputTypeDef]]
+        self, *, repositoryName: str, triggers: Sequence[RepositoryTriggerUnionTypeDef]
     ) -> TestRepositoryTriggersOutputTypeDef:
         """
         Tests the functionality of repository triggers by sending information to the
         trigger target.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit.Client.test_repository_triggers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit/client/#test_repository_triggers)
```

### Comparing `mypy-boto3-codecommit-1.28.15.post1/mypy_boto3_codecommit/literals.py` & `mypy-boto3-codecommit-1.28.16/mypy_boto3_codecommit/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codecommit-1.28.15.post1/mypy_boto3_codecommit/literals.pyi` & `mypy-boto3-codecommit-1.28.16/mypy_boto3_codecommit/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codecommit-1.28.15.post1/mypy_boto3_codecommit/paginator.py` & `mypy-boto3-codecommit-1.28.16/mypy_boto3_codecommit/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codecommit-1.28.15.post1/mypy_boto3_codecommit/paginator.pyi` & `mypy-boto3-codecommit-1.28.16/mypy_boto3_codecommit/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codecommit-1.28.15.post1/mypy_boto3_codecommit/type_defs.py` & `mypy-boto3-codecommit-1.28.16/mypy_boto3_codecommit/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_codecommit.type_defs import ApprovalRuleEventMetadataTypeDef
 
-    data: ApprovalRuleEventMetadataTypeDef = {...}
+    data: ApprovalRuleEventMetadataTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -57,25 +57,25 @@
     "BatchDisassociateApprovalRuleTemplateFromRepositoriesErrorTypeDef",
     "BatchDisassociateApprovalRuleTemplateFromRepositoriesInputRequestTypeDef",
     "BatchGetCommitsErrorTypeDef",
     "BatchGetCommitsInputRequestTypeDef",
     "BatchGetRepositoriesInputRequestTypeDef",
     "RepositoryMetadataTypeDef",
     "BlobMetadataTypeDef",
+    "BlobTypeDef",
     "BranchInfoTypeDef",
     "CommentTypeDef",
     "LocationTypeDef",
     "UserInfoTypeDef",
     "FileModesTypeDef",
     "FileSizesTypeDef",
     "IsBinaryFileTypeDef",
     "MergeOperationsTypeDef",
     "ObjectTypesTypeDef",
     "DeleteFileEntryTypeDef",
-    "ReplaceContentEntryTypeDef",
     "SetFileModeEntryTypeDef",
     "CreateApprovalRuleTemplateInputRequestTypeDef",
     "CreateBranchInputRequestTypeDef",
     "FileMetadataTypeDef",
     "CreatePullRequestApprovalRuleInputRequestTypeDef",
     "TargetTypeDef",
     "CreateRepositoryInputRequestTypeDef",
@@ -130,18 +130,17 @@
     "OverridePullRequestApprovalRulesInputRequestTypeDef",
     "PostCommentReplyInputRequestTypeDef",
     "PullRequestCreatedEventMetadataTypeDef",
     "PullRequestSourceReferenceUpdatedEventMetadataTypeDef",
     "PullRequestStatusChangedEventMetadataTypeDef",
     "PutCommentReactionInputRequestTypeDef",
     "SourceFileSpecifierTypeDef",
-    "PutFileInputRequestTypeDef",
-    "RepositoryTriggerTypeDef",
     "ReactionValueFormatsTypeDef",
     "RepositoryTriggerExecutionFailureTypeDef",
+    "RepositoryTriggerTypeDef",
     "TagResourceInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateApprovalRuleTemplateContentInputRequestTypeDef",
     "UpdateApprovalRuleTemplateDescriptionInputRequestTypeDef",
     "UpdateApprovalRuleTemplateNameInputRequestTypeDef",
     "UpdateCommentInputRequestTypeDef",
     "UpdateDefaultBranchInputRequestTypeDef",
@@ -183,29 +182,30 @@
     "UpdateApprovalRuleTemplateDescriptionOutputTypeDef",
     "UpdateApprovalRuleTemplateNameOutputTypeDef",
     "BatchDisassociateApprovalRuleTemplateFromRepositoriesOutputTypeDef",
     "BatchGetRepositoriesOutputTypeDef",
     "CreateRepositoryOutputTypeDef",
     "GetRepositoryOutputTypeDef",
     "DifferenceTypeDef",
+    "PutFileInputRequestTypeDef",
+    "ReplaceContentEntryTypeDef",
     "DeleteBranchOutputTypeDef",
     "GetBranchOutputTypeDef",
     "DeleteCommentContentOutputTypeDef",
     "GetCommentOutputTypeDef",
     "PostCommentReplyOutputTypeDef",
     "UpdateCommentOutputTypeDef",
     "CommentsForComparedCommitTypeDef",
     "CommentsForPullRequestTypeDef",
     "PostCommentForComparedCommitInputRequestTypeDef",
     "PostCommentForComparedCommitOutputTypeDef",
     "PostCommentForPullRequestInputRequestTypeDef",
     "PostCommentForPullRequestOutputTypeDef",
     "CommitTypeDef",
     "ConflictMetadataTypeDef",
-    "ConflictResolutionTypeDef",
     "CreateCommitOutputTypeDef",
     "CreatePullRequestInputRequestTypeDef",
     "DescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef",
     "GetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef",
     "GetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef",
     "GetDifferencesInputGetDifferencesPaginateTypeDef",
     "ListBranchesInputListBranchesPaginateTypeDef",
@@ -215,37 +215,39 @@
     "GetFolderOutputTypeDef",
     "GetRepositoryTriggersOutputTypeDef",
     "ListRepositoriesOutputTypeDef",
     "MergeHunkTypeDef",
     "PullRequestMergedStateChangedEventMetadataTypeDef",
     "PullRequestTargetTypeDef",
     "PutFileEntryTypeDef",
-    "PutRepositoryTriggersInputRequestTypeDef",
-    "TestRepositoryTriggersInputRequestTypeDef",
     "ReactionForCommentTypeDef",
     "TestRepositoryTriggersOutputTypeDef",
+    "RepositoryTriggerUnionTypeDef",
     "CreatePullRequestApprovalRuleOutputTypeDef",
     "UpdatePullRequestApprovalRuleContentOutputTypeDef",
     "GetDifferencesOutputTypeDef",
+    "ConflictResolutionTypeDef",
     "GetCommentsForComparedCommitOutputTypeDef",
     "GetCommentsForPullRequestOutputTypeDef",
     "BatchGetCommitsOutputTypeDef",
     "GetCommitOutputTypeDef",
     "GetMergeConflictsOutputTypeDef",
-    "CreateUnreferencedMergeCommitInputRequestTypeDef",
-    "MergeBranchesBySquashInputRequestTypeDef",
-    "MergeBranchesByThreeWayInputRequestTypeDef",
-    "MergePullRequestBySquashInputRequestTypeDef",
-    "MergePullRequestByThreeWayInputRequestTypeDef",
     "ConflictTypeDef",
     "DescribeMergeConflictsOutputTypeDef",
     "PullRequestEventTypeDef",
     "PullRequestTypeDef",
     "CreateCommitInputRequestTypeDef",
     "GetCommentReactionsOutputTypeDef",
+    "PutRepositoryTriggersInputRequestTypeDef",
+    "TestRepositoryTriggersInputRequestTypeDef",
+    "CreateUnreferencedMergeCommitInputRequestTypeDef",
+    "MergeBranchesBySquashInputRequestTypeDef",
+    "MergeBranchesByThreeWayInputRequestTypeDef",
+    "MergePullRequestBySquashInputRequestTypeDef",
+    "MergePullRequestByThreeWayInputRequestTypeDef",
     "BatchDescribeMergeConflictsOutputTypeDef",
     "DescribePullRequestEventsOutputTypeDef",
     "CreatePullRequestOutputTypeDef",
     "GetPullRequestOutputTypeDef",
     "MergePullRequestByFastForwardOutputTypeDef",
     "MergePullRequestBySquashOutputTypeDef",
     "MergePullRequestByThreeWayOutputTypeDef",
@@ -457,14 +459,15 @@
         "blobId": str,
         "path": str,
         "mode": str,
     },
     total=False,
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 BranchInfoTypeDef = TypedDict(
     "BranchInfoTypeDef",
     {
         "branchName": str,
         "commitId": str,
     },
     total=False,
@@ -559,37 +562,14 @@
 DeleteFileEntryTypeDef = TypedDict(
     "DeleteFileEntryTypeDef",
     {
         "filePath": str,
     },
 )
 
-_RequiredReplaceContentEntryTypeDef = TypedDict(
-    "_RequiredReplaceContentEntryTypeDef",
-    {
-        "filePath": str,
-        "replacementType": ReplacementTypeEnumType,
-    },
-)
-_OptionalReplaceContentEntryTypeDef = TypedDict(
-    "_OptionalReplaceContentEntryTypeDef",
-    {
-        "content": Union[str, bytes, IO[Any], StreamingBody],
-        "fileMode": FileModeTypeEnumType,
-    },
-    total=False,
-)
-
-
-class ReplaceContentEntryTypeDef(
-    _RequiredReplaceContentEntryTypeDef, _OptionalReplaceContentEntryTypeDef
-):
-    pass
-
-
 SetFileModeEntryTypeDef = TypedDict(
     "SetFileModeEntryTypeDef",
     {
         "filePath": str,
         "fileMode": FileModeTypeEnumType,
     },
 )
@@ -1497,42 +1477,33 @@
 
 class SourceFileSpecifierTypeDef(
     _RequiredSourceFileSpecifierTypeDef, _OptionalSourceFileSpecifierTypeDef
 ):
     pass
 
 
-_RequiredPutFileInputRequestTypeDef = TypedDict(
-    "_RequiredPutFileInputRequestTypeDef",
+ReactionValueFormatsTypeDef = TypedDict(
+    "ReactionValueFormatsTypeDef",
     {
-        "repositoryName": str,
-        "branchName": str,
-        "fileContent": Union[str, bytes, IO[Any], StreamingBody],
-        "filePath": str,
+        "emoji": str,
+        "shortCode": str,
+        "unicode": str,
     },
+    total=False,
 )
-_OptionalPutFileInputRequestTypeDef = TypedDict(
-    "_OptionalPutFileInputRequestTypeDef",
+
+RepositoryTriggerExecutionFailureTypeDef = TypedDict(
+    "RepositoryTriggerExecutionFailureTypeDef",
     {
-        "fileMode": FileModeTypeEnumType,
-        "parentCommitId": str,
-        "commitMessage": str,
-        "name": str,
-        "email": str,
+        "trigger": str,
+        "failureMessage": str,
     },
     total=False,
 )
 
-
-class PutFileInputRequestTypeDef(
-    _RequiredPutFileInputRequestTypeDef, _OptionalPutFileInputRequestTypeDef
-):
-    pass
-
-
 _RequiredRepositoryTriggerTypeDef = TypedDict(
     "_RequiredRepositoryTriggerTypeDef",
     {
         "name": str,
         "destinationArn": str,
         "events": Sequence[RepositoryTriggerEventEnumType],
     },
@@ -1549,33 +1520,14 @@
 
 class RepositoryTriggerTypeDef(
     _RequiredRepositoryTriggerTypeDef, _OptionalRepositoryTriggerTypeDef
 ):
     pass
 
 
-ReactionValueFormatsTypeDef = TypedDict(
-    "ReactionValueFormatsTypeDef",
-    {
-        "emoji": str,
-        "shortCode": str,
-        "unicode": str,
-    },
-    total=False,
-)
-
-RepositoryTriggerExecutionFailureTypeDef = TypedDict(
-    "RepositoryTriggerExecutionFailureTypeDef",
-    {
-        "trigger": str,
-        "failureMessage": str,
-    },
-    total=False,
-)
-
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -2044,14 +1996,65 @@
         "beforeBlob": BlobMetadataTypeDef,
         "afterBlob": BlobMetadataTypeDef,
         "changeType": ChangeTypeEnumType,
     },
     total=False,
 )
 
+_RequiredPutFileInputRequestTypeDef = TypedDict(
+    "_RequiredPutFileInputRequestTypeDef",
+    {
+        "repositoryName": str,
+        "branchName": str,
+        "fileContent": BlobTypeDef,
+        "filePath": str,
+    },
+)
+_OptionalPutFileInputRequestTypeDef = TypedDict(
+    "_OptionalPutFileInputRequestTypeDef",
+    {
+        "fileMode": FileModeTypeEnumType,
+        "parentCommitId": str,
+        "commitMessage": str,
+        "name": str,
+        "email": str,
+    },
+    total=False,
+)
+
+
+class PutFileInputRequestTypeDef(
+    _RequiredPutFileInputRequestTypeDef, _OptionalPutFileInputRequestTypeDef
+):
+    pass
+
+
+_RequiredReplaceContentEntryTypeDef = TypedDict(
+    "_RequiredReplaceContentEntryTypeDef",
+    {
+        "filePath": str,
+        "replacementType": ReplacementTypeEnumType,
+    },
+)
+_OptionalReplaceContentEntryTypeDef = TypedDict(
+    "_OptionalReplaceContentEntryTypeDef",
+    {
+        "content": BlobTypeDef,
+        "fileMode": FileModeTypeEnumType,
+    },
+    total=False,
+)
+
+
+class ReplaceContentEntryTypeDef(
+    _RequiredReplaceContentEntryTypeDef, _OptionalReplaceContentEntryTypeDef
+):
+    pass
+
+
 DeleteBranchOutputTypeDef = TypedDict(
     "DeleteBranchOutputTypeDef",
     {
         "deletedBranch": BranchInfoTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2234,24 +2237,14 @@
         "fileModeConflict": bool,
         "objectTypeConflict": bool,
         "mergeOperations": MergeOperationsTypeDef,
     },
     total=False,
 )
 
-ConflictResolutionTypeDef = TypedDict(
-    "ConflictResolutionTypeDef",
-    {
-        "replaceContents": Sequence[ReplaceContentEntryTypeDef],
-        "deleteFiles": Sequence[DeleteFileEntryTypeDef],
-        "setFileModes": Sequence[SetFileModeEntryTypeDef],
-    },
-    total=False,
-)
-
 CreateCommitOutputTypeDef = TypedDict(
     "CreateCommitOutputTypeDef",
     {
         "commitId": str,
         "treeId": str,
         "filesAdded": List[FileMetadataTypeDef],
         "filesUpdated": List[FileMetadataTypeDef],
@@ -2519,41 +2512,25 @@
         "filePath": str,
     },
 )
 _OptionalPutFileEntryTypeDef = TypedDict(
     "_OptionalPutFileEntryTypeDef",
     {
         "fileMode": FileModeTypeEnumType,
-        "fileContent": Union[str, bytes, IO[Any], StreamingBody],
+        "fileContent": BlobTypeDef,
         "sourceFile": SourceFileSpecifierTypeDef,
     },
     total=False,
 )
 
 
 class PutFileEntryTypeDef(_RequiredPutFileEntryTypeDef, _OptionalPutFileEntryTypeDef):
     pass
 
 
-PutRepositoryTriggersInputRequestTypeDef = TypedDict(
-    "PutRepositoryTriggersInputRequestTypeDef",
-    {
-        "repositoryName": str,
-        "triggers": Sequence[Union[RepositoryTriggerTypeDef, RepositoryTriggerOutputTypeDef]],
-    },
-)
-
-TestRepositoryTriggersInputRequestTypeDef = TypedDict(
-    "TestRepositoryTriggersInputRequestTypeDef",
-    {
-        "repositoryName": str,
-        "triggers": Sequence[Union[RepositoryTriggerTypeDef, RepositoryTriggerOutputTypeDef]],
-    },
-)
-
 ReactionForCommentTypeDef = TypedDict(
     "ReactionForCommentTypeDef",
     {
         "reaction": ReactionValueFormatsTypeDef,
         "reactionUsers": List[str],
         "reactionsFromDeletedUsersCount": int,
     },
@@ -2565,14 +2542,15 @@
     {
         "successfulExecutions": List[str],
         "failedExecutions": List[RepositoryTriggerExecutionFailureTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+RepositoryTriggerUnionTypeDef = Union[RepositoryTriggerTypeDef, RepositoryTriggerOutputTypeDef]
 CreatePullRequestApprovalRuleOutputTypeDef = TypedDict(
     "CreatePullRequestApprovalRuleOutputTypeDef",
     {
         "approvalRule": ApprovalRuleTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2590,14 +2568,24 @@
     {
         "differences": List[DifferenceTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ConflictResolutionTypeDef = TypedDict(
+    "ConflictResolutionTypeDef",
+    {
+        "replaceContents": Sequence[ReplaceContentEntryTypeDef],
+        "deleteFiles": Sequence[DeleteFileEntryTypeDef],
+        "setFileModes": Sequence[SetFileModeEntryTypeDef],
+    },
+    total=False,
+)
+
 GetCommentsForComparedCommitOutputTypeDef = TypedDict(
     "GetCommentsForComparedCommitOutputTypeDef",
     {
         "commentsForComparedCommitData": List[CommentsForComparedCommitTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2638,14 +2626,130 @@
         "baseCommitId": str,
         "conflictMetadataList": List[ConflictMetadataTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ConflictTypeDef = TypedDict(
+    "ConflictTypeDef",
+    {
+        "conflictMetadata": ConflictMetadataTypeDef,
+        "mergeHunks": List[MergeHunkTypeDef],
+    },
+    total=False,
+)
+
+DescribeMergeConflictsOutputTypeDef = TypedDict(
+    "DescribeMergeConflictsOutputTypeDef",
+    {
+        "conflictMetadata": ConflictMetadataTypeDef,
+        "mergeHunks": List[MergeHunkTypeDef],
+        "nextToken": str,
+        "destinationCommitId": str,
+        "sourceCommitId": str,
+        "baseCommitId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PullRequestEventTypeDef = TypedDict(
+    "PullRequestEventTypeDef",
+    {
+        "pullRequestId": str,
+        "eventDate": datetime,
+        "pullRequestEventType": PullRequestEventTypeType,
+        "actorArn": str,
+        "pullRequestCreatedEventMetadata": PullRequestCreatedEventMetadataTypeDef,
+        "pullRequestStatusChangedEventMetadata": PullRequestStatusChangedEventMetadataTypeDef,
+        "pullRequestSourceReferenceUpdatedEventMetadata": (
+            PullRequestSourceReferenceUpdatedEventMetadataTypeDef
+        ),
+        "pullRequestMergedStateChangedEventMetadata": (
+            PullRequestMergedStateChangedEventMetadataTypeDef
+        ),
+        "approvalRuleEventMetadata": ApprovalRuleEventMetadataTypeDef,
+        "approvalStateChangedEventMetadata": ApprovalStateChangedEventMetadataTypeDef,
+        "approvalRuleOverriddenEventMetadata": ApprovalRuleOverriddenEventMetadataTypeDef,
+    },
+    total=False,
+)
+
+PullRequestTypeDef = TypedDict(
+    "PullRequestTypeDef",
+    {
+        "pullRequestId": str,
+        "title": str,
+        "description": str,
+        "lastActivityDate": datetime,
+        "creationDate": datetime,
+        "pullRequestStatus": PullRequestStatusEnumType,
+        "authorArn": str,
+        "pullRequestTargets": List[PullRequestTargetTypeDef],
+        "clientRequestToken": str,
+        "revisionId": str,
+        "approvalRules": List[ApprovalRuleTypeDef],
+    },
+    total=False,
+)
+
+_RequiredCreateCommitInputRequestTypeDef = TypedDict(
+    "_RequiredCreateCommitInputRequestTypeDef",
+    {
+        "repositoryName": str,
+        "branchName": str,
+    },
+)
+_OptionalCreateCommitInputRequestTypeDef = TypedDict(
+    "_OptionalCreateCommitInputRequestTypeDef",
+    {
+        "parentCommitId": str,
+        "authorName": str,
+        "email": str,
+        "commitMessage": str,
+        "keepEmptyFolders": bool,
+        "putFiles": Sequence[PutFileEntryTypeDef],
+        "deleteFiles": Sequence[DeleteFileEntryTypeDef],
+        "setFileModes": Sequence[SetFileModeEntryTypeDef],
+    },
+    total=False,
+)
+
+
+class CreateCommitInputRequestTypeDef(
+    _RequiredCreateCommitInputRequestTypeDef, _OptionalCreateCommitInputRequestTypeDef
+):
+    pass
+
+
+GetCommentReactionsOutputTypeDef = TypedDict(
+    "GetCommentReactionsOutputTypeDef",
+    {
+        "reactionsForComment": List[ReactionForCommentTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutRepositoryTriggersInputRequestTypeDef = TypedDict(
+    "PutRepositoryTriggersInputRequestTypeDef",
+    {
+        "repositoryName": str,
+        "triggers": Sequence[RepositoryTriggerUnionTypeDef],
+    },
+)
+
+TestRepositoryTriggersInputRequestTypeDef = TypedDict(
+    "TestRepositoryTriggersInputRequestTypeDef",
+    {
+        "repositoryName": str,
+        "triggers": Sequence[RepositoryTriggerUnionTypeDef],
+    },
+)
+
 _RequiredCreateUnreferencedMergeCommitInputRequestTypeDef = TypedDict(
     "_RequiredCreateUnreferencedMergeCommitInputRequestTypeDef",
     {
         "repositoryName": str,
         "sourceCommitSpecifier": str,
         "destinationCommitSpecifier": str,
         "mergeOption": MergeOptionTypeEnumType,
@@ -2791,114 +2895,14 @@
 class MergePullRequestByThreeWayInputRequestTypeDef(
     _RequiredMergePullRequestByThreeWayInputRequestTypeDef,
     _OptionalMergePullRequestByThreeWayInputRequestTypeDef,
 ):
     pass
 
 
-ConflictTypeDef = TypedDict(
-    "ConflictTypeDef",
-    {
-        "conflictMetadata": ConflictMetadataTypeDef,
-        "mergeHunks": List[MergeHunkTypeDef],
-    },
-    total=False,
-)
-
-DescribeMergeConflictsOutputTypeDef = TypedDict(
-    "DescribeMergeConflictsOutputTypeDef",
-    {
-        "conflictMetadata": ConflictMetadataTypeDef,
-        "mergeHunks": List[MergeHunkTypeDef],
-        "nextToken": str,
-        "destinationCommitId": str,
-        "sourceCommitId": str,
-        "baseCommitId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PullRequestEventTypeDef = TypedDict(
-    "PullRequestEventTypeDef",
-    {
-        "pullRequestId": str,
-        "eventDate": datetime,
-        "pullRequestEventType": PullRequestEventTypeType,
-        "actorArn": str,
-        "pullRequestCreatedEventMetadata": PullRequestCreatedEventMetadataTypeDef,
-        "pullRequestStatusChangedEventMetadata": PullRequestStatusChangedEventMetadataTypeDef,
-        "pullRequestSourceReferenceUpdatedEventMetadata": (
-            PullRequestSourceReferenceUpdatedEventMetadataTypeDef
-        ),
-        "pullRequestMergedStateChangedEventMetadata": (
-            PullRequestMergedStateChangedEventMetadataTypeDef
-        ),
-        "approvalRuleEventMetadata": ApprovalRuleEventMetadataTypeDef,
-        "approvalStateChangedEventMetadata": ApprovalStateChangedEventMetadataTypeDef,
-        "approvalRuleOverriddenEventMetadata": ApprovalRuleOverriddenEventMetadataTypeDef,
-    },
-    total=False,
-)
-
-PullRequestTypeDef = TypedDict(
-    "PullRequestTypeDef",
-    {
-        "pullRequestId": str,
-        "title": str,
-        "description": str,
-        "lastActivityDate": datetime,
-        "creationDate": datetime,
-        "pullRequestStatus": PullRequestStatusEnumType,
-        "authorArn": str,
-        "pullRequestTargets": List[PullRequestTargetTypeDef],
-        "clientRequestToken": str,
-        "revisionId": str,
-        "approvalRules": List[ApprovalRuleTypeDef],
-    },
-    total=False,
-)
-
-_RequiredCreateCommitInputRequestTypeDef = TypedDict(
-    "_RequiredCreateCommitInputRequestTypeDef",
-    {
-        "repositoryName": str,
-        "branchName": str,
-    },
-)
-_OptionalCreateCommitInputRequestTypeDef = TypedDict(
-    "_OptionalCreateCommitInputRequestTypeDef",
-    {
-        "parentCommitId": str,
-        "authorName": str,
-        "email": str,
-        "commitMessage": str,
-        "keepEmptyFolders": bool,
-        "putFiles": Sequence[PutFileEntryTypeDef],
-        "deleteFiles": Sequence[DeleteFileEntryTypeDef],
-        "setFileModes": Sequence[SetFileModeEntryTypeDef],
-    },
-    total=False,
-)
-
-
-class CreateCommitInputRequestTypeDef(
-    _RequiredCreateCommitInputRequestTypeDef, _OptionalCreateCommitInputRequestTypeDef
-):
-    pass
-
-
-GetCommentReactionsOutputTypeDef = TypedDict(
-    "GetCommentReactionsOutputTypeDef",
-    {
-        "reactionsForComment": List[ReactionForCommentTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 BatchDescribeMergeConflictsOutputTypeDef = TypedDict(
     "BatchDescribeMergeConflictsOutputTypeDef",
     {
         "conflicts": List[ConflictTypeDef],
         "nextToken": str,
         "errors": List[BatchDescribeMergeConflictsErrorTypeDef],
         "destinationCommitId": str,
```

### Comparing `mypy-boto3-codecommit-1.28.15.post1/mypy_boto3_codecommit/type_defs.pyi` & `mypy-boto3-codecommit-1.28.16/mypy_boto3_codecommit/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_codecommit.type_defs import ApprovalRuleEventMetadataTypeDef
 
-    data: ApprovalRuleEventMetadataTypeDef = {...}
+    data: ApprovalRuleEventMetadataTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -56,25 +56,25 @@
     "BatchDisassociateApprovalRuleTemplateFromRepositoriesErrorTypeDef",
     "BatchDisassociateApprovalRuleTemplateFromRepositoriesInputRequestTypeDef",
     "BatchGetCommitsErrorTypeDef",
     "BatchGetCommitsInputRequestTypeDef",
     "BatchGetRepositoriesInputRequestTypeDef",
     "RepositoryMetadataTypeDef",
     "BlobMetadataTypeDef",
+    "BlobTypeDef",
     "BranchInfoTypeDef",
     "CommentTypeDef",
     "LocationTypeDef",
     "UserInfoTypeDef",
     "FileModesTypeDef",
     "FileSizesTypeDef",
     "IsBinaryFileTypeDef",
     "MergeOperationsTypeDef",
     "ObjectTypesTypeDef",
     "DeleteFileEntryTypeDef",
-    "ReplaceContentEntryTypeDef",
     "SetFileModeEntryTypeDef",
     "CreateApprovalRuleTemplateInputRequestTypeDef",
     "CreateBranchInputRequestTypeDef",
     "FileMetadataTypeDef",
     "CreatePullRequestApprovalRuleInputRequestTypeDef",
     "TargetTypeDef",
     "CreateRepositoryInputRequestTypeDef",
@@ -129,18 +129,17 @@
     "OverridePullRequestApprovalRulesInputRequestTypeDef",
     "PostCommentReplyInputRequestTypeDef",
     "PullRequestCreatedEventMetadataTypeDef",
     "PullRequestSourceReferenceUpdatedEventMetadataTypeDef",
     "PullRequestStatusChangedEventMetadataTypeDef",
     "PutCommentReactionInputRequestTypeDef",
     "SourceFileSpecifierTypeDef",
-    "PutFileInputRequestTypeDef",
-    "RepositoryTriggerTypeDef",
     "ReactionValueFormatsTypeDef",
     "RepositoryTriggerExecutionFailureTypeDef",
+    "RepositoryTriggerTypeDef",
     "TagResourceInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateApprovalRuleTemplateContentInputRequestTypeDef",
     "UpdateApprovalRuleTemplateDescriptionInputRequestTypeDef",
     "UpdateApprovalRuleTemplateNameInputRequestTypeDef",
     "UpdateCommentInputRequestTypeDef",
     "UpdateDefaultBranchInputRequestTypeDef",
@@ -182,29 +181,30 @@
     "UpdateApprovalRuleTemplateDescriptionOutputTypeDef",
     "UpdateApprovalRuleTemplateNameOutputTypeDef",
     "BatchDisassociateApprovalRuleTemplateFromRepositoriesOutputTypeDef",
     "BatchGetRepositoriesOutputTypeDef",
     "CreateRepositoryOutputTypeDef",
     "GetRepositoryOutputTypeDef",
     "DifferenceTypeDef",
+    "PutFileInputRequestTypeDef",
+    "ReplaceContentEntryTypeDef",
     "DeleteBranchOutputTypeDef",
     "GetBranchOutputTypeDef",
     "DeleteCommentContentOutputTypeDef",
     "GetCommentOutputTypeDef",
     "PostCommentReplyOutputTypeDef",
     "UpdateCommentOutputTypeDef",
     "CommentsForComparedCommitTypeDef",
     "CommentsForPullRequestTypeDef",
     "PostCommentForComparedCommitInputRequestTypeDef",
     "PostCommentForComparedCommitOutputTypeDef",
     "PostCommentForPullRequestInputRequestTypeDef",
     "PostCommentForPullRequestOutputTypeDef",
     "CommitTypeDef",
     "ConflictMetadataTypeDef",
-    "ConflictResolutionTypeDef",
     "CreateCommitOutputTypeDef",
     "CreatePullRequestInputRequestTypeDef",
     "DescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef",
     "GetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef",
     "GetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef",
     "GetDifferencesInputGetDifferencesPaginateTypeDef",
     "ListBranchesInputListBranchesPaginateTypeDef",
@@ -214,37 +214,39 @@
     "GetFolderOutputTypeDef",
     "GetRepositoryTriggersOutputTypeDef",
     "ListRepositoriesOutputTypeDef",
     "MergeHunkTypeDef",
     "PullRequestMergedStateChangedEventMetadataTypeDef",
     "PullRequestTargetTypeDef",
     "PutFileEntryTypeDef",
-    "PutRepositoryTriggersInputRequestTypeDef",
-    "TestRepositoryTriggersInputRequestTypeDef",
     "ReactionForCommentTypeDef",
     "TestRepositoryTriggersOutputTypeDef",
+    "RepositoryTriggerUnionTypeDef",
     "CreatePullRequestApprovalRuleOutputTypeDef",
     "UpdatePullRequestApprovalRuleContentOutputTypeDef",
     "GetDifferencesOutputTypeDef",
+    "ConflictResolutionTypeDef",
     "GetCommentsForComparedCommitOutputTypeDef",
     "GetCommentsForPullRequestOutputTypeDef",
     "BatchGetCommitsOutputTypeDef",
     "GetCommitOutputTypeDef",
     "GetMergeConflictsOutputTypeDef",
-    "CreateUnreferencedMergeCommitInputRequestTypeDef",
-    "MergeBranchesBySquashInputRequestTypeDef",
-    "MergeBranchesByThreeWayInputRequestTypeDef",
-    "MergePullRequestBySquashInputRequestTypeDef",
-    "MergePullRequestByThreeWayInputRequestTypeDef",
     "ConflictTypeDef",
     "DescribeMergeConflictsOutputTypeDef",
     "PullRequestEventTypeDef",
     "PullRequestTypeDef",
     "CreateCommitInputRequestTypeDef",
     "GetCommentReactionsOutputTypeDef",
+    "PutRepositoryTriggersInputRequestTypeDef",
+    "TestRepositoryTriggersInputRequestTypeDef",
+    "CreateUnreferencedMergeCommitInputRequestTypeDef",
+    "MergeBranchesBySquashInputRequestTypeDef",
+    "MergeBranchesByThreeWayInputRequestTypeDef",
+    "MergePullRequestBySquashInputRequestTypeDef",
+    "MergePullRequestByThreeWayInputRequestTypeDef",
     "BatchDescribeMergeConflictsOutputTypeDef",
     "DescribePullRequestEventsOutputTypeDef",
     "CreatePullRequestOutputTypeDef",
     "GetPullRequestOutputTypeDef",
     "MergePullRequestByFastForwardOutputTypeDef",
     "MergePullRequestBySquashOutputTypeDef",
     "MergePullRequestByThreeWayOutputTypeDef",
@@ -454,14 +456,15 @@
         "blobId": str,
         "path": str,
         "mode": str,
     },
     total=False,
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 BranchInfoTypeDef = TypedDict(
     "BranchInfoTypeDef",
     {
         "branchName": str,
         "commitId": str,
     },
     total=False,
@@ -556,35 +559,14 @@
 DeleteFileEntryTypeDef = TypedDict(
     "DeleteFileEntryTypeDef",
     {
         "filePath": str,
     },
 )
 
-_RequiredReplaceContentEntryTypeDef = TypedDict(
-    "_RequiredReplaceContentEntryTypeDef",
-    {
-        "filePath": str,
-        "replacementType": ReplacementTypeEnumType,
-    },
-)
-_OptionalReplaceContentEntryTypeDef = TypedDict(
-    "_OptionalReplaceContentEntryTypeDef",
-    {
-        "content": Union[str, bytes, IO[Any], StreamingBody],
-        "fileMode": FileModeTypeEnumType,
-    },
-    total=False,
-)
-
-class ReplaceContentEntryTypeDef(
-    _RequiredReplaceContentEntryTypeDef, _OptionalReplaceContentEntryTypeDef
-):
-    pass
-
 SetFileModeEntryTypeDef = TypedDict(
     "SetFileModeEntryTypeDef",
     {
         "filePath": str,
         "fileMode": FileModeTypeEnumType,
     },
 )
@@ -1442,40 +1424,33 @@
 )
 
 class SourceFileSpecifierTypeDef(
     _RequiredSourceFileSpecifierTypeDef, _OptionalSourceFileSpecifierTypeDef
 ):
     pass
 
-_RequiredPutFileInputRequestTypeDef = TypedDict(
-    "_RequiredPutFileInputRequestTypeDef",
+ReactionValueFormatsTypeDef = TypedDict(
+    "ReactionValueFormatsTypeDef",
     {
-        "repositoryName": str,
-        "branchName": str,
-        "fileContent": Union[str, bytes, IO[Any], StreamingBody],
-        "filePath": str,
+        "emoji": str,
+        "shortCode": str,
+        "unicode": str,
     },
+    total=False,
 )
-_OptionalPutFileInputRequestTypeDef = TypedDict(
-    "_OptionalPutFileInputRequestTypeDef",
+
+RepositoryTriggerExecutionFailureTypeDef = TypedDict(
+    "RepositoryTriggerExecutionFailureTypeDef",
     {
-        "fileMode": FileModeTypeEnumType,
-        "parentCommitId": str,
-        "commitMessage": str,
-        "name": str,
-        "email": str,
+        "trigger": str,
+        "failureMessage": str,
     },
     total=False,
 )
 
-class PutFileInputRequestTypeDef(
-    _RequiredPutFileInputRequestTypeDef, _OptionalPutFileInputRequestTypeDef
-):
-    pass
-
 _RequiredRepositoryTriggerTypeDef = TypedDict(
     "_RequiredRepositoryTriggerTypeDef",
     {
         "name": str,
         "destinationArn": str,
         "events": Sequence[RepositoryTriggerEventEnumType],
     },
@@ -1490,33 +1465,14 @@
 )
 
 class RepositoryTriggerTypeDef(
     _RequiredRepositoryTriggerTypeDef, _OptionalRepositoryTriggerTypeDef
 ):
     pass
 
-ReactionValueFormatsTypeDef = TypedDict(
-    "ReactionValueFormatsTypeDef",
-    {
-        "emoji": str,
-        "shortCode": str,
-        "unicode": str,
-    },
-    total=False,
-)
-
-RepositoryTriggerExecutionFailureTypeDef = TypedDict(
-    "RepositoryTriggerExecutionFailureTypeDef",
-    {
-        "trigger": str,
-        "failureMessage": str,
-    },
-    total=False,
-)
-
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -1979,14 +1935,61 @@
         "beforeBlob": BlobMetadataTypeDef,
         "afterBlob": BlobMetadataTypeDef,
         "changeType": ChangeTypeEnumType,
     },
     total=False,
 )
 
+_RequiredPutFileInputRequestTypeDef = TypedDict(
+    "_RequiredPutFileInputRequestTypeDef",
+    {
+        "repositoryName": str,
+        "branchName": str,
+        "fileContent": BlobTypeDef,
+        "filePath": str,
+    },
+)
+_OptionalPutFileInputRequestTypeDef = TypedDict(
+    "_OptionalPutFileInputRequestTypeDef",
+    {
+        "fileMode": FileModeTypeEnumType,
+        "parentCommitId": str,
+        "commitMessage": str,
+        "name": str,
+        "email": str,
+    },
+    total=False,
+)
+
+class PutFileInputRequestTypeDef(
+    _RequiredPutFileInputRequestTypeDef, _OptionalPutFileInputRequestTypeDef
+):
+    pass
+
+_RequiredReplaceContentEntryTypeDef = TypedDict(
+    "_RequiredReplaceContentEntryTypeDef",
+    {
+        "filePath": str,
+        "replacementType": ReplacementTypeEnumType,
+    },
+)
+_OptionalReplaceContentEntryTypeDef = TypedDict(
+    "_OptionalReplaceContentEntryTypeDef",
+    {
+        "content": BlobTypeDef,
+        "fileMode": FileModeTypeEnumType,
+    },
+    total=False,
+)
+
+class ReplaceContentEntryTypeDef(
+    _RequiredReplaceContentEntryTypeDef, _OptionalReplaceContentEntryTypeDef
+):
+    pass
+
 DeleteBranchOutputTypeDef = TypedDict(
     "DeleteBranchOutputTypeDef",
     {
         "deletedBranch": BranchInfoTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2165,24 +2168,14 @@
         "fileModeConflict": bool,
         "objectTypeConflict": bool,
         "mergeOperations": MergeOperationsTypeDef,
     },
     total=False,
 )
 
-ConflictResolutionTypeDef = TypedDict(
-    "ConflictResolutionTypeDef",
-    {
-        "replaceContents": Sequence[ReplaceContentEntryTypeDef],
-        "deleteFiles": Sequence[DeleteFileEntryTypeDef],
-        "setFileModes": Sequence[SetFileModeEntryTypeDef],
-    },
-    total=False,
-)
-
 CreateCommitOutputTypeDef = TypedDict(
     "CreateCommitOutputTypeDef",
     {
         "commitId": str,
         "treeId": str,
         "filesAdded": List[FileMetadataTypeDef],
         "filesUpdated": List[FileMetadataTypeDef],
@@ -2436,39 +2429,23 @@
         "filePath": str,
     },
 )
 _OptionalPutFileEntryTypeDef = TypedDict(
     "_OptionalPutFileEntryTypeDef",
     {
         "fileMode": FileModeTypeEnumType,
-        "fileContent": Union[str, bytes, IO[Any], StreamingBody],
+        "fileContent": BlobTypeDef,
         "sourceFile": SourceFileSpecifierTypeDef,
     },
     total=False,
 )
 
 class PutFileEntryTypeDef(_RequiredPutFileEntryTypeDef, _OptionalPutFileEntryTypeDef):
     pass
 
-PutRepositoryTriggersInputRequestTypeDef = TypedDict(
-    "PutRepositoryTriggersInputRequestTypeDef",
-    {
-        "repositoryName": str,
-        "triggers": Sequence[Union[RepositoryTriggerTypeDef, RepositoryTriggerOutputTypeDef]],
-    },
-)
-
-TestRepositoryTriggersInputRequestTypeDef = TypedDict(
-    "TestRepositoryTriggersInputRequestTypeDef",
-    {
-        "repositoryName": str,
-        "triggers": Sequence[Union[RepositoryTriggerTypeDef, RepositoryTriggerOutputTypeDef]],
-    },
-)
-
 ReactionForCommentTypeDef = TypedDict(
     "ReactionForCommentTypeDef",
     {
         "reaction": ReactionValueFormatsTypeDef,
         "reactionUsers": List[str],
         "reactionsFromDeletedUsersCount": int,
     },
@@ -2480,14 +2457,15 @@
     {
         "successfulExecutions": List[str],
         "failedExecutions": List[RepositoryTriggerExecutionFailureTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+RepositoryTriggerUnionTypeDef = Union[RepositoryTriggerTypeDef, RepositoryTriggerOutputTypeDef]
 CreatePullRequestApprovalRuleOutputTypeDef = TypedDict(
     "CreatePullRequestApprovalRuleOutputTypeDef",
     {
         "approvalRule": ApprovalRuleTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2505,14 +2483,24 @@
     {
         "differences": List[DifferenceTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ConflictResolutionTypeDef = TypedDict(
+    "ConflictResolutionTypeDef",
+    {
+        "replaceContents": Sequence[ReplaceContentEntryTypeDef],
+        "deleteFiles": Sequence[DeleteFileEntryTypeDef],
+        "setFileModes": Sequence[SetFileModeEntryTypeDef],
+    },
+    total=False,
+)
+
 GetCommentsForComparedCommitOutputTypeDef = TypedDict(
     "GetCommentsForComparedCommitOutputTypeDef",
     {
         "commentsForComparedCommitData": List[CommentsForComparedCommitTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2553,14 +2541,128 @@
         "baseCommitId": str,
         "conflictMetadataList": List[ConflictMetadataTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ConflictTypeDef = TypedDict(
+    "ConflictTypeDef",
+    {
+        "conflictMetadata": ConflictMetadataTypeDef,
+        "mergeHunks": List[MergeHunkTypeDef],
+    },
+    total=False,
+)
+
+DescribeMergeConflictsOutputTypeDef = TypedDict(
+    "DescribeMergeConflictsOutputTypeDef",
+    {
+        "conflictMetadata": ConflictMetadataTypeDef,
+        "mergeHunks": List[MergeHunkTypeDef],
+        "nextToken": str,
+        "destinationCommitId": str,
+        "sourceCommitId": str,
+        "baseCommitId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PullRequestEventTypeDef = TypedDict(
+    "PullRequestEventTypeDef",
+    {
+        "pullRequestId": str,
+        "eventDate": datetime,
+        "pullRequestEventType": PullRequestEventTypeType,
+        "actorArn": str,
+        "pullRequestCreatedEventMetadata": PullRequestCreatedEventMetadataTypeDef,
+        "pullRequestStatusChangedEventMetadata": PullRequestStatusChangedEventMetadataTypeDef,
+        "pullRequestSourceReferenceUpdatedEventMetadata": (
+            PullRequestSourceReferenceUpdatedEventMetadataTypeDef
+        ),
+        "pullRequestMergedStateChangedEventMetadata": (
+            PullRequestMergedStateChangedEventMetadataTypeDef
+        ),
+        "approvalRuleEventMetadata": ApprovalRuleEventMetadataTypeDef,
+        "approvalStateChangedEventMetadata": ApprovalStateChangedEventMetadataTypeDef,
+        "approvalRuleOverriddenEventMetadata": ApprovalRuleOverriddenEventMetadataTypeDef,
+    },
+    total=False,
+)
+
+PullRequestTypeDef = TypedDict(
+    "PullRequestTypeDef",
+    {
+        "pullRequestId": str,
+        "title": str,
+        "description": str,
+        "lastActivityDate": datetime,
+        "creationDate": datetime,
+        "pullRequestStatus": PullRequestStatusEnumType,
+        "authorArn": str,
+        "pullRequestTargets": List[PullRequestTargetTypeDef],
+        "clientRequestToken": str,
+        "revisionId": str,
+        "approvalRules": List[ApprovalRuleTypeDef],
+    },
+    total=False,
+)
+
+_RequiredCreateCommitInputRequestTypeDef = TypedDict(
+    "_RequiredCreateCommitInputRequestTypeDef",
+    {
+        "repositoryName": str,
+        "branchName": str,
+    },
+)
+_OptionalCreateCommitInputRequestTypeDef = TypedDict(
+    "_OptionalCreateCommitInputRequestTypeDef",
+    {
+        "parentCommitId": str,
+        "authorName": str,
+        "email": str,
+        "commitMessage": str,
+        "keepEmptyFolders": bool,
+        "putFiles": Sequence[PutFileEntryTypeDef],
+        "deleteFiles": Sequence[DeleteFileEntryTypeDef],
+        "setFileModes": Sequence[SetFileModeEntryTypeDef],
+    },
+    total=False,
+)
+
+class CreateCommitInputRequestTypeDef(
+    _RequiredCreateCommitInputRequestTypeDef, _OptionalCreateCommitInputRequestTypeDef
+):
+    pass
+
+GetCommentReactionsOutputTypeDef = TypedDict(
+    "GetCommentReactionsOutputTypeDef",
+    {
+        "reactionsForComment": List[ReactionForCommentTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutRepositoryTriggersInputRequestTypeDef = TypedDict(
+    "PutRepositoryTriggersInputRequestTypeDef",
+    {
+        "repositoryName": str,
+        "triggers": Sequence[RepositoryTriggerUnionTypeDef],
+    },
+)
+
+TestRepositoryTriggersInputRequestTypeDef = TypedDict(
+    "TestRepositoryTriggersInputRequestTypeDef",
+    {
+        "repositoryName": str,
+        "triggers": Sequence[RepositoryTriggerUnionTypeDef],
+    },
+)
+
 _RequiredCreateUnreferencedMergeCommitInputRequestTypeDef = TypedDict(
     "_RequiredCreateUnreferencedMergeCommitInputRequestTypeDef",
     {
         "repositoryName": str,
         "sourceCommitSpecifier": str,
         "destinationCommitSpecifier": str,
         "mergeOption": MergeOptionTypeEnumType,
@@ -2696,112 +2798,14 @@
 
 class MergePullRequestByThreeWayInputRequestTypeDef(
     _RequiredMergePullRequestByThreeWayInputRequestTypeDef,
     _OptionalMergePullRequestByThreeWayInputRequestTypeDef,
 ):
     pass
 
-ConflictTypeDef = TypedDict(
-    "ConflictTypeDef",
-    {
-        "conflictMetadata": ConflictMetadataTypeDef,
-        "mergeHunks": List[MergeHunkTypeDef],
-    },
-    total=False,
-)
-
-DescribeMergeConflictsOutputTypeDef = TypedDict(
-    "DescribeMergeConflictsOutputTypeDef",
-    {
-        "conflictMetadata": ConflictMetadataTypeDef,
-        "mergeHunks": List[MergeHunkTypeDef],
-        "nextToken": str,
-        "destinationCommitId": str,
-        "sourceCommitId": str,
-        "baseCommitId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PullRequestEventTypeDef = TypedDict(
-    "PullRequestEventTypeDef",
-    {
-        "pullRequestId": str,
-        "eventDate": datetime,
-        "pullRequestEventType": PullRequestEventTypeType,
-        "actorArn": str,
-        "pullRequestCreatedEventMetadata": PullRequestCreatedEventMetadataTypeDef,
-        "pullRequestStatusChangedEventMetadata": PullRequestStatusChangedEventMetadataTypeDef,
-        "pullRequestSourceReferenceUpdatedEventMetadata": (
-            PullRequestSourceReferenceUpdatedEventMetadataTypeDef
-        ),
-        "pullRequestMergedStateChangedEventMetadata": (
-            PullRequestMergedStateChangedEventMetadataTypeDef
-        ),
-        "approvalRuleEventMetadata": ApprovalRuleEventMetadataTypeDef,
-        "approvalStateChangedEventMetadata": ApprovalStateChangedEventMetadataTypeDef,
-        "approvalRuleOverriddenEventMetadata": ApprovalRuleOverriddenEventMetadataTypeDef,
-    },
-    total=False,
-)
-
-PullRequestTypeDef = TypedDict(
-    "PullRequestTypeDef",
-    {
-        "pullRequestId": str,
-        "title": str,
-        "description": str,
-        "lastActivityDate": datetime,
-        "creationDate": datetime,
-        "pullRequestStatus": PullRequestStatusEnumType,
-        "authorArn": str,
-        "pullRequestTargets": List[PullRequestTargetTypeDef],
-        "clientRequestToken": str,
-        "revisionId": str,
-        "approvalRules": List[ApprovalRuleTypeDef],
-    },
-    total=False,
-)
-
-_RequiredCreateCommitInputRequestTypeDef = TypedDict(
-    "_RequiredCreateCommitInputRequestTypeDef",
-    {
-        "repositoryName": str,
-        "branchName": str,
-    },
-)
-_OptionalCreateCommitInputRequestTypeDef = TypedDict(
-    "_OptionalCreateCommitInputRequestTypeDef",
-    {
-        "parentCommitId": str,
-        "authorName": str,
-        "email": str,
-        "commitMessage": str,
-        "keepEmptyFolders": bool,
-        "putFiles": Sequence[PutFileEntryTypeDef],
-        "deleteFiles": Sequence[DeleteFileEntryTypeDef],
-        "setFileModes": Sequence[SetFileModeEntryTypeDef],
-    },
-    total=False,
-)
-
-class CreateCommitInputRequestTypeDef(
-    _RequiredCreateCommitInputRequestTypeDef, _OptionalCreateCommitInputRequestTypeDef
-):
-    pass
-
-GetCommentReactionsOutputTypeDef = TypedDict(
-    "GetCommentReactionsOutputTypeDef",
-    {
-        "reactionsForComment": List[ReactionForCommentTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 BatchDescribeMergeConflictsOutputTypeDef = TypedDict(
     "BatchDescribeMergeConflictsOutputTypeDef",
     {
         "conflicts": List[ConflictTypeDef],
         "nextToken": str,
         "errors": List[BatchDescribeMergeConflictsErrorTypeDef],
         "destinationCommitId": str,
```

### Comparing `mypy-boto3-codecommit-1.28.15.post1/mypy_boto3_codecommit.egg-info/PKG-INFO` & `mypy-boto3-codecommit-1.28.16/mypy_boto3_codecommit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-codecommit
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.CodeCommit 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.CodeCommit 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 codecommit type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 codecommit type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codecommit.svg?color=blue)](https://pypi.org/project/mypy-boto3-codecommit)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codecommit)](https://pepy.tech/project/mypy-boto3-codecommit)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeCommit 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit)
+[boto3.CodeCommit 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit)
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
 [mypy-boto3-codecommit docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit/).
 
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
@@ -350,20 +350,20 @@
 )
 
 
 def check_value(value: ApprovalStateType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_codecommit.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_codecommit.type_defs import (
     ApprovalRuleEventMetadataTypeDef,
     ApprovalRuleOverriddenEventMetadataTypeDef,
     ApprovalRuleTemplateTypeDef,
     OriginApprovalRuleTemplateTypeDef,
@@ -378,25 +378,25 @@
     BatchDisassociateApprovalRuleTemplateFromRepositoriesErrorTypeDef,
     BatchDisassociateApprovalRuleTemplateFromRepositoriesInputRequestTypeDef,
     BatchGetCommitsErrorTypeDef,
     BatchGetCommitsInputRequestTypeDef,
     BatchGetRepositoriesInputRequestTypeDef,
     RepositoryMetadataTypeDef,
     BlobMetadataTypeDef,
+    BlobTypeDef,
     BranchInfoTypeDef,
     CommentTypeDef,
     LocationTypeDef,
     UserInfoTypeDef,
     FileModesTypeDef,
     FileSizesTypeDef,
     IsBinaryFileTypeDef,
     MergeOperationsTypeDef,
     ObjectTypesTypeDef,
     DeleteFileEntryTypeDef,
-    ReplaceContentEntryTypeDef,
     SetFileModeEntryTypeDef,
     CreateApprovalRuleTemplateInputRequestTypeDef,
     CreateBranchInputRequestTypeDef,
     FileMetadataTypeDef,
     CreatePullRequestApprovalRuleInputRequestTypeDef,
     TargetTypeDef,
     CreateRepositoryInputRequestTypeDef,
@@ -451,18 +451,17 @@
     OverridePullRequestApprovalRulesInputRequestTypeDef,
     PostCommentReplyInputRequestTypeDef,
     PullRequestCreatedEventMetadataTypeDef,
     PullRequestSourceReferenceUpdatedEventMetadataTypeDef,
     PullRequestStatusChangedEventMetadataTypeDef,
     PutCommentReactionInputRequestTypeDef,
     SourceFileSpecifierTypeDef,
-    PutFileInputRequestTypeDef,
-    RepositoryTriggerTypeDef,
     ReactionValueFormatsTypeDef,
     RepositoryTriggerExecutionFailureTypeDef,
+    RepositoryTriggerTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateApprovalRuleTemplateContentInputRequestTypeDef,
     UpdateApprovalRuleTemplateDescriptionInputRequestTypeDef,
     UpdateApprovalRuleTemplateNameInputRequestTypeDef,
     UpdateCommentInputRequestTypeDef,
     UpdateDefaultBranchInputRequestTypeDef,
@@ -504,29 +503,30 @@
     UpdateApprovalRuleTemplateDescriptionOutputTypeDef,
     UpdateApprovalRuleTemplateNameOutputTypeDef,
     BatchDisassociateApprovalRuleTemplateFromRepositoriesOutputTypeDef,
     BatchGetRepositoriesOutputTypeDef,
     CreateRepositoryOutputTypeDef,
     GetRepositoryOutputTypeDef,
     DifferenceTypeDef,
+    PutFileInputRequestTypeDef,
+    ReplaceContentEntryTypeDef,
     DeleteBranchOutputTypeDef,
     GetBranchOutputTypeDef,
     DeleteCommentContentOutputTypeDef,
     GetCommentOutputTypeDef,
     PostCommentReplyOutputTypeDef,
     UpdateCommentOutputTypeDef,
     CommentsForComparedCommitTypeDef,
     CommentsForPullRequestTypeDef,
     PostCommentForComparedCommitInputRequestTypeDef,
     PostCommentForComparedCommitOutputTypeDef,
     PostCommentForPullRequestInputRequestTypeDef,
     PostCommentForPullRequestOutputTypeDef,
     CommitTypeDef,
     ConflictMetadataTypeDef,
-    ConflictResolutionTypeDef,
     CreateCommitOutputTypeDef,
     CreatePullRequestInputRequestTypeDef,
     DescribePullRequestEventsInputDescribePullRequestEventsPaginateTypeDef,
     GetCommentsForComparedCommitInputGetCommentsForComparedCommitPaginateTypeDef,
     GetCommentsForPullRequestInputGetCommentsForPullRequestPaginateTypeDef,
     GetDifferencesInputGetDifferencesPaginateTypeDef,
     ListBranchesInputListBranchesPaginateTypeDef,
@@ -536,51 +536,53 @@
     GetFolderOutputTypeDef,
     GetRepositoryTriggersOutputTypeDef,
     ListRepositoriesOutputTypeDef,
     MergeHunkTypeDef,
     PullRequestMergedStateChangedEventMetadataTypeDef,
     PullRequestTargetTypeDef,
     PutFileEntryTypeDef,
-    PutRepositoryTriggersInputRequestTypeDef,
-    TestRepositoryTriggersInputRequestTypeDef,
     ReactionForCommentTypeDef,
     TestRepositoryTriggersOutputTypeDef,
+    RepositoryTriggerUnionTypeDef,
     CreatePullRequestApprovalRuleOutputTypeDef,
     UpdatePullRequestApprovalRuleContentOutputTypeDef,
     GetDifferencesOutputTypeDef,
+    ConflictResolutionTypeDef,
     GetCommentsForComparedCommitOutputTypeDef,
     GetCommentsForPullRequestOutputTypeDef,
     BatchGetCommitsOutputTypeDef,
     GetCommitOutputTypeDef,
     GetMergeConflictsOutputTypeDef,
-    CreateUnreferencedMergeCommitInputRequestTypeDef,
-    MergeBranchesBySquashInputRequestTypeDef,
-    MergeBranchesByThreeWayInputRequestTypeDef,
-    MergePullRequestBySquashInputRequestTypeDef,
-    MergePullRequestByThreeWayInputRequestTypeDef,
     ConflictTypeDef,
     DescribeMergeConflictsOutputTypeDef,
     PullRequestEventTypeDef,
     PullRequestTypeDef,
     CreateCommitInputRequestTypeDef,
     GetCommentReactionsOutputTypeDef,
+    PutRepositoryTriggersInputRequestTypeDef,
+    TestRepositoryTriggersInputRequestTypeDef,
+    CreateUnreferencedMergeCommitInputRequestTypeDef,
+    MergeBranchesBySquashInputRequestTypeDef,
+    MergeBranchesByThreeWayInputRequestTypeDef,
+    MergePullRequestBySquashInputRequestTypeDef,
+    MergePullRequestByThreeWayInputRequestTypeDef,
     BatchDescribeMergeConflictsOutputTypeDef,
     DescribePullRequestEventsOutputTypeDef,
     CreatePullRequestOutputTypeDef,
     GetPullRequestOutputTypeDef,
     MergePullRequestByFastForwardOutputTypeDef,
     MergePullRequestBySquashOutputTypeDef,
     MergePullRequestByThreeWayOutputTypeDef,
     UpdatePullRequestDescriptionOutputTypeDef,
     UpdatePullRequestStatusOutputTypeDef,
     UpdatePullRequestTitleOutputTypeDef,
 )
 
 
-def get_structure() -> ApprovalRuleEventMetadataTypeDef:
+def get_value() -> ApprovalRuleEventMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-codecommit-1.28.15.post1/mypy_boto3_codecommit.egg-info/SOURCES.txt` & `mypy-boto3-codecommit-1.28.16/mypy_boto3_codecommit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codecommit-1.28.15.post1/setup.py` & `mypy-boto3-codecommit-1.28.16/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-codecommit",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_codecommit"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CodeCommit 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.2"
+        "Type annotations for boto3.CodeCommit 1.28.16 service generated with mypy-boto3-builder"
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
-    keywords="boto3 codecommit type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 codecommit type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_codecommit": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

