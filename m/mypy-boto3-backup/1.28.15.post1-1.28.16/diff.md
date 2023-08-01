# Comparing `tmp/mypy-boto3-backup-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-backup-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-backup-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:34 2023, max compression
+gzip compressed data, was "mypy-boto3-backup-1.28.16.tar", last modified: Tue Aug  1 11:36:15 2023, max compression
```

## Comparing `mypy-boto3-backup-1.28.15.post1.tar` & `mypy-boto3-backup-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:34.645022 mypy-boto3-backup-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:38:54.000000 mypy-boto3-backup-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    22321 2023-07-29 10:02:34.645022 mypy-boto3-backup-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20832 2023-07-29 09:38:54.000000 mypy-boto3-backup-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:34.645022 mypy-boto3-backup-1.28.15.post1/mypy_boto3_backup/
--rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-07-29 09:38:54.000000 mypy-boto3-backup-1.28.15.post1/mypy_boto3_backup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-07-29 09:38:54.000000 mypy-boto3-backup-1.28.15.post1/mypy_boto3_backup/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-29 09:38:54.000000 mypy-boto3-backup-1.28.15.post1/mypy_boto3_backup/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    55491 2023-07-29 09:38:54.000000 mypy-boto3-backup-1.28.15.post1/mypy_boto3_backup/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    55399 2023-07-29 09:38:54.000000 mypy-boto3-backup-1.28.15.post1/mypy_boto3_backup/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-07-29 09:38:55.000000 mypy-boto3-backup-1.28.15.post1/mypy_boto3_backup/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-29 09:38:55.000000 mypy-boto3-backup-1.28.15.post1/mypy_boto3_backup/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    16562 2023-07-29 09:38:55.000000 mypy-boto3-backup-1.28.15.post1/mypy_boto3_backup/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    16547 2023-07-29 09:38:55.000000 mypy-boto3-backup-1.28.15.post1/mypy_boto3_backup/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:38:54.000000 mypy-boto3-backup-1.28.15.post1/mypy_boto3_backup/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    71561 2023-07-29 09:38:58.000000 mypy-boto3-backup-1.28.15.post1/mypy_boto3_backup/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    71478 2023-07-29 09:38:56.000000 mypy-boto3-backup-1.28.15.post1/mypy_boto3_backup/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:38:54.000000 mypy-boto3-backup-1.28.15.post1/mypy_boto3_backup/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:34.645022 mypy-boto3-backup-1.28.15.post1/mypy_boto3_backup.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22321 2023-07-29 10:02:34.000000 mypy-boto3-backup-1.28.15.post1/mypy_boto3_backup.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-29 10:02:34.000000 mypy-boto3-backup-1.28.15.post1/mypy_boto3_backup.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:34.000000 mypy-boto3-backup-1.28.15.post1/mypy_boto3_backup.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:34.000000 mypy-boto3-backup-1.28.15.post1/mypy_boto3_backup.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:34.000000 mypy-boto3-backup-1.28.15.post1/mypy_boto3_backup.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-29 10:02:34.000000 mypy-boto3-backup-1.28.15.post1/mypy_boto3_backup.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:34.645022 mypy-boto3-backup-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-29 09:38:54.000000 mypy-boto3-backup-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:15.472945 mypy-boto3-backup-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:11:27.000000 mypy-boto3-backup-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22510 2023-08-01 11:36:15.472945 mypy-boto3-backup-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21030 2023-08-01 11:11:27.000000 mypy-boto3-backup-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:15.464944 mypy-boto3-backup-1.28.16/mypy_boto3_backup/
+-rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-08-01 11:11:27.000000 mypy-boto3-backup-1.28.16/mypy_boto3_backup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-08-01 11:11:27.000000 mypy-boto3-backup-1.28.16/mypy_boto3_backup/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-08-01 11:11:27.000000 mypy-boto3-backup-1.28.16/mypy_boto3_backup/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54894 2023-08-01 11:11:27.000000 mypy-boto3-backup-1.28.16/mypy_boto3_backup/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54802 2023-08-01 11:11:27.000000 mypy-boto3-backup-1.28.16/mypy_boto3_backup/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-08-01 11:11:28.000000 mypy-boto3-backup-1.28.16/mypy_boto3_backup/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-08-01 11:11:28.000000 mypy-boto3-backup-1.28.16/mypy_boto3_backup/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    16491 2023-08-01 11:11:28.000000 mypy-boto3-backup-1.28.16/mypy_boto3_backup/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16476 2023-08-01 11:11:28.000000 mypy-boto3-backup-1.28.16/mypy_boto3_backup/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:11:27.000000 mypy-boto3-backup-1.28.16/mypy_boto3_backup/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    72070 2023-08-01 11:11:31.000000 mypy-boto3-backup-1.28.16/mypy_boto3_backup/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71987 2023-08-01 11:11:30.000000 mypy-boto3-backup-1.28.16/mypy_boto3_backup/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:11:27.000000 mypy-boto3-backup-1.28.16/mypy_boto3_backup/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:15.472945 mypy-boto3-backup-1.28.16/mypy_boto3_backup.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22510 2023-08-01 11:36:15.000000 mypy-boto3-backup-1.28.16/mypy_boto3_backup.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-08-01 11:36:15.000000 mypy-boto3-backup-1.28.16/mypy_boto3_backup.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:15.000000 mypy-boto3-backup-1.28.16/mypy_boto3_backup.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:15.000000 mypy-boto3-backup-1.28.16/mypy_boto3_backup.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:15.000000 mypy-boto3-backup-1.28.16/mypy_boto3_backup.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-01 11:36:15.000000 mypy-boto3-backup-1.28.16/mypy_boto3_backup.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:15.472945 mypy-boto3-backup-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-08-01 11:11:27.000000 mypy-boto3-backup-1.28.16/setup.py
```

### Comparing `mypy-boto3-backup-1.28.15.post1/LICENSE` & `mypy-boto3-backup-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-backup-1.28.15.post1/PKG-INFO` & `mypy-boto3-backup-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-backup
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.Backup 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.Backup 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 backup type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 backup type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-backup.svg?color=blue)](https://pypi.org/project/mypy-boto3-backup)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-backup)](https://pepy.tech/project/mypy-boto3-backup)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Backup 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup)
+[boto3.Backup 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup)
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
 [mypy-boto3-backup docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/).
 
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
@@ -369,20 +369,20 @@
 )
 
 
 def check_value(value: BackupJobStateType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_backup.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_backup.type_defs import (
     AdvancedBackupSettingOutputTypeDef,
     AdvancedBackupSettingTypeDef,
     RecoveryPointCreatorTypeDef,
     BackupPlanTemplatesListMemberTypeDef,
@@ -397,15 +397,15 @@
     ControlScopeOutputTypeDef,
     ControlScopeTypeDef,
     ResponseMetadataTypeDef,
     CreateBackupVaultInputRequestTypeDef,
     ReportDeliveryChannelTypeDef,
     ReportSettingTypeDef,
     DateRangeOutputTypeDef,
-    DateRangeTypeDef,
+    TimestampTypeDef,
     DeleteBackupPlanInputRequestTypeDef,
     DeleteBackupSelectionInputRequestTypeDef,
     DeleteBackupVaultAccessPolicyInputRequestTypeDef,
     DeleteBackupVaultInputRequestTypeDef,
     DeleteBackupVaultLockConfigurationInputRequestTypeDef,
     DeleteBackupVaultNotificationsInputRequestTypeDef,
     DeleteFrameworkInputRequestTypeDef,
@@ -430,33 +430,28 @@
     GetBackupSelectionInputRequestTypeDef,
     GetBackupVaultAccessPolicyInputRequestTypeDef,
     GetBackupVaultNotificationsInputRequestTypeDef,
     GetLegalHoldInputRequestTypeDef,
     GetRecoveryPointRestoreMetadataInputRequestTypeDef,
     LegalHoldTypeDef,
     PaginatorConfigTypeDef,
-    ListBackupJobsInputRequestTypeDef,
     ListBackupPlanTemplatesInputRequestTypeDef,
     ListBackupPlanVersionsInputRequestTypeDef,
     ListBackupPlansInputRequestTypeDef,
     ListBackupSelectionsInputRequestTypeDef,
     ListBackupVaultsInputRequestTypeDef,
-    ListCopyJobsInputRequestTypeDef,
     ListFrameworksInputRequestTypeDef,
     ListLegalHoldsInputRequestTypeDef,
     ListProtectedResourcesInputRequestTypeDef,
     ProtectedResourceTypeDef,
-    ListRecoveryPointsByBackupVaultInputRequestTypeDef,
     ListRecoveryPointsByLegalHoldInputRequestTypeDef,
     RecoveryPointMemberTypeDef,
     ListRecoveryPointsByResourceInputRequestTypeDef,
     RecoveryPointByResourceTypeDef,
-    ListReportJobsInputRequestTypeDef,
     ListReportPlansInputRequestTypeDef,
-    ListRestoreJobsInputRequestTypeDef,
     RestoreJobsListMemberTypeDef,
     ListTagsInputRequestTypeDef,
     PutBackupVaultAccessPolicyInputRequestTypeDef,
     PutBackupVaultLockConfigurationInputRequestTypeDef,
     PutBackupVaultNotificationsInputRequestTypeDef,
     ReportDeliveryChannelOutputTypeDef,
     ReportDestinationTypeDef,
@@ -510,15 +505,20 @@
     UpdateBackupPlanOutputTypeDef,
     UpdateFrameworkOutputTypeDef,
     UpdateRecoveryPointLifecycleOutputTypeDef,
     UpdateReportPlanOutputTypeDef,
     CreateReportPlanInputRequestTypeDef,
     UpdateReportPlanInputRequestTypeDef,
     RecoveryPointSelectionOutputTypeDef,
-    RecoveryPointSelectionTypeDef,
+    DateRangeTypeDef,
+    ListBackupJobsInputRequestTypeDef,
+    ListCopyJobsInputRequestTypeDef,
+    ListRecoveryPointsByBackupVaultInputRequestTypeDef,
+    ListReportJobsInputRequestTypeDef,
+    ListRestoreJobsInputRequestTypeDef,
     ListFrameworksOutputTypeDef,
     ListLegalHoldsOutputTypeDef,
     ListBackupJobsInputListBackupJobsPaginateTypeDef,
     ListBackupPlanTemplatesInputListBackupPlanTemplatesPaginateTypeDef,
     ListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef,
     ListBackupPlansInputListBackupPlansPaginateTypeDef,
     ListBackupSelectionsInputListBackupSelectionsPaginateTypeDef,
@@ -530,49 +530,55 @@
     ListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef,
     ListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef,
     ListRestoreJobsInputListRestoreJobsPaginateTypeDef,
     ListProtectedResourcesOutputTypeDef,
     ListRecoveryPointsByLegalHoldOutputTypeDef,
     ListRecoveryPointsByResourceOutputTypeDef,
     ListRestoreJobsOutputTypeDef,
+    ReportDeliveryChannelUnionTypeDef,
     ReportJobTypeDef,
     ReportPlanTypeDef,
+    ReportSettingUnionTypeDef,
     ListBackupPlanVersionsOutputTypeDef,
     ListBackupPlansOutputTypeDef,
     ListBackupJobsOutputTypeDef,
     DescribeCopyJobOutputTypeDef,
     ListCopyJobsOutputTypeDef,
     BackupRuleInputTypeDef,
     BackupRuleTypeDef,
     ListRecoveryPointsByBackupVaultOutputTypeDef,
     BackupSelectionOutputTypeDef,
     BackupSelectionTypeDef,
     DescribeFrameworkOutputTypeDef,
-    CreateFrameworkInputRequestTypeDef,
-    UpdateFrameworkInputRequestTypeDef,
+    FrameworkControlUnionTypeDef,
     CreateLegalHoldOutputTypeDef,
     GetLegalHoldOutputTypeDef,
-    CreateLegalHoldInputRequestTypeDef,
+    RecoveryPointSelectionTypeDef,
     DescribeReportJobOutputTypeDef,
     ListReportJobsOutputTypeDef,
     DescribeReportPlanOutputTypeDef,
     ListReportPlansOutputTypeDef,
     BackupPlanInputTypeDef,
     BackupPlanTypeDef,
     GetBackupSelectionOutputTypeDef,
+    BackupSelectionUnionTypeDef,
     CreateBackupSelectionInputRequestTypeDef,
+    CreateFrameworkInputRequestTypeDef,
+    UpdateFrameworkInputRequestTypeDef,
+    CreateLegalHoldInputRequestTypeDef,
+    RecoveryPointSelectionUnionTypeDef,
     CreateBackupPlanInputRequestTypeDef,
     UpdateBackupPlanInputRequestTypeDef,
     GetBackupPlanFromJSONOutputTypeDef,
     GetBackupPlanFromTemplateOutputTypeDef,
     GetBackupPlanOutputTypeDef,
 )
 
 
-def get_structure() -> AdvancedBackupSettingOutputTypeDef:
+def get_value() -> AdvancedBackupSettingOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-backup-1.28.15.post1/README.md` & `mypy-boto3-backup-1.28.16/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-backup.svg?color=blue)](https://pypi.org/project/mypy-boto3-backup)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-backup)](https://pepy.tech/project/mypy-boto3-backup)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Backup 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup)
+[boto3.Backup 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup)
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
 [mypy-boto3-backup docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/).
 
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
@@ -337,20 +337,20 @@
 )
 
 
 def check_value(value: BackupJobStateType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_backup.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_backup.type_defs import (
     AdvancedBackupSettingOutputTypeDef,
     AdvancedBackupSettingTypeDef,
     RecoveryPointCreatorTypeDef,
     BackupPlanTemplatesListMemberTypeDef,
@@ -365,15 +365,15 @@
     ControlScopeOutputTypeDef,
     ControlScopeTypeDef,
     ResponseMetadataTypeDef,
     CreateBackupVaultInputRequestTypeDef,
     ReportDeliveryChannelTypeDef,
     ReportSettingTypeDef,
     DateRangeOutputTypeDef,
-    DateRangeTypeDef,
+    TimestampTypeDef,
     DeleteBackupPlanInputRequestTypeDef,
     DeleteBackupSelectionInputRequestTypeDef,
     DeleteBackupVaultAccessPolicyInputRequestTypeDef,
     DeleteBackupVaultInputRequestTypeDef,
     DeleteBackupVaultLockConfigurationInputRequestTypeDef,
     DeleteBackupVaultNotificationsInputRequestTypeDef,
     DeleteFrameworkInputRequestTypeDef,
@@ -398,33 +398,28 @@
     GetBackupSelectionInputRequestTypeDef,
     GetBackupVaultAccessPolicyInputRequestTypeDef,
     GetBackupVaultNotificationsInputRequestTypeDef,
     GetLegalHoldInputRequestTypeDef,
     GetRecoveryPointRestoreMetadataInputRequestTypeDef,
     LegalHoldTypeDef,
     PaginatorConfigTypeDef,
-    ListBackupJobsInputRequestTypeDef,
     ListBackupPlanTemplatesInputRequestTypeDef,
     ListBackupPlanVersionsInputRequestTypeDef,
     ListBackupPlansInputRequestTypeDef,
     ListBackupSelectionsInputRequestTypeDef,
     ListBackupVaultsInputRequestTypeDef,
-    ListCopyJobsInputRequestTypeDef,
     ListFrameworksInputRequestTypeDef,
     ListLegalHoldsInputRequestTypeDef,
     ListProtectedResourcesInputRequestTypeDef,
     ProtectedResourceTypeDef,
-    ListRecoveryPointsByBackupVaultInputRequestTypeDef,
     ListRecoveryPointsByLegalHoldInputRequestTypeDef,
     RecoveryPointMemberTypeDef,
     ListRecoveryPointsByResourceInputRequestTypeDef,
     RecoveryPointByResourceTypeDef,
-    ListReportJobsInputRequestTypeDef,
     ListReportPlansInputRequestTypeDef,
-    ListRestoreJobsInputRequestTypeDef,
     RestoreJobsListMemberTypeDef,
     ListTagsInputRequestTypeDef,
     PutBackupVaultAccessPolicyInputRequestTypeDef,
     PutBackupVaultLockConfigurationInputRequestTypeDef,
     PutBackupVaultNotificationsInputRequestTypeDef,
     ReportDeliveryChannelOutputTypeDef,
     ReportDestinationTypeDef,
@@ -478,15 +473,20 @@
     UpdateBackupPlanOutputTypeDef,
     UpdateFrameworkOutputTypeDef,
     UpdateRecoveryPointLifecycleOutputTypeDef,
     UpdateReportPlanOutputTypeDef,
     CreateReportPlanInputRequestTypeDef,
     UpdateReportPlanInputRequestTypeDef,
     RecoveryPointSelectionOutputTypeDef,
-    RecoveryPointSelectionTypeDef,
+    DateRangeTypeDef,
+    ListBackupJobsInputRequestTypeDef,
+    ListCopyJobsInputRequestTypeDef,
+    ListRecoveryPointsByBackupVaultInputRequestTypeDef,
+    ListReportJobsInputRequestTypeDef,
+    ListRestoreJobsInputRequestTypeDef,
     ListFrameworksOutputTypeDef,
     ListLegalHoldsOutputTypeDef,
     ListBackupJobsInputListBackupJobsPaginateTypeDef,
     ListBackupPlanTemplatesInputListBackupPlanTemplatesPaginateTypeDef,
     ListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef,
     ListBackupPlansInputListBackupPlansPaginateTypeDef,
     ListBackupSelectionsInputListBackupSelectionsPaginateTypeDef,
@@ -498,49 +498,55 @@
     ListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef,
     ListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef,
     ListRestoreJobsInputListRestoreJobsPaginateTypeDef,
     ListProtectedResourcesOutputTypeDef,
     ListRecoveryPointsByLegalHoldOutputTypeDef,
     ListRecoveryPointsByResourceOutputTypeDef,
     ListRestoreJobsOutputTypeDef,
+    ReportDeliveryChannelUnionTypeDef,
     ReportJobTypeDef,
     ReportPlanTypeDef,
+    ReportSettingUnionTypeDef,
     ListBackupPlanVersionsOutputTypeDef,
     ListBackupPlansOutputTypeDef,
     ListBackupJobsOutputTypeDef,
     DescribeCopyJobOutputTypeDef,
     ListCopyJobsOutputTypeDef,
     BackupRuleInputTypeDef,
     BackupRuleTypeDef,
     ListRecoveryPointsByBackupVaultOutputTypeDef,
     BackupSelectionOutputTypeDef,
     BackupSelectionTypeDef,
     DescribeFrameworkOutputTypeDef,
-    CreateFrameworkInputRequestTypeDef,
-    UpdateFrameworkInputRequestTypeDef,
+    FrameworkControlUnionTypeDef,
     CreateLegalHoldOutputTypeDef,
     GetLegalHoldOutputTypeDef,
-    CreateLegalHoldInputRequestTypeDef,
+    RecoveryPointSelectionTypeDef,
     DescribeReportJobOutputTypeDef,
     ListReportJobsOutputTypeDef,
     DescribeReportPlanOutputTypeDef,
     ListReportPlansOutputTypeDef,
     BackupPlanInputTypeDef,
     BackupPlanTypeDef,
     GetBackupSelectionOutputTypeDef,
+    BackupSelectionUnionTypeDef,
     CreateBackupSelectionInputRequestTypeDef,
+    CreateFrameworkInputRequestTypeDef,
+    UpdateFrameworkInputRequestTypeDef,
+    CreateLegalHoldInputRequestTypeDef,
+    RecoveryPointSelectionUnionTypeDef,
     CreateBackupPlanInputRequestTypeDef,
     UpdateBackupPlanInputRequestTypeDef,
     GetBackupPlanFromJSONOutputTypeDef,
     GetBackupPlanFromTemplateOutputTypeDef,
     GetBackupPlanOutputTypeDef,
 )
 
 
-def get_structure() -> AdvancedBackupSettingOutputTypeDef:
+def get_value() -> AdvancedBackupSettingOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-backup-1.28.15.post1/mypy_boto3_backup/__init__.py` & `mypy-boto3-backup-1.28.16/mypy_boto3_backup/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-backup-1.28.15.post1/mypy_boto3_backup/__init__.pyi` & `mypy-boto3-backup-1.28.16/mypy_boto3_backup/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-backup-1.28.15.post1/mypy_boto3_backup/__main__.py` & `mypy-boto3-backup-1.28.16/mypy_boto3_backup/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Backup 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.Backup 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup\nOther"
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

### Comparing `mypy-boto3-backup-1.28.15.post1/mypy_boto3_backup/client.py` & `mypy-boto3-backup-1.28.16/mypy_boto3_backup/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from mypy_boto3_backup.client import BackupClient
 
     session = Session()
     client: BackupClient = session.client("backup")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     BackupJobStateType,
     BackupVaultEventType,
     CopyJobStateType,
@@ -38,16 +37,15 @@
     ListRecoveryPointsByBackupVaultPaginator,
     ListRecoveryPointsByLegalHoldPaginator,
     ListRecoveryPointsByResourcePaginator,
     ListRestoreJobsPaginator,
 )
 from .type_defs import (
     BackupPlanInputTypeDef,
-    BackupSelectionOutputTypeDef,
-    BackupSelectionTypeDef,
+    BackupSelectionUnionTypeDef,
     CreateBackupPlanOutputTypeDef,
     CreateBackupSelectionOutputTypeDef,
     CreateBackupVaultOutputTypeDef,
     CreateFrameworkOutputTypeDef,
     CreateLegalHoldOutputTypeDef,
     CreateReportPlanOutputTypeDef,
     DeleteBackupPlanOutputTypeDef,
@@ -60,16 +58,15 @@
     DescribeRecoveryPointOutputTypeDef,
     DescribeRegionSettingsOutputTypeDef,
     DescribeReportJobOutputTypeDef,
     DescribeReportPlanOutputTypeDef,
     DescribeRestoreJobOutputTypeDef,
     EmptyResponseMetadataTypeDef,
     ExportBackupPlanTemplateOutputTypeDef,
-    FrameworkControlOutputTypeDef,
-    FrameworkControlTypeDef,
+    FrameworkControlUnionTypeDef,
     GetBackupPlanFromJSONOutputTypeDef,
     GetBackupPlanFromTemplateOutputTypeDef,
     GetBackupPlanOutputTypeDef,
     GetBackupSelectionOutputTypeDef,
     GetBackupVaultAccessPolicyOutputTypeDef,
     GetBackupVaultNotificationsOutputTypeDef,
     GetLegalHoldOutputTypeDef,
@@ -89,61 +86,55 @@
     ListRecoveryPointsByBackupVaultOutputTypeDef,
     ListRecoveryPointsByLegalHoldOutputTypeDef,
     ListRecoveryPointsByResourceOutputTypeDef,
     ListReportJobsOutputTypeDef,
     ListReportPlansOutputTypeDef,
     ListRestoreJobsOutputTypeDef,
     ListTagsOutputTypeDef,
-    RecoveryPointSelectionOutputTypeDef,
-    RecoveryPointSelectionTypeDef,
-    ReportDeliveryChannelOutputTypeDef,
-    ReportDeliveryChannelTypeDef,
-    ReportSettingOutputTypeDef,
-    ReportSettingTypeDef,
+    RecoveryPointSelectionUnionTypeDef,
+    ReportDeliveryChannelUnionTypeDef,
+    ReportSettingUnionTypeDef,
     StartBackupJobOutputTypeDef,
     StartCopyJobOutputTypeDef,
     StartReportJobOutputTypeDef,
     StartRestoreJobOutputTypeDef,
+    TimestampTypeDef,
     UpdateBackupPlanOutputTypeDef,
     UpdateFrameworkOutputTypeDef,
     UpdateRecoveryPointLifecycleOutputTypeDef,
     UpdateReportPlanOutputTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("BackupClient",)
 
-
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     AlreadyExistsException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     DependencyFailureException: Type[BotocoreClientError]
     InvalidParameterValueException: Type[BotocoreClientError]
     InvalidRequestException: Type[BotocoreClientError]
     InvalidResourceStateException: Type[BotocoreClientError]
     LimitExceededException: Type[BotocoreClientError]
     MissingParameterValueException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ServiceUnavailableException: Type[BotocoreClientError]
 
-
 class BackupClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/)
     """
 
     meta: ClientMeta
@@ -152,699 +143,634 @@
     def exceptions(self) -> Exceptions:
         """
         BackupClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#exceptions)
         """
-
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#can_paginate)
         """
-
     def cancel_legal_hold(
         self, *, LegalHoldId: str, CancelDescription: str, RetainRecordInDays: int = ...
     ) -> Dict[str, Any]:
         """
         This action removes the specified legal hold on a recovery point.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.cancel_legal_hold)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#cancel_legal_hold)
         """
-
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#close)
         """
-
     def create_backup_plan(
         self,
         *,
         BackupPlan: BackupPlanInputTypeDef,
         BackupPlanTags: Mapping[str, str] = ...,
         CreatorRequestId: str = ...
     ) -> CreateBackupPlanOutputTypeDef:
         """
         Creates a backup plan using a backup plan name and backup rules.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.create_backup_plan)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#create_backup_plan)
         """
-
     def create_backup_selection(
         self,
         *,
         BackupPlanId: str,
-        BackupSelection: Union[BackupSelectionTypeDef, BackupSelectionOutputTypeDef],
+        BackupSelection: BackupSelectionUnionTypeDef,
         CreatorRequestId: str = ...
     ) -> CreateBackupSelectionOutputTypeDef:
         """
         Creates a JSON document that specifies a set of resources to assign to a backup
         plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.create_backup_selection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#create_backup_selection)
         """
-
     def create_backup_vault(
         self,
         *,
         BackupVaultName: str,
         BackupVaultTags: Mapping[str, str] = ...,
         EncryptionKeyArn: str = ...,
         CreatorRequestId: str = ...
     ) -> CreateBackupVaultOutputTypeDef:
         """
         Creates a logical container where backups are stored.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.create_backup_vault)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#create_backup_vault)
         """
-
     def create_framework(
         self,
         *,
         FrameworkName: str,
-        FrameworkControls: Sequence[Union[FrameworkControlTypeDef, FrameworkControlOutputTypeDef]],
+        FrameworkControls: Sequence[FrameworkControlUnionTypeDef],
         FrameworkDescription: str = ...,
         IdempotencyToken: str = ...,
         FrameworkTags: Mapping[str, str] = ...
     ) -> CreateFrameworkOutputTypeDef:
         """
         Creates a framework with one or more controls.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.create_framework)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#create_framework)
         """
-
     def create_legal_hold(
         self,
         *,
         Title: str,
         Description: str,
         IdempotencyToken: str = ...,
-        RecoveryPointSelection: Union[
-            RecoveryPointSelectionTypeDef, RecoveryPointSelectionOutputTypeDef
-        ] = ...,
+        RecoveryPointSelection: RecoveryPointSelectionUnionTypeDef = ...,
         Tags: Mapping[str, str] = ...
     ) -> CreateLegalHoldOutputTypeDef:
         """
         This action creates a legal hold on a recovery point (backup).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.create_legal_hold)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#create_legal_hold)
         """
-
     def create_report_plan(
         self,
         *,
         ReportPlanName: str,
-        ReportDeliveryChannel: Union[
-            ReportDeliveryChannelTypeDef, ReportDeliveryChannelOutputTypeDef
-        ],
-        ReportSetting: Union[ReportSettingTypeDef, ReportSettingOutputTypeDef],
+        ReportDeliveryChannel: ReportDeliveryChannelUnionTypeDef,
+        ReportSetting: ReportSettingUnionTypeDef,
         ReportPlanDescription: str = ...,
         ReportPlanTags: Mapping[str, str] = ...,
         IdempotencyToken: str = ...
     ) -> CreateReportPlanOutputTypeDef:
         """
         Creates a report plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.create_report_plan)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#create_report_plan)
         """
-
     def delete_backup_plan(self, *, BackupPlanId: str) -> DeleteBackupPlanOutputTypeDef:
         """
         Deletes a backup plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.delete_backup_plan)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#delete_backup_plan)
         """
-
     def delete_backup_selection(
         self, *, BackupPlanId: str, SelectionId: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the resource selection associated with a backup plan that is specified
         by the `SelectionId`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.delete_backup_selection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#delete_backup_selection)
         """
-
     def delete_backup_vault(self, *, BackupVaultName: str) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the backup vault identified by its name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.delete_backup_vault)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#delete_backup_vault)
         """
-
     def delete_backup_vault_access_policy(
         self, *, BackupVaultName: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the policy document that manages permissions on a backup vault.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.delete_backup_vault_access_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#delete_backup_vault_access_policy)
         """
-
     def delete_backup_vault_lock_configuration(
         self, *, BackupVaultName: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes Backup Vault Lock from a backup vault specified by a backup vault name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.delete_backup_vault_lock_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#delete_backup_vault_lock_configuration)
         """
-
     def delete_backup_vault_notifications(
         self, *, BackupVaultName: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes event notifications for the specified backup vault.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.delete_backup_vault_notifications)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#delete_backup_vault_notifications)
         """
-
     def delete_framework(self, *, FrameworkName: str) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the framework specified by a framework name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.delete_framework)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#delete_framework)
         """
-
     def delete_recovery_point(
         self, *, BackupVaultName: str, RecoveryPointArn: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the recovery point specified by a recovery point ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.delete_recovery_point)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#delete_recovery_point)
         """
-
     def delete_report_plan(self, *, ReportPlanName: str) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the report plan specified by a report plan name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.delete_report_plan)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#delete_report_plan)
         """
-
     def describe_backup_job(self, *, BackupJobId: str) -> DescribeBackupJobOutputTypeDef:
         """
         Returns backup job details for the specified `BackupJobId`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.describe_backup_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#describe_backup_job)
         """
-
     def describe_backup_vault(self, *, BackupVaultName: str) -> DescribeBackupVaultOutputTypeDef:
         """
         Returns metadata about a backup vault specified by its name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.describe_backup_vault)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#describe_backup_vault)
         """
-
     def describe_copy_job(self, *, CopyJobId: str) -> DescribeCopyJobOutputTypeDef:
         """
         Returns metadata associated with creating a copy of a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.describe_copy_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#describe_copy_job)
         """
-
     def describe_framework(self, *, FrameworkName: str) -> DescribeFrameworkOutputTypeDef:
         """
         Returns the framework details for the specified `FrameworkName`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.describe_framework)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#describe_framework)
         """
-
     def describe_global_settings(self) -> DescribeGlobalSettingsOutputTypeDef:
         """
         Describes whether the Amazon Web Services account is opted in to cross-account
         backup.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.describe_global_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#describe_global_settings)
         """
-
     def describe_protected_resource(
         self, *, ResourceArn: str
     ) -> DescribeProtectedResourceOutputTypeDef:
         """
         Returns information about a saved resource, including the last time it was
         backed up, its Amazon Resource Name (ARN), and the Amazon Web Services service
         type of the saved resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.describe_protected_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#describe_protected_resource)
         """
-
     def describe_recovery_point(
         self, *, BackupVaultName: str, RecoveryPointArn: str
     ) -> DescribeRecoveryPointOutputTypeDef:
         """
         Returns metadata associated with a recovery point, including ID, status,
         encryption, and lifecycle.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.describe_recovery_point)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#describe_recovery_point)
         """
-
     def describe_region_settings(self) -> DescribeRegionSettingsOutputTypeDef:
         """
         Returns the current service opt-in settings for the Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.describe_region_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#describe_region_settings)
         """
-
     def describe_report_job(self, *, ReportJobId: str) -> DescribeReportJobOutputTypeDef:
         """
         Returns the details associated with creating a report as specified by its
         `ReportJobId`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.describe_report_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#describe_report_job)
         """
-
     def describe_report_plan(self, *, ReportPlanName: str) -> DescribeReportPlanOutputTypeDef:
         """
         Returns a list of all report plans for an Amazon Web Services account and Amazon
         Web Services Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.describe_report_plan)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#describe_report_plan)
         """
-
     def describe_restore_job(self, *, RestoreJobId: str) -> DescribeRestoreJobOutputTypeDef:
         """
         Returns metadata associated with a restore job that is specified by a job ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.describe_restore_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#describe_restore_job)
         """
-
     def disassociate_recovery_point(
         self, *, BackupVaultName: str, RecoveryPointArn: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the specified continuous backup recovery point from Backup and releases
         control of that continuous backup to the source service, such as Amazon RDS.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.disassociate_recovery_point)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#disassociate_recovery_point)
         """
-
     def disassociate_recovery_point_from_parent(
         self, *, BackupVaultName: str, RecoveryPointArn: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         This action to a specific child (nested) recovery point removes the relationship
         between the specified recovery point and its parent (composite) recovery point.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.disassociate_recovery_point_from_parent)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#disassociate_recovery_point_from_parent)
         """
-
     def export_backup_plan_template(
         self, *, BackupPlanId: str
     ) -> ExportBackupPlanTemplateOutputTypeDef:
         """
         Returns the backup plan that is specified by the plan ID as a backup template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.export_backup_plan_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#export_backup_plan_template)
         """
-
     def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#generate_presigned_url)
         """
-
     def get_backup_plan(
         self, *, BackupPlanId: str, VersionId: str = ...
     ) -> GetBackupPlanOutputTypeDef:
         """
         Returns `BackupPlan` details for the specified `BackupPlanId`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.get_backup_plan)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#get_backup_plan)
         """
-
     def get_backup_plan_from_json(
         self, *, BackupPlanTemplateJson: str
     ) -> GetBackupPlanFromJSONOutputTypeDef:
         """
         Returns a valid JSON document specifying a backup plan or an error.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.get_backup_plan_from_json)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#get_backup_plan_from_json)
         """
-
     def get_backup_plan_from_template(
         self, *, BackupPlanTemplateId: str
     ) -> GetBackupPlanFromTemplateOutputTypeDef:
         """
         Returns the template specified by its `templateId` as a backup plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.get_backup_plan_from_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#get_backup_plan_from_template)
         """
-
     def get_backup_selection(
         self, *, BackupPlanId: str, SelectionId: str
     ) -> GetBackupSelectionOutputTypeDef:
         """
         Returns selection metadata and a document in JSON format that specifies a list
         of resources that are associated with a backup plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.get_backup_selection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#get_backup_selection)
         """
-
     def get_backup_vault_access_policy(
         self, *, BackupVaultName: str
     ) -> GetBackupVaultAccessPolicyOutputTypeDef:
         """
         Returns the access policy document that is associated with the named backup
         vault.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.get_backup_vault_access_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#get_backup_vault_access_policy)
         """
-
     def get_backup_vault_notifications(
         self, *, BackupVaultName: str
     ) -> GetBackupVaultNotificationsOutputTypeDef:
         """
         Returns event notifications for the specified backup vault.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.get_backup_vault_notifications)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#get_backup_vault_notifications)
         """
-
     def get_legal_hold(self, *, LegalHoldId: str) -> GetLegalHoldOutputTypeDef:
         """
         This action returns details for a specified legal hold.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.get_legal_hold)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#get_legal_hold)
         """
-
     def get_recovery_point_restore_metadata(
         self, *, BackupVaultName: str, RecoveryPointArn: str
     ) -> GetRecoveryPointRestoreMetadataOutputTypeDef:
         """
         Returns a set of metadata key-value pairs that were used to create the backup.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.get_recovery_point_restore_metadata)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#get_recovery_point_restore_metadata)
         """
-
     def get_supported_resource_types(self) -> GetSupportedResourceTypesOutputTypeDef:
         """
         Returns the Amazon Web Services resource types supported by Backup.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.get_supported_resource_types)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#get_supported_resource_types)
         """
-
     def list_backup_jobs(
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
         ByResourceArn: str = ...,
         ByState: BackupJobStateType = ...,
         ByBackupVaultName: str = ...,
-        ByCreatedBefore: Union[datetime, str] = ...,
-        ByCreatedAfter: Union[datetime, str] = ...,
+        ByCreatedBefore: TimestampTypeDef = ...,
+        ByCreatedAfter: TimestampTypeDef = ...,
         ByResourceType: str = ...,
         ByAccountId: str = ...,
-        ByCompleteAfter: Union[datetime, str] = ...,
-        ByCompleteBefore: Union[datetime, str] = ...,
+        ByCompleteAfter: TimestampTypeDef = ...,
+        ByCompleteBefore: TimestampTypeDef = ...,
         ByParentJobId: str = ...
     ) -> ListBackupJobsOutputTypeDef:
         """
         Returns a list of existing backup jobs for an authenticated account for the last
         30 days.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.list_backup_jobs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#list_backup_jobs)
         """
-
     def list_backup_plan_templates(
         self, *, NextToken: str = ..., MaxResults: int = ...
     ) -> ListBackupPlanTemplatesOutputTypeDef:
         """
         Returns metadata of your saved backup plan templates, including the template ID,
         name, and the creation and deletion dates.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.list_backup_plan_templates)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#list_backup_plan_templates)
         """
-
     def list_backup_plan_versions(
         self, *, BackupPlanId: str, NextToken: str = ..., MaxResults: int = ...
     ) -> ListBackupPlanVersionsOutputTypeDef:
         """
         Returns version metadata of your backup plans, including Amazon Resource Names
         (ARNs), backup plan IDs, creation and deletion dates, plan names, and version
         IDs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.list_backup_plan_versions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#list_backup_plan_versions)
         """
-
     def list_backup_plans(
         self, *, NextToken: str = ..., MaxResults: int = ..., IncludeDeleted: bool = ...
     ) -> ListBackupPlansOutputTypeDef:
         """
         Returns a list of all active backup plans for an authenticated account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.list_backup_plans)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#list_backup_plans)
         """
-
     def list_backup_selections(
         self, *, BackupPlanId: str, NextToken: str = ..., MaxResults: int = ...
     ) -> ListBackupSelectionsOutputTypeDef:
         """
         Returns an array containing metadata of the resources associated with the target
         backup plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.list_backup_selections)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#list_backup_selections)
         """
-
     def list_backup_vaults(
         self, *, NextToken: str = ..., MaxResults: int = ...
     ) -> ListBackupVaultsOutputTypeDef:
         """
         Returns a list of recovery point storage containers along with information about
         them.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.list_backup_vaults)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#list_backup_vaults)
         """
-
     def list_copy_jobs(
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
         ByResourceArn: str = ...,
         ByState: CopyJobStateType = ...,
-        ByCreatedBefore: Union[datetime, str] = ...,
-        ByCreatedAfter: Union[datetime, str] = ...,
+        ByCreatedBefore: TimestampTypeDef = ...,
+        ByCreatedAfter: TimestampTypeDef = ...,
         ByResourceType: str = ...,
         ByDestinationVaultArn: str = ...,
         ByAccountId: str = ...,
-        ByCompleteBefore: Union[datetime, str] = ...,
-        ByCompleteAfter: Union[datetime, str] = ...,
+        ByCompleteBefore: TimestampTypeDef = ...,
+        ByCompleteAfter: TimestampTypeDef = ...,
         ByParentJobId: str = ...
     ) -> ListCopyJobsOutputTypeDef:
         """
         Returns metadata about your copy jobs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.list_copy_jobs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#list_copy_jobs)
         """
-
     def list_frameworks(
         self, *, MaxResults: int = ..., NextToken: str = ...
     ) -> ListFrameworksOutputTypeDef:
         """
         Returns a list of all frameworks for an Amazon Web Services account and Amazon
         Web Services Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.list_frameworks)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#list_frameworks)
         """
-
     def list_legal_holds(
         self, *, NextToken: str = ..., MaxResults: int = ...
     ) -> ListLegalHoldsOutputTypeDef:
         """
         This action returns metadata about active and previous legal holds.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.list_legal_holds)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#list_legal_holds)
         """
-
     def list_protected_resources(
         self, *, NextToken: str = ..., MaxResults: int = ...
     ) -> ListProtectedResourcesOutputTypeDef:
         """
         Returns an array of resources successfully backed up by Backup, including the
         time the resource was saved, an Amazon Resource Name (ARN) of the resource, and
         a resource type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.list_protected_resources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#list_protected_resources)
         """
-
     def list_recovery_points_by_backup_vault(
         self,
         *,
         BackupVaultName: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         ByResourceArn: str = ...,
         ByResourceType: str = ...,
         ByBackupPlanId: str = ...,
-        ByCreatedBefore: Union[datetime, str] = ...,
-        ByCreatedAfter: Union[datetime, str] = ...,
+        ByCreatedBefore: TimestampTypeDef = ...,
+        ByCreatedAfter: TimestampTypeDef = ...,
         ByParentRecoveryPointArn: str = ...
     ) -> ListRecoveryPointsByBackupVaultOutputTypeDef:
         """
         Returns detailed information about the recovery points stored in a backup vault.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.list_recovery_points_by_backup_vault)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#list_recovery_points_by_backup_vault)
         """
-
     def list_recovery_points_by_legal_hold(
         self, *, LegalHoldId: str, NextToken: str = ..., MaxResults: int = ...
     ) -> ListRecoveryPointsByLegalHoldOutputTypeDef:
         """
         This action returns recovery point ARNs (Amazon Resource Names) of the specified
         legal hold.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.list_recovery_points_by_legal_hold)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#list_recovery_points_by_legal_hold)
         """
-
     def list_recovery_points_by_resource(
         self, *, ResourceArn: str, NextToken: str = ..., MaxResults: int = ...
     ) -> ListRecoveryPointsByResourceOutputTypeDef:
         """
         Returns detailed information about all the recovery points of the type specified
         by a resource Amazon Resource Name (ARN).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.list_recovery_points_by_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#list_recovery_points_by_resource)
         """
-
     def list_report_jobs(
         self,
         *,
         ByReportPlanName: str = ...,
-        ByCreationBefore: Union[datetime, str] = ...,
-        ByCreationAfter: Union[datetime, str] = ...,
+        ByCreationBefore: TimestampTypeDef = ...,
+        ByCreationAfter: TimestampTypeDef = ...,
         ByStatus: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> ListReportJobsOutputTypeDef:
         """
         Returns details about your report jobs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.list_report_jobs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#list_report_jobs)
         """
-
     def list_report_plans(
         self, *, MaxResults: int = ..., NextToken: str = ...
     ) -> ListReportPlansOutputTypeDef:
         """
         Returns a list of your report plans.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.list_report_plans)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#list_report_plans)
         """
-
     def list_restore_jobs(
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
         ByAccountId: str = ...,
-        ByCreatedBefore: Union[datetime, str] = ...,
-        ByCreatedAfter: Union[datetime, str] = ...,
+        ByCreatedBefore: TimestampTypeDef = ...,
+        ByCreatedAfter: TimestampTypeDef = ...,
         ByStatus: RestoreJobStatusType = ...,
-        ByCompleteBefore: Union[datetime, str] = ...,
-        ByCompleteAfter: Union[datetime, str] = ...
+        ByCompleteBefore: TimestampTypeDef = ...,
+        ByCompleteAfter: TimestampTypeDef = ...
     ) -> ListRestoreJobsOutputTypeDef:
         """
         Returns a list of jobs that Backup initiated to restore a saved resource,
         including details about the recovery process.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.list_restore_jobs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#list_restore_jobs)
         """
-
     def list_tags(
         self, *, ResourceArn: str, NextToken: str = ..., MaxResults: int = ...
     ) -> ListTagsOutputTypeDef:
         """
         Returns a list of key-value pairs assigned to a target recovery point, backup
         plan, or backup vault.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.list_tags)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#list_tags)
         """
-
     def put_backup_vault_access_policy(
         self, *, BackupVaultName: str, Policy: str = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Sets a resource-based policy that is used to manage access permissions on the
         target backup vault.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.put_backup_vault_access_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#put_backup_vault_access_policy)
         """
-
     def put_backup_vault_lock_configuration(
         self,
         *,
         BackupVaultName: str,
         MinRetentionDays: int = ...,
         MaxRetentionDays: int = ...,
         ChangeableForDays: int = ...
@@ -852,29 +778,27 @@
         """
         Applies Backup Vault Lock to a backup vault, preventing attempts to delete any
         recovery point stored in or created in a backup vault.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.put_backup_vault_lock_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#put_backup_vault_lock_configuration)
         """
-
     def put_backup_vault_notifications(
         self,
         *,
         BackupVaultName: str,
         SNSTopicArn: str,
         BackupVaultEvents: Sequence[BackupVaultEventType]
     ) -> EmptyResponseMetadataTypeDef:
         """
         Turns on notifications on a backup vault for the specified topic and events.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.put_backup_vault_notifications)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#put_backup_vault_notifications)
         """
-
     def start_backup_job(
         self,
         *,
         BackupVaultName: str,
         ResourceArn: str,
         IamRoleArn: str,
         IdempotencyToken: str = ...,
@@ -886,15 +810,14 @@
     ) -> StartBackupJobOutputTypeDef:
         """
         Starts an on-demand backup job for the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.start_backup_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#start_backup_job)
         """
-
     def start_copy_job(
         self,
         *,
         RecoveryPointArn: str,
         SourceBackupVaultName: str,
         DestinationBackupVaultArn: str,
         IamRoleArn: str,
@@ -903,25 +826,23 @@
     ) -> StartCopyJobOutputTypeDef:
         """
         Starts a job to create a one-time copy of the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.start_copy_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#start_copy_job)
         """
-
     def start_report_job(
         self, *, ReportPlanName: str, IdempotencyToken: str = ...
     ) -> StartReportJobOutputTypeDef:
         """
         Starts an on-demand report job for the specified report plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.start_report_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#start_report_job)
         """
-
     def start_restore_job(
         self,
         *,
         RecoveryPointArn: str,
         Metadata: Mapping[str, str],
         IamRoleArn: str = ...,
         IdempotencyToken: str = ...,
@@ -930,230 +851,204 @@
     ) -> StartRestoreJobOutputTypeDef:
         """
         Recovers the saved resource identified by an Amazon Resource Name (ARN).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.start_restore_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#start_restore_job)
         """
-
     def stop_backup_job(self, *, BackupJobId: str) -> EmptyResponseMetadataTypeDef:
         """
         Attempts to cancel a job to create a one-time backup of a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.stop_backup_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#stop_backup_job)
         """
-
     def tag_resource(
         self, *, ResourceArn: str, Tags: Mapping[str, str]
     ) -> EmptyResponseMetadataTypeDef:
         """
         Assigns a set of key-value pairs to a recovery point, backup plan, or backup
         vault identified by an Amazon Resource Name (ARN).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#tag_resource)
         """
-
     def untag_resource(
         self, *, ResourceArn: str, TagKeyList: Sequence[str]
     ) -> EmptyResponseMetadataTypeDef:
         """
         Removes a set of key-value pairs from a recovery point, backup plan, or backup
         vault identified by an Amazon Resource Name (ARN) See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/backup-2018-11-15/UntagResource).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#untag_resource)
         """
-
     def update_backup_plan(
         self, *, BackupPlanId: str, BackupPlan: BackupPlanInputTypeDef
     ) -> UpdateBackupPlanOutputTypeDef:
         """
         Updates an existing backup plan identified by its `backupPlanId` with the input
         document in JSON format.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.update_backup_plan)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#update_backup_plan)
         """
-
     def update_framework(
         self,
         *,
         FrameworkName: str,
         FrameworkDescription: str = ...,
-        FrameworkControls: Sequence[
-            Union[FrameworkControlTypeDef, FrameworkControlOutputTypeDef]
-        ] = ...,
+        FrameworkControls: Sequence[FrameworkControlUnionTypeDef] = ...,
         IdempotencyToken: str = ...
     ) -> UpdateFrameworkOutputTypeDef:
         """
         Updates an existing framework identified by its `FrameworkName` with the input
         document in JSON format.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.update_framework)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#update_framework)
         """
-
     def update_global_settings(
         self, *, GlobalSettings: Mapping[str, str] = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates whether the Amazon Web Services account is opted in to cross-account
         backup.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.update_global_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#update_global_settings)
         """
-
     def update_recovery_point_lifecycle(
         self, *, BackupVaultName: str, RecoveryPointArn: str, Lifecycle: LifecycleTypeDef = ...
     ) -> UpdateRecoveryPointLifecycleOutputTypeDef:
         """
         Sets the transition lifecycle of a recovery point.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.update_recovery_point_lifecycle)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#update_recovery_point_lifecycle)
         """
-
     def update_region_settings(
         self,
         *,
         ResourceTypeOptInPreference: Mapping[str, bool] = ...,
         ResourceTypeManagementPreference: Mapping[str, bool] = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates the current service opt-in settings for the Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.update_region_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#update_region_settings)
         """
-
     def update_report_plan(
         self,
         *,
         ReportPlanName: str,
         ReportPlanDescription: str = ...,
-        ReportDeliveryChannel: Union[
-            ReportDeliveryChannelTypeDef, ReportDeliveryChannelOutputTypeDef
-        ] = ...,
-        ReportSetting: Union[ReportSettingTypeDef, ReportSettingOutputTypeDef] = ...,
+        ReportDeliveryChannel: ReportDeliveryChannelUnionTypeDef = ...,
+        ReportSetting: ReportSettingUnionTypeDef = ...,
         IdempotencyToken: str = ...
     ) -> UpdateReportPlanOutputTypeDef:
         """
         Updates an existing report plan identified by its `ReportPlanName` with the
         input document in JSON format.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.update_report_plan)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#update_report_plan)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["list_backup_jobs"]) -> ListBackupJobsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_backup_plan_templates"]
     ) -> ListBackupPlanTemplatesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_backup_plan_versions"]
     ) -> ListBackupPlanVersionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_backup_plans"]
     ) -> ListBackupPlansPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_backup_selections"]
     ) -> ListBackupSelectionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_backup_vaults"]
     ) -> ListBackupVaultsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["list_copy_jobs"]) -> ListCopyJobsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["list_legal_holds"]) -> ListLegalHoldsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_protected_resources"]
     ) -> ListProtectedResourcesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_recovery_points_by_backup_vault"]
     ) -> ListRecoveryPointsByBackupVaultPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_recovery_points_by_legal_hold"]
     ) -> ListRecoveryPointsByLegalHoldPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_recovery_points_by_resource"]
     ) -> ListRecoveryPointsByResourcePaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_restore_jobs"]
     ) -> ListRestoreJobsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#get_paginator)
```

### Comparing `mypy-boto3-backup-1.28.15.post1/mypy_boto3_backup/client.pyi` & `mypy-boto3-backup-1.28.16/mypy_boto3_backup/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from mypy_boto3_backup.client import BackupClient
 
     session = Session()
     client: BackupClient = session.client("backup")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     BackupJobStateType,
     BackupVaultEventType,
     CopyJobStateType,
@@ -38,16 +37,15 @@
     ListRecoveryPointsByBackupVaultPaginator,
     ListRecoveryPointsByLegalHoldPaginator,
     ListRecoveryPointsByResourcePaginator,
     ListRestoreJobsPaginator,
 )
 from .type_defs import (
     BackupPlanInputTypeDef,
-    BackupSelectionOutputTypeDef,
-    BackupSelectionTypeDef,
+    BackupSelectionUnionTypeDef,
     CreateBackupPlanOutputTypeDef,
     CreateBackupSelectionOutputTypeDef,
     CreateBackupVaultOutputTypeDef,
     CreateFrameworkOutputTypeDef,
     CreateLegalHoldOutputTypeDef,
     CreateReportPlanOutputTypeDef,
     DeleteBackupPlanOutputTypeDef,
@@ -60,16 +58,15 @@
     DescribeRecoveryPointOutputTypeDef,
     DescribeRegionSettingsOutputTypeDef,
     DescribeReportJobOutputTypeDef,
     DescribeReportPlanOutputTypeDef,
     DescribeRestoreJobOutputTypeDef,
     EmptyResponseMetadataTypeDef,
     ExportBackupPlanTemplateOutputTypeDef,
-    FrameworkControlOutputTypeDef,
-    FrameworkControlTypeDef,
+    FrameworkControlUnionTypeDef,
     GetBackupPlanFromJSONOutputTypeDef,
     GetBackupPlanFromTemplateOutputTypeDef,
     GetBackupPlanOutputTypeDef,
     GetBackupSelectionOutputTypeDef,
     GetBackupVaultAccessPolicyOutputTypeDef,
     GetBackupVaultNotificationsOutputTypeDef,
     GetLegalHoldOutputTypeDef,
@@ -89,57 +86,59 @@
     ListRecoveryPointsByBackupVaultOutputTypeDef,
     ListRecoveryPointsByLegalHoldOutputTypeDef,
     ListRecoveryPointsByResourceOutputTypeDef,
     ListReportJobsOutputTypeDef,
     ListReportPlansOutputTypeDef,
     ListRestoreJobsOutputTypeDef,
     ListTagsOutputTypeDef,
-    RecoveryPointSelectionOutputTypeDef,
-    RecoveryPointSelectionTypeDef,
-    ReportDeliveryChannelOutputTypeDef,
-    ReportDeliveryChannelTypeDef,
-    ReportSettingOutputTypeDef,
-    ReportSettingTypeDef,
+    RecoveryPointSelectionUnionTypeDef,
+    ReportDeliveryChannelUnionTypeDef,
+    ReportSettingUnionTypeDef,
     StartBackupJobOutputTypeDef,
     StartCopyJobOutputTypeDef,
     StartReportJobOutputTypeDef,
     StartRestoreJobOutputTypeDef,
+    TimestampTypeDef,
     UpdateBackupPlanOutputTypeDef,
     UpdateFrameworkOutputTypeDef,
     UpdateRecoveryPointLifecycleOutputTypeDef,
     UpdateReportPlanOutputTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = ("BackupClient",)
 
+
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     AlreadyExistsException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     DependencyFailureException: Type[BotocoreClientError]
     InvalidParameterValueException: Type[BotocoreClientError]
     InvalidRequestException: Type[BotocoreClientError]
     InvalidResourceStateException: Type[BotocoreClientError]
     LimitExceededException: Type[BotocoreClientError]
     MissingParameterValueException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ServiceUnavailableException: Type[BotocoreClientError]
 
+
 class BackupClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/)
     """
 
     meta: ClientMeta
@@ -148,638 +147,695 @@
     def exceptions(self) -> Exceptions:
         """
         BackupClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#exceptions)
         """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#can_paginate)
         """
+
     def cancel_legal_hold(
         self, *, LegalHoldId: str, CancelDescription: str, RetainRecordInDays: int = ...
     ) -> Dict[str, Any]:
         """
         This action removes the specified legal hold on a recovery point.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.cancel_legal_hold)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#cancel_legal_hold)
         """
+
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#close)
         """
+
     def create_backup_plan(
         self,
         *,
         BackupPlan: BackupPlanInputTypeDef,
         BackupPlanTags: Mapping[str, str] = ...,
         CreatorRequestId: str = ...
     ) -> CreateBackupPlanOutputTypeDef:
         """
         Creates a backup plan using a backup plan name and backup rules.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.create_backup_plan)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#create_backup_plan)
         """
+
     def create_backup_selection(
         self,
         *,
         BackupPlanId: str,
-        BackupSelection: Union[BackupSelectionTypeDef, BackupSelectionOutputTypeDef],
+        BackupSelection: BackupSelectionUnionTypeDef,
         CreatorRequestId: str = ...
     ) -> CreateBackupSelectionOutputTypeDef:
         """
         Creates a JSON document that specifies a set of resources to assign to a backup
         plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.create_backup_selection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#create_backup_selection)
         """
+
     def create_backup_vault(
         self,
         *,
         BackupVaultName: str,
         BackupVaultTags: Mapping[str, str] = ...,
         EncryptionKeyArn: str = ...,
         CreatorRequestId: str = ...
     ) -> CreateBackupVaultOutputTypeDef:
         """
         Creates a logical container where backups are stored.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.create_backup_vault)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#create_backup_vault)
         """
+
     def create_framework(
         self,
         *,
         FrameworkName: str,
-        FrameworkControls: Sequence[Union[FrameworkControlTypeDef, FrameworkControlOutputTypeDef]],
+        FrameworkControls: Sequence[FrameworkControlUnionTypeDef],
         FrameworkDescription: str = ...,
         IdempotencyToken: str = ...,
         FrameworkTags: Mapping[str, str] = ...
     ) -> CreateFrameworkOutputTypeDef:
         """
         Creates a framework with one or more controls.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.create_framework)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#create_framework)
         """
+
     def create_legal_hold(
         self,
         *,
         Title: str,
         Description: str,
         IdempotencyToken: str = ...,
-        RecoveryPointSelection: Union[
-            RecoveryPointSelectionTypeDef, RecoveryPointSelectionOutputTypeDef
-        ] = ...,
+        RecoveryPointSelection: RecoveryPointSelectionUnionTypeDef = ...,
         Tags: Mapping[str, str] = ...
     ) -> CreateLegalHoldOutputTypeDef:
         """
         This action creates a legal hold on a recovery point (backup).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.create_legal_hold)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#create_legal_hold)
         """
+
     def create_report_plan(
         self,
         *,
         ReportPlanName: str,
-        ReportDeliveryChannel: Union[
-            ReportDeliveryChannelTypeDef, ReportDeliveryChannelOutputTypeDef
-        ],
-        ReportSetting: Union[ReportSettingTypeDef, ReportSettingOutputTypeDef],
+        ReportDeliveryChannel: ReportDeliveryChannelUnionTypeDef,
+        ReportSetting: ReportSettingUnionTypeDef,
         ReportPlanDescription: str = ...,
         ReportPlanTags: Mapping[str, str] = ...,
         IdempotencyToken: str = ...
     ) -> CreateReportPlanOutputTypeDef:
         """
         Creates a report plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.create_report_plan)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#create_report_plan)
         """
+
     def delete_backup_plan(self, *, BackupPlanId: str) -> DeleteBackupPlanOutputTypeDef:
         """
         Deletes a backup plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.delete_backup_plan)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#delete_backup_plan)
         """
+
     def delete_backup_selection(
         self, *, BackupPlanId: str, SelectionId: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the resource selection associated with a backup plan that is specified
         by the `SelectionId`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.delete_backup_selection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#delete_backup_selection)
         """
+
     def delete_backup_vault(self, *, BackupVaultName: str) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the backup vault identified by its name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.delete_backup_vault)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#delete_backup_vault)
         """
+
     def delete_backup_vault_access_policy(
         self, *, BackupVaultName: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the policy document that manages permissions on a backup vault.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.delete_backup_vault_access_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#delete_backup_vault_access_policy)
         """
+
     def delete_backup_vault_lock_configuration(
         self, *, BackupVaultName: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes Backup Vault Lock from a backup vault specified by a backup vault name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.delete_backup_vault_lock_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#delete_backup_vault_lock_configuration)
         """
+
     def delete_backup_vault_notifications(
         self, *, BackupVaultName: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes event notifications for the specified backup vault.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.delete_backup_vault_notifications)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#delete_backup_vault_notifications)
         """
+
     def delete_framework(self, *, FrameworkName: str) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the framework specified by a framework name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.delete_framework)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#delete_framework)
         """
+
     def delete_recovery_point(
         self, *, BackupVaultName: str, RecoveryPointArn: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the recovery point specified by a recovery point ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.delete_recovery_point)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#delete_recovery_point)
         """
+
     def delete_report_plan(self, *, ReportPlanName: str) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the report plan specified by a report plan name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.delete_report_plan)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#delete_report_plan)
         """
+
     def describe_backup_job(self, *, BackupJobId: str) -> DescribeBackupJobOutputTypeDef:
         """
         Returns backup job details for the specified `BackupJobId`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.describe_backup_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#describe_backup_job)
         """
+
     def describe_backup_vault(self, *, BackupVaultName: str) -> DescribeBackupVaultOutputTypeDef:
         """
         Returns metadata about a backup vault specified by its name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.describe_backup_vault)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#describe_backup_vault)
         """
+
     def describe_copy_job(self, *, CopyJobId: str) -> DescribeCopyJobOutputTypeDef:
         """
         Returns metadata associated with creating a copy of a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.describe_copy_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#describe_copy_job)
         """
+
     def describe_framework(self, *, FrameworkName: str) -> DescribeFrameworkOutputTypeDef:
         """
         Returns the framework details for the specified `FrameworkName`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.describe_framework)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#describe_framework)
         """
+
     def describe_global_settings(self) -> DescribeGlobalSettingsOutputTypeDef:
         """
         Describes whether the Amazon Web Services account is opted in to cross-account
         backup.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.describe_global_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#describe_global_settings)
         """
+
     def describe_protected_resource(
         self, *, ResourceArn: str
     ) -> DescribeProtectedResourceOutputTypeDef:
         """
         Returns information about a saved resource, including the last time it was
         backed up, its Amazon Resource Name (ARN), and the Amazon Web Services service
         type of the saved resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.describe_protected_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#describe_protected_resource)
         """
+
     def describe_recovery_point(
         self, *, BackupVaultName: str, RecoveryPointArn: str
     ) -> DescribeRecoveryPointOutputTypeDef:
         """
         Returns metadata associated with a recovery point, including ID, status,
         encryption, and lifecycle.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.describe_recovery_point)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#describe_recovery_point)
         """
+
     def describe_region_settings(self) -> DescribeRegionSettingsOutputTypeDef:
         """
         Returns the current service opt-in settings for the Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.describe_region_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#describe_region_settings)
         """
+
     def describe_report_job(self, *, ReportJobId: str) -> DescribeReportJobOutputTypeDef:
         """
         Returns the details associated with creating a report as specified by its
         `ReportJobId`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.describe_report_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#describe_report_job)
         """
+
     def describe_report_plan(self, *, ReportPlanName: str) -> DescribeReportPlanOutputTypeDef:
         """
         Returns a list of all report plans for an Amazon Web Services account and Amazon
         Web Services Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.describe_report_plan)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#describe_report_plan)
         """
+
     def describe_restore_job(self, *, RestoreJobId: str) -> DescribeRestoreJobOutputTypeDef:
         """
         Returns metadata associated with a restore job that is specified by a job ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.describe_restore_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#describe_restore_job)
         """
+
     def disassociate_recovery_point(
         self, *, BackupVaultName: str, RecoveryPointArn: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the specified continuous backup recovery point from Backup and releases
         control of that continuous backup to the source service, such as Amazon RDS.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.disassociate_recovery_point)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#disassociate_recovery_point)
         """
+
     def disassociate_recovery_point_from_parent(
         self, *, BackupVaultName: str, RecoveryPointArn: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         This action to a specific child (nested) recovery point removes the relationship
         between the specified recovery point and its parent (composite) recovery point.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.disassociate_recovery_point_from_parent)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#disassociate_recovery_point_from_parent)
         """
+
     def export_backup_plan_template(
         self, *, BackupPlanId: str
     ) -> ExportBackupPlanTemplateOutputTypeDef:
         """
         Returns the backup plan that is specified by the plan ID as a backup template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.export_backup_plan_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#export_backup_plan_template)
         """
+
     def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#generate_presigned_url)
         """
+
     def get_backup_plan(
         self, *, BackupPlanId: str, VersionId: str = ...
     ) -> GetBackupPlanOutputTypeDef:
         """
         Returns `BackupPlan` details for the specified `BackupPlanId`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.get_backup_plan)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#get_backup_plan)
         """
+
     def get_backup_plan_from_json(
         self, *, BackupPlanTemplateJson: str
     ) -> GetBackupPlanFromJSONOutputTypeDef:
         """
         Returns a valid JSON document specifying a backup plan or an error.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.get_backup_plan_from_json)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#get_backup_plan_from_json)
         """
+
     def get_backup_plan_from_template(
         self, *, BackupPlanTemplateId: str
     ) -> GetBackupPlanFromTemplateOutputTypeDef:
         """
         Returns the template specified by its `templateId` as a backup plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.get_backup_plan_from_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#get_backup_plan_from_template)
         """
+
     def get_backup_selection(
         self, *, BackupPlanId: str, SelectionId: str
     ) -> GetBackupSelectionOutputTypeDef:
         """
         Returns selection metadata and a document in JSON format that specifies a list
         of resources that are associated with a backup plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.get_backup_selection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#get_backup_selection)
         """
+
     def get_backup_vault_access_policy(
         self, *, BackupVaultName: str
     ) -> GetBackupVaultAccessPolicyOutputTypeDef:
         """
         Returns the access policy document that is associated with the named backup
         vault.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.get_backup_vault_access_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#get_backup_vault_access_policy)
         """
+
     def get_backup_vault_notifications(
         self, *, BackupVaultName: str
     ) -> GetBackupVaultNotificationsOutputTypeDef:
         """
         Returns event notifications for the specified backup vault.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.get_backup_vault_notifications)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#get_backup_vault_notifications)
         """
+
     def get_legal_hold(self, *, LegalHoldId: str) -> GetLegalHoldOutputTypeDef:
         """
         This action returns details for a specified legal hold.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.get_legal_hold)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#get_legal_hold)
         """
+
     def get_recovery_point_restore_metadata(
         self, *, BackupVaultName: str, RecoveryPointArn: str
     ) -> GetRecoveryPointRestoreMetadataOutputTypeDef:
         """
         Returns a set of metadata key-value pairs that were used to create the backup.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.get_recovery_point_restore_metadata)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#get_recovery_point_restore_metadata)
         """
+
     def get_supported_resource_types(self) -> GetSupportedResourceTypesOutputTypeDef:
         """
         Returns the Amazon Web Services resource types supported by Backup.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.get_supported_resource_types)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#get_supported_resource_types)
         """
+
     def list_backup_jobs(
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
         ByResourceArn: str = ...,
         ByState: BackupJobStateType = ...,
         ByBackupVaultName: str = ...,
-        ByCreatedBefore: Union[datetime, str] = ...,
-        ByCreatedAfter: Union[datetime, str] = ...,
+        ByCreatedBefore: TimestampTypeDef = ...,
+        ByCreatedAfter: TimestampTypeDef = ...,
         ByResourceType: str = ...,
         ByAccountId: str = ...,
-        ByCompleteAfter: Union[datetime, str] = ...,
-        ByCompleteBefore: Union[datetime, str] = ...,
+        ByCompleteAfter: TimestampTypeDef = ...,
+        ByCompleteBefore: TimestampTypeDef = ...,
         ByParentJobId: str = ...
     ) -> ListBackupJobsOutputTypeDef:
         """
         Returns a list of existing backup jobs for an authenticated account for the last
         30 days.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.list_backup_jobs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#list_backup_jobs)
         """
+
     def list_backup_plan_templates(
         self, *, NextToken: str = ..., MaxResults: int = ...
     ) -> ListBackupPlanTemplatesOutputTypeDef:
         """
         Returns metadata of your saved backup plan templates, including the template ID,
         name, and the creation and deletion dates.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.list_backup_plan_templates)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#list_backup_plan_templates)
         """
+
     def list_backup_plan_versions(
         self, *, BackupPlanId: str, NextToken: str = ..., MaxResults: int = ...
     ) -> ListBackupPlanVersionsOutputTypeDef:
         """
         Returns version metadata of your backup plans, including Amazon Resource Names
         (ARNs), backup plan IDs, creation and deletion dates, plan names, and version
         IDs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.list_backup_plan_versions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#list_backup_plan_versions)
         """
+
     def list_backup_plans(
         self, *, NextToken: str = ..., MaxResults: int = ..., IncludeDeleted: bool = ...
     ) -> ListBackupPlansOutputTypeDef:
         """
         Returns a list of all active backup plans for an authenticated account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.list_backup_plans)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#list_backup_plans)
         """
+
     def list_backup_selections(
         self, *, BackupPlanId: str, NextToken: str = ..., MaxResults: int = ...
     ) -> ListBackupSelectionsOutputTypeDef:
         """
         Returns an array containing metadata of the resources associated with the target
         backup plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.list_backup_selections)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#list_backup_selections)
         """
+
     def list_backup_vaults(
         self, *, NextToken: str = ..., MaxResults: int = ...
     ) -> ListBackupVaultsOutputTypeDef:
         """
         Returns a list of recovery point storage containers along with information about
         them.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.list_backup_vaults)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#list_backup_vaults)
         """
+
     def list_copy_jobs(
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
         ByResourceArn: str = ...,
         ByState: CopyJobStateType = ...,
-        ByCreatedBefore: Union[datetime, str] = ...,
-        ByCreatedAfter: Union[datetime, str] = ...,
+        ByCreatedBefore: TimestampTypeDef = ...,
+        ByCreatedAfter: TimestampTypeDef = ...,
         ByResourceType: str = ...,
         ByDestinationVaultArn: str = ...,
         ByAccountId: str = ...,
-        ByCompleteBefore: Union[datetime, str] = ...,
-        ByCompleteAfter: Union[datetime, str] = ...,
+        ByCompleteBefore: TimestampTypeDef = ...,
+        ByCompleteAfter: TimestampTypeDef = ...,
         ByParentJobId: str = ...
     ) -> ListCopyJobsOutputTypeDef:
         """
         Returns metadata about your copy jobs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.list_copy_jobs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#list_copy_jobs)
         """
+
     def list_frameworks(
         self, *, MaxResults: int = ..., NextToken: str = ...
     ) -> ListFrameworksOutputTypeDef:
         """
         Returns a list of all frameworks for an Amazon Web Services account and Amazon
         Web Services Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.list_frameworks)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#list_frameworks)
         """
+
     def list_legal_holds(
         self, *, NextToken: str = ..., MaxResults: int = ...
     ) -> ListLegalHoldsOutputTypeDef:
         """
         This action returns metadata about active and previous legal holds.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.list_legal_holds)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#list_legal_holds)
         """
+
     def list_protected_resources(
         self, *, NextToken: str = ..., MaxResults: int = ...
     ) -> ListProtectedResourcesOutputTypeDef:
         """
         Returns an array of resources successfully backed up by Backup, including the
         time the resource was saved, an Amazon Resource Name (ARN) of the resource, and
         a resource type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.list_protected_resources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#list_protected_resources)
         """
+
     def list_recovery_points_by_backup_vault(
         self,
         *,
         BackupVaultName: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         ByResourceArn: str = ...,
         ByResourceType: str = ...,
         ByBackupPlanId: str = ...,
-        ByCreatedBefore: Union[datetime, str] = ...,
-        ByCreatedAfter: Union[datetime, str] = ...,
+        ByCreatedBefore: TimestampTypeDef = ...,
+        ByCreatedAfter: TimestampTypeDef = ...,
         ByParentRecoveryPointArn: str = ...
     ) -> ListRecoveryPointsByBackupVaultOutputTypeDef:
         """
         Returns detailed information about the recovery points stored in a backup vault.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.list_recovery_points_by_backup_vault)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#list_recovery_points_by_backup_vault)
         """
+
     def list_recovery_points_by_legal_hold(
         self, *, LegalHoldId: str, NextToken: str = ..., MaxResults: int = ...
     ) -> ListRecoveryPointsByLegalHoldOutputTypeDef:
         """
         This action returns recovery point ARNs (Amazon Resource Names) of the specified
         legal hold.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.list_recovery_points_by_legal_hold)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#list_recovery_points_by_legal_hold)
         """
+
     def list_recovery_points_by_resource(
         self, *, ResourceArn: str, NextToken: str = ..., MaxResults: int = ...
     ) -> ListRecoveryPointsByResourceOutputTypeDef:
         """
         Returns detailed information about all the recovery points of the type specified
         by a resource Amazon Resource Name (ARN).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.list_recovery_points_by_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#list_recovery_points_by_resource)
         """
+
     def list_report_jobs(
         self,
         *,
         ByReportPlanName: str = ...,
-        ByCreationBefore: Union[datetime, str] = ...,
-        ByCreationAfter: Union[datetime, str] = ...,
+        ByCreationBefore: TimestampTypeDef = ...,
+        ByCreationAfter: TimestampTypeDef = ...,
         ByStatus: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> ListReportJobsOutputTypeDef:
         """
         Returns details about your report jobs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.list_report_jobs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#list_report_jobs)
         """
+
     def list_report_plans(
         self, *, MaxResults: int = ..., NextToken: str = ...
     ) -> ListReportPlansOutputTypeDef:
         """
         Returns a list of your report plans.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.list_report_plans)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#list_report_plans)
         """
+
     def list_restore_jobs(
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
         ByAccountId: str = ...,
-        ByCreatedBefore: Union[datetime, str] = ...,
-        ByCreatedAfter: Union[datetime, str] = ...,
+        ByCreatedBefore: TimestampTypeDef = ...,
+        ByCreatedAfter: TimestampTypeDef = ...,
         ByStatus: RestoreJobStatusType = ...,
-        ByCompleteBefore: Union[datetime, str] = ...,
-        ByCompleteAfter: Union[datetime, str] = ...
+        ByCompleteBefore: TimestampTypeDef = ...,
+        ByCompleteAfter: TimestampTypeDef = ...
     ) -> ListRestoreJobsOutputTypeDef:
         """
         Returns a list of jobs that Backup initiated to restore a saved resource,
         including details about the recovery process.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.list_restore_jobs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#list_restore_jobs)
         """
+
     def list_tags(
         self, *, ResourceArn: str, NextToken: str = ..., MaxResults: int = ...
     ) -> ListTagsOutputTypeDef:
         """
         Returns a list of key-value pairs assigned to a target recovery point, backup
         plan, or backup vault.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.list_tags)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#list_tags)
         """
+
     def put_backup_vault_access_policy(
         self, *, BackupVaultName: str, Policy: str = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Sets a resource-based policy that is used to manage access permissions on the
         target backup vault.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.put_backup_vault_access_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#put_backup_vault_access_policy)
         """
+
     def put_backup_vault_lock_configuration(
         self,
         *,
         BackupVaultName: str,
         MinRetentionDays: int = ...,
         MaxRetentionDays: int = ...,
         ChangeableForDays: int = ...
@@ -787,27 +843,29 @@
         """
         Applies Backup Vault Lock to a backup vault, preventing attempts to delete any
         recovery point stored in or created in a backup vault.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.put_backup_vault_lock_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#put_backup_vault_lock_configuration)
         """
+
     def put_backup_vault_notifications(
         self,
         *,
         BackupVaultName: str,
         SNSTopicArn: str,
         BackupVaultEvents: Sequence[BackupVaultEventType]
     ) -> EmptyResponseMetadataTypeDef:
         """
         Turns on notifications on a backup vault for the specified topic and events.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.put_backup_vault_notifications)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#put_backup_vault_notifications)
         """
+
     def start_backup_job(
         self,
         *,
         BackupVaultName: str,
         ResourceArn: str,
         IamRoleArn: str,
         IdempotencyToken: str = ...,
@@ -819,14 +877,15 @@
     ) -> StartBackupJobOutputTypeDef:
         """
         Starts an on-demand backup job for the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.start_backup_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#start_backup_job)
         """
+
     def start_copy_job(
         self,
         *,
         RecoveryPointArn: str,
         SourceBackupVaultName: str,
         DestinationBackupVaultArn: str,
         IamRoleArn: str,
@@ -835,23 +894,25 @@
     ) -> StartCopyJobOutputTypeDef:
         """
         Starts a job to create a one-time copy of the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.start_copy_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#start_copy_job)
         """
+
     def start_report_job(
         self, *, ReportPlanName: str, IdempotencyToken: str = ...
     ) -> StartReportJobOutputTypeDef:
         """
         Starts an on-demand report job for the specified report plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.start_report_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#start_report_job)
         """
+
     def start_restore_job(
         self,
         *,
         RecoveryPointArn: str,
         Metadata: Mapping[str, str],
         IamRoleArn: str = ...,
         IdempotencyToken: str = ...,
@@ -860,208 +921,226 @@
     ) -> StartRestoreJobOutputTypeDef:
         """
         Recovers the saved resource identified by an Amazon Resource Name (ARN).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.start_restore_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#start_restore_job)
         """
+
     def stop_backup_job(self, *, BackupJobId: str) -> EmptyResponseMetadataTypeDef:
         """
         Attempts to cancel a job to create a one-time backup of a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.stop_backup_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#stop_backup_job)
         """
+
     def tag_resource(
         self, *, ResourceArn: str, Tags: Mapping[str, str]
     ) -> EmptyResponseMetadataTypeDef:
         """
         Assigns a set of key-value pairs to a recovery point, backup plan, or backup
         vault identified by an Amazon Resource Name (ARN).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#tag_resource)
         """
+
     def untag_resource(
         self, *, ResourceArn: str, TagKeyList: Sequence[str]
     ) -> EmptyResponseMetadataTypeDef:
         """
         Removes a set of key-value pairs from a recovery point, backup plan, or backup
         vault identified by an Amazon Resource Name (ARN) See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/backup-2018-11-15/UntagResource).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#untag_resource)
         """
+
     def update_backup_plan(
         self, *, BackupPlanId: str, BackupPlan: BackupPlanInputTypeDef
     ) -> UpdateBackupPlanOutputTypeDef:
         """
         Updates an existing backup plan identified by its `backupPlanId` with the input
         document in JSON format.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.update_backup_plan)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#update_backup_plan)
         """
+
     def update_framework(
         self,
         *,
         FrameworkName: str,
         FrameworkDescription: str = ...,
-        FrameworkControls: Sequence[
-            Union[FrameworkControlTypeDef, FrameworkControlOutputTypeDef]
-        ] = ...,
+        FrameworkControls: Sequence[FrameworkControlUnionTypeDef] = ...,
         IdempotencyToken: str = ...
     ) -> UpdateFrameworkOutputTypeDef:
         """
         Updates an existing framework identified by its `FrameworkName` with the input
         document in JSON format.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.update_framework)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#update_framework)
         """
+
     def update_global_settings(
         self, *, GlobalSettings: Mapping[str, str] = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates whether the Amazon Web Services account is opted in to cross-account
         backup.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.update_global_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#update_global_settings)
         """
+
     def update_recovery_point_lifecycle(
         self, *, BackupVaultName: str, RecoveryPointArn: str, Lifecycle: LifecycleTypeDef = ...
     ) -> UpdateRecoveryPointLifecycleOutputTypeDef:
         """
         Sets the transition lifecycle of a recovery point.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.update_recovery_point_lifecycle)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#update_recovery_point_lifecycle)
         """
+
     def update_region_settings(
         self,
         *,
         ResourceTypeOptInPreference: Mapping[str, bool] = ...,
         ResourceTypeManagementPreference: Mapping[str, bool] = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates the current service opt-in settings for the Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.update_region_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#update_region_settings)
         """
+
     def update_report_plan(
         self,
         *,
         ReportPlanName: str,
         ReportPlanDescription: str = ...,
-        ReportDeliveryChannel: Union[
-            ReportDeliveryChannelTypeDef, ReportDeliveryChannelOutputTypeDef
-        ] = ...,
-        ReportSetting: Union[ReportSettingTypeDef, ReportSettingOutputTypeDef] = ...,
+        ReportDeliveryChannel: ReportDeliveryChannelUnionTypeDef = ...,
+        ReportSetting: ReportSettingUnionTypeDef = ...,
         IdempotencyToken: str = ...
     ) -> UpdateReportPlanOutputTypeDef:
         """
         Updates an existing report plan identified by its `ReportPlanName` with the
         input document in JSON format.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.update_report_plan)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#update_report_plan)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["list_backup_jobs"]) -> ListBackupJobsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_backup_plan_templates"]
     ) -> ListBackupPlanTemplatesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_backup_plan_versions"]
     ) -> ListBackupPlanVersionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_backup_plans"]
     ) -> ListBackupPlansPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_backup_selections"]
     ) -> ListBackupSelectionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_backup_vaults"]
     ) -> ListBackupVaultsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["list_copy_jobs"]) -> ListCopyJobsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["list_legal_holds"]) -> ListLegalHoldsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_protected_resources"]
     ) -> ListProtectedResourcesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_recovery_points_by_backup_vault"]
     ) -> ListRecoveryPointsByBackupVaultPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_recovery_points_by_legal_hold"]
     ) -> ListRecoveryPointsByLegalHoldPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_recovery_points_by_resource"]
     ) -> ListRecoveryPointsByResourcePaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_restore_jobs"]
     ) -> ListRestoreJobsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/client/#get_paginator)
```

### Comparing `mypy-boto3-backup-1.28.15.post1/mypy_boto3_backup/literals.py` & `mypy-boto3-backup-1.28.16/mypy_boto3_backup/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-backup-1.28.15.post1/mypy_boto3_backup/literals.pyi` & `mypy-boto3-backup-1.28.16/mypy_boto3_backup/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-backup-1.28.15.post1/mypy_boto3_backup/paginator.py` & `mypy-boto3-backup-1.28.16/mypy_boto3_backup/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,16 +39,15 @@
     list_protected_resources_paginator: ListProtectedResourcesPaginator = client.get_paginator("list_protected_resources")
     list_recovery_points_by_backup_vault_paginator: ListRecoveryPointsByBackupVaultPaginator = client.get_paginator("list_recovery_points_by_backup_vault")
     list_recovery_points_by_legal_hold_paginator: ListRecoveryPointsByLegalHoldPaginator = client.get_paginator("list_recovery_points_by_legal_hold")
     list_recovery_points_by_resource_paginator: ListRecoveryPointsByResourcePaginator = client.get_paginator("list_recovery_points_by_resource")
     list_restore_jobs_paginator: ListRestoreJobsPaginator = client.get_paginator("list_restore_jobs")
     ```
 """
-from datetime import datetime
-from typing import Generic, Iterator, TypeVar, Union
+from typing import Generic, Iterator, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import BackupJobStateType, CopyJobStateType, RestoreJobStatusType
 from .type_defs import (
     ListBackupJobsOutputTypeDef,
     ListBackupPlansOutputTypeDef,
@@ -60,14 +59,15 @@
     ListLegalHoldsOutputTypeDef,
     ListProtectedResourcesOutputTypeDef,
     ListRecoveryPointsByBackupVaultOutputTypeDef,
     ListRecoveryPointsByLegalHoldOutputTypeDef,
     ListRecoveryPointsByResourceOutputTypeDef,
     ListRestoreJobsOutputTypeDef,
     PaginatorConfigTypeDef,
+    TimestampTypeDef,
 )
 
 __all__ = (
     "ListBackupJobsPaginator",
     "ListBackupPlanTemplatesPaginator",
     "ListBackupPlanVersionsPaginator",
     "ListBackupPlansPaginator",
@@ -101,20 +101,20 @@
 
     def paginate(
         self,
         *,
         ByResourceArn: str = ...,
         ByState: BackupJobStateType = ...,
         ByBackupVaultName: str = ...,
-        ByCreatedBefore: Union[datetime, str] = ...,
-        ByCreatedAfter: Union[datetime, str] = ...,
+        ByCreatedBefore: TimestampTypeDef = ...,
+        ByCreatedAfter: TimestampTypeDef = ...,
         ByResourceType: str = ...,
         ByAccountId: str = ...,
-        ByCompleteAfter: Union[datetime, str] = ...,
-        ByCompleteBefore: Union[datetime, str] = ...,
+        ByCompleteAfter: TimestampTypeDef = ...,
+        ByCompleteBefore: TimestampTypeDef = ...,
         ByParentJobId: str = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListBackupJobsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListBackupJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/paginators/#listbackupjobspaginator)
         """
@@ -202,21 +202,21 @@
     """
 
     def paginate(
         self,
         *,
         ByResourceArn: str = ...,
         ByState: CopyJobStateType = ...,
-        ByCreatedBefore: Union[datetime, str] = ...,
-        ByCreatedAfter: Union[datetime, str] = ...,
+        ByCreatedBefore: TimestampTypeDef = ...,
+        ByCreatedAfter: TimestampTypeDef = ...,
         ByResourceType: str = ...,
         ByDestinationVaultArn: str = ...,
         ByAccountId: str = ...,
-        ByCompleteBefore: Union[datetime, str] = ...,
-        ByCompleteAfter: Union[datetime, str] = ...,
+        ByCompleteBefore: TimestampTypeDef = ...,
+        ByCompleteAfter: TimestampTypeDef = ...,
         ByParentJobId: str = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListCopyJobsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListCopyJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/paginators/#listcopyjobspaginator)
         """
@@ -261,16 +261,16 @@
     def paginate(
         self,
         *,
         BackupVaultName: str,
         ByResourceArn: str = ...,
         ByResourceType: str = ...,
         ByBackupPlanId: str = ...,
-        ByCreatedBefore: Union[datetime, str] = ...,
-        ByCreatedAfter: Union[datetime, str] = ...,
+        ByCreatedBefore: TimestampTypeDef = ...,
+        ByCreatedAfter: TimestampTypeDef = ...,
         ByParentRecoveryPointArn: str = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRecoveryPointsByBackupVaultOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListRecoveryPointsByBackupVault.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/paginators/#listrecoverypointsbybackupvaultpaginator)
         """
@@ -312,18 +312,18 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/paginators/#listrestorejobspaginator)
     """
 
     def paginate(
         self,
         *,
         ByAccountId: str = ...,
-        ByCreatedBefore: Union[datetime, str] = ...,
-        ByCreatedAfter: Union[datetime, str] = ...,
+        ByCreatedBefore: TimestampTypeDef = ...,
+        ByCreatedAfter: TimestampTypeDef = ...,
         ByStatus: RestoreJobStatusType = ...,
-        ByCompleteBefore: Union[datetime, str] = ...,
-        ByCompleteAfter: Union[datetime, str] = ...,
+        ByCompleteBefore: TimestampTypeDef = ...,
+        ByCompleteAfter: TimestampTypeDef = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRestoreJobsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListRestoreJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/paginators/#listrestorejobspaginator)
         """
```

### Comparing `mypy-boto3-backup-1.28.15.post1/mypy_boto3_backup/paginator.pyi` & `mypy-boto3-backup-1.28.16/mypy_boto3_backup/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -39,16 +39,15 @@
     list_protected_resources_paginator: ListProtectedResourcesPaginator = client.get_paginator("list_protected_resources")
     list_recovery_points_by_backup_vault_paginator: ListRecoveryPointsByBackupVaultPaginator = client.get_paginator("list_recovery_points_by_backup_vault")
     list_recovery_points_by_legal_hold_paginator: ListRecoveryPointsByLegalHoldPaginator = client.get_paginator("list_recovery_points_by_legal_hold")
     list_recovery_points_by_resource_paginator: ListRecoveryPointsByResourcePaginator = client.get_paginator("list_recovery_points_by_resource")
     list_restore_jobs_paginator: ListRestoreJobsPaginator = client.get_paginator("list_restore_jobs")
     ```
 """
-from datetime import datetime
-from typing import Generic, Iterator, TypeVar, Union
+from typing import Generic, Iterator, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import BackupJobStateType, CopyJobStateType, RestoreJobStatusType
 from .type_defs import (
     ListBackupJobsOutputTypeDef,
     ListBackupPlansOutputTypeDef,
@@ -60,14 +59,15 @@
     ListLegalHoldsOutputTypeDef,
     ListProtectedResourcesOutputTypeDef,
     ListRecoveryPointsByBackupVaultOutputTypeDef,
     ListRecoveryPointsByLegalHoldOutputTypeDef,
     ListRecoveryPointsByResourceOutputTypeDef,
     ListRestoreJobsOutputTypeDef,
     PaginatorConfigTypeDef,
+    TimestampTypeDef,
 )
 
 __all__ = (
     "ListBackupJobsPaginator",
     "ListBackupPlanTemplatesPaginator",
     "ListBackupPlanVersionsPaginator",
     "ListBackupPlansPaginator",
@@ -98,20 +98,20 @@
 
     def paginate(
         self,
         *,
         ByResourceArn: str = ...,
         ByState: BackupJobStateType = ...,
         ByBackupVaultName: str = ...,
-        ByCreatedBefore: Union[datetime, str] = ...,
-        ByCreatedAfter: Union[datetime, str] = ...,
+        ByCreatedBefore: TimestampTypeDef = ...,
+        ByCreatedAfter: TimestampTypeDef = ...,
         ByResourceType: str = ...,
         ByAccountId: str = ...,
-        ByCompleteAfter: Union[datetime, str] = ...,
-        ByCompleteBefore: Union[datetime, str] = ...,
+        ByCompleteAfter: TimestampTypeDef = ...,
+        ByCompleteBefore: TimestampTypeDef = ...,
         ByParentJobId: str = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListBackupJobsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListBackupJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/paginators/#listbackupjobspaginator)
         """
@@ -193,21 +193,21 @@
     """
 
     def paginate(
         self,
         *,
         ByResourceArn: str = ...,
         ByState: CopyJobStateType = ...,
-        ByCreatedBefore: Union[datetime, str] = ...,
-        ByCreatedAfter: Union[datetime, str] = ...,
+        ByCreatedBefore: TimestampTypeDef = ...,
+        ByCreatedAfter: TimestampTypeDef = ...,
         ByResourceType: str = ...,
         ByDestinationVaultArn: str = ...,
         ByAccountId: str = ...,
-        ByCompleteBefore: Union[datetime, str] = ...,
-        ByCompleteAfter: Union[datetime, str] = ...,
+        ByCompleteBefore: TimestampTypeDef = ...,
+        ByCompleteAfter: TimestampTypeDef = ...,
         ByParentJobId: str = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListCopyJobsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListCopyJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/paginators/#listcopyjobspaginator)
         """
@@ -249,16 +249,16 @@
     def paginate(
         self,
         *,
         BackupVaultName: str,
         ByResourceArn: str = ...,
         ByResourceType: str = ...,
         ByBackupPlanId: str = ...,
-        ByCreatedBefore: Union[datetime, str] = ...,
-        ByCreatedAfter: Union[datetime, str] = ...,
+        ByCreatedBefore: TimestampTypeDef = ...,
+        ByCreatedAfter: TimestampTypeDef = ...,
         ByParentRecoveryPointArn: str = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRecoveryPointsByBackupVaultOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListRecoveryPointsByBackupVault.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/paginators/#listrecoverypointsbybackupvaultpaginator)
         """
@@ -297,18 +297,18 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/paginators/#listrestorejobspaginator)
     """
 
     def paginate(
         self,
         *,
         ByAccountId: str = ...,
-        ByCreatedBefore: Union[datetime, str] = ...,
-        ByCreatedAfter: Union[datetime, str] = ...,
+        ByCreatedBefore: TimestampTypeDef = ...,
+        ByCreatedAfter: TimestampTypeDef = ...,
         ByStatus: RestoreJobStatusType = ...,
-        ByCompleteBefore: Union[datetime, str] = ...,
-        ByCompleteAfter: Union[datetime, str] = ...,
+        ByCompleteBefore: TimestampTypeDef = ...,
+        ByCompleteAfter: TimestampTypeDef = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRestoreJobsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListRestoreJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/paginators/#listrestorejobspaginator)
         """
```

### Comparing `mypy-boto3-backup-1.28.15.post1/mypy_boto3_backup/type_defs.py` & `mypy-boto3-backup-1.28.16/mypy_boto3_backup/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_backup.type_defs import AdvancedBackupSettingOutputTypeDef
 
-    data: AdvancedBackupSettingOutputTypeDef = {...}
+    data: AdvancedBackupSettingOutputTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -51,15 +51,15 @@
     "ControlScopeOutputTypeDef",
     "ControlScopeTypeDef",
     "ResponseMetadataTypeDef",
     "CreateBackupVaultInputRequestTypeDef",
     "ReportDeliveryChannelTypeDef",
     "ReportSettingTypeDef",
     "DateRangeOutputTypeDef",
-    "DateRangeTypeDef",
+    "TimestampTypeDef",
     "DeleteBackupPlanInputRequestTypeDef",
     "DeleteBackupSelectionInputRequestTypeDef",
     "DeleteBackupVaultAccessPolicyInputRequestTypeDef",
     "DeleteBackupVaultInputRequestTypeDef",
     "DeleteBackupVaultLockConfigurationInputRequestTypeDef",
     "DeleteBackupVaultNotificationsInputRequestTypeDef",
     "DeleteFrameworkInputRequestTypeDef",
@@ -84,33 +84,28 @@
     "GetBackupSelectionInputRequestTypeDef",
     "GetBackupVaultAccessPolicyInputRequestTypeDef",
     "GetBackupVaultNotificationsInputRequestTypeDef",
     "GetLegalHoldInputRequestTypeDef",
     "GetRecoveryPointRestoreMetadataInputRequestTypeDef",
     "LegalHoldTypeDef",
     "PaginatorConfigTypeDef",
-    "ListBackupJobsInputRequestTypeDef",
     "ListBackupPlanTemplatesInputRequestTypeDef",
     "ListBackupPlanVersionsInputRequestTypeDef",
     "ListBackupPlansInputRequestTypeDef",
     "ListBackupSelectionsInputRequestTypeDef",
     "ListBackupVaultsInputRequestTypeDef",
-    "ListCopyJobsInputRequestTypeDef",
     "ListFrameworksInputRequestTypeDef",
     "ListLegalHoldsInputRequestTypeDef",
     "ListProtectedResourcesInputRequestTypeDef",
     "ProtectedResourceTypeDef",
-    "ListRecoveryPointsByBackupVaultInputRequestTypeDef",
     "ListRecoveryPointsByLegalHoldInputRequestTypeDef",
     "RecoveryPointMemberTypeDef",
     "ListRecoveryPointsByResourceInputRequestTypeDef",
     "RecoveryPointByResourceTypeDef",
-    "ListReportJobsInputRequestTypeDef",
     "ListReportPlansInputRequestTypeDef",
-    "ListRestoreJobsInputRequestTypeDef",
     "RestoreJobsListMemberTypeDef",
     "ListTagsInputRequestTypeDef",
     "PutBackupVaultAccessPolicyInputRequestTypeDef",
     "PutBackupVaultLockConfigurationInputRequestTypeDef",
     "PutBackupVaultNotificationsInputRequestTypeDef",
     "ReportDeliveryChannelOutputTypeDef",
     "ReportDestinationTypeDef",
@@ -164,15 +159,20 @@
     "UpdateBackupPlanOutputTypeDef",
     "UpdateFrameworkOutputTypeDef",
     "UpdateRecoveryPointLifecycleOutputTypeDef",
     "UpdateReportPlanOutputTypeDef",
     "CreateReportPlanInputRequestTypeDef",
     "UpdateReportPlanInputRequestTypeDef",
     "RecoveryPointSelectionOutputTypeDef",
-    "RecoveryPointSelectionTypeDef",
+    "DateRangeTypeDef",
+    "ListBackupJobsInputRequestTypeDef",
+    "ListCopyJobsInputRequestTypeDef",
+    "ListRecoveryPointsByBackupVaultInputRequestTypeDef",
+    "ListReportJobsInputRequestTypeDef",
+    "ListRestoreJobsInputRequestTypeDef",
     "ListFrameworksOutputTypeDef",
     "ListLegalHoldsOutputTypeDef",
     "ListBackupJobsInputListBackupJobsPaginateTypeDef",
     "ListBackupPlanTemplatesInputListBackupPlanTemplatesPaginateTypeDef",
     "ListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef",
     "ListBackupPlansInputListBackupPlansPaginateTypeDef",
     "ListBackupSelectionsInputListBackupSelectionsPaginateTypeDef",
@@ -184,40 +184,46 @@
     "ListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef",
     "ListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef",
     "ListRestoreJobsInputListRestoreJobsPaginateTypeDef",
     "ListProtectedResourcesOutputTypeDef",
     "ListRecoveryPointsByLegalHoldOutputTypeDef",
     "ListRecoveryPointsByResourceOutputTypeDef",
     "ListRestoreJobsOutputTypeDef",
+    "ReportDeliveryChannelUnionTypeDef",
     "ReportJobTypeDef",
     "ReportPlanTypeDef",
+    "ReportSettingUnionTypeDef",
     "ListBackupPlanVersionsOutputTypeDef",
     "ListBackupPlansOutputTypeDef",
     "ListBackupJobsOutputTypeDef",
     "DescribeCopyJobOutputTypeDef",
     "ListCopyJobsOutputTypeDef",
     "BackupRuleInputTypeDef",
     "BackupRuleTypeDef",
     "ListRecoveryPointsByBackupVaultOutputTypeDef",
     "BackupSelectionOutputTypeDef",
     "BackupSelectionTypeDef",
     "DescribeFrameworkOutputTypeDef",
-    "CreateFrameworkInputRequestTypeDef",
-    "UpdateFrameworkInputRequestTypeDef",
+    "FrameworkControlUnionTypeDef",
     "CreateLegalHoldOutputTypeDef",
     "GetLegalHoldOutputTypeDef",
-    "CreateLegalHoldInputRequestTypeDef",
+    "RecoveryPointSelectionTypeDef",
     "DescribeReportJobOutputTypeDef",
     "ListReportJobsOutputTypeDef",
     "DescribeReportPlanOutputTypeDef",
     "ListReportPlansOutputTypeDef",
     "BackupPlanInputTypeDef",
     "BackupPlanTypeDef",
     "GetBackupSelectionOutputTypeDef",
+    "BackupSelectionUnionTypeDef",
     "CreateBackupSelectionInputRequestTypeDef",
+    "CreateFrameworkInputRequestTypeDef",
+    "UpdateFrameworkInputRequestTypeDef",
+    "CreateLegalHoldInputRequestTypeDef",
+    "RecoveryPointSelectionUnionTypeDef",
     "CreateBackupPlanInputRequestTypeDef",
     "UpdateBackupPlanInputRequestTypeDef",
     "GetBackupPlanFromJSONOutputTypeDef",
     "GetBackupPlanFromTemplateOutputTypeDef",
     "GetBackupPlanOutputTypeDef",
 )
 
@@ -459,22 +465,15 @@
     "DateRangeOutputTypeDef",
     {
         "FromDate": datetime,
         "ToDate": datetime,
     },
 )
 
-DateRangeTypeDef = TypedDict(
-    "DateRangeTypeDef",
-    {
-        "FromDate": Union[datetime, str],
-        "ToDate": Union[datetime, str],
-    },
-)
-
+TimestampTypeDef = Union[datetime, str]
 DeleteBackupPlanInputRequestTypeDef = TypedDict(
     "DeleteBackupPlanInputRequestTypeDef",
     {
         "BackupPlanId": str,
     },
 )
 
@@ -728,33 +727,14 @@
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
-ListBackupJobsInputRequestTypeDef = TypedDict(
-    "ListBackupJobsInputRequestTypeDef",
-    {
-        "NextToken": str,
-        "MaxResults": int,
-        "ByResourceArn": str,
-        "ByState": BackupJobStateType,
-        "ByBackupVaultName": str,
-        "ByCreatedBefore": Union[datetime, str],
-        "ByCreatedAfter": Union[datetime, str],
-        "ByResourceType": str,
-        "ByAccountId": str,
-        "ByCompleteAfter": Union[datetime, str],
-        "ByCompleteBefore": Union[datetime, str],
-        "ByParentJobId": str,
-    },
-    total=False,
-)
-
 ListBackupPlanTemplatesInputRequestTypeDef = TypedDict(
     "ListBackupPlanTemplatesInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -821,33 +801,14 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListCopyJobsInputRequestTypeDef = TypedDict(
-    "ListCopyJobsInputRequestTypeDef",
-    {
-        "NextToken": str,
-        "MaxResults": int,
-        "ByResourceArn": str,
-        "ByState": CopyJobStateType,
-        "ByCreatedBefore": Union[datetime, str],
-        "ByCreatedAfter": Union[datetime, str],
-        "ByResourceType": str,
-        "ByDestinationVaultArn": str,
-        "ByAccountId": str,
-        "ByCompleteBefore": Union[datetime, str],
-        "ByCompleteAfter": Union[datetime, str],
-        "ByParentJobId": str,
-    },
-    total=False,
-)
-
 ListFrameworksInputRequestTypeDef = TypedDict(
     "ListFrameworksInputRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -878,43 +839,14 @@
         "ResourceType": str,
         "LastBackupTime": datetime,
         "ResourceName": str,
     },
     total=False,
 )
 
-_RequiredListRecoveryPointsByBackupVaultInputRequestTypeDef = TypedDict(
-    "_RequiredListRecoveryPointsByBackupVaultInputRequestTypeDef",
-    {
-        "BackupVaultName": str,
-    },
-)
-_OptionalListRecoveryPointsByBackupVaultInputRequestTypeDef = TypedDict(
-    "_OptionalListRecoveryPointsByBackupVaultInputRequestTypeDef",
-    {
-        "NextToken": str,
-        "MaxResults": int,
-        "ByResourceArn": str,
-        "ByResourceType": str,
-        "ByBackupPlanId": str,
-        "ByCreatedBefore": Union[datetime, str],
-        "ByCreatedAfter": Union[datetime, str],
-        "ByParentRecoveryPointArn": str,
-    },
-    total=False,
-)
-
-
-class ListRecoveryPointsByBackupVaultInputRequestTypeDef(
-    _RequiredListRecoveryPointsByBackupVaultInputRequestTypeDef,
-    _OptionalListRecoveryPointsByBackupVaultInputRequestTypeDef,
-):
-    pass
-
-
 _RequiredListRecoveryPointsByLegalHoldInputRequestTypeDef = TypedDict(
     "_RequiredListRecoveryPointsByLegalHoldInputRequestTypeDef",
     {
         "LegalHoldId": str,
     },
 )
 _OptionalListRecoveryPointsByLegalHoldInputRequestTypeDef = TypedDict(
@@ -981,51 +913,23 @@
         "IsParent": bool,
         "ParentRecoveryPointArn": str,
         "ResourceName": str,
     },
     total=False,
 )
 
-ListReportJobsInputRequestTypeDef = TypedDict(
-    "ListReportJobsInputRequestTypeDef",
-    {
-        "ByReportPlanName": str,
-        "ByCreationBefore": Union[datetime, str],
-        "ByCreationAfter": Union[datetime, str],
-        "ByStatus": str,
-        "MaxResults": int,
-        "NextToken": str,
-    },
-    total=False,
-)
-
 ListReportPlansInputRequestTypeDef = TypedDict(
     "ListReportPlansInputRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListRestoreJobsInputRequestTypeDef = TypedDict(
-    "ListRestoreJobsInputRequestTypeDef",
-    {
-        "NextToken": str,
-        "MaxResults": int,
-        "ByAccountId": str,
-        "ByCreatedBefore": Union[datetime, str],
-        "ByCreatedAfter": Union[datetime, str],
-        "ByStatus": RestoreJobStatusType,
-        "ByCompleteBefore": Union[datetime, str],
-        "ByCompleteAfter": Union[datetime, str],
-    },
-    total=False,
-)
-
 RestoreJobsListMemberTypeDef = TypedDict(
     "RestoreJobsListMemberTypeDef",
     {
         "AccountId": str,
         "RestoreJobId": str,
         "RecoveryPointArn": str,
         "CreationDate": datetime,
@@ -1938,20 +1842,113 @@
         "VaultNames": List[str],
         "ResourceIdentifiers": List[str],
         "DateRange": DateRangeOutputTypeDef,
     },
     total=False,
 )
 
-RecoveryPointSelectionTypeDef = TypedDict(
-    "RecoveryPointSelectionTypeDef",
+DateRangeTypeDef = TypedDict(
+    "DateRangeTypeDef",
     {
-        "VaultNames": Sequence[str],
-        "ResourceIdentifiers": Sequence[str],
-        "DateRange": DateRangeTypeDef,
+        "FromDate": TimestampTypeDef,
+        "ToDate": TimestampTypeDef,
+    },
+)
+
+ListBackupJobsInputRequestTypeDef = TypedDict(
+    "ListBackupJobsInputRequestTypeDef",
+    {
+        "NextToken": str,
+        "MaxResults": int,
+        "ByResourceArn": str,
+        "ByState": BackupJobStateType,
+        "ByBackupVaultName": str,
+        "ByCreatedBefore": TimestampTypeDef,
+        "ByCreatedAfter": TimestampTypeDef,
+        "ByResourceType": str,
+        "ByAccountId": str,
+        "ByCompleteAfter": TimestampTypeDef,
+        "ByCompleteBefore": TimestampTypeDef,
+        "ByParentJobId": str,
+    },
+    total=False,
+)
+
+ListCopyJobsInputRequestTypeDef = TypedDict(
+    "ListCopyJobsInputRequestTypeDef",
+    {
+        "NextToken": str,
+        "MaxResults": int,
+        "ByResourceArn": str,
+        "ByState": CopyJobStateType,
+        "ByCreatedBefore": TimestampTypeDef,
+        "ByCreatedAfter": TimestampTypeDef,
+        "ByResourceType": str,
+        "ByDestinationVaultArn": str,
+        "ByAccountId": str,
+        "ByCompleteBefore": TimestampTypeDef,
+        "ByCompleteAfter": TimestampTypeDef,
+        "ByParentJobId": str,
+    },
+    total=False,
+)
+
+_RequiredListRecoveryPointsByBackupVaultInputRequestTypeDef = TypedDict(
+    "_RequiredListRecoveryPointsByBackupVaultInputRequestTypeDef",
+    {
+        "BackupVaultName": str,
+    },
+)
+_OptionalListRecoveryPointsByBackupVaultInputRequestTypeDef = TypedDict(
+    "_OptionalListRecoveryPointsByBackupVaultInputRequestTypeDef",
+    {
+        "NextToken": str,
+        "MaxResults": int,
+        "ByResourceArn": str,
+        "ByResourceType": str,
+        "ByBackupPlanId": str,
+        "ByCreatedBefore": TimestampTypeDef,
+        "ByCreatedAfter": TimestampTypeDef,
+        "ByParentRecoveryPointArn": str,
+    },
+    total=False,
+)
+
+
+class ListRecoveryPointsByBackupVaultInputRequestTypeDef(
+    _RequiredListRecoveryPointsByBackupVaultInputRequestTypeDef,
+    _OptionalListRecoveryPointsByBackupVaultInputRequestTypeDef,
+):
+    pass
+
+
+ListReportJobsInputRequestTypeDef = TypedDict(
+    "ListReportJobsInputRequestTypeDef",
+    {
+        "ByReportPlanName": str,
+        "ByCreationBefore": TimestampTypeDef,
+        "ByCreationAfter": TimestampTypeDef,
+        "ByStatus": str,
+        "MaxResults": int,
+        "NextToken": str,
+    },
+    total=False,
+)
+
+ListRestoreJobsInputRequestTypeDef = TypedDict(
+    "ListRestoreJobsInputRequestTypeDef",
+    {
+        "NextToken": str,
+        "MaxResults": int,
+        "ByAccountId": str,
+        "ByCreatedBefore": TimestampTypeDef,
+        "ByCreatedAfter": TimestampTypeDef,
+        "ByStatus": RestoreJobStatusType,
+        "ByCompleteBefore": TimestampTypeDef,
+        "ByCompleteAfter": TimestampTypeDef,
     },
     total=False,
 )
 
 ListFrameworksOutputTypeDef = TypedDict(
     "ListFrameworksOutputTypeDef",
     {
@@ -1972,20 +1969,20 @@
 
 ListBackupJobsInputListBackupJobsPaginateTypeDef = TypedDict(
     "ListBackupJobsInputListBackupJobsPaginateTypeDef",
     {
         "ByResourceArn": str,
         "ByState": BackupJobStateType,
         "ByBackupVaultName": str,
-        "ByCreatedBefore": Union[datetime, str],
-        "ByCreatedAfter": Union[datetime, str],
+        "ByCreatedBefore": TimestampTypeDef,
+        "ByCreatedAfter": TimestampTypeDef,
         "ByResourceType": str,
         "ByAccountId": str,
-        "ByCompleteAfter": Union[datetime, str],
-        "ByCompleteBefore": Union[datetime, str],
+        "ByCompleteAfter": TimestampTypeDef,
+        "ByCompleteBefore": TimestampTypeDef,
         "ByParentJobId": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListBackupPlanTemplatesInputListBackupPlanTemplatesPaginateTypeDef = TypedDict(
@@ -2058,21 +2055,21 @@
 )
 
 ListCopyJobsInputListCopyJobsPaginateTypeDef = TypedDict(
     "ListCopyJobsInputListCopyJobsPaginateTypeDef",
     {
         "ByResourceArn": str,
         "ByState": CopyJobStateType,
-        "ByCreatedBefore": Union[datetime, str],
-        "ByCreatedAfter": Union[datetime, str],
+        "ByCreatedBefore": TimestampTypeDef,
+        "ByCreatedAfter": TimestampTypeDef,
         "ByResourceType": str,
         "ByDestinationVaultArn": str,
         "ByAccountId": str,
-        "ByCompleteBefore": Union[datetime, str],
-        "ByCompleteAfter": Union[datetime, str],
+        "ByCompleteBefore": TimestampTypeDef,
+        "ByCompleteAfter": TimestampTypeDef,
         "ByParentJobId": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListLegalHoldsInputListLegalHoldsPaginateTypeDef = TypedDict(
@@ -2099,16 +2096,16 @@
 )
 _OptionalListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef = TypedDict(
     "_OptionalListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef",
     {
         "ByResourceArn": str,
         "ByResourceType": str,
         "ByBackupPlanId": str,
-        "ByCreatedBefore": Union[datetime, str],
-        "ByCreatedAfter": Union[datetime, str],
+        "ByCreatedBefore": TimestampTypeDef,
+        "ByCreatedAfter": TimestampTypeDef,
         "ByParentRecoveryPointArn": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
@@ -2163,19 +2160,19 @@
     pass
 
 
 ListRestoreJobsInputListRestoreJobsPaginateTypeDef = TypedDict(
     "ListRestoreJobsInputListRestoreJobsPaginateTypeDef",
     {
         "ByAccountId": str,
-        "ByCreatedBefore": Union[datetime, str],
-        "ByCreatedAfter": Union[datetime, str],
+        "ByCreatedBefore": TimestampTypeDef,
+        "ByCreatedAfter": TimestampTypeDef,
         "ByStatus": RestoreJobStatusType,
-        "ByCompleteBefore": Union[datetime, str],
-        "ByCompleteAfter": Union[datetime, str],
+        "ByCompleteBefore": TimestampTypeDef,
+        "ByCompleteAfter": TimestampTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListProtectedResourcesOutputTypeDef = TypedDict(
     "ListProtectedResourcesOutputTypeDef",
@@ -2209,14 +2206,17 @@
     {
         "RestoreJobs": List[RestoreJobsListMemberTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ReportDeliveryChannelUnionTypeDef = Union[
+    ReportDeliveryChannelTypeDef, ReportDeliveryChannelOutputTypeDef
+]
 ReportJobTypeDef = TypedDict(
     "ReportJobTypeDef",
     {
         "ReportJobId": str,
         "ReportPlanArn": str,
         "ReportTemplate": str,
         "CreationTime": datetime,
@@ -2240,14 +2240,15 @@
         "CreationTime": datetime,
         "LastAttemptedExecutionTime": datetime,
         "LastSuccessfulExecutionTime": datetime,
     },
     total=False,
 )
 
+ReportSettingUnionTypeDef = Union[ReportSettingTypeDef, ReportSettingOutputTypeDef]
 ListBackupPlanVersionsOutputTypeDef = TypedDict(
     "ListBackupPlanVersionsOutputTypeDef",
     {
         "NextToken": str,
         "BackupPlanVersionsList": List[BackupPlansListMemberTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2409,65 +2410,15 @@
         "DeploymentStatus": str,
         "FrameworkStatus": str,
         "IdempotencyToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateFrameworkInputRequestTypeDef = TypedDict(
-    "_RequiredCreateFrameworkInputRequestTypeDef",
-    {
-        "FrameworkName": str,
-        "FrameworkControls": Sequence[
-            Union[FrameworkControlTypeDef, FrameworkControlOutputTypeDef]
-        ],
-    },
-)
-_OptionalCreateFrameworkInputRequestTypeDef = TypedDict(
-    "_OptionalCreateFrameworkInputRequestTypeDef",
-    {
-        "FrameworkDescription": str,
-        "IdempotencyToken": str,
-        "FrameworkTags": Mapping[str, str],
-    },
-    total=False,
-)
-
-
-class CreateFrameworkInputRequestTypeDef(
-    _RequiredCreateFrameworkInputRequestTypeDef, _OptionalCreateFrameworkInputRequestTypeDef
-):
-    pass
-
-
-_RequiredUpdateFrameworkInputRequestTypeDef = TypedDict(
-    "_RequiredUpdateFrameworkInputRequestTypeDef",
-    {
-        "FrameworkName": str,
-    },
-)
-_OptionalUpdateFrameworkInputRequestTypeDef = TypedDict(
-    "_OptionalUpdateFrameworkInputRequestTypeDef",
-    {
-        "FrameworkDescription": str,
-        "FrameworkControls": Sequence[
-            Union[FrameworkControlTypeDef, FrameworkControlOutputTypeDef]
-        ],
-        "IdempotencyToken": str,
-    },
-    total=False,
-)
-
-
-class UpdateFrameworkInputRequestTypeDef(
-    _RequiredUpdateFrameworkInputRequestTypeDef, _OptionalUpdateFrameworkInputRequestTypeDef
-):
-    pass
-
-
+FrameworkControlUnionTypeDef = Union[FrameworkControlTypeDef, FrameworkControlOutputTypeDef]
 CreateLegalHoldOutputTypeDef = TypedDict(
     "CreateLegalHoldOutputTypeDef",
     {
         "Title": str,
         "Status": LegalHoldStatusType,
         "Description": str,
         "LegalHoldId": str,
@@ -2491,38 +2442,24 @@
         "CancellationDate": datetime,
         "RetainRecordUntil": datetime,
         "RecoveryPointSelection": RecoveryPointSelectionOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateLegalHoldInputRequestTypeDef = TypedDict(
-    "_RequiredCreateLegalHoldInputRequestTypeDef",
-    {
-        "Title": str,
-        "Description": str,
-    },
-)
-_OptionalCreateLegalHoldInputRequestTypeDef = TypedDict(
-    "_OptionalCreateLegalHoldInputRequestTypeDef",
+RecoveryPointSelectionTypeDef = TypedDict(
+    "RecoveryPointSelectionTypeDef",
     {
-        "IdempotencyToken": str,
-        "RecoveryPointSelection": RecoveryPointSelectionTypeDef,
-        "Tags": Mapping[str, str],
+        "VaultNames": Sequence[str],
+        "ResourceIdentifiers": Sequence[str],
+        "DateRange": DateRangeTypeDef,
     },
     total=False,
 )
 
-
-class CreateLegalHoldInputRequestTypeDef(
-    _RequiredCreateLegalHoldInputRequestTypeDef, _OptionalCreateLegalHoldInputRequestTypeDef
-):
-    pass
-
-
 DescribeReportJobOutputTypeDef = TypedDict(
     "DescribeReportJobOutputTypeDef",
     {
         "ReportJob": ReportJobTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2601,14 +2538,15 @@
         "BackupPlanId": str,
         "CreationDate": datetime,
         "CreatorRequestId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+BackupSelectionUnionTypeDef = Union[BackupSelectionTypeDef, BackupSelectionOutputTypeDef]
 _RequiredCreateBackupSelectionInputRequestTypeDef = TypedDict(
     "_RequiredCreateBackupSelectionInputRequestTypeDef",
     {
         "BackupPlanId": str,
         "BackupSelection": BackupSelectionTypeDef,
     },
 )
@@ -2624,14 +2562,88 @@
 class CreateBackupSelectionInputRequestTypeDef(
     _RequiredCreateBackupSelectionInputRequestTypeDef,
     _OptionalCreateBackupSelectionInputRequestTypeDef,
 ):
     pass
 
 
+_RequiredCreateFrameworkInputRequestTypeDef = TypedDict(
+    "_RequiredCreateFrameworkInputRequestTypeDef",
+    {
+        "FrameworkName": str,
+        "FrameworkControls": Sequence[FrameworkControlUnionTypeDef],
+    },
+)
+_OptionalCreateFrameworkInputRequestTypeDef = TypedDict(
+    "_OptionalCreateFrameworkInputRequestTypeDef",
+    {
+        "FrameworkDescription": str,
+        "IdempotencyToken": str,
+        "FrameworkTags": Mapping[str, str],
+    },
+    total=False,
+)
+
+
+class CreateFrameworkInputRequestTypeDef(
+    _RequiredCreateFrameworkInputRequestTypeDef, _OptionalCreateFrameworkInputRequestTypeDef
+):
+    pass
+
+
+_RequiredUpdateFrameworkInputRequestTypeDef = TypedDict(
+    "_RequiredUpdateFrameworkInputRequestTypeDef",
+    {
+        "FrameworkName": str,
+    },
+)
+_OptionalUpdateFrameworkInputRequestTypeDef = TypedDict(
+    "_OptionalUpdateFrameworkInputRequestTypeDef",
+    {
+        "FrameworkDescription": str,
+        "FrameworkControls": Sequence[FrameworkControlUnionTypeDef],
+        "IdempotencyToken": str,
+    },
+    total=False,
+)
+
+
+class UpdateFrameworkInputRequestTypeDef(
+    _RequiredUpdateFrameworkInputRequestTypeDef, _OptionalUpdateFrameworkInputRequestTypeDef
+):
+    pass
+
+
+_RequiredCreateLegalHoldInputRequestTypeDef = TypedDict(
+    "_RequiredCreateLegalHoldInputRequestTypeDef",
+    {
+        "Title": str,
+        "Description": str,
+    },
+)
+_OptionalCreateLegalHoldInputRequestTypeDef = TypedDict(
+    "_OptionalCreateLegalHoldInputRequestTypeDef",
+    {
+        "IdempotencyToken": str,
+        "RecoveryPointSelection": RecoveryPointSelectionTypeDef,
+        "Tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+
+class CreateLegalHoldInputRequestTypeDef(
+    _RequiredCreateLegalHoldInputRequestTypeDef, _OptionalCreateLegalHoldInputRequestTypeDef
+):
+    pass
+
+
+RecoveryPointSelectionUnionTypeDef = Union[
+    RecoveryPointSelectionTypeDef, RecoveryPointSelectionOutputTypeDef
+]
 _RequiredCreateBackupPlanInputRequestTypeDef = TypedDict(
     "_RequiredCreateBackupPlanInputRequestTypeDef",
     {
         "BackupPlan": BackupPlanInputTypeDef,
     },
 )
 _OptionalCreateBackupPlanInputRequestTypeDef = TypedDict(
```

### Comparing `mypy-boto3-backup-1.28.15.post1/mypy_boto3_backup/type_defs.pyi` & `mypy-boto3-backup-1.28.16/mypy_boto3_backup/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_backup.type_defs import AdvancedBackupSettingOutputTypeDef
 
-    data: AdvancedBackupSettingOutputTypeDef = {...}
+    data: AdvancedBackupSettingOutputTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -50,15 +50,15 @@
     "ControlScopeOutputTypeDef",
     "ControlScopeTypeDef",
     "ResponseMetadataTypeDef",
     "CreateBackupVaultInputRequestTypeDef",
     "ReportDeliveryChannelTypeDef",
     "ReportSettingTypeDef",
     "DateRangeOutputTypeDef",
-    "DateRangeTypeDef",
+    "TimestampTypeDef",
     "DeleteBackupPlanInputRequestTypeDef",
     "DeleteBackupSelectionInputRequestTypeDef",
     "DeleteBackupVaultAccessPolicyInputRequestTypeDef",
     "DeleteBackupVaultInputRequestTypeDef",
     "DeleteBackupVaultLockConfigurationInputRequestTypeDef",
     "DeleteBackupVaultNotificationsInputRequestTypeDef",
     "DeleteFrameworkInputRequestTypeDef",
@@ -83,33 +83,28 @@
     "GetBackupSelectionInputRequestTypeDef",
     "GetBackupVaultAccessPolicyInputRequestTypeDef",
     "GetBackupVaultNotificationsInputRequestTypeDef",
     "GetLegalHoldInputRequestTypeDef",
     "GetRecoveryPointRestoreMetadataInputRequestTypeDef",
     "LegalHoldTypeDef",
     "PaginatorConfigTypeDef",
-    "ListBackupJobsInputRequestTypeDef",
     "ListBackupPlanTemplatesInputRequestTypeDef",
     "ListBackupPlanVersionsInputRequestTypeDef",
     "ListBackupPlansInputRequestTypeDef",
     "ListBackupSelectionsInputRequestTypeDef",
     "ListBackupVaultsInputRequestTypeDef",
-    "ListCopyJobsInputRequestTypeDef",
     "ListFrameworksInputRequestTypeDef",
     "ListLegalHoldsInputRequestTypeDef",
     "ListProtectedResourcesInputRequestTypeDef",
     "ProtectedResourceTypeDef",
-    "ListRecoveryPointsByBackupVaultInputRequestTypeDef",
     "ListRecoveryPointsByLegalHoldInputRequestTypeDef",
     "RecoveryPointMemberTypeDef",
     "ListRecoveryPointsByResourceInputRequestTypeDef",
     "RecoveryPointByResourceTypeDef",
-    "ListReportJobsInputRequestTypeDef",
     "ListReportPlansInputRequestTypeDef",
-    "ListRestoreJobsInputRequestTypeDef",
     "RestoreJobsListMemberTypeDef",
     "ListTagsInputRequestTypeDef",
     "PutBackupVaultAccessPolicyInputRequestTypeDef",
     "PutBackupVaultLockConfigurationInputRequestTypeDef",
     "PutBackupVaultNotificationsInputRequestTypeDef",
     "ReportDeliveryChannelOutputTypeDef",
     "ReportDestinationTypeDef",
@@ -163,15 +158,20 @@
     "UpdateBackupPlanOutputTypeDef",
     "UpdateFrameworkOutputTypeDef",
     "UpdateRecoveryPointLifecycleOutputTypeDef",
     "UpdateReportPlanOutputTypeDef",
     "CreateReportPlanInputRequestTypeDef",
     "UpdateReportPlanInputRequestTypeDef",
     "RecoveryPointSelectionOutputTypeDef",
-    "RecoveryPointSelectionTypeDef",
+    "DateRangeTypeDef",
+    "ListBackupJobsInputRequestTypeDef",
+    "ListCopyJobsInputRequestTypeDef",
+    "ListRecoveryPointsByBackupVaultInputRequestTypeDef",
+    "ListReportJobsInputRequestTypeDef",
+    "ListRestoreJobsInputRequestTypeDef",
     "ListFrameworksOutputTypeDef",
     "ListLegalHoldsOutputTypeDef",
     "ListBackupJobsInputListBackupJobsPaginateTypeDef",
     "ListBackupPlanTemplatesInputListBackupPlanTemplatesPaginateTypeDef",
     "ListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef",
     "ListBackupPlansInputListBackupPlansPaginateTypeDef",
     "ListBackupSelectionsInputListBackupSelectionsPaginateTypeDef",
@@ -183,40 +183,46 @@
     "ListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef",
     "ListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef",
     "ListRestoreJobsInputListRestoreJobsPaginateTypeDef",
     "ListProtectedResourcesOutputTypeDef",
     "ListRecoveryPointsByLegalHoldOutputTypeDef",
     "ListRecoveryPointsByResourceOutputTypeDef",
     "ListRestoreJobsOutputTypeDef",
+    "ReportDeliveryChannelUnionTypeDef",
     "ReportJobTypeDef",
     "ReportPlanTypeDef",
+    "ReportSettingUnionTypeDef",
     "ListBackupPlanVersionsOutputTypeDef",
     "ListBackupPlansOutputTypeDef",
     "ListBackupJobsOutputTypeDef",
     "DescribeCopyJobOutputTypeDef",
     "ListCopyJobsOutputTypeDef",
     "BackupRuleInputTypeDef",
     "BackupRuleTypeDef",
     "ListRecoveryPointsByBackupVaultOutputTypeDef",
     "BackupSelectionOutputTypeDef",
     "BackupSelectionTypeDef",
     "DescribeFrameworkOutputTypeDef",
-    "CreateFrameworkInputRequestTypeDef",
-    "UpdateFrameworkInputRequestTypeDef",
+    "FrameworkControlUnionTypeDef",
     "CreateLegalHoldOutputTypeDef",
     "GetLegalHoldOutputTypeDef",
-    "CreateLegalHoldInputRequestTypeDef",
+    "RecoveryPointSelectionTypeDef",
     "DescribeReportJobOutputTypeDef",
     "ListReportJobsOutputTypeDef",
     "DescribeReportPlanOutputTypeDef",
     "ListReportPlansOutputTypeDef",
     "BackupPlanInputTypeDef",
     "BackupPlanTypeDef",
     "GetBackupSelectionOutputTypeDef",
+    "BackupSelectionUnionTypeDef",
     "CreateBackupSelectionInputRequestTypeDef",
+    "CreateFrameworkInputRequestTypeDef",
+    "UpdateFrameworkInputRequestTypeDef",
+    "CreateLegalHoldInputRequestTypeDef",
+    "RecoveryPointSelectionUnionTypeDef",
     "CreateBackupPlanInputRequestTypeDef",
     "UpdateBackupPlanInputRequestTypeDef",
     "GetBackupPlanFromJSONOutputTypeDef",
     "GetBackupPlanFromTemplateOutputTypeDef",
     "GetBackupPlanOutputTypeDef",
 )
 
@@ -450,22 +456,15 @@
     "DateRangeOutputTypeDef",
     {
         "FromDate": datetime,
         "ToDate": datetime,
     },
 )
 
-DateRangeTypeDef = TypedDict(
-    "DateRangeTypeDef",
-    {
-        "FromDate": Union[datetime, str],
-        "ToDate": Union[datetime, str],
-    },
-)
-
+TimestampTypeDef = Union[datetime, str]
 DeleteBackupPlanInputRequestTypeDef = TypedDict(
     "DeleteBackupPlanInputRequestTypeDef",
     {
         "BackupPlanId": str,
     },
 )
 
@@ -717,33 +716,14 @@
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
-ListBackupJobsInputRequestTypeDef = TypedDict(
-    "ListBackupJobsInputRequestTypeDef",
-    {
-        "NextToken": str,
-        "MaxResults": int,
-        "ByResourceArn": str,
-        "ByState": BackupJobStateType,
-        "ByBackupVaultName": str,
-        "ByCreatedBefore": Union[datetime, str],
-        "ByCreatedAfter": Union[datetime, str],
-        "ByResourceType": str,
-        "ByAccountId": str,
-        "ByCompleteAfter": Union[datetime, str],
-        "ByCompleteBefore": Union[datetime, str],
-        "ByParentJobId": str,
-    },
-    total=False,
-)
-
 ListBackupPlanTemplatesInputRequestTypeDef = TypedDict(
     "ListBackupPlanTemplatesInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -806,33 +786,14 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListCopyJobsInputRequestTypeDef = TypedDict(
-    "ListCopyJobsInputRequestTypeDef",
-    {
-        "NextToken": str,
-        "MaxResults": int,
-        "ByResourceArn": str,
-        "ByState": CopyJobStateType,
-        "ByCreatedBefore": Union[datetime, str],
-        "ByCreatedAfter": Union[datetime, str],
-        "ByResourceType": str,
-        "ByDestinationVaultArn": str,
-        "ByAccountId": str,
-        "ByCompleteBefore": Union[datetime, str],
-        "ByCompleteAfter": Union[datetime, str],
-        "ByParentJobId": str,
-    },
-    total=False,
-)
-
 ListFrameworksInputRequestTypeDef = TypedDict(
     "ListFrameworksInputRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -863,41 +824,14 @@
         "ResourceType": str,
         "LastBackupTime": datetime,
         "ResourceName": str,
     },
     total=False,
 )
 
-_RequiredListRecoveryPointsByBackupVaultInputRequestTypeDef = TypedDict(
-    "_RequiredListRecoveryPointsByBackupVaultInputRequestTypeDef",
-    {
-        "BackupVaultName": str,
-    },
-)
-_OptionalListRecoveryPointsByBackupVaultInputRequestTypeDef = TypedDict(
-    "_OptionalListRecoveryPointsByBackupVaultInputRequestTypeDef",
-    {
-        "NextToken": str,
-        "MaxResults": int,
-        "ByResourceArn": str,
-        "ByResourceType": str,
-        "ByBackupPlanId": str,
-        "ByCreatedBefore": Union[datetime, str],
-        "ByCreatedAfter": Union[datetime, str],
-        "ByParentRecoveryPointArn": str,
-    },
-    total=False,
-)
-
-class ListRecoveryPointsByBackupVaultInputRequestTypeDef(
-    _RequiredListRecoveryPointsByBackupVaultInputRequestTypeDef,
-    _OptionalListRecoveryPointsByBackupVaultInputRequestTypeDef,
-):
-    pass
-
 _RequiredListRecoveryPointsByLegalHoldInputRequestTypeDef = TypedDict(
     "_RequiredListRecoveryPointsByLegalHoldInputRequestTypeDef",
     {
         "LegalHoldId": str,
     },
 )
 _OptionalListRecoveryPointsByLegalHoldInputRequestTypeDef = TypedDict(
@@ -960,51 +894,23 @@
         "IsParent": bool,
         "ParentRecoveryPointArn": str,
         "ResourceName": str,
     },
     total=False,
 )
 
-ListReportJobsInputRequestTypeDef = TypedDict(
-    "ListReportJobsInputRequestTypeDef",
-    {
-        "ByReportPlanName": str,
-        "ByCreationBefore": Union[datetime, str],
-        "ByCreationAfter": Union[datetime, str],
-        "ByStatus": str,
-        "MaxResults": int,
-        "NextToken": str,
-    },
-    total=False,
-)
-
 ListReportPlansInputRequestTypeDef = TypedDict(
     "ListReportPlansInputRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListRestoreJobsInputRequestTypeDef = TypedDict(
-    "ListRestoreJobsInputRequestTypeDef",
-    {
-        "NextToken": str,
-        "MaxResults": int,
-        "ByAccountId": str,
-        "ByCreatedBefore": Union[datetime, str],
-        "ByCreatedAfter": Union[datetime, str],
-        "ByStatus": RestoreJobStatusType,
-        "ByCompleteBefore": Union[datetime, str],
-        "ByCompleteAfter": Union[datetime, str],
-    },
-    total=False,
-)
-
 RestoreJobsListMemberTypeDef = TypedDict(
     "RestoreJobsListMemberTypeDef",
     {
         "AccountId": str,
         "RestoreJobId": str,
         "RecoveryPointArn": str,
         "CreationDate": datetime,
@@ -1887,20 +1793,111 @@
         "VaultNames": List[str],
         "ResourceIdentifiers": List[str],
         "DateRange": DateRangeOutputTypeDef,
     },
     total=False,
 )
 
-RecoveryPointSelectionTypeDef = TypedDict(
-    "RecoveryPointSelectionTypeDef",
+DateRangeTypeDef = TypedDict(
+    "DateRangeTypeDef",
     {
-        "VaultNames": Sequence[str],
-        "ResourceIdentifiers": Sequence[str],
-        "DateRange": DateRangeTypeDef,
+        "FromDate": TimestampTypeDef,
+        "ToDate": TimestampTypeDef,
+    },
+)
+
+ListBackupJobsInputRequestTypeDef = TypedDict(
+    "ListBackupJobsInputRequestTypeDef",
+    {
+        "NextToken": str,
+        "MaxResults": int,
+        "ByResourceArn": str,
+        "ByState": BackupJobStateType,
+        "ByBackupVaultName": str,
+        "ByCreatedBefore": TimestampTypeDef,
+        "ByCreatedAfter": TimestampTypeDef,
+        "ByResourceType": str,
+        "ByAccountId": str,
+        "ByCompleteAfter": TimestampTypeDef,
+        "ByCompleteBefore": TimestampTypeDef,
+        "ByParentJobId": str,
+    },
+    total=False,
+)
+
+ListCopyJobsInputRequestTypeDef = TypedDict(
+    "ListCopyJobsInputRequestTypeDef",
+    {
+        "NextToken": str,
+        "MaxResults": int,
+        "ByResourceArn": str,
+        "ByState": CopyJobStateType,
+        "ByCreatedBefore": TimestampTypeDef,
+        "ByCreatedAfter": TimestampTypeDef,
+        "ByResourceType": str,
+        "ByDestinationVaultArn": str,
+        "ByAccountId": str,
+        "ByCompleteBefore": TimestampTypeDef,
+        "ByCompleteAfter": TimestampTypeDef,
+        "ByParentJobId": str,
+    },
+    total=False,
+)
+
+_RequiredListRecoveryPointsByBackupVaultInputRequestTypeDef = TypedDict(
+    "_RequiredListRecoveryPointsByBackupVaultInputRequestTypeDef",
+    {
+        "BackupVaultName": str,
+    },
+)
+_OptionalListRecoveryPointsByBackupVaultInputRequestTypeDef = TypedDict(
+    "_OptionalListRecoveryPointsByBackupVaultInputRequestTypeDef",
+    {
+        "NextToken": str,
+        "MaxResults": int,
+        "ByResourceArn": str,
+        "ByResourceType": str,
+        "ByBackupPlanId": str,
+        "ByCreatedBefore": TimestampTypeDef,
+        "ByCreatedAfter": TimestampTypeDef,
+        "ByParentRecoveryPointArn": str,
+    },
+    total=False,
+)
+
+class ListRecoveryPointsByBackupVaultInputRequestTypeDef(
+    _RequiredListRecoveryPointsByBackupVaultInputRequestTypeDef,
+    _OptionalListRecoveryPointsByBackupVaultInputRequestTypeDef,
+):
+    pass
+
+ListReportJobsInputRequestTypeDef = TypedDict(
+    "ListReportJobsInputRequestTypeDef",
+    {
+        "ByReportPlanName": str,
+        "ByCreationBefore": TimestampTypeDef,
+        "ByCreationAfter": TimestampTypeDef,
+        "ByStatus": str,
+        "MaxResults": int,
+        "NextToken": str,
+    },
+    total=False,
+)
+
+ListRestoreJobsInputRequestTypeDef = TypedDict(
+    "ListRestoreJobsInputRequestTypeDef",
+    {
+        "NextToken": str,
+        "MaxResults": int,
+        "ByAccountId": str,
+        "ByCreatedBefore": TimestampTypeDef,
+        "ByCreatedAfter": TimestampTypeDef,
+        "ByStatus": RestoreJobStatusType,
+        "ByCompleteBefore": TimestampTypeDef,
+        "ByCompleteAfter": TimestampTypeDef,
     },
     total=False,
 )
 
 ListFrameworksOutputTypeDef = TypedDict(
     "ListFrameworksOutputTypeDef",
     {
@@ -1921,20 +1918,20 @@
 
 ListBackupJobsInputListBackupJobsPaginateTypeDef = TypedDict(
     "ListBackupJobsInputListBackupJobsPaginateTypeDef",
     {
         "ByResourceArn": str,
         "ByState": BackupJobStateType,
         "ByBackupVaultName": str,
-        "ByCreatedBefore": Union[datetime, str],
-        "ByCreatedAfter": Union[datetime, str],
+        "ByCreatedBefore": TimestampTypeDef,
+        "ByCreatedAfter": TimestampTypeDef,
         "ByResourceType": str,
         "ByAccountId": str,
-        "ByCompleteAfter": Union[datetime, str],
-        "ByCompleteBefore": Union[datetime, str],
+        "ByCompleteAfter": TimestampTypeDef,
+        "ByCompleteBefore": TimestampTypeDef,
         "ByParentJobId": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListBackupPlanTemplatesInputListBackupPlanTemplatesPaginateTypeDef = TypedDict(
@@ -2003,21 +2000,21 @@
 )
 
 ListCopyJobsInputListCopyJobsPaginateTypeDef = TypedDict(
     "ListCopyJobsInputListCopyJobsPaginateTypeDef",
     {
         "ByResourceArn": str,
         "ByState": CopyJobStateType,
-        "ByCreatedBefore": Union[datetime, str],
-        "ByCreatedAfter": Union[datetime, str],
+        "ByCreatedBefore": TimestampTypeDef,
+        "ByCreatedAfter": TimestampTypeDef,
         "ByResourceType": str,
         "ByDestinationVaultArn": str,
         "ByAccountId": str,
-        "ByCompleteBefore": Union[datetime, str],
-        "ByCompleteAfter": Union[datetime, str],
+        "ByCompleteBefore": TimestampTypeDef,
+        "ByCompleteAfter": TimestampTypeDef,
         "ByParentJobId": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListLegalHoldsInputListLegalHoldsPaginateTypeDef = TypedDict(
@@ -2044,16 +2041,16 @@
 )
 _OptionalListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef = TypedDict(
     "_OptionalListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef",
     {
         "ByResourceArn": str,
         "ByResourceType": str,
         "ByBackupPlanId": str,
-        "ByCreatedBefore": Union[datetime, str],
-        "ByCreatedAfter": Union[datetime, str],
+        "ByCreatedBefore": TimestampTypeDef,
+        "ByCreatedAfter": TimestampTypeDef,
         "ByParentRecoveryPointArn": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class ListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef(
@@ -2102,19 +2099,19 @@
 ):
     pass
 
 ListRestoreJobsInputListRestoreJobsPaginateTypeDef = TypedDict(
     "ListRestoreJobsInputListRestoreJobsPaginateTypeDef",
     {
         "ByAccountId": str,
-        "ByCreatedBefore": Union[datetime, str],
-        "ByCreatedAfter": Union[datetime, str],
+        "ByCreatedBefore": TimestampTypeDef,
+        "ByCreatedAfter": TimestampTypeDef,
         "ByStatus": RestoreJobStatusType,
-        "ByCompleteBefore": Union[datetime, str],
-        "ByCompleteAfter": Union[datetime, str],
+        "ByCompleteBefore": TimestampTypeDef,
+        "ByCompleteAfter": TimestampTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListProtectedResourcesOutputTypeDef = TypedDict(
     "ListProtectedResourcesOutputTypeDef",
@@ -2148,14 +2145,17 @@
     {
         "RestoreJobs": List[RestoreJobsListMemberTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ReportDeliveryChannelUnionTypeDef = Union[
+    ReportDeliveryChannelTypeDef, ReportDeliveryChannelOutputTypeDef
+]
 ReportJobTypeDef = TypedDict(
     "ReportJobTypeDef",
     {
         "ReportJobId": str,
         "ReportPlanArn": str,
         "ReportTemplate": str,
         "CreationTime": datetime,
@@ -2179,14 +2179,15 @@
         "CreationTime": datetime,
         "LastAttemptedExecutionTime": datetime,
         "LastSuccessfulExecutionTime": datetime,
     },
     total=False,
 )
 
+ReportSettingUnionTypeDef = Union[ReportSettingTypeDef, ReportSettingOutputTypeDef]
 ListBackupPlanVersionsOutputTypeDef = TypedDict(
     "ListBackupPlanVersionsOutputTypeDef",
     {
         "NextToken": str,
         "BackupPlanVersionsList": List[BackupPlansListMemberTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2340,61 +2341,15 @@
         "DeploymentStatus": str,
         "FrameworkStatus": str,
         "IdempotencyToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateFrameworkInputRequestTypeDef = TypedDict(
-    "_RequiredCreateFrameworkInputRequestTypeDef",
-    {
-        "FrameworkName": str,
-        "FrameworkControls": Sequence[
-            Union[FrameworkControlTypeDef, FrameworkControlOutputTypeDef]
-        ],
-    },
-)
-_OptionalCreateFrameworkInputRequestTypeDef = TypedDict(
-    "_OptionalCreateFrameworkInputRequestTypeDef",
-    {
-        "FrameworkDescription": str,
-        "IdempotencyToken": str,
-        "FrameworkTags": Mapping[str, str],
-    },
-    total=False,
-)
-
-class CreateFrameworkInputRequestTypeDef(
-    _RequiredCreateFrameworkInputRequestTypeDef, _OptionalCreateFrameworkInputRequestTypeDef
-):
-    pass
-
-_RequiredUpdateFrameworkInputRequestTypeDef = TypedDict(
-    "_RequiredUpdateFrameworkInputRequestTypeDef",
-    {
-        "FrameworkName": str,
-    },
-)
-_OptionalUpdateFrameworkInputRequestTypeDef = TypedDict(
-    "_OptionalUpdateFrameworkInputRequestTypeDef",
-    {
-        "FrameworkDescription": str,
-        "FrameworkControls": Sequence[
-            Union[FrameworkControlTypeDef, FrameworkControlOutputTypeDef]
-        ],
-        "IdempotencyToken": str,
-    },
-    total=False,
-)
-
-class UpdateFrameworkInputRequestTypeDef(
-    _RequiredUpdateFrameworkInputRequestTypeDef, _OptionalUpdateFrameworkInputRequestTypeDef
-):
-    pass
-
+FrameworkControlUnionTypeDef = Union[FrameworkControlTypeDef, FrameworkControlOutputTypeDef]
 CreateLegalHoldOutputTypeDef = TypedDict(
     "CreateLegalHoldOutputTypeDef",
     {
         "Title": str,
         "Status": LegalHoldStatusType,
         "Description": str,
         "LegalHoldId": str,
@@ -2418,36 +2373,24 @@
         "CancellationDate": datetime,
         "RetainRecordUntil": datetime,
         "RecoveryPointSelection": RecoveryPointSelectionOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateLegalHoldInputRequestTypeDef = TypedDict(
-    "_RequiredCreateLegalHoldInputRequestTypeDef",
-    {
-        "Title": str,
-        "Description": str,
-    },
-)
-_OptionalCreateLegalHoldInputRequestTypeDef = TypedDict(
-    "_OptionalCreateLegalHoldInputRequestTypeDef",
+RecoveryPointSelectionTypeDef = TypedDict(
+    "RecoveryPointSelectionTypeDef",
     {
-        "IdempotencyToken": str,
-        "RecoveryPointSelection": RecoveryPointSelectionTypeDef,
-        "Tags": Mapping[str, str],
+        "VaultNames": Sequence[str],
+        "ResourceIdentifiers": Sequence[str],
+        "DateRange": DateRangeTypeDef,
     },
     total=False,
 )
 
-class CreateLegalHoldInputRequestTypeDef(
-    _RequiredCreateLegalHoldInputRequestTypeDef, _OptionalCreateLegalHoldInputRequestTypeDef
-):
-    pass
-
 DescribeReportJobOutputTypeDef = TypedDict(
     "DescribeReportJobOutputTypeDef",
     {
         "ReportJob": ReportJobTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2522,14 +2465,15 @@
         "BackupPlanId": str,
         "CreationDate": datetime,
         "CreatorRequestId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+BackupSelectionUnionTypeDef = Union[BackupSelectionTypeDef, BackupSelectionOutputTypeDef]
 _RequiredCreateBackupSelectionInputRequestTypeDef = TypedDict(
     "_RequiredCreateBackupSelectionInputRequestTypeDef",
     {
         "BackupPlanId": str,
         "BackupSelection": BackupSelectionTypeDef,
     },
 )
@@ -2543,14 +2487,82 @@
 
 class CreateBackupSelectionInputRequestTypeDef(
     _RequiredCreateBackupSelectionInputRequestTypeDef,
     _OptionalCreateBackupSelectionInputRequestTypeDef,
 ):
     pass
 
+_RequiredCreateFrameworkInputRequestTypeDef = TypedDict(
+    "_RequiredCreateFrameworkInputRequestTypeDef",
+    {
+        "FrameworkName": str,
+        "FrameworkControls": Sequence[FrameworkControlUnionTypeDef],
+    },
+)
+_OptionalCreateFrameworkInputRequestTypeDef = TypedDict(
+    "_OptionalCreateFrameworkInputRequestTypeDef",
+    {
+        "FrameworkDescription": str,
+        "IdempotencyToken": str,
+        "FrameworkTags": Mapping[str, str],
+    },
+    total=False,
+)
+
+class CreateFrameworkInputRequestTypeDef(
+    _RequiredCreateFrameworkInputRequestTypeDef, _OptionalCreateFrameworkInputRequestTypeDef
+):
+    pass
+
+_RequiredUpdateFrameworkInputRequestTypeDef = TypedDict(
+    "_RequiredUpdateFrameworkInputRequestTypeDef",
+    {
+        "FrameworkName": str,
+    },
+)
+_OptionalUpdateFrameworkInputRequestTypeDef = TypedDict(
+    "_OptionalUpdateFrameworkInputRequestTypeDef",
+    {
+        "FrameworkDescription": str,
+        "FrameworkControls": Sequence[FrameworkControlUnionTypeDef],
+        "IdempotencyToken": str,
+    },
+    total=False,
+)
+
+class UpdateFrameworkInputRequestTypeDef(
+    _RequiredUpdateFrameworkInputRequestTypeDef, _OptionalUpdateFrameworkInputRequestTypeDef
+):
+    pass
+
+_RequiredCreateLegalHoldInputRequestTypeDef = TypedDict(
+    "_RequiredCreateLegalHoldInputRequestTypeDef",
+    {
+        "Title": str,
+        "Description": str,
+    },
+)
+_OptionalCreateLegalHoldInputRequestTypeDef = TypedDict(
+    "_OptionalCreateLegalHoldInputRequestTypeDef",
+    {
+        "IdempotencyToken": str,
+        "RecoveryPointSelection": RecoveryPointSelectionTypeDef,
+        "Tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+class CreateLegalHoldInputRequestTypeDef(
+    _RequiredCreateLegalHoldInputRequestTypeDef, _OptionalCreateLegalHoldInputRequestTypeDef
+):
+    pass
+
+RecoveryPointSelectionUnionTypeDef = Union[
+    RecoveryPointSelectionTypeDef, RecoveryPointSelectionOutputTypeDef
+]
 _RequiredCreateBackupPlanInputRequestTypeDef = TypedDict(
     "_RequiredCreateBackupPlanInputRequestTypeDef",
     {
         "BackupPlan": BackupPlanInputTypeDef,
     },
 )
 _OptionalCreateBackupPlanInputRequestTypeDef = TypedDict(
```

### Comparing `mypy-boto3-backup-1.28.15.post1/mypy_boto3_backup.egg-info/PKG-INFO` & `mypy-boto3-backup-1.28.16/mypy_boto3_backup.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-backup
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.Backup 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.Backup 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 backup type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 backup type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-backup.svg?color=blue)](https://pypi.org/project/mypy-boto3-backup)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-backup)](https://pepy.tech/project/mypy-boto3-backup)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Backup 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup)
+[boto3.Backup 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup)
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
 [mypy-boto3-backup docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/).
 
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
@@ -369,20 +369,20 @@
 )
 
 
 def check_value(value: BackupJobStateType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_backup.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_backup.type_defs import (
     AdvancedBackupSettingOutputTypeDef,
     AdvancedBackupSettingTypeDef,
     RecoveryPointCreatorTypeDef,
     BackupPlanTemplatesListMemberTypeDef,
@@ -397,15 +397,15 @@
     ControlScopeOutputTypeDef,
     ControlScopeTypeDef,
     ResponseMetadataTypeDef,
     CreateBackupVaultInputRequestTypeDef,
     ReportDeliveryChannelTypeDef,
     ReportSettingTypeDef,
     DateRangeOutputTypeDef,
-    DateRangeTypeDef,
+    TimestampTypeDef,
     DeleteBackupPlanInputRequestTypeDef,
     DeleteBackupSelectionInputRequestTypeDef,
     DeleteBackupVaultAccessPolicyInputRequestTypeDef,
     DeleteBackupVaultInputRequestTypeDef,
     DeleteBackupVaultLockConfigurationInputRequestTypeDef,
     DeleteBackupVaultNotificationsInputRequestTypeDef,
     DeleteFrameworkInputRequestTypeDef,
@@ -430,33 +430,28 @@
     GetBackupSelectionInputRequestTypeDef,
     GetBackupVaultAccessPolicyInputRequestTypeDef,
     GetBackupVaultNotificationsInputRequestTypeDef,
     GetLegalHoldInputRequestTypeDef,
     GetRecoveryPointRestoreMetadataInputRequestTypeDef,
     LegalHoldTypeDef,
     PaginatorConfigTypeDef,
-    ListBackupJobsInputRequestTypeDef,
     ListBackupPlanTemplatesInputRequestTypeDef,
     ListBackupPlanVersionsInputRequestTypeDef,
     ListBackupPlansInputRequestTypeDef,
     ListBackupSelectionsInputRequestTypeDef,
     ListBackupVaultsInputRequestTypeDef,
-    ListCopyJobsInputRequestTypeDef,
     ListFrameworksInputRequestTypeDef,
     ListLegalHoldsInputRequestTypeDef,
     ListProtectedResourcesInputRequestTypeDef,
     ProtectedResourceTypeDef,
-    ListRecoveryPointsByBackupVaultInputRequestTypeDef,
     ListRecoveryPointsByLegalHoldInputRequestTypeDef,
     RecoveryPointMemberTypeDef,
     ListRecoveryPointsByResourceInputRequestTypeDef,
     RecoveryPointByResourceTypeDef,
-    ListReportJobsInputRequestTypeDef,
     ListReportPlansInputRequestTypeDef,
-    ListRestoreJobsInputRequestTypeDef,
     RestoreJobsListMemberTypeDef,
     ListTagsInputRequestTypeDef,
     PutBackupVaultAccessPolicyInputRequestTypeDef,
     PutBackupVaultLockConfigurationInputRequestTypeDef,
     PutBackupVaultNotificationsInputRequestTypeDef,
     ReportDeliveryChannelOutputTypeDef,
     ReportDestinationTypeDef,
@@ -510,15 +505,20 @@
     UpdateBackupPlanOutputTypeDef,
     UpdateFrameworkOutputTypeDef,
     UpdateRecoveryPointLifecycleOutputTypeDef,
     UpdateReportPlanOutputTypeDef,
     CreateReportPlanInputRequestTypeDef,
     UpdateReportPlanInputRequestTypeDef,
     RecoveryPointSelectionOutputTypeDef,
-    RecoveryPointSelectionTypeDef,
+    DateRangeTypeDef,
+    ListBackupJobsInputRequestTypeDef,
+    ListCopyJobsInputRequestTypeDef,
+    ListRecoveryPointsByBackupVaultInputRequestTypeDef,
+    ListReportJobsInputRequestTypeDef,
+    ListRestoreJobsInputRequestTypeDef,
     ListFrameworksOutputTypeDef,
     ListLegalHoldsOutputTypeDef,
     ListBackupJobsInputListBackupJobsPaginateTypeDef,
     ListBackupPlanTemplatesInputListBackupPlanTemplatesPaginateTypeDef,
     ListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef,
     ListBackupPlansInputListBackupPlansPaginateTypeDef,
     ListBackupSelectionsInputListBackupSelectionsPaginateTypeDef,
@@ -530,49 +530,55 @@
     ListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef,
     ListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef,
     ListRestoreJobsInputListRestoreJobsPaginateTypeDef,
     ListProtectedResourcesOutputTypeDef,
     ListRecoveryPointsByLegalHoldOutputTypeDef,
     ListRecoveryPointsByResourceOutputTypeDef,
     ListRestoreJobsOutputTypeDef,
+    ReportDeliveryChannelUnionTypeDef,
     ReportJobTypeDef,
     ReportPlanTypeDef,
+    ReportSettingUnionTypeDef,
     ListBackupPlanVersionsOutputTypeDef,
     ListBackupPlansOutputTypeDef,
     ListBackupJobsOutputTypeDef,
     DescribeCopyJobOutputTypeDef,
     ListCopyJobsOutputTypeDef,
     BackupRuleInputTypeDef,
     BackupRuleTypeDef,
     ListRecoveryPointsByBackupVaultOutputTypeDef,
     BackupSelectionOutputTypeDef,
     BackupSelectionTypeDef,
     DescribeFrameworkOutputTypeDef,
-    CreateFrameworkInputRequestTypeDef,
-    UpdateFrameworkInputRequestTypeDef,
+    FrameworkControlUnionTypeDef,
     CreateLegalHoldOutputTypeDef,
     GetLegalHoldOutputTypeDef,
-    CreateLegalHoldInputRequestTypeDef,
+    RecoveryPointSelectionTypeDef,
     DescribeReportJobOutputTypeDef,
     ListReportJobsOutputTypeDef,
     DescribeReportPlanOutputTypeDef,
     ListReportPlansOutputTypeDef,
     BackupPlanInputTypeDef,
     BackupPlanTypeDef,
     GetBackupSelectionOutputTypeDef,
+    BackupSelectionUnionTypeDef,
     CreateBackupSelectionInputRequestTypeDef,
+    CreateFrameworkInputRequestTypeDef,
+    UpdateFrameworkInputRequestTypeDef,
+    CreateLegalHoldInputRequestTypeDef,
+    RecoveryPointSelectionUnionTypeDef,
     CreateBackupPlanInputRequestTypeDef,
     UpdateBackupPlanInputRequestTypeDef,
     GetBackupPlanFromJSONOutputTypeDef,
     GetBackupPlanFromTemplateOutputTypeDef,
     GetBackupPlanOutputTypeDef,
 )
 
 
-def get_structure() -> AdvancedBackupSettingOutputTypeDef:
+def get_value() -> AdvancedBackupSettingOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-backup-1.28.15.post1/mypy_boto3_backup.egg-info/SOURCES.txt` & `mypy-boto3-backup-1.28.16/mypy_boto3_backup.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-backup-1.28.15.post1/setup.py` & `mypy-boto3-backup-1.28.16/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-backup",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_backup"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Backup 1.28.15 service generated with mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.Backup 1.28.16 service generated with mypy-boto3-builder 7.17.1"
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
-    keywords="boto3 backup type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 backup type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_backup": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

