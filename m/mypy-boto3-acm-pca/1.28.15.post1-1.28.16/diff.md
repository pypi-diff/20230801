# Comparing `tmp/mypy-boto3-acm-pca-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-acm-pca-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-acm-pca-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:23 2023, max compression
+gzip compressed data, was "mypy-boto3-acm-pca-1.28.16.tar", last modified: Tue Aug  1 11:36:04 2023, max compression
```

## Comparing `mypy-boto3-acm-pca-1.28.15.post1.tar` & `mypy-boto3-acm-pca-1.28.16.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:23.940978 mypy-boto3-acm-pca-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:37:30.000000 mypy-boto3-acm-pca-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17333 2023-07-29 10:02:23.940978 mypy-boto3-acm-pca-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15841 2023-07-29 09:37:30.000000 mypy-boto3-acm-pca-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:23.924978 mypy-boto3-acm-pca-1.28.15.post1/mypy_boto3_acm_pca/
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-07-29 09:37:30.000000 mypy-boto3-acm-pca-1.28.15.post1/mypy_boto3_acm_pca/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-07-29 09:37:30.000000 mypy-boto3-acm-pca-1.28.15.post1/mypy_boto3_acm_pca/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-07-29 09:37:30.000000 mypy-boto3-acm-pca-1.28.15.post1/mypy_boto3_acm_pca/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22510 2023-07-29 09:37:30.000000 mypy-boto3-acm-pca-1.28.15.post1/mypy_boto3_acm_pca/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    22474 2023-07-29 09:37:30.000000 mypy-boto3-acm-pca-1.28.15.post1/mypy_boto3_acm_pca/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11294 2023-07-29 09:37:31.000000 mypy-boto3-acm-pca-1.28.15.post1/mypy_boto3_acm_pca/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11292 2023-07-29 09:37:31.000000 mypy-boto3-acm-pca-1.28.15.post1/mypy_boto3_acm_pca/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-07-29 09:37:30.000000 mypy-boto3-acm-pca-1.28.15.post1/mypy_boto3_acm_pca/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-07-29 09:37:30.000000 mypy-boto3-acm-pca-1.28.15.post1/mypy_boto3_acm_pca/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:37:30.000000 mypy-boto3-acm-pca-1.28.15.post1/mypy_boto3_acm_pca/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    29584 2023-07-29 09:37:32.000000 mypy-boto3-acm-pca-1.28.15.post1/mypy_boto3_acm_pca/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    29539 2023-07-29 09:37:32.000000 mypy-boto3-acm-pca-1.28.15.post1/mypy_boto3_acm_pca/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:37:30.000000 mypy-boto3-acm-pca-1.28.15.post1/mypy_boto3_acm_pca/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-07-29 09:37:30.000000 mypy-boto3-acm-pca-1.28.15.post1/mypy_boto3_acm_pca/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-07-29 09:37:30.000000 mypy-boto3-acm-pca-1.28.15.post1/mypy_boto3_acm_pca/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:23.940978 mypy-boto3-acm-pca-1.28.15.post1/mypy_boto3_acm_pca.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17333 2023-07-29 10:02:23.000000 mypy-boto3-acm-pca-1.28.15.post1/mypy_boto3_acm_pca.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-29 10:02:23.000000 mypy-boto3-acm-pca-1.28.15.post1/mypy_boto3_acm_pca.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:23.000000 mypy-boto3-acm-pca-1.28.15.post1/mypy_boto3_acm_pca.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:23.000000 mypy-boto3-acm-pca-1.28.15.post1/mypy_boto3_acm_pca.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:23.000000 mypy-boto3-acm-pca-1.28.15.post1/mypy_boto3_acm_pca.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-29 10:02:23.000000 mypy-boto3-acm-pca-1.28.15.post1/mypy_boto3_acm_pca.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:23.940978 mypy-boto3-acm-pca-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-07-29 09:37:30.000000 mypy-boto3-acm-pca-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:04.784961 mypy-boto3-acm-pca-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:09:59.000000 mypy-boto3-acm-pca-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17391 2023-08-01 11:36:04.784961 mypy-boto3-acm-pca-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15908 2023-08-01 11:09:59.000000 mypy-boto3-acm-pca-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:04.776961 mypy-boto3-acm-pca-1.28.16/mypy_boto3_acm_pca/
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-08-01 11:09:59.000000 mypy-boto3-acm-pca-1.28.16/mypy_boto3_acm_pca/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-08-01 11:09:59.000000 mypy-boto3-acm-pca-1.28.16/mypy_boto3_acm_pca/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-08-01 11:10:00.000000 mypy-boto3-acm-pca-1.28.16/mypy_boto3_acm_pca/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22263 2023-08-01 11:10:00.000000 mypy-boto3-acm-pca-1.28.16/mypy_boto3_acm_pca/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22227 2023-08-01 11:10:00.000000 mypy-boto3-acm-pca-1.28.16/mypy_boto3_acm_pca/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11294 2023-08-01 11:10:01.000000 mypy-boto3-acm-pca-1.28.16/mypy_boto3_acm_pca/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11292 2023-08-01 11:10:01.000000 mypy-boto3-acm-pca-1.28.16/mypy_boto3_acm_pca/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-08-01 11:10:00.000000 mypy-boto3-acm-pca-1.28.16/mypy_boto3_acm_pca/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-08-01 11:10:00.000000 mypy-boto3-acm-pca-1.28.16/mypy_boto3_acm_pca/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:10:00.000000 mypy-boto3-acm-pca-1.28.16/mypy_boto3_acm_pca/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    29770 2023-08-01 11:10:02.000000 mypy-boto3-acm-pca-1.28.16/mypy_boto3_acm_pca/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29725 2023-08-01 11:10:01.000000 mypy-boto3-acm-pca-1.28.16/mypy_boto3_acm_pca/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:09:59.000000 mypy-boto3-acm-pca-1.28.16/mypy_boto3_acm_pca/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-08-01 11:10:00.000000 mypy-boto3-acm-pca-1.28.16/mypy_boto3_acm_pca/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-08-01 11:10:00.000000 mypy-boto3-acm-pca-1.28.16/mypy_boto3_acm_pca/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:04.780961 mypy-boto3-acm-pca-1.28.16/mypy_boto3_acm_pca.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17391 2023-08-01 11:36:04.000000 mypy-boto3-acm-pca-1.28.16/mypy_boto3_acm_pca.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-08-01 11:36:04.000000 mypy-boto3-acm-pca-1.28.16/mypy_boto3_acm_pca.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:04.000000 mypy-boto3-acm-pca-1.28.16/mypy_boto3_acm_pca.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:04.000000 mypy-boto3-acm-pca-1.28.16/mypy_boto3_acm_pca.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:04.000000 mypy-boto3-acm-pca-1.28.16/mypy_boto3_acm_pca.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-01 11:36:04.000000 mypy-boto3-acm-pca-1.28.16/mypy_boto3_acm_pca.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:04.784961 mypy-boto3-acm-pca-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-08-01 11:09:59.000000 mypy-boto3-acm-pca-1.28.16/setup.py
```

### Comparing `mypy-boto3-acm-pca-1.28.15.post1/LICENSE` & `mypy-boto3-acm-pca-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-pca-1.28.15.post1/PKG-INFO` & `mypy-boto3-acm-pca-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-acm-pca
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.ACMPCA 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.ACMPCA 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm_pca/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 acm-pca type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 acm-pca type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-acm-pca.svg?color=blue)](https://pypi.org/project/mypy-boto3-acm-pca)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm_pca/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-acm-pca)](https://pepy.tech/project/mypy-boto3-acm-pca)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ACMPCA 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA)
+[boto3.ACMPCA 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA)
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
 [mypy-boto3-acm-pca docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm_pca/).
 
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
@@ -368,25 +368,26 @@
 )
 
 
 def check_value(value: AccessMethodTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_acm_pca.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_acm_pca.type_defs import (
     CustomAttributeTypeDef,
     AccessMethodTypeDef,
+    BlobTypeDef,
     CreateCertificateAuthorityAuditReportRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     TagTypeDef,
     CreatePermissionRequestRequestTypeDef,
     CrlConfigurationTypeDef,
     KeyUsageTypeDef,
     CustomExtensionTypeDef,
@@ -399,28 +400,28 @@
     EdiPartyNameTypeDef,
     ExtendedKeyUsageTypeDef,
     OtherNameTypeDef,
     GetCertificateAuthorityCertificateRequestRequestTypeDef,
     GetCertificateAuthorityCsrRequestRequestTypeDef,
     GetCertificateRequestRequestTypeDef,
     GetPolicyRequestRequestTypeDef,
-    ImportCertificateAuthorityCertificateRequestRequestTypeDef,
     ValidityTypeDef,
     PaginatorConfigTypeDef,
     ListCertificateAuthoritiesRequestRequestTypeDef,
     ListPermissionsRequestRequestTypeDef,
     PermissionTypeDef,
     ListTagsRequestRequestTypeDef,
     OcspConfigurationTypeDef,
     QualifierTypeDef,
     PutPolicyRequestRequestTypeDef,
     RestoreCertificateAuthorityRequestRequestTypeDef,
     RevokeCertificateRequestRequestTypeDef,
     ASN1SubjectOutputTypeDef,
     ASN1SubjectTypeDef,
+    ImportCertificateAuthorityCertificateRequestRequestTypeDef,
     CreateCertificateAuthorityAuditReportResponseTypeDef,
     CreateCertificateAuthorityResponseTypeDef,
     DescribeCertificateAuthorityAuditReportResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetCertificateAuthorityCertificateResponseTypeDef,
     GetCertificateAuthorityCsrResponseTypeDef,
     GetCertificateResponseTypeDef,
@@ -448,21 +449,22 @@
     CsrExtensionsOutputTypeDef,
     CsrExtensionsTypeDef,
     ApiPassthroughTypeDef,
     CertificateAuthorityConfigurationOutputTypeDef,
     CertificateAuthorityConfigurationTypeDef,
     IssueCertificateRequestRequestTypeDef,
     CertificateAuthorityTypeDef,
+    CertificateAuthorityConfigurationUnionTypeDef,
     CreateCertificateAuthorityRequestRequestTypeDef,
     DescribeCertificateAuthorityResponseTypeDef,
     ListCertificateAuthoritiesResponseTypeDef,
 )
 
 
-def get_structure() -> CustomAttributeTypeDef:
+def get_value() -> CustomAttributeTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-acm-pca-1.28.15.post1/README.md` & `mypy-boto3-acm-pca-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-acm-pca.svg?color=blue)](https://pypi.org/project/mypy-boto3-acm-pca)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm_pca/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-acm-pca)](https://pepy.tech/project/mypy-boto3-acm-pca)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ACMPCA 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA)
+[boto3.ACMPCA 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA)
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
 [mypy-boto3-acm-pca docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm_pca/).
 
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
@@ -336,25 +336,26 @@
 )
 
 
 def check_value(value: AccessMethodTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_acm_pca.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_acm_pca.type_defs import (
     CustomAttributeTypeDef,
     AccessMethodTypeDef,
+    BlobTypeDef,
     CreateCertificateAuthorityAuditReportRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     TagTypeDef,
     CreatePermissionRequestRequestTypeDef,
     CrlConfigurationTypeDef,
     KeyUsageTypeDef,
     CustomExtensionTypeDef,
@@ -367,28 +368,28 @@
     EdiPartyNameTypeDef,
     ExtendedKeyUsageTypeDef,
     OtherNameTypeDef,
     GetCertificateAuthorityCertificateRequestRequestTypeDef,
     GetCertificateAuthorityCsrRequestRequestTypeDef,
     GetCertificateRequestRequestTypeDef,
     GetPolicyRequestRequestTypeDef,
-    ImportCertificateAuthorityCertificateRequestRequestTypeDef,
     ValidityTypeDef,
     PaginatorConfigTypeDef,
     ListCertificateAuthoritiesRequestRequestTypeDef,
     ListPermissionsRequestRequestTypeDef,
     PermissionTypeDef,
     ListTagsRequestRequestTypeDef,
     OcspConfigurationTypeDef,
     QualifierTypeDef,
     PutPolicyRequestRequestTypeDef,
     RestoreCertificateAuthorityRequestRequestTypeDef,
     RevokeCertificateRequestRequestTypeDef,
     ASN1SubjectOutputTypeDef,
     ASN1SubjectTypeDef,
+    ImportCertificateAuthorityCertificateRequestRequestTypeDef,
     CreateCertificateAuthorityAuditReportResponseTypeDef,
     CreateCertificateAuthorityResponseTypeDef,
     DescribeCertificateAuthorityAuditReportResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetCertificateAuthorityCertificateResponseTypeDef,
     GetCertificateAuthorityCsrResponseTypeDef,
     GetCertificateResponseTypeDef,
@@ -416,21 +417,22 @@
     CsrExtensionsOutputTypeDef,
     CsrExtensionsTypeDef,
     ApiPassthroughTypeDef,
     CertificateAuthorityConfigurationOutputTypeDef,
     CertificateAuthorityConfigurationTypeDef,
     IssueCertificateRequestRequestTypeDef,
     CertificateAuthorityTypeDef,
+    CertificateAuthorityConfigurationUnionTypeDef,
     CreateCertificateAuthorityRequestRequestTypeDef,
     DescribeCertificateAuthorityResponseTypeDef,
     ListCertificateAuthoritiesResponseTypeDef,
 )
 
 
-def get_structure() -> CustomAttributeTypeDef:
+def get_value() -> CustomAttributeTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-acm-pca-1.28.15.post1/mypy_boto3_acm_pca/__init__.py` & `mypy-boto3-acm-pca-1.28.16/mypy_boto3_acm_pca/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-pca-1.28.15.post1/mypy_boto3_acm_pca/__init__.pyi` & `mypy-boto3-acm-pca-1.28.16/mypy_boto3_acm_pca/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-pca-1.28.15.post1/mypy_boto3_acm_pca/__main__.py` & `mypy-boto3-acm-pca-1.28.16/mypy_boto3_acm_pca/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ACMPCA 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.ACMPCA 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm_pca//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA\nOther"
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

### Comparing `mypy-boto3-acm-pca-1.28.15.post1/mypy_boto3_acm_pca/client.py` & `mypy-boto3-acm-pca-1.28.16/mypy_boto3_acm_pca/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,18 +10,17 @@
     from mypy_boto3_acm_pca.client import ACMPCAClient
 
     session = Session()
     client: ACMPCAClient = session.client("acm-pca")
     ```
 """
 import sys
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
-from botocore.response import StreamingBody
 
 from .literals import (
     ActionTypeType,
     AuditReportResponseFormatType,
     CertificateAuthorityStatusType,
     CertificateAuthorityTypeType,
     CertificateAuthorityUsageModeType,
@@ -33,16 +32,16 @@
 from .paginator import (
     ListCertificateAuthoritiesPaginator,
     ListPermissionsPaginator,
     ListTagsPaginator,
 )
 from .type_defs import (
     ApiPassthroughTypeDef,
-    CertificateAuthorityConfigurationOutputTypeDef,
-    CertificateAuthorityConfigurationTypeDef,
+    BlobTypeDef,
+    CertificateAuthorityConfigurationUnionTypeDef,
     CreateCertificateAuthorityAuditReportResponseTypeDef,
     CreateCertificateAuthorityResponseTypeDef,
     DescribeCertificateAuthorityAuditReportResponseTypeDef,
     DescribeCertificateAuthorityResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetCertificateAuthorityCertificateResponseTypeDef,
     GetCertificateAuthorityCsrResponseTypeDef,
@@ -134,17 +133,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm_pca/client/#close)
         """
 
     def create_certificate_authority(
         self,
         *,
-        CertificateAuthorityConfiguration: Union[
-            CertificateAuthorityConfigurationTypeDef, CertificateAuthorityConfigurationOutputTypeDef
-        ],
+        CertificateAuthorityConfiguration: CertificateAuthorityConfigurationUnionTypeDef,
         CertificateAuthorityType: CertificateAuthorityTypeType,
         RevocationConfiguration: RevocationConfigurationTypeDef = ...,
         IdempotencyToken: str = ...,
         KeyStorageSecurityStandard: KeyStorageSecurityStandardType = ...,
         Tags: Sequence[TagTypeDef] = ...,
         UsageMode: CertificateAuthorityUsageModeType = ...
     ) -> CreateCertificateAuthorityResponseTypeDef:
@@ -292,29 +289,29 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm_pca/client/#get_policy)
         """
 
     def import_certificate_authority_certificate(
         self,
         *,
         CertificateAuthorityArn: str,
-        Certificate: Union[str, bytes, IO[Any], StreamingBody],
-        CertificateChain: Union[str, bytes, IO[Any], StreamingBody] = ...
+        Certificate: BlobTypeDef,
+        CertificateChain: BlobTypeDef = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Imports a signed private CA certificate into Amazon Web Services Private CA.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA.Client.import_certificate_authority_certificate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm_pca/client/#import_certificate_authority_certificate)
         """
 
     def issue_certificate(
         self,
         *,
         CertificateAuthorityArn: str,
-        Csr: Union[str, bytes, IO[Any], StreamingBody],
+        Csr: BlobTypeDef,
         SigningAlgorithm: SigningAlgorithmType,
         Validity: ValidityTypeDef,
         ApiPassthrough: ApiPassthroughTypeDef = ...,
         TemplateArn: str = ...,
         ValidityNotBefore: ValidityTypeDef = ...,
         IdempotencyToken: str = ...
     ) -> IssueCertificateResponseTypeDef:
```

### Comparing `mypy-boto3-acm-pca-1.28.15.post1/mypy_boto3_acm_pca/client.pyi` & `mypy-boto3-acm-pca-1.28.16/mypy_boto3_acm_pca/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -10,18 +10,17 @@
     from mypy_boto3_acm_pca.client import ACMPCAClient
 
     session = Session()
     client: ACMPCAClient = session.client("acm-pca")
     ```
 """
 import sys
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
-from botocore.response import StreamingBody
 
 from .literals import (
     ActionTypeType,
     AuditReportResponseFormatType,
     CertificateAuthorityStatusType,
     CertificateAuthorityTypeType,
     CertificateAuthorityUsageModeType,
@@ -33,16 +32,16 @@
 from .paginator import (
     ListCertificateAuthoritiesPaginator,
     ListPermissionsPaginator,
     ListTagsPaginator,
 )
 from .type_defs import (
     ApiPassthroughTypeDef,
-    CertificateAuthorityConfigurationOutputTypeDef,
-    CertificateAuthorityConfigurationTypeDef,
+    BlobTypeDef,
+    CertificateAuthorityConfigurationUnionTypeDef,
     CreateCertificateAuthorityAuditReportResponseTypeDef,
     CreateCertificateAuthorityResponseTypeDef,
     DescribeCertificateAuthorityAuditReportResponseTypeDef,
     DescribeCertificateAuthorityResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetCertificateAuthorityCertificateResponseTypeDef,
     GetCertificateAuthorityCsrResponseTypeDef,
@@ -127,17 +126,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm_pca/client/#close)
         """
     def create_certificate_authority(
         self,
         *,
-        CertificateAuthorityConfiguration: Union[
-            CertificateAuthorityConfigurationTypeDef, CertificateAuthorityConfigurationOutputTypeDef
-        ],
+        CertificateAuthorityConfiguration: CertificateAuthorityConfigurationUnionTypeDef,
         CertificateAuthorityType: CertificateAuthorityTypeType,
         RevocationConfiguration: RevocationConfigurationTypeDef = ...,
         IdempotencyToken: str = ...,
         KeyStorageSecurityStandard: KeyStorageSecurityStandardType = ...,
         Tags: Sequence[TagTypeDef] = ...,
         UsageMode: CertificateAuthorityUsageModeType = ...
     ) -> CreateCertificateAuthorityResponseTypeDef:
@@ -272,28 +269,28 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA.Client.get_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm_pca/client/#get_policy)
         """
     def import_certificate_authority_certificate(
         self,
         *,
         CertificateAuthorityArn: str,
-        Certificate: Union[str, bytes, IO[Any], StreamingBody],
-        CertificateChain: Union[str, bytes, IO[Any], StreamingBody] = ...
+        Certificate: BlobTypeDef,
+        CertificateChain: BlobTypeDef = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Imports a signed private CA certificate into Amazon Web Services Private CA.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA.Client.import_certificate_authority_certificate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm_pca/client/#import_certificate_authority_certificate)
         """
     def issue_certificate(
         self,
         *,
         CertificateAuthorityArn: str,
-        Csr: Union[str, bytes, IO[Any], StreamingBody],
+        Csr: BlobTypeDef,
         SigningAlgorithm: SigningAlgorithmType,
         Validity: ValidityTypeDef,
         ApiPassthrough: ApiPassthroughTypeDef = ...,
         TemplateArn: str = ...,
         ValidityNotBefore: ValidityTypeDef = ...,
         IdempotencyToken: str = ...
     ) -> IssueCertificateResponseTypeDef:
```

### Comparing `mypy-boto3-acm-pca-1.28.15.post1/mypy_boto3_acm_pca/literals.py` & `mypy-boto3-acm-pca-1.28.16/mypy_boto3_acm_pca/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-pca-1.28.15.post1/mypy_boto3_acm_pca/literals.pyi` & `mypy-boto3-acm-pca-1.28.16/mypy_boto3_acm_pca/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-pca-1.28.15.post1/mypy_boto3_acm_pca/paginator.py` & `mypy-boto3-acm-pca-1.28.16/mypy_boto3_acm_pca/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-pca-1.28.15.post1/mypy_boto3_acm_pca/paginator.pyi` & `mypy-boto3-acm-pca-1.28.16/mypy_boto3_acm_pca/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-pca-1.28.15.post1/mypy_boto3_acm_pca/type_defs.py` & `mypy-boto3-acm-pca-1.28.16/mypy_boto3_acm_pca/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm_pca/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_acm_pca.type_defs import CustomAttributeTypeDef
 
-    data: CustomAttributeTypeDef = {...}
+    data: CustomAttributeTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -41,18 +41,18 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "CustomAttributeTypeDef",
     "AccessMethodTypeDef",
+    "BlobTypeDef",
     "CreateCertificateAuthorityAuditReportRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "TagTypeDef",
     "CreatePermissionRequestRequestTypeDef",
     "CrlConfigurationTypeDef",
     "KeyUsageTypeDef",
     "CustomExtensionTypeDef",
@@ -65,28 +65,28 @@
     "EdiPartyNameTypeDef",
     "ExtendedKeyUsageTypeDef",
     "OtherNameTypeDef",
     "GetCertificateAuthorityCertificateRequestRequestTypeDef",
     "GetCertificateAuthorityCsrRequestRequestTypeDef",
     "GetCertificateRequestRequestTypeDef",
     "GetPolicyRequestRequestTypeDef",
-    "ImportCertificateAuthorityCertificateRequestRequestTypeDef",
     "ValidityTypeDef",
     "PaginatorConfigTypeDef",
     "ListCertificateAuthoritiesRequestRequestTypeDef",
     "ListPermissionsRequestRequestTypeDef",
     "PermissionTypeDef",
     "ListTagsRequestRequestTypeDef",
     "OcspConfigurationTypeDef",
     "QualifierTypeDef",
     "PutPolicyRequestRequestTypeDef",
     "RestoreCertificateAuthorityRequestRequestTypeDef",
     "RevokeCertificateRequestRequestTypeDef",
     "ASN1SubjectOutputTypeDef",
     "ASN1SubjectTypeDef",
+    "ImportCertificateAuthorityCertificateRequestRequestTypeDef",
     "CreateCertificateAuthorityAuditReportResponseTypeDef",
     "CreateCertificateAuthorityResponseTypeDef",
     "DescribeCertificateAuthorityAuditReportResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetCertificateAuthorityCertificateResponseTypeDef",
     "GetCertificateAuthorityCsrResponseTypeDef",
     "GetCertificateResponseTypeDef",
@@ -114,14 +114,15 @@
     "CsrExtensionsOutputTypeDef",
     "CsrExtensionsTypeDef",
     "ApiPassthroughTypeDef",
     "CertificateAuthorityConfigurationOutputTypeDef",
     "CertificateAuthorityConfigurationTypeDef",
     "IssueCertificateRequestRequestTypeDef",
     "CertificateAuthorityTypeDef",
+    "CertificateAuthorityConfigurationUnionTypeDef",
     "CreateCertificateAuthorityRequestRequestTypeDef",
     "DescribeCertificateAuthorityResponseTypeDef",
     "ListCertificateAuthoritiesResponseTypeDef",
 )
 
 CustomAttributeTypeDef = TypedDict(
     "CustomAttributeTypeDef",
@@ -136,14 +137,15 @@
     {
         "CustomObjectIdentifier": str,
         "AccessMethodType": AccessMethodTypeType,
     },
     total=False,
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 CreateCertificateAuthorityAuditReportRequestRequestTypeDef = TypedDict(
     "CreateCertificateAuthorityAuditReportRequestRequestTypeDef",
     {
         "CertificateAuthorityArn": str,
         "S3BucketName": str,
         "AuditReportResponseFormat": AuditReportResponseFormatType,
     },
@@ -170,19 +172,17 @@
     "_OptionalTagTypeDef",
     {
         "Value": str,
     },
     total=False,
 )
 
-
 class TagTypeDef(_RequiredTagTypeDef, _OptionalTagTypeDef):
     pass
 
-
 _RequiredCreatePermissionRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePermissionRequestRequestTypeDef",
     {
         "CertificateAuthorityArn": str,
         "Principal": str,
         "Actions": Sequence[ActionTypeType],
     },
@@ -191,21 +191,19 @@
     "_OptionalCreatePermissionRequestRequestTypeDef",
     {
         "SourceAccount": str,
     },
     total=False,
 )
 
-
 class CreatePermissionRequestRequestTypeDef(
     _RequiredCreatePermissionRequestRequestTypeDef, _OptionalCreatePermissionRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredCrlConfigurationTypeDef = TypedDict(
     "_RequiredCrlConfigurationTypeDef",
     {
         "Enabled": bool,
     },
 )
 _OptionalCrlConfigurationTypeDef = TypedDict(
@@ -215,19 +213,17 @@
         "CustomCname": str,
         "S3BucketName": str,
         "S3ObjectAcl": S3ObjectAclType,
     },
     total=False,
 )
 
-
 class CrlConfigurationTypeDef(_RequiredCrlConfigurationTypeDef, _OptionalCrlConfigurationTypeDef):
     pass
 
-
 KeyUsageTypeDef = TypedDict(
     "KeyUsageTypeDef",
     {
         "DigitalSignature": bool,
         "NonRepudiation": bool,
         "KeyEncipherment": bool,
         "DataEncipherment": bool,
@@ -251,41 +247,37 @@
     "_OptionalCustomExtensionTypeDef",
     {
         "Critical": bool,
     },
     total=False,
 )
 
-
 class CustomExtensionTypeDef(_RequiredCustomExtensionTypeDef, _OptionalCustomExtensionTypeDef):
     pass
 
-
 _RequiredDeleteCertificateAuthorityRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteCertificateAuthorityRequestRequestTypeDef",
     {
         "CertificateAuthorityArn": str,
     },
 )
 _OptionalDeleteCertificateAuthorityRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteCertificateAuthorityRequestRequestTypeDef",
     {
         "PermanentDeletionTimeInDays": int,
     },
     total=False,
 )
 
-
 class DeleteCertificateAuthorityRequestRequestTypeDef(
     _RequiredDeleteCertificateAuthorityRequestRequestTypeDef,
     _OptionalDeleteCertificateAuthorityRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDeletePermissionRequestRequestTypeDef = TypedDict(
     "_RequiredDeletePermissionRequestRequestTypeDef",
     {
         "CertificateAuthorityArn": str,
         "Principal": str,
     },
 )
@@ -293,21 +285,19 @@
     "_OptionalDeletePermissionRequestRequestTypeDef",
     {
         "SourceAccount": str,
     },
     total=False,
 )
 
-
 class DeletePermissionRequestRequestTypeDef(
     _RequiredDeletePermissionRequestRequestTypeDef, _OptionalDeletePermissionRequestRequestTypeDef
 ):
     pass
 
-
 DeletePolicyRequestRequestTypeDef = TypedDict(
     "DeletePolicyRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
@@ -345,19 +335,17 @@
     "_OptionalEdiPartyNameTypeDef",
     {
         "NameAssigner": str,
     },
     total=False,
 )
 
-
 class EdiPartyNameTypeDef(_RequiredEdiPartyNameTypeDef, _OptionalEdiPartyNameTypeDef):
     pass
 
-
 ExtendedKeyUsageTypeDef = TypedDict(
     "ExtendedKeyUsageTypeDef",
     {
         "ExtendedKeyUsageType": ExtendedKeyUsageTypeType,
         "ExtendedKeyUsageObjectIdentifier": str,
     },
     total=False,
@@ -396,37 +384,14 @@
 GetPolicyRequestRequestTypeDef = TypedDict(
     "GetPolicyRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-_RequiredImportCertificateAuthorityCertificateRequestRequestTypeDef = TypedDict(
-    "_RequiredImportCertificateAuthorityCertificateRequestRequestTypeDef",
-    {
-        "CertificateAuthorityArn": str,
-        "Certificate": Union[str, bytes, IO[Any], StreamingBody],
-    },
-)
-_OptionalImportCertificateAuthorityCertificateRequestRequestTypeDef = TypedDict(
-    "_OptionalImportCertificateAuthorityCertificateRequestRequestTypeDef",
-    {
-        "CertificateChain": Union[str, bytes, IO[Any], StreamingBody],
-    },
-    total=False,
-)
-
-
-class ImportCertificateAuthorityCertificateRequestRequestTypeDef(
-    _RequiredImportCertificateAuthorityCertificateRequestRequestTypeDef,
-    _OptionalImportCertificateAuthorityCertificateRequestRequestTypeDef,
-):
-    pass
-
-
 ValidityTypeDef = TypedDict(
     "ValidityTypeDef",
     {
         "Value": int,
         "Type": ValidityPeriodTypeType,
     },
 )
@@ -462,21 +427,19 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListPermissionsRequestRequestTypeDef(
     _RequiredListPermissionsRequestRequestTypeDef, _OptionalListPermissionsRequestRequestTypeDef
 ):
     pass
 
-
 PermissionTypeDef = TypedDict(
     "PermissionTypeDef",
     {
         "CertificateAuthorityArn": str,
         "CreatedAt": datetime,
         "Principal": str,
         "SourceAccount": str,
@@ -497,42 +460,38 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListTagsRequestRequestTypeDef(
     _RequiredListTagsRequestRequestTypeDef, _OptionalListTagsRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredOcspConfigurationTypeDef = TypedDict(
     "_RequiredOcspConfigurationTypeDef",
     {
         "Enabled": bool,
     },
 )
 _OptionalOcspConfigurationTypeDef = TypedDict(
     "_OptionalOcspConfigurationTypeDef",
     {
         "OcspCustomCname": str,
     },
     total=False,
 )
 
-
 class OcspConfigurationTypeDef(
     _RequiredOcspConfigurationTypeDef, _OptionalOcspConfigurationTypeDef
 ):
     pass
 
-
 QualifierTypeDef = TypedDict(
     "QualifierTypeDef",
     {
         "CpsUri": str,
     },
 )
 
@@ -600,14 +559,35 @@
         "Pseudonym": str,
         "GenerationQualifier": str,
         "CustomAttributes": Sequence[CustomAttributeTypeDef],
     },
     total=False,
 )
 
+_RequiredImportCertificateAuthorityCertificateRequestRequestTypeDef = TypedDict(
+    "_RequiredImportCertificateAuthorityCertificateRequestRequestTypeDef",
+    {
+        "CertificateAuthorityArn": str,
+        "Certificate": BlobTypeDef,
+    },
+)
+_OptionalImportCertificateAuthorityCertificateRequestRequestTypeDef = TypedDict(
+    "_OptionalImportCertificateAuthorityCertificateRequestRequestTypeDef",
+    {
+        "CertificateChain": BlobTypeDef,
+    },
+    total=False,
+)
+
+class ImportCertificateAuthorityCertificateRequestRequestTypeDef(
+    _RequiredImportCertificateAuthorityCertificateRequestRequestTypeDef,
+    _OptionalImportCertificateAuthorityCertificateRequestRequestTypeDef,
+):
+    pass
+
 CreateCertificateAuthorityAuditReportResponseTypeDef = TypedDict(
     "CreateCertificateAuthorityAuditReportResponseTypeDef",
     {
         "AuditReportId": str,
         "S3Key": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -717,44 +697,40 @@
     "_OptionalDescribeCertificateAuthorityAuditReportRequestAuditReportCreatedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeCertificateAuthorityAuditReportRequestAuditReportCreatedWaitTypeDef(
     _RequiredDescribeCertificateAuthorityAuditReportRequestAuditReportCreatedWaitTypeDef,
     _OptionalDescribeCertificateAuthorityAuditReportRequestAuditReportCreatedWaitTypeDef,
 ):
     pass
 
-
 _RequiredGetCertificateAuthorityCsrRequestCertificateAuthorityCSRCreatedWaitTypeDef = TypedDict(
     "_RequiredGetCertificateAuthorityCsrRequestCertificateAuthorityCSRCreatedWaitTypeDef",
     {
         "CertificateAuthorityArn": str,
     },
 )
 _OptionalGetCertificateAuthorityCsrRequestCertificateAuthorityCSRCreatedWaitTypeDef = TypedDict(
     "_OptionalGetCertificateAuthorityCsrRequestCertificateAuthorityCSRCreatedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetCertificateAuthorityCsrRequestCertificateAuthorityCSRCreatedWaitTypeDef(
     _RequiredGetCertificateAuthorityCsrRequestCertificateAuthorityCSRCreatedWaitTypeDef,
     _OptionalGetCertificateAuthorityCsrRequestCertificateAuthorityCSRCreatedWaitTypeDef,
 ):
     pass
 
-
 _RequiredGetCertificateRequestCertificateIssuedWaitTypeDef = TypedDict(
     "_RequiredGetCertificateRequestCertificateIssuedWaitTypeDef",
     {
         "CertificateAuthorityArn": str,
         "CertificateArn": str,
     },
 )
@@ -762,22 +738,20 @@
     "_OptionalGetCertificateRequestCertificateIssuedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetCertificateRequestCertificateIssuedWaitTypeDef(
     _RequiredGetCertificateRequestCertificateIssuedWaitTypeDef,
     _OptionalGetCertificateRequestCertificateIssuedWaitTypeDef,
 ):
     pass
 
-
 ListCertificateAuthoritiesRequestListCertificateAuthoritiesPaginateTypeDef = TypedDict(
     "ListCertificateAuthoritiesRequestListCertificateAuthoritiesPaginateTypeDef",
     {
         "ResourceOwner": ResourceOwnerType,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -793,43 +767,39 @@
     "_OptionalListPermissionsRequestListPermissionsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListPermissionsRequestListPermissionsPaginateTypeDef(
     _RequiredListPermissionsRequestListPermissionsPaginateTypeDef,
     _OptionalListPermissionsRequestListPermissionsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListTagsRequestListTagsPaginateTypeDef = TypedDict(
     "_RequiredListTagsRequestListTagsPaginateTypeDef",
     {
         "CertificateAuthorityArn": str,
     },
 )
 _OptionalListTagsRequestListTagsPaginateTypeDef = TypedDict(
     "_OptionalListTagsRequestListTagsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListTagsRequestListTagsPaginateTypeDef(
     _RequiredListTagsRequestListTagsPaginateTypeDef, _OptionalListTagsRequestListTagsPaginateTypeDef
 ):
     pass
 
-
 ListPermissionsResponseTypeDef = TypedDict(
     "ListPermissionsResponseTypeDef",
     {
         "Permissions": List[PermissionTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -893,43 +863,39 @@
     {
         "RevocationConfiguration": RevocationConfigurationTypeDef,
         "Status": CertificateAuthorityStatusType,
     },
     total=False,
 )
 
-
 class UpdateCertificateAuthorityRequestRequestTypeDef(
     _RequiredUpdateCertificateAuthorityRequestRequestTypeDef,
     _OptionalUpdateCertificateAuthorityRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredPolicyInformationTypeDef = TypedDict(
     "_RequiredPolicyInformationTypeDef",
     {
         "CertPolicyId": str,
     },
 )
 _OptionalPolicyInformationTypeDef = TypedDict(
     "_OptionalPolicyInformationTypeDef",
     {
         "PolicyQualifiers": Sequence[PolicyQualifierInfoTypeDef],
     },
     total=False,
 )
 
-
 class PolicyInformationTypeDef(
     _RequiredPolicyInformationTypeDef, _OptionalPolicyInformationTypeDef
 ):
     pass
 
-
 AccessDescriptionOutputTypeDef = TypedDict(
     "AccessDescriptionOutputTypeDef",
     {
         "AccessMethod": AccessMethodTypeDef,
         "AccessLocation": GeneralNameOutputTypeDef,
     },
 )
@@ -993,22 +959,20 @@
     "_OptionalCertificateAuthorityConfigurationOutputTypeDef",
     {
         "CsrExtensions": CsrExtensionsOutputTypeDef,
     },
     total=False,
 )
 
-
 class CertificateAuthorityConfigurationOutputTypeDef(
     _RequiredCertificateAuthorityConfigurationOutputTypeDef,
     _OptionalCertificateAuthorityConfigurationOutputTypeDef,
 ):
     pass
 
-
 _RequiredCertificateAuthorityConfigurationTypeDef = TypedDict(
     "_RequiredCertificateAuthorityConfigurationTypeDef",
     {
         "KeyAlgorithm": KeyAlgorithmType,
         "SigningAlgorithm": SigningAlgorithmType,
         "Subject": ASN1SubjectTypeDef,
     },
@@ -1017,27 +981,25 @@
     "_OptionalCertificateAuthorityConfigurationTypeDef",
     {
         "CsrExtensions": CsrExtensionsTypeDef,
     },
     total=False,
 )
 
-
 class CertificateAuthorityConfigurationTypeDef(
     _RequiredCertificateAuthorityConfigurationTypeDef,
     _OptionalCertificateAuthorityConfigurationTypeDef,
 ):
     pass
 
-
 _RequiredIssueCertificateRequestRequestTypeDef = TypedDict(
     "_RequiredIssueCertificateRequestRequestTypeDef",
     {
         "CertificateAuthorityArn": str,
-        "Csr": Union[str, bytes, IO[Any], StreamingBody],
+        "Csr": BlobTypeDef,
         "SigningAlgorithm": SigningAlgorithmType,
         "Validity": ValidityTypeDef,
     },
 )
 _OptionalIssueCertificateRequestRequestTypeDef = TypedDict(
     "_OptionalIssueCertificateRequestRequestTypeDef",
     {
@@ -1045,21 +1007,19 @@
         "TemplateArn": str,
         "ValidityNotBefore": ValidityTypeDef,
         "IdempotencyToken": str,
     },
     total=False,
 )
 
-
 class IssueCertificateRequestRequestTypeDef(
     _RequiredIssueCertificateRequestRequestTypeDef, _OptionalIssueCertificateRequestRequestTypeDef
 ):
     pass
 
-
 CertificateAuthorityTypeDef = TypedDict(
     "CertificateAuthorityTypeDef",
     {
         "Arn": str,
         "OwnerAccount": str,
         "CreatedAt": datetime,
         "LastStateChangeAt": datetime,
@@ -1074,14 +1034,17 @@
         "RestorableUntil": datetime,
         "KeyStorageSecurityStandard": KeyStorageSecurityStandardType,
         "UsageMode": CertificateAuthorityUsageModeType,
     },
     total=False,
 )
 
+CertificateAuthorityConfigurationUnionTypeDef = Union[
+    CertificateAuthorityConfigurationTypeDef, CertificateAuthorityConfigurationOutputTypeDef
+]
 _RequiredCreateCertificateAuthorityRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCertificateAuthorityRequestRequestTypeDef",
     {
         "CertificateAuthorityConfiguration": CertificateAuthorityConfigurationTypeDef,
         "CertificateAuthorityType": CertificateAuthorityTypeType,
     },
 )
@@ -1093,22 +1056,20 @@
         "KeyStorageSecurityStandard": KeyStorageSecurityStandardType,
         "Tags": Sequence[TagTypeDef],
         "UsageMode": CertificateAuthorityUsageModeType,
     },
     total=False,
 )
 
-
 class CreateCertificateAuthorityRequestRequestTypeDef(
     _RequiredCreateCertificateAuthorityRequestRequestTypeDef,
     _OptionalCreateCertificateAuthorityRequestRequestTypeDef,
 ):
     pass
 
-
 DescribeCertificateAuthorityResponseTypeDef = TypedDict(
     "DescribeCertificateAuthorityResponseTypeDef",
     {
         "CertificateAuthority": CertificateAuthorityTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-acm-pca-1.28.15.post1/mypy_boto3_acm_pca/type_defs.pyi` & `mypy-boto3-acm-pca-1.28.16/mypy_boto3_acm_pca/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm_pca/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_acm_pca.type_defs import CustomAttributeTypeDef
 
-    data: CustomAttributeTypeDef = {...}
+    data: CustomAttributeTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -41,17 +41,19 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "CustomAttributeTypeDef",
     "AccessMethodTypeDef",
+    "BlobTypeDef",
     "CreateCertificateAuthorityAuditReportRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "TagTypeDef",
     "CreatePermissionRequestRequestTypeDef",
     "CrlConfigurationTypeDef",
     "KeyUsageTypeDef",
     "CustomExtensionTypeDef",
@@ -64,28 +66,28 @@
     "EdiPartyNameTypeDef",
     "ExtendedKeyUsageTypeDef",
     "OtherNameTypeDef",
     "GetCertificateAuthorityCertificateRequestRequestTypeDef",
     "GetCertificateAuthorityCsrRequestRequestTypeDef",
     "GetCertificateRequestRequestTypeDef",
     "GetPolicyRequestRequestTypeDef",
-    "ImportCertificateAuthorityCertificateRequestRequestTypeDef",
     "ValidityTypeDef",
     "PaginatorConfigTypeDef",
     "ListCertificateAuthoritiesRequestRequestTypeDef",
     "ListPermissionsRequestRequestTypeDef",
     "PermissionTypeDef",
     "ListTagsRequestRequestTypeDef",
     "OcspConfigurationTypeDef",
     "QualifierTypeDef",
     "PutPolicyRequestRequestTypeDef",
     "RestoreCertificateAuthorityRequestRequestTypeDef",
     "RevokeCertificateRequestRequestTypeDef",
     "ASN1SubjectOutputTypeDef",
     "ASN1SubjectTypeDef",
+    "ImportCertificateAuthorityCertificateRequestRequestTypeDef",
     "CreateCertificateAuthorityAuditReportResponseTypeDef",
     "CreateCertificateAuthorityResponseTypeDef",
     "DescribeCertificateAuthorityAuditReportResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetCertificateAuthorityCertificateResponseTypeDef",
     "GetCertificateAuthorityCsrResponseTypeDef",
     "GetCertificateResponseTypeDef",
@@ -113,14 +115,15 @@
     "CsrExtensionsOutputTypeDef",
     "CsrExtensionsTypeDef",
     "ApiPassthroughTypeDef",
     "CertificateAuthorityConfigurationOutputTypeDef",
     "CertificateAuthorityConfigurationTypeDef",
     "IssueCertificateRequestRequestTypeDef",
     "CertificateAuthorityTypeDef",
+    "CertificateAuthorityConfigurationUnionTypeDef",
     "CreateCertificateAuthorityRequestRequestTypeDef",
     "DescribeCertificateAuthorityResponseTypeDef",
     "ListCertificateAuthoritiesResponseTypeDef",
 )
 
 CustomAttributeTypeDef = TypedDict(
     "CustomAttributeTypeDef",
@@ -135,14 +138,15 @@
     {
         "CustomObjectIdentifier": str,
         "AccessMethodType": AccessMethodTypeType,
     },
     total=False,
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 CreateCertificateAuthorityAuditReportRequestRequestTypeDef = TypedDict(
     "CreateCertificateAuthorityAuditReportRequestRequestTypeDef",
     {
         "CertificateAuthorityArn": str,
         "S3BucketName": str,
         "AuditReportResponseFormat": AuditReportResponseFormatType,
     },
@@ -169,17 +173,19 @@
     "_OptionalTagTypeDef",
     {
         "Value": str,
     },
     total=False,
 )
 
+
 class TagTypeDef(_RequiredTagTypeDef, _OptionalTagTypeDef):
     pass
 
+
 _RequiredCreatePermissionRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePermissionRequestRequestTypeDef",
     {
         "CertificateAuthorityArn": str,
         "Principal": str,
         "Actions": Sequence[ActionTypeType],
     },
@@ -188,19 +194,21 @@
     "_OptionalCreatePermissionRequestRequestTypeDef",
     {
         "SourceAccount": str,
     },
     total=False,
 )
 
+
 class CreatePermissionRequestRequestTypeDef(
     _RequiredCreatePermissionRequestRequestTypeDef, _OptionalCreatePermissionRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredCrlConfigurationTypeDef = TypedDict(
     "_RequiredCrlConfigurationTypeDef",
     {
         "Enabled": bool,
     },
 )
 _OptionalCrlConfigurationTypeDef = TypedDict(
@@ -210,17 +218,19 @@
         "CustomCname": str,
         "S3BucketName": str,
         "S3ObjectAcl": S3ObjectAclType,
     },
     total=False,
 )
 
+
 class CrlConfigurationTypeDef(_RequiredCrlConfigurationTypeDef, _OptionalCrlConfigurationTypeDef):
     pass
 
+
 KeyUsageTypeDef = TypedDict(
     "KeyUsageTypeDef",
     {
         "DigitalSignature": bool,
         "NonRepudiation": bool,
         "KeyEncipherment": bool,
         "DataEncipherment": bool,
@@ -244,37 +254,41 @@
     "_OptionalCustomExtensionTypeDef",
     {
         "Critical": bool,
     },
     total=False,
 )
 
+
 class CustomExtensionTypeDef(_RequiredCustomExtensionTypeDef, _OptionalCustomExtensionTypeDef):
     pass
 
+
 _RequiredDeleteCertificateAuthorityRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteCertificateAuthorityRequestRequestTypeDef",
     {
         "CertificateAuthorityArn": str,
     },
 )
 _OptionalDeleteCertificateAuthorityRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteCertificateAuthorityRequestRequestTypeDef",
     {
         "PermanentDeletionTimeInDays": int,
     },
     total=False,
 )
 
+
 class DeleteCertificateAuthorityRequestRequestTypeDef(
     _RequiredDeleteCertificateAuthorityRequestRequestTypeDef,
     _OptionalDeleteCertificateAuthorityRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDeletePermissionRequestRequestTypeDef = TypedDict(
     "_RequiredDeletePermissionRequestRequestTypeDef",
     {
         "CertificateAuthorityArn": str,
         "Principal": str,
     },
 )
@@ -282,19 +296,21 @@
     "_OptionalDeletePermissionRequestRequestTypeDef",
     {
         "SourceAccount": str,
     },
     total=False,
 )
 
+
 class DeletePermissionRequestRequestTypeDef(
     _RequiredDeletePermissionRequestRequestTypeDef, _OptionalDeletePermissionRequestRequestTypeDef
 ):
     pass
 
+
 DeletePolicyRequestRequestTypeDef = TypedDict(
     "DeletePolicyRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
@@ -332,17 +348,19 @@
     "_OptionalEdiPartyNameTypeDef",
     {
         "NameAssigner": str,
     },
     total=False,
 )
 
+
 class EdiPartyNameTypeDef(_RequiredEdiPartyNameTypeDef, _OptionalEdiPartyNameTypeDef):
     pass
 
+
 ExtendedKeyUsageTypeDef = TypedDict(
     "ExtendedKeyUsageTypeDef",
     {
         "ExtendedKeyUsageType": ExtendedKeyUsageTypeType,
         "ExtendedKeyUsageObjectIdentifier": str,
     },
     total=False,
@@ -381,35 +399,14 @@
 GetPolicyRequestRequestTypeDef = TypedDict(
     "GetPolicyRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-_RequiredImportCertificateAuthorityCertificateRequestRequestTypeDef = TypedDict(
-    "_RequiredImportCertificateAuthorityCertificateRequestRequestTypeDef",
-    {
-        "CertificateAuthorityArn": str,
-        "Certificate": Union[str, bytes, IO[Any], StreamingBody],
-    },
-)
-_OptionalImportCertificateAuthorityCertificateRequestRequestTypeDef = TypedDict(
-    "_OptionalImportCertificateAuthorityCertificateRequestRequestTypeDef",
-    {
-        "CertificateChain": Union[str, bytes, IO[Any], StreamingBody],
-    },
-    total=False,
-)
-
-class ImportCertificateAuthorityCertificateRequestRequestTypeDef(
-    _RequiredImportCertificateAuthorityCertificateRequestRequestTypeDef,
-    _OptionalImportCertificateAuthorityCertificateRequestRequestTypeDef,
-):
-    pass
-
 ValidityTypeDef = TypedDict(
     "ValidityTypeDef",
     {
         "Value": int,
         "Type": ValidityPeriodTypeType,
     },
 )
@@ -445,19 +442,21 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListPermissionsRequestRequestTypeDef(
     _RequiredListPermissionsRequestRequestTypeDef, _OptionalListPermissionsRequestRequestTypeDef
 ):
     pass
 
+
 PermissionTypeDef = TypedDict(
     "PermissionTypeDef",
     {
         "CertificateAuthorityArn": str,
         "CreatedAt": datetime,
         "Principal": str,
         "SourceAccount": str,
@@ -478,38 +477,42 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListTagsRequestRequestTypeDef(
     _RequiredListTagsRequestRequestTypeDef, _OptionalListTagsRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredOcspConfigurationTypeDef = TypedDict(
     "_RequiredOcspConfigurationTypeDef",
     {
         "Enabled": bool,
     },
 )
 _OptionalOcspConfigurationTypeDef = TypedDict(
     "_OptionalOcspConfigurationTypeDef",
     {
         "OcspCustomCname": str,
     },
     total=False,
 )
 
+
 class OcspConfigurationTypeDef(
     _RequiredOcspConfigurationTypeDef, _OptionalOcspConfigurationTypeDef
 ):
     pass
 
+
 QualifierTypeDef = TypedDict(
     "QualifierTypeDef",
     {
         "CpsUri": str,
     },
 )
 
@@ -577,14 +580,37 @@
         "Pseudonym": str,
         "GenerationQualifier": str,
         "CustomAttributes": Sequence[CustomAttributeTypeDef],
     },
     total=False,
 )
 
+_RequiredImportCertificateAuthorityCertificateRequestRequestTypeDef = TypedDict(
+    "_RequiredImportCertificateAuthorityCertificateRequestRequestTypeDef",
+    {
+        "CertificateAuthorityArn": str,
+        "Certificate": BlobTypeDef,
+    },
+)
+_OptionalImportCertificateAuthorityCertificateRequestRequestTypeDef = TypedDict(
+    "_OptionalImportCertificateAuthorityCertificateRequestRequestTypeDef",
+    {
+        "CertificateChain": BlobTypeDef,
+    },
+    total=False,
+)
+
+
+class ImportCertificateAuthorityCertificateRequestRequestTypeDef(
+    _RequiredImportCertificateAuthorityCertificateRequestRequestTypeDef,
+    _OptionalImportCertificateAuthorityCertificateRequestRequestTypeDef,
+):
+    pass
+
+
 CreateCertificateAuthorityAuditReportResponseTypeDef = TypedDict(
     "CreateCertificateAuthorityAuditReportResponseTypeDef",
     {
         "AuditReportId": str,
         "S3Key": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -694,40 +720,44 @@
     "_OptionalDescribeCertificateAuthorityAuditReportRequestAuditReportCreatedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeCertificateAuthorityAuditReportRequestAuditReportCreatedWaitTypeDef(
     _RequiredDescribeCertificateAuthorityAuditReportRequestAuditReportCreatedWaitTypeDef,
     _OptionalDescribeCertificateAuthorityAuditReportRequestAuditReportCreatedWaitTypeDef,
 ):
     pass
 
+
 _RequiredGetCertificateAuthorityCsrRequestCertificateAuthorityCSRCreatedWaitTypeDef = TypedDict(
     "_RequiredGetCertificateAuthorityCsrRequestCertificateAuthorityCSRCreatedWaitTypeDef",
     {
         "CertificateAuthorityArn": str,
     },
 )
 _OptionalGetCertificateAuthorityCsrRequestCertificateAuthorityCSRCreatedWaitTypeDef = TypedDict(
     "_OptionalGetCertificateAuthorityCsrRequestCertificateAuthorityCSRCreatedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetCertificateAuthorityCsrRequestCertificateAuthorityCSRCreatedWaitTypeDef(
     _RequiredGetCertificateAuthorityCsrRequestCertificateAuthorityCSRCreatedWaitTypeDef,
     _OptionalGetCertificateAuthorityCsrRequestCertificateAuthorityCSRCreatedWaitTypeDef,
 ):
     pass
 
+
 _RequiredGetCertificateRequestCertificateIssuedWaitTypeDef = TypedDict(
     "_RequiredGetCertificateRequestCertificateIssuedWaitTypeDef",
     {
         "CertificateAuthorityArn": str,
         "CertificateArn": str,
     },
 )
@@ -735,20 +765,22 @@
     "_OptionalGetCertificateRequestCertificateIssuedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetCertificateRequestCertificateIssuedWaitTypeDef(
     _RequiredGetCertificateRequestCertificateIssuedWaitTypeDef,
     _OptionalGetCertificateRequestCertificateIssuedWaitTypeDef,
 ):
     pass
 
+
 ListCertificateAuthoritiesRequestListCertificateAuthoritiesPaginateTypeDef = TypedDict(
     "ListCertificateAuthoritiesRequestListCertificateAuthoritiesPaginateTypeDef",
     {
         "ResourceOwner": ResourceOwnerType,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -764,39 +796,43 @@
     "_OptionalListPermissionsRequestListPermissionsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListPermissionsRequestListPermissionsPaginateTypeDef(
     _RequiredListPermissionsRequestListPermissionsPaginateTypeDef,
     _OptionalListPermissionsRequestListPermissionsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListTagsRequestListTagsPaginateTypeDef = TypedDict(
     "_RequiredListTagsRequestListTagsPaginateTypeDef",
     {
         "CertificateAuthorityArn": str,
     },
 )
 _OptionalListTagsRequestListTagsPaginateTypeDef = TypedDict(
     "_OptionalListTagsRequestListTagsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListTagsRequestListTagsPaginateTypeDef(
     _RequiredListTagsRequestListTagsPaginateTypeDef, _OptionalListTagsRequestListTagsPaginateTypeDef
 ):
     pass
 
+
 ListPermissionsResponseTypeDef = TypedDict(
     "ListPermissionsResponseTypeDef",
     {
         "Permissions": List[PermissionTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -860,39 +896,43 @@
     {
         "RevocationConfiguration": RevocationConfigurationTypeDef,
         "Status": CertificateAuthorityStatusType,
     },
     total=False,
 )
 
+
 class UpdateCertificateAuthorityRequestRequestTypeDef(
     _RequiredUpdateCertificateAuthorityRequestRequestTypeDef,
     _OptionalUpdateCertificateAuthorityRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredPolicyInformationTypeDef = TypedDict(
     "_RequiredPolicyInformationTypeDef",
     {
         "CertPolicyId": str,
     },
 )
 _OptionalPolicyInformationTypeDef = TypedDict(
     "_OptionalPolicyInformationTypeDef",
     {
         "PolicyQualifiers": Sequence[PolicyQualifierInfoTypeDef],
     },
     total=False,
 )
 
+
 class PolicyInformationTypeDef(
     _RequiredPolicyInformationTypeDef, _OptionalPolicyInformationTypeDef
 ):
     pass
 
+
 AccessDescriptionOutputTypeDef = TypedDict(
     "AccessDescriptionOutputTypeDef",
     {
         "AccessMethod": AccessMethodTypeDef,
         "AccessLocation": GeneralNameOutputTypeDef,
     },
 )
@@ -956,20 +996,22 @@
     "_OptionalCertificateAuthorityConfigurationOutputTypeDef",
     {
         "CsrExtensions": CsrExtensionsOutputTypeDef,
     },
     total=False,
 )
 
+
 class CertificateAuthorityConfigurationOutputTypeDef(
     _RequiredCertificateAuthorityConfigurationOutputTypeDef,
     _OptionalCertificateAuthorityConfigurationOutputTypeDef,
 ):
     pass
 
+
 _RequiredCertificateAuthorityConfigurationTypeDef = TypedDict(
     "_RequiredCertificateAuthorityConfigurationTypeDef",
     {
         "KeyAlgorithm": KeyAlgorithmType,
         "SigningAlgorithm": SigningAlgorithmType,
         "Subject": ASN1SubjectTypeDef,
     },
@@ -978,25 +1020,27 @@
     "_OptionalCertificateAuthorityConfigurationTypeDef",
     {
         "CsrExtensions": CsrExtensionsTypeDef,
     },
     total=False,
 )
 
+
 class CertificateAuthorityConfigurationTypeDef(
     _RequiredCertificateAuthorityConfigurationTypeDef,
     _OptionalCertificateAuthorityConfigurationTypeDef,
 ):
     pass
 
+
 _RequiredIssueCertificateRequestRequestTypeDef = TypedDict(
     "_RequiredIssueCertificateRequestRequestTypeDef",
     {
         "CertificateAuthorityArn": str,
-        "Csr": Union[str, bytes, IO[Any], StreamingBody],
+        "Csr": BlobTypeDef,
         "SigningAlgorithm": SigningAlgorithmType,
         "Validity": ValidityTypeDef,
     },
 )
 _OptionalIssueCertificateRequestRequestTypeDef = TypedDict(
     "_OptionalIssueCertificateRequestRequestTypeDef",
     {
@@ -1004,19 +1048,21 @@
         "TemplateArn": str,
         "ValidityNotBefore": ValidityTypeDef,
         "IdempotencyToken": str,
     },
     total=False,
 )
 
+
 class IssueCertificateRequestRequestTypeDef(
     _RequiredIssueCertificateRequestRequestTypeDef, _OptionalIssueCertificateRequestRequestTypeDef
 ):
     pass
 
+
 CertificateAuthorityTypeDef = TypedDict(
     "CertificateAuthorityTypeDef",
     {
         "Arn": str,
         "OwnerAccount": str,
         "CreatedAt": datetime,
         "LastStateChangeAt": datetime,
@@ -1031,14 +1077,17 @@
         "RestorableUntil": datetime,
         "KeyStorageSecurityStandard": KeyStorageSecurityStandardType,
         "UsageMode": CertificateAuthorityUsageModeType,
     },
     total=False,
 )
 
+CertificateAuthorityConfigurationUnionTypeDef = Union[
+    CertificateAuthorityConfigurationTypeDef, CertificateAuthorityConfigurationOutputTypeDef
+]
 _RequiredCreateCertificateAuthorityRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCertificateAuthorityRequestRequestTypeDef",
     {
         "CertificateAuthorityConfiguration": CertificateAuthorityConfigurationTypeDef,
         "CertificateAuthorityType": CertificateAuthorityTypeType,
     },
 )
@@ -1050,20 +1099,22 @@
         "KeyStorageSecurityStandard": KeyStorageSecurityStandardType,
         "Tags": Sequence[TagTypeDef],
         "UsageMode": CertificateAuthorityUsageModeType,
     },
     total=False,
 )
 
+
 class CreateCertificateAuthorityRequestRequestTypeDef(
     _RequiredCreateCertificateAuthorityRequestRequestTypeDef,
     _OptionalCreateCertificateAuthorityRequestRequestTypeDef,
 ):
     pass
 
+
 DescribeCertificateAuthorityResponseTypeDef = TypedDict(
     "DescribeCertificateAuthorityResponseTypeDef",
     {
         "CertificateAuthority": CertificateAuthorityTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-acm-pca-1.28.15.post1/mypy_boto3_acm_pca/waiter.py` & `mypy-boto3-acm-pca-1.28.16/mypy_boto3_acm_pca/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-pca-1.28.15.post1/mypy_boto3_acm_pca/waiter.pyi` & `mypy-boto3-acm-pca-1.28.16/mypy_boto3_acm_pca/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-pca-1.28.15.post1/mypy_boto3_acm_pca.egg-info/PKG-INFO` & `mypy-boto3-acm-pca-1.28.16/mypy_boto3_acm_pca.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-acm-pca
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.ACMPCA 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.ACMPCA 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm_pca/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 acm-pca type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 acm-pca type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-acm-pca.svg?color=blue)](https://pypi.org/project/mypy-boto3-acm-pca)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm_pca/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-acm-pca)](https://pepy.tech/project/mypy-boto3-acm-pca)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ACMPCA 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA)
+[boto3.ACMPCA 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA)
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
 [mypy-boto3-acm-pca docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm_pca/).
 
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
@@ -368,25 +368,26 @@
 )
 
 
 def check_value(value: AccessMethodTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_acm_pca.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_acm_pca.type_defs import (
     CustomAttributeTypeDef,
     AccessMethodTypeDef,
+    BlobTypeDef,
     CreateCertificateAuthorityAuditReportRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     TagTypeDef,
     CreatePermissionRequestRequestTypeDef,
     CrlConfigurationTypeDef,
     KeyUsageTypeDef,
     CustomExtensionTypeDef,
@@ -399,28 +400,28 @@
     EdiPartyNameTypeDef,
     ExtendedKeyUsageTypeDef,
     OtherNameTypeDef,
     GetCertificateAuthorityCertificateRequestRequestTypeDef,
     GetCertificateAuthorityCsrRequestRequestTypeDef,
     GetCertificateRequestRequestTypeDef,
     GetPolicyRequestRequestTypeDef,
-    ImportCertificateAuthorityCertificateRequestRequestTypeDef,
     ValidityTypeDef,
     PaginatorConfigTypeDef,
     ListCertificateAuthoritiesRequestRequestTypeDef,
     ListPermissionsRequestRequestTypeDef,
     PermissionTypeDef,
     ListTagsRequestRequestTypeDef,
     OcspConfigurationTypeDef,
     QualifierTypeDef,
     PutPolicyRequestRequestTypeDef,
     RestoreCertificateAuthorityRequestRequestTypeDef,
     RevokeCertificateRequestRequestTypeDef,
     ASN1SubjectOutputTypeDef,
     ASN1SubjectTypeDef,
+    ImportCertificateAuthorityCertificateRequestRequestTypeDef,
     CreateCertificateAuthorityAuditReportResponseTypeDef,
     CreateCertificateAuthorityResponseTypeDef,
     DescribeCertificateAuthorityAuditReportResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetCertificateAuthorityCertificateResponseTypeDef,
     GetCertificateAuthorityCsrResponseTypeDef,
     GetCertificateResponseTypeDef,
@@ -448,21 +449,22 @@
     CsrExtensionsOutputTypeDef,
     CsrExtensionsTypeDef,
     ApiPassthroughTypeDef,
     CertificateAuthorityConfigurationOutputTypeDef,
     CertificateAuthorityConfigurationTypeDef,
     IssueCertificateRequestRequestTypeDef,
     CertificateAuthorityTypeDef,
+    CertificateAuthorityConfigurationUnionTypeDef,
     CreateCertificateAuthorityRequestRequestTypeDef,
     DescribeCertificateAuthorityResponseTypeDef,
     ListCertificateAuthoritiesResponseTypeDef,
 )
 
 
-def get_structure() -> CustomAttributeTypeDef:
+def get_value() -> CustomAttributeTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-acm-pca-1.28.15.post1/mypy_boto3_acm_pca.egg-info/SOURCES.txt` & `mypy-boto3-acm-pca-1.28.16/mypy_boto3_acm_pca.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-pca-1.28.15.post1/setup.py` & `mypy-boto3-acm-pca-1.28.16/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-acm-pca",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_acm_pca"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ACMPCA 1.28.15 service generated with mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.ACMPCA 1.28.16 service generated with mypy-boto3-builder 7.17.1"
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
-    keywords="boto3 acm-pca type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 acm-pca type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_acm_pca": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm_pca/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

