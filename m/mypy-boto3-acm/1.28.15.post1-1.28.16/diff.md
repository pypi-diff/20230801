# Comparing `tmp/mypy-boto3-acm-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-acm-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-acm-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:24 2023, max compression
+gzip compressed data, was "mypy-boto3-acm-1.28.16.tar", last modified: Tue Aug  1 11:36:04 2023, max compression
```

## Comparing `mypy-boto3-acm-1.28.15.post1.tar` & `mypy-boto3-acm-1.28.16.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:24.000978 mypy-boto3-acm-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:37:29.000000 mypy-boto3-acm-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14778 2023-07-29 10:02:24.000978 mypy-boto3-acm-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13301 2023-07-29 09:37:29.000000 mypy-boto3-acm-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:23.980978 mypy-boto3-acm-1.28.15.post1/mypy_boto3_acm/
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-29 09:37:29.000000 mypy-boto3-acm-1.28.15.post1/mypy_boto3_acm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-29 09:37:29.000000 mypy-boto3-acm-1.28.15.post1/mypy_boto3_acm/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-29 09:37:29.000000 mypy-boto3-acm-1.28.15.post1/mypy_boto3_acm/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13747 2023-07-29 09:37:29.000000 mypy-boto3-acm-1.28.15.post1/mypy_boto3_acm/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    13723 2023-07-29 09:37:29.000000 mypy-boto3-acm-1.28.15.post1/mypy_boto3_acm/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11013 2023-07-29 09:37:29.000000 mypy-boto3-acm-1.28.15.post1/mypy_boto3_acm/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11011 2023-07-29 09:37:29.000000 mypy-boto3-acm-1.28.15.post1/mypy_boto3_acm/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-07-29 09:37:29.000000 mypy-boto3-acm-1.28.15.post1/mypy_boto3_acm/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-07-29 09:37:29.000000 mypy-boto3-acm-1.28.15.post1/mypy_boto3_acm/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:37:29.000000 mypy-boto3-acm-1.28.15.post1/mypy_boto3_acm/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    14779 2023-07-29 09:37:30.000000 mypy-boto3-acm-1.28.15.post1/mypy_boto3_acm/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    14764 2023-07-29 09:37:29.000000 mypy-boto3-acm-1.28.15.post1/mypy_boto3_acm/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:37:29.000000 mypy-boto3-acm-1.28.15.post1/mypy_boto3_acm/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-07-29 09:37:29.000000 mypy-boto3-acm-1.28.15.post1/mypy_boto3_acm/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-07-29 09:37:29.000000 mypy-boto3-acm-1.28.15.post1/mypy_boto3_acm/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:24.000978 mypy-boto3-acm-1.28.15.post1/mypy_boto3_acm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14778 2023-07-29 10:02:23.000000 mypy-boto3-acm-1.28.15.post1/mypy_boto3_acm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-29 10:02:23.000000 mypy-boto3-acm-1.28.15.post1/mypy_boto3_acm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:23.000000 mypy-boto3-acm-1.28.15.post1/mypy_boto3_acm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:23.000000 mypy-boto3-acm-1.28.15.post1/mypy_boto3_acm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:23.000000 mypy-boto3-acm-1.28.15.post1/mypy_boto3_acm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-29 10:02:23.000000 mypy-boto3-acm-1.28.15.post1/mypy_boto3_acm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:24.000978 mypy-boto3-acm-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-29 09:37:29.000000 mypy-boto3-acm-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:04.792961 mypy-boto3-acm-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:09:58.000000 mypy-boto3-acm-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14785 2023-08-01 11:36:04.784961 mypy-boto3-acm-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13317 2023-08-01 11:09:58.000000 mypy-boto3-acm-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:04.780961 mypy-boto3-acm-1.28.16/mypy_boto3_acm/
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-08-01 11:09:58.000000 mypy-boto3-acm-1.28.16/mypy_boto3_acm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-08-01 11:09:58.000000 mypy-boto3-acm-1.28.16/mypy_boto3_acm/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-08-01 11:09:58.000000 mypy-boto3-acm-1.28.16/mypy_boto3_acm/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13589 2023-08-01 11:09:58.000000 mypy-boto3-acm-1.28.16/mypy_boto3_acm/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13565 2023-08-01 11:09:58.000000 mypy-boto3-acm-1.28.16/mypy_boto3_acm/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11013 2023-08-01 11:09:58.000000 mypy-boto3-acm-1.28.16/mypy_boto3_acm/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11011 2023-08-01 11:09:58.000000 mypy-boto3-acm-1.28.16/mypy_boto3_acm/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-08-01 11:09:58.000000 mypy-boto3-acm-1.28.16/mypy_boto3_acm/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-08-01 11:09:58.000000 mypy-boto3-acm-1.28.16/mypy_boto3_acm/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:09:58.000000 mypy-boto3-acm-1.28.16/mypy_boto3_acm/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    14732 2023-08-01 11:09:59.000000 mypy-boto3-acm-1.28.16/mypy_boto3_acm/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14717 2023-08-01 11:09:59.000000 mypy-boto3-acm-1.28.16/mypy_boto3_acm/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:09:58.000000 mypy-boto3-acm-1.28.16/mypy_boto3_acm/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-08-01 11:09:58.000000 mypy-boto3-acm-1.28.16/mypy_boto3_acm/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-08-01 11:09:58.000000 mypy-boto3-acm-1.28.16/mypy_boto3_acm/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:04.784961 mypy-boto3-acm-1.28.16/mypy_boto3_acm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14785 2023-08-01 11:36:04.000000 mypy-boto3-acm-1.28.16/mypy_boto3_acm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-08-01 11:36:04.000000 mypy-boto3-acm-1.28.16/mypy_boto3_acm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:04.000000 mypy-boto3-acm-1.28.16/mypy_boto3_acm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:04.000000 mypy-boto3-acm-1.28.16/mypy_boto3_acm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:04.000000 mypy-boto3-acm-1.28.16/mypy_boto3_acm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-01 11:36:04.000000 mypy-boto3-acm-1.28.16/mypy_boto3_acm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:04.792961 mypy-boto3-acm-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-08-01 11:09:58.000000 mypy-boto3-acm-1.28.16/setup.py
```

### Comparing `mypy-boto3-acm-1.28.15.post1/LICENSE` & `mypy-boto3-acm-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-1.28.15.post1/PKG-INFO` & `mypy-boto3-acm-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-acm
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.ACM 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.ACM 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 acm type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 acm type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-acm.svg?color=blue)](https://pypi.org/project/mypy-boto3-acm)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-acm)](https://pepy.tech/project/mypy-boto3-acm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ACM 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM)
+[boto3.ACM 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM)
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
 [mypy-boto3-acm docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm/).
 
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
@@ -347,45 +347,46 @@
 )
 
 
 def check_value(value: CertificateStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_acm.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_acm.type_defs import (
     TagTypeDef,
+    BlobTypeDef,
     CertificateOptionsTypeDef,
     ExtendedKeyUsageTypeDef,
     KeyUsageTypeDef,
     CertificateSummaryTypeDef,
     DeleteCertificateRequestRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeCertificateRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     DomainValidationOptionTypeDef,
     ResourceRecordTypeDef,
     ExpiryEventsConfigurationTypeDef,
-    ExportCertificateRequestRequestTypeDef,
     FiltersTypeDef,
     GetCertificateRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     ListTagsForCertificateRequestRequestTypeDef,
     RenewCertificateRequestRequestTypeDef,
     ResendValidationEmailRequestRequestTypeDef,
     AddTagsToCertificateRequestRequestTypeDef,
-    ImportCertificateRequestRequestTypeDef,
     RemoveTagsFromCertificateRequestRequestTypeDef,
+    ExportCertificateRequestRequestTypeDef,
+    ImportCertificateRequestRequestTypeDef,
     UpdateCertificateOptionsRequestRequestTypeDef,
     DescribeCertificateRequestCertificateValidatedWaitTypeDef,
     EmptyResponseMetadataTypeDef,
     ExportCertificateResponseTypeDef,
     GetCertificateResponseTypeDef,
     ImportCertificateResponseTypeDef,
     ListCertificatesResponseTypeDef,
@@ -399,15 +400,15 @@
     ListCertificatesRequestListCertificatesPaginateTypeDef,
     RenewalSummaryTypeDef,
     CertificateDetailTypeDef,
     DescribeCertificateResponseTypeDef,
 )
 
 
-def get_structure() -> TagTypeDef:
+def get_value() -> TagTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-acm-1.28.15.post1/README.md` & `mypy-boto3-acm-1.28.16/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-acm.svg?color=blue)](https://pypi.org/project/mypy-boto3-acm)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-acm)](https://pepy.tech/project/mypy-boto3-acm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ACM 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM)
+[boto3.ACM 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM)
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
 [mypy-boto3-acm docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm/).
 
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
@@ -315,45 +315,46 @@
 )
 
 
 def check_value(value: CertificateStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_acm.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_acm.type_defs import (
     TagTypeDef,
+    BlobTypeDef,
     CertificateOptionsTypeDef,
     ExtendedKeyUsageTypeDef,
     KeyUsageTypeDef,
     CertificateSummaryTypeDef,
     DeleteCertificateRequestRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeCertificateRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     DomainValidationOptionTypeDef,
     ResourceRecordTypeDef,
     ExpiryEventsConfigurationTypeDef,
-    ExportCertificateRequestRequestTypeDef,
     FiltersTypeDef,
     GetCertificateRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     ListTagsForCertificateRequestRequestTypeDef,
     RenewCertificateRequestRequestTypeDef,
     ResendValidationEmailRequestRequestTypeDef,
     AddTagsToCertificateRequestRequestTypeDef,
-    ImportCertificateRequestRequestTypeDef,
     RemoveTagsFromCertificateRequestRequestTypeDef,
+    ExportCertificateRequestRequestTypeDef,
+    ImportCertificateRequestRequestTypeDef,
     UpdateCertificateOptionsRequestRequestTypeDef,
     DescribeCertificateRequestCertificateValidatedWaitTypeDef,
     EmptyResponseMetadataTypeDef,
     ExportCertificateResponseTypeDef,
     GetCertificateResponseTypeDef,
     ImportCertificateResponseTypeDef,
     ListCertificatesResponseTypeDef,
@@ -367,15 +368,15 @@
     ListCertificatesRequestListCertificatesPaginateTypeDef,
     RenewalSummaryTypeDef,
     CertificateDetailTypeDef,
     DescribeCertificateResponseTypeDef,
 )
 
 
-def get_structure() -> TagTypeDef:
+def get_value() -> TagTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-acm-1.28.15.post1/mypy_boto3_acm/__init__.py` & `mypy-boto3-acm-1.28.16/mypy_boto3_acm/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-1.28.15.post1/mypy_boto3_acm/__init__.pyi` & `mypy-boto3-acm-1.28.16/mypy_boto3_acm/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-1.28.15.post1/mypy_boto3_acm/client.py` & `mypy-boto3-acm-1.28.16/mypy_boto3_acm/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,22 +10,22 @@
     from mypy_boto3_acm.client import ACMClient
 
     session = Session()
     client: ACMClient = session.client("acm")
     ```
 """
 import sys
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
-from botocore.response import StreamingBody
 
 from .literals import CertificateStatusType, KeyAlgorithmType, SortOrderType, ValidationMethodType
 from .paginator import ListCertificatesPaginator
 from .type_defs import (
+    BlobTypeDef,
     CertificateOptionsTypeDef,
     DescribeCertificateResponseTypeDef,
     DomainValidationOptionTypeDef,
     EmptyResponseMetadataTypeDef,
     ExpiryEventsConfigurationTypeDef,
     ExportCertificateResponseTypeDef,
     FiltersTypeDef,
@@ -132,15 +132,15 @@
         Returns detailed metadata about the specified ACM certificate.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM.Client.describe_certificate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm/client/#describe_certificate)
         """
 
     def export_certificate(
-        self, *, CertificateArn: str, Passphrase: Union[str, bytes, IO[Any], StreamingBody]
+        self, *, CertificateArn: str, Passphrase: BlobTypeDef
     ) -> ExportCertificateResponseTypeDef:
         """
         Exports a private certificate issued by a private certificate authority (CA) for
         use anywhere.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM.Client.export_certificate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm/client/#export_certificate)
@@ -176,18 +176,18 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM.Client.get_certificate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm/client/#get_certificate)
         """
 
     def import_certificate(
         self,
         *,
-        Certificate: Union[str, bytes, IO[Any], StreamingBody],
-        PrivateKey: Union[str, bytes, IO[Any], StreamingBody],
+        Certificate: BlobTypeDef,
+        PrivateKey: BlobTypeDef,
         CertificateArn: str = ...,
-        CertificateChain: Union[str, bytes, IO[Any], StreamingBody] = ...,
+        CertificateChain: BlobTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> ImportCertificateResponseTypeDef:
         """
         Imports a certificate into Certificate Manager (ACM) to use with services that
         are integrated with ACM.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM.Client.import_certificate)
```

### Comparing `mypy-boto3-acm-1.28.15.post1/mypy_boto3_acm/client.pyi` & `mypy-boto3-acm-1.28.16/mypy_boto3_acm/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -10,22 +10,22 @@
     from mypy_boto3_acm.client import ACMClient
 
     session = Session()
     client: ACMClient = session.client("acm")
     ```
 """
 import sys
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
-from botocore.response import StreamingBody
 
 from .literals import CertificateStatusType, KeyAlgorithmType, SortOrderType, ValidationMethodType
 from .paginator import ListCertificatesPaginator
 from .type_defs import (
+    BlobTypeDef,
     CertificateOptionsTypeDef,
     DescribeCertificateResponseTypeDef,
     DomainValidationOptionTypeDef,
     EmptyResponseMetadataTypeDef,
     ExpiryEventsConfigurationTypeDef,
     ExportCertificateResponseTypeDef,
     FiltersTypeDef,
@@ -122,15 +122,15 @@
         """
         Returns detailed metadata about the specified ACM certificate.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM.Client.describe_certificate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm/client/#describe_certificate)
         """
     def export_certificate(
-        self, *, CertificateArn: str, Passphrase: Union[str, bytes, IO[Any], StreamingBody]
+        self, *, CertificateArn: str, Passphrase: BlobTypeDef
     ) -> ExportCertificateResponseTypeDef:
         """
         Exports a private certificate issued by a private certificate authority (CA) for
         use anywhere.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM.Client.export_certificate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm/client/#export_certificate)
@@ -162,18 +162,18 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM.Client.get_certificate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm/client/#get_certificate)
         """
     def import_certificate(
         self,
         *,
-        Certificate: Union[str, bytes, IO[Any], StreamingBody],
-        PrivateKey: Union[str, bytes, IO[Any], StreamingBody],
+        Certificate: BlobTypeDef,
+        PrivateKey: BlobTypeDef,
         CertificateArn: str = ...,
-        CertificateChain: Union[str, bytes, IO[Any], StreamingBody] = ...,
+        CertificateChain: BlobTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> ImportCertificateResponseTypeDef:
         """
         Imports a certificate into Certificate Manager (ACM) to use with services that
         are integrated with ACM.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM.Client.import_certificate)
```

### Comparing `mypy-boto3-acm-1.28.15.post1/mypy_boto3_acm/literals.py` & `mypy-boto3-acm-1.28.16/mypy_boto3_acm/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-1.28.15.post1/mypy_boto3_acm/literals.pyi` & `mypy-boto3-acm-1.28.16/mypy_boto3_acm/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-1.28.15.post1/mypy_boto3_acm/paginator.py` & `mypy-boto3-acm-1.28.16/mypy_boto3_acm/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-1.28.15.post1/mypy_boto3_acm/paginator.pyi` & `mypy-boto3-acm-1.28.16/mypy_boto3_acm/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-1.28.15.post1/mypy_boto3_acm/type_defs.py` & `mypy-boto3-acm-1.28.16/mypy_boto3_acm/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_acm.type_defs import TagTypeDef
 
-    data: TagTypeDef = {...}
+    data: TagTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -41,35 +41,36 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "TagTypeDef",
+    "BlobTypeDef",
     "CertificateOptionsTypeDef",
     "ExtendedKeyUsageTypeDef",
     "KeyUsageTypeDef",
     "CertificateSummaryTypeDef",
     "DeleteCertificateRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeCertificateRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "DomainValidationOptionTypeDef",
     "ResourceRecordTypeDef",
     "ExpiryEventsConfigurationTypeDef",
-    "ExportCertificateRequestRequestTypeDef",
     "FiltersTypeDef",
     "GetCertificateRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "ListTagsForCertificateRequestRequestTypeDef",
     "RenewCertificateRequestRequestTypeDef",
     "ResendValidationEmailRequestRequestTypeDef",
     "AddTagsToCertificateRequestRequestTypeDef",
-    "ImportCertificateRequestRequestTypeDef",
     "RemoveTagsFromCertificateRequestRequestTypeDef",
+    "ExportCertificateRequestRequestTypeDef",
+    "ImportCertificateRequestRequestTypeDef",
     "UpdateCertificateOptionsRequestRequestTypeDef",
     "DescribeCertificateRequestCertificateValidatedWaitTypeDef",
     "EmptyResponseMetadataTypeDef",
     "ExportCertificateResponseTypeDef",
     "GetCertificateResponseTypeDef",
     "ImportCertificateResponseTypeDef",
     "ListCertificatesResponseTypeDef",
@@ -101,14 +102,15 @@
 )
 
 
 class TagTypeDef(_RequiredTagTypeDef, _OptionalTagTypeDef):
     pass
 
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 CertificateOptionsTypeDef = TypedDict(
     "CertificateOptionsTypeDef",
     {
         "CertificateTransparencyLoggingPreference": CertificateTransparencyLoggingPreferenceType,
     },
     total=False,
 )
@@ -210,22 +212,14 @@
     "ExpiryEventsConfigurationTypeDef",
     {
         "DaysBeforeExpiry": int,
     },
     total=False,
 )
 
-ExportCertificateRequestRequestTypeDef = TypedDict(
-    "ExportCertificateRequestRequestTypeDef",
-    {
-        "CertificateArn": str,
-        "Passphrase": Union[str, bytes, IO[Any], StreamingBody],
-    },
-)
-
 FiltersTypeDef = TypedDict(
     "FiltersTypeDef",
     {
         "extendedKeyUsage": Sequence[ExtendedKeyUsageNameType],
         "keyUsage": Sequence[KeyUsageNameType],
         "keyTypes": Sequence[KeyAlgorithmType],
     },
@@ -276,46 +270,54 @@
     "AddTagsToCertificateRequestRequestTypeDef",
     {
         "CertificateArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
+RemoveTagsFromCertificateRequestRequestTypeDef = TypedDict(
+    "RemoveTagsFromCertificateRequestRequestTypeDef",
+    {
+        "CertificateArn": str,
+        "Tags": Sequence[TagTypeDef],
+    },
+)
+
+ExportCertificateRequestRequestTypeDef = TypedDict(
+    "ExportCertificateRequestRequestTypeDef",
+    {
+        "CertificateArn": str,
+        "Passphrase": BlobTypeDef,
+    },
+)
+
 _RequiredImportCertificateRequestRequestTypeDef = TypedDict(
     "_RequiredImportCertificateRequestRequestTypeDef",
     {
-        "Certificate": Union[str, bytes, IO[Any], StreamingBody],
-        "PrivateKey": Union[str, bytes, IO[Any], StreamingBody],
+        "Certificate": BlobTypeDef,
+        "PrivateKey": BlobTypeDef,
     },
 )
 _OptionalImportCertificateRequestRequestTypeDef = TypedDict(
     "_OptionalImportCertificateRequestRequestTypeDef",
     {
         "CertificateArn": str,
-        "CertificateChain": Union[str, bytes, IO[Any], StreamingBody],
+        "CertificateChain": BlobTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
 
 class ImportCertificateRequestRequestTypeDef(
     _RequiredImportCertificateRequestRequestTypeDef, _OptionalImportCertificateRequestRequestTypeDef
 ):
     pass
 
 
-RemoveTagsFromCertificateRequestRequestTypeDef = TypedDict(
-    "RemoveTagsFromCertificateRequestRequestTypeDef",
-    {
-        "CertificateArn": str,
-        "Tags": Sequence[TagTypeDef],
-    },
-)
-
 UpdateCertificateOptionsRequestRequestTypeDef = TypedDict(
     "UpdateCertificateOptionsRequestRequestTypeDef",
     {
         "CertificateArn": str,
         "Options": CertificateOptionsTypeDef,
     },
 )
```

### Comparing `mypy-boto3-acm-1.28.15.post1/mypy_boto3_acm/type_defs.pyi` & `mypy-boto3-acm-1.28.16/mypy_boto3_acm/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_acm.type_defs import TagTypeDef
 
-    data: TagTypeDef = {...}
+    data: TagTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -40,35 +40,36 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "TagTypeDef",
+    "BlobTypeDef",
     "CertificateOptionsTypeDef",
     "ExtendedKeyUsageTypeDef",
     "KeyUsageTypeDef",
     "CertificateSummaryTypeDef",
     "DeleteCertificateRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeCertificateRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "DomainValidationOptionTypeDef",
     "ResourceRecordTypeDef",
     "ExpiryEventsConfigurationTypeDef",
-    "ExportCertificateRequestRequestTypeDef",
     "FiltersTypeDef",
     "GetCertificateRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "ListTagsForCertificateRequestRequestTypeDef",
     "RenewCertificateRequestRequestTypeDef",
     "ResendValidationEmailRequestRequestTypeDef",
     "AddTagsToCertificateRequestRequestTypeDef",
-    "ImportCertificateRequestRequestTypeDef",
     "RemoveTagsFromCertificateRequestRequestTypeDef",
+    "ExportCertificateRequestRequestTypeDef",
+    "ImportCertificateRequestRequestTypeDef",
     "UpdateCertificateOptionsRequestRequestTypeDef",
     "DescribeCertificateRequestCertificateValidatedWaitTypeDef",
     "EmptyResponseMetadataTypeDef",
     "ExportCertificateResponseTypeDef",
     "GetCertificateResponseTypeDef",
     "ImportCertificateResponseTypeDef",
     "ListCertificatesResponseTypeDef",
@@ -98,14 +99,15 @@
     },
     total=False,
 )
 
 class TagTypeDef(_RequiredTagTypeDef, _OptionalTagTypeDef):
     pass
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 CertificateOptionsTypeDef = TypedDict(
     "CertificateOptionsTypeDef",
     {
         "CertificateTransparencyLoggingPreference": CertificateTransparencyLoggingPreferenceType,
     },
     total=False,
 )
@@ -207,22 +209,14 @@
     "ExpiryEventsConfigurationTypeDef",
     {
         "DaysBeforeExpiry": int,
     },
     total=False,
 )
 
-ExportCertificateRequestRequestTypeDef = TypedDict(
-    "ExportCertificateRequestRequestTypeDef",
-    {
-        "CertificateArn": str,
-        "Passphrase": Union[str, bytes, IO[Any], StreamingBody],
-    },
-)
-
 FiltersTypeDef = TypedDict(
     "FiltersTypeDef",
     {
         "extendedKeyUsage": Sequence[ExtendedKeyUsageNameType],
         "keyUsage": Sequence[KeyUsageNameType],
         "keyTypes": Sequence[KeyAlgorithmType],
     },
@@ -273,44 +267,52 @@
     "AddTagsToCertificateRequestRequestTypeDef",
     {
         "CertificateArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
+RemoveTagsFromCertificateRequestRequestTypeDef = TypedDict(
+    "RemoveTagsFromCertificateRequestRequestTypeDef",
+    {
+        "CertificateArn": str,
+        "Tags": Sequence[TagTypeDef],
+    },
+)
+
+ExportCertificateRequestRequestTypeDef = TypedDict(
+    "ExportCertificateRequestRequestTypeDef",
+    {
+        "CertificateArn": str,
+        "Passphrase": BlobTypeDef,
+    },
+)
+
 _RequiredImportCertificateRequestRequestTypeDef = TypedDict(
     "_RequiredImportCertificateRequestRequestTypeDef",
     {
-        "Certificate": Union[str, bytes, IO[Any], StreamingBody],
-        "PrivateKey": Union[str, bytes, IO[Any], StreamingBody],
+        "Certificate": BlobTypeDef,
+        "PrivateKey": BlobTypeDef,
     },
 )
 _OptionalImportCertificateRequestRequestTypeDef = TypedDict(
     "_OptionalImportCertificateRequestRequestTypeDef",
     {
         "CertificateArn": str,
-        "CertificateChain": Union[str, bytes, IO[Any], StreamingBody],
+        "CertificateChain": BlobTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
 class ImportCertificateRequestRequestTypeDef(
     _RequiredImportCertificateRequestRequestTypeDef, _OptionalImportCertificateRequestRequestTypeDef
 ):
     pass
 
-RemoveTagsFromCertificateRequestRequestTypeDef = TypedDict(
-    "RemoveTagsFromCertificateRequestRequestTypeDef",
-    {
-        "CertificateArn": str,
-        "Tags": Sequence[TagTypeDef],
-    },
-)
-
 UpdateCertificateOptionsRequestRequestTypeDef = TypedDict(
     "UpdateCertificateOptionsRequestRequestTypeDef",
     {
         "CertificateArn": str,
         "Options": CertificateOptionsTypeDef,
     },
 )
```

### Comparing `mypy-boto3-acm-1.28.15.post1/mypy_boto3_acm/waiter.py` & `mypy-boto3-acm-1.28.16/mypy_boto3_acm/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-1.28.15.post1/mypy_boto3_acm/waiter.pyi` & `mypy-boto3-acm-1.28.16/mypy_boto3_acm/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-1.28.15.post1/mypy_boto3_acm.egg-info/PKG-INFO` & `mypy-boto3-acm-1.28.16/mypy_boto3_acm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-acm
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.ACM 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.ACM 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 acm type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 acm type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-acm.svg?color=blue)](https://pypi.org/project/mypy-boto3-acm)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-acm)](https://pepy.tech/project/mypy-boto3-acm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ACM 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM)
+[boto3.ACM 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM)
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
 [mypy-boto3-acm docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm/).
 
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
@@ -347,45 +347,46 @@
 )
 
 
 def check_value(value: CertificateStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_acm.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_acm.type_defs import (
     TagTypeDef,
+    BlobTypeDef,
     CertificateOptionsTypeDef,
     ExtendedKeyUsageTypeDef,
     KeyUsageTypeDef,
     CertificateSummaryTypeDef,
     DeleteCertificateRequestRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeCertificateRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     DomainValidationOptionTypeDef,
     ResourceRecordTypeDef,
     ExpiryEventsConfigurationTypeDef,
-    ExportCertificateRequestRequestTypeDef,
     FiltersTypeDef,
     GetCertificateRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     ListTagsForCertificateRequestRequestTypeDef,
     RenewCertificateRequestRequestTypeDef,
     ResendValidationEmailRequestRequestTypeDef,
     AddTagsToCertificateRequestRequestTypeDef,
-    ImportCertificateRequestRequestTypeDef,
     RemoveTagsFromCertificateRequestRequestTypeDef,
+    ExportCertificateRequestRequestTypeDef,
+    ImportCertificateRequestRequestTypeDef,
     UpdateCertificateOptionsRequestRequestTypeDef,
     DescribeCertificateRequestCertificateValidatedWaitTypeDef,
     EmptyResponseMetadataTypeDef,
     ExportCertificateResponseTypeDef,
     GetCertificateResponseTypeDef,
     ImportCertificateResponseTypeDef,
     ListCertificatesResponseTypeDef,
@@ -399,15 +400,15 @@
     ListCertificatesRequestListCertificatesPaginateTypeDef,
     RenewalSummaryTypeDef,
     CertificateDetailTypeDef,
     DescribeCertificateResponseTypeDef,
 )
 
 
-def get_structure() -> TagTypeDef:
+def get_value() -> TagTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-acm-1.28.15.post1/mypy_boto3_acm.egg-info/SOURCES.txt` & `mypy-boto3-acm-1.28.16/mypy_boto3_acm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-1.28.15.post1/setup.py` & `mypy-boto3-acm-1.28.16/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-acm",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_acm"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ACM 1.28.15 service generated with mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.ACM 1.28.16 service generated with mypy-boto3-builder 7.17.1"
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
-    keywords="boto3 acm type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 acm type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_acm": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

