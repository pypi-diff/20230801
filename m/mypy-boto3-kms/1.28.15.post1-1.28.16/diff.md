# Comparing `tmp/mypy-boto3-kms-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-kms-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-kms-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:30 2023, max compression
+gzip compressed data, was "mypy-boto3-kms-1.28.16.tar", last modified: Tue Aug  1 11:37:10 2023, max compression
```

## Comparing `mypy-boto3-kms-1.28.15.post1.tar` & `mypy-boto3-kms-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:30.181230 mypy-boto3-kms-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:49:01.000000 mypy-boto3-kms-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17819 2023-07-29 10:03:30.181230 mypy-boto3-kms-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16342 2023-07-29 09:49:01.000000 mypy-boto3-kms-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:30.161230 mypy-boto3-kms-1.28.15.post1/mypy_boto3_kms/
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-07-29 09:49:01.000000 mypy-boto3-kms-1.28.15.post1/mypy_boto3_kms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-07-29 09:49:01.000000 mypy-boto3-kms-1.28.15.post1/mypy_boto3_kms/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-29 09:49:01.000000 mypy-boto3-kms-1.28.15.post1/mypy_boto3_kms/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41322 2023-07-29 09:49:01.000000 mypy-boto3-kms-1.28.15.post1/mypy_boto3_kms/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    41258 2023-07-29 09:49:01.000000 mypy-boto3-kms-1.28.15.post1/mypy_boto3_kms/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13021 2023-07-29 09:49:02.000000 mypy-boto3-kms-1.28.15.post1/mypy_boto3_kms/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13019 2023-07-29 09:49:02.000000 mypy-boto3-kms-1.28.15.post1/mypy_boto3_kms/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7983 2023-07-29 09:49:02.000000 mypy-boto3-kms-1.28.15.post1/mypy_boto3_kms/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7974 2023-07-29 09:49:02.000000 mypy-boto3-kms-1.28.15.post1/mypy_boto3_kms/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:49:01.000000 mypy-boto3-kms-1.28.15.post1/mypy_boto3_kms/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    41198 2023-07-29 09:49:05.000000 mypy-boto3-kms-1.28.15.post1/mypy_boto3_kms/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    41137 2023-07-29 09:49:02.000000 mypy-boto3-kms-1.28.15.post1/mypy_boto3_kms/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:49:01.000000 mypy-boto3-kms-1.28.15.post1/mypy_boto3_kms/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:30.181230 mypy-boto3-kms-1.28.15.post1/mypy_boto3_kms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17819 2023-07-29 10:03:29.000000 mypy-boto3-kms-1.28.15.post1/mypy_boto3_kms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-29 10:03:29.000000 mypy-boto3-kms-1.28.15.post1/mypy_boto3_kms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:29.000000 mypy-boto3-kms-1.28.15.post1/mypy_boto3_kms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:29.000000 mypy-boto3-kms-1.28.15.post1/mypy_boto3_kms.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:29.000000 mypy-boto3-kms-1.28.15.post1/mypy_boto3_kms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-29 10:03:29.000000 mypy-boto3-kms-1.28.15.post1/mypy_boto3_kms.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:30.181230 mypy-boto3-kms-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-29 09:49:01.000000 mypy-boto3-kms-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:10.040845 mypy-boto3-kms-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:21:51.000000 mypy-boto3-kms-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17882 2023-08-01 11:37:10.040845 mypy-boto3-kms-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16414 2023-08-01 11:21:51.000000 mypy-boto3-kms-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:10.024845 mypy-boto3-kms-1.28.16/mypy_boto3_kms/
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-08-01 11:21:51.000000 mypy-boto3-kms-1.28.16/mypy_boto3_kms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-08-01 11:21:51.000000 mypy-boto3-kms-1.28.16/mypy_boto3_kms/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-08-01 11:21:51.000000 mypy-boto3-kms-1.28.16/mypy_boto3_kms/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40879 2023-08-01 11:21:51.000000 mypy-boto3-kms-1.28.16/mypy_boto3_kms/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40815 2023-08-01 11:21:51.000000 mypy-boto3-kms-1.28.16/mypy_boto3_kms/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13021 2023-08-01 11:21:52.000000 mypy-boto3-kms-1.28.16/mypy_boto3_kms/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13019 2023-08-01 11:21:52.000000 mypy-boto3-kms-1.28.16/mypy_boto3_kms/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7983 2023-08-01 11:21:51.000000 mypy-boto3-kms-1.28.16/mypy_boto3_kms/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7974 2023-08-01 11:21:51.000000 mypy-boto3-kms-1.28.16/mypy_boto3_kms/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:21:51.000000 mypy-boto3-kms-1.28.16/mypy_boto3_kms/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    41100 2023-08-01 11:21:53.000000 mypy-boto3-kms-1.28.16/mypy_boto3_kms/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41039 2023-08-01 11:21:52.000000 mypy-boto3-kms-1.28.16/mypy_boto3_kms/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:21:51.000000 mypy-boto3-kms-1.28.16/mypy_boto3_kms/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:10.040845 mypy-boto3-kms-1.28.16/mypy_boto3_kms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17882 2023-08-01 11:37:09.000000 mypy-boto3-kms-1.28.16/mypy_boto3_kms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-08-01 11:37:09.000000 mypy-boto3-kms-1.28.16/mypy_boto3_kms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:09.000000 mypy-boto3-kms-1.28.16/mypy_boto3_kms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:09.000000 mypy-boto3-kms-1.28.16/mypy_boto3_kms.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:09.000000 mypy-boto3-kms-1.28.16/mypy_boto3_kms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-01 11:37:09.000000 mypy-boto3-kms-1.28.16/mypy_boto3_kms.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:10.040845 mypy-boto3-kms-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-08-01 11:21:51.000000 mypy-boto3-kms-1.28.16/setup.py
```

### Comparing `mypy-boto3-kms-1.28.15.post1/LICENSE` & `mypy-boto3-kms-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kms-1.28.15.post1/PKG-INFO` & `mypy-boto3-kms-1.28.16/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-kms
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.KMS 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.KMS 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 kms type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 kms type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kms.svg?color=blue)](https://pypi.org/project/mypy-boto3-kms)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-kms)](https://pepy.tech/project/mypy-boto3-kms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.KMS 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS)
+[boto3.KMS 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS)
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
 [mypy-boto3-kms docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/).
 
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
@@ -354,73 +354,74 @@
 )
 
 
 def check_value(value: AlgorithmSpecType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_kms.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_kms.type_defs import (
     AliasListEntryTypeDef,
+    BlobTypeDef,
     CancelKeyDeletionRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     ConnectCustomKeyStoreRequestRequestTypeDef,
     CreateAliasRequestRequestTypeDef,
     XksProxyAuthenticationCredentialTypeTypeDef,
     GrantConstraintsTypeDef,
     TagTypeDef,
     XksProxyConfigurationTypeTypeDef,
-    RecipientInfoTypeDef,
     DeleteAliasRequestRequestTypeDef,
     DeleteCustomKeyStoreRequestRequestTypeDef,
     DeleteImportedKeyMaterialRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     DescribeCustomKeyStoresRequestRequestTypeDef,
     DescribeKeyRequestRequestTypeDef,
     DisableKeyRequestRequestTypeDef,
     DisableKeyRotationRequestRequestTypeDef,
     DisconnectCustomKeyStoreRequestRequestTypeDef,
     EnableKeyRequestRequestTypeDef,
     EnableKeyRotationRequestRequestTypeDef,
-    EncryptRequestRequestTypeDef,
     GenerateDataKeyPairWithoutPlaintextRequestRequestTypeDef,
     GenerateDataKeyWithoutPlaintextRequestRequestTypeDef,
-    GenerateMacRequestRequestTypeDef,
     GetKeyPolicyRequestRequestTypeDef,
     GetKeyRotationStatusRequestRequestTypeDef,
     GetParametersForImportRequestRequestTypeDef,
     GetPublicKeyRequestRequestTypeDef,
     GrantConstraintsOutputTypeDef,
-    ImportKeyMaterialRequestRequestTypeDef,
+    TimestampTypeDef,
     KeyListEntryTypeDef,
     XksKeyConfigurationTypeTypeDef,
     ListAliasesRequestRequestTypeDef,
     ListGrantsRequestRequestTypeDef,
     ListKeyPoliciesRequestRequestTypeDef,
     ListKeysRequestRequestTypeDef,
     ListResourceTagsRequestRequestTypeDef,
     ListRetirableGrantsRequestRequestTypeDef,
     MultiRegionKeyTypeDef,
     PutKeyPolicyRequestRequestTypeDef,
-    ReEncryptRequestRequestTypeDef,
     RetireGrantRequestRequestTypeDef,
     RevokeGrantRequestRequestTypeDef,
     ScheduleKeyDeletionRequestRequestTypeDef,
-    SignRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAliasRequestRequestTypeDef,
     UpdateKeyDescriptionRequestRequestTypeDef,
     UpdatePrimaryRegionRequestRequestTypeDef,
+    EncryptRequestRequestTypeDef,
+    GenerateMacRequestRequestTypeDef,
+    ReEncryptRequestRequestTypeDef,
+    RecipientInfoTypeDef,
+    SignRequestRequestTypeDef,
     VerifyMacRequestRequestTypeDef,
     VerifyRequestRequestTypeDef,
     CancelKeyDeletionResponseTypeDef,
     CreateCustomKeyStoreResponseTypeDef,
     CreateGrantResponseTypeDef,
     DecryptResponseTypeDef,
     EmptyResponseMetadataTypeDef,
@@ -446,38 +447,40 @@
     UpdateCustomKeyStoreRequestRequestTypeDef,
     CreateGrantRequestRequestTypeDef,
     CreateKeyRequestRequestTypeDef,
     ListResourceTagsResponseTypeDef,
     ReplicateKeyRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     CustomKeyStoresListEntryTypeDef,
-    DecryptRequestRequestTypeDef,
-    GenerateDataKeyPairRequestRequestTypeDef,
-    GenerateDataKeyRequestRequestTypeDef,
-    GenerateRandomRequestRequestTypeDef,
     DescribeCustomKeyStoresRequestDescribeCustomKeyStoresPaginateTypeDef,
     ListAliasesRequestListAliasesPaginateTypeDef,
     ListGrantsRequestListGrantsPaginateTypeDef,
     ListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef,
     ListKeysRequestListKeysPaginateTypeDef,
     ListResourceTagsRequestListResourceTagsPaginateTypeDef,
     ListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef,
+    GrantConstraintsUnionTypeDef,
     GrantListEntryTypeDef,
+    ImportKeyMaterialRequestRequestTypeDef,
     ListKeysResponseTypeDef,
     MultiRegionConfigurationTypeDef,
+    DecryptRequestRequestTypeDef,
+    GenerateDataKeyPairRequestRequestTypeDef,
+    GenerateDataKeyRequestRequestTypeDef,
+    GenerateRandomRequestRequestTypeDef,
     DescribeCustomKeyStoresResponseTypeDef,
     ListGrantsResponseTypeDef,
     KeyMetadataTypeDef,
     CreateKeyResponseTypeDef,
     DescribeKeyResponseTypeDef,
     ReplicateKeyResponseTypeDef,
 )
 
 
-def get_structure() -> AliasListEntryTypeDef:
+def get_value() -> AliasListEntryTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-kms-1.28.15.post1/README.md` & `mypy-boto3-kms-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kms.svg?color=blue)](https://pypi.org/project/mypy-boto3-kms)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-kms)](https://pepy.tech/project/mypy-boto3-kms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.KMS 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS)
+[boto3.KMS 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS)
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
 [mypy-boto3-kms docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/).
 
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
@@ -322,73 +322,74 @@
 )
 
 
 def check_value(value: AlgorithmSpecType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_kms.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_kms.type_defs import (
     AliasListEntryTypeDef,
+    BlobTypeDef,
     CancelKeyDeletionRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     ConnectCustomKeyStoreRequestRequestTypeDef,
     CreateAliasRequestRequestTypeDef,
     XksProxyAuthenticationCredentialTypeTypeDef,
     GrantConstraintsTypeDef,
     TagTypeDef,
     XksProxyConfigurationTypeTypeDef,
-    RecipientInfoTypeDef,
     DeleteAliasRequestRequestTypeDef,
     DeleteCustomKeyStoreRequestRequestTypeDef,
     DeleteImportedKeyMaterialRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     DescribeCustomKeyStoresRequestRequestTypeDef,
     DescribeKeyRequestRequestTypeDef,
     DisableKeyRequestRequestTypeDef,
     DisableKeyRotationRequestRequestTypeDef,
     DisconnectCustomKeyStoreRequestRequestTypeDef,
     EnableKeyRequestRequestTypeDef,
     EnableKeyRotationRequestRequestTypeDef,
-    EncryptRequestRequestTypeDef,
     GenerateDataKeyPairWithoutPlaintextRequestRequestTypeDef,
     GenerateDataKeyWithoutPlaintextRequestRequestTypeDef,
-    GenerateMacRequestRequestTypeDef,
     GetKeyPolicyRequestRequestTypeDef,
     GetKeyRotationStatusRequestRequestTypeDef,
     GetParametersForImportRequestRequestTypeDef,
     GetPublicKeyRequestRequestTypeDef,
     GrantConstraintsOutputTypeDef,
-    ImportKeyMaterialRequestRequestTypeDef,
+    TimestampTypeDef,
     KeyListEntryTypeDef,
     XksKeyConfigurationTypeTypeDef,
     ListAliasesRequestRequestTypeDef,
     ListGrantsRequestRequestTypeDef,
     ListKeyPoliciesRequestRequestTypeDef,
     ListKeysRequestRequestTypeDef,
     ListResourceTagsRequestRequestTypeDef,
     ListRetirableGrantsRequestRequestTypeDef,
     MultiRegionKeyTypeDef,
     PutKeyPolicyRequestRequestTypeDef,
-    ReEncryptRequestRequestTypeDef,
     RetireGrantRequestRequestTypeDef,
     RevokeGrantRequestRequestTypeDef,
     ScheduleKeyDeletionRequestRequestTypeDef,
-    SignRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAliasRequestRequestTypeDef,
     UpdateKeyDescriptionRequestRequestTypeDef,
     UpdatePrimaryRegionRequestRequestTypeDef,
+    EncryptRequestRequestTypeDef,
+    GenerateMacRequestRequestTypeDef,
+    ReEncryptRequestRequestTypeDef,
+    RecipientInfoTypeDef,
+    SignRequestRequestTypeDef,
     VerifyMacRequestRequestTypeDef,
     VerifyRequestRequestTypeDef,
     CancelKeyDeletionResponseTypeDef,
     CreateCustomKeyStoreResponseTypeDef,
     CreateGrantResponseTypeDef,
     DecryptResponseTypeDef,
     EmptyResponseMetadataTypeDef,
@@ -414,38 +415,40 @@
     UpdateCustomKeyStoreRequestRequestTypeDef,
     CreateGrantRequestRequestTypeDef,
     CreateKeyRequestRequestTypeDef,
     ListResourceTagsResponseTypeDef,
     ReplicateKeyRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     CustomKeyStoresListEntryTypeDef,
-    DecryptRequestRequestTypeDef,
-    GenerateDataKeyPairRequestRequestTypeDef,
-    GenerateDataKeyRequestRequestTypeDef,
-    GenerateRandomRequestRequestTypeDef,
     DescribeCustomKeyStoresRequestDescribeCustomKeyStoresPaginateTypeDef,
     ListAliasesRequestListAliasesPaginateTypeDef,
     ListGrantsRequestListGrantsPaginateTypeDef,
     ListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef,
     ListKeysRequestListKeysPaginateTypeDef,
     ListResourceTagsRequestListResourceTagsPaginateTypeDef,
     ListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef,
+    GrantConstraintsUnionTypeDef,
     GrantListEntryTypeDef,
+    ImportKeyMaterialRequestRequestTypeDef,
     ListKeysResponseTypeDef,
     MultiRegionConfigurationTypeDef,
+    DecryptRequestRequestTypeDef,
+    GenerateDataKeyPairRequestRequestTypeDef,
+    GenerateDataKeyRequestRequestTypeDef,
+    GenerateRandomRequestRequestTypeDef,
     DescribeCustomKeyStoresResponseTypeDef,
     ListGrantsResponseTypeDef,
     KeyMetadataTypeDef,
     CreateKeyResponseTypeDef,
     DescribeKeyResponseTypeDef,
     ReplicateKeyResponseTypeDef,
 )
 
 
-def get_structure() -> AliasListEntryTypeDef:
+def get_value() -> AliasListEntryTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-kms-1.28.15.post1/mypy_boto3_kms/__init__.py` & `mypy-boto3-kms-1.28.16/mypy_boto3_kms/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kms-1.28.15.post1/mypy_boto3_kms/__init__.pyi` & `mypy-boto3-kms-1.28.16/mypy_boto3_kms/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kms-1.28.15.post1/mypy_boto3_kms/__main__.py` & `mypy-boto3-kms-1.28.16/mypy_boto3_kms/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.KMS 1.28.15\nVersion:         1.28.15.post1\nBuilder version:"
-        " 7.16.2\nDocs:           "
+        "Type annotations for boto3.KMS 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS\nOther"
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

### Comparing `mypy-boto3-kms-1.28.15.post1/mypy_boto3_kms/client.py` & `mypy-boto3-kms-1.28.16/mypy_boto3_kms/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,19 +10,17 @@
     from mypy_boto3_kms.client import KMSClient
 
     session = Session()
     client: KMSClient = session.client("kms")
     ```
 """
 import sys
-from datetime import datetime
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
-from botocore.response import StreamingBody
 
 from .literals import (
     AlgorithmSpecType,
     CustomerMasterKeySpecType,
     CustomKeyStoreTypeType,
     DataKeyPairSpecType,
     DataKeySpecType,
@@ -44,14 +42,15 @@
     ListGrantsPaginator,
     ListKeyPoliciesPaginator,
     ListKeysPaginator,
     ListResourceTagsPaginator,
     ListRetirableGrantsPaginator,
 )
 from .type_defs import (
+    BlobTypeDef,
     CancelKeyDeletionResponseTypeDef,
     CreateCustomKeyStoreResponseTypeDef,
     CreateGrantResponseTypeDef,
     CreateKeyResponseTypeDef,
     DecryptResponseTypeDef,
     DescribeCustomKeyStoresResponseTypeDef,
     DescribeKeyResponseTypeDef,
@@ -63,27 +62,27 @@
     GenerateDataKeyWithoutPlaintextResponseTypeDef,
     GenerateMacResponseTypeDef,
     GenerateRandomResponseTypeDef,
     GetKeyPolicyResponseTypeDef,
     GetKeyRotationStatusResponseTypeDef,
     GetParametersForImportResponseTypeDef,
     GetPublicKeyResponseTypeDef,
-    GrantConstraintsOutputTypeDef,
-    GrantConstraintsTypeDef,
+    GrantConstraintsUnionTypeDef,
     ListAliasesResponseTypeDef,
     ListGrantsResponseTypeDef,
     ListKeyPoliciesResponseTypeDef,
     ListKeysResponseTypeDef,
     ListResourceTagsResponseTypeDef,
     RecipientInfoTypeDef,
     ReEncryptResponseTypeDef,
     ReplicateKeyResponseTypeDef,
     ScheduleKeyDeletionResponseTypeDef,
     SignResponseTypeDef,
     TagTypeDef,
+    TimestampTypeDef,
     VerifyMacResponseTypeDef,
     VerifyResponseTypeDef,
     XksProxyAuthenticationCredentialTypeTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
@@ -238,15 +237,15 @@
     def create_grant(
         self,
         *,
         KeyId: str,
         GranteePrincipal: str,
         Operations: Sequence[GrantOperationType],
         RetiringPrincipal: str = ...,
-        Constraints: Union[GrantConstraintsTypeDef, GrantConstraintsOutputTypeDef] = ...,
+        Constraints: GrantConstraintsUnionTypeDef = ...,
         GrantTokens: Sequence[str] = ...,
         Name: str = ...,
         DryRun: bool = ...
     ) -> CreateGrantResponseTypeDef:
         """
         Adds a grant to a KMS key.
 
@@ -277,15 +276,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.create_key)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#create_key)
         """
 
     def decrypt(
         self,
         *,
-        CiphertextBlob: Union[str, bytes, IO[Any], StreamingBody],
+        CiphertextBlob: BlobTypeDef,
         EncryptionContext: Mapping[str, str] = ...,
         GrantTokens: Sequence[str] = ...,
         KeyId: str = ...,
         EncryptionAlgorithm: EncryptionAlgorithmSpecType = ...,
         Recipient: RecipientInfoTypeDef = ...,
         DryRun: bool = ...
     ) -> DecryptResponseTypeDef:
@@ -398,15 +397,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#enable_key_rotation)
         """
 
     def encrypt(
         self,
         *,
         KeyId: str,
-        Plaintext: Union[str, bytes, IO[Any], StreamingBody],
+        Plaintext: BlobTypeDef,
         EncryptionContext: Mapping[str, str] = ...,
         GrantTokens: Sequence[str] = ...,
         EncryptionAlgorithm: EncryptionAlgorithmSpecType = ...,
         DryRun: bool = ...
     ) -> EncryptResponseTypeDef:
         """
         Encrypts plaintext of up to 4,096 bytes using a KMS key.
@@ -482,15 +481,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.generate_data_key_without_plaintext)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#generate_data_key_without_plaintext)
         """
 
     def generate_mac(
         self,
         *,
-        Message: Union[str, bytes, IO[Any], StreamingBody],
+        Message: BlobTypeDef,
         KeyId: str,
         MacAlgorithm: MacAlgorithmSpecType,
         GrantTokens: Sequence[str] = ...,
         DryRun: bool = ...
     ) -> GenerateMacResponseTypeDef:
         """
         Generates a hash-based message authentication code (HMAC) for a message using an
@@ -571,17 +570,17 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#get_public_key)
         """
 
     def import_key_material(
         self,
         *,
         KeyId: str,
-        ImportToken: Union[str, bytes, IO[Any], StreamingBody],
-        EncryptedKeyMaterial: Union[str, bytes, IO[Any], StreamingBody],
-        ValidTo: Union[datetime, str] = ...,
+        ImportToken: BlobTypeDef,
+        EncryptedKeyMaterial: BlobTypeDef,
+        ValidTo: TimestampTypeDef = ...,
         ExpirationModel: ExpirationModelTypeType = ...
     ) -> Dict[str, Any]:
         """
         Imports or reimports key material into an existing KMS key that was created
         without key material.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.import_key_material)
@@ -668,15 +667,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.put_key_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#put_key_policy)
         """
 
     def re_encrypt(
         self,
         *,
-        CiphertextBlob: Union[str, bytes, IO[Any], StreamingBody],
+        CiphertextBlob: BlobTypeDef,
         DestinationKeyId: str,
         SourceEncryptionContext: Mapping[str, str] = ...,
         SourceKeyId: str = ...,
         DestinationEncryptionContext: Mapping[str, str] = ...,
         SourceEncryptionAlgorithm: EncryptionAlgorithmSpecType = ...,
         DestinationEncryptionAlgorithm: EncryptionAlgorithmSpecType = ...,
         GrantTokens: Sequence[str] = ...,
@@ -736,15 +735,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#schedule_key_deletion)
         """
 
     def sign(
         self,
         *,
         KeyId: str,
-        Message: Union[str, bytes, IO[Any], StreamingBody],
+        Message: BlobTypeDef,
         SigningAlgorithm: SigningAlgorithmSpecType,
         MessageType: MessageTypeType = ...,
         GrantTokens: Sequence[str] = ...,
         DryRun: bool = ...
     ) -> SignResponseTypeDef:
         """
         Creates a [digital signature](https://en.wikipedia.org/wiki/Digital_signature)_
@@ -825,16 +824,16 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#update_primary_region)
         """
 
     def verify(
         self,
         *,
         KeyId: str,
-        Message: Union[str, bytes, IO[Any], StreamingBody],
-        Signature: Union[str, bytes, IO[Any], StreamingBody],
+        Message: BlobTypeDef,
+        Signature: BlobTypeDef,
         SigningAlgorithm: SigningAlgorithmSpecType,
         MessageType: MessageTypeType = ...,
         GrantTokens: Sequence[str] = ...,
         DryRun: bool = ...
     ) -> VerifyResponseTypeDef:
         """
         Verifies a digital signature that was generated by the  Sign operation.
@@ -842,18 +841,18 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.verify)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#verify)
         """
 
     def verify_mac(
         self,
         *,
-        Message: Union[str, bytes, IO[Any], StreamingBody],
+        Message: BlobTypeDef,
         KeyId: str,
         MacAlgorithm: MacAlgorithmSpecType,
-        Mac: Union[str, bytes, IO[Any], StreamingBody],
+        Mac: BlobTypeDef,
         GrantTokens: Sequence[str] = ...,
         DryRun: bool = ...
     ) -> VerifyMacResponseTypeDef:
         """
         Verifies the hash-based message authentication code (HMAC) for a specified
         message, HMAC KMS key, and MAC algorithm.
```

### Comparing `mypy-boto3-kms-1.28.15.post1/mypy_boto3_kms/client.pyi` & `mypy-boto3-kms-1.28.16/mypy_boto3_kms/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -10,19 +10,17 @@
     from mypy_boto3_kms.client import KMSClient
 
     session = Session()
     client: KMSClient = session.client("kms")
     ```
 """
 import sys
-from datetime import datetime
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
-from botocore.response import StreamingBody
 
 from .literals import (
     AlgorithmSpecType,
     CustomerMasterKeySpecType,
     CustomKeyStoreTypeType,
     DataKeyPairSpecType,
     DataKeySpecType,
@@ -44,14 +42,15 @@
     ListGrantsPaginator,
     ListKeyPoliciesPaginator,
     ListKeysPaginator,
     ListResourceTagsPaginator,
     ListRetirableGrantsPaginator,
 )
 from .type_defs import (
+    BlobTypeDef,
     CancelKeyDeletionResponseTypeDef,
     CreateCustomKeyStoreResponseTypeDef,
     CreateGrantResponseTypeDef,
     CreateKeyResponseTypeDef,
     DecryptResponseTypeDef,
     DescribeCustomKeyStoresResponseTypeDef,
     DescribeKeyResponseTypeDef,
@@ -63,27 +62,27 @@
     GenerateDataKeyWithoutPlaintextResponseTypeDef,
     GenerateMacResponseTypeDef,
     GenerateRandomResponseTypeDef,
     GetKeyPolicyResponseTypeDef,
     GetKeyRotationStatusResponseTypeDef,
     GetParametersForImportResponseTypeDef,
     GetPublicKeyResponseTypeDef,
-    GrantConstraintsOutputTypeDef,
-    GrantConstraintsTypeDef,
+    GrantConstraintsUnionTypeDef,
     ListAliasesResponseTypeDef,
     ListGrantsResponseTypeDef,
     ListKeyPoliciesResponseTypeDef,
     ListKeysResponseTypeDef,
     ListResourceTagsResponseTypeDef,
     RecipientInfoTypeDef,
     ReEncryptResponseTypeDef,
     ReplicateKeyResponseTypeDef,
     ScheduleKeyDeletionResponseTypeDef,
     SignResponseTypeDef,
     TagTypeDef,
+    TimestampTypeDef,
     VerifyMacResponseTypeDef,
     VerifyResponseTypeDef,
     XksProxyAuthenticationCredentialTypeTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
@@ -227,15 +226,15 @@
     def create_grant(
         self,
         *,
         KeyId: str,
         GranteePrincipal: str,
         Operations: Sequence[GrantOperationType],
         RetiringPrincipal: str = ...,
-        Constraints: Union[GrantConstraintsTypeDef, GrantConstraintsOutputTypeDef] = ...,
+        Constraints: GrantConstraintsUnionTypeDef = ...,
         GrantTokens: Sequence[str] = ...,
         Name: str = ...,
         DryRun: bool = ...
     ) -> CreateGrantResponseTypeDef:
         """
         Adds a grant to a KMS key.
 
@@ -264,15 +263,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.create_key)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#create_key)
         """
     def decrypt(
         self,
         *,
-        CiphertextBlob: Union[str, bytes, IO[Any], StreamingBody],
+        CiphertextBlob: BlobTypeDef,
         EncryptionContext: Mapping[str, str] = ...,
         GrantTokens: Sequence[str] = ...,
         KeyId: str = ...,
         EncryptionAlgorithm: EncryptionAlgorithmSpecType = ...,
         Recipient: RecipientInfoTypeDef = ...,
         DryRun: bool = ...
     ) -> DecryptResponseTypeDef:
@@ -374,15 +373,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.enable_key_rotation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#enable_key_rotation)
         """
     def encrypt(
         self,
         *,
         KeyId: str,
-        Plaintext: Union[str, bytes, IO[Any], StreamingBody],
+        Plaintext: BlobTypeDef,
         EncryptionContext: Mapping[str, str] = ...,
         GrantTokens: Sequence[str] = ...,
         EncryptionAlgorithm: EncryptionAlgorithmSpecType = ...,
         DryRun: bool = ...
     ) -> EncryptResponseTypeDef:
         """
         Encrypts plaintext of up to 4,096 bytes using a KMS key.
@@ -453,15 +452,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.generate_data_key_without_plaintext)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#generate_data_key_without_plaintext)
         """
     def generate_mac(
         self,
         *,
-        Message: Union[str, bytes, IO[Any], StreamingBody],
+        Message: BlobTypeDef,
         KeyId: str,
         MacAlgorithm: MacAlgorithmSpecType,
         GrantTokens: Sequence[str] = ...,
         DryRun: bool = ...
     ) -> GenerateMacResponseTypeDef:
         """
         Generates a hash-based message authentication code (HMAC) for a message using an
@@ -535,17 +534,17 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.get_public_key)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#get_public_key)
         """
     def import_key_material(
         self,
         *,
         KeyId: str,
-        ImportToken: Union[str, bytes, IO[Any], StreamingBody],
-        EncryptedKeyMaterial: Union[str, bytes, IO[Any], StreamingBody],
-        ValidTo: Union[datetime, str] = ...,
+        ImportToken: BlobTypeDef,
+        EncryptedKeyMaterial: BlobTypeDef,
+        ValidTo: TimestampTypeDef = ...,
         ExpirationModel: ExpirationModelTypeType = ...
     ) -> Dict[str, Any]:
         """
         Imports or reimports key material into an existing KMS key that was created
         without key material.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.import_key_material)
@@ -624,15 +623,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.put_key_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#put_key_policy)
         """
     def re_encrypt(
         self,
         *,
-        CiphertextBlob: Union[str, bytes, IO[Any], StreamingBody],
+        CiphertextBlob: BlobTypeDef,
         DestinationKeyId: str,
         SourceEncryptionContext: Mapping[str, str] = ...,
         SourceKeyId: str = ...,
         DestinationEncryptionContext: Mapping[str, str] = ...,
         SourceEncryptionAlgorithm: EncryptionAlgorithmSpecType = ...,
         DestinationEncryptionAlgorithm: EncryptionAlgorithmSpecType = ...,
         GrantTokens: Sequence[str] = ...,
@@ -687,15 +686,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.schedule_key_deletion)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#schedule_key_deletion)
         """
     def sign(
         self,
         *,
         KeyId: str,
-        Message: Union[str, bytes, IO[Any], StreamingBody],
+        Message: BlobTypeDef,
         SigningAlgorithm: SigningAlgorithmSpecType,
         MessageType: MessageTypeType = ...,
         GrantTokens: Sequence[str] = ...,
         DryRun: bool = ...
     ) -> SignResponseTypeDef:
         """
         Creates a [digital signature](https://en.wikipedia.org/wiki/Digital_signature)_
@@ -769,34 +768,34 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.update_primary_region)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#update_primary_region)
         """
     def verify(
         self,
         *,
         KeyId: str,
-        Message: Union[str, bytes, IO[Any], StreamingBody],
-        Signature: Union[str, bytes, IO[Any], StreamingBody],
+        Message: BlobTypeDef,
+        Signature: BlobTypeDef,
         SigningAlgorithm: SigningAlgorithmSpecType,
         MessageType: MessageTypeType = ...,
         GrantTokens: Sequence[str] = ...,
         DryRun: bool = ...
     ) -> VerifyResponseTypeDef:
         """
         Verifies a digital signature that was generated by the  Sign operation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.verify)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#verify)
         """
     def verify_mac(
         self,
         *,
-        Message: Union[str, bytes, IO[Any], StreamingBody],
+        Message: BlobTypeDef,
         KeyId: str,
         MacAlgorithm: MacAlgorithmSpecType,
-        Mac: Union[str, bytes, IO[Any], StreamingBody],
+        Mac: BlobTypeDef,
         GrantTokens: Sequence[str] = ...,
         DryRun: bool = ...
     ) -> VerifyMacResponseTypeDef:
         """
         Verifies the hash-based message authentication code (HMAC) for a specified
         message, HMAC KMS key, and MAC algorithm.
```

### Comparing `mypy-boto3-kms-1.28.15.post1/mypy_boto3_kms/literals.py` & `mypy-boto3-kms-1.28.16/mypy_boto3_kms/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kms-1.28.15.post1/mypy_boto3_kms/literals.pyi` & `mypy-boto3-kms-1.28.16/mypy_boto3_kms/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kms-1.28.15.post1/mypy_boto3_kms/paginator.py` & `mypy-boto3-kms-1.28.16/mypy_boto3_kms/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kms-1.28.15.post1/mypy_boto3_kms/paginator.pyi` & `mypy-boto3-kms-1.28.16/mypy_boto3_kms/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kms-1.28.15.post1/mypy_boto3_kms/type_defs.py` & `mypy-boto3-kms-1.28.16/mypy_boto3_kms/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_kms.type_defs import AliasListEntryTypeDef
 
-    data: AliasListEntryTypeDef = {...}
+    data: AliasListEntryTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -49,63 +49,64 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AliasListEntryTypeDef",
+    "BlobTypeDef",
     "CancelKeyDeletionRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "ConnectCustomKeyStoreRequestRequestTypeDef",
     "CreateAliasRequestRequestTypeDef",
     "XksProxyAuthenticationCredentialTypeTypeDef",
     "GrantConstraintsTypeDef",
     "TagTypeDef",
     "XksProxyConfigurationTypeTypeDef",
-    "RecipientInfoTypeDef",
     "DeleteAliasRequestRequestTypeDef",
     "DeleteCustomKeyStoreRequestRequestTypeDef",
     "DeleteImportedKeyMaterialRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "DescribeCustomKeyStoresRequestRequestTypeDef",
     "DescribeKeyRequestRequestTypeDef",
     "DisableKeyRequestRequestTypeDef",
     "DisableKeyRotationRequestRequestTypeDef",
     "DisconnectCustomKeyStoreRequestRequestTypeDef",
     "EnableKeyRequestRequestTypeDef",
     "EnableKeyRotationRequestRequestTypeDef",
-    "EncryptRequestRequestTypeDef",
     "GenerateDataKeyPairWithoutPlaintextRequestRequestTypeDef",
     "GenerateDataKeyWithoutPlaintextRequestRequestTypeDef",
-    "GenerateMacRequestRequestTypeDef",
     "GetKeyPolicyRequestRequestTypeDef",
     "GetKeyRotationStatusRequestRequestTypeDef",
     "GetParametersForImportRequestRequestTypeDef",
     "GetPublicKeyRequestRequestTypeDef",
     "GrantConstraintsOutputTypeDef",
-    "ImportKeyMaterialRequestRequestTypeDef",
+    "TimestampTypeDef",
     "KeyListEntryTypeDef",
     "XksKeyConfigurationTypeTypeDef",
     "ListAliasesRequestRequestTypeDef",
     "ListGrantsRequestRequestTypeDef",
     "ListKeyPoliciesRequestRequestTypeDef",
     "ListKeysRequestRequestTypeDef",
     "ListResourceTagsRequestRequestTypeDef",
     "ListRetirableGrantsRequestRequestTypeDef",
     "MultiRegionKeyTypeDef",
     "PutKeyPolicyRequestRequestTypeDef",
-    "ReEncryptRequestRequestTypeDef",
     "RetireGrantRequestRequestTypeDef",
     "RevokeGrantRequestRequestTypeDef",
     "ScheduleKeyDeletionRequestRequestTypeDef",
-    "SignRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAliasRequestRequestTypeDef",
     "UpdateKeyDescriptionRequestRequestTypeDef",
     "UpdatePrimaryRegionRequestRequestTypeDef",
+    "EncryptRequestRequestTypeDef",
+    "GenerateMacRequestRequestTypeDef",
+    "ReEncryptRequestRequestTypeDef",
+    "RecipientInfoTypeDef",
+    "SignRequestRequestTypeDef",
     "VerifyMacRequestRequestTypeDef",
     "VerifyRequestRequestTypeDef",
     "CancelKeyDeletionResponseTypeDef",
     "CreateCustomKeyStoreResponseTypeDef",
     "CreateGrantResponseTypeDef",
     "DecryptResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
@@ -131,28 +132,30 @@
     "UpdateCustomKeyStoreRequestRequestTypeDef",
     "CreateGrantRequestRequestTypeDef",
     "CreateKeyRequestRequestTypeDef",
     "ListResourceTagsResponseTypeDef",
     "ReplicateKeyRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CustomKeyStoresListEntryTypeDef",
-    "DecryptRequestRequestTypeDef",
-    "GenerateDataKeyPairRequestRequestTypeDef",
-    "GenerateDataKeyRequestRequestTypeDef",
-    "GenerateRandomRequestRequestTypeDef",
     "DescribeCustomKeyStoresRequestDescribeCustomKeyStoresPaginateTypeDef",
     "ListAliasesRequestListAliasesPaginateTypeDef",
     "ListGrantsRequestListGrantsPaginateTypeDef",
     "ListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef",
     "ListKeysRequestListKeysPaginateTypeDef",
     "ListResourceTagsRequestListResourceTagsPaginateTypeDef",
     "ListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef",
+    "GrantConstraintsUnionTypeDef",
     "GrantListEntryTypeDef",
+    "ImportKeyMaterialRequestRequestTypeDef",
     "ListKeysResponseTypeDef",
     "MultiRegionConfigurationTypeDef",
+    "DecryptRequestRequestTypeDef",
+    "GenerateDataKeyPairRequestRequestTypeDef",
+    "GenerateDataKeyRequestRequestTypeDef",
+    "GenerateRandomRequestRequestTypeDef",
     "DescribeCustomKeyStoresResponseTypeDef",
     "ListGrantsResponseTypeDef",
     "KeyMetadataTypeDef",
     "CreateKeyResponseTypeDef",
     "DescribeKeyResponseTypeDef",
     "ReplicateKeyResponseTypeDef",
 )
@@ -165,14 +168,15 @@
         "TargetKeyId": str,
         "CreationDate": datetime,
         "LastUpdatedDate": datetime,
     },
     total=False,
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 CancelKeyDeletionRequestRequestTypeDef = TypedDict(
     "CancelKeyDeletionRequestRequestTypeDef",
     {
         "KeyId": str,
     },
 )
 
@@ -235,23 +239,14 @@
         "UriEndpoint": str,
         "UriPath": str,
         "VpcEndpointServiceName": str,
     },
     total=False,
 )
 
-RecipientInfoTypeDef = TypedDict(
-    "RecipientInfoTypeDef",
-    {
-        "KeyEncryptionAlgorithm": Literal["RSAES_OAEP_SHA_256"],
-        "AttestationDocument": Union[str, bytes, IO[Any], StreamingBody],
-    },
-    total=False,
-)
-
 DeleteAliasRequestRequestTypeDef = TypedDict(
     "DeleteAliasRequestRequestTypeDef",
     {
         "AliasName": str,
     },
 )
 
@@ -342,39 +337,14 @@
 EnableKeyRotationRequestRequestTypeDef = TypedDict(
     "EnableKeyRotationRequestRequestTypeDef",
     {
         "KeyId": str,
     },
 )
 
-_RequiredEncryptRequestRequestTypeDef = TypedDict(
-    "_RequiredEncryptRequestRequestTypeDef",
-    {
-        "KeyId": str,
-        "Plaintext": Union[str, bytes, IO[Any], StreamingBody],
-    },
-)
-_OptionalEncryptRequestRequestTypeDef = TypedDict(
-    "_OptionalEncryptRequestRequestTypeDef",
-    {
-        "EncryptionContext": Mapping[str, str],
-        "GrantTokens": Sequence[str],
-        "EncryptionAlgorithm": EncryptionAlgorithmSpecType,
-        "DryRun": bool,
-    },
-    total=False,
-)
-
-
-class EncryptRequestRequestTypeDef(
-    _RequiredEncryptRequestRequestTypeDef, _OptionalEncryptRequestRequestTypeDef
-):
-    pass
-
-
 _RequiredGenerateDataKeyPairWithoutPlaintextRequestRequestTypeDef = TypedDict(
     "_RequiredGenerateDataKeyPairWithoutPlaintextRequestRequestTypeDef",
     {
         "KeyId": str,
         "KeyPairSpec": DataKeyPairSpecType,
     },
 )
@@ -418,38 +388,14 @@
 class GenerateDataKeyWithoutPlaintextRequestRequestTypeDef(
     _RequiredGenerateDataKeyWithoutPlaintextRequestRequestTypeDef,
     _OptionalGenerateDataKeyWithoutPlaintextRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredGenerateMacRequestRequestTypeDef = TypedDict(
-    "_RequiredGenerateMacRequestRequestTypeDef",
-    {
-        "Message": Union[str, bytes, IO[Any], StreamingBody],
-        "KeyId": str,
-        "MacAlgorithm": MacAlgorithmSpecType,
-    },
-)
-_OptionalGenerateMacRequestRequestTypeDef = TypedDict(
-    "_OptionalGenerateMacRequestRequestTypeDef",
-    {
-        "GrantTokens": Sequence[str],
-        "DryRun": bool,
-    },
-    total=False,
-)
-
-
-class GenerateMacRequestRequestTypeDef(
-    _RequiredGenerateMacRequestRequestTypeDef, _OptionalGenerateMacRequestRequestTypeDef
-):
-    pass
-
-
 GetKeyPolicyRequestRequestTypeDef = TypedDict(
     "GetKeyPolicyRequestRequestTypeDef",
     {
         "KeyId": str,
         "PolicyName": str,
     },
 )
@@ -496,38 +442,15 @@
     {
         "EncryptionContextSubset": Dict[str, str],
         "EncryptionContextEquals": Dict[str, str],
     },
     total=False,
 )
 
-_RequiredImportKeyMaterialRequestRequestTypeDef = TypedDict(
-    "_RequiredImportKeyMaterialRequestRequestTypeDef",
-    {
-        "KeyId": str,
-        "ImportToken": Union[str, bytes, IO[Any], StreamingBody],
-        "EncryptedKeyMaterial": Union[str, bytes, IO[Any], StreamingBody],
-    },
-)
-_OptionalImportKeyMaterialRequestRequestTypeDef = TypedDict(
-    "_OptionalImportKeyMaterialRequestRequestTypeDef",
-    {
-        "ValidTo": Union[datetime, str],
-        "ExpirationModel": ExpirationModelTypeType,
-    },
-    total=False,
-)
-
-
-class ImportKeyMaterialRequestRequestTypeDef(
-    _RequiredImportKeyMaterialRequestRequestTypeDef, _OptionalImportKeyMaterialRequestRequestTypeDef
-):
-    pass
-
-
+TimestampTypeDef = Union[datetime, str]
 KeyListEntryTypeDef = TypedDict(
     "KeyListEntryTypeDef",
     {
         "KeyId": str,
         "KeyArn": str,
     },
     total=False,
@@ -679,42 +602,14 @@
 
 class PutKeyPolicyRequestRequestTypeDef(
     _RequiredPutKeyPolicyRequestRequestTypeDef, _OptionalPutKeyPolicyRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredReEncryptRequestRequestTypeDef = TypedDict(
-    "_RequiredReEncryptRequestRequestTypeDef",
-    {
-        "CiphertextBlob": Union[str, bytes, IO[Any], StreamingBody],
-        "DestinationKeyId": str,
-    },
-)
-_OptionalReEncryptRequestRequestTypeDef = TypedDict(
-    "_OptionalReEncryptRequestRequestTypeDef",
-    {
-        "SourceEncryptionContext": Mapping[str, str],
-        "SourceKeyId": str,
-        "DestinationEncryptionContext": Mapping[str, str],
-        "SourceEncryptionAlgorithm": EncryptionAlgorithmSpecType,
-        "DestinationEncryptionAlgorithm": EncryptionAlgorithmSpecType,
-        "GrantTokens": Sequence[str],
-        "DryRun": bool,
-    },
-    total=False,
-)
-
-
-class ReEncryptRequestRequestTypeDef(
-    _RequiredReEncryptRequestRequestTypeDef, _OptionalReEncryptRequestRequestTypeDef
-):
-    pass
-
-
 RetireGrantRequestRequestTypeDef = TypedDict(
     "RetireGrantRequestRequestTypeDef",
     {
         "GrantToken": str,
         "KeyId": str,
         "GrantId": str,
         "DryRun": bool,
@@ -762,78 +657,164 @@
 class ScheduleKeyDeletionRequestRequestTypeDef(
     _RequiredScheduleKeyDeletionRequestRequestTypeDef,
     _OptionalScheduleKeyDeletionRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredSignRequestRequestTypeDef = TypedDict(
-    "_RequiredSignRequestRequestTypeDef",
+UntagResourceRequestRequestTypeDef = TypedDict(
+    "UntagResourceRequestRequestTypeDef",
     {
         "KeyId": str,
-        "Message": Union[str, bytes, IO[Any], StreamingBody],
-        "SigningAlgorithm": SigningAlgorithmSpecType,
+        "TagKeys": Sequence[str],
     },
 )
-_OptionalSignRequestRequestTypeDef = TypedDict(
-    "_OptionalSignRequestRequestTypeDef",
+
+UpdateAliasRequestRequestTypeDef = TypedDict(
+    "UpdateAliasRequestRequestTypeDef",
     {
-        "MessageType": MessageTypeType,
+        "AliasName": str,
+        "TargetKeyId": str,
+    },
+)
+
+UpdateKeyDescriptionRequestRequestTypeDef = TypedDict(
+    "UpdateKeyDescriptionRequestRequestTypeDef",
+    {
+        "KeyId": str,
+        "Description": str,
+    },
+)
+
+UpdatePrimaryRegionRequestRequestTypeDef = TypedDict(
+    "UpdatePrimaryRegionRequestRequestTypeDef",
+    {
+        "KeyId": str,
+        "PrimaryRegion": str,
+    },
+)
+
+_RequiredEncryptRequestRequestTypeDef = TypedDict(
+    "_RequiredEncryptRequestRequestTypeDef",
+    {
+        "KeyId": str,
+        "Plaintext": BlobTypeDef,
+    },
+)
+_OptionalEncryptRequestRequestTypeDef = TypedDict(
+    "_OptionalEncryptRequestRequestTypeDef",
+    {
+        "EncryptionContext": Mapping[str, str],
         "GrantTokens": Sequence[str],
+        "EncryptionAlgorithm": EncryptionAlgorithmSpecType,
         "DryRun": bool,
     },
     total=False,
 )
 
 
-class SignRequestRequestTypeDef(
-    _RequiredSignRequestRequestTypeDef, _OptionalSignRequestRequestTypeDef
+class EncryptRequestRequestTypeDef(
+    _RequiredEncryptRequestRequestTypeDef, _OptionalEncryptRequestRequestTypeDef
 ):
     pass
 
 
-UntagResourceRequestRequestTypeDef = TypedDict(
-    "UntagResourceRequestRequestTypeDef",
+_RequiredGenerateMacRequestRequestTypeDef = TypedDict(
+    "_RequiredGenerateMacRequestRequestTypeDef",
     {
+        "Message": BlobTypeDef,
         "KeyId": str,
-        "TagKeys": Sequence[str],
+        "MacAlgorithm": MacAlgorithmSpecType,
+    },
+)
+_OptionalGenerateMacRequestRequestTypeDef = TypedDict(
+    "_OptionalGenerateMacRequestRequestTypeDef",
+    {
+        "GrantTokens": Sequence[str],
+        "DryRun": bool,
     },
+    total=False,
 )
 
-UpdateAliasRequestRequestTypeDef = TypedDict(
-    "UpdateAliasRequestRequestTypeDef",
+
+class GenerateMacRequestRequestTypeDef(
+    _RequiredGenerateMacRequestRequestTypeDef, _OptionalGenerateMacRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredReEncryptRequestRequestTypeDef = TypedDict(
+    "_RequiredReEncryptRequestRequestTypeDef",
     {
-        "AliasName": str,
-        "TargetKeyId": str,
+        "CiphertextBlob": BlobTypeDef,
+        "DestinationKeyId": str,
     },
 )
+_OptionalReEncryptRequestRequestTypeDef = TypedDict(
+    "_OptionalReEncryptRequestRequestTypeDef",
+    {
+        "SourceEncryptionContext": Mapping[str, str],
+        "SourceKeyId": str,
+        "DestinationEncryptionContext": Mapping[str, str],
+        "SourceEncryptionAlgorithm": EncryptionAlgorithmSpecType,
+        "DestinationEncryptionAlgorithm": EncryptionAlgorithmSpecType,
+        "GrantTokens": Sequence[str],
+        "DryRun": bool,
+    },
+    total=False,
+)
 
-UpdateKeyDescriptionRequestRequestTypeDef = TypedDict(
-    "UpdateKeyDescriptionRequestRequestTypeDef",
+
+class ReEncryptRequestRequestTypeDef(
+    _RequiredReEncryptRequestRequestTypeDef, _OptionalReEncryptRequestRequestTypeDef
+):
+    pass
+
+
+RecipientInfoTypeDef = TypedDict(
+    "RecipientInfoTypeDef",
     {
-        "KeyId": str,
-        "Description": str,
+        "KeyEncryptionAlgorithm": Literal["RSAES_OAEP_SHA_256"],
+        "AttestationDocument": BlobTypeDef,
     },
+    total=False,
 )
 
-UpdatePrimaryRegionRequestRequestTypeDef = TypedDict(
-    "UpdatePrimaryRegionRequestRequestTypeDef",
+_RequiredSignRequestRequestTypeDef = TypedDict(
+    "_RequiredSignRequestRequestTypeDef",
     {
         "KeyId": str,
-        "PrimaryRegion": str,
+        "Message": BlobTypeDef,
+        "SigningAlgorithm": SigningAlgorithmSpecType,
+    },
+)
+_OptionalSignRequestRequestTypeDef = TypedDict(
+    "_OptionalSignRequestRequestTypeDef",
+    {
+        "MessageType": MessageTypeType,
+        "GrantTokens": Sequence[str],
+        "DryRun": bool,
     },
+    total=False,
 )
 
+
+class SignRequestRequestTypeDef(
+    _RequiredSignRequestRequestTypeDef, _OptionalSignRequestRequestTypeDef
+):
+    pass
+
+
 _RequiredVerifyMacRequestRequestTypeDef = TypedDict(
     "_RequiredVerifyMacRequestRequestTypeDef",
     {
-        "Message": Union[str, bytes, IO[Any], StreamingBody],
+        "Message": BlobTypeDef,
         "KeyId": str,
         "MacAlgorithm": MacAlgorithmSpecType,
-        "Mac": Union[str, bytes, IO[Any], StreamingBody],
+        "Mac": BlobTypeDef,
     },
 )
 _OptionalVerifyMacRequestRequestTypeDef = TypedDict(
     "_OptionalVerifyMacRequestRequestTypeDef",
     {
         "GrantTokens": Sequence[str],
         "DryRun": bool,
@@ -848,16 +829,16 @@
     pass
 
 
 _RequiredVerifyRequestRequestTypeDef = TypedDict(
     "_RequiredVerifyRequestRequestTypeDef",
     {
         "KeyId": str,
-        "Message": Union[str, bytes, IO[Any], StreamingBody],
-        "Signature": Union[str, bytes, IO[Any], StreamingBody],
+        "Message": BlobTypeDef,
+        "Signature": BlobTypeDef,
         "SigningAlgorithm": SigningAlgorithmSpecType,
     },
 )
 _OptionalVerifyRequestRequestTypeDef = TypedDict(
     "_OptionalVerifyRequestRequestTypeDef",
     {
         "MessageType": MessageTypeType,
@@ -1263,102 +1244,14 @@
         "CreationDate": datetime,
         "CustomKeyStoreType": CustomKeyStoreTypeType,
         "XksProxyConfiguration": XksProxyConfigurationTypeTypeDef,
     },
     total=False,
 )
 
-_RequiredDecryptRequestRequestTypeDef = TypedDict(
-    "_RequiredDecryptRequestRequestTypeDef",
-    {
-        "CiphertextBlob": Union[str, bytes, IO[Any], StreamingBody],
-    },
-)
-_OptionalDecryptRequestRequestTypeDef = TypedDict(
-    "_OptionalDecryptRequestRequestTypeDef",
-    {
-        "EncryptionContext": Mapping[str, str],
-        "GrantTokens": Sequence[str],
-        "KeyId": str,
-        "EncryptionAlgorithm": EncryptionAlgorithmSpecType,
-        "Recipient": RecipientInfoTypeDef,
-        "DryRun": bool,
-    },
-    total=False,
-)
-
-
-class DecryptRequestRequestTypeDef(
-    _RequiredDecryptRequestRequestTypeDef, _OptionalDecryptRequestRequestTypeDef
-):
-    pass
-
-
-_RequiredGenerateDataKeyPairRequestRequestTypeDef = TypedDict(
-    "_RequiredGenerateDataKeyPairRequestRequestTypeDef",
-    {
-        "KeyId": str,
-        "KeyPairSpec": DataKeyPairSpecType,
-    },
-)
-_OptionalGenerateDataKeyPairRequestRequestTypeDef = TypedDict(
-    "_OptionalGenerateDataKeyPairRequestRequestTypeDef",
-    {
-        "EncryptionContext": Mapping[str, str],
-        "GrantTokens": Sequence[str],
-        "Recipient": RecipientInfoTypeDef,
-        "DryRun": bool,
-    },
-    total=False,
-)
-
-
-class GenerateDataKeyPairRequestRequestTypeDef(
-    _RequiredGenerateDataKeyPairRequestRequestTypeDef,
-    _OptionalGenerateDataKeyPairRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredGenerateDataKeyRequestRequestTypeDef = TypedDict(
-    "_RequiredGenerateDataKeyRequestRequestTypeDef",
-    {
-        "KeyId": str,
-    },
-)
-_OptionalGenerateDataKeyRequestRequestTypeDef = TypedDict(
-    "_OptionalGenerateDataKeyRequestRequestTypeDef",
-    {
-        "EncryptionContext": Mapping[str, str],
-        "NumberOfBytes": int,
-        "KeySpec": DataKeySpecType,
-        "GrantTokens": Sequence[str],
-        "Recipient": RecipientInfoTypeDef,
-        "DryRun": bool,
-    },
-    total=False,
-)
-
-
-class GenerateDataKeyRequestRequestTypeDef(
-    _RequiredGenerateDataKeyRequestRequestTypeDef, _OptionalGenerateDataKeyRequestRequestTypeDef
-):
-    pass
-
-
-GenerateRandomRequestRequestTypeDef = TypedDict(
-    "GenerateRandomRequestRequestTypeDef",
-    {
-        "NumberOfBytes": int,
-        "CustomKeyStoreId": str,
-        "Recipient": RecipientInfoTypeDef,
-    },
-    total=False,
-)
-
 DescribeCustomKeyStoresRequestDescribeCustomKeyStoresPaginateTypeDef = TypedDict(
     "DescribeCustomKeyStoresRequestDescribeCustomKeyStoresPaginateTypeDef",
     {
         "CustomKeyStoreId": str,
         "CustomKeyStoreName": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
@@ -1468,14 +1361,15 @@
 class ListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef(
     _RequiredListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef,
     _OptionalListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef,
 ):
     pass
 
 
+GrantConstraintsUnionTypeDef = Union[GrantConstraintsTypeDef, GrantConstraintsOutputTypeDef]
 GrantListEntryTypeDef = TypedDict(
     "GrantListEntryTypeDef",
     {
         "KeyId": str,
         "GrantId": str,
         "Name": str,
         "CreationDate": datetime,
@@ -1484,14 +1378,38 @@
         "IssuingAccount": str,
         "Operations": List[GrantOperationType],
         "Constraints": GrantConstraintsOutputTypeDef,
     },
     total=False,
 )
 
+_RequiredImportKeyMaterialRequestRequestTypeDef = TypedDict(
+    "_RequiredImportKeyMaterialRequestRequestTypeDef",
+    {
+        "KeyId": str,
+        "ImportToken": BlobTypeDef,
+        "EncryptedKeyMaterial": BlobTypeDef,
+    },
+)
+_OptionalImportKeyMaterialRequestRequestTypeDef = TypedDict(
+    "_OptionalImportKeyMaterialRequestRequestTypeDef",
+    {
+        "ValidTo": TimestampTypeDef,
+        "ExpirationModel": ExpirationModelTypeType,
+    },
+    total=False,
+)
+
+
+class ImportKeyMaterialRequestRequestTypeDef(
+    _RequiredImportKeyMaterialRequestRequestTypeDef, _OptionalImportKeyMaterialRequestRequestTypeDef
+):
+    pass
+
+
 ListKeysResponseTypeDef = TypedDict(
     "ListKeysResponseTypeDef",
     {
         "Keys": List[KeyListEntryTypeDef],
         "NextMarker": str,
         "Truncated": bool,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1504,14 +1422,102 @@
         "MultiRegionKeyType": MultiRegionKeyTypeType,
         "PrimaryKey": MultiRegionKeyTypeDef,
         "ReplicaKeys": List[MultiRegionKeyTypeDef],
     },
     total=False,
 )
 
+_RequiredDecryptRequestRequestTypeDef = TypedDict(
+    "_RequiredDecryptRequestRequestTypeDef",
+    {
+        "CiphertextBlob": BlobTypeDef,
+    },
+)
+_OptionalDecryptRequestRequestTypeDef = TypedDict(
+    "_OptionalDecryptRequestRequestTypeDef",
+    {
+        "EncryptionContext": Mapping[str, str],
+        "GrantTokens": Sequence[str],
+        "KeyId": str,
+        "EncryptionAlgorithm": EncryptionAlgorithmSpecType,
+        "Recipient": RecipientInfoTypeDef,
+        "DryRun": bool,
+    },
+    total=False,
+)
+
+
+class DecryptRequestRequestTypeDef(
+    _RequiredDecryptRequestRequestTypeDef, _OptionalDecryptRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredGenerateDataKeyPairRequestRequestTypeDef = TypedDict(
+    "_RequiredGenerateDataKeyPairRequestRequestTypeDef",
+    {
+        "KeyId": str,
+        "KeyPairSpec": DataKeyPairSpecType,
+    },
+)
+_OptionalGenerateDataKeyPairRequestRequestTypeDef = TypedDict(
+    "_OptionalGenerateDataKeyPairRequestRequestTypeDef",
+    {
+        "EncryptionContext": Mapping[str, str],
+        "GrantTokens": Sequence[str],
+        "Recipient": RecipientInfoTypeDef,
+        "DryRun": bool,
+    },
+    total=False,
+)
+
+
+class GenerateDataKeyPairRequestRequestTypeDef(
+    _RequiredGenerateDataKeyPairRequestRequestTypeDef,
+    _OptionalGenerateDataKeyPairRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredGenerateDataKeyRequestRequestTypeDef = TypedDict(
+    "_RequiredGenerateDataKeyRequestRequestTypeDef",
+    {
+        "KeyId": str,
+    },
+)
+_OptionalGenerateDataKeyRequestRequestTypeDef = TypedDict(
+    "_OptionalGenerateDataKeyRequestRequestTypeDef",
+    {
+        "EncryptionContext": Mapping[str, str],
+        "NumberOfBytes": int,
+        "KeySpec": DataKeySpecType,
+        "GrantTokens": Sequence[str],
+        "Recipient": RecipientInfoTypeDef,
+        "DryRun": bool,
+    },
+    total=False,
+)
+
+
+class GenerateDataKeyRequestRequestTypeDef(
+    _RequiredGenerateDataKeyRequestRequestTypeDef, _OptionalGenerateDataKeyRequestRequestTypeDef
+):
+    pass
+
+
+GenerateRandomRequestRequestTypeDef = TypedDict(
+    "GenerateRandomRequestRequestTypeDef",
+    {
+        "NumberOfBytes": int,
+        "CustomKeyStoreId": str,
+        "Recipient": RecipientInfoTypeDef,
+    },
+    total=False,
+)
+
 DescribeCustomKeyStoresResponseTypeDef = TypedDict(
     "DescribeCustomKeyStoresResponseTypeDef",
     {
         "CustomKeyStores": List[CustomKeyStoresListEntryTypeDef],
         "NextMarker": str,
         "Truncated": bool,
         "ResponseMetadata": ResponseMetadataTypeDef,
```

### Comparing `mypy-boto3-kms-1.28.15.post1/mypy_boto3_kms/type_defs.pyi` & `mypy-boto3-kms-1.28.16/mypy_boto3_kms/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_kms.type_defs import AliasListEntryTypeDef
 
-    data: AliasListEntryTypeDef = {...}
+    data: AliasListEntryTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -48,63 +48,64 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AliasListEntryTypeDef",
+    "BlobTypeDef",
     "CancelKeyDeletionRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "ConnectCustomKeyStoreRequestRequestTypeDef",
     "CreateAliasRequestRequestTypeDef",
     "XksProxyAuthenticationCredentialTypeTypeDef",
     "GrantConstraintsTypeDef",
     "TagTypeDef",
     "XksProxyConfigurationTypeTypeDef",
-    "RecipientInfoTypeDef",
     "DeleteAliasRequestRequestTypeDef",
     "DeleteCustomKeyStoreRequestRequestTypeDef",
     "DeleteImportedKeyMaterialRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "DescribeCustomKeyStoresRequestRequestTypeDef",
     "DescribeKeyRequestRequestTypeDef",
     "DisableKeyRequestRequestTypeDef",
     "DisableKeyRotationRequestRequestTypeDef",
     "DisconnectCustomKeyStoreRequestRequestTypeDef",
     "EnableKeyRequestRequestTypeDef",
     "EnableKeyRotationRequestRequestTypeDef",
-    "EncryptRequestRequestTypeDef",
     "GenerateDataKeyPairWithoutPlaintextRequestRequestTypeDef",
     "GenerateDataKeyWithoutPlaintextRequestRequestTypeDef",
-    "GenerateMacRequestRequestTypeDef",
     "GetKeyPolicyRequestRequestTypeDef",
     "GetKeyRotationStatusRequestRequestTypeDef",
     "GetParametersForImportRequestRequestTypeDef",
     "GetPublicKeyRequestRequestTypeDef",
     "GrantConstraintsOutputTypeDef",
-    "ImportKeyMaterialRequestRequestTypeDef",
+    "TimestampTypeDef",
     "KeyListEntryTypeDef",
     "XksKeyConfigurationTypeTypeDef",
     "ListAliasesRequestRequestTypeDef",
     "ListGrantsRequestRequestTypeDef",
     "ListKeyPoliciesRequestRequestTypeDef",
     "ListKeysRequestRequestTypeDef",
     "ListResourceTagsRequestRequestTypeDef",
     "ListRetirableGrantsRequestRequestTypeDef",
     "MultiRegionKeyTypeDef",
     "PutKeyPolicyRequestRequestTypeDef",
-    "ReEncryptRequestRequestTypeDef",
     "RetireGrantRequestRequestTypeDef",
     "RevokeGrantRequestRequestTypeDef",
     "ScheduleKeyDeletionRequestRequestTypeDef",
-    "SignRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAliasRequestRequestTypeDef",
     "UpdateKeyDescriptionRequestRequestTypeDef",
     "UpdatePrimaryRegionRequestRequestTypeDef",
+    "EncryptRequestRequestTypeDef",
+    "GenerateMacRequestRequestTypeDef",
+    "ReEncryptRequestRequestTypeDef",
+    "RecipientInfoTypeDef",
+    "SignRequestRequestTypeDef",
     "VerifyMacRequestRequestTypeDef",
     "VerifyRequestRequestTypeDef",
     "CancelKeyDeletionResponseTypeDef",
     "CreateCustomKeyStoreResponseTypeDef",
     "CreateGrantResponseTypeDef",
     "DecryptResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
@@ -130,28 +131,30 @@
     "UpdateCustomKeyStoreRequestRequestTypeDef",
     "CreateGrantRequestRequestTypeDef",
     "CreateKeyRequestRequestTypeDef",
     "ListResourceTagsResponseTypeDef",
     "ReplicateKeyRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CustomKeyStoresListEntryTypeDef",
-    "DecryptRequestRequestTypeDef",
-    "GenerateDataKeyPairRequestRequestTypeDef",
-    "GenerateDataKeyRequestRequestTypeDef",
-    "GenerateRandomRequestRequestTypeDef",
     "DescribeCustomKeyStoresRequestDescribeCustomKeyStoresPaginateTypeDef",
     "ListAliasesRequestListAliasesPaginateTypeDef",
     "ListGrantsRequestListGrantsPaginateTypeDef",
     "ListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef",
     "ListKeysRequestListKeysPaginateTypeDef",
     "ListResourceTagsRequestListResourceTagsPaginateTypeDef",
     "ListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef",
+    "GrantConstraintsUnionTypeDef",
     "GrantListEntryTypeDef",
+    "ImportKeyMaterialRequestRequestTypeDef",
     "ListKeysResponseTypeDef",
     "MultiRegionConfigurationTypeDef",
+    "DecryptRequestRequestTypeDef",
+    "GenerateDataKeyPairRequestRequestTypeDef",
+    "GenerateDataKeyRequestRequestTypeDef",
+    "GenerateRandomRequestRequestTypeDef",
     "DescribeCustomKeyStoresResponseTypeDef",
     "ListGrantsResponseTypeDef",
     "KeyMetadataTypeDef",
     "CreateKeyResponseTypeDef",
     "DescribeKeyResponseTypeDef",
     "ReplicateKeyResponseTypeDef",
 )
@@ -164,14 +167,15 @@
         "TargetKeyId": str,
         "CreationDate": datetime,
         "LastUpdatedDate": datetime,
     },
     total=False,
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 CancelKeyDeletionRequestRequestTypeDef = TypedDict(
     "CancelKeyDeletionRequestRequestTypeDef",
     {
         "KeyId": str,
     },
 )
 
@@ -234,23 +238,14 @@
         "UriEndpoint": str,
         "UriPath": str,
         "VpcEndpointServiceName": str,
     },
     total=False,
 )
 
-RecipientInfoTypeDef = TypedDict(
-    "RecipientInfoTypeDef",
-    {
-        "KeyEncryptionAlgorithm": Literal["RSAES_OAEP_SHA_256"],
-        "AttestationDocument": Union[str, bytes, IO[Any], StreamingBody],
-    },
-    total=False,
-)
-
 DeleteAliasRequestRequestTypeDef = TypedDict(
     "DeleteAliasRequestRequestTypeDef",
     {
         "AliasName": str,
     },
 )
 
@@ -339,37 +334,14 @@
 EnableKeyRotationRequestRequestTypeDef = TypedDict(
     "EnableKeyRotationRequestRequestTypeDef",
     {
         "KeyId": str,
     },
 )
 
-_RequiredEncryptRequestRequestTypeDef = TypedDict(
-    "_RequiredEncryptRequestRequestTypeDef",
-    {
-        "KeyId": str,
-        "Plaintext": Union[str, bytes, IO[Any], StreamingBody],
-    },
-)
-_OptionalEncryptRequestRequestTypeDef = TypedDict(
-    "_OptionalEncryptRequestRequestTypeDef",
-    {
-        "EncryptionContext": Mapping[str, str],
-        "GrantTokens": Sequence[str],
-        "EncryptionAlgorithm": EncryptionAlgorithmSpecType,
-        "DryRun": bool,
-    },
-    total=False,
-)
-
-class EncryptRequestRequestTypeDef(
-    _RequiredEncryptRequestRequestTypeDef, _OptionalEncryptRequestRequestTypeDef
-):
-    pass
-
 _RequiredGenerateDataKeyPairWithoutPlaintextRequestRequestTypeDef = TypedDict(
     "_RequiredGenerateDataKeyPairWithoutPlaintextRequestRequestTypeDef",
     {
         "KeyId": str,
         "KeyPairSpec": DataKeyPairSpecType,
     },
 )
@@ -409,36 +381,14 @@
 
 class GenerateDataKeyWithoutPlaintextRequestRequestTypeDef(
     _RequiredGenerateDataKeyWithoutPlaintextRequestRequestTypeDef,
     _OptionalGenerateDataKeyWithoutPlaintextRequestRequestTypeDef,
 ):
     pass
 
-_RequiredGenerateMacRequestRequestTypeDef = TypedDict(
-    "_RequiredGenerateMacRequestRequestTypeDef",
-    {
-        "Message": Union[str, bytes, IO[Any], StreamingBody],
-        "KeyId": str,
-        "MacAlgorithm": MacAlgorithmSpecType,
-    },
-)
-_OptionalGenerateMacRequestRequestTypeDef = TypedDict(
-    "_OptionalGenerateMacRequestRequestTypeDef",
-    {
-        "GrantTokens": Sequence[str],
-        "DryRun": bool,
-    },
-    total=False,
-)
-
-class GenerateMacRequestRequestTypeDef(
-    _RequiredGenerateMacRequestRequestTypeDef, _OptionalGenerateMacRequestRequestTypeDef
-):
-    pass
-
 GetKeyPolicyRequestRequestTypeDef = TypedDict(
     "GetKeyPolicyRequestRequestTypeDef",
     {
         "KeyId": str,
         "PolicyName": str,
     },
 )
@@ -483,36 +433,15 @@
     {
         "EncryptionContextSubset": Dict[str, str],
         "EncryptionContextEquals": Dict[str, str],
     },
     total=False,
 )
 
-_RequiredImportKeyMaterialRequestRequestTypeDef = TypedDict(
-    "_RequiredImportKeyMaterialRequestRequestTypeDef",
-    {
-        "KeyId": str,
-        "ImportToken": Union[str, bytes, IO[Any], StreamingBody],
-        "EncryptedKeyMaterial": Union[str, bytes, IO[Any], StreamingBody],
-    },
-)
-_OptionalImportKeyMaterialRequestRequestTypeDef = TypedDict(
-    "_OptionalImportKeyMaterialRequestRequestTypeDef",
-    {
-        "ValidTo": Union[datetime, str],
-        "ExpirationModel": ExpirationModelTypeType,
-    },
-    total=False,
-)
-
-class ImportKeyMaterialRequestRequestTypeDef(
-    _RequiredImportKeyMaterialRequestRequestTypeDef, _OptionalImportKeyMaterialRequestRequestTypeDef
-):
-    pass
-
+TimestampTypeDef = Union[datetime, str]
 KeyListEntryTypeDef = TypedDict(
     "KeyListEntryTypeDef",
     {
         "KeyId": str,
         "KeyArn": str,
     },
     total=False,
@@ -654,40 +583,14 @@
 )
 
 class PutKeyPolicyRequestRequestTypeDef(
     _RequiredPutKeyPolicyRequestRequestTypeDef, _OptionalPutKeyPolicyRequestRequestTypeDef
 ):
     pass
 
-_RequiredReEncryptRequestRequestTypeDef = TypedDict(
-    "_RequiredReEncryptRequestRequestTypeDef",
-    {
-        "CiphertextBlob": Union[str, bytes, IO[Any], StreamingBody],
-        "DestinationKeyId": str,
-    },
-)
-_OptionalReEncryptRequestRequestTypeDef = TypedDict(
-    "_OptionalReEncryptRequestRequestTypeDef",
-    {
-        "SourceEncryptionContext": Mapping[str, str],
-        "SourceKeyId": str,
-        "DestinationEncryptionContext": Mapping[str, str],
-        "SourceEncryptionAlgorithm": EncryptionAlgorithmSpecType,
-        "DestinationEncryptionAlgorithm": EncryptionAlgorithmSpecType,
-        "GrantTokens": Sequence[str],
-        "DryRun": bool,
-    },
-    total=False,
-)
-
-class ReEncryptRequestRequestTypeDef(
-    _RequiredReEncryptRequestRequestTypeDef, _OptionalReEncryptRequestRequestTypeDef
-):
-    pass
-
 RetireGrantRequestRequestTypeDef = TypedDict(
     "RetireGrantRequestRequestTypeDef",
     {
         "GrantToken": str,
         "KeyId": str,
         "GrantId": str,
         "DryRun": bool,
@@ -731,37 +634,14 @@
 
 class ScheduleKeyDeletionRequestRequestTypeDef(
     _RequiredScheduleKeyDeletionRequestRequestTypeDef,
     _OptionalScheduleKeyDeletionRequestRequestTypeDef,
 ):
     pass
 
-_RequiredSignRequestRequestTypeDef = TypedDict(
-    "_RequiredSignRequestRequestTypeDef",
-    {
-        "KeyId": str,
-        "Message": Union[str, bytes, IO[Any], StreamingBody],
-        "SigningAlgorithm": SigningAlgorithmSpecType,
-    },
-)
-_OptionalSignRequestRequestTypeDef = TypedDict(
-    "_OptionalSignRequestRequestTypeDef",
-    {
-        "MessageType": MessageTypeType,
-        "GrantTokens": Sequence[str],
-        "DryRun": bool,
-    },
-    total=False,
-)
-
-class SignRequestRequestTypeDef(
-    _RequiredSignRequestRequestTypeDef, _OptionalSignRequestRequestTypeDef
-):
-    pass
-
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "KeyId": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -786,21 +666,124 @@
     "UpdatePrimaryRegionRequestRequestTypeDef",
     {
         "KeyId": str,
         "PrimaryRegion": str,
     },
 )
 
+_RequiredEncryptRequestRequestTypeDef = TypedDict(
+    "_RequiredEncryptRequestRequestTypeDef",
+    {
+        "KeyId": str,
+        "Plaintext": BlobTypeDef,
+    },
+)
+_OptionalEncryptRequestRequestTypeDef = TypedDict(
+    "_OptionalEncryptRequestRequestTypeDef",
+    {
+        "EncryptionContext": Mapping[str, str],
+        "GrantTokens": Sequence[str],
+        "EncryptionAlgorithm": EncryptionAlgorithmSpecType,
+        "DryRun": bool,
+    },
+    total=False,
+)
+
+class EncryptRequestRequestTypeDef(
+    _RequiredEncryptRequestRequestTypeDef, _OptionalEncryptRequestRequestTypeDef
+):
+    pass
+
+_RequiredGenerateMacRequestRequestTypeDef = TypedDict(
+    "_RequiredGenerateMacRequestRequestTypeDef",
+    {
+        "Message": BlobTypeDef,
+        "KeyId": str,
+        "MacAlgorithm": MacAlgorithmSpecType,
+    },
+)
+_OptionalGenerateMacRequestRequestTypeDef = TypedDict(
+    "_OptionalGenerateMacRequestRequestTypeDef",
+    {
+        "GrantTokens": Sequence[str],
+        "DryRun": bool,
+    },
+    total=False,
+)
+
+class GenerateMacRequestRequestTypeDef(
+    _RequiredGenerateMacRequestRequestTypeDef, _OptionalGenerateMacRequestRequestTypeDef
+):
+    pass
+
+_RequiredReEncryptRequestRequestTypeDef = TypedDict(
+    "_RequiredReEncryptRequestRequestTypeDef",
+    {
+        "CiphertextBlob": BlobTypeDef,
+        "DestinationKeyId": str,
+    },
+)
+_OptionalReEncryptRequestRequestTypeDef = TypedDict(
+    "_OptionalReEncryptRequestRequestTypeDef",
+    {
+        "SourceEncryptionContext": Mapping[str, str],
+        "SourceKeyId": str,
+        "DestinationEncryptionContext": Mapping[str, str],
+        "SourceEncryptionAlgorithm": EncryptionAlgorithmSpecType,
+        "DestinationEncryptionAlgorithm": EncryptionAlgorithmSpecType,
+        "GrantTokens": Sequence[str],
+        "DryRun": bool,
+    },
+    total=False,
+)
+
+class ReEncryptRequestRequestTypeDef(
+    _RequiredReEncryptRequestRequestTypeDef, _OptionalReEncryptRequestRequestTypeDef
+):
+    pass
+
+RecipientInfoTypeDef = TypedDict(
+    "RecipientInfoTypeDef",
+    {
+        "KeyEncryptionAlgorithm": Literal["RSAES_OAEP_SHA_256"],
+        "AttestationDocument": BlobTypeDef,
+    },
+    total=False,
+)
+
+_RequiredSignRequestRequestTypeDef = TypedDict(
+    "_RequiredSignRequestRequestTypeDef",
+    {
+        "KeyId": str,
+        "Message": BlobTypeDef,
+        "SigningAlgorithm": SigningAlgorithmSpecType,
+    },
+)
+_OptionalSignRequestRequestTypeDef = TypedDict(
+    "_OptionalSignRequestRequestTypeDef",
+    {
+        "MessageType": MessageTypeType,
+        "GrantTokens": Sequence[str],
+        "DryRun": bool,
+    },
+    total=False,
+)
+
+class SignRequestRequestTypeDef(
+    _RequiredSignRequestRequestTypeDef, _OptionalSignRequestRequestTypeDef
+):
+    pass
+
 _RequiredVerifyMacRequestRequestTypeDef = TypedDict(
     "_RequiredVerifyMacRequestRequestTypeDef",
     {
-        "Message": Union[str, bytes, IO[Any], StreamingBody],
+        "Message": BlobTypeDef,
         "KeyId": str,
         "MacAlgorithm": MacAlgorithmSpecType,
-        "Mac": Union[str, bytes, IO[Any], StreamingBody],
+        "Mac": BlobTypeDef,
     },
 )
 _OptionalVerifyMacRequestRequestTypeDef = TypedDict(
     "_OptionalVerifyMacRequestRequestTypeDef",
     {
         "GrantTokens": Sequence[str],
         "DryRun": bool,
@@ -813,16 +796,16 @@
 ):
     pass
 
 _RequiredVerifyRequestRequestTypeDef = TypedDict(
     "_RequiredVerifyRequestRequestTypeDef",
     {
         "KeyId": str,
-        "Message": Union[str, bytes, IO[Any], StreamingBody],
-        "Signature": Union[str, bytes, IO[Any], StreamingBody],
+        "Message": BlobTypeDef,
+        "Signature": BlobTypeDef,
         "SigningAlgorithm": SigningAlgorithmSpecType,
     },
 )
 _OptionalVerifyRequestRequestTypeDef = TypedDict(
     "_OptionalVerifyRequestRequestTypeDef",
     {
         "MessageType": MessageTypeType,
@@ -1218,96 +1201,14 @@
         "CreationDate": datetime,
         "CustomKeyStoreType": CustomKeyStoreTypeType,
         "XksProxyConfiguration": XksProxyConfigurationTypeTypeDef,
     },
     total=False,
 )
 
-_RequiredDecryptRequestRequestTypeDef = TypedDict(
-    "_RequiredDecryptRequestRequestTypeDef",
-    {
-        "CiphertextBlob": Union[str, bytes, IO[Any], StreamingBody],
-    },
-)
-_OptionalDecryptRequestRequestTypeDef = TypedDict(
-    "_OptionalDecryptRequestRequestTypeDef",
-    {
-        "EncryptionContext": Mapping[str, str],
-        "GrantTokens": Sequence[str],
-        "KeyId": str,
-        "EncryptionAlgorithm": EncryptionAlgorithmSpecType,
-        "Recipient": RecipientInfoTypeDef,
-        "DryRun": bool,
-    },
-    total=False,
-)
-
-class DecryptRequestRequestTypeDef(
-    _RequiredDecryptRequestRequestTypeDef, _OptionalDecryptRequestRequestTypeDef
-):
-    pass
-
-_RequiredGenerateDataKeyPairRequestRequestTypeDef = TypedDict(
-    "_RequiredGenerateDataKeyPairRequestRequestTypeDef",
-    {
-        "KeyId": str,
-        "KeyPairSpec": DataKeyPairSpecType,
-    },
-)
-_OptionalGenerateDataKeyPairRequestRequestTypeDef = TypedDict(
-    "_OptionalGenerateDataKeyPairRequestRequestTypeDef",
-    {
-        "EncryptionContext": Mapping[str, str],
-        "GrantTokens": Sequence[str],
-        "Recipient": RecipientInfoTypeDef,
-        "DryRun": bool,
-    },
-    total=False,
-)
-
-class GenerateDataKeyPairRequestRequestTypeDef(
-    _RequiredGenerateDataKeyPairRequestRequestTypeDef,
-    _OptionalGenerateDataKeyPairRequestRequestTypeDef,
-):
-    pass
-
-_RequiredGenerateDataKeyRequestRequestTypeDef = TypedDict(
-    "_RequiredGenerateDataKeyRequestRequestTypeDef",
-    {
-        "KeyId": str,
-    },
-)
-_OptionalGenerateDataKeyRequestRequestTypeDef = TypedDict(
-    "_OptionalGenerateDataKeyRequestRequestTypeDef",
-    {
-        "EncryptionContext": Mapping[str, str],
-        "NumberOfBytes": int,
-        "KeySpec": DataKeySpecType,
-        "GrantTokens": Sequence[str],
-        "Recipient": RecipientInfoTypeDef,
-        "DryRun": bool,
-    },
-    total=False,
-)
-
-class GenerateDataKeyRequestRequestTypeDef(
-    _RequiredGenerateDataKeyRequestRequestTypeDef, _OptionalGenerateDataKeyRequestRequestTypeDef
-):
-    pass
-
-GenerateRandomRequestRequestTypeDef = TypedDict(
-    "GenerateRandomRequestRequestTypeDef",
-    {
-        "NumberOfBytes": int,
-        "CustomKeyStoreId": str,
-        "Recipient": RecipientInfoTypeDef,
-    },
-    total=False,
-)
-
 DescribeCustomKeyStoresRequestDescribeCustomKeyStoresPaginateTypeDef = TypedDict(
     "DescribeCustomKeyStoresRequestDescribeCustomKeyStoresPaginateTypeDef",
     {
         "CustomKeyStoreId": str,
         "CustomKeyStoreName": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
@@ -1409,14 +1310,15 @@
 
 class ListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef(
     _RequiredListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef,
     _OptionalListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef,
 ):
     pass
 
+GrantConstraintsUnionTypeDef = Union[GrantConstraintsTypeDef, GrantConstraintsOutputTypeDef]
 GrantListEntryTypeDef = TypedDict(
     "GrantListEntryTypeDef",
     {
         "KeyId": str,
         "GrantId": str,
         "Name": str,
         "CreationDate": datetime,
@@ -1425,14 +1327,36 @@
         "IssuingAccount": str,
         "Operations": List[GrantOperationType],
         "Constraints": GrantConstraintsOutputTypeDef,
     },
     total=False,
 )
 
+_RequiredImportKeyMaterialRequestRequestTypeDef = TypedDict(
+    "_RequiredImportKeyMaterialRequestRequestTypeDef",
+    {
+        "KeyId": str,
+        "ImportToken": BlobTypeDef,
+        "EncryptedKeyMaterial": BlobTypeDef,
+    },
+)
+_OptionalImportKeyMaterialRequestRequestTypeDef = TypedDict(
+    "_OptionalImportKeyMaterialRequestRequestTypeDef",
+    {
+        "ValidTo": TimestampTypeDef,
+        "ExpirationModel": ExpirationModelTypeType,
+    },
+    total=False,
+)
+
+class ImportKeyMaterialRequestRequestTypeDef(
+    _RequiredImportKeyMaterialRequestRequestTypeDef, _OptionalImportKeyMaterialRequestRequestTypeDef
+):
+    pass
+
 ListKeysResponseTypeDef = TypedDict(
     "ListKeysResponseTypeDef",
     {
         "Keys": List[KeyListEntryTypeDef],
         "NextMarker": str,
         "Truncated": bool,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1445,14 +1369,96 @@
         "MultiRegionKeyType": MultiRegionKeyTypeType,
         "PrimaryKey": MultiRegionKeyTypeDef,
         "ReplicaKeys": List[MultiRegionKeyTypeDef],
     },
     total=False,
 )
 
+_RequiredDecryptRequestRequestTypeDef = TypedDict(
+    "_RequiredDecryptRequestRequestTypeDef",
+    {
+        "CiphertextBlob": BlobTypeDef,
+    },
+)
+_OptionalDecryptRequestRequestTypeDef = TypedDict(
+    "_OptionalDecryptRequestRequestTypeDef",
+    {
+        "EncryptionContext": Mapping[str, str],
+        "GrantTokens": Sequence[str],
+        "KeyId": str,
+        "EncryptionAlgorithm": EncryptionAlgorithmSpecType,
+        "Recipient": RecipientInfoTypeDef,
+        "DryRun": bool,
+    },
+    total=False,
+)
+
+class DecryptRequestRequestTypeDef(
+    _RequiredDecryptRequestRequestTypeDef, _OptionalDecryptRequestRequestTypeDef
+):
+    pass
+
+_RequiredGenerateDataKeyPairRequestRequestTypeDef = TypedDict(
+    "_RequiredGenerateDataKeyPairRequestRequestTypeDef",
+    {
+        "KeyId": str,
+        "KeyPairSpec": DataKeyPairSpecType,
+    },
+)
+_OptionalGenerateDataKeyPairRequestRequestTypeDef = TypedDict(
+    "_OptionalGenerateDataKeyPairRequestRequestTypeDef",
+    {
+        "EncryptionContext": Mapping[str, str],
+        "GrantTokens": Sequence[str],
+        "Recipient": RecipientInfoTypeDef,
+        "DryRun": bool,
+    },
+    total=False,
+)
+
+class GenerateDataKeyPairRequestRequestTypeDef(
+    _RequiredGenerateDataKeyPairRequestRequestTypeDef,
+    _OptionalGenerateDataKeyPairRequestRequestTypeDef,
+):
+    pass
+
+_RequiredGenerateDataKeyRequestRequestTypeDef = TypedDict(
+    "_RequiredGenerateDataKeyRequestRequestTypeDef",
+    {
+        "KeyId": str,
+    },
+)
+_OptionalGenerateDataKeyRequestRequestTypeDef = TypedDict(
+    "_OptionalGenerateDataKeyRequestRequestTypeDef",
+    {
+        "EncryptionContext": Mapping[str, str],
+        "NumberOfBytes": int,
+        "KeySpec": DataKeySpecType,
+        "GrantTokens": Sequence[str],
+        "Recipient": RecipientInfoTypeDef,
+        "DryRun": bool,
+    },
+    total=False,
+)
+
+class GenerateDataKeyRequestRequestTypeDef(
+    _RequiredGenerateDataKeyRequestRequestTypeDef, _OptionalGenerateDataKeyRequestRequestTypeDef
+):
+    pass
+
+GenerateRandomRequestRequestTypeDef = TypedDict(
+    "GenerateRandomRequestRequestTypeDef",
+    {
+        "NumberOfBytes": int,
+        "CustomKeyStoreId": str,
+        "Recipient": RecipientInfoTypeDef,
+    },
+    total=False,
+)
+
 DescribeCustomKeyStoresResponseTypeDef = TypedDict(
     "DescribeCustomKeyStoresResponseTypeDef",
     {
         "CustomKeyStores": List[CustomKeyStoresListEntryTypeDef],
         "NextMarker": str,
         "Truncated": bool,
         "ResponseMetadata": ResponseMetadataTypeDef,
```

### Comparing `mypy-boto3-kms-1.28.15.post1/mypy_boto3_kms.egg-info/PKG-INFO` & `mypy-boto3-kms-1.28.16/mypy_boto3_kms.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-kms
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.KMS 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.KMS 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 kms type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 kms type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kms.svg?color=blue)](https://pypi.org/project/mypy-boto3-kms)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-kms)](https://pepy.tech/project/mypy-boto3-kms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.KMS 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS)
+[boto3.KMS 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS)
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
 [mypy-boto3-kms docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/).
 
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
@@ -354,73 +354,74 @@
 )
 
 
 def check_value(value: AlgorithmSpecType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_kms.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_kms.type_defs import (
     AliasListEntryTypeDef,
+    BlobTypeDef,
     CancelKeyDeletionRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     ConnectCustomKeyStoreRequestRequestTypeDef,
     CreateAliasRequestRequestTypeDef,
     XksProxyAuthenticationCredentialTypeTypeDef,
     GrantConstraintsTypeDef,
     TagTypeDef,
     XksProxyConfigurationTypeTypeDef,
-    RecipientInfoTypeDef,
     DeleteAliasRequestRequestTypeDef,
     DeleteCustomKeyStoreRequestRequestTypeDef,
     DeleteImportedKeyMaterialRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     DescribeCustomKeyStoresRequestRequestTypeDef,
     DescribeKeyRequestRequestTypeDef,
     DisableKeyRequestRequestTypeDef,
     DisableKeyRotationRequestRequestTypeDef,
     DisconnectCustomKeyStoreRequestRequestTypeDef,
     EnableKeyRequestRequestTypeDef,
     EnableKeyRotationRequestRequestTypeDef,
-    EncryptRequestRequestTypeDef,
     GenerateDataKeyPairWithoutPlaintextRequestRequestTypeDef,
     GenerateDataKeyWithoutPlaintextRequestRequestTypeDef,
-    GenerateMacRequestRequestTypeDef,
     GetKeyPolicyRequestRequestTypeDef,
     GetKeyRotationStatusRequestRequestTypeDef,
     GetParametersForImportRequestRequestTypeDef,
     GetPublicKeyRequestRequestTypeDef,
     GrantConstraintsOutputTypeDef,
-    ImportKeyMaterialRequestRequestTypeDef,
+    TimestampTypeDef,
     KeyListEntryTypeDef,
     XksKeyConfigurationTypeTypeDef,
     ListAliasesRequestRequestTypeDef,
     ListGrantsRequestRequestTypeDef,
     ListKeyPoliciesRequestRequestTypeDef,
     ListKeysRequestRequestTypeDef,
     ListResourceTagsRequestRequestTypeDef,
     ListRetirableGrantsRequestRequestTypeDef,
     MultiRegionKeyTypeDef,
     PutKeyPolicyRequestRequestTypeDef,
-    ReEncryptRequestRequestTypeDef,
     RetireGrantRequestRequestTypeDef,
     RevokeGrantRequestRequestTypeDef,
     ScheduleKeyDeletionRequestRequestTypeDef,
-    SignRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAliasRequestRequestTypeDef,
     UpdateKeyDescriptionRequestRequestTypeDef,
     UpdatePrimaryRegionRequestRequestTypeDef,
+    EncryptRequestRequestTypeDef,
+    GenerateMacRequestRequestTypeDef,
+    ReEncryptRequestRequestTypeDef,
+    RecipientInfoTypeDef,
+    SignRequestRequestTypeDef,
     VerifyMacRequestRequestTypeDef,
     VerifyRequestRequestTypeDef,
     CancelKeyDeletionResponseTypeDef,
     CreateCustomKeyStoreResponseTypeDef,
     CreateGrantResponseTypeDef,
     DecryptResponseTypeDef,
     EmptyResponseMetadataTypeDef,
@@ -446,38 +447,40 @@
     UpdateCustomKeyStoreRequestRequestTypeDef,
     CreateGrantRequestRequestTypeDef,
     CreateKeyRequestRequestTypeDef,
     ListResourceTagsResponseTypeDef,
     ReplicateKeyRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     CustomKeyStoresListEntryTypeDef,
-    DecryptRequestRequestTypeDef,
-    GenerateDataKeyPairRequestRequestTypeDef,
-    GenerateDataKeyRequestRequestTypeDef,
-    GenerateRandomRequestRequestTypeDef,
     DescribeCustomKeyStoresRequestDescribeCustomKeyStoresPaginateTypeDef,
     ListAliasesRequestListAliasesPaginateTypeDef,
     ListGrantsRequestListGrantsPaginateTypeDef,
     ListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef,
     ListKeysRequestListKeysPaginateTypeDef,
     ListResourceTagsRequestListResourceTagsPaginateTypeDef,
     ListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef,
+    GrantConstraintsUnionTypeDef,
     GrantListEntryTypeDef,
+    ImportKeyMaterialRequestRequestTypeDef,
     ListKeysResponseTypeDef,
     MultiRegionConfigurationTypeDef,
+    DecryptRequestRequestTypeDef,
+    GenerateDataKeyPairRequestRequestTypeDef,
+    GenerateDataKeyRequestRequestTypeDef,
+    GenerateRandomRequestRequestTypeDef,
     DescribeCustomKeyStoresResponseTypeDef,
     ListGrantsResponseTypeDef,
     KeyMetadataTypeDef,
     CreateKeyResponseTypeDef,
     DescribeKeyResponseTypeDef,
     ReplicateKeyResponseTypeDef,
 )
 
 
-def get_structure() -> AliasListEntryTypeDef:
+def get_value() -> AliasListEntryTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-kms-1.28.15.post1/mypy_boto3_kms.egg-info/SOURCES.txt` & `mypy-boto3-kms-1.28.16/mypy_boto3_kms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kms-1.28.15.post1/setup.py` & `mypy-boto3-kms-1.28.16/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-kms",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_kms"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.KMS 1.28.15 service generated with mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.KMS 1.28.16 service generated with mypy-boto3-builder 7.17.1"
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
-    keywords="boto3 kms type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 kms type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_kms": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

