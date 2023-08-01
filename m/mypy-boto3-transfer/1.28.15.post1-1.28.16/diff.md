# Comparing `tmp/mypy-boto3-transfer-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-transfer-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-transfer-1.28.15.post1.tar", last modified: Sat Jul 29 10:04:22 2023, max compression
+gzip compressed data, was "mypy-boto3-transfer-1.28.16.tar", last modified: Tue Aug  1 11:38:01 2023, max compression
```

## Comparing `mypy-boto3-transfer-1.28.15.post1.tar` & `mypy-boto3-transfer-1.28.16.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:22.825446 mypy-boto3-transfer-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 10:00:56.000000 mypy-boto3-transfer-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21979 2023-07-29 10:04:22.821445 mypy-boto3-transfer-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20482 2023-07-29 10:00:56.000000 mypy-boto3-transfer-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:22.813445 mypy-boto3-transfer-1.28.15.post1/mypy_boto3_transfer/
--rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-07-29 10:00:56.000000 mypy-boto3-transfer-1.28.15.post1/mypy_boto3_transfer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-07-29 10:00:56.000000 mypy-boto3-transfer-1.28.15.post1/mypy_boto3_transfer/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-29 10:00:56.000000 mypy-boto3-transfer-1.28.15.post1/mypy_boto3_transfer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47789 2023-07-29 10:00:57.000000 mypy-boto3-transfer-1.28.15.post1/mypy_boto3_transfer/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    47710 2023-07-29 10:00:56.000000 mypy-boto3-transfer-1.28.15.post1/mypy_boto3_transfer/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12273 2023-07-29 10:00:57.000000 mypy-boto3-transfer-1.28.15.post1/mypy_boto3_transfer/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12271 2023-07-29 10:00:57.000000 mypy-boto3-transfer-1.28.15.post1/mypy_boto3_transfer/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12188 2023-07-29 10:00:57.000000 mypy-boto3-transfer-1.28.15.post1/mypy_boto3_transfer/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12175 2023-07-29 10:00:57.000000 mypy-boto3-transfer-1.28.15.post1/mypy_boto3_transfer/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 10:00:56.000000 mypy-boto3-transfer-1.28.15.post1/mypy_boto3_transfer/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    62748 2023-07-29 10:01:03.000000 mypy-boto3-transfer-1.28.15.post1/mypy_boto3_transfer/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    62655 2023-07-29 10:00:58.000000 mypy-boto3-transfer-1.28.15.post1/mypy_boto3_transfer/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 10:00:56.000000 mypy-boto3-transfer-1.28.15.post1/mypy_boto3_transfer/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-07-29 10:00:57.000000 mypy-boto3-transfer-1.28.15.post1/mypy_boto3_transfer/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-07-29 10:00:57.000000 mypy-boto3-transfer-1.28.15.post1/mypy_boto3_transfer/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:22.821445 mypy-boto3-transfer-1.28.15.post1/mypy_boto3_transfer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21979 2023-07-29 10:04:22.000000 mypy-boto3-transfer-1.28.15.post1/mypy_boto3_transfer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-29 10:04:22.000000 mypy-boto3-transfer-1.28.15.post1/mypy_boto3_transfer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:22.000000 mypy-boto3-transfer-1.28.15.post1/mypy_boto3_transfer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:22.000000 mypy-boto3-transfer-1.28.15.post1/mypy_boto3_transfer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:04:22.000000 mypy-boto3-transfer-1.28.15.post1/mypy_boto3_transfer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-29 10:04:22.000000 mypy-boto3-transfer-1.28.15.post1/mypy_boto3_transfer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:04:22.825446 mypy-boto3-transfer-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-07-29 10:00:56.000000 mypy-boto3-transfer-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:38:01.836694 mypy-boto3-transfer-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:34:34.000000 mypy-boto3-transfer-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22187 2023-08-01 11:38:01.836694 mypy-boto3-transfer-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20699 2023-08-01 11:34:34.000000 mypy-boto3-transfer-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:38:01.836694 mypy-boto3-transfer-1.28.16/mypy_boto3_transfer/
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-08-01 11:34:34.000000 mypy-boto3-transfer-1.28.16/mypy_boto3_transfer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-08-01 11:34:34.000000 mypy-boto3-transfer-1.28.16/mypy_boto3_transfer/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-08-01 11:34:34.000000 mypy-boto3-transfer-1.28.16/mypy_boto3_transfer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47148 2023-08-01 11:34:35.000000 mypy-boto3-transfer-1.28.16/mypy_boto3_transfer/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47069 2023-08-01 11:34:34.000000 mypy-boto3-transfer-1.28.16/mypy_boto3_transfer/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12273 2023-08-01 11:34:40.000000 mypy-boto3-transfer-1.28.16/mypy_boto3_transfer/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12271 2023-08-01 11:34:35.000000 mypy-boto3-transfer-1.28.16/mypy_boto3_transfer/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12188 2023-08-01 11:34:35.000000 mypy-boto3-transfer-1.28.16/mypy_boto3_transfer/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12175 2023-08-01 11:34:35.000000 mypy-boto3-transfer-1.28.16/mypy_boto3_transfer/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:34:34.000000 mypy-boto3-transfer-1.28.16/mypy_boto3_transfer/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    63483 2023-08-01 11:34:41.000000 mypy-boto3-transfer-1.28.16/mypy_boto3_transfer/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63391 2023-08-01 11:34:40.000000 mypy-boto3-transfer-1.28.16/mypy_boto3_transfer/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:34:34.000000 mypy-boto3-transfer-1.28.16/mypy_boto3_transfer/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-08-01 11:34:35.000000 mypy-boto3-transfer-1.28.16/mypy_boto3_transfer/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-08-01 11:34:35.000000 mypy-boto3-transfer-1.28.16/mypy_boto3_transfer/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:38:01.836694 mypy-boto3-transfer-1.28.16/mypy_boto3_transfer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22187 2023-08-01 11:38:01.000000 mypy-boto3-transfer-1.28.16/mypy_boto3_transfer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-08-01 11:38:01.000000 mypy-boto3-transfer-1.28.16/mypy_boto3_transfer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:38:01.000000 mypy-boto3-transfer-1.28.16/mypy_boto3_transfer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:38:01.000000 mypy-boto3-transfer-1.28.16/mypy_boto3_transfer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:38:01.000000 mypy-boto3-transfer-1.28.16/mypy_boto3_transfer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-01 11:38:01.000000 mypy-boto3-transfer-1.28.16/mypy_boto3_transfer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:38:01.836694 mypy-boto3-transfer-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-08-01 11:34:34.000000 mypy-boto3-transfer-1.28.16/setup.py
```

### Comparing `mypy-boto3-transfer-1.28.15.post1/LICENSE` & `mypy-boto3-transfer-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transfer-1.28.15.post1/PKG-INFO` & `mypy-boto3-transfer-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-transfer
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.Transfer 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.Transfer 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 transfer type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 transfer type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-transfer.svg?color=blue)](https://pypi.org/project/mypy-boto3-transfer)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-transfer)](https://pepy.tech/project/mypy-boto3-transfer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Transfer 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer)
+[boto3.Transfer 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer)
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
 [mypy-boto3-transfer docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/).
 
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
@@ -395,20 +395,20 @@
 )
 
 
 def check_value(value: AgreementStatusTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_transfer.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_transfer.type_defs import (
     As2ConnectorConfigTypeDef,
     HomeDirectoryMapEntryTypeDef,
     PosixProfileTypeDef,
     ResponseMetadataTypeDef,
@@ -447,14 +447,15 @@
     LoggingConfigurationTypeDef,
     EndpointDetailsOutputTypeDef,
     ProtocolDetailsOutputTypeDef,
     SshPublicKeyTypeDef,
     EfsFileLocationTypeDef,
     ExecutionErrorTypeDef,
     S3FileLocationTypeDef,
+    TimestampTypeDef,
     ImportSshPublicKeyRequestRequestTypeDef,
     S3InputFileLocationTypeDef,
     PaginatorConfigTypeDef,
     ListAccessesRequestRequestTypeDef,
     ListedAccessTypeDef,
     ListAgreementsRequestRequestTypeDef,
     ListedAgreementTypeDef,
@@ -481,15 +482,14 @@
     StartFileTransferRequestRequestTypeDef,
     StartServerRequestRequestTypeDef,
     StopServerRequestRequestTypeDef,
     TestConnectionRequestRequestTypeDef,
     TestIdentityProviderRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAgreementRequestRequestTypeDef,
-    UpdateCertificateRequestRequestTypeDef,
     UpdateHostKeyRequestRequestTypeDef,
     UpdateProfileRequestRequestTypeDef,
     WorkflowDetailTypeDef,
     CreateAccessRequestRequestTypeDef,
     UpdateAccessRequestRequestTypeDef,
     UpdateUserRequestRequestTypeDef,
     CreateAccessResponseTypeDef,
@@ -518,28 +518,33 @@
     CreateAgreementRequestRequestTypeDef,
     CreateProfileRequestRequestTypeDef,
     CreateUserRequestRequestTypeDef,
     DescribedAgreementTypeDef,
     DescribedCertificateTypeDef,
     DescribedHostKeyTypeDef,
     DescribedProfileTypeDef,
-    ImportCertificateRequestRequestTypeDef,
     ImportHostKeyRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateConnectorRequestRequestTypeDef,
     UpdateConnectorRequestRequestTypeDef,
     DescribeSecurityPolicyResponseTypeDef,
     DescribeServerRequestServerOfflineWaitTypeDef,
     DescribeServerRequestServerOnlineWaitTypeDef,
     DescribedAccessTypeDef,
+    PosixProfileUnionTypeDef,
     DescribedConnectorTypeDef,
+    SftpConnectorConfigUnionTypeDef,
+    EndpointDetailsUnionTypeDef,
+    ProtocolDetailsUnionTypeDef,
     DescribedUserTypeDef,
     ExecutionStepResultTypeDef,
     FileLocationTypeDef,
+    ImportCertificateRequestRequestTypeDef,
+    UpdateCertificateRequestRequestTypeDef,
     InputFileLocationTypeDef,
     ListAccessesRequestListAccessesPaginateTypeDef,
     ListAgreementsRequestListAgreementsPaginateTypeDef,
     ListCertificatesRequestListCertificatesPaginateTypeDef,
     ListConnectorsRequestListConnectorsPaginateTypeDef,
     ListExecutionsRequestListExecutionsPaginateTypeDef,
     ListProfilesRequestListProfilesPaginateTypeDef,
@@ -572,27 +577,29 @@
     ExecutionResultsTypeDef,
     CopyStepDetailsTypeDef,
     DecryptStepDetailsTypeDef,
     ListedExecutionTypeDef,
     DescribedServerTypeDef,
     CreateServerRequestRequestTypeDef,
     UpdateServerRequestRequestTypeDef,
+    WorkflowDetailsUnionTypeDef,
     DescribedExecutionTypeDef,
     WorkflowStepOutputTypeDef,
     WorkflowStepTypeDef,
     ListExecutionsResponseTypeDef,
     DescribeServerResponseTypeDef,
     DescribeExecutionResponseTypeDef,
     DescribedWorkflowTypeDef,
-    CreateWorkflowRequestRequestTypeDef,
+    WorkflowStepUnionTypeDef,
     DescribeWorkflowResponseTypeDef,
+    CreateWorkflowRequestRequestTypeDef,
 )
 
 
-def get_structure() -> As2ConnectorConfigTypeDef:
+def get_value() -> As2ConnectorConfigTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-transfer-1.28.15.post1/README.md` & `mypy-boto3-transfer-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-transfer.svg?color=blue)](https://pypi.org/project/mypy-boto3-transfer)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-transfer)](https://pepy.tech/project/mypy-boto3-transfer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Transfer 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer)
+[boto3.Transfer 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer)
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
 [mypy-boto3-transfer docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/).
 
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
@@ -363,20 +363,20 @@
 )
 
 
 def check_value(value: AgreementStatusTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_transfer.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_transfer.type_defs import (
     As2ConnectorConfigTypeDef,
     HomeDirectoryMapEntryTypeDef,
     PosixProfileTypeDef,
     ResponseMetadataTypeDef,
@@ -415,14 +415,15 @@
     LoggingConfigurationTypeDef,
     EndpointDetailsOutputTypeDef,
     ProtocolDetailsOutputTypeDef,
     SshPublicKeyTypeDef,
     EfsFileLocationTypeDef,
     ExecutionErrorTypeDef,
     S3FileLocationTypeDef,
+    TimestampTypeDef,
     ImportSshPublicKeyRequestRequestTypeDef,
     S3InputFileLocationTypeDef,
     PaginatorConfigTypeDef,
     ListAccessesRequestRequestTypeDef,
     ListedAccessTypeDef,
     ListAgreementsRequestRequestTypeDef,
     ListedAgreementTypeDef,
@@ -449,15 +450,14 @@
     StartFileTransferRequestRequestTypeDef,
     StartServerRequestRequestTypeDef,
     StopServerRequestRequestTypeDef,
     TestConnectionRequestRequestTypeDef,
     TestIdentityProviderRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAgreementRequestRequestTypeDef,
-    UpdateCertificateRequestRequestTypeDef,
     UpdateHostKeyRequestRequestTypeDef,
     UpdateProfileRequestRequestTypeDef,
     WorkflowDetailTypeDef,
     CreateAccessRequestRequestTypeDef,
     UpdateAccessRequestRequestTypeDef,
     UpdateUserRequestRequestTypeDef,
     CreateAccessResponseTypeDef,
@@ -486,28 +486,33 @@
     CreateAgreementRequestRequestTypeDef,
     CreateProfileRequestRequestTypeDef,
     CreateUserRequestRequestTypeDef,
     DescribedAgreementTypeDef,
     DescribedCertificateTypeDef,
     DescribedHostKeyTypeDef,
     DescribedProfileTypeDef,
-    ImportCertificateRequestRequestTypeDef,
     ImportHostKeyRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateConnectorRequestRequestTypeDef,
     UpdateConnectorRequestRequestTypeDef,
     DescribeSecurityPolicyResponseTypeDef,
     DescribeServerRequestServerOfflineWaitTypeDef,
     DescribeServerRequestServerOnlineWaitTypeDef,
     DescribedAccessTypeDef,
+    PosixProfileUnionTypeDef,
     DescribedConnectorTypeDef,
+    SftpConnectorConfigUnionTypeDef,
+    EndpointDetailsUnionTypeDef,
+    ProtocolDetailsUnionTypeDef,
     DescribedUserTypeDef,
     ExecutionStepResultTypeDef,
     FileLocationTypeDef,
+    ImportCertificateRequestRequestTypeDef,
+    UpdateCertificateRequestRequestTypeDef,
     InputFileLocationTypeDef,
     ListAccessesRequestListAccessesPaginateTypeDef,
     ListAgreementsRequestListAgreementsPaginateTypeDef,
     ListCertificatesRequestListCertificatesPaginateTypeDef,
     ListConnectorsRequestListConnectorsPaginateTypeDef,
     ListExecutionsRequestListExecutionsPaginateTypeDef,
     ListProfilesRequestListProfilesPaginateTypeDef,
@@ -540,27 +545,29 @@
     ExecutionResultsTypeDef,
     CopyStepDetailsTypeDef,
     DecryptStepDetailsTypeDef,
     ListedExecutionTypeDef,
     DescribedServerTypeDef,
     CreateServerRequestRequestTypeDef,
     UpdateServerRequestRequestTypeDef,
+    WorkflowDetailsUnionTypeDef,
     DescribedExecutionTypeDef,
     WorkflowStepOutputTypeDef,
     WorkflowStepTypeDef,
     ListExecutionsResponseTypeDef,
     DescribeServerResponseTypeDef,
     DescribeExecutionResponseTypeDef,
     DescribedWorkflowTypeDef,
-    CreateWorkflowRequestRequestTypeDef,
+    WorkflowStepUnionTypeDef,
     DescribeWorkflowResponseTypeDef,
+    CreateWorkflowRequestRequestTypeDef,
 )
 
 
-def get_structure() -> As2ConnectorConfigTypeDef:
+def get_value() -> As2ConnectorConfigTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-transfer-1.28.15.post1/mypy_boto3_transfer/__init__.py` & `mypy-boto3-transfer-1.28.16/mypy_boto3_transfer/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transfer-1.28.15.post1/mypy_boto3_transfer/__init__.pyi` & `mypy-boto3-transfer-1.28.16/mypy_boto3_transfer/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transfer-1.28.15.post1/mypy_boto3_transfer/__main__.py` & `mypy-boto3-transfer-1.28.16/mypy_boto3_transfer/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Transfer 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.Transfer 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer\nOther"
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

### Comparing `mypy-boto3-transfer-1.28.15.post1/mypy_boto3_transfer/client.py` & `mypy-boto3-transfer-1.28.16/mypy_boto3_transfer/client.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from mypy_boto3_transfer.client import TransferClient
 
     session = Session()
     client: TransferClient = session.client("transfer")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AgreementStatusTypeType,
     CertificateUsageTypeType,
     CustomStepStatusType,
@@ -60,16 +59,15 @@
     DescribeHostKeyResponseTypeDef,
     DescribeProfileResponseTypeDef,
     DescribeSecurityPolicyResponseTypeDef,
     DescribeServerResponseTypeDef,
     DescribeUserResponseTypeDef,
     DescribeWorkflowResponseTypeDef,
     EmptyResponseMetadataTypeDef,
-    EndpointDetailsOutputTypeDef,
-    EndpointDetailsTypeDef,
+    EndpointDetailsUnionTypeDef,
     HomeDirectoryMapEntryTypeDef,
     IdentityProviderDetailsTypeDef,
     ImportCertificateResponseTypeDef,
     ImportHostKeyResponseTypeDef,
     ImportSshPublicKeyResponseTypeDef,
     ListAccessesResponseTypeDef,
     ListAgreementsResponseTypeDef,
@@ -79,69 +77,61 @@
     ListHostKeysResponseTypeDef,
     ListProfilesResponseTypeDef,
     ListSecurityPoliciesResponseTypeDef,
     ListServersResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListUsersResponseTypeDef,
     ListWorkflowsResponseTypeDef,
-    PosixProfileOutputTypeDef,
-    PosixProfileTypeDef,
-    ProtocolDetailsOutputTypeDef,
-    ProtocolDetailsTypeDef,
-    SftpConnectorConfigOutputTypeDef,
-    SftpConnectorConfigTypeDef,
+    PosixProfileUnionTypeDef,
+    ProtocolDetailsUnionTypeDef,
+    SftpConnectorConfigUnionTypeDef,
     StartFileTransferResponseTypeDef,
     TagTypeDef,
     TestConnectionResponseTypeDef,
     TestIdentityProviderResponseTypeDef,
+    TimestampTypeDef,
     UpdateAccessResponseTypeDef,
     UpdateAgreementResponseTypeDef,
     UpdateCertificateResponseTypeDef,
     UpdateConnectorResponseTypeDef,
     UpdateHostKeyResponseTypeDef,
     UpdateProfileResponseTypeDef,
     UpdateServerResponseTypeDef,
     UpdateUserResponseTypeDef,
-    WorkflowDetailsOutputTypeDef,
-    WorkflowDetailsTypeDef,
-    WorkflowStepOutputTypeDef,
-    WorkflowStepTypeDef,
+    WorkflowDetailsUnionTypeDef,
+    WorkflowStepUnionTypeDef,
 )
 from .waiter import ServerOfflineWaiter, ServerOnlineWaiter
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("TransferClient",)
 
-
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     InternalServiceError: Type[BotocoreClientError]
     InvalidNextTokenException: Type[BotocoreClientError]
     InvalidRequestException: Type[BotocoreClientError]
     ResourceExistsException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ServiceUnavailableException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
 
-
 class TransferClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/)
     """
 
     meta: ClientMeta
@@ -150,52 +140,48 @@
     def exceptions(self) -> Exceptions:
         """
         TransferClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#exceptions)
         """
-
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#can_paginate)
         """
-
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#close)
         """
-
     def create_access(
         self,
         *,
         Role: str,
         ServerId: str,
         ExternalId: str,
         HomeDirectory: str = ...,
         HomeDirectoryType: HomeDirectoryTypeType = ...,
         HomeDirectoryMappings: Sequence[HomeDirectoryMapEntryTypeDef] = ...,
         Policy: str = ...,
-        PosixProfile: Union[PosixProfileTypeDef, PosixProfileOutputTypeDef] = ...
+        PosixProfile: PosixProfileUnionTypeDef = ...
     ) -> CreateAccessResponseTypeDef:
         """
         Used by administrators to choose which groups in the directory should have
         access to upload and download files over the enabled protocols using Transfer
         Family.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.create_access)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#create_access)
         """
-
     def create_agreement(
         self,
         *,
         ServerId: str,
         LocalProfileId: str,
         PartnerProfileId: str,
         BaseDirectory: str,
@@ -206,499 +192,455 @@
     ) -> CreateAgreementResponseTypeDef:
         """
         Creates an agreement.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.create_agreement)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#create_agreement)
         """
-
     def create_connector(
         self,
         *,
         Url: str,
         AccessRole: str,
         As2Config: As2ConnectorConfigTypeDef = ...,
         LoggingRole: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        SftpConfig: Union[SftpConnectorConfigTypeDef, SftpConnectorConfigOutputTypeDef] = ...
+        SftpConfig: SftpConnectorConfigUnionTypeDef = ...
     ) -> CreateConnectorResponseTypeDef:
         """
         Creates the connector, which captures the parameters for an outbound connection
         for the AS2 or SFTP protocol.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.create_connector)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#create_connector)
         """
-
     def create_profile(
         self,
         *,
         As2Id: str,
         ProfileType: ProfileTypeType,
         CertificateIds: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateProfileResponseTypeDef:
         """
         Creates the local or partner profile to use for AS2 transfers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.create_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#create_profile)
         """
-
     def create_server(
         self,
         *,
         Certificate: str = ...,
         Domain: DomainType = ...,
-        EndpointDetails: Union[EndpointDetailsTypeDef, EndpointDetailsOutputTypeDef] = ...,
+        EndpointDetails: EndpointDetailsUnionTypeDef = ...,
         EndpointType: EndpointTypeType = ...,
         HostKey: str = ...,
         IdentityProviderDetails: IdentityProviderDetailsTypeDef = ...,
         IdentityProviderType: IdentityProviderTypeType = ...,
         LoggingRole: str = ...,
         PostAuthenticationLoginBanner: str = ...,
         PreAuthenticationLoginBanner: str = ...,
         Protocols: Sequence[ProtocolType] = ...,
-        ProtocolDetails: Union[ProtocolDetailsTypeDef, ProtocolDetailsOutputTypeDef] = ...,
+        ProtocolDetails: ProtocolDetailsUnionTypeDef = ...,
         SecurityPolicyName: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        WorkflowDetails: Union[WorkflowDetailsTypeDef, WorkflowDetailsOutputTypeDef] = ...,
+        WorkflowDetails: WorkflowDetailsUnionTypeDef = ...,
         StructuredLogDestinations: Sequence[str] = ...
     ) -> CreateServerResponseTypeDef:
         """
         Instantiates an auto-scaling virtual server based on the selected file transfer
         protocol in Amazon Web Services.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.create_server)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#create_server)
         """
-
     def create_user(
         self,
         *,
         Role: str,
         ServerId: str,
         UserName: str,
         HomeDirectory: str = ...,
         HomeDirectoryType: HomeDirectoryTypeType = ...,
         HomeDirectoryMappings: Sequence[HomeDirectoryMapEntryTypeDef] = ...,
         Policy: str = ...,
-        PosixProfile: Union[PosixProfileTypeDef, PosixProfileOutputTypeDef] = ...,
+        PosixProfile: PosixProfileUnionTypeDef = ...,
         SshPublicKeyBody: str = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateUserResponseTypeDef:
         """
         Creates a user and associates them with an existing file transfer protocol-
         enabled server.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.create_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#create_user)
         """
-
     def create_workflow(
         self,
         *,
-        Steps: Sequence[Union[WorkflowStepTypeDef, WorkflowStepOutputTypeDef]],
+        Steps: Sequence[WorkflowStepUnionTypeDef],
         Description: str = ...,
-        OnExceptionSteps: Sequence[Union[WorkflowStepTypeDef, WorkflowStepOutputTypeDef]] = ...,
+        OnExceptionSteps: Sequence[WorkflowStepUnionTypeDef] = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateWorkflowResponseTypeDef:
         """
         Allows you to create a workflow with specified steps and step details the
         workflow invokes after file transfer completes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.create_workflow)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#create_workflow)
         """
-
     def delete_access(self, *, ServerId: str, ExternalId: str) -> EmptyResponseMetadataTypeDef:
         """
         Allows you to delete the access specified in the `ServerID` and `ExternalID`
         parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.delete_access)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#delete_access)
         """
-
     def delete_agreement(self, *, AgreementId: str, ServerId: str) -> EmptyResponseMetadataTypeDef:
         """
         Delete the agreement that's specified in the provided `AgreementId`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.delete_agreement)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#delete_agreement)
         """
-
     def delete_certificate(self, *, CertificateId: str) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the certificate that's specified in the `CertificateId` parameter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.delete_certificate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#delete_certificate)
         """
-
     def delete_connector(self, *, ConnectorId: str) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the connector that's specified in the provided `ConnectorId`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.delete_connector)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#delete_connector)
         """
-
     def delete_host_key(self, *, ServerId: str, HostKeyId: str) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the host key that's specified in the `HostKeyId` parameter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.delete_host_key)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#delete_host_key)
         """
-
     def delete_profile(self, *, ProfileId: str) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the profile that's specified in the `ProfileId` parameter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.delete_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#delete_profile)
         """
-
     def delete_server(self, *, ServerId: str) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the file transfer protocol-enabled server that you specify.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.delete_server)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#delete_server)
         """
-
     def delete_ssh_public_key(
         self, *, ServerId: str, SshPublicKeyId: str, UserName: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes a user's Secure Shell (SSH) public key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.delete_ssh_public_key)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#delete_ssh_public_key)
         """
-
     def delete_user(self, *, ServerId: str, UserName: str) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the user belonging to a file transfer protocol-enabled server you
         specify.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.delete_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#delete_user)
         """
-
     def delete_workflow(self, *, WorkflowId: str) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the specified workflow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.delete_workflow)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#delete_workflow)
         """
-
     def describe_access(self, *, ServerId: str, ExternalId: str) -> DescribeAccessResponseTypeDef:
         """
         Describes the access that is assigned to the specific file transfer protocol-
         enabled server, as identified by its `ServerId` property and its `ExternalId`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.describe_access)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#describe_access)
         """
-
     def describe_agreement(
         self, *, AgreementId: str, ServerId: str
     ) -> DescribeAgreementResponseTypeDef:
         """
         Describes the agreement that's identified by the `AgreementId`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.describe_agreement)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#describe_agreement)
         """
-
     def describe_certificate(self, *, CertificateId: str) -> DescribeCertificateResponseTypeDef:
         """
         Describes the certificate that's identified by the `CertificateId`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.describe_certificate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#describe_certificate)
         """
-
     def describe_connector(self, *, ConnectorId: str) -> DescribeConnectorResponseTypeDef:
         """
         Describes the connector that's identified by the `ConnectorId.` See also: [AWS
         API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/transfer-2018-11-05/DescribeConnector).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.describe_connector)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#describe_connector)
         """
-
     def describe_execution(
         self, *, ExecutionId: str, WorkflowId: str
     ) -> DescribeExecutionResponseTypeDef:
         """
         You can use `DescribeExecution` to check the details of the execution of the
         specified workflow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.describe_execution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#describe_execution)
         """
-
     def describe_host_key(self, *, ServerId: str, HostKeyId: str) -> DescribeHostKeyResponseTypeDef:
         """
         Returns the details of the host key that's specified by the `HostKeyId` and
         `ServerId`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.describe_host_key)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#describe_host_key)
         """
-
     def describe_profile(self, *, ProfileId: str) -> DescribeProfileResponseTypeDef:
         """
         Returns the details of the profile that's specified by the `ProfileId`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.describe_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#describe_profile)
         """
-
     def describe_security_policy(
         self, *, SecurityPolicyName: str
     ) -> DescribeSecurityPolicyResponseTypeDef:
         """
         Describes the security policy that is attached to your file transfer protocol-
         enabled server.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.describe_security_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#describe_security_policy)
         """
-
     def describe_server(self, *, ServerId: str) -> DescribeServerResponseTypeDef:
         """
         Describes a file transfer protocol-enabled server that you specify by passing
         the `ServerId` parameter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.describe_server)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#describe_server)
         """
-
     def describe_user(self, *, ServerId: str, UserName: str) -> DescribeUserResponseTypeDef:
         """
         Describes the user assigned to the specific file transfer protocol-enabled
         server, as identified by its `ServerId` property.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.describe_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#describe_user)
         """
-
     def describe_workflow(self, *, WorkflowId: str) -> DescribeWorkflowResponseTypeDef:
         """
         Describes the specified workflow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.describe_workflow)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#describe_workflow)
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
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#generate_presigned_url)
         """
-
     def import_certificate(
         self,
         *,
         Usage: CertificateUsageTypeType,
         Certificate: str,
         CertificateChain: str = ...,
         PrivateKey: str = ...,
-        ActiveDate: Union[datetime, str] = ...,
-        InactiveDate: Union[datetime, str] = ...,
+        ActiveDate: TimestampTypeDef = ...,
+        InactiveDate: TimestampTypeDef = ...,
         Description: str = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> ImportCertificateResponseTypeDef:
         """
         Imports the signing and encryption certificates that you need to create local
         (AS2) profiles and partner profiles.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.import_certificate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#import_certificate)
         """
-
     def import_host_key(
         self,
         *,
         ServerId: str,
         HostKeyBody: str,
         Description: str = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> ImportHostKeyResponseTypeDef:
         """
         Adds a host key to the server that's specified by the `ServerId` parameter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.import_host_key)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#import_host_key)
         """
-
     def import_ssh_public_key(
         self, *, ServerId: str, SshPublicKeyBody: str, UserName: str
     ) -> ImportSshPublicKeyResponseTypeDef:
         """
         Adds a Secure Shell (SSH) public key to a Transfer Family user identified by a
         `UserName` value assigned to the specific file transfer protocol-enabled server,
         identified by `ServerId`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.import_ssh_public_key)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#import_ssh_public_key)
         """
-
     def list_accesses(
         self, *, ServerId: str, MaxResults: int = ..., NextToken: str = ...
     ) -> ListAccessesResponseTypeDef:
         """
         Lists the details for all the accesses you have on your server.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.list_accesses)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#list_accesses)
         """
-
     def list_agreements(
         self, *, ServerId: str, MaxResults: int = ..., NextToken: str = ...
     ) -> ListAgreementsResponseTypeDef:
         """
         Returns a list of the agreements for the server that's identified by the
         `ServerId` that you supply.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.list_agreements)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#list_agreements)
         """
-
     def list_certificates(
         self, *, MaxResults: int = ..., NextToken: str = ...
     ) -> ListCertificatesResponseTypeDef:
         """
         Returns a list of the current certificates that have been imported into Transfer
         Family.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.list_certificates)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#list_certificates)
         """
-
     def list_connectors(
         self, *, MaxResults: int = ..., NextToken: str = ...
     ) -> ListConnectorsResponseTypeDef:
         """
         Lists the connectors for the specified Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.list_connectors)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#list_connectors)
         """
-
     def list_executions(
         self, *, WorkflowId: str, MaxResults: int = ..., NextToken: str = ...
     ) -> ListExecutionsResponseTypeDef:
         """
         Lists all in-progress executions for the specified workflow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.list_executions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#list_executions)
         """
-
     def list_host_keys(
         self, *, ServerId: str, MaxResults: int = ..., NextToken: str = ...
     ) -> ListHostKeysResponseTypeDef:
         """
         Returns a list of host keys for the server that's specified by the `ServerId`
         parameter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.list_host_keys)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#list_host_keys)
         """
-
     def list_profiles(
         self, *, MaxResults: int = ..., NextToken: str = ..., ProfileType: ProfileTypeType = ...
     ) -> ListProfilesResponseTypeDef:
         """
         Returns a list of the profiles for your system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.list_profiles)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#list_profiles)
         """
-
     def list_security_policies(
         self, *, MaxResults: int = ..., NextToken: str = ...
     ) -> ListSecurityPoliciesResponseTypeDef:
         """
         Lists the security policies that are attached to your file transfer protocol-
         enabled servers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.list_security_policies)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#list_security_policies)
         """
-
     def list_servers(
         self, *, MaxResults: int = ..., NextToken: str = ...
     ) -> ListServersResponseTypeDef:
         """
         Lists the file transfer protocol-enabled servers that are associated with your
         Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.list_servers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#list_servers)
         """
-
     def list_tags_for_resource(
         self, *, Arn: str, MaxResults: int = ..., NextToken: str = ...
     ) -> ListTagsForResourceResponseTypeDef:
         """
         Lists all of the tags associated with the Amazon Resource Name (ARN) that you
         specify.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#list_tags_for_resource)
         """
-
     def list_users(
         self, *, ServerId: str, MaxResults: int = ..., NextToken: str = ...
     ) -> ListUsersResponseTypeDef:
         """
         Lists the users for a file transfer protocol-enabled server that you specify by
         passing the `ServerId` parameter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.list_users)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#list_users)
         """
-
     def list_workflows(
         self, *, MaxResults: int = ..., NextToken: str = ...
     ) -> ListWorkflowsResponseTypeDef:
         """
         Lists all workflows associated with your Amazon Web Services account for your
         current region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.list_workflows)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#list_workflows)
         """
-
     def send_workflow_step_state(
         self, *, WorkflowId: str, ExecutionId: str, Token: str, Status: CustomStepStatusType
     ) -> Dict[str, Any]:
         """
         Sends a callback for asynchronous custom steps.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.send_workflow_step_state)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#send_workflow_step_state)
         """
-
     def start_file_transfer(
         self,
         *,
         ConnectorId: str,
         SendFilePaths: Sequence[str] = ...,
         RetrieveFilePaths: Sequence[str] = ...,
         LocalDirectoryPath: str = ...,
@@ -707,50 +649,45 @@
         """
         Begins a file transfer between local Amazon Web Services storage and a remote
         AS2 or SFTP server.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.start_file_transfer)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#start_file_transfer)
         """
-
     def start_server(self, *, ServerId: str) -> EmptyResponseMetadataTypeDef:
         """
         Changes the state of a file transfer protocol-enabled server from `OFFLINE` to
         `ONLINE`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.start_server)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#start_server)
         """
-
     def stop_server(self, *, ServerId: str) -> EmptyResponseMetadataTypeDef:
         """
         Changes the state of a file transfer protocol-enabled server from `ONLINE` to
         `OFFLINE`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.stop_server)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#stop_server)
         """
-
     def tag_resource(self, *, Arn: str, Tags: Sequence[TagTypeDef]) -> EmptyResponseMetadataTypeDef:
         """
         Attaches a key-value pair to a resource, as identified by its Amazon Resource
         Name (ARN).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#tag_resource)
         """
-
     def test_connection(self, *, ConnectorId: str) -> TestConnectionResponseTypeDef:
         """
         Tests whether your SFTP connector is set up successfully.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.test_connection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#test_connection)
         """
-
     def test_identity_provider(
         self,
         *,
         ServerId: str,
         UserName: str,
         ServerProtocol: ProtocolType = ...,
         SourceIp: str = ...,
@@ -760,44 +697,41 @@
         If the `IdentityProviderType` of a file transfer protocol-enabled server is
         `AWS_DIRECTORY_SERVICE` or `API_Gateway`, tests whether your identity provider
         is set up successfully.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.test_identity_provider)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#test_identity_provider)
         """
-
     def untag_resource(self, *, Arn: str, TagKeys: Sequence[str]) -> EmptyResponseMetadataTypeDef:
         """
         Detaches a key-value pair from a resource, as identified by its Amazon Resource
         Name (ARN).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#untag_resource)
         """
-
     def update_access(
         self,
         *,
         ServerId: str,
         ExternalId: str,
         HomeDirectory: str = ...,
         HomeDirectoryType: HomeDirectoryTypeType = ...,
         HomeDirectoryMappings: Sequence[HomeDirectoryMapEntryTypeDef] = ...,
         Policy: str = ...,
-        PosixProfile: Union[PosixProfileTypeDef, PosixProfileOutputTypeDef] = ...,
+        PosixProfile: PosixProfileUnionTypeDef = ...,
         Role: str = ...
     ) -> UpdateAccessResponseTypeDef:
         """
         Allows you to update parameters for the access specified in the `ServerID` and
         `ExternalID` parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.update_access)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#update_access)
         """
-
     def update_agreement(
         self,
         *,
         AgreementId: str,
         ServerId: str,
         Description: str = ...,
         Status: AgreementStatusTypeType = ...,
@@ -808,202 +742,183 @@
     ) -> UpdateAgreementResponseTypeDef:
         """
         Updates some of the parameters for an existing agreement.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.update_agreement)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#update_agreement)
         """
-
     def update_certificate(
         self,
         *,
         CertificateId: str,
-        ActiveDate: Union[datetime, str] = ...,
-        InactiveDate: Union[datetime, str] = ...,
+        ActiveDate: TimestampTypeDef = ...,
+        InactiveDate: TimestampTypeDef = ...,
         Description: str = ...
     ) -> UpdateCertificateResponseTypeDef:
         """
         Updates the active and inactive dates for a certificate.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.update_certificate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#update_certificate)
         """
-
     def update_connector(
         self,
         *,
         ConnectorId: str,
         Url: str = ...,
         As2Config: As2ConnectorConfigTypeDef = ...,
         AccessRole: str = ...,
         LoggingRole: str = ...,
-        SftpConfig: Union[SftpConnectorConfigTypeDef, SftpConnectorConfigOutputTypeDef] = ...
+        SftpConfig: SftpConnectorConfigUnionTypeDef = ...
     ) -> UpdateConnectorResponseTypeDef:
         """
         Updates some of the parameters for an existing connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.update_connector)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#update_connector)
         """
-
     def update_host_key(
         self, *, ServerId: str, HostKeyId: str, Description: str
     ) -> UpdateHostKeyResponseTypeDef:
         """
         Updates the description for the host key that's specified by the `ServerId` and
         `HostKeyId` parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.update_host_key)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#update_host_key)
         """
-
     def update_profile(
         self, *, ProfileId: str, CertificateIds: Sequence[str] = ...
     ) -> UpdateProfileResponseTypeDef:
         """
         Updates some of the parameters for an existing profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.update_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#update_profile)
         """
-
     def update_server(
         self,
         *,
         ServerId: str,
         Certificate: str = ...,
-        ProtocolDetails: Union[ProtocolDetailsTypeDef, ProtocolDetailsOutputTypeDef] = ...,
-        EndpointDetails: Union[EndpointDetailsTypeDef, EndpointDetailsOutputTypeDef] = ...,
+        ProtocolDetails: ProtocolDetailsUnionTypeDef = ...,
+        EndpointDetails: EndpointDetailsUnionTypeDef = ...,
         EndpointType: EndpointTypeType = ...,
         HostKey: str = ...,
         IdentityProviderDetails: IdentityProviderDetailsTypeDef = ...,
         LoggingRole: str = ...,
         PostAuthenticationLoginBanner: str = ...,
         PreAuthenticationLoginBanner: str = ...,
         Protocols: Sequence[ProtocolType] = ...,
         SecurityPolicyName: str = ...,
-        WorkflowDetails: Union[WorkflowDetailsTypeDef, WorkflowDetailsOutputTypeDef] = ...,
+        WorkflowDetails: WorkflowDetailsUnionTypeDef = ...,
         StructuredLogDestinations: Sequence[str] = ...
     ) -> UpdateServerResponseTypeDef:
         """
         Updates the file transfer protocol-enabled server's properties after that server
         has been created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.update_server)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#update_server)
         """
-
     def update_user(
         self,
         *,
         ServerId: str,
         UserName: str,
         HomeDirectory: str = ...,
         HomeDirectoryType: HomeDirectoryTypeType = ...,
         HomeDirectoryMappings: Sequence[HomeDirectoryMapEntryTypeDef] = ...,
         Policy: str = ...,
-        PosixProfile: Union[PosixProfileTypeDef, PosixProfileOutputTypeDef] = ...,
+        PosixProfile: PosixProfileUnionTypeDef = ...,
         Role: str = ...
     ) -> UpdateUserResponseTypeDef:
         """
         Assigns new properties to a user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.update_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#update_user)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["list_accesses"]) -> ListAccessesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["list_agreements"]) -> ListAgreementsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_certificates"]
     ) -> ListCertificatesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["list_connectors"]) -> ListConnectorsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["list_executions"]) -> ListExecutionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["list_profiles"]) -> ListProfilesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_security_policies"]
     ) -> ListSecurityPoliciesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["list_servers"]) -> ListServersPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_tags_for_resource"]
     ) -> ListTagsForResourcePaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["list_users"]) -> ListUsersPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["list_workflows"]) -> ListWorkflowsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#get_paginator)
         """
-
     @overload
     def get_waiter(self, waiter_name: Literal["server_offline"]) -> ServerOfflineWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.get_waiter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#get_waiter)
         """
-
     @overload
     def get_waiter(self, waiter_name: Literal["server_online"]) -> ServerOnlineWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.get_waiter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#get_waiter)
         """
```

### Comparing `mypy-boto3-transfer-1.28.15.post1/mypy_boto3_transfer/client.pyi` & `mypy-boto3-transfer-1.28.16/mypy_boto3_transfer/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from mypy_boto3_transfer.client import TransferClient
 
     session = Session()
     client: TransferClient = session.client("transfer")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AgreementStatusTypeType,
     CertificateUsageTypeType,
     CustomStepStatusType,
@@ -60,16 +59,15 @@
     DescribeHostKeyResponseTypeDef,
     DescribeProfileResponseTypeDef,
     DescribeSecurityPolicyResponseTypeDef,
     DescribeServerResponseTypeDef,
     DescribeUserResponseTypeDef,
     DescribeWorkflowResponseTypeDef,
     EmptyResponseMetadataTypeDef,
-    EndpointDetailsOutputTypeDef,
-    EndpointDetailsTypeDef,
+    EndpointDetailsUnionTypeDef,
     HomeDirectoryMapEntryTypeDef,
     IdentityProviderDetailsTypeDef,
     ImportCertificateResponseTypeDef,
     ImportHostKeyResponseTypeDef,
     ImportSshPublicKeyResponseTypeDef,
     ListAccessesResponseTypeDef,
     ListAgreementsResponseTypeDef,
@@ -79,65 +77,65 @@
     ListHostKeysResponseTypeDef,
     ListProfilesResponseTypeDef,
     ListSecurityPoliciesResponseTypeDef,
     ListServersResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListUsersResponseTypeDef,
     ListWorkflowsResponseTypeDef,
-    PosixProfileOutputTypeDef,
-    PosixProfileTypeDef,
-    ProtocolDetailsOutputTypeDef,
-    ProtocolDetailsTypeDef,
-    SftpConnectorConfigOutputTypeDef,
-    SftpConnectorConfigTypeDef,
+    PosixProfileUnionTypeDef,
+    ProtocolDetailsUnionTypeDef,
+    SftpConnectorConfigUnionTypeDef,
     StartFileTransferResponseTypeDef,
     TagTypeDef,
     TestConnectionResponseTypeDef,
     TestIdentityProviderResponseTypeDef,
+    TimestampTypeDef,
     UpdateAccessResponseTypeDef,
     UpdateAgreementResponseTypeDef,
     UpdateCertificateResponseTypeDef,
     UpdateConnectorResponseTypeDef,
     UpdateHostKeyResponseTypeDef,
     UpdateProfileResponseTypeDef,
     UpdateServerResponseTypeDef,
     UpdateUserResponseTypeDef,
-    WorkflowDetailsOutputTypeDef,
-    WorkflowDetailsTypeDef,
-    WorkflowStepOutputTypeDef,
-    WorkflowStepTypeDef,
+    WorkflowDetailsUnionTypeDef,
+    WorkflowStepUnionTypeDef,
 )
 from .waiter import ServerOfflineWaiter, ServerOnlineWaiter
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = ("TransferClient",)
 
+
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     InternalServiceError: Type[BotocoreClientError]
     InvalidNextTokenException: Type[BotocoreClientError]
     InvalidRequestException: Type[BotocoreClientError]
     ResourceExistsException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ServiceUnavailableException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
 
+
 class TransferClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/)
     """
 
     meta: ClientMeta
@@ -146,48 +144,52 @@
     def exceptions(self) -> Exceptions:
         """
         TransferClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#exceptions)
         """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#can_paginate)
         """
+
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#close)
         """
+
     def create_access(
         self,
         *,
         Role: str,
         ServerId: str,
         ExternalId: str,
         HomeDirectory: str = ...,
         HomeDirectoryType: HomeDirectoryTypeType = ...,
         HomeDirectoryMappings: Sequence[HomeDirectoryMapEntryTypeDef] = ...,
         Policy: str = ...,
-        PosixProfile: Union[PosixProfileTypeDef, PosixProfileOutputTypeDef] = ...
+        PosixProfile: PosixProfileUnionTypeDef = ...
     ) -> CreateAccessResponseTypeDef:
         """
         Used by administrators to choose which groups in the directory should have
         access to upload and download files over the enabled protocols using Transfer
         Family.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.create_access)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#create_access)
         """
+
     def create_agreement(
         self,
         *,
         ServerId: str,
         LocalProfileId: str,
         PartnerProfileId: str,
         BaseDirectory: str,
@@ -198,455 +200,499 @@
     ) -> CreateAgreementResponseTypeDef:
         """
         Creates an agreement.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.create_agreement)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#create_agreement)
         """
+
     def create_connector(
         self,
         *,
         Url: str,
         AccessRole: str,
         As2Config: As2ConnectorConfigTypeDef = ...,
         LoggingRole: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        SftpConfig: Union[SftpConnectorConfigTypeDef, SftpConnectorConfigOutputTypeDef] = ...
+        SftpConfig: SftpConnectorConfigUnionTypeDef = ...
     ) -> CreateConnectorResponseTypeDef:
         """
         Creates the connector, which captures the parameters for an outbound connection
         for the AS2 or SFTP protocol.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.create_connector)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#create_connector)
         """
+
     def create_profile(
         self,
         *,
         As2Id: str,
         ProfileType: ProfileTypeType,
         CertificateIds: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateProfileResponseTypeDef:
         """
         Creates the local or partner profile to use for AS2 transfers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.create_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#create_profile)
         """
+
     def create_server(
         self,
         *,
         Certificate: str = ...,
         Domain: DomainType = ...,
-        EndpointDetails: Union[EndpointDetailsTypeDef, EndpointDetailsOutputTypeDef] = ...,
+        EndpointDetails: EndpointDetailsUnionTypeDef = ...,
         EndpointType: EndpointTypeType = ...,
         HostKey: str = ...,
         IdentityProviderDetails: IdentityProviderDetailsTypeDef = ...,
         IdentityProviderType: IdentityProviderTypeType = ...,
         LoggingRole: str = ...,
         PostAuthenticationLoginBanner: str = ...,
         PreAuthenticationLoginBanner: str = ...,
         Protocols: Sequence[ProtocolType] = ...,
-        ProtocolDetails: Union[ProtocolDetailsTypeDef, ProtocolDetailsOutputTypeDef] = ...,
+        ProtocolDetails: ProtocolDetailsUnionTypeDef = ...,
         SecurityPolicyName: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        WorkflowDetails: Union[WorkflowDetailsTypeDef, WorkflowDetailsOutputTypeDef] = ...,
+        WorkflowDetails: WorkflowDetailsUnionTypeDef = ...,
         StructuredLogDestinations: Sequence[str] = ...
     ) -> CreateServerResponseTypeDef:
         """
         Instantiates an auto-scaling virtual server based on the selected file transfer
         protocol in Amazon Web Services.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.create_server)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#create_server)
         """
+
     def create_user(
         self,
         *,
         Role: str,
         ServerId: str,
         UserName: str,
         HomeDirectory: str = ...,
         HomeDirectoryType: HomeDirectoryTypeType = ...,
         HomeDirectoryMappings: Sequence[HomeDirectoryMapEntryTypeDef] = ...,
         Policy: str = ...,
-        PosixProfile: Union[PosixProfileTypeDef, PosixProfileOutputTypeDef] = ...,
+        PosixProfile: PosixProfileUnionTypeDef = ...,
         SshPublicKeyBody: str = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateUserResponseTypeDef:
         """
         Creates a user and associates them with an existing file transfer protocol-
         enabled server.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.create_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#create_user)
         """
+
     def create_workflow(
         self,
         *,
-        Steps: Sequence[Union[WorkflowStepTypeDef, WorkflowStepOutputTypeDef]],
+        Steps: Sequence[WorkflowStepUnionTypeDef],
         Description: str = ...,
-        OnExceptionSteps: Sequence[Union[WorkflowStepTypeDef, WorkflowStepOutputTypeDef]] = ...,
+        OnExceptionSteps: Sequence[WorkflowStepUnionTypeDef] = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateWorkflowResponseTypeDef:
         """
         Allows you to create a workflow with specified steps and step details the
         workflow invokes after file transfer completes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.create_workflow)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#create_workflow)
         """
+
     def delete_access(self, *, ServerId: str, ExternalId: str) -> EmptyResponseMetadataTypeDef:
         """
         Allows you to delete the access specified in the `ServerID` and `ExternalID`
         parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.delete_access)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#delete_access)
         """
+
     def delete_agreement(self, *, AgreementId: str, ServerId: str) -> EmptyResponseMetadataTypeDef:
         """
         Delete the agreement that's specified in the provided `AgreementId`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.delete_agreement)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#delete_agreement)
         """
+
     def delete_certificate(self, *, CertificateId: str) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the certificate that's specified in the `CertificateId` parameter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.delete_certificate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#delete_certificate)
         """
+
     def delete_connector(self, *, ConnectorId: str) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the connector that's specified in the provided `ConnectorId`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.delete_connector)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#delete_connector)
         """
+
     def delete_host_key(self, *, ServerId: str, HostKeyId: str) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the host key that's specified in the `HostKeyId` parameter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.delete_host_key)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#delete_host_key)
         """
+
     def delete_profile(self, *, ProfileId: str) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the profile that's specified in the `ProfileId` parameter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.delete_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#delete_profile)
         """
+
     def delete_server(self, *, ServerId: str) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the file transfer protocol-enabled server that you specify.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.delete_server)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#delete_server)
         """
+
     def delete_ssh_public_key(
         self, *, ServerId: str, SshPublicKeyId: str, UserName: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes a user's Secure Shell (SSH) public key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.delete_ssh_public_key)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#delete_ssh_public_key)
         """
+
     def delete_user(self, *, ServerId: str, UserName: str) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the user belonging to a file transfer protocol-enabled server you
         specify.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.delete_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#delete_user)
         """
+
     def delete_workflow(self, *, WorkflowId: str) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the specified workflow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.delete_workflow)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#delete_workflow)
         """
+
     def describe_access(self, *, ServerId: str, ExternalId: str) -> DescribeAccessResponseTypeDef:
         """
         Describes the access that is assigned to the specific file transfer protocol-
         enabled server, as identified by its `ServerId` property and its `ExternalId`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.describe_access)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#describe_access)
         """
+
     def describe_agreement(
         self, *, AgreementId: str, ServerId: str
     ) -> DescribeAgreementResponseTypeDef:
         """
         Describes the agreement that's identified by the `AgreementId`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.describe_agreement)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#describe_agreement)
         """
+
     def describe_certificate(self, *, CertificateId: str) -> DescribeCertificateResponseTypeDef:
         """
         Describes the certificate that's identified by the `CertificateId`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.describe_certificate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#describe_certificate)
         """
+
     def describe_connector(self, *, ConnectorId: str) -> DescribeConnectorResponseTypeDef:
         """
         Describes the connector that's identified by the `ConnectorId.` See also: [AWS
         API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/transfer-2018-11-05/DescribeConnector).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.describe_connector)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#describe_connector)
         """
+
     def describe_execution(
         self, *, ExecutionId: str, WorkflowId: str
     ) -> DescribeExecutionResponseTypeDef:
         """
         You can use `DescribeExecution` to check the details of the execution of the
         specified workflow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.describe_execution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#describe_execution)
         """
+
     def describe_host_key(self, *, ServerId: str, HostKeyId: str) -> DescribeHostKeyResponseTypeDef:
         """
         Returns the details of the host key that's specified by the `HostKeyId` and
         `ServerId`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.describe_host_key)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#describe_host_key)
         """
+
     def describe_profile(self, *, ProfileId: str) -> DescribeProfileResponseTypeDef:
         """
         Returns the details of the profile that's specified by the `ProfileId`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.describe_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#describe_profile)
         """
+
     def describe_security_policy(
         self, *, SecurityPolicyName: str
     ) -> DescribeSecurityPolicyResponseTypeDef:
         """
         Describes the security policy that is attached to your file transfer protocol-
         enabled server.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.describe_security_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#describe_security_policy)
         """
+
     def describe_server(self, *, ServerId: str) -> DescribeServerResponseTypeDef:
         """
         Describes a file transfer protocol-enabled server that you specify by passing
         the `ServerId` parameter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.describe_server)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#describe_server)
         """
+
     def describe_user(self, *, ServerId: str, UserName: str) -> DescribeUserResponseTypeDef:
         """
         Describes the user assigned to the specific file transfer protocol-enabled
         server, as identified by its `ServerId` property.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.describe_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#describe_user)
         """
+
     def describe_workflow(self, *, WorkflowId: str) -> DescribeWorkflowResponseTypeDef:
         """
         Describes the specified workflow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.describe_workflow)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#describe_workflow)
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
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#generate_presigned_url)
         """
+
     def import_certificate(
         self,
         *,
         Usage: CertificateUsageTypeType,
         Certificate: str,
         CertificateChain: str = ...,
         PrivateKey: str = ...,
-        ActiveDate: Union[datetime, str] = ...,
-        InactiveDate: Union[datetime, str] = ...,
+        ActiveDate: TimestampTypeDef = ...,
+        InactiveDate: TimestampTypeDef = ...,
         Description: str = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> ImportCertificateResponseTypeDef:
         """
         Imports the signing and encryption certificates that you need to create local
         (AS2) profiles and partner profiles.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.import_certificate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#import_certificate)
         """
+
     def import_host_key(
         self,
         *,
         ServerId: str,
         HostKeyBody: str,
         Description: str = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> ImportHostKeyResponseTypeDef:
         """
         Adds a host key to the server that's specified by the `ServerId` parameter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.import_host_key)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#import_host_key)
         """
+
     def import_ssh_public_key(
         self, *, ServerId: str, SshPublicKeyBody: str, UserName: str
     ) -> ImportSshPublicKeyResponseTypeDef:
         """
         Adds a Secure Shell (SSH) public key to a Transfer Family user identified by a
         `UserName` value assigned to the specific file transfer protocol-enabled server,
         identified by `ServerId`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.import_ssh_public_key)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#import_ssh_public_key)
         """
+
     def list_accesses(
         self, *, ServerId: str, MaxResults: int = ..., NextToken: str = ...
     ) -> ListAccessesResponseTypeDef:
         """
         Lists the details for all the accesses you have on your server.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.list_accesses)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#list_accesses)
         """
+
     def list_agreements(
         self, *, ServerId: str, MaxResults: int = ..., NextToken: str = ...
     ) -> ListAgreementsResponseTypeDef:
         """
         Returns a list of the agreements for the server that's identified by the
         `ServerId` that you supply.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.list_agreements)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#list_agreements)
         """
+
     def list_certificates(
         self, *, MaxResults: int = ..., NextToken: str = ...
     ) -> ListCertificatesResponseTypeDef:
         """
         Returns a list of the current certificates that have been imported into Transfer
         Family.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.list_certificates)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#list_certificates)
         """
+
     def list_connectors(
         self, *, MaxResults: int = ..., NextToken: str = ...
     ) -> ListConnectorsResponseTypeDef:
         """
         Lists the connectors for the specified Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.list_connectors)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#list_connectors)
         """
+
     def list_executions(
         self, *, WorkflowId: str, MaxResults: int = ..., NextToken: str = ...
     ) -> ListExecutionsResponseTypeDef:
         """
         Lists all in-progress executions for the specified workflow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.list_executions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#list_executions)
         """
+
     def list_host_keys(
         self, *, ServerId: str, MaxResults: int = ..., NextToken: str = ...
     ) -> ListHostKeysResponseTypeDef:
         """
         Returns a list of host keys for the server that's specified by the `ServerId`
         parameter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.list_host_keys)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#list_host_keys)
         """
+
     def list_profiles(
         self, *, MaxResults: int = ..., NextToken: str = ..., ProfileType: ProfileTypeType = ...
     ) -> ListProfilesResponseTypeDef:
         """
         Returns a list of the profiles for your system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.list_profiles)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#list_profiles)
         """
+
     def list_security_policies(
         self, *, MaxResults: int = ..., NextToken: str = ...
     ) -> ListSecurityPoliciesResponseTypeDef:
         """
         Lists the security policies that are attached to your file transfer protocol-
         enabled servers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.list_security_policies)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#list_security_policies)
         """
+
     def list_servers(
         self, *, MaxResults: int = ..., NextToken: str = ...
     ) -> ListServersResponseTypeDef:
         """
         Lists the file transfer protocol-enabled servers that are associated with your
         Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.list_servers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#list_servers)
         """
+
     def list_tags_for_resource(
         self, *, Arn: str, MaxResults: int = ..., NextToken: str = ...
     ) -> ListTagsForResourceResponseTypeDef:
         """
         Lists all of the tags associated with the Amazon Resource Name (ARN) that you
         specify.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#list_tags_for_resource)
         """
+
     def list_users(
         self, *, ServerId: str, MaxResults: int = ..., NextToken: str = ...
     ) -> ListUsersResponseTypeDef:
         """
         Lists the users for a file transfer protocol-enabled server that you specify by
         passing the `ServerId` parameter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.list_users)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#list_users)
         """
+
     def list_workflows(
         self, *, MaxResults: int = ..., NextToken: str = ...
     ) -> ListWorkflowsResponseTypeDef:
         """
         Lists all workflows associated with your Amazon Web Services account for your
         current region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.list_workflows)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#list_workflows)
         """
+
     def send_workflow_step_state(
         self, *, WorkflowId: str, ExecutionId: str, Token: str, Status: CustomStepStatusType
     ) -> Dict[str, Any]:
         """
         Sends a callback for asynchronous custom steps.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.send_workflow_step_state)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#send_workflow_step_state)
         """
+
     def start_file_transfer(
         self,
         *,
         ConnectorId: str,
         SendFilePaths: Sequence[str] = ...,
         RetrieveFilePaths: Sequence[str] = ...,
         LocalDirectoryPath: str = ...,
@@ -655,45 +701,50 @@
         """
         Begins a file transfer between local Amazon Web Services storage and a remote
         AS2 or SFTP server.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.start_file_transfer)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#start_file_transfer)
         """
+
     def start_server(self, *, ServerId: str) -> EmptyResponseMetadataTypeDef:
         """
         Changes the state of a file transfer protocol-enabled server from `OFFLINE` to
         `ONLINE`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.start_server)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#start_server)
         """
+
     def stop_server(self, *, ServerId: str) -> EmptyResponseMetadataTypeDef:
         """
         Changes the state of a file transfer protocol-enabled server from `ONLINE` to
         `OFFLINE`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.stop_server)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#stop_server)
         """
+
     def tag_resource(self, *, Arn: str, Tags: Sequence[TagTypeDef]) -> EmptyResponseMetadataTypeDef:
         """
         Attaches a key-value pair to a resource, as identified by its Amazon Resource
         Name (ARN).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#tag_resource)
         """
+
     def test_connection(self, *, ConnectorId: str) -> TestConnectionResponseTypeDef:
         """
         Tests whether your SFTP connector is set up successfully.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.test_connection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#test_connection)
         """
+
     def test_identity_provider(
         self,
         *,
         ServerId: str,
         UserName: str,
         ServerProtocol: ProtocolType = ...,
         SourceIp: str = ...,
@@ -703,41 +754,44 @@
         If the `IdentityProviderType` of a file transfer protocol-enabled server is
         `AWS_DIRECTORY_SERVICE` or `API_Gateway`, tests whether your identity provider
         is set up successfully.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.test_identity_provider)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#test_identity_provider)
         """
+
     def untag_resource(self, *, Arn: str, TagKeys: Sequence[str]) -> EmptyResponseMetadataTypeDef:
         """
         Detaches a key-value pair from a resource, as identified by its Amazon Resource
         Name (ARN).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#untag_resource)
         """
+
     def update_access(
         self,
         *,
         ServerId: str,
         ExternalId: str,
         HomeDirectory: str = ...,
         HomeDirectoryType: HomeDirectoryTypeType = ...,
         HomeDirectoryMappings: Sequence[HomeDirectoryMapEntryTypeDef] = ...,
         Policy: str = ...,
-        PosixProfile: Union[PosixProfileTypeDef, PosixProfileOutputTypeDef] = ...,
+        PosixProfile: PosixProfileUnionTypeDef = ...,
         Role: str = ...
     ) -> UpdateAccessResponseTypeDef:
         """
         Allows you to update parameters for the access specified in the `ServerID` and
         `ExternalID` parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.update_access)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#update_access)
         """
+
     def update_agreement(
         self,
         *,
         AgreementId: str,
         ServerId: str,
         Description: str = ...,
         Status: AgreementStatusTypeType = ...,
@@ -748,183 +802,202 @@
     ) -> UpdateAgreementResponseTypeDef:
         """
         Updates some of the parameters for an existing agreement.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.update_agreement)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#update_agreement)
         """
+
     def update_certificate(
         self,
         *,
         CertificateId: str,
-        ActiveDate: Union[datetime, str] = ...,
-        InactiveDate: Union[datetime, str] = ...,
+        ActiveDate: TimestampTypeDef = ...,
+        InactiveDate: TimestampTypeDef = ...,
         Description: str = ...
     ) -> UpdateCertificateResponseTypeDef:
         """
         Updates the active and inactive dates for a certificate.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.update_certificate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#update_certificate)
         """
+
     def update_connector(
         self,
         *,
         ConnectorId: str,
         Url: str = ...,
         As2Config: As2ConnectorConfigTypeDef = ...,
         AccessRole: str = ...,
         LoggingRole: str = ...,
-        SftpConfig: Union[SftpConnectorConfigTypeDef, SftpConnectorConfigOutputTypeDef] = ...
+        SftpConfig: SftpConnectorConfigUnionTypeDef = ...
     ) -> UpdateConnectorResponseTypeDef:
         """
         Updates some of the parameters for an existing connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.update_connector)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#update_connector)
         """
+
     def update_host_key(
         self, *, ServerId: str, HostKeyId: str, Description: str
     ) -> UpdateHostKeyResponseTypeDef:
         """
         Updates the description for the host key that's specified by the `ServerId` and
         `HostKeyId` parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.update_host_key)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#update_host_key)
         """
+
     def update_profile(
         self, *, ProfileId: str, CertificateIds: Sequence[str] = ...
     ) -> UpdateProfileResponseTypeDef:
         """
         Updates some of the parameters for an existing profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.update_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#update_profile)
         """
+
     def update_server(
         self,
         *,
         ServerId: str,
         Certificate: str = ...,
-        ProtocolDetails: Union[ProtocolDetailsTypeDef, ProtocolDetailsOutputTypeDef] = ...,
-        EndpointDetails: Union[EndpointDetailsTypeDef, EndpointDetailsOutputTypeDef] = ...,
+        ProtocolDetails: ProtocolDetailsUnionTypeDef = ...,
+        EndpointDetails: EndpointDetailsUnionTypeDef = ...,
         EndpointType: EndpointTypeType = ...,
         HostKey: str = ...,
         IdentityProviderDetails: IdentityProviderDetailsTypeDef = ...,
         LoggingRole: str = ...,
         PostAuthenticationLoginBanner: str = ...,
         PreAuthenticationLoginBanner: str = ...,
         Protocols: Sequence[ProtocolType] = ...,
         SecurityPolicyName: str = ...,
-        WorkflowDetails: Union[WorkflowDetailsTypeDef, WorkflowDetailsOutputTypeDef] = ...,
+        WorkflowDetails: WorkflowDetailsUnionTypeDef = ...,
         StructuredLogDestinations: Sequence[str] = ...
     ) -> UpdateServerResponseTypeDef:
         """
         Updates the file transfer protocol-enabled server's properties after that server
         has been created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.update_server)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#update_server)
         """
+
     def update_user(
         self,
         *,
         ServerId: str,
         UserName: str,
         HomeDirectory: str = ...,
         HomeDirectoryType: HomeDirectoryTypeType = ...,
         HomeDirectoryMappings: Sequence[HomeDirectoryMapEntryTypeDef] = ...,
         Policy: str = ...,
-        PosixProfile: Union[PosixProfileTypeDef, PosixProfileOutputTypeDef] = ...,
+        PosixProfile: PosixProfileUnionTypeDef = ...,
         Role: str = ...
     ) -> UpdateUserResponseTypeDef:
         """
         Assigns new properties to a user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.update_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#update_user)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["list_accesses"]) -> ListAccessesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["list_agreements"]) -> ListAgreementsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_certificates"]
     ) -> ListCertificatesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["list_connectors"]) -> ListConnectorsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["list_executions"]) -> ListExecutionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["list_profiles"]) -> ListProfilesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_security_policies"]
     ) -> ListSecurityPoliciesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["list_servers"]) -> ListServersPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_tags_for_resource"]
     ) -> ListTagsForResourcePaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["list_users"]) -> ListUsersPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["list_workflows"]) -> ListWorkflowsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#get_paginator)
         """
+
     @overload
     def get_waiter(self, waiter_name: Literal["server_offline"]) -> ServerOfflineWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.get_waiter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#get_waiter)
         """
+
     @overload
     def get_waiter(self, waiter_name: Literal["server_online"]) -> ServerOnlineWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.get_waiter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#get_waiter)
         """
```

### Comparing `mypy-boto3-transfer-1.28.15.post1/mypy_boto3_transfer/literals.py` & `mypy-boto3-transfer-1.28.16/mypy_boto3_transfer/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transfer-1.28.15.post1/mypy_boto3_transfer/literals.pyi` & `mypy-boto3-transfer-1.28.16/mypy_boto3_transfer/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transfer-1.28.15.post1/mypy_boto3_transfer/paginator.py` & `mypy-boto3-transfer-1.28.16/mypy_boto3_transfer/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transfer-1.28.15.post1/mypy_boto3_transfer/paginator.pyi` & `mypy-boto3-transfer-1.28.16/mypy_boto3_transfer/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transfer-1.28.15.post1/mypy_boto3_transfer/type_defs.py` & `mypy-boto3-transfer-1.28.16/mypy_boto3_transfer/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_transfer.type_defs import As2ConnectorConfigTypeDef
 
-    data: As2ConnectorConfigTypeDef = {...}
+    data: As2ConnectorConfigTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -92,14 +92,15 @@
     "LoggingConfigurationTypeDef",
     "EndpointDetailsOutputTypeDef",
     "ProtocolDetailsOutputTypeDef",
     "SshPublicKeyTypeDef",
     "EfsFileLocationTypeDef",
     "ExecutionErrorTypeDef",
     "S3FileLocationTypeDef",
+    "TimestampTypeDef",
     "ImportSshPublicKeyRequestRequestTypeDef",
     "S3InputFileLocationTypeDef",
     "PaginatorConfigTypeDef",
     "ListAccessesRequestRequestTypeDef",
     "ListedAccessTypeDef",
     "ListAgreementsRequestRequestTypeDef",
     "ListedAgreementTypeDef",
@@ -126,15 +127,14 @@
     "StartFileTransferRequestRequestTypeDef",
     "StartServerRequestRequestTypeDef",
     "StopServerRequestRequestTypeDef",
     "TestConnectionRequestRequestTypeDef",
     "TestIdentityProviderRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAgreementRequestRequestTypeDef",
-    "UpdateCertificateRequestRequestTypeDef",
     "UpdateHostKeyRequestRequestTypeDef",
     "UpdateProfileRequestRequestTypeDef",
     "WorkflowDetailTypeDef",
     "CreateAccessRequestRequestTypeDef",
     "UpdateAccessRequestRequestTypeDef",
     "UpdateUserRequestRequestTypeDef",
     "CreateAccessResponseTypeDef",
@@ -163,28 +163,33 @@
     "CreateAgreementRequestRequestTypeDef",
     "CreateProfileRequestRequestTypeDef",
     "CreateUserRequestRequestTypeDef",
     "DescribedAgreementTypeDef",
     "DescribedCertificateTypeDef",
     "DescribedHostKeyTypeDef",
     "DescribedProfileTypeDef",
-    "ImportCertificateRequestRequestTypeDef",
     "ImportHostKeyRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateConnectorRequestRequestTypeDef",
     "UpdateConnectorRequestRequestTypeDef",
     "DescribeSecurityPolicyResponseTypeDef",
     "DescribeServerRequestServerOfflineWaitTypeDef",
     "DescribeServerRequestServerOnlineWaitTypeDef",
     "DescribedAccessTypeDef",
+    "PosixProfileUnionTypeDef",
     "DescribedConnectorTypeDef",
+    "SftpConnectorConfigUnionTypeDef",
+    "EndpointDetailsUnionTypeDef",
+    "ProtocolDetailsUnionTypeDef",
     "DescribedUserTypeDef",
     "ExecutionStepResultTypeDef",
     "FileLocationTypeDef",
+    "ImportCertificateRequestRequestTypeDef",
+    "UpdateCertificateRequestRequestTypeDef",
     "InputFileLocationTypeDef",
     "ListAccessesRequestListAccessesPaginateTypeDef",
     "ListAgreementsRequestListAgreementsPaginateTypeDef",
     "ListCertificatesRequestListCertificatesPaginateTypeDef",
     "ListConnectorsRequestListConnectorsPaginateTypeDef",
     "ListExecutionsRequestListExecutionsPaginateTypeDef",
     "ListProfilesRequestListProfilesPaginateTypeDef",
@@ -217,23 +222,25 @@
     "ExecutionResultsTypeDef",
     "CopyStepDetailsTypeDef",
     "DecryptStepDetailsTypeDef",
     "ListedExecutionTypeDef",
     "DescribedServerTypeDef",
     "CreateServerRequestRequestTypeDef",
     "UpdateServerRequestRequestTypeDef",
+    "WorkflowDetailsUnionTypeDef",
     "DescribedExecutionTypeDef",
     "WorkflowStepOutputTypeDef",
     "WorkflowStepTypeDef",
     "ListExecutionsResponseTypeDef",
     "DescribeServerResponseTypeDef",
     "DescribeExecutionResponseTypeDef",
     "DescribedWorkflowTypeDef",
-    "CreateWorkflowRequestRequestTypeDef",
+    "WorkflowStepUnionTypeDef",
     "DescribeWorkflowResponseTypeDef",
+    "CreateWorkflowRequestRequestTypeDef",
 )
 
 As2ConnectorConfigTypeDef = TypedDict(
     "As2ConnectorConfigTypeDef",
     {
         "LocalProfileId": str,
         "PartnerProfileId": str,
@@ -647,14 +654,15 @@
         "Key": str,
         "VersionId": str,
         "Etag": str,
     },
     total=False,
 )
 
+TimestampTypeDef = Union[datetime, str]
 ImportSshPublicKeyRequestRequestTypeDef = TypedDict(
     "ImportSshPublicKeyRequestRequestTypeDef",
     {
         "ServerId": str,
         "SshPublicKeyBody": str,
         "UserName": str,
     },
@@ -1148,37 +1156,14 @@
 
 class UpdateAgreementRequestRequestTypeDef(
     _RequiredUpdateAgreementRequestRequestTypeDef, _OptionalUpdateAgreementRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredUpdateCertificateRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateCertificateRequestRequestTypeDef",
-    {
-        "CertificateId": str,
-    },
-)
-_OptionalUpdateCertificateRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateCertificateRequestRequestTypeDef",
-    {
-        "ActiveDate": Union[datetime, str],
-        "InactiveDate": Union[datetime, str],
-        "Description": str,
-    },
-    total=False,
-)
-
-
-class UpdateCertificateRequestRequestTypeDef(
-    _RequiredUpdateCertificateRequestRequestTypeDef, _OptionalUpdateCertificateRequestRequestTypeDef
-):
-    pass
-
-
 UpdateHostKeyRequestRequestTypeDef = TypedDict(
     "UpdateHostKeyRequestRequestTypeDef",
     {
         "ServerId": str,
         "HostKeyId": str,
         "Description": str,
     },
@@ -1675,41 +1660,14 @@
 )
 
 
 class DescribedProfileTypeDef(_RequiredDescribedProfileTypeDef, _OptionalDescribedProfileTypeDef):
     pass
 
 
-_RequiredImportCertificateRequestRequestTypeDef = TypedDict(
-    "_RequiredImportCertificateRequestRequestTypeDef",
-    {
-        "Usage": CertificateUsageTypeType,
-        "Certificate": str,
-    },
-)
-_OptionalImportCertificateRequestRequestTypeDef = TypedDict(
-    "_OptionalImportCertificateRequestRequestTypeDef",
-    {
-        "CertificateChain": str,
-        "PrivateKey": str,
-        "ActiveDate": Union[datetime, str],
-        "InactiveDate": Union[datetime, str],
-        "Description": str,
-        "Tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-
-class ImportCertificateRequestRequestTypeDef(
-    _RequiredImportCertificateRequestRequestTypeDef, _OptionalImportCertificateRequestRequestTypeDef
-):
-    pass
-
-
 _RequiredImportHostKeyRequestRequestTypeDef = TypedDict(
     "_RequiredImportHostKeyRequestRequestTypeDef",
     {
         "ServerId": str,
         "HostKeyBody": str,
     },
 )
@@ -1859,14 +1817,15 @@
         "PosixProfile": PosixProfileOutputTypeDef,
         "Role": str,
         "ExternalId": str,
     },
     total=False,
 )
 
+PosixProfileUnionTypeDef = Union[PosixProfileTypeDef, PosixProfileOutputTypeDef]
 _RequiredDescribedConnectorTypeDef = TypedDict(
     "_RequiredDescribedConnectorTypeDef",
     {
         "Arn": str,
     },
 )
 _OptionalDescribedConnectorTypeDef = TypedDict(
@@ -1886,14 +1845,19 @@
 
 class DescribedConnectorTypeDef(
     _RequiredDescribedConnectorTypeDef, _OptionalDescribedConnectorTypeDef
 ):
     pass
 
 
+SftpConnectorConfigUnionTypeDef = Union[
+    SftpConnectorConfigTypeDef, SftpConnectorConfigOutputTypeDef
+]
+EndpointDetailsUnionTypeDef = Union[EndpointDetailsTypeDef, EndpointDetailsOutputTypeDef]
+ProtocolDetailsUnionTypeDef = Union[ProtocolDetailsTypeDef, ProtocolDetailsOutputTypeDef]
 _RequiredDescribedUserTypeDef = TypedDict(
     "_RequiredDescribedUserTypeDef",
     {
         "Arn": str,
     },
 )
 _OptionalDescribedUserTypeDef = TypedDict(
@@ -1932,14 +1896,64 @@
     {
         "S3FileLocation": S3FileLocationTypeDef,
         "EfsFileLocation": EfsFileLocationTypeDef,
     },
     total=False,
 )
 
+_RequiredImportCertificateRequestRequestTypeDef = TypedDict(
+    "_RequiredImportCertificateRequestRequestTypeDef",
+    {
+        "Usage": CertificateUsageTypeType,
+        "Certificate": str,
+    },
+)
+_OptionalImportCertificateRequestRequestTypeDef = TypedDict(
+    "_OptionalImportCertificateRequestRequestTypeDef",
+    {
+        "CertificateChain": str,
+        "PrivateKey": str,
+        "ActiveDate": TimestampTypeDef,
+        "InactiveDate": TimestampTypeDef,
+        "Description": str,
+        "Tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+
+class ImportCertificateRequestRequestTypeDef(
+    _RequiredImportCertificateRequestRequestTypeDef, _OptionalImportCertificateRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredUpdateCertificateRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateCertificateRequestRequestTypeDef",
+    {
+        "CertificateId": str,
+    },
+)
+_OptionalUpdateCertificateRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateCertificateRequestRequestTypeDef",
+    {
+        "ActiveDate": TimestampTypeDef,
+        "InactiveDate": TimestampTypeDef,
+        "Description": str,
+    },
+    total=False,
+)
+
+
+class UpdateCertificateRequestRequestTypeDef(
+    _RequiredUpdateCertificateRequestRequestTypeDef, _OptionalUpdateCertificateRequestRequestTypeDef
+):
+    pass
+
+
 InputFileLocationTypeDef = TypedDict(
     "InputFileLocationTypeDef",
     {
         "S3FileLocation": S3InputFileLocationTypeDef,
         "EfsFileLocation": EfsFileLocationTypeDef,
     },
     total=False,
@@ -2435,14 +2449,15 @@
 
 class UpdateServerRequestRequestTypeDef(
     _RequiredUpdateServerRequestRequestTypeDef, _OptionalUpdateServerRequestRequestTypeDef
 ):
     pass
 
 
+WorkflowDetailsUnionTypeDef = Union[WorkflowDetailsTypeDef, WorkflowDetailsOutputTypeDef]
 DescribedExecutionTypeDef = TypedDict(
     "DescribedExecutionTypeDef",
     {
         "ExecutionId": str,
         "InitialFileLocation": FileLocationTypeDef,
         "ServiceMetadata": ServiceMetadataTypeDef,
         "ExecutionRole": str,
@@ -2528,37 +2543,37 @@
 
 class DescribedWorkflowTypeDef(
     _RequiredDescribedWorkflowTypeDef, _OptionalDescribedWorkflowTypeDef
 ):
     pass
 
 
+WorkflowStepUnionTypeDef = Union[WorkflowStepTypeDef, WorkflowStepOutputTypeDef]
+DescribeWorkflowResponseTypeDef = TypedDict(
+    "DescribeWorkflowResponseTypeDef",
+    {
+        "Workflow": DescribedWorkflowTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateWorkflowRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWorkflowRequestRequestTypeDef",
     {
-        "Steps": Sequence[Union[WorkflowStepTypeDef, WorkflowStepOutputTypeDef]],
+        "Steps": Sequence[WorkflowStepUnionTypeDef],
     },
 )
 _OptionalCreateWorkflowRequestRequestTypeDef = TypedDict(
     "_OptionalCreateWorkflowRequestRequestTypeDef",
     {
         "Description": str,
-        "OnExceptionSteps": Sequence[Union[WorkflowStepTypeDef, WorkflowStepOutputTypeDef]],
+        "OnExceptionSteps": Sequence[WorkflowStepUnionTypeDef],
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
 
 class CreateWorkflowRequestRequestTypeDef(
     _RequiredCreateWorkflowRequestRequestTypeDef, _OptionalCreateWorkflowRequestRequestTypeDef
 ):
     pass
-
-
-DescribeWorkflowResponseTypeDef = TypedDict(
-    "DescribeWorkflowResponseTypeDef",
-    {
-        "Workflow": DescribedWorkflowTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
```

### Comparing `mypy-boto3-transfer-1.28.15.post1/mypy_boto3_transfer/type_defs.pyi` & `mypy-boto3-transfer-1.28.16/mypy_boto3_transfer/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_transfer.type_defs import As2ConnectorConfigTypeDef
 
-    data: As2ConnectorConfigTypeDef = {...}
+    data: As2ConnectorConfigTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -91,14 +91,15 @@
     "LoggingConfigurationTypeDef",
     "EndpointDetailsOutputTypeDef",
     "ProtocolDetailsOutputTypeDef",
     "SshPublicKeyTypeDef",
     "EfsFileLocationTypeDef",
     "ExecutionErrorTypeDef",
     "S3FileLocationTypeDef",
+    "TimestampTypeDef",
     "ImportSshPublicKeyRequestRequestTypeDef",
     "S3InputFileLocationTypeDef",
     "PaginatorConfigTypeDef",
     "ListAccessesRequestRequestTypeDef",
     "ListedAccessTypeDef",
     "ListAgreementsRequestRequestTypeDef",
     "ListedAgreementTypeDef",
@@ -125,15 +126,14 @@
     "StartFileTransferRequestRequestTypeDef",
     "StartServerRequestRequestTypeDef",
     "StopServerRequestRequestTypeDef",
     "TestConnectionRequestRequestTypeDef",
     "TestIdentityProviderRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAgreementRequestRequestTypeDef",
-    "UpdateCertificateRequestRequestTypeDef",
     "UpdateHostKeyRequestRequestTypeDef",
     "UpdateProfileRequestRequestTypeDef",
     "WorkflowDetailTypeDef",
     "CreateAccessRequestRequestTypeDef",
     "UpdateAccessRequestRequestTypeDef",
     "UpdateUserRequestRequestTypeDef",
     "CreateAccessResponseTypeDef",
@@ -162,28 +162,33 @@
     "CreateAgreementRequestRequestTypeDef",
     "CreateProfileRequestRequestTypeDef",
     "CreateUserRequestRequestTypeDef",
     "DescribedAgreementTypeDef",
     "DescribedCertificateTypeDef",
     "DescribedHostKeyTypeDef",
     "DescribedProfileTypeDef",
-    "ImportCertificateRequestRequestTypeDef",
     "ImportHostKeyRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateConnectorRequestRequestTypeDef",
     "UpdateConnectorRequestRequestTypeDef",
     "DescribeSecurityPolicyResponseTypeDef",
     "DescribeServerRequestServerOfflineWaitTypeDef",
     "DescribeServerRequestServerOnlineWaitTypeDef",
     "DescribedAccessTypeDef",
+    "PosixProfileUnionTypeDef",
     "DescribedConnectorTypeDef",
+    "SftpConnectorConfigUnionTypeDef",
+    "EndpointDetailsUnionTypeDef",
+    "ProtocolDetailsUnionTypeDef",
     "DescribedUserTypeDef",
     "ExecutionStepResultTypeDef",
     "FileLocationTypeDef",
+    "ImportCertificateRequestRequestTypeDef",
+    "UpdateCertificateRequestRequestTypeDef",
     "InputFileLocationTypeDef",
     "ListAccessesRequestListAccessesPaginateTypeDef",
     "ListAgreementsRequestListAgreementsPaginateTypeDef",
     "ListCertificatesRequestListCertificatesPaginateTypeDef",
     "ListConnectorsRequestListConnectorsPaginateTypeDef",
     "ListExecutionsRequestListExecutionsPaginateTypeDef",
     "ListProfilesRequestListProfilesPaginateTypeDef",
@@ -216,23 +221,25 @@
     "ExecutionResultsTypeDef",
     "CopyStepDetailsTypeDef",
     "DecryptStepDetailsTypeDef",
     "ListedExecutionTypeDef",
     "DescribedServerTypeDef",
     "CreateServerRequestRequestTypeDef",
     "UpdateServerRequestRequestTypeDef",
+    "WorkflowDetailsUnionTypeDef",
     "DescribedExecutionTypeDef",
     "WorkflowStepOutputTypeDef",
     "WorkflowStepTypeDef",
     "ListExecutionsResponseTypeDef",
     "DescribeServerResponseTypeDef",
     "DescribeExecutionResponseTypeDef",
     "DescribedWorkflowTypeDef",
-    "CreateWorkflowRequestRequestTypeDef",
+    "WorkflowStepUnionTypeDef",
     "DescribeWorkflowResponseTypeDef",
+    "CreateWorkflowRequestRequestTypeDef",
 )
 
 As2ConnectorConfigTypeDef = TypedDict(
     "As2ConnectorConfigTypeDef",
     {
         "LocalProfileId": str,
         "PartnerProfileId": str,
@@ -640,14 +647,15 @@
         "Key": str,
         "VersionId": str,
         "Etag": str,
     },
     total=False,
 )
 
+TimestampTypeDef = Union[datetime, str]
 ImportSshPublicKeyRequestRequestTypeDef = TypedDict(
     "ImportSshPublicKeyRequestRequestTypeDef",
     {
         "ServerId": str,
         "SshPublicKeyBody": str,
         "UserName": str,
     },
@@ -1115,35 +1123,14 @@
 )
 
 class UpdateAgreementRequestRequestTypeDef(
     _RequiredUpdateAgreementRequestRequestTypeDef, _OptionalUpdateAgreementRequestRequestTypeDef
 ):
     pass
 
-_RequiredUpdateCertificateRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateCertificateRequestRequestTypeDef",
-    {
-        "CertificateId": str,
-    },
-)
-_OptionalUpdateCertificateRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateCertificateRequestRequestTypeDef",
-    {
-        "ActiveDate": Union[datetime, str],
-        "InactiveDate": Union[datetime, str],
-        "Description": str,
-    },
-    total=False,
-)
-
-class UpdateCertificateRequestRequestTypeDef(
-    _RequiredUpdateCertificateRequestRequestTypeDef, _OptionalUpdateCertificateRequestRequestTypeDef
-):
-    pass
-
 UpdateHostKeyRequestRequestTypeDef = TypedDict(
     "UpdateHostKeyRequestRequestTypeDef",
     {
         "ServerId": str,
         "HostKeyId": str,
         "Description": str,
     },
@@ -1618,39 +1605,14 @@
     },
     total=False,
 )
 
 class DescribedProfileTypeDef(_RequiredDescribedProfileTypeDef, _OptionalDescribedProfileTypeDef):
     pass
 
-_RequiredImportCertificateRequestRequestTypeDef = TypedDict(
-    "_RequiredImportCertificateRequestRequestTypeDef",
-    {
-        "Usage": CertificateUsageTypeType,
-        "Certificate": str,
-    },
-)
-_OptionalImportCertificateRequestRequestTypeDef = TypedDict(
-    "_OptionalImportCertificateRequestRequestTypeDef",
-    {
-        "CertificateChain": str,
-        "PrivateKey": str,
-        "ActiveDate": Union[datetime, str],
-        "InactiveDate": Union[datetime, str],
-        "Description": str,
-        "Tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-class ImportCertificateRequestRequestTypeDef(
-    _RequiredImportCertificateRequestRequestTypeDef, _OptionalImportCertificateRequestRequestTypeDef
-):
-    pass
-
 _RequiredImportHostKeyRequestRequestTypeDef = TypedDict(
     "_RequiredImportHostKeyRequestRequestTypeDef",
     {
         "ServerId": str,
         "HostKeyBody": str,
     },
 )
@@ -1790,14 +1752,15 @@
         "PosixProfile": PosixProfileOutputTypeDef,
         "Role": str,
         "ExternalId": str,
     },
     total=False,
 )
 
+PosixProfileUnionTypeDef = Union[PosixProfileTypeDef, PosixProfileOutputTypeDef]
 _RequiredDescribedConnectorTypeDef = TypedDict(
     "_RequiredDescribedConnectorTypeDef",
     {
         "Arn": str,
     },
 )
 _OptionalDescribedConnectorTypeDef = TypedDict(
@@ -1815,14 +1778,19 @@
 )
 
 class DescribedConnectorTypeDef(
     _RequiredDescribedConnectorTypeDef, _OptionalDescribedConnectorTypeDef
 ):
     pass
 
+SftpConnectorConfigUnionTypeDef = Union[
+    SftpConnectorConfigTypeDef, SftpConnectorConfigOutputTypeDef
+]
+EndpointDetailsUnionTypeDef = Union[EndpointDetailsTypeDef, EndpointDetailsOutputTypeDef]
+ProtocolDetailsUnionTypeDef = Union[ProtocolDetailsTypeDef, ProtocolDetailsOutputTypeDef]
 _RequiredDescribedUserTypeDef = TypedDict(
     "_RequiredDescribedUserTypeDef",
     {
         "Arn": str,
     },
 )
 _OptionalDescribedUserTypeDef = TypedDict(
@@ -1859,14 +1827,60 @@
     {
         "S3FileLocation": S3FileLocationTypeDef,
         "EfsFileLocation": EfsFileLocationTypeDef,
     },
     total=False,
 )
 
+_RequiredImportCertificateRequestRequestTypeDef = TypedDict(
+    "_RequiredImportCertificateRequestRequestTypeDef",
+    {
+        "Usage": CertificateUsageTypeType,
+        "Certificate": str,
+    },
+)
+_OptionalImportCertificateRequestRequestTypeDef = TypedDict(
+    "_OptionalImportCertificateRequestRequestTypeDef",
+    {
+        "CertificateChain": str,
+        "PrivateKey": str,
+        "ActiveDate": TimestampTypeDef,
+        "InactiveDate": TimestampTypeDef,
+        "Description": str,
+        "Tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+class ImportCertificateRequestRequestTypeDef(
+    _RequiredImportCertificateRequestRequestTypeDef, _OptionalImportCertificateRequestRequestTypeDef
+):
+    pass
+
+_RequiredUpdateCertificateRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateCertificateRequestRequestTypeDef",
+    {
+        "CertificateId": str,
+    },
+)
+_OptionalUpdateCertificateRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateCertificateRequestRequestTypeDef",
+    {
+        "ActiveDate": TimestampTypeDef,
+        "InactiveDate": TimestampTypeDef,
+        "Description": str,
+    },
+    total=False,
+)
+
+class UpdateCertificateRequestRequestTypeDef(
+    _RequiredUpdateCertificateRequestRequestTypeDef, _OptionalUpdateCertificateRequestRequestTypeDef
+):
+    pass
+
 InputFileLocationTypeDef = TypedDict(
     "InputFileLocationTypeDef",
     {
         "S3FileLocation": S3InputFileLocationTypeDef,
         "EfsFileLocation": EfsFileLocationTypeDef,
     },
     total=False,
@@ -2346,14 +2360,15 @@
 )
 
 class UpdateServerRequestRequestTypeDef(
     _RequiredUpdateServerRequestRequestTypeDef, _OptionalUpdateServerRequestRequestTypeDef
 ):
     pass
 
+WorkflowDetailsUnionTypeDef = Union[WorkflowDetailsTypeDef, WorkflowDetailsOutputTypeDef]
 DescribedExecutionTypeDef = TypedDict(
     "DescribedExecutionTypeDef",
     {
         "ExecutionId": str,
         "InitialFileLocation": FileLocationTypeDef,
         "ServiceMetadata": ServiceMetadataTypeDef,
         "ExecutionRole": str,
@@ -2437,35 +2452,36 @@
 )
 
 class DescribedWorkflowTypeDef(
     _RequiredDescribedWorkflowTypeDef, _OptionalDescribedWorkflowTypeDef
 ):
     pass
 
+WorkflowStepUnionTypeDef = Union[WorkflowStepTypeDef, WorkflowStepOutputTypeDef]
+DescribeWorkflowResponseTypeDef = TypedDict(
+    "DescribeWorkflowResponseTypeDef",
+    {
+        "Workflow": DescribedWorkflowTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateWorkflowRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWorkflowRequestRequestTypeDef",
     {
-        "Steps": Sequence[Union[WorkflowStepTypeDef, WorkflowStepOutputTypeDef]],
+        "Steps": Sequence[WorkflowStepUnionTypeDef],
     },
 )
 _OptionalCreateWorkflowRequestRequestTypeDef = TypedDict(
     "_OptionalCreateWorkflowRequestRequestTypeDef",
     {
         "Description": str,
-        "OnExceptionSteps": Sequence[Union[WorkflowStepTypeDef, WorkflowStepOutputTypeDef]],
+        "OnExceptionSteps": Sequence[WorkflowStepUnionTypeDef],
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
 class CreateWorkflowRequestRequestTypeDef(
     _RequiredCreateWorkflowRequestRequestTypeDef, _OptionalCreateWorkflowRequestRequestTypeDef
 ):
     pass
-
-DescribeWorkflowResponseTypeDef = TypedDict(
-    "DescribeWorkflowResponseTypeDef",
-    {
-        "Workflow": DescribedWorkflowTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
```

### Comparing `mypy-boto3-transfer-1.28.15.post1/mypy_boto3_transfer/waiter.py` & `mypy-boto3-transfer-1.28.16/mypy_boto3_transfer/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transfer-1.28.15.post1/mypy_boto3_transfer/waiter.pyi` & `mypy-boto3-transfer-1.28.16/mypy_boto3_transfer/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transfer-1.28.15.post1/mypy_boto3_transfer.egg-info/PKG-INFO` & `mypy-boto3-transfer-1.28.16/mypy_boto3_transfer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-transfer
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.Transfer 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.Transfer 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 transfer type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 transfer type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-transfer.svg?color=blue)](https://pypi.org/project/mypy-boto3-transfer)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-transfer)](https://pepy.tech/project/mypy-boto3-transfer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Transfer 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer)
+[boto3.Transfer 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer)
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
 [mypy-boto3-transfer docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/).
 
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
@@ -395,20 +395,20 @@
 )
 
 
 def check_value(value: AgreementStatusTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_transfer.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_transfer.type_defs import (
     As2ConnectorConfigTypeDef,
     HomeDirectoryMapEntryTypeDef,
     PosixProfileTypeDef,
     ResponseMetadataTypeDef,
@@ -447,14 +447,15 @@
     LoggingConfigurationTypeDef,
     EndpointDetailsOutputTypeDef,
     ProtocolDetailsOutputTypeDef,
     SshPublicKeyTypeDef,
     EfsFileLocationTypeDef,
     ExecutionErrorTypeDef,
     S3FileLocationTypeDef,
+    TimestampTypeDef,
     ImportSshPublicKeyRequestRequestTypeDef,
     S3InputFileLocationTypeDef,
     PaginatorConfigTypeDef,
     ListAccessesRequestRequestTypeDef,
     ListedAccessTypeDef,
     ListAgreementsRequestRequestTypeDef,
     ListedAgreementTypeDef,
@@ -481,15 +482,14 @@
     StartFileTransferRequestRequestTypeDef,
     StartServerRequestRequestTypeDef,
     StopServerRequestRequestTypeDef,
     TestConnectionRequestRequestTypeDef,
     TestIdentityProviderRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAgreementRequestRequestTypeDef,
-    UpdateCertificateRequestRequestTypeDef,
     UpdateHostKeyRequestRequestTypeDef,
     UpdateProfileRequestRequestTypeDef,
     WorkflowDetailTypeDef,
     CreateAccessRequestRequestTypeDef,
     UpdateAccessRequestRequestTypeDef,
     UpdateUserRequestRequestTypeDef,
     CreateAccessResponseTypeDef,
@@ -518,28 +518,33 @@
     CreateAgreementRequestRequestTypeDef,
     CreateProfileRequestRequestTypeDef,
     CreateUserRequestRequestTypeDef,
     DescribedAgreementTypeDef,
     DescribedCertificateTypeDef,
     DescribedHostKeyTypeDef,
     DescribedProfileTypeDef,
-    ImportCertificateRequestRequestTypeDef,
     ImportHostKeyRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateConnectorRequestRequestTypeDef,
     UpdateConnectorRequestRequestTypeDef,
     DescribeSecurityPolicyResponseTypeDef,
     DescribeServerRequestServerOfflineWaitTypeDef,
     DescribeServerRequestServerOnlineWaitTypeDef,
     DescribedAccessTypeDef,
+    PosixProfileUnionTypeDef,
     DescribedConnectorTypeDef,
+    SftpConnectorConfigUnionTypeDef,
+    EndpointDetailsUnionTypeDef,
+    ProtocolDetailsUnionTypeDef,
     DescribedUserTypeDef,
     ExecutionStepResultTypeDef,
     FileLocationTypeDef,
+    ImportCertificateRequestRequestTypeDef,
+    UpdateCertificateRequestRequestTypeDef,
     InputFileLocationTypeDef,
     ListAccessesRequestListAccessesPaginateTypeDef,
     ListAgreementsRequestListAgreementsPaginateTypeDef,
     ListCertificatesRequestListCertificatesPaginateTypeDef,
     ListConnectorsRequestListConnectorsPaginateTypeDef,
     ListExecutionsRequestListExecutionsPaginateTypeDef,
     ListProfilesRequestListProfilesPaginateTypeDef,
@@ -572,27 +577,29 @@
     ExecutionResultsTypeDef,
     CopyStepDetailsTypeDef,
     DecryptStepDetailsTypeDef,
     ListedExecutionTypeDef,
     DescribedServerTypeDef,
     CreateServerRequestRequestTypeDef,
     UpdateServerRequestRequestTypeDef,
+    WorkflowDetailsUnionTypeDef,
     DescribedExecutionTypeDef,
     WorkflowStepOutputTypeDef,
     WorkflowStepTypeDef,
     ListExecutionsResponseTypeDef,
     DescribeServerResponseTypeDef,
     DescribeExecutionResponseTypeDef,
     DescribedWorkflowTypeDef,
-    CreateWorkflowRequestRequestTypeDef,
+    WorkflowStepUnionTypeDef,
     DescribeWorkflowResponseTypeDef,
+    CreateWorkflowRequestRequestTypeDef,
 )
 
 
-def get_structure() -> As2ConnectorConfigTypeDef:
+def get_value() -> As2ConnectorConfigTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-transfer-1.28.15.post1/mypy_boto3_transfer.egg-info/SOURCES.txt` & `mypy-boto3-transfer-1.28.16/mypy_boto3_transfer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transfer-1.28.15.post1/setup.py` & `mypy-boto3-transfer-1.28.16/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-transfer",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_transfer"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Transfer 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.2"
+        "Type annotations for boto3.Transfer 1.28.16 service generated with mypy-boto3-builder"
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
-    keywords="boto3 transfer type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 transfer type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_transfer": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

