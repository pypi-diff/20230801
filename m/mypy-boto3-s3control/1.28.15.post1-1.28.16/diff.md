# Comparing `tmp/mypy-boto3-s3control-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-s3control-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-s3control-1.28.15.post1.tar", last modified: Sat Jul 29 10:04:04 2023, max compression
+gzip compressed data, was "mypy-boto3-s3control-1.28.16.tar", last modified: Tue Aug  1 11:37:44 2023, max compression
```

## Comparing `mypy-boto3-s3control-1.28.15.post1.tar` & `mypy-boto3-s3control-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:04.869378 mypy-boto3-s3control-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:57:49.000000 mypy-boto3-s3control-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    24030 2023-07-29 10:04:04.869378 mypy-boto3-s3control-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22529 2023-07-29 09:57:49.000000 mypy-boto3-s3control-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:04.861378 mypy-boto3-s3control-1.28.15.post1/mypy_boto3_s3control/
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-29 09:57:49.000000 mypy-boto3-s3control-1.28.15.post1/mypy_boto3_s3control/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-07-29 09:57:49.000000 mypy-boto3-s3control-1.28.15.post1/mypy_boto3_s3control/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-29 09:57:49.000000 mypy-boto3-s3control-1.28.15.post1/mypy_boto3_s3control/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43922 2023-07-29 09:57:50.000000 mypy-boto3-s3control-1.28.15.post1/mypy_boto3_s3control/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    43850 2023-07-29 09:57:49.000000 mypy-boto3-s3control-1.28.15.post1/mypy_boto3_s3control/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13694 2023-07-29 09:57:50.000000 mypy-boto3-s3control-1.28.15.post1/mypy_boto3_s3control/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13692 2023-07-29 09:57:50.000000 mypy-boto3-s3control-1.28.15.post1/mypy_boto3_s3control/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-07-29 09:57:50.000000 mypy-boto3-s3control-1.28.15.post1/mypy_boto3_s3control/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-07-29 09:57:50.000000 mypy-boto3-s3control-1.28.15.post1/mypy_boto3_s3control/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:57:49.000000 mypy-boto3-s3control-1.28.15.post1/mypy_boto3_s3control/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    85262 2023-07-29 09:57:52.000000 mypy-boto3-s3control-1.28.15.post1/mypy_boto3_s3control/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    85163 2023-07-29 09:57:51.000000 mypy-boto3-s3control-1.28.15.post1/mypy_boto3_s3control/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:57:49.000000 mypy-boto3-s3control-1.28.15.post1/mypy_boto3_s3control/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:04.869378 mypy-boto3-s3control-1.28.15.post1/mypy_boto3_s3control.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    24030 2023-07-29 10:04:04.000000 mypy-boto3-s3control-1.28.15.post1/mypy_boto3_s3control.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-29 10:04:04.000000 mypy-boto3-s3control-1.28.15.post1/mypy_boto3_s3control.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:04.000000 mypy-boto3-s3control-1.28.15.post1/mypy_boto3_s3control.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:04.000000 mypy-boto3-s3control-1.28.15.post1/mypy_boto3_s3control.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:04:04.000000 mypy-boto3-s3control-1.28.15.post1/mypy_boto3_s3control.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-29 10:04:04.000000 mypy-boto3-s3control-1.28.15.post1/mypy_boto3_s3control.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:04:04.869378 mypy-boto3-s3control-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-07-29 09:57:49.000000 mypy-boto3-s3control-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:44.764757 mypy-boto3-s3control-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:31:15.000000 mypy-boto3-s3control-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    24317 2023-08-01 11:37:44.756757 mypy-boto3-s3control-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22825 2023-08-01 11:31:14.000000 mypy-boto3-s3control-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:44.748757 mypy-boto3-s3control-1.28.16/mypy_boto3_s3control/
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-08-01 11:31:15.000000 mypy-boto3-s3control-1.28.16/mypy_boto3_s3control/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-08-01 11:31:15.000000 mypy-boto3-s3control-1.28.16/mypy_boto3_s3control/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-08-01 11:31:15.000000 mypy-boto3-s3control-1.28.16/mypy_boto3_s3control/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43162 2023-08-01 11:31:15.000000 mypy-boto3-s3control-1.28.16/mypy_boto3_s3control/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43090 2023-08-01 11:31:15.000000 mypy-boto3-s3control-1.28.16/mypy_boto3_s3control/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13694 2023-08-01 11:31:15.000000 mypy-boto3-s3control-1.28.16/mypy_boto3_s3control/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13692 2023-08-01 11:31:15.000000 mypy-boto3-s3control-1.28.16/mypy_boto3_s3control/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-08-01 11:31:15.000000 mypy-boto3-s3control-1.28.16/mypy_boto3_s3control/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-08-01 11:31:15.000000 mypy-boto3-s3control-1.28.16/mypy_boto3_s3control/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:31:15.000000 mypy-boto3-s3control-1.28.16/mypy_boto3_s3control/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    86369 2023-08-01 11:31:18.000000 mypy-boto3-s3control-1.28.16/mypy_boto3_s3control/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86270 2023-08-01 11:31:16.000000 mypy-boto3-s3control-1.28.16/mypy_boto3_s3control/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:31:15.000000 mypy-boto3-s3control-1.28.16/mypy_boto3_s3control/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:44.756757 mypy-boto3-s3control-1.28.16/mypy_boto3_s3control.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    24317 2023-08-01 11:37:44.000000 mypy-boto3-s3control-1.28.16/mypy_boto3_s3control.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-08-01 11:37:44.000000 mypy-boto3-s3control-1.28.16/mypy_boto3_s3control.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:44.000000 mypy-boto3-s3control-1.28.16/mypy_boto3_s3control.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:44.000000 mypy-boto3-s3control-1.28.16/mypy_boto3_s3control.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:44.000000 mypy-boto3-s3control-1.28.16/mypy_boto3_s3control.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-01 11:37:44.000000 mypy-boto3-s3control-1.28.16/mypy_boto3_s3control.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:44.764757 mypy-boto3-s3control-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-08-01 11:31:14.000000 mypy-boto3-s3control-1.28.16/setup.py
```

### Comparing `mypy-boto3-s3control-1.28.15.post1/LICENSE` & `mypy-boto3-s3control-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3control-1.28.15.post1/PKG-INFO` & `mypy-boto3-s3control-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-s3control
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.S3Control 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.S3Control 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 s3control type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 s3control type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-s3control.svg?color=blue)](https://pypi.org/project/mypy-boto3-s3control)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-s3control)](https://pepy.tech/project/mypy-boto3-s3control)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.S3Control 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control)
+[boto3.S3Control 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control)
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
 [mypy-boto3-s3control docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/).
 
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
@@ -355,20 +355,20 @@
 )
 
 
 def check_value(value: AsyncOperationNameType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_s3control.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_s3control.type_defs import (
     AbortIncompleteMultipartUploadTypeDef,
     AccessControlTranslationTypeDef,
     VpcConfigurationTypeDef,
     ActivityMetricsTypeDef,
@@ -433,27 +433,25 @@
     GetStorageLensConfigurationRequestRequestTypeDef,
     GetStorageLensConfigurationTaggingRequestRequestTypeDef,
     StorageLensTagTypeDef,
     IncludeOutputTypeDef,
     IncludeTypeDef,
     JobFailureTypeDef,
     JobManifestGeneratorFilterOutputTypeDef,
-    JobManifestGeneratorFilterTypeDef,
+    TimestampTypeDef,
     JobManifestLocationTypeDef,
     JobManifestSpecOutputTypeDef,
     JobManifestSpecTypeDef,
     LambdaInvokeOperationTypeDef,
     S3InitiateRestoreObjectOperationTypeDef,
     JobTimersTypeDef,
     LifecycleExpirationOutputTypeDef,
-    LifecycleExpirationTypeDef,
     NoncurrentVersionExpirationTypeDef,
     NoncurrentVersionTransitionTypeDef,
     TransitionOutputTypeDef,
-    TransitionTypeDef,
     PaginatorConfigTypeDef,
     ListAccessPointsForObjectLambdaRequestRequestTypeDef,
     ListAccessPointsRequestRequestTypeDef,
     ListJobsRequestRequestTypeDef,
     ListMultiRegionAccessPointsRequestRequestTypeDef,
     ListRegionalBucketsRequestRequestTypeDef,
     RegionalBucketTypeDef,
@@ -467,19 +465,17 @@
     PutAccessPointPolicyForObjectLambdaRequestRequestTypeDef,
     PutAccessPointPolicyRequestRequestTypeDef,
     PutBucketPolicyRequestRequestTypeDef,
     VersioningConfigurationTypeDef,
     ReplicaModificationsTypeDef,
     S3ObjectOwnerTypeDef,
     S3ObjectMetadataOutputTypeDef,
-    S3ObjectMetadataTypeDef,
     S3GranteeTypeDef,
     S3ObjectLockLegalHoldTypeDef,
     S3RetentionOutputTypeDef,
-    S3RetentionTypeDef,
     SSEKMSTypeDef,
     SseKmsEncryptedObjectsTypeDef,
     StorageLensAwsOrgTypeDef,
     UpdateJobPriorityRequestRequestTypeDef,
     UpdateJobStatusRequestRequestTypeDef,
     AccessPointTypeDef,
     DeleteMultiRegionAccessPointRequestRequestTypeDef,
@@ -524,14 +520,19 @@
     GetAccessPointPolicyStatusForObjectLambdaResultTypeDef,
     GetAccessPointPolicyStatusResultTypeDef,
     GetMultiRegionAccessPointPolicyStatusResultTypeDef,
     GetMultiRegionAccessPointRoutesResultTypeDef,
     SubmitMultiRegionAccessPointRoutesRequestRequestTypeDef,
     GetStorageLensConfigurationTaggingResultTypeDef,
     PutStorageLensConfigurationTaggingRequestRequestTypeDef,
+    JobManifestGeneratorFilterTypeDef,
+    LifecycleExpirationTypeDef,
+    S3ObjectMetadataTypeDef,
+    S3RetentionTypeDef,
+    TransitionTypeDef,
     S3GeneratedManifestDescriptorTypeDef,
     JobManifestOutputTypeDef,
     JobManifestTypeDef,
     JobProgressSummaryTypeDef,
     ListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef,
     ListRegionalBucketsResultTypeDef,
     ListStorageLensConfigurationsResultTypeDef,
@@ -541,31 +542,33 @@
     MultiRegionAccessPointsAsyncResponseTypeDef,
     MultiRegionAccessPointReportTypeDef,
     PrefixLevelStorageMetricsTypeDef,
     PutBucketVersioningRequestRequestTypeDef,
     S3GrantTypeDef,
     S3SetObjectLegalHoldOperationTypeDef,
     S3SetObjectRetentionOperationOutputTypeDef,
-    S3SetObjectRetentionOperationTypeDef,
     StorageLensDataExportEncryptionOutputTypeDef,
     StorageLensDataExportEncryptionTypeDef,
     SourceSelectionCriteriaTypeDef,
     ListAccessPointsResultTypeDef,
     ObjectLambdaTransformationConfigurationOutputTypeDef,
     ObjectLambdaTransformationConfigurationTypeDef,
     ListAccessPointsForObjectLambdaResultTypeDef,
     LifecycleRuleFilterOutputTypeDef,
     LifecycleRuleFilterTypeDef,
     ReplicationRuleFilterOutputTypeDef,
     ReplicationRuleFilterTypeDef,
     PutBucketTaggingRequestRequestTypeDef,
     AsyncRequestParametersTypeDef,
+    CreateMultiRegionAccessPointInputUnionTypeDef,
     CreateMultiRegionAccessPointRequestRequestTypeDef,
     S3ManifestOutputLocationOutputTypeDef,
     S3ManifestOutputLocationTypeDef,
+    S3SetObjectRetentionOperationTypeDef,
+    JobManifestUnionTypeDef,
     JobListDescriptorTypeDef,
     DestinationTypeDef,
     GetMultiRegionAccessPointPolicyResultTypeDef,
     AsyncResponseDetailsTypeDef,
     GetMultiRegionAccessPointResultTypeDef,
     ListMultiRegionAccessPointsResultTypeDef,
     PrefixLevelTypeDef,
@@ -588,41 +591,46 @@
     BucketLevelTypeDef,
     S3AccessControlPolicyOutputTypeDef,
     S3AccessControlPolicyTypeDef,
     StorageLensDataExportOutputTypeDef,
     StorageLensDataExportTypeDef,
     GetAccessPointConfigurationForObjectLambdaResultTypeDef,
     CreateAccessPointForObjectLambdaRequestRequestTypeDef,
+    ObjectLambdaConfigurationUnionTypeDef,
     PutAccessPointConfigurationForObjectLambdaRequestRequestTypeDef,
     GetBucketLifecycleConfigurationResultTypeDef,
     LifecycleConfigurationTypeDef,
     JobManifestGeneratorOutputTypeDef,
     JobManifestGeneratorTypeDef,
     ReplicationConfigurationOutputTypeDef,
     ReplicationConfigurationTypeDef,
     DescribeMultiRegionAccessPointOperationResultTypeDef,
     AccountLevelTypeDef,
     S3SetObjectAclOperationOutputTypeDef,
     S3SetObjectAclOperationTypeDef,
     PutBucketLifecycleConfigurationRequestRequestTypeDef,
+    JobManifestGeneratorUnionTypeDef,
     GetBucketReplicationResultTypeDef,
     PutBucketReplicationRequestRequestTypeDef,
+    ReplicationConfigurationUnionTypeDef,
     StorageLensConfigurationOutputTypeDef,
     StorageLensConfigurationTypeDef,
     JobOperationOutputTypeDef,
     JobOperationTypeDef,
     GetStorageLensConfigurationResultTypeDef,
     PutStorageLensConfigurationRequestRequestTypeDef,
+    StorageLensConfigurationUnionTypeDef,
     JobDescriptorTypeDef,
     CreateJobRequestRequestTypeDef,
+    JobOperationUnionTypeDef,
     DescribeJobResultTypeDef,
 )
 
 
-def get_structure() -> AbortIncompleteMultipartUploadTypeDef:
+def get_value() -> AbortIncompleteMultipartUploadTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-s3control-1.28.15.post1/README.md` & `mypy-boto3-s3control-1.28.16/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-s3control.svg?color=blue)](https://pypi.org/project/mypy-boto3-s3control)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-s3control)](https://pepy.tech/project/mypy-boto3-s3control)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.S3Control 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control)
+[boto3.S3Control 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control)
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
 [mypy-boto3-s3control docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/).
 
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
@@ -323,20 +323,20 @@
 )
 
 
 def check_value(value: AsyncOperationNameType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_s3control.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_s3control.type_defs import (
     AbortIncompleteMultipartUploadTypeDef,
     AccessControlTranslationTypeDef,
     VpcConfigurationTypeDef,
     ActivityMetricsTypeDef,
@@ -401,27 +401,25 @@
     GetStorageLensConfigurationRequestRequestTypeDef,
     GetStorageLensConfigurationTaggingRequestRequestTypeDef,
     StorageLensTagTypeDef,
     IncludeOutputTypeDef,
     IncludeTypeDef,
     JobFailureTypeDef,
     JobManifestGeneratorFilterOutputTypeDef,
-    JobManifestGeneratorFilterTypeDef,
+    TimestampTypeDef,
     JobManifestLocationTypeDef,
     JobManifestSpecOutputTypeDef,
     JobManifestSpecTypeDef,
     LambdaInvokeOperationTypeDef,
     S3InitiateRestoreObjectOperationTypeDef,
     JobTimersTypeDef,
     LifecycleExpirationOutputTypeDef,
-    LifecycleExpirationTypeDef,
     NoncurrentVersionExpirationTypeDef,
     NoncurrentVersionTransitionTypeDef,
     TransitionOutputTypeDef,
-    TransitionTypeDef,
     PaginatorConfigTypeDef,
     ListAccessPointsForObjectLambdaRequestRequestTypeDef,
     ListAccessPointsRequestRequestTypeDef,
     ListJobsRequestRequestTypeDef,
     ListMultiRegionAccessPointsRequestRequestTypeDef,
     ListRegionalBucketsRequestRequestTypeDef,
     RegionalBucketTypeDef,
@@ -435,19 +433,17 @@
     PutAccessPointPolicyForObjectLambdaRequestRequestTypeDef,
     PutAccessPointPolicyRequestRequestTypeDef,
     PutBucketPolicyRequestRequestTypeDef,
     VersioningConfigurationTypeDef,
     ReplicaModificationsTypeDef,
     S3ObjectOwnerTypeDef,
     S3ObjectMetadataOutputTypeDef,
-    S3ObjectMetadataTypeDef,
     S3GranteeTypeDef,
     S3ObjectLockLegalHoldTypeDef,
     S3RetentionOutputTypeDef,
-    S3RetentionTypeDef,
     SSEKMSTypeDef,
     SseKmsEncryptedObjectsTypeDef,
     StorageLensAwsOrgTypeDef,
     UpdateJobPriorityRequestRequestTypeDef,
     UpdateJobStatusRequestRequestTypeDef,
     AccessPointTypeDef,
     DeleteMultiRegionAccessPointRequestRequestTypeDef,
@@ -492,14 +488,19 @@
     GetAccessPointPolicyStatusForObjectLambdaResultTypeDef,
     GetAccessPointPolicyStatusResultTypeDef,
     GetMultiRegionAccessPointPolicyStatusResultTypeDef,
     GetMultiRegionAccessPointRoutesResultTypeDef,
     SubmitMultiRegionAccessPointRoutesRequestRequestTypeDef,
     GetStorageLensConfigurationTaggingResultTypeDef,
     PutStorageLensConfigurationTaggingRequestRequestTypeDef,
+    JobManifestGeneratorFilterTypeDef,
+    LifecycleExpirationTypeDef,
+    S3ObjectMetadataTypeDef,
+    S3RetentionTypeDef,
+    TransitionTypeDef,
     S3GeneratedManifestDescriptorTypeDef,
     JobManifestOutputTypeDef,
     JobManifestTypeDef,
     JobProgressSummaryTypeDef,
     ListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef,
     ListRegionalBucketsResultTypeDef,
     ListStorageLensConfigurationsResultTypeDef,
@@ -509,31 +510,33 @@
     MultiRegionAccessPointsAsyncResponseTypeDef,
     MultiRegionAccessPointReportTypeDef,
     PrefixLevelStorageMetricsTypeDef,
     PutBucketVersioningRequestRequestTypeDef,
     S3GrantTypeDef,
     S3SetObjectLegalHoldOperationTypeDef,
     S3SetObjectRetentionOperationOutputTypeDef,
-    S3SetObjectRetentionOperationTypeDef,
     StorageLensDataExportEncryptionOutputTypeDef,
     StorageLensDataExportEncryptionTypeDef,
     SourceSelectionCriteriaTypeDef,
     ListAccessPointsResultTypeDef,
     ObjectLambdaTransformationConfigurationOutputTypeDef,
     ObjectLambdaTransformationConfigurationTypeDef,
     ListAccessPointsForObjectLambdaResultTypeDef,
     LifecycleRuleFilterOutputTypeDef,
     LifecycleRuleFilterTypeDef,
     ReplicationRuleFilterOutputTypeDef,
     ReplicationRuleFilterTypeDef,
     PutBucketTaggingRequestRequestTypeDef,
     AsyncRequestParametersTypeDef,
+    CreateMultiRegionAccessPointInputUnionTypeDef,
     CreateMultiRegionAccessPointRequestRequestTypeDef,
     S3ManifestOutputLocationOutputTypeDef,
     S3ManifestOutputLocationTypeDef,
+    S3SetObjectRetentionOperationTypeDef,
+    JobManifestUnionTypeDef,
     JobListDescriptorTypeDef,
     DestinationTypeDef,
     GetMultiRegionAccessPointPolicyResultTypeDef,
     AsyncResponseDetailsTypeDef,
     GetMultiRegionAccessPointResultTypeDef,
     ListMultiRegionAccessPointsResultTypeDef,
     PrefixLevelTypeDef,
@@ -556,41 +559,46 @@
     BucketLevelTypeDef,
     S3AccessControlPolicyOutputTypeDef,
     S3AccessControlPolicyTypeDef,
     StorageLensDataExportOutputTypeDef,
     StorageLensDataExportTypeDef,
     GetAccessPointConfigurationForObjectLambdaResultTypeDef,
     CreateAccessPointForObjectLambdaRequestRequestTypeDef,
+    ObjectLambdaConfigurationUnionTypeDef,
     PutAccessPointConfigurationForObjectLambdaRequestRequestTypeDef,
     GetBucketLifecycleConfigurationResultTypeDef,
     LifecycleConfigurationTypeDef,
     JobManifestGeneratorOutputTypeDef,
     JobManifestGeneratorTypeDef,
     ReplicationConfigurationOutputTypeDef,
     ReplicationConfigurationTypeDef,
     DescribeMultiRegionAccessPointOperationResultTypeDef,
     AccountLevelTypeDef,
     S3SetObjectAclOperationOutputTypeDef,
     S3SetObjectAclOperationTypeDef,
     PutBucketLifecycleConfigurationRequestRequestTypeDef,
+    JobManifestGeneratorUnionTypeDef,
     GetBucketReplicationResultTypeDef,
     PutBucketReplicationRequestRequestTypeDef,
+    ReplicationConfigurationUnionTypeDef,
     StorageLensConfigurationOutputTypeDef,
     StorageLensConfigurationTypeDef,
     JobOperationOutputTypeDef,
     JobOperationTypeDef,
     GetStorageLensConfigurationResultTypeDef,
     PutStorageLensConfigurationRequestRequestTypeDef,
+    StorageLensConfigurationUnionTypeDef,
     JobDescriptorTypeDef,
     CreateJobRequestRequestTypeDef,
+    JobOperationUnionTypeDef,
     DescribeJobResultTypeDef,
 )
 
 
-def get_structure() -> AbortIncompleteMultipartUploadTypeDef:
+def get_value() -> AbortIncompleteMultipartUploadTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-s3control-1.28.15.post1/mypy_boto3_s3control/__init__.py` & `mypy-boto3-s3control-1.28.16/mypy_boto3_s3control/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3control-1.28.15.post1/mypy_boto3_s3control/__init__.pyi` & `mypy-boto3-s3control-1.28.16/mypy_boto3_s3control/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3control-1.28.15.post1/mypy_boto3_s3control/__main__.py` & `mypy-boto3-s3control-1.28.16/mypy_boto3_s3control/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.S3Control 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.S3Control 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control\nOther"
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

### Comparing `mypy-boto3-s3control-1.28.15.post1/mypy_boto3_s3control/client.py` & `mypy-boto3-s3control-1.28.16/mypy_boto3_s3control/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,28 +10,27 @@
     from mypy_boto3_s3control.client import S3ControlClient
 
     session = Session()
     client: S3ControlClient = session.client("s3control")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import BucketCannedACLType, JobStatusType, RequestedJobStatusType
 from .paginator import ListAccessPointsForObjectLambdaPaginator
 from .type_defs import (
     CreateAccessPointForObjectLambdaResultTypeDef,
     CreateAccessPointResultTypeDef,
     CreateBucketConfigurationTypeDef,
     CreateBucketResultTypeDef,
     CreateJobResultTypeDef,
-    CreateMultiRegionAccessPointInputOutputTypeDef,
-    CreateMultiRegionAccessPointInputTypeDef,
+    CreateMultiRegionAccessPointInputUnionTypeDef,
     CreateMultiRegionAccessPointResultTypeDef,
     DeleteMultiRegionAccessPointInputTypeDef,
     DeleteMultiRegionAccessPointResultTypeDef,
     DescribeJobResultTypeDef,
     DescribeMultiRegionAccessPointOperationResultTypeDef,
     EmptyResponseMetadataTypeDef,
     GetAccessPointConfigurationForObjectLambdaResultTypeDef,
@@ -51,39 +50,33 @@
     GetMultiRegionAccessPointPolicyResultTypeDef,
     GetMultiRegionAccessPointPolicyStatusResultTypeDef,
     GetMultiRegionAccessPointResultTypeDef,
     GetMultiRegionAccessPointRoutesResultTypeDef,
     GetPublicAccessBlockOutputTypeDef,
     GetStorageLensConfigurationResultTypeDef,
     GetStorageLensConfigurationTaggingResultTypeDef,
-    JobManifestGeneratorOutputTypeDef,
-    JobManifestGeneratorTypeDef,
-    JobManifestOutputTypeDef,
-    JobManifestTypeDef,
-    JobOperationOutputTypeDef,
-    JobOperationTypeDef,
+    JobManifestGeneratorUnionTypeDef,
+    JobManifestUnionTypeDef,
+    JobOperationUnionTypeDef,
     JobReportTypeDef,
     LifecycleConfigurationTypeDef,
     ListAccessPointsForObjectLambdaResultTypeDef,
     ListAccessPointsResultTypeDef,
     ListJobsResultTypeDef,
     ListMultiRegionAccessPointsResultTypeDef,
     ListRegionalBucketsResultTypeDef,
     ListStorageLensConfigurationsResultTypeDef,
     MultiRegionAccessPointRouteTypeDef,
-    ObjectLambdaConfigurationOutputTypeDef,
-    ObjectLambdaConfigurationTypeDef,
+    ObjectLambdaConfigurationUnionTypeDef,
     PublicAccessBlockConfigurationTypeDef,
     PutMultiRegionAccessPointPolicyInputTypeDef,
     PutMultiRegionAccessPointPolicyResultTypeDef,
-    ReplicationConfigurationOutputTypeDef,
-    ReplicationConfigurationTypeDef,
+    ReplicationConfigurationUnionTypeDef,
     S3TagTypeDef,
-    StorageLensConfigurationOutputTypeDef,
-    StorageLensConfigurationTypeDef,
+    StorageLensConfigurationUnionTypeDef,
     StorageLensTagTypeDef,
     TaggingTypeDef,
     UpdateJobPriorityResultTypeDef,
     UpdateJobStatusResultTypeDef,
     VersioningConfigurationTypeDef,
     VpcConfigurationTypeDef,
 )
@@ -168,21 +161,15 @@
         Creates an access point and associates it with the specified bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.create_access_point)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/client/#create_access_point)
         """
 
     def create_access_point_for_object_lambda(
-        self,
-        *,
-        AccountId: str,
-        Name: str,
-        Configuration: Union[
-            ObjectLambdaConfigurationTypeDef, ObjectLambdaConfigurationOutputTypeDef
-        ]
+        self, *, AccountId: str, Name: str, Configuration: ObjectLambdaConfigurationUnionTypeDef
     ) -> CreateAccessPointForObjectLambdaResultTypeDef:
         """
         Creates an Object Lambda Access Point.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.create_access_point_for_object_lambda)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/client/#create_access_point_for_object_lambda)
         """
@@ -208,43 +195,39 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/client/#create_bucket)
         """
 
     def create_job(
         self,
         *,
         AccountId: str,
-        Operation: Union[JobOperationTypeDef, JobOperationOutputTypeDef],
+        Operation: JobOperationUnionTypeDef,
         Report: JobReportTypeDef,
         ClientRequestToken: str,
         Priority: int,
         RoleArn: str,
         ConfirmationRequired: bool = ...,
-        Manifest: Union[JobManifestTypeDef, JobManifestOutputTypeDef] = ...,
+        Manifest: JobManifestUnionTypeDef = ...,
         Description: str = ...,
         Tags: Sequence[S3TagTypeDef] = ...,
-        ManifestGenerator: Union[
-            JobManifestGeneratorTypeDef, JobManifestGeneratorOutputTypeDef
-        ] = ...
+        ManifestGenerator: JobManifestGeneratorUnionTypeDef = ...
     ) -> CreateJobResultTypeDef:
         """
         You can use S3 Batch Operations to perform large-scale batch actions on Amazon
         S3 objects.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.create_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/client/#create_job)
         """
 
     def create_multi_region_access_point(
         self,
         *,
         AccountId: str,
         ClientToken: str,
-        Details: Union[
-            CreateMultiRegionAccessPointInputTypeDef, CreateMultiRegionAccessPointInputOutputTypeDef
-        ]
+        Details: CreateMultiRegionAccessPointInputUnionTypeDef
     ) -> CreateMultiRegionAccessPointResultTypeDef:
         """
         Creates a Multi-Region Access Point and associates it with the specified
         buckets.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.create_multi_region_access_point)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/client/#create_multi_region_access_point)
@@ -685,21 +668,15 @@
         Gets a list of Amazon S3 Storage Lens configurations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.list_storage_lens_configurations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/client/#list_storage_lens_configurations)
         """
 
     def put_access_point_configuration_for_object_lambda(
-        self,
-        *,
-        AccountId: str,
-        Name: str,
-        Configuration: Union[
-            ObjectLambdaConfigurationTypeDef, ObjectLambdaConfigurationOutputTypeDef
-        ]
+        self, *, AccountId: str, Name: str, Configuration: ObjectLambdaConfigurationUnionTypeDef
     ) -> EmptyResponseMetadataTypeDef:
         """
         Replaces configuration for an Object Lambda Access Point.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.put_access_point_configuration_for_object_lambda)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/client/#put_access_point_configuration_for_object_lambda)
         """
@@ -749,17 +726,15 @@
         """
 
     def put_bucket_replication(
         self,
         *,
         AccountId: str,
         Bucket: str,
-        ReplicationConfiguration: Union[
-            ReplicationConfigurationTypeDef, ReplicationConfigurationOutputTypeDef
-        ]
+        ReplicationConfiguration: ReplicationConfigurationUnionTypeDef
     ) -> EmptyResponseMetadataTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.put_bucket_replication)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/client/#put_bucket_replication)
         """
@@ -829,17 +804,15 @@
         """
 
     def put_storage_lens_configuration(
         self,
         *,
         ConfigId: str,
         AccountId: str,
-        StorageLensConfiguration: Union[
-            StorageLensConfigurationTypeDef, StorageLensConfigurationOutputTypeDef
-        ],
+        StorageLensConfiguration: StorageLensConfigurationUnionTypeDef,
         Tags: Sequence[StorageLensTagTypeDef] = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Puts an Amazon S3 Storage Lens configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.put_storage_lens_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/client/#put_storage_lens_configuration)
```

### Comparing `mypy-boto3-s3control-1.28.15.post1/mypy_boto3_s3control/client.pyi` & `mypy-boto3-s3control-1.28.16/mypy_boto3_s3control/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -10,28 +10,27 @@
     from mypy_boto3_s3control.client import S3ControlClient
 
     session = Session()
     client: S3ControlClient = session.client("s3control")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import BucketCannedACLType, JobStatusType, RequestedJobStatusType
 from .paginator import ListAccessPointsForObjectLambdaPaginator
 from .type_defs import (
     CreateAccessPointForObjectLambdaResultTypeDef,
     CreateAccessPointResultTypeDef,
     CreateBucketConfigurationTypeDef,
     CreateBucketResultTypeDef,
     CreateJobResultTypeDef,
-    CreateMultiRegionAccessPointInputOutputTypeDef,
-    CreateMultiRegionAccessPointInputTypeDef,
+    CreateMultiRegionAccessPointInputUnionTypeDef,
     CreateMultiRegionAccessPointResultTypeDef,
     DeleteMultiRegionAccessPointInputTypeDef,
     DeleteMultiRegionAccessPointResultTypeDef,
     DescribeJobResultTypeDef,
     DescribeMultiRegionAccessPointOperationResultTypeDef,
     EmptyResponseMetadataTypeDef,
     GetAccessPointConfigurationForObjectLambdaResultTypeDef,
@@ -51,39 +50,33 @@
     GetMultiRegionAccessPointPolicyResultTypeDef,
     GetMultiRegionAccessPointPolicyStatusResultTypeDef,
     GetMultiRegionAccessPointResultTypeDef,
     GetMultiRegionAccessPointRoutesResultTypeDef,
     GetPublicAccessBlockOutputTypeDef,
     GetStorageLensConfigurationResultTypeDef,
     GetStorageLensConfigurationTaggingResultTypeDef,
-    JobManifestGeneratorOutputTypeDef,
-    JobManifestGeneratorTypeDef,
-    JobManifestOutputTypeDef,
-    JobManifestTypeDef,
-    JobOperationOutputTypeDef,
-    JobOperationTypeDef,
+    JobManifestGeneratorUnionTypeDef,
+    JobManifestUnionTypeDef,
+    JobOperationUnionTypeDef,
     JobReportTypeDef,
     LifecycleConfigurationTypeDef,
     ListAccessPointsForObjectLambdaResultTypeDef,
     ListAccessPointsResultTypeDef,
     ListJobsResultTypeDef,
     ListMultiRegionAccessPointsResultTypeDef,
     ListRegionalBucketsResultTypeDef,
     ListStorageLensConfigurationsResultTypeDef,
     MultiRegionAccessPointRouteTypeDef,
-    ObjectLambdaConfigurationOutputTypeDef,
-    ObjectLambdaConfigurationTypeDef,
+    ObjectLambdaConfigurationUnionTypeDef,
     PublicAccessBlockConfigurationTypeDef,
     PutMultiRegionAccessPointPolicyInputTypeDef,
     PutMultiRegionAccessPointPolicyResultTypeDef,
-    ReplicationConfigurationOutputTypeDef,
-    ReplicationConfigurationTypeDef,
+    ReplicationConfigurationUnionTypeDef,
     S3TagTypeDef,
-    StorageLensConfigurationOutputTypeDef,
-    StorageLensConfigurationTypeDef,
+    StorageLensConfigurationUnionTypeDef,
     StorageLensTagTypeDef,
     TaggingTypeDef,
     UpdateJobPriorityResultTypeDef,
     UpdateJobStatusResultTypeDef,
     VersioningConfigurationTypeDef,
     VpcConfigurationTypeDef,
 )
@@ -160,21 +153,15 @@
         """
         Creates an access point and associates it with the specified bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.create_access_point)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/client/#create_access_point)
         """
     def create_access_point_for_object_lambda(
-        self,
-        *,
-        AccountId: str,
-        Name: str,
-        Configuration: Union[
-            ObjectLambdaConfigurationTypeDef, ObjectLambdaConfigurationOutputTypeDef
-        ]
+        self, *, AccountId: str, Name: str, Configuration: ObjectLambdaConfigurationUnionTypeDef
     ) -> CreateAccessPointForObjectLambdaResultTypeDef:
         """
         Creates an Object Lambda Access Point.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.create_access_point_for_object_lambda)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/client/#create_access_point_for_object_lambda)
         """
@@ -198,42 +185,38 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.create_bucket)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/client/#create_bucket)
         """
     def create_job(
         self,
         *,
         AccountId: str,
-        Operation: Union[JobOperationTypeDef, JobOperationOutputTypeDef],
+        Operation: JobOperationUnionTypeDef,
         Report: JobReportTypeDef,
         ClientRequestToken: str,
         Priority: int,
         RoleArn: str,
         ConfirmationRequired: bool = ...,
-        Manifest: Union[JobManifestTypeDef, JobManifestOutputTypeDef] = ...,
+        Manifest: JobManifestUnionTypeDef = ...,
         Description: str = ...,
         Tags: Sequence[S3TagTypeDef] = ...,
-        ManifestGenerator: Union[
-            JobManifestGeneratorTypeDef, JobManifestGeneratorOutputTypeDef
-        ] = ...
+        ManifestGenerator: JobManifestGeneratorUnionTypeDef = ...
     ) -> CreateJobResultTypeDef:
         """
         You can use S3 Batch Operations to perform large-scale batch actions on Amazon
         S3 objects.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.create_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/client/#create_job)
         """
     def create_multi_region_access_point(
         self,
         *,
         AccountId: str,
         ClientToken: str,
-        Details: Union[
-            CreateMultiRegionAccessPointInputTypeDef, CreateMultiRegionAccessPointInputOutputTypeDef
-        ]
+        Details: CreateMultiRegionAccessPointInputUnionTypeDef
     ) -> CreateMultiRegionAccessPointResultTypeDef:
         """
         Creates a Multi-Region Access Point and associates it with the specified
         buckets.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.create_multi_region_access_point)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/client/#create_multi_region_access_point)
@@ -629,21 +612,15 @@
         """
         Gets a list of Amazon S3 Storage Lens configurations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.list_storage_lens_configurations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/client/#list_storage_lens_configurations)
         """
     def put_access_point_configuration_for_object_lambda(
-        self,
-        *,
-        AccountId: str,
-        Name: str,
-        Configuration: Union[
-            ObjectLambdaConfigurationTypeDef, ObjectLambdaConfigurationOutputTypeDef
-        ]
+        self, *, AccountId: str, Name: str, Configuration: ObjectLambdaConfigurationUnionTypeDef
     ) -> EmptyResponseMetadataTypeDef:
         """
         Replaces configuration for an Object Lambda Access Point.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.put_access_point_configuration_for_object_lambda)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/client/#put_access_point_configuration_for_object_lambda)
         """
@@ -688,17 +665,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/client/#put_bucket_policy)
         """
     def put_bucket_replication(
         self,
         *,
         AccountId: str,
         Bucket: str,
-        ReplicationConfiguration: Union[
-            ReplicationConfigurationTypeDef, ReplicationConfigurationOutputTypeDef
-        ]
+        ReplicationConfiguration: ReplicationConfigurationUnionTypeDef
     ) -> EmptyResponseMetadataTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.put_bucket_replication)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/client/#put_bucket_replication)
         """
@@ -762,17 +737,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/client/#put_public_access_block)
         """
     def put_storage_lens_configuration(
         self,
         *,
         ConfigId: str,
         AccountId: str,
-        StorageLensConfiguration: Union[
-            StorageLensConfigurationTypeDef, StorageLensConfigurationOutputTypeDef
-        ],
+        StorageLensConfiguration: StorageLensConfigurationUnionTypeDef,
         Tags: Sequence[StorageLensTagTypeDef] = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Puts an Amazon S3 Storage Lens configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Client.put_storage_lens_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/client/#put_storage_lens_configuration)
```

### Comparing `mypy-boto3-s3control-1.28.15.post1/mypy_boto3_s3control/literals.py` & `mypy-boto3-s3control-1.28.16/mypy_boto3_s3control/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3control-1.28.15.post1/mypy_boto3_s3control/literals.pyi` & `mypy-boto3-s3control-1.28.16/mypy_boto3_s3control/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3control-1.28.15.post1/mypy_boto3_s3control/paginator.py` & `mypy-boto3-s3control-1.28.16/mypy_boto3_s3control/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3control-1.28.15.post1/mypy_boto3_s3control/paginator.pyi` & `mypy-boto3-s3control-1.28.16/mypy_boto3_s3control/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3control-1.28.15.post1/mypy_boto3_s3control/type_defs.py` & `mypy-boto3-s3control-1.28.16/mypy_boto3_s3control/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_s3control.type_defs import AbortIncompleteMultipartUploadTypeDef
 
-    data: AbortIncompleteMultipartUploadTypeDef = {...}
+    data: AbortIncompleteMultipartUploadTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -134,27 +134,25 @@
     "GetStorageLensConfigurationRequestRequestTypeDef",
     "GetStorageLensConfigurationTaggingRequestRequestTypeDef",
     "StorageLensTagTypeDef",
     "IncludeOutputTypeDef",
     "IncludeTypeDef",
     "JobFailureTypeDef",
     "JobManifestGeneratorFilterOutputTypeDef",
-    "JobManifestGeneratorFilterTypeDef",
+    "TimestampTypeDef",
     "JobManifestLocationTypeDef",
     "JobManifestSpecOutputTypeDef",
     "JobManifestSpecTypeDef",
     "LambdaInvokeOperationTypeDef",
     "S3InitiateRestoreObjectOperationTypeDef",
     "JobTimersTypeDef",
     "LifecycleExpirationOutputTypeDef",
-    "LifecycleExpirationTypeDef",
     "NoncurrentVersionExpirationTypeDef",
     "NoncurrentVersionTransitionTypeDef",
     "TransitionOutputTypeDef",
-    "TransitionTypeDef",
     "PaginatorConfigTypeDef",
     "ListAccessPointsForObjectLambdaRequestRequestTypeDef",
     "ListAccessPointsRequestRequestTypeDef",
     "ListJobsRequestRequestTypeDef",
     "ListMultiRegionAccessPointsRequestRequestTypeDef",
     "ListRegionalBucketsRequestRequestTypeDef",
     "RegionalBucketTypeDef",
@@ -168,19 +166,17 @@
     "PutAccessPointPolicyForObjectLambdaRequestRequestTypeDef",
     "PutAccessPointPolicyRequestRequestTypeDef",
     "PutBucketPolicyRequestRequestTypeDef",
     "VersioningConfigurationTypeDef",
     "ReplicaModificationsTypeDef",
     "S3ObjectOwnerTypeDef",
     "S3ObjectMetadataOutputTypeDef",
-    "S3ObjectMetadataTypeDef",
     "S3GranteeTypeDef",
     "S3ObjectLockLegalHoldTypeDef",
     "S3RetentionOutputTypeDef",
-    "S3RetentionTypeDef",
     "SSEKMSTypeDef",
     "SseKmsEncryptedObjectsTypeDef",
     "StorageLensAwsOrgTypeDef",
     "UpdateJobPriorityRequestRequestTypeDef",
     "UpdateJobStatusRequestRequestTypeDef",
     "AccessPointTypeDef",
     "DeleteMultiRegionAccessPointRequestRequestTypeDef",
@@ -225,14 +221,19 @@
     "GetAccessPointPolicyStatusForObjectLambdaResultTypeDef",
     "GetAccessPointPolicyStatusResultTypeDef",
     "GetMultiRegionAccessPointPolicyStatusResultTypeDef",
     "GetMultiRegionAccessPointRoutesResultTypeDef",
     "SubmitMultiRegionAccessPointRoutesRequestRequestTypeDef",
     "GetStorageLensConfigurationTaggingResultTypeDef",
     "PutStorageLensConfigurationTaggingRequestRequestTypeDef",
+    "JobManifestGeneratorFilterTypeDef",
+    "LifecycleExpirationTypeDef",
+    "S3ObjectMetadataTypeDef",
+    "S3RetentionTypeDef",
+    "TransitionTypeDef",
     "S3GeneratedManifestDescriptorTypeDef",
     "JobManifestOutputTypeDef",
     "JobManifestTypeDef",
     "JobProgressSummaryTypeDef",
     "ListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef",
     "ListRegionalBucketsResultTypeDef",
     "ListStorageLensConfigurationsResultTypeDef",
@@ -242,31 +243,33 @@
     "MultiRegionAccessPointsAsyncResponseTypeDef",
     "MultiRegionAccessPointReportTypeDef",
     "PrefixLevelStorageMetricsTypeDef",
     "PutBucketVersioningRequestRequestTypeDef",
     "S3GrantTypeDef",
     "S3SetObjectLegalHoldOperationTypeDef",
     "S3SetObjectRetentionOperationOutputTypeDef",
-    "S3SetObjectRetentionOperationTypeDef",
     "StorageLensDataExportEncryptionOutputTypeDef",
     "StorageLensDataExportEncryptionTypeDef",
     "SourceSelectionCriteriaTypeDef",
     "ListAccessPointsResultTypeDef",
     "ObjectLambdaTransformationConfigurationOutputTypeDef",
     "ObjectLambdaTransformationConfigurationTypeDef",
     "ListAccessPointsForObjectLambdaResultTypeDef",
     "LifecycleRuleFilterOutputTypeDef",
     "LifecycleRuleFilterTypeDef",
     "ReplicationRuleFilterOutputTypeDef",
     "ReplicationRuleFilterTypeDef",
     "PutBucketTaggingRequestRequestTypeDef",
     "AsyncRequestParametersTypeDef",
+    "CreateMultiRegionAccessPointInputUnionTypeDef",
     "CreateMultiRegionAccessPointRequestRequestTypeDef",
     "S3ManifestOutputLocationOutputTypeDef",
     "S3ManifestOutputLocationTypeDef",
+    "S3SetObjectRetentionOperationTypeDef",
+    "JobManifestUnionTypeDef",
     "JobListDescriptorTypeDef",
     "DestinationTypeDef",
     "GetMultiRegionAccessPointPolicyResultTypeDef",
     "AsyncResponseDetailsTypeDef",
     "GetMultiRegionAccessPointResultTypeDef",
     "ListMultiRegionAccessPointsResultTypeDef",
     "PrefixLevelTypeDef",
@@ -289,36 +292,41 @@
     "BucketLevelTypeDef",
     "S3AccessControlPolicyOutputTypeDef",
     "S3AccessControlPolicyTypeDef",
     "StorageLensDataExportOutputTypeDef",
     "StorageLensDataExportTypeDef",
     "GetAccessPointConfigurationForObjectLambdaResultTypeDef",
     "CreateAccessPointForObjectLambdaRequestRequestTypeDef",
+    "ObjectLambdaConfigurationUnionTypeDef",
     "PutAccessPointConfigurationForObjectLambdaRequestRequestTypeDef",
     "GetBucketLifecycleConfigurationResultTypeDef",
     "LifecycleConfigurationTypeDef",
     "JobManifestGeneratorOutputTypeDef",
     "JobManifestGeneratorTypeDef",
     "ReplicationConfigurationOutputTypeDef",
     "ReplicationConfigurationTypeDef",
     "DescribeMultiRegionAccessPointOperationResultTypeDef",
     "AccountLevelTypeDef",
     "S3SetObjectAclOperationOutputTypeDef",
     "S3SetObjectAclOperationTypeDef",
     "PutBucketLifecycleConfigurationRequestRequestTypeDef",
+    "JobManifestGeneratorUnionTypeDef",
     "GetBucketReplicationResultTypeDef",
     "PutBucketReplicationRequestRequestTypeDef",
+    "ReplicationConfigurationUnionTypeDef",
     "StorageLensConfigurationOutputTypeDef",
     "StorageLensConfigurationTypeDef",
     "JobOperationOutputTypeDef",
     "JobOperationTypeDef",
     "GetStorageLensConfigurationResultTypeDef",
     "PutStorageLensConfigurationRequestRequestTypeDef",
+    "StorageLensConfigurationUnionTypeDef",
     "JobDescriptorTypeDef",
     "CreateJobRequestRequestTypeDef",
+    "JobOperationUnionTypeDef",
     "DescribeJobResultTypeDef",
 )
 
 AbortIncompleteMultipartUploadTypeDef = TypedDict(
     "AbortIncompleteMultipartUploadTypeDef",
     {
         "DaysAfterInitiation": int,
@@ -927,25 +935,15 @@
         "CreatedAfter": datetime,
         "CreatedBefore": datetime,
         "ObjectReplicationStatuses": List[ReplicationStatusType],
     },
     total=False,
 )
 
-JobManifestGeneratorFilterTypeDef = TypedDict(
-    "JobManifestGeneratorFilterTypeDef",
-    {
-        "EligibleForReplication": bool,
-        "CreatedAfter": Union[datetime, str],
-        "CreatedBefore": Union[datetime, str],
-        "ObjectReplicationStatuses": Sequence[ReplicationStatusType],
-    },
-    total=False,
-)
-
+TimestampTypeDef = Union[datetime, str]
 _RequiredJobManifestLocationTypeDef = TypedDict(
     "_RequiredJobManifestLocationTypeDef",
     {
         "ObjectArn": str,
         "ETag": str,
     },
 )
@@ -1035,24 +1033,14 @@
         "Date": datetime,
         "Days": int,
         "ExpiredObjectDeleteMarker": bool,
     },
     total=False,
 )
 
-LifecycleExpirationTypeDef = TypedDict(
-    "LifecycleExpirationTypeDef",
-    {
-        "Date": Union[datetime, str],
-        "Days": int,
-        "ExpiredObjectDeleteMarker": bool,
-    },
-    total=False,
-)
-
 NoncurrentVersionExpirationTypeDef = TypedDict(
     "NoncurrentVersionExpirationTypeDef",
     {
         "NoncurrentDays": int,
         "NewerNoncurrentVersions": int,
     },
     total=False,
@@ -1073,24 +1061,14 @@
         "Date": datetime,
         "Days": int,
         "StorageClass": TransitionStorageClassType,
     },
     total=False,
 )
 
-TransitionTypeDef = TypedDict(
-    "TransitionTypeDef",
-    {
-        "Date": Union[datetime, str],
-        "Days": int,
-        "StorageClass": TransitionStorageClassType,
-    },
-    total=False,
-)
-
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
@@ -1406,32 +1384,14 @@
         "HttpExpiresDate": datetime,
         "RequesterCharged": bool,
         "SSEAlgorithm": S3SSEAlgorithmType,
     },
     total=False,
 )
 
-S3ObjectMetadataTypeDef = TypedDict(
-    "S3ObjectMetadataTypeDef",
-    {
-        "CacheControl": str,
-        "ContentDisposition": str,
-        "ContentEncoding": str,
-        "ContentLanguage": str,
-        "UserMetadata": Mapping[str, str],
-        "ContentLength": int,
-        "ContentMD5": str,
-        "ContentType": str,
-        "HttpExpiresDate": Union[datetime, str],
-        "RequesterCharged": bool,
-        "SSEAlgorithm": S3SSEAlgorithmType,
-    },
-    total=False,
-)
-
 S3GranteeTypeDef = TypedDict(
     "S3GranteeTypeDef",
     {
         "TypeIdentifier": S3GranteeTypeIdentifierType,
         "Identifier": str,
         "DisplayName": str,
     },
@@ -1450,23 +1410,14 @@
     {
         "RetainUntilDate": datetime,
         "Mode": S3ObjectLockRetentionModeType,
     },
     total=False,
 )
 
-S3RetentionTypeDef = TypedDict(
-    "S3RetentionTypeDef",
-    {
-        "RetainUntilDate": Union[datetime, str],
-        "Mode": S3ObjectLockRetentionModeType,
-    },
-    total=False,
-)
-
 SSEKMSTypeDef = TypedDict(
     "SSEKMSTypeDef",
     {
         "KeyId": str,
     },
 )
 
@@ -2021,14 +1972,72 @@
     {
         "ConfigId": str,
         "AccountId": str,
         "Tags": Sequence[StorageLensTagTypeDef],
     },
 )
 
+JobManifestGeneratorFilterTypeDef = TypedDict(
+    "JobManifestGeneratorFilterTypeDef",
+    {
+        "EligibleForReplication": bool,
+        "CreatedAfter": TimestampTypeDef,
+        "CreatedBefore": TimestampTypeDef,
+        "ObjectReplicationStatuses": Sequence[ReplicationStatusType],
+    },
+    total=False,
+)
+
+LifecycleExpirationTypeDef = TypedDict(
+    "LifecycleExpirationTypeDef",
+    {
+        "Date": TimestampTypeDef,
+        "Days": int,
+        "ExpiredObjectDeleteMarker": bool,
+    },
+    total=False,
+)
+
+S3ObjectMetadataTypeDef = TypedDict(
+    "S3ObjectMetadataTypeDef",
+    {
+        "CacheControl": str,
+        "ContentDisposition": str,
+        "ContentEncoding": str,
+        "ContentLanguage": str,
+        "UserMetadata": Mapping[str, str],
+        "ContentLength": int,
+        "ContentMD5": str,
+        "ContentType": str,
+        "HttpExpiresDate": TimestampTypeDef,
+        "RequesterCharged": bool,
+        "SSEAlgorithm": S3SSEAlgorithmType,
+    },
+    total=False,
+)
+
+S3RetentionTypeDef = TypedDict(
+    "S3RetentionTypeDef",
+    {
+        "RetainUntilDate": TimestampTypeDef,
+        "Mode": S3ObjectLockRetentionModeType,
+    },
+    total=False,
+)
+
+TransitionTypeDef = TypedDict(
+    "TransitionTypeDef",
+    {
+        "Date": TimestampTypeDef,
+        "Days": int,
+        "StorageClass": TransitionStorageClassType,
+    },
+    total=False,
+)
+
 S3GeneratedManifestDescriptorTypeDef = TypedDict(
     "S3GeneratedManifestDescriptorTypeDef",
     {
         "Format": Literal["S3InventoryReport_CSV_20211130"],
         "Location": JobManifestLocationTypeDef,
     },
     total=False,
@@ -2225,35 +2234,14 @@
 class S3SetObjectRetentionOperationOutputTypeDef(
     _RequiredS3SetObjectRetentionOperationOutputTypeDef,
     _OptionalS3SetObjectRetentionOperationOutputTypeDef,
 ):
     pass
 
 
-_RequiredS3SetObjectRetentionOperationTypeDef = TypedDict(
-    "_RequiredS3SetObjectRetentionOperationTypeDef",
-    {
-        "Retention": S3RetentionTypeDef,
-    },
-)
-_OptionalS3SetObjectRetentionOperationTypeDef = TypedDict(
-    "_OptionalS3SetObjectRetentionOperationTypeDef",
-    {
-        "BypassGovernanceRetention": bool,
-    },
-    total=False,
-)
-
-
-class S3SetObjectRetentionOperationTypeDef(
-    _RequiredS3SetObjectRetentionOperationTypeDef, _OptionalS3SetObjectRetentionOperationTypeDef
-):
-    pass
-
-
 StorageLensDataExportEncryptionOutputTypeDef = TypedDict(
     "StorageLensDataExportEncryptionOutputTypeDef",
     {
         "SSES3": Dict[str, Any],
         "SSEKMS": SSEKMSTypeDef,
     },
     total=False,
@@ -2370,14 +2358,17 @@
         "CreateMultiRegionAccessPointRequest": CreateMultiRegionAccessPointInputOutputTypeDef,
         "DeleteMultiRegionAccessPointRequest": DeleteMultiRegionAccessPointInputTypeDef,
         "PutMultiRegionAccessPointPolicyRequest": PutMultiRegionAccessPointPolicyInputTypeDef,
     },
     total=False,
 )
 
+CreateMultiRegionAccessPointInputUnionTypeDef = Union[
+    CreateMultiRegionAccessPointInputTypeDef, CreateMultiRegionAccessPointInputOutputTypeDef
+]
 CreateMultiRegionAccessPointRequestRequestTypeDef = TypedDict(
     "CreateMultiRegionAccessPointRequestRequestTypeDef",
     {
         "AccountId": str,
         "ClientToken": str,
         "Details": CreateMultiRegionAccessPointInputTypeDef,
     },
@@ -2427,14 +2418,36 @@
 
 class S3ManifestOutputLocationTypeDef(
     _RequiredS3ManifestOutputLocationTypeDef, _OptionalS3ManifestOutputLocationTypeDef
 ):
     pass
 
 
+_RequiredS3SetObjectRetentionOperationTypeDef = TypedDict(
+    "_RequiredS3SetObjectRetentionOperationTypeDef",
+    {
+        "Retention": S3RetentionTypeDef,
+    },
+)
+_OptionalS3SetObjectRetentionOperationTypeDef = TypedDict(
+    "_OptionalS3SetObjectRetentionOperationTypeDef",
+    {
+        "BypassGovernanceRetention": bool,
+    },
+    total=False,
+)
+
+
+class S3SetObjectRetentionOperationTypeDef(
+    _RequiredS3SetObjectRetentionOperationTypeDef, _OptionalS3SetObjectRetentionOperationTypeDef
+):
+    pass
+
+
+JobManifestUnionTypeDef = Union[JobManifestTypeDef, JobManifestOutputTypeDef]
 JobListDescriptorTypeDef = TypedDict(
     "JobListDescriptorTypeDef",
     {
         "JobId": str,
         "Description": str,
         "Operation": OperationNameType,
         "Priority": int,
@@ -2581,26 +2594,26 @@
 S3CopyObjectOperationTypeDef = TypedDict(
     "S3CopyObjectOperationTypeDef",
     {
         "TargetResource": str,
         "CannedAccessControlList": S3CannedAccessControlListType,
         "AccessControlGrants": Sequence[S3GrantTypeDef],
         "MetadataDirective": S3MetadataDirectiveType,
-        "ModifiedSinceConstraint": Union[datetime, str],
+        "ModifiedSinceConstraint": TimestampTypeDef,
         "NewObjectMetadata": S3ObjectMetadataTypeDef,
         "NewObjectTagging": Sequence[S3TagTypeDef],
         "RedirectLocation": str,
         "RequesterPays": bool,
         "StorageClass": S3StorageClassType,
-        "UnModifiedSinceConstraint": Union[datetime, str],
+        "UnModifiedSinceConstraint": TimestampTypeDef,
         "SSEAwsKmsKeyId": str,
         "TargetKeyPrefix": str,
         "ObjectLockLegalHoldStatus": S3ObjectLockLegalHoldStatusType,
         "ObjectLockMode": S3ObjectLockModeType,
-        "ObjectLockRetainUntilDate": Union[datetime, str],
+        "ObjectLockRetainUntilDate": TimestampTypeDef,
         "BucketKeyEnabled": bool,
         "ChecksumAlgorithm": S3ChecksumAlgorithmType,
     },
     total=False,
 )
 
 _RequiredS3BucketDestinationOutputTypeDef = TypedDict(
@@ -2938,14 +2951,17 @@
     {
         "AccountId": str,
         "Name": str,
         "Configuration": ObjectLambdaConfigurationTypeDef,
     },
 )
 
+ObjectLambdaConfigurationUnionTypeDef = Union[
+    ObjectLambdaConfigurationTypeDef, ObjectLambdaConfigurationOutputTypeDef
+]
 PutAccessPointConfigurationForObjectLambdaRequestRequestTypeDef = TypedDict(
     "PutAccessPointConfigurationForObjectLambdaRequestRequestTypeDef",
     {
         "AccountId": str,
         "Name": str,
         "Configuration": ObjectLambdaConfigurationTypeDef,
     },
@@ -3064,14 +3080,17 @@
 class PutBucketLifecycleConfigurationRequestRequestTypeDef(
     _RequiredPutBucketLifecycleConfigurationRequestRequestTypeDef,
     _OptionalPutBucketLifecycleConfigurationRequestRequestTypeDef,
 ):
     pass
 
 
+JobManifestGeneratorUnionTypeDef = Union[
+    JobManifestGeneratorTypeDef, JobManifestGeneratorOutputTypeDef
+]
 GetBucketReplicationResultTypeDef = TypedDict(
     "GetBucketReplicationResultTypeDef",
     {
         "ReplicationConfiguration": ReplicationConfigurationOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -3081,14 +3100,17 @@
     {
         "AccountId": str,
         "Bucket": str,
         "ReplicationConfiguration": ReplicationConfigurationTypeDef,
     },
 )
 
+ReplicationConfigurationUnionTypeDef = Union[
+    ReplicationConfigurationTypeDef, ReplicationConfigurationOutputTypeDef
+]
 _RequiredStorageLensConfigurationOutputTypeDef = TypedDict(
     "_RequiredStorageLensConfigurationOutputTypeDef",
     {
         "Id": str,
         "AccountLevel": AccountLevelTypeDef,
         "IsEnabled": bool,
     },
@@ -3199,14 +3221,17 @@
 class PutStorageLensConfigurationRequestRequestTypeDef(
     _RequiredPutStorageLensConfigurationRequestRequestTypeDef,
     _OptionalPutStorageLensConfigurationRequestRequestTypeDef,
 ):
     pass
 
 
+StorageLensConfigurationUnionTypeDef = Union[
+    StorageLensConfigurationTypeDef, StorageLensConfigurationOutputTypeDef
+]
 JobDescriptorTypeDef = TypedDict(
     "JobDescriptorTypeDef",
     {
         "JobId": str,
         "ConfirmationRequired": bool,
         "Description": str,
         "JobArn": str,
@@ -3255,14 +3280,15 @@
 
 class CreateJobRequestRequestTypeDef(
     _RequiredCreateJobRequestRequestTypeDef, _OptionalCreateJobRequestRequestTypeDef
 ):
     pass
 
 
+JobOperationUnionTypeDef = Union[JobOperationTypeDef, JobOperationOutputTypeDef]
 DescribeJobResultTypeDef = TypedDict(
     "DescribeJobResultTypeDef",
     {
         "Job": JobDescriptorTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-s3control-1.28.15.post1/mypy_boto3_s3control/type_defs.pyi` & `mypy-boto3-s3control-1.28.16/mypy_boto3_s3control/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_s3control.type_defs import AbortIncompleteMultipartUploadTypeDef
 
-    data: AbortIncompleteMultipartUploadTypeDef = {...}
+    data: AbortIncompleteMultipartUploadTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -133,27 +133,25 @@
     "GetStorageLensConfigurationRequestRequestTypeDef",
     "GetStorageLensConfigurationTaggingRequestRequestTypeDef",
     "StorageLensTagTypeDef",
     "IncludeOutputTypeDef",
     "IncludeTypeDef",
     "JobFailureTypeDef",
     "JobManifestGeneratorFilterOutputTypeDef",
-    "JobManifestGeneratorFilterTypeDef",
+    "TimestampTypeDef",
     "JobManifestLocationTypeDef",
     "JobManifestSpecOutputTypeDef",
     "JobManifestSpecTypeDef",
     "LambdaInvokeOperationTypeDef",
     "S3InitiateRestoreObjectOperationTypeDef",
     "JobTimersTypeDef",
     "LifecycleExpirationOutputTypeDef",
-    "LifecycleExpirationTypeDef",
     "NoncurrentVersionExpirationTypeDef",
     "NoncurrentVersionTransitionTypeDef",
     "TransitionOutputTypeDef",
-    "TransitionTypeDef",
     "PaginatorConfigTypeDef",
     "ListAccessPointsForObjectLambdaRequestRequestTypeDef",
     "ListAccessPointsRequestRequestTypeDef",
     "ListJobsRequestRequestTypeDef",
     "ListMultiRegionAccessPointsRequestRequestTypeDef",
     "ListRegionalBucketsRequestRequestTypeDef",
     "RegionalBucketTypeDef",
@@ -167,19 +165,17 @@
     "PutAccessPointPolicyForObjectLambdaRequestRequestTypeDef",
     "PutAccessPointPolicyRequestRequestTypeDef",
     "PutBucketPolicyRequestRequestTypeDef",
     "VersioningConfigurationTypeDef",
     "ReplicaModificationsTypeDef",
     "S3ObjectOwnerTypeDef",
     "S3ObjectMetadataOutputTypeDef",
-    "S3ObjectMetadataTypeDef",
     "S3GranteeTypeDef",
     "S3ObjectLockLegalHoldTypeDef",
     "S3RetentionOutputTypeDef",
-    "S3RetentionTypeDef",
     "SSEKMSTypeDef",
     "SseKmsEncryptedObjectsTypeDef",
     "StorageLensAwsOrgTypeDef",
     "UpdateJobPriorityRequestRequestTypeDef",
     "UpdateJobStatusRequestRequestTypeDef",
     "AccessPointTypeDef",
     "DeleteMultiRegionAccessPointRequestRequestTypeDef",
@@ -224,14 +220,19 @@
     "GetAccessPointPolicyStatusForObjectLambdaResultTypeDef",
     "GetAccessPointPolicyStatusResultTypeDef",
     "GetMultiRegionAccessPointPolicyStatusResultTypeDef",
     "GetMultiRegionAccessPointRoutesResultTypeDef",
     "SubmitMultiRegionAccessPointRoutesRequestRequestTypeDef",
     "GetStorageLensConfigurationTaggingResultTypeDef",
     "PutStorageLensConfigurationTaggingRequestRequestTypeDef",
+    "JobManifestGeneratorFilterTypeDef",
+    "LifecycleExpirationTypeDef",
+    "S3ObjectMetadataTypeDef",
+    "S3RetentionTypeDef",
+    "TransitionTypeDef",
     "S3GeneratedManifestDescriptorTypeDef",
     "JobManifestOutputTypeDef",
     "JobManifestTypeDef",
     "JobProgressSummaryTypeDef",
     "ListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef",
     "ListRegionalBucketsResultTypeDef",
     "ListStorageLensConfigurationsResultTypeDef",
@@ -241,31 +242,33 @@
     "MultiRegionAccessPointsAsyncResponseTypeDef",
     "MultiRegionAccessPointReportTypeDef",
     "PrefixLevelStorageMetricsTypeDef",
     "PutBucketVersioningRequestRequestTypeDef",
     "S3GrantTypeDef",
     "S3SetObjectLegalHoldOperationTypeDef",
     "S3SetObjectRetentionOperationOutputTypeDef",
-    "S3SetObjectRetentionOperationTypeDef",
     "StorageLensDataExportEncryptionOutputTypeDef",
     "StorageLensDataExportEncryptionTypeDef",
     "SourceSelectionCriteriaTypeDef",
     "ListAccessPointsResultTypeDef",
     "ObjectLambdaTransformationConfigurationOutputTypeDef",
     "ObjectLambdaTransformationConfigurationTypeDef",
     "ListAccessPointsForObjectLambdaResultTypeDef",
     "LifecycleRuleFilterOutputTypeDef",
     "LifecycleRuleFilterTypeDef",
     "ReplicationRuleFilterOutputTypeDef",
     "ReplicationRuleFilterTypeDef",
     "PutBucketTaggingRequestRequestTypeDef",
     "AsyncRequestParametersTypeDef",
+    "CreateMultiRegionAccessPointInputUnionTypeDef",
     "CreateMultiRegionAccessPointRequestRequestTypeDef",
     "S3ManifestOutputLocationOutputTypeDef",
     "S3ManifestOutputLocationTypeDef",
+    "S3SetObjectRetentionOperationTypeDef",
+    "JobManifestUnionTypeDef",
     "JobListDescriptorTypeDef",
     "DestinationTypeDef",
     "GetMultiRegionAccessPointPolicyResultTypeDef",
     "AsyncResponseDetailsTypeDef",
     "GetMultiRegionAccessPointResultTypeDef",
     "ListMultiRegionAccessPointsResultTypeDef",
     "PrefixLevelTypeDef",
@@ -288,36 +291,41 @@
     "BucketLevelTypeDef",
     "S3AccessControlPolicyOutputTypeDef",
     "S3AccessControlPolicyTypeDef",
     "StorageLensDataExportOutputTypeDef",
     "StorageLensDataExportTypeDef",
     "GetAccessPointConfigurationForObjectLambdaResultTypeDef",
     "CreateAccessPointForObjectLambdaRequestRequestTypeDef",
+    "ObjectLambdaConfigurationUnionTypeDef",
     "PutAccessPointConfigurationForObjectLambdaRequestRequestTypeDef",
     "GetBucketLifecycleConfigurationResultTypeDef",
     "LifecycleConfigurationTypeDef",
     "JobManifestGeneratorOutputTypeDef",
     "JobManifestGeneratorTypeDef",
     "ReplicationConfigurationOutputTypeDef",
     "ReplicationConfigurationTypeDef",
     "DescribeMultiRegionAccessPointOperationResultTypeDef",
     "AccountLevelTypeDef",
     "S3SetObjectAclOperationOutputTypeDef",
     "S3SetObjectAclOperationTypeDef",
     "PutBucketLifecycleConfigurationRequestRequestTypeDef",
+    "JobManifestGeneratorUnionTypeDef",
     "GetBucketReplicationResultTypeDef",
     "PutBucketReplicationRequestRequestTypeDef",
+    "ReplicationConfigurationUnionTypeDef",
     "StorageLensConfigurationOutputTypeDef",
     "StorageLensConfigurationTypeDef",
     "JobOperationOutputTypeDef",
     "JobOperationTypeDef",
     "GetStorageLensConfigurationResultTypeDef",
     "PutStorageLensConfigurationRequestRequestTypeDef",
+    "StorageLensConfigurationUnionTypeDef",
     "JobDescriptorTypeDef",
     "CreateJobRequestRequestTypeDef",
+    "JobOperationUnionTypeDef",
     "DescribeJobResultTypeDef",
 )
 
 AbortIncompleteMultipartUploadTypeDef = TypedDict(
     "AbortIncompleteMultipartUploadTypeDef",
     {
         "DaysAfterInitiation": int,
@@ -918,25 +926,15 @@
         "CreatedAfter": datetime,
         "CreatedBefore": datetime,
         "ObjectReplicationStatuses": List[ReplicationStatusType],
     },
     total=False,
 )
 
-JobManifestGeneratorFilterTypeDef = TypedDict(
-    "JobManifestGeneratorFilterTypeDef",
-    {
-        "EligibleForReplication": bool,
-        "CreatedAfter": Union[datetime, str],
-        "CreatedBefore": Union[datetime, str],
-        "ObjectReplicationStatuses": Sequence[ReplicationStatusType],
-    },
-    total=False,
-)
-
+TimestampTypeDef = Union[datetime, str]
 _RequiredJobManifestLocationTypeDef = TypedDict(
     "_RequiredJobManifestLocationTypeDef",
     {
         "ObjectArn": str,
         "ETag": str,
     },
 )
@@ -1020,24 +1018,14 @@
         "Date": datetime,
         "Days": int,
         "ExpiredObjectDeleteMarker": bool,
     },
     total=False,
 )
 
-LifecycleExpirationTypeDef = TypedDict(
-    "LifecycleExpirationTypeDef",
-    {
-        "Date": Union[datetime, str],
-        "Days": int,
-        "ExpiredObjectDeleteMarker": bool,
-    },
-    total=False,
-)
-
 NoncurrentVersionExpirationTypeDef = TypedDict(
     "NoncurrentVersionExpirationTypeDef",
     {
         "NoncurrentDays": int,
         "NewerNoncurrentVersions": int,
     },
     total=False,
@@ -1058,24 +1046,14 @@
         "Date": datetime,
         "Days": int,
         "StorageClass": TransitionStorageClassType,
     },
     total=False,
 )
 
-TransitionTypeDef = TypedDict(
-    "TransitionTypeDef",
-    {
-        "Date": Union[datetime, str],
-        "Days": int,
-        "StorageClass": TransitionStorageClassType,
-    },
-    total=False,
-)
-
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
@@ -1373,32 +1351,14 @@
         "HttpExpiresDate": datetime,
         "RequesterCharged": bool,
         "SSEAlgorithm": S3SSEAlgorithmType,
     },
     total=False,
 )
 
-S3ObjectMetadataTypeDef = TypedDict(
-    "S3ObjectMetadataTypeDef",
-    {
-        "CacheControl": str,
-        "ContentDisposition": str,
-        "ContentEncoding": str,
-        "ContentLanguage": str,
-        "UserMetadata": Mapping[str, str],
-        "ContentLength": int,
-        "ContentMD5": str,
-        "ContentType": str,
-        "HttpExpiresDate": Union[datetime, str],
-        "RequesterCharged": bool,
-        "SSEAlgorithm": S3SSEAlgorithmType,
-    },
-    total=False,
-)
-
 S3GranteeTypeDef = TypedDict(
     "S3GranteeTypeDef",
     {
         "TypeIdentifier": S3GranteeTypeIdentifierType,
         "Identifier": str,
         "DisplayName": str,
     },
@@ -1417,23 +1377,14 @@
     {
         "RetainUntilDate": datetime,
         "Mode": S3ObjectLockRetentionModeType,
     },
     total=False,
 )
 
-S3RetentionTypeDef = TypedDict(
-    "S3RetentionTypeDef",
-    {
-        "RetainUntilDate": Union[datetime, str],
-        "Mode": S3ObjectLockRetentionModeType,
-    },
-    total=False,
-)
-
 SSEKMSTypeDef = TypedDict(
     "SSEKMSTypeDef",
     {
         "KeyId": str,
     },
 )
 
@@ -1974,14 +1925,72 @@
     {
         "ConfigId": str,
         "AccountId": str,
         "Tags": Sequence[StorageLensTagTypeDef],
     },
 )
 
+JobManifestGeneratorFilterTypeDef = TypedDict(
+    "JobManifestGeneratorFilterTypeDef",
+    {
+        "EligibleForReplication": bool,
+        "CreatedAfter": TimestampTypeDef,
+        "CreatedBefore": TimestampTypeDef,
+        "ObjectReplicationStatuses": Sequence[ReplicationStatusType],
+    },
+    total=False,
+)
+
+LifecycleExpirationTypeDef = TypedDict(
+    "LifecycleExpirationTypeDef",
+    {
+        "Date": TimestampTypeDef,
+        "Days": int,
+        "ExpiredObjectDeleteMarker": bool,
+    },
+    total=False,
+)
+
+S3ObjectMetadataTypeDef = TypedDict(
+    "S3ObjectMetadataTypeDef",
+    {
+        "CacheControl": str,
+        "ContentDisposition": str,
+        "ContentEncoding": str,
+        "ContentLanguage": str,
+        "UserMetadata": Mapping[str, str],
+        "ContentLength": int,
+        "ContentMD5": str,
+        "ContentType": str,
+        "HttpExpiresDate": TimestampTypeDef,
+        "RequesterCharged": bool,
+        "SSEAlgorithm": S3SSEAlgorithmType,
+    },
+    total=False,
+)
+
+S3RetentionTypeDef = TypedDict(
+    "S3RetentionTypeDef",
+    {
+        "RetainUntilDate": TimestampTypeDef,
+        "Mode": S3ObjectLockRetentionModeType,
+    },
+    total=False,
+)
+
+TransitionTypeDef = TypedDict(
+    "TransitionTypeDef",
+    {
+        "Date": TimestampTypeDef,
+        "Days": int,
+        "StorageClass": TransitionStorageClassType,
+    },
+    total=False,
+)
+
 S3GeneratedManifestDescriptorTypeDef = TypedDict(
     "S3GeneratedManifestDescriptorTypeDef",
     {
         "Format": Literal["S3InventoryReport_CSV_20211130"],
         "Location": JobManifestLocationTypeDef,
     },
     total=False,
@@ -2170,33 +2179,14 @@
 
 class S3SetObjectRetentionOperationOutputTypeDef(
     _RequiredS3SetObjectRetentionOperationOutputTypeDef,
     _OptionalS3SetObjectRetentionOperationOutputTypeDef,
 ):
     pass
 
-_RequiredS3SetObjectRetentionOperationTypeDef = TypedDict(
-    "_RequiredS3SetObjectRetentionOperationTypeDef",
-    {
-        "Retention": S3RetentionTypeDef,
-    },
-)
-_OptionalS3SetObjectRetentionOperationTypeDef = TypedDict(
-    "_OptionalS3SetObjectRetentionOperationTypeDef",
-    {
-        "BypassGovernanceRetention": bool,
-    },
-    total=False,
-)
-
-class S3SetObjectRetentionOperationTypeDef(
-    _RequiredS3SetObjectRetentionOperationTypeDef, _OptionalS3SetObjectRetentionOperationTypeDef
-):
-    pass
-
 StorageLensDataExportEncryptionOutputTypeDef = TypedDict(
     "StorageLensDataExportEncryptionOutputTypeDef",
     {
         "SSES3": Dict[str, Any],
         "SSEKMS": SSEKMSTypeDef,
     },
     total=False,
@@ -2313,14 +2303,17 @@
         "CreateMultiRegionAccessPointRequest": CreateMultiRegionAccessPointInputOutputTypeDef,
         "DeleteMultiRegionAccessPointRequest": DeleteMultiRegionAccessPointInputTypeDef,
         "PutMultiRegionAccessPointPolicyRequest": PutMultiRegionAccessPointPolicyInputTypeDef,
     },
     total=False,
 )
 
+CreateMultiRegionAccessPointInputUnionTypeDef = Union[
+    CreateMultiRegionAccessPointInputTypeDef, CreateMultiRegionAccessPointInputOutputTypeDef
+]
 CreateMultiRegionAccessPointRequestRequestTypeDef = TypedDict(
     "CreateMultiRegionAccessPointRequestRequestTypeDef",
     {
         "AccountId": str,
         "ClientToken": str,
         "Details": CreateMultiRegionAccessPointInputTypeDef,
     },
@@ -2366,14 +2359,34 @@
 )
 
 class S3ManifestOutputLocationTypeDef(
     _RequiredS3ManifestOutputLocationTypeDef, _OptionalS3ManifestOutputLocationTypeDef
 ):
     pass
 
+_RequiredS3SetObjectRetentionOperationTypeDef = TypedDict(
+    "_RequiredS3SetObjectRetentionOperationTypeDef",
+    {
+        "Retention": S3RetentionTypeDef,
+    },
+)
+_OptionalS3SetObjectRetentionOperationTypeDef = TypedDict(
+    "_OptionalS3SetObjectRetentionOperationTypeDef",
+    {
+        "BypassGovernanceRetention": bool,
+    },
+    total=False,
+)
+
+class S3SetObjectRetentionOperationTypeDef(
+    _RequiredS3SetObjectRetentionOperationTypeDef, _OptionalS3SetObjectRetentionOperationTypeDef
+):
+    pass
+
+JobManifestUnionTypeDef = Union[JobManifestTypeDef, JobManifestOutputTypeDef]
 JobListDescriptorTypeDef = TypedDict(
     "JobListDescriptorTypeDef",
     {
         "JobId": str,
         "Description": str,
         "Operation": OperationNameType,
         "Priority": int,
@@ -2514,26 +2527,26 @@
 S3CopyObjectOperationTypeDef = TypedDict(
     "S3CopyObjectOperationTypeDef",
     {
         "TargetResource": str,
         "CannedAccessControlList": S3CannedAccessControlListType,
         "AccessControlGrants": Sequence[S3GrantTypeDef],
         "MetadataDirective": S3MetadataDirectiveType,
-        "ModifiedSinceConstraint": Union[datetime, str],
+        "ModifiedSinceConstraint": TimestampTypeDef,
         "NewObjectMetadata": S3ObjectMetadataTypeDef,
         "NewObjectTagging": Sequence[S3TagTypeDef],
         "RedirectLocation": str,
         "RequesterPays": bool,
         "StorageClass": S3StorageClassType,
-        "UnModifiedSinceConstraint": Union[datetime, str],
+        "UnModifiedSinceConstraint": TimestampTypeDef,
         "SSEAwsKmsKeyId": str,
         "TargetKeyPrefix": str,
         "ObjectLockLegalHoldStatus": S3ObjectLockLegalHoldStatusType,
         "ObjectLockMode": S3ObjectLockModeType,
-        "ObjectLockRetainUntilDate": Union[datetime, str],
+        "ObjectLockRetainUntilDate": TimestampTypeDef,
         "BucketKeyEnabled": bool,
         "ChecksumAlgorithm": S3ChecksumAlgorithmType,
     },
     total=False,
 )
 
 _RequiredS3BucketDestinationOutputTypeDef = TypedDict(
@@ -2851,14 +2864,17 @@
     {
         "AccountId": str,
         "Name": str,
         "Configuration": ObjectLambdaConfigurationTypeDef,
     },
 )
 
+ObjectLambdaConfigurationUnionTypeDef = Union[
+    ObjectLambdaConfigurationTypeDef, ObjectLambdaConfigurationOutputTypeDef
+]
 PutAccessPointConfigurationForObjectLambdaRequestRequestTypeDef = TypedDict(
     "PutAccessPointConfigurationForObjectLambdaRequestRequestTypeDef",
     {
         "AccountId": str,
         "Name": str,
         "Configuration": ObjectLambdaConfigurationTypeDef,
     },
@@ -2973,14 +2989,17 @@
 
 class PutBucketLifecycleConfigurationRequestRequestTypeDef(
     _RequiredPutBucketLifecycleConfigurationRequestRequestTypeDef,
     _OptionalPutBucketLifecycleConfigurationRequestRequestTypeDef,
 ):
     pass
 
+JobManifestGeneratorUnionTypeDef = Union[
+    JobManifestGeneratorTypeDef, JobManifestGeneratorOutputTypeDef
+]
 GetBucketReplicationResultTypeDef = TypedDict(
     "GetBucketReplicationResultTypeDef",
     {
         "ReplicationConfiguration": ReplicationConfigurationOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2990,14 +3009,17 @@
     {
         "AccountId": str,
         "Bucket": str,
         "ReplicationConfiguration": ReplicationConfigurationTypeDef,
     },
 )
 
+ReplicationConfigurationUnionTypeDef = Union[
+    ReplicationConfigurationTypeDef, ReplicationConfigurationOutputTypeDef
+]
 _RequiredStorageLensConfigurationOutputTypeDef = TypedDict(
     "_RequiredStorageLensConfigurationOutputTypeDef",
     {
         "Id": str,
         "AccountLevel": AccountLevelTypeDef,
         "IsEnabled": bool,
     },
@@ -3102,14 +3124,17 @@
 
 class PutStorageLensConfigurationRequestRequestTypeDef(
     _RequiredPutStorageLensConfigurationRequestRequestTypeDef,
     _OptionalPutStorageLensConfigurationRequestRequestTypeDef,
 ):
     pass
 
+StorageLensConfigurationUnionTypeDef = Union[
+    StorageLensConfigurationTypeDef, StorageLensConfigurationOutputTypeDef
+]
 JobDescriptorTypeDef = TypedDict(
     "JobDescriptorTypeDef",
     {
         "JobId": str,
         "ConfirmationRequired": bool,
         "Description": str,
         "JobArn": str,
@@ -3156,14 +3181,15 @@
 )
 
 class CreateJobRequestRequestTypeDef(
     _RequiredCreateJobRequestRequestTypeDef, _OptionalCreateJobRequestRequestTypeDef
 ):
     pass
 
+JobOperationUnionTypeDef = Union[JobOperationTypeDef, JobOperationOutputTypeDef]
 DescribeJobResultTypeDef = TypedDict(
     "DescribeJobResultTypeDef",
     {
         "Job": JobDescriptorTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-s3control-1.28.15.post1/mypy_boto3_s3control.egg-info/PKG-INFO` & `mypy-boto3-s3control-1.28.16/mypy_boto3_s3control.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-s3control
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.S3Control 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.S3Control 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 s3control type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 s3control type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-s3control.svg?color=blue)](https://pypi.org/project/mypy-boto3-s3control)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-s3control)](https://pepy.tech/project/mypy-boto3-s3control)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.S3Control 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control)
+[boto3.S3Control 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control)
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
 [mypy-boto3-s3control docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/).
 
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
@@ -355,20 +355,20 @@
 )
 
 
 def check_value(value: AsyncOperationNameType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_s3control.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_s3control.type_defs import (
     AbortIncompleteMultipartUploadTypeDef,
     AccessControlTranslationTypeDef,
     VpcConfigurationTypeDef,
     ActivityMetricsTypeDef,
@@ -433,27 +433,25 @@
     GetStorageLensConfigurationRequestRequestTypeDef,
     GetStorageLensConfigurationTaggingRequestRequestTypeDef,
     StorageLensTagTypeDef,
     IncludeOutputTypeDef,
     IncludeTypeDef,
     JobFailureTypeDef,
     JobManifestGeneratorFilterOutputTypeDef,
-    JobManifestGeneratorFilterTypeDef,
+    TimestampTypeDef,
     JobManifestLocationTypeDef,
     JobManifestSpecOutputTypeDef,
     JobManifestSpecTypeDef,
     LambdaInvokeOperationTypeDef,
     S3InitiateRestoreObjectOperationTypeDef,
     JobTimersTypeDef,
     LifecycleExpirationOutputTypeDef,
-    LifecycleExpirationTypeDef,
     NoncurrentVersionExpirationTypeDef,
     NoncurrentVersionTransitionTypeDef,
     TransitionOutputTypeDef,
-    TransitionTypeDef,
     PaginatorConfigTypeDef,
     ListAccessPointsForObjectLambdaRequestRequestTypeDef,
     ListAccessPointsRequestRequestTypeDef,
     ListJobsRequestRequestTypeDef,
     ListMultiRegionAccessPointsRequestRequestTypeDef,
     ListRegionalBucketsRequestRequestTypeDef,
     RegionalBucketTypeDef,
@@ -467,19 +465,17 @@
     PutAccessPointPolicyForObjectLambdaRequestRequestTypeDef,
     PutAccessPointPolicyRequestRequestTypeDef,
     PutBucketPolicyRequestRequestTypeDef,
     VersioningConfigurationTypeDef,
     ReplicaModificationsTypeDef,
     S3ObjectOwnerTypeDef,
     S3ObjectMetadataOutputTypeDef,
-    S3ObjectMetadataTypeDef,
     S3GranteeTypeDef,
     S3ObjectLockLegalHoldTypeDef,
     S3RetentionOutputTypeDef,
-    S3RetentionTypeDef,
     SSEKMSTypeDef,
     SseKmsEncryptedObjectsTypeDef,
     StorageLensAwsOrgTypeDef,
     UpdateJobPriorityRequestRequestTypeDef,
     UpdateJobStatusRequestRequestTypeDef,
     AccessPointTypeDef,
     DeleteMultiRegionAccessPointRequestRequestTypeDef,
@@ -524,14 +520,19 @@
     GetAccessPointPolicyStatusForObjectLambdaResultTypeDef,
     GetAccessPointPolicyStatusResultTypeDef,
     GetMultiRegionAccessPointPolicyStatusResultTypeDef,
     GetMultiRegionAccessPointRoutesResultTypeDef,
     SubmitMultiRegionAccessPointRoutesRequestRequestTypeDef,
     GetStorageLensConfigurationTaggingResultTypeDef,
     PutStorageLensConfigurationTaggingRequestRequestTypeDef,
+    JobManifestGeneratorFilterTypeDef,
+    LifecycleExpirationTypeDef,
+    S3ObjectMetadataTypeDef,
+    S3RetentionTypeDef,
+    TransitionTypeDef,
     S3GeneratedManifestDescriptorTypeDef,
     JobManifestOutputTypeDef,
     JobManifestTypeDef,
     JobProgressSummaryTypeDef,
     ListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef,
     ListRegionalBucketsResultTypeDef,
     ListStorageLensConfigurationsResultTypeDef,
@@ -541,31 +542,33 @@
     MultiRegionAccessPointsAsyncResponseTypeDef,
     MultiRegionAccessPointReportTypeDef,
     PrefixLevelStorageMetricsTypeDef,
     PutBucketVersioningRequestRequestTypeDef,
     S3GrantTypeDef,
     S3SetObjectLegalHoldOperationTypeDef,
     S3SetObjectRetentionOperationOutputTypeDef,
-    S3SetObjectRetentionOperationTypeDef,
     StorageLensDataExportEncryptionOutputTypeDef,
     StorageLensDataExportEncryptionTypeDef,
     SourceSelectionCriteriaTypeDef,
     ListAccessPointsResultTypeDef,
     ObjectLambdaTransformationConfigurationOutputTypeDef,
     ObjectLambdaTransformationConfigurationTypeDef,
     ListAccessPointsForObjectLambdaResultTypeDef,
     LifecycleRuleFilterOutputTypeDef,
     LifecycleRuleFilterTypeDef,
     ReplicationRuleFilterOutputTypeDef,
     ReplicationRuleFilterTypeDef,
     PutBucketTaggingRequestRequestTypeDef,
     AsyncRequestParametersTypeDef,
+    CreateMultiRegionAccessPointInputUnionTypeDef,
     CreateMultiRegionAccessPointRequestRequestTypeDef,
     S3ManifestOutputLocationOutputTypeDef,
     S3ManifestOutputLocationTypeDef,
+    S3SetObjectRetentionOperationTypeDef,
+    JobManifestUnionTypeDef,
     JobListDescriptorTypeDef,
     DestinationTypeDef,
     GetMultiRegionAccessPointPolicyResultTypeDef,
     AsyncResponseDetailsTypeDef,
     GetMultiRegionAccessPointResultTypeDef,
     ListMultiRegionAccessPointsResultTypeDef,
     PrefixLevelTypeDef,
@@ -588,41 +591,46 @@
     BucketLevelTypeDef,
     S3AccessControlPolicyOutputTypeDef,
     S3AccessControlPolicyTypeDef,
     StorageLensDataExportOutputTypeDef,
     StorageLensDataExportTypeDef,
     GetAccessPointConfigurationForObjectLambdaResultTypeDef,
     CreateAccessPointForObjectLambdaRequestRequestTypeDef,
+    ObjectLambdaConfigurationUnionTypeDef,
     PutAccessPointConfigurationForObjectLambdaRequestRequestTypeDef,
     GetBucketLifecycleConfigurationResultTypeDef,
     LifecycleConfigurationTypeDef,
     JobManifestGeneratorOutputTypeDef,
     JobManifestGeneratorTypeDef,
     ReplicationConfigurationOutputTypeDef,
     ReplicationConfigurationTypeDef,
     DescribeMultiRegionAccessPointOperationResultTypeDef,
     AccountLevelTypeDef,
     S3SetObjectAclOperationOutputTypeDef,
     S3SetObjectAclOperationTypeDef,
     PutBucketLifecycleConfigurationRequestRequestTypeDef,
+    JobManifestGeneratorUnionTypeDef,
     GetBucketReplicationResultTypeDef,
     PutBucketReplicationRequestRequestTypeDef,
+    ReplicationConfigurationUnionTypeDef,
     StorageLensConfigurationOutputTypeDef,
     StorageLensConfigurationTypeDef,
     JobOperationOutputTypeDef,
     JobOperationTypeDef,
     GetStorageLensConfigurationResultTypeDef,
     PutStorageLensConfigurationRequestRequestTypeDef,
+    StorageLensConfigurationUnionTypeDef,
     JobDescriptorTypeDef,
     CreateJobRequestRequestTypeDef,
+    JobOperationUnionTypeDef,
     DescribeJobResultTypeDef,
 )
 
 
-def get_structure() -> AbortIncompleteMultipartUploadTypeDef:
+def get_value() -> AbortIncompleteMultipartUploadTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-s3control-1.28.15.post1/mypy_boto3_s3control.egg-info/SOURCES.txt` & `mypy-boto3-s3control-1.28.16/mypy_boto3_s3control.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3control-1.28.15.post1/setup.py` & `mypy-boto3-s3control-1.28.16/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-s3control",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_s3control"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.S3Control 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.2"
+        "Type annotations for boto3.S3Control 1.28.16 service generated with mypy-boto3-builder"
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
-    keywords="boto3 s3control type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 s3control type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_s3control": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

