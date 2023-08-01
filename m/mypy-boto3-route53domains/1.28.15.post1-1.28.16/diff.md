# Comparing `tmp/mypy-boto3-route53domains-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-route53domains-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-route53domains-1.28.15.post1.tar", last modified: Sat Jul 29 10:04:03 2023, max compression
+gzip compressed data, was "mypy-boto3-route53domains-1.28.16.tar", last modified: Tue Aug  1 11:37:43 2023, max compression
```

## Comparing `mypy-boto3-route53domains-1.28.15.post1.tar` & `mypy-boto3-route53domains-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:03.149372 mypy-boto3-route53domains-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:57:24.000000 mypy-boto3-route53domains-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17313 2023-07-29 10:04:03.141372 mypy-boto3-route53domains-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15792 2023-07-29 09:57:24.000000 mypy-boto3-route53domains-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:03.129372 mypy-boto3-route53domains-1.28.15.post1/mypy_boto3_route53domains/
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-29 09:57:24.000000 mypy-boto3-route53domains-1.28.15.post1/mypy_boto3_route53domains/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-07-29 09:57:24.000000 mypy-boto3-route53domains-1.28.15.post1/mypy_boto3_route53domains/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-29 09:57:24.000000 mypy-boto3-route53domains-1.28.15.post1/mypy_boto3_route53domains/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29405 2023-07-29 09:57:24.000000 mypy-boto3-route53domains-1.28.15.post1/mypy_boto3_route53domains/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    29360 2023-07-29 09:57:24.000000 mypy-boto3-route53domains-1.28.15.post1/mypy_boto3_route53domains/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13307 2023-07-29 09:57:24.000000 mypy-boto3-route53domains-1.28.15.post1/mypy_boto3_route53domains/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13305 2023-07-29 09:57:24.000000 mypy-boto3-route53domains-1.28.15.post1/mypy_boto3_route53domains/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5776 2023-07-29 09:57:24.000000 mypy-boto3-route53domains-1.28.15.post1/mypy_boto3_route53domains/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5769 2023-07-29 09:57:24.000000 mypy-boto3-route53domains-1.28.15.post1/mypy_boto3_route53domains/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:57:24.000000 mypy-boto3-route53domains-1.28.15.post1/mypy_boto3_route53domains/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    28569 2023-07-29 09:57:25.000000 mypy-boto3-route53domains-1.28.15.post1/mypy_boto3_route53domains/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    28546 2023-07-29 09:57:25.000000 mypy-boto3-route53domains-1.28.15.post1/mypy_boto3_route53domains/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:57:24.000000 mypy-boto3-route53domains-1.28.15.post1/mypy_boto3_route53domains/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:03.141372 mypy-boto3-route53domains-1.28.15.post1/mypy_boto3_route53domains.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17313 2023-07-29 10:04:02.000000 mypy-boto3-route53domains-1.28.15.post1/mypy_boto3_route53domains.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-29 10:04:02.000000 mypy-boto3-route53domains-1.28.15.post1/mypy_boto3_route53domains.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:02.000000 mypy-boto3-route53domains-1.28.15.post1/mypy_boto3_route53domains.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:02.000000 mypy-boto3-route53domains-1.28.15.post1/mypy_boto3_route53domains.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:04:02.000000 mypy-boto3-route53domains-1.28.15.post1/mypy_boto3_route53domains.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-29 10:04:02.000000 mypy-boto3-route53domains-1.28.15.post1/mypy_boto3_route53domains.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:04:03.149372 mypy-boto3-route53domains-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-07-29 09:57:24.000000 mypy-boto3-route53domains-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:43.748760 mypy-boto3-route53domains-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:30:47.000000 mypy-boto3-route53domains-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17384 2023-08-01 11:37:43.748760 mypy-boto3-route53domains-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15872 2023-08-01 11:30:47.000000 mypy-boto3-route53domains-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:43.740760 mypy-boto3-route53domains-1.28.16/mypy_boto3_route53domains/
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-08-01 11:30:47.000000 mypy-boto3-route53domains-1.28.16/mypy_boto3_route53domains/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-08-01 11:30:47.000000 mypy-boto3-route53domains-1.28.16/mypy_boto3_route53domains/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-08-01 11:30:48.000000 mypy-boto3-route53domains-1.28.16/mypy_boto3_route53domains/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29003 2023-08-01 11:30:48.000000 mypy-boto3-route53domains-1.28.16/mypy_boto3_route53domains/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28958 2023-08-01 11:30:48.000000 mypy-boto3-route53domains-1.28.16/mypy_boto3_route53domains/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13307 2023-08-01 11:30:48.000000 mypy-boto3-route53domains-1.28.16/mypy_boto3_route53domains/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13305 2023-08-01 11:30:48.000000 mypy-boto3-route53domains-1.28.16/mypy_boto3_route53domains/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5749 2023-08-01 11:30:48.000000 mypy-boto3-route53domains-1.28.16/mypy_boto3_route53domains/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5742 2023-08-01 11:30:48.000000 mypy-boto3-route53domains-1.28.16/mypy_boto3_route53domains/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:30:48.000000 mypy-boto3-route53domains-1.28.16/mypy_boto3_route53domains/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    28774 2023-08-01 11:30:53.000000 mypy-boto3-route53domains-1.28.16/mypy_boto3_route53domains/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28752 2023-08-01 11:30:49.000000 mypy-boto3-route53domains-1.28.16/mypy_boto3_route53domains/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:30:47.000000 mypy-boto3-route53domains-1.28.16/mypy_boto3_route53domains/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:43.748760 mypy-boto3-route53domains-1.28.16/mypy_boto3_route53domains.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17384 2023-08-01 11:37:43.000000 mypy-boto3-route53domains-1.28.16/mypy_boto3_route53domains.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-08-01 11:37:43.000000 mypy-boto3-route53domains-1.28.16/mypy_boto3_route53domains.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:43.000000 mypy-boto3-route53domains-1.28.16/mypy_boto3_route53domains.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:43.000000 mypy-boto3-route53domains-1.28.16/mypy_boto3_route53domains.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:43.000000 mypy-boto3-route53domains-1.28.16/mypy_boto3_route53domains.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-01 11:37:43.000000 mypy-boto3-route53domains-1.28.16/mypy_boto3_route53domains.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:43.748760 mypy-boto3-route53domains-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-08-01 11:30:47.000000 mypy-boto3-route53domains-1.28.16/setup.py
```

### Comparing `mypy-boto3-route53domains-1.28.15.post1/LICENSE` & `mypy-boto3-route53domains-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53domains-1.28.15.post1/PKG-INFO` & `mypy-boto3-route53domains-1.28.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-route53domains
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.Route53Domains 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.Route53Domains 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 route53domains type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 route53domains type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-route53domains.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53domains)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-route53domains)](https://pepy.tech/project/mypy-boto3-route53domains)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Route53Domains 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains)
+[boto3.Route53Domains 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains)
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
 [mypy-boto3-route53domains docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/).
 
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
@@ -335,20 +335,20 @@
 )
 
 
 def check_value(value: ContactTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_route53domains.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_route53domains.type_defs import (
     AcceptDomainTransferFromAnotherAwsAccountRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     DnssecSigningAttributesTypeDef,
     BillingRecordTypeDef,
@@ -373,29 +373,28 @@
     GetContactReachabilityStatusRequestRequestTypeDef,
     GetDomainDetailRequestRequestTypeDef,
     NameserverOutputTypeDef,
     GetDomainSuggestionsRequestRequestTypeDef,
     GetOperationDetailRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     SortConditionTypeDef,
-    ListOperationsRequestRequestTypeDef,
+    TimestampTypeDef,
     OperationSummaryTypeDef,
     ListPricesRequestRequestTypeDef,
     ListTagsForDomainRequestRequestTypeDef,
     TagTypeDef,
     NameserverTypeDef,
     PushDomainRequestRequestTypeDef,
     RejectDomainTransferFromAnotherAwsAccountRequestRequestTypeDef,
     RenewDomainRequestRequestTypeDef,
     ResendContactReachabilityEmailRequestRequestTypeDef,
     ResendOperationAuthorizationRequestRequestTypeDef,
     RetrieveDomainAuthCodeRequestRequestTypeDef,
     TransferDomainToAnotherAwsAccountRequestRequestTypeDef,
     UpdateDomainContactPrivacyRequestRequestTypeDef,
-    ViewBillingRequestRequestTypeDef,
     AcceptDomainTransferFromAnotherAwsAccountResponseTypeDef,
     AssociateDelegationSignerToDomainResponseTypeDef,
     CancelDomainTransferToAnotherAwsAccountResponseTypeDef,
     CheckDomainAvailabilityResponseTypeDef,
     DeleteDomainResponseTypeDef,
     DisableDomainTransferLockResponseTypeDef,
     DisassociateDelegationSignerFromDomainResponseTypeDef,
@@ -417,32 +416,36 @@
     ViewBillingResponseTypeDef,
     CheckDomainTransferabilityResponseTypeDef,
     ContactDetailOutputTypeDef,
     ContactDetailTypeDef,
     DomainPriceTypeDef,
     GetDomainSuggestionsResponseTypeDef,
     ListDomainsResponseTypeDef,
-    ListOperationsRequestListOperationsPaginateTypeDef,
     ListPricesRequestListPricesPaginateTypeDef,
-    ViewBillingRequestViewBillingPaginateTypeDef,
     ListDomainsRequestListDomainsPaginateTypeDef,
     ListDomainsRequestRequestTypeDef,
+    ListOperationsRequestListOperationsPaginateTypeDef,
+    ListOperationsRequestRequestTypeDef,
+    ViewBillingRequestRequestTypeDef,
+    ViewBillingRequestViewBillingPaginateTypeDef,
     ListOperationsResponseTypeDef,
     ListTagsForDomainResponseTypeDef,
     UpdateTagsForDomainRequestRequestTypeDef,
-    UpdateDomainNameserversRequestRequestTypeDef,
+    NameserverUnionTypeDef,
     GetDomainDetailResponseTypeDef,
+    ContactDetailUnionTypeDef,
     RegisterDomainRequestRequestTypeDef,
-    TransferDomainRequestRequestTypeDef,
     UpdateDomainContactRequestRequestTypeDef,
     ListPricesResponseTypeDef,
+    TransferDomainRequestRequestTypeDef,
+    UpdateDomainNameserversRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AcceptDomainTransferFromAnotherAwsAccountRequestRequestTypeDef:
+def get_value() -> AcceptDomainTransferFromAnotherAwsAccountRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-route53domains-1.28.15.post1/README.md` & `mypy-boto3-route53domains-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-route53domains.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53domains)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-route53domains)](https://pepy.tech/project/mypy-boto3-route53domains)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Route53Domains 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains)
+[boto3.Route53Domains 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains)
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
 [mypy-boto3-route53domains docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/).
 
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
@@ -303,20 +303,20 @@
 )
 
 
 def check_value(value: ContactTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_route53domains.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_route53domains.type_defs import (
     AcceptDomainTransferFromAnotherAwsAccountRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     DnssecSigningAttributesTypeDef,
     BillingRecordTypeDef,
@@ -341,29 +341,28 @@
     GetContactReachabilityStatusRequestRequestTypeDef,
     GetDomainDetailRequestRequestTypeDef,
     NameserverOutputTypeDef,
     GetDomainSuggestionsRequestRequestTypeDef,
     GetOperationDetailRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     SortConditionTypeDef,
-    ListOperationsRequestRequestTypeDef,
+    TimestampTypeDef,
     OperationSummaryTypeDef,
     ListPricesRequestRequestTypeDef,
     ListTagsForDomainRequestRequestTypeDef,
     TagTypeDef,
     NameserverTypeDef,
     PushDomainRequestRequestTypeDef,
     RejectDomainTransferFromAnotherAwsAccountRequestRequestTypeDef,
     RenewDomainRequestRequestTypeDef,
     ResendContactReachabilityEmailRequestRequestTypeDef,
     ResendOperationAuthorizationRequestRequestTypeDef,
     RetrieveDomainAuthCodeRequestRequestTypeDef,
     TransferDomainToAnotherAwsAccountRequestRequestTypeDef,
     UpdateDomainContactPrivacyRequestRequestTypeDef,
-    ViewBillingRequestRequestTypeDef,
     AcceptDomainTransferFromAnotherAwsAccountResponseTypeDef,
     AssociateDelegationSignerToDomainResponseTypeDef,
     CancelDomainTransferToAnotherAwsAccountResponseTypeDef,
     CheckDomainAvailabilityResponseTypeDef,
     DeleteDomainResponseTypeDef,
     DisableDomainTransferLockResponseTypeDef,
     DisassociateDelegationSignerFromDomainResponseTypeDef,
@@ -385,32 +384,36 @@
     ViewBillingResponseTypeDef,
     CheckDomainTransferabilityResponseTypeDef,
     ContactDetailOutputTypeDef,
     ContactDetailTypeDef,
     DomainPriceTypeDef,
     GetDomainSuggestionsResponseTypeDef,
     ListDomainsResponseTypeDef,
-    ListOperationsRequestListOperationsPaginateTypeDef,
     ListPricesRequestListPricesPaginateTypeDef,
-    ViewBillingRequestViewBillingPaginateTypeDef,
     ListDomainsRequestListDomainsPaginateTypeDef,
     ListDomainsRequestRequestTypeDef,
+    ListOperationsRequestListOperationsPaginateTypeDef,
+    ListOperationsRequestRequestTypeDef,
+    ViewBillingRequestRequestTypeDef,
+    ViewBillingRequestViewBillingPaginateTypeDef,
     ListOperationsResponseTypeDef,
     ListTagsForDomainResponseTypeDef,
     UpdateTagsForDomainRequestRequestTypeDef,
-    UpdateDomainNameserversRequestRequestTypeDef,
+    NameserverUnionTypeDef,
     GetDomainDetailResponseTypeDef,
+    ContactDetailUnionTypeDef,
     RegisterDomainRequestRequestTypeDef,
-    TransferDomainRequestRequestTypeDef,
     UpdateDomainContactRequestRequestTypeDef,
     ListPricesResponseTypeDef,
+    TransferDomainRequestRequestTypeDef,
+    UpdateDomainNameserversRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AcceptDomainTransferFromAnotherAwsAccountRequestRequestTypeDef:
+def get_value() -> AcceptDomainTransferFromAnotherAwsAccountRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-route53domains-1.28.15.post1/mypy_boto3_route53domains/__init__.py` & `mypy-boto3-route53domains-1.28.16/mypy_boto3_route53domains/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53domains-1.28.15.post1/mypy_boto3_route53domains/__init__.pyi` & `mypy-boto3-route53domains-1.28.16/mypy_boto3_route53domains/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53domains-1.28.15.post1/mypy_boto3_route53domains/client.py` & `mypy-boto3-route53domains-1.28.16/mypy_boto3_route53domains/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from mypy_boto3_route53domains.client import Route53DomainsClient
 
     session = Session()
     client: Route53DomainsClient = session.client("route53domains")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import OperationStatusType, OperationTypeType, SortOrderType
 from .paginator import (
     ListDomainsPaginator,
     ListOperationsPaginator,
@@ -29,16 +28,15 @@
 from .type_defs import (
     AcceptDomainTransferFromAnotherAwsAccountResponseTypeDef,
     AssociateDelegationSignerToDomainResponseTypeDef,
     CancelDomainTransferToAnotherAwsAccountResponseTypeDef,
     CheckDomainAvailabilityResponseTypeDef,
     CheckDomainTransferabilityResponseTypeDef,
     ConsentTypeDef,
-    ContactDetailOutputTypeDef,
-    ContactDetailTypeDef,
+    ContactDetailUnionTypeDef,
     DeleteDomainResponseTypeDef,
     DisableDomainTransferLockResponseTypeDef,
     DisassociateDelegationSignerFromDomainResponseTypeDef,
     DnssecSigningAttributesTypeDef,
     EmptyResponseMetadataTypeDef,
     EnableDomainTransferLockResponseTypeDef,
     FilterConditionTypeDef,
@@ -46,59 +44,55 @@
     GetDomainDetailResponseTypeDef,
     GetDomainSuggestionsResponseTypeDef,
     GetOperationDetailResponseTypeDef,
     ListDomainsResponseTypeDef,
     ListOperationsResponseTypeDef,
     ListPricesResponseTypeDef,
     ListTagsForDomainResponseTypeDef,
-    NameserverOutputTypeDef,
-    NameserverTypeDef,
+    NameserverUnionTypeDef,
     RegisterDomainResponseTypeDef,
     RejectDomainTransferFromAnotherAwsAccountResponseTypeDef,
     RenewDomainResponseTypeDef,
     ResendContactReachabilityEmailResponseTypeDef,
     RetrieveDomainAuthCodeResponseTypeDef,
     SortConditionTypeDef,
     TagTypeDef,
+    TimestampTypeDef,
     TransferDomainResponseTypeDef,
     TransferDomainToAnotherAwsAccountResponseTypeDef,
     UpdateDomainContactPrivacyResponseTypeDef,
     UpdateDomainContactResponseTypeDef,
     UpdateDomainNameserversResponseTypeDef,
     ViewBillingResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("Route53DomainsClient",)
 
-
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     ClientError: Type[BotocoreClientError]
     DnssecLimitExceeded: Type[BotocoreClientError]
     DomainLimitExceeded: Type[BotocoreClientError]
     DuplicateRequest: Type[BotocoreClientError]
     InvalidInput: Type[BotocoreClientError]
     OperationLimitExceeded: Type[BotocoreClientError]
     TLDRulesViolation: Type[BotocoreClientError]
     UnsupportedTLD: Type[BotocoreClientError]
 
-
 class Route53DomainsClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/client/)
     """
 
     meta: ClientMeta
@@ -107,206 +101,186 @@
     def exceptions(self) -> Exceptions:
         """
         Route53DomainsClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/client/#exceptions)
         """
-
     def accept_domain_transfer_from_another_aws_account(
         self, *, DomainName: str, Password: str
     ) -> AcceptDomainTransferFromAnotherAwsAccountResponseTypeDef:
         """
         Accepts the transfer of a domain from another Amazon Web Services account to the
         currentAmazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.accept_domain_transfer_from_another_aws_account)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/client/#accept_domain_transfer_from_another_aws_account)
         """
-
     def associate_delegation_signer_to_domain(
         self, *, DomainName: str, SigningAttributes: DnssecSigningAttributesTypeDef
     ) -> AssociateDelegationSignerToDomainResponseTypeDef:
         """
         Creates a delegation signer (DS) record in the registry zone for this domain
         name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.associate_delegation_signer_to_domain)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/client/#associate_delegation_signer_to_domain)
         """
-
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/client/#can_paginate)
         """
-
     def cancel_domain_transfer_to_another_aws_account(
         self, *, DomainName: str
     ) -> CancelDomainTransferToAnotherAwsAccountResponseTypeDef:
         """
         Cancels the transfer of a domain from the current Amazon Web Services account to
         another Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.cancel_domain_transfer_to_another_aws_account)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/client/#cancel_domain_transfer_to_another_aws_account)
         """
-
     def check_domain_availability(
         self, *, DomainName: str, IdnLangCode: str = ...
     ) -> CheckDomainAvailabilityResponseTypeDef:
         """
         This operation checks the availability of one domain name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.check_domain_availability)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/client/#check_domain_availability)
         """
-
     def check_domain_transferability(
         self, *, DomainName: str, AuthCode: str = ...
     ) -> CheckDomainTransferabilityResponseTypeDef:
         """
         Checks whether a domain name can be transferred to Amazon Route 53.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.check_domain_transferability)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/client/#check_domain_transferability)
         """
-
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/client/#close)
         """
-
     def delete_domain(self, *, DomainName: str) -> DeleteDomainResponseTypeDef:
         """
         This operation deletes the specified domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.delete_domain)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/client/#delete_domain)
         """
-
     def delete_tags_for_domain(
         self, *, DomainName: str, TagsToDelete: Sequence[str]
     ) -> Dict[str, Any]:
         """
         This operation deletes the specified tags for a domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.delete_tags_for_domain)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/client/#delete_tags_for_domain)
         """
-
     def disable_domain_auto_renew(self, *, DomainName: str) -> Dict[str, Any]:
         """
         This operation disables automatic renewal of domain registration for the
         specified domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.disable_domain_auto_renew)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/client/#disable_domain_auto_renew)
         """
-
     def disable_domain_transfer_lock(
         self, *, DomainName: str
     ) -> DisableDomainTransferLockResponseTypeDef:
         """
         This operation removes the transfer lock on the domain (specifically the
         `clientTransferProhibited` status) to allow domain transfers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.disable_domain_transfer_lock)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/client/#disable_domain_transfer_lock)
         """
-
     def disassociate_delegation_signer_from_domain(
         self, *, DomainName: str, Id: str
     ) -> DisassociateDelegationSignerFromDomainResponseTypeDef:
         """
         Deletes a delegation signer (DS) record in the registry zone for this domain
         name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.disassociate_delegation_signer_from_domain)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/client/#disassociate_delegation_signer_from_domain)
         """
-
     def enable_domain_auto_renew(self, *, DomainName: str) -> Dict[str, Any]:
         """
         This operation configures Amazon Route 53 to automatically renew the specified
         domain before the domain registration expires.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.enable_domain_auto_renew)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/client/#enable_domain_auto_renew)
         """
-
     def enable_domain_transfer_lock(
         self, *, DomainName: str
     ) -> EnableDomainTransferLockResponseTypeDef:
         """
         This operation sets the transfer lock on the domain (specifically the
         `clientTransferProhibited` status) to prevent domain transfers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.enable_domain_transfer_lock)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/client/#enable_domain_transfer_lock)
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
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/client/#generate_presigned_url)
         """
-
     def get_contact_reachability_status(
         self, *, domainName: str = ...
     ) -> GetContactReachabilityStatusResponseTypeDef:
         """
         For operations that require confirmation that the email address for the
         registrant contact is valid, such as registering a new domain, this operation
         returns information about whether the registrant contact has responded.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.get_contact_reachability_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/client/#get_contact_reachability_status)
         """
-
     def get_domain_detail(self, *, DomainName: str) -> GetDomainDetailResponseTypeDef:
         """
         This operation returns detailed information about a specified domain that is
         associated with the current Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.get_domain_detail)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/client/#get_domain_detail)
         """
-
     def get_domain_suggestions(
         self, *, DomainName: str, SuggestionCount: int, OnlyAvailable: bool
     ) -> GetDomainSuggestionsResponseTypeDef:
         """
         The GetDomainSuggestions operation returns a list of suggested domain names.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.get_domain_suggestions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/client/#get_domain_suggestions)
         """
-
     def get_operation_detail(self, *, OperationId: str) -> GetOperationDetailResponseTypeDef:
         """
         This operation returns the current status of an operation that is not completed.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.get_operation_detail)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/client/#get_operation_detail)
         """
-
     def list_domains(
         self,
         *,
         FilterConditions: Sequence[FilterConditionTypeDef] = ...,
         SortCondition: SortConditionTypeDef = ...,
         Marker: str = ...,
         MaxItems: int = ...
@@ -314,19 +288,18 @@
         """
         This operation returns all the domain names registered with Amazon Route 53 for
         the current Amazon Web Services account if no filtering conditions are used.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.list_domains)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/client/#list_domains)
         """
-
     def list_operations(
         self,
         *,
-        SubmittedSince: Union[datetime, str] = ...,
+        SubmittedSince: TimestampTypeDef = ...,
         Marker: str = ...,
         MaxItems: int = ...,
         Status: Sequence[OperationStatusType] = ...,
         Type: Sequence[OperationTypeType] = ...,
         SortBy: Literal["SubmittedDate"] = ...,
         SortOrder: SortOrderType = ...
     ) -> ListOperationsResponseTypeDef:
@@ -334,245 +307,225 @@
         Returns information about all of the operations that return an operation ID and
         that have ever been performed on domains that were registered by the current
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.list_operations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/client/#list_operations)
         """
-
     def list_prices(
         self, *, Tld: str = ..., Marker: str = ..., MaxItems: int = ...
     ) -> ListPricesResponseTypeDef:
         """
         Lists the following prices for either all the TLDs supported by Route 53, or the
         specified TLD: * Registration * Transfer * Owner change * Domain renewal *
         Domain restoration See also: `AWS API Documentation
         <https://docs.aws.amazon.com/goto/WebAPI/route53domains-2014-05-15/ListP...`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.list_prices)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/client/#list_prices)
         """
-
     def list_tags_for_domain(self, *, DomainName: str) -> ListTagsForDomainResponseTypeDef:
         """
         This operation returns all of the tags that are associated with the specified
         domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.list_tags_for_domain)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/client/#list_tags_for_domain)
         """
-
     def push_domain(self, *, DomainName: str, Target: str) -> EmptyResponseMetadataTypeDef:
         """
         Moves a domain from Amazon Web Services to another registrar.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.push_domain)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/client/#push_domain)
         """
-
     def register_domain(
         self,
         *,
         DomainName: str,
         DurationInYears: int,
-        AdminContact: Union[ContactDetailTypeDef, ContactDetailOutputTypeDef],
-        RegistrantContact: Union[ContactDetailTypeDef, ContactDetailOutputTypeDef],
-        TechContact: Union[ContactDetailTypeDef, ContactDetailOutputTypeDef],
+        AdminContact: ContactDetailUnionTypeDef,
+        RegistrantContact: ContactDetailUnionTypeDef,
+        TechContact: ContactDetailUnionTypeDef,
         IdnLangCode: str = ...,
         AutoRenew: bool = ...,
         PrivacyProtectAdminContact: bool = ...,
         PrivacyProtectRegistrantContact: bool = ...,
         PrivacyProtectTechContact: bool = ...
     ) -> RegisterDomainResponseTypeDef:
         """
         This operation registers a domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.register_domain)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/client/#register_domain)
         """
-
     def reject_domain_transfer_from_another_aws_account(
         self, *, DomainName: str
     ) -> RejectDomainTransferFromAnotherAwsAccountResponseTypeDef:
         """
         Rejects the transfer of a domain from another Amazon Web Services account to the
         current Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.reject_domain_transfer_from_another_aws_account)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/client/#reject_domain_transfer_from_another_aws_account)
         """
-
     def renew_domain(
         self, *, DomainName: str, CurrentExpiryYear: int, DurationInYears: int = ...
     ) -> RenewDomainResponseTypeDef:
         """
         This operation renews a domain for the specified number of years.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.renew_domain)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/client/#renew_domain)
         """
-
     def resend_contact_reachability_email(
         self, *, domainName: str = ...
     ) -> ResendContactReachabilityEmailResponseTypeDef:
         """
         For operations that require confirmation that the email address for the
         registrant contact is valid, such as registering a new domain, this operation
         resends the confirmation email to the current email address for the registrant
         contact.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.resend_contact_reachability_email)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/client/#resend_contact_reachability_email)
         """
-
     def resend_operation_authorization(self, *, OperationId: str) -> EmptyResponseMetadataTypeDef:
         """
         Resend the form of authorization email for this operation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.resend_operation_authorization)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/client/#resend_operation_authorization)
         """
-
     def retrieve_domain_auth_code(
         self, *, DomainName: str
     ) -> RetrieveDomainAuthCodeResponseTypeDef:
         """
         This operation returns the authorization code for the domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.retrieve_domain_auth_code)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/client/#retrieve_domain_auth_code)
         """
-
     def transfer_domain(
         self,
         *,
         DomainName: str,
         DurationInYears: int,
-        AdminContact: Union[ContactDetailTypeDef, ContactDetailOutputTypeDef],
-        RegistrantContact: Union[ContactDetailTypeDef, ContactDetailOutputTypeDef],
-        TechContact: Union[ContactDetailTypeDef, ContactDetailOutputTypeDef],
+        AdminContact: ContactDetailUnionTypeDef,
+        RegistrantContact: ContactDetailUnionTypeDef,
+        TechContact: ContactDetailUnionTypeDef,
         IdnLangCode: str = ...,
-        Nameservers: Sequence[Union[NameserverTypeDef, NameserverOutputTypeDef]] = ...,
+        Nameservers: Sequence[NameserverUnionTypeDef] = ...,
         AuthCode: str = ...,
         AutoRenew: bool = ...,
         PrivacyProtectAdminContact: bool = ...,
         PrivacyProtectRegistrantContact: bool = ...,
         PrivacyProtectTechContact: bool = ...
     ) -> TransferDomainResponseTypeDef:
         """
         Transfers a domain from another registrar to Amazon Route 53.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.transfer_domain)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/client/#transfer_domain)
         """
-
     def transfer_domain_to_another_aws_account(
         self, *, DomainName: str, AccountId: str
     ) -> TransferDomainToAnotherAwsAccountResponseTypeDef:
         """
         Transfers a domain from the current Amazon Web Services account to another
         Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.transfer_domain_to_another_aws_account)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/client/#transfer_domain_to_another_aws_account)
         """
-
     def update_domain_contact(
         self,
         *,
         DomainName: str,
-        AdminContact: Union[ContactDetailTypeDef, ContactDetailOutputTypeDef] = ...,
-        RegistrantContact: Union[ContactDetailTypeDef, ContactDetailOutputTypeDef] = ...,
-        TechContact: Union[ContactDetailTypeDef, ContactDetailOutputTypeDef] = ...,
+        AdminContact: ContactDetailUnionTypeDef = ...,
+        RegistrantContact: ContactDetailUnionTypeDef = ...,
+        TechContact: ContactDetailUnionTypeDef = ...,
         Consent: ConsentTypeDef = ...
     ) -> UpdateDomainContactResponseTypeDef:
         """
         This operation updates the contact information for a particular domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.update_domain_contact)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/client/#update_domain_contact)
         """
-
     def update_domain_contact_privacy(
         self,
         *,
         DomainName: str,
         AdminPrivacy: bool = ...,
         RegistrantPrivacy: bool = ...,
         TechPrivacy: bool = ...
     ) -> UpdateDomainContactPrivacyResponseTypeDef:
         """
         This operation updates the specified domain contact's privacy setting.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.update_domain_contact_privacy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/client/#update_domain_contact_privacy)
         """
-
     def update_domain_nameservers(
         self,
         *,
         DomainName: str,
-        Nameservers: Sequence[Union[NameserverTypeDef, NameserverOutputTypeDef]],
+        Nameservers: Sequence[NameserverUnionTypeDef],
         FIAuthKey: str = ...
     ) -> UpdateDomainNameserversResponseTypeDef:
         """
         This operation replaces the current set of name servers for the domain with the
         specified set of name servers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.update_domain_nameservers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/client/#update_domain_nameservers)
         """
-
     def update_tags_for_domain(
         self, *, DomainName: str, TagsToUpdate: Sequence[TagTypeDef] = ...
     ) -> Dict[str, Any]:
         """
         This operation adds or updates tags for a specified domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.update_tags_for_domain)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/client/#update_tags_for_domain)
         """
-
     def view_billing(
         self,
         *,
-        Start: Union[datetime, str] = ...,
-        End: Union[datetime, str] = ...,
+        Start: TimestampTypeDef = ...,
+        End: TimestampTypeDef = ...,
         Marker: str = ...,
         MaxItems: int = ...
     ) -> ViewBillingResponseTypeDef:
         """
         Returns all the domain-related billing records for the current Amazon Web
         Services account for a specified period See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/route53domains-2014-05-15/ViewBilling).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.view_billing)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/client/#view_billing)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["list_domains"]) -> ListDomainsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["list_operations"]) -> ListOperationsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["list_prices"]) -> ListPricesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["view_billing"]) -> ViewBillingPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/client/#get_paginator)
         """
```

### Comparing `mypy-boto3-route53domains-1.28.15.post1/mypy_boto3_route53domains/client.pyi` & `mypy-boto3-route53domains-1.28.16/mypy_boto3_route53domains/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from mypy_boto3_route53domains.client import Route53DomainsClient
 
     session = Session()
     client: Route53DomainsClient = session.client("route53domains")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import OperationStatusType, OperationTypeType, SortOrderType
 from .paginator import (
     ListDomainsPaginator,
     ListOperationsPaginator,
@@ -29,16 +28,15 @@
 from .type_defs import (
     AcceptDomainTransferFromAnotherAwsAccountResponseTypeDef,
     AssociateDelegationSignerToDomainResponseTypeDef,
     CancelDomainTransferToAnotherAwsAccountResponseTypeDef,
     CheckDomainAvailabilityResponseTypeDef,
     CheckDomainTransferabilityResponseTypeDef,
     ConsentTypeDef,
-    ContactDetailOutputTypeDef,
-    ContactDetailTypeDef,
+    ContactDetailUnionTypeDef,
     DeleteDomainResponseTypeDef,
     DisableDomainTransferLockResponseTypeDef,
     DisassociateDelegationSignerFromDomainResponseTypeDef,
     DnssecSigningAttributesTypeDef,
     EmptyResponseMetadataTypeDef,
     EnableDomainTransferLockResponseTypeDef,
     FilterConditionTypeDef,
@@ -46,55 +44,59 @@
     GetDomainDetailResponseTypeDef,
     GetDomainSuggestionsResponseTypeDef,
     GetOperationDetailResponseTypeDef,
     ListDomainsResponseTypeDef,
     ListOperationsResponseTypeDef,
     ListPricesResponseTypeDef,
     ListTagsForDomainResponseTypeDef,
-    NameserverOutputTypeDef,
-    NameserverTypeDef,
+    NameserverUnionTypeDef,
     RegisterDomainResponseTypeDef,
     RejectDomainTransferFromAnotherAwsAccountResponseTypeDef,
     RenewDomainResponseTypeDef,
     ResendContactReachabilityEmailResponseTypeDef,
     RetrieveDomainAuthCodeResponseTypeDef,
     SortConditionTypeDef,
     TagTypeDef,
+    TimestampTypeDef,
     TransferDomainResponseTypeDef,
     TransferDomainToAnotherAwsAccountResponseTypeDef,
     UpdateDomainContactPrivacyResponseTypeDef,
     UpdateDomainContactResponseTypeDef,
     UpdateDomainNameserversResponseTypeDef,
     ViewBillingResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = ("Route53DomainsClient",)
 
+
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     ClientError: Type[BotocoreClientError]
     DnssecLimitExceeded: Type[BotocoreClientError]
     DomainLimitExceeded: Type[BotocoreClientError]
     DuplicateRequest: Type[BotocoreClientError]
     InvalidInput: Type[BotocoreClientError]
     OperationLimitExceeded: Type[BotocoreClientError]
     TLDRulesViolation: Type[BotocoreClientError]
     UnsupportedTLD: Type[BotocoreClientError]
 
+
 class Route53DomainsClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/client/)
     """
 
     meta: ClientMeta
@@ -103,186 +105,206 @@
     def exceptions(self) -> Exceptions:
         """
         Route53DomainsClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/client/#exceptions)
         """
+
     def accept_domain_transfer_from_another_aws_account(
         self, *, DomainName: str, Password: str
     ) -> AcceptDomainTransferFromAnotherAwsAccountResponseTypeDef:
         """
         Accepts the transfer of a domain from another Amazon Web Services account to the
         currentAmazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.accept_domain_transfer_from_another_aws_account)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/client/#accept_domain_transfer_from_another_aws_account)
         """
+
     def associate_delegation_signer_to_domain(
         self, *, DomainName: str, SigningAttributes: DnssecSigningAttributesTypeDef
     ) -> AssociateDelegationSignerToDomainResponseTypeDef:
         """
         Creates a delegation signer (DS) record in the registry zone for this domain
         name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.associate_delegation_signer_to_domain)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/client/#associate_delegation_signer_to_domain)
         """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/client/#can_paginate)
         """
+
     def cancel_domain_transfer_to_another_aws_account(
         self, *, DomainName: str
     ) -> CancelDomainTransferToAnotherAwsAccountResponseTypeDef:
         """
         Cancels the transfer of a domain from the current Amazon Web Services account to
         another Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.cancel_domain_transfer_to_another_aws_account)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/client/#cancel_domain_transfer_to_another_aws_account)
         """
+
     def check_domain_availability(
         self, *, DomainName: str, IdnLangCode: str = ...
     ) -> CheckDomainAvailabilityResponseTypeDef:
         """
         This operation checks the availability of one domain name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.check_domain_availability)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/client/#check_domain_availability)
         """
+
     def check_domain_transferability(
         self, *, DomainName: str, AuthCode: str = ...
     ) -> CheckDomainTransferabilityResponseTypeDef:
         """
         Checks whether a domain name can be transferred to Amazon Route 53.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.check_domain_transferability)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/client/#check_domain_transferability)
         """
+
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/client/#close)
         """
+
     def delete_domain(self, *, DomainName: str) -> DeleteDomainResponseTypeDef:
         """
         This operation deletes the specified domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.delete_domain)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/client/#delete_domain)
         """
+
     def delete_tags_for_domain(
         self, *, DomainName: str, TagsToDelete: Sequence[str]
     ) -> Dict[str, Any]:
         """
         This operation deletes the specified tags for a domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.delete_tags_for_domain)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/client/#delete_tags_for_domain)
         """
+
     def disable_domain_auto_renew(self, *, DomainName: str) -> Dict[str, Any]:
         """
         This operation disables automatic renewal of domain registration for the
         specified domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.disable_domain_auto_renew)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/client/#disable_domain_auto_renew)
         """
+
     def disable_domain_transfer_lock(
         self, *, DomainName: str
     ) -> DisableDomainTransferLockResponseTypeDef:
         """
         This operation removes the transfer lock on the domain (specifically the
         `clientTransferProhibited` status) to allow domain transfers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.disable_domain_transfer_lock)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/client/#disable_domain_transfer_lock)
         """
+
     def disassociate_delegation_signer_from_domain(
         self, *, DomainName: str, Id: str
     ) -> DisassociateDelegationSignerFromDomainResponseTypeDef:
         """
         Deletes a delegation signer (DS) record in the registry zone for this domain
         name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.disassociate_delegation_signer_from_domain)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/client/#disassociate_delegation_signer_from_domain)
         """
+
     def enable_domain_auto_renew(self, *, DomainName: str) -> Dict[str, Any]:
         """
         This operation configures Amazon Route 53 to automatically renew the specified
         domain before the domain registration expires.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.enable_domain_auto_renew)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/client/#enable_domain_auto_renew)
         """
+
     def enable_domain_transfer_lock(
         self, *, DomainName: str
     ) -> EnableDomainTransferLockResponseTypeDef:
         """
         This operation sets the transfer lock on the domain (specifically the
         `clientTransferProhibited` status) to prevent domain transfers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.enable_domain_transfer_lock)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/client/#enable_domain_transfer_lock)
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
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/client/#generate_presigned_url)
         """
+
     def get_contact_reachability_status(
         self, *, domainName: str = ...
     ) -> GetContactReachabilityStatusResponseTypeDef:
         """
         For operations that require confirmation that the email address for the
         registrant contact is valid, such as registering a new domain, this operation
         returns information about whether the registrant contact has responded.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.get_contact_reachability_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/client/#get_contact_reachability_status)
         """
+
     def get_domain_detail(self, *, DomainName: str) -> GetDomainDetailResponseTypeDef:
         """
         This operation returns detailed information about a specified domain that is
         associated with the current Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.get_domain_detail)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/client/#get_domain_detail)
         """
+
     def get_domain_suggestions(
         self, *, DomainName: str, SuggestionCount: int, OnlyAvailable: bool
     ) -> GetDomainSuggestionsResponseTypeDef:
         """
         The GetDomainSuggestions operation returns a list of suggested domain names.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.get_domain_suggestions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/client/#get_domain_suggestions)
         """
+
     def get_operation_detail(self, *, OperationId: str) -> GetOperationDetailResponseTypeDef:
         """
         This operation returns the current status of an operation that is not completed.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.get_operation_detail)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/client/#get_operation_detail)
         """
+
     def list_domains(
         self,
         *,
         FilterConditions: Sequence[FilterConditionTypeDef] = ...,
         SortCondition: SortConditionTypeDef = ...,
         Marker: str = ...,
         MaxItems: int = ...
@@ -290,18 +312,19 @@
         """
         This operation returns all the domain names registered with Amazon Route 53 for
         the current Amazon Web Services account if no filtering conditions are used.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.list_domains)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/client/#list_domains)
         """
+
     def list_operations(
         self,
         *,
-        SubmittedSince: Union[datetime, str] = ...,
+        SubmittedSince: TimestampTypeDef = ...,
         Marker: str = ...,
         MaxItems: int = ...,
         Status: Sequence[OperationStatusType] = ...,
         Type: Sequence[OperationTypeType] = ...,
         SortBy: Literal["SubmittedDate"] = ...,
         SortOrder: SortOrderType = ...
     ) -> ListOperationsResponseTypeDef:
@@ -309,225 +332,245 @@
         Returns information about all of the operations that return an operation ID and
         that have ever been performed on domains that were registered by the current
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.list_operations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/client/#list_operations)
         """
+
     def list_prices(
         self, *, Tld: str = ..., Marker: str = ..., MaxItems: int = ...
     ) -> ListPricesResponseTypeDef:
         """
         Lists the following prices for either all the TLDs supported by Route 53, or the
         specified TLD: * Registration * Transfer * Owner change * Domain renewal *
         Domain restoration See also: `AWS API Documentation
         <https://docs.aws.amazon.com/goto/WebAPI/route53domains-2014-05-15/ListP...`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.list_prices)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/client/#list_prices)
         """
+
     def list_tags_for_domain(self, *, DomainName: str) -> ListTagsForDomainResponseTypeDef:
         """
         This operation returns all of the tags that are associated with the specified
         domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.list_tags_for_domain)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/client/#list_tags_for_domain)
         """
+
     def push_domain(self, *, DomainName: str, Target: str) -> EmptyResponseMetadataTypeDef:
         """
         Moves a domain from Amazon Web Services to another registrar.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.push_domain)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/client/#push_domain)
         """
+
     def register_domain(
         self,
         *,
         DomainName: str,
         DurationInYears: int,
-        AdminContact: Union[ContactDetailTypeDef, ContactDetailOutputTypeDef],
-        RegistrantContact: Union[ContactDetailTypeDef, ContactDetailOutputTypeDef],
-        TechContact: Union[ContactDetailTypeDef, ContactDetailOutputTypeDef],
+        AdminContact: ContactDetailUnionTypeDef,
+        RegistrantContact: ContactDetailUnionTypeDef,
+        TechContact: ContactDetailUnionTypeDef,
         IdnLangCode: str = ...,
         AutoRenew: bool = ...,
         PrivacyProtectAdminContact: bool = ...,
         PrivacyProtectRegistrantContact: bool = ...,
         PrivacyProtectTechContact: bool = ...
     ) -> RegisterDomainResponseTypeDef:
         """
         This operation registers a domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.register_domain)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/client/#register_domain)
         """
+
     def reject_domain_transfer_from_another_aws_account(
         self, *, DomainName: str
     ) -> RejectDomainTransferFromAnotherAwsAccountResponseTypeDef:
         """
         Rejects the transfer of a domain from another Amazon Web Services account to the
         current Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.reject_domain_transfer_from_another_aws_account)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/client/#reject_domain_transfer_from_another_aws_account)
         """
+
     def renew_domain(
         self, *, DomainName: str, CurrentExpiryYear: int, DurationInYears: int = ...
     ) -> RenewDomainResponseTypeDef:
         """
         This operation renews a domain for the specified number of years.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.renew_domain)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/client/#renew_domain)
         """
+
     def resend_contact_reachability_email(
         self, *, domainName: str = ...
     ) -> ResendContactReachabilityEmailResponseTypeDef:
         """
         For operations that require confirmation that the email address for the
         registrant contact is valid, such as registering a new domain, this operation
         resends the confirmation email to the current email address for the registrant
         contact.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.resend_contact_reachability_email)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/client/#resend_contact_reachability_email)
         """
+
     def resend_operation_authorization(self, *, OperationId: str) -> EmptyResponseMetadataTypeDef:
         """
         Resend the form of authorization email for this operation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.resend_operation_authorization)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/client/#resend_operation_authorization)
         """
+
     def retrieve_domain_auth_code(
         self, *, DomainName: str
     ) -> RetrieveDomainAuthCodeResponseTypeDef:
         """
         This operation returns the authorization code for the domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.retrieve_domain_auth_code)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/client/#retrieve_domain_auth_code)
         """
+
     def transfer_domain(
         self,
         *,
         DomainName: str,
         DurationInYears: int,
-        AdminContact: Union[ContactDetailTypeDef, ContactDetailOutputTypeDef],
-        RegistrantContact: Union[ContactDetailTypeDef, ContactDetailOutputTypeDef],
-        TechContact: Union[ContactDetailTypeDef, ContactDetailOutputTypeDef],
+        AdminContact: ContactDetailUnionTypeDef,
+        RegistrantContact: ContactDetailUnionTypeDef,
+        TechContact: ContactDetailUnionTypeDef,
         IdnLangCode: str = ...,
-        Nameservers: Sequence[Union[NameserverTypeDef, NameserverOutputTypeDef]] = ...,
+        Nameservers: Sequence[NameserverUnionTypeDef] = ...,
         AuthCode: str = ...,
         AutoRenew: bool = ...,
         PrivacyProtectAdminContact: bool = ...,
         PrivacyProtectRegistrantContact: bool = ...,
         PrivacyProtectTechContact: bool = ...
     ) -> TransferDomainResponseTypeDef:
         """
         Transfers a domain from another registrar to Amazon Route 53.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.transfer_domain)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/client/#transfer_domain)
         """
+
     def transfer_domain_to_another_aws_account(
         self, *, DomainName: str, AccountId: str
     ) -> TransferDomainToAnotherAwsAccountResponseTypeDef:
         """
         Transfers a domain from the current Amazon Web Services account to another
         Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.transfer_domain_to_another_aws_account)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/client/#transfer_domain_to_another_aws_account)
         """
+
     def update_domain_contact(
         self,
         *,
         DomainName: str,
-        AdminContact: Union[ContactDetailTypeDef, ContactDetailOutputTypeDef] = ...,
-        RegistrantContact: Union[ContactDetailTypeDef, ContactDetailOutputTypeDef] = ...,
-        TechContact: Union[ContactDetailTypeDef, ContactDetailOutputTypeDef] = ...,
+        AdminContact: ContactDetailUnionTypeDef = ...,
+        RegistrantContact: ContactDetailUnionTypeDef = ...,
+        TechContact: ContactDetailUnionTypeDef = ...,
         Consent: ConsentTypeDef = ...
     ) -> UpdateDomainContactResponseTypeDef:
         """
         This operation updates the contact information for a particular domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.update_domain_contact)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/client/#update_domain_contact)
         """
+
     def update_domain_contact_privacy(
         self,
         *,
         DomainName: str,
         AdminPrivacy: bool = ...,
         RegistrantPrivacy: bool = ...,
         TechPrivacy: bool = ...
     ) -> UpdateDomainContactPrivacyResponseTypeDef:
         """
         This operation updates the specified domain contact's privacy setting.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.update_domain_contact_privacy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/client/#update_domain_contact_privacy)
         """
+
     def update_domain_nameservers(
         self,
         *,
         DomainName: str,
-        Nameservers: Sequence[Union[NameserverTypeDef, NameserverOutputTypeDef]],
+        Nameservers: Sequence[NameserverUnionTypeDef],
         FIAuthKey: str = ...
     ) -> UpdateDomainNameserversResponseTypeDef:
         """
         This operation replaces the current set of name servers for the domain with the
         specified set of name servers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.update_domain_nameservers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/client/#update_domain_nameservers)
         """
+
     def update_tags_for_domain(
         self, *, DomainName: str, TagsToUpdate: Sequence[TagTypeDef] = ...
     ) -> Dict[str, Any]:
         """
         This operation adds or updates tags for a specified domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.update_tags_for_domain)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/client/#update_tags_for_domain)
         """
+
     def view_billing(
         self,
         *,
-        Start: Union[datetime, str] = ...,
-        End: Union[datetime, str] = ...,
+        Start: TimestampTypeDef = ...,
+        End: TimestampTypeDef = ...,
         Marker: str = ...,
         MaxItems: int = ...
     ) -> ViewBillingResponseTypeDef:
         """
         Returns all the domain-related billing records for the current Amazon Web
         Services account for a specified period See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/route53domains-2014-05-15/ViewBilling).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.view_billing)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/client/#view_billing)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["list_domains"]) -> ListDomainsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["list_operations"]) -> ListOperationsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["list_prices"]) -> ListPricesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["view_billing"]) -> ViewBillingPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/client/#get_paginator)
         """
```

### Comparing `mypy-boto3-route53domains-1.28.15.post1/mypy_boto3_route53domains/literals.py` & `mypy-boto3-route53domains-1.28.16/mypy_boto3_route53domains/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53domains-1.28.15.post1/mypy_boto3_route53domains/literals.pyi` & `mypy-boto3-route53domains-1.28.16/mypy_boto3_route53domains/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53domains-1.28.15.post1/mypy_boto3_route53domains/paginator.py` & `mypy-boto3-route53domains-1.28.16/mypy_boto3_route53domains/paginator.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,27 +22,27 @@
     list_domains_paginator: ListDomainsPaginator = client.get_paginator("list_domains")
     list_operations_paginator: ListOperationsPaginator = client.get_paginator("list_operations")
     list_prices_paginator: ListPricesPaginator = client.get_paginator("list_prices")
     view_billing_paginator: ViewBillingPaginator = client.get_paginator("view_billing")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Generic, Iterator, Sequence, TypeVar, Union
+from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import OperationStatusType, OperationTypeType, SortOrderType
 from .type_defs import (
     FilterConditionTypeDef,
     ListDomainsResponseTypeDef,
     ListOperationsResponseTypeDef,
     ListPricesResponseTypeDef,
     PaginatorConfigTypeDef,
     SortConditionTypeDef,
+    TimestampTypeDef,
     ViewBillingResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -90,15 +90,15 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Paginator.ListOperations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/paginators/#listoperationspaginator)
     """
 
     def paginate(
         self,
         *,
-        SubmittedSince: Union[datetime, str] = ...,
+        SubmittedSince: TimestampTypeDef = ...,
         Status: Sequence[OperationStatusType] = ...,
         Type: Sequence[OperationTypeType] = ...,
         SortBy: Literal["SubmittedDate"] = ...,
         SortOrder: SortOrderType = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListOperationsResponseTypeDef]:
         """
@@ -127,15 +127,15 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Paginator.ViewBilling)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/paginators/#viewbillingpaginator)
     """
 
     def paginate(
         self,
         *,
-        Start: Union[datetime, str] = ...,
-        End: Union[datetime, str] = ...,
+        Start: TimestampTypeDef = ...,
+        End: TimestampTypeDef = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ViewBillingResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Paginator.ViewBilling.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/paginators/#viewbillingpaginator)
         """
```

### Comparing `mypy-boto3-route53domains-1.28.15.post1/mypy_boto3_route53domains/paginator.pyi` & `mypy-boto3-route53domains-1.28.16/mypy_boto3_route53domains/paginator.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -22,27 +22,27 @@
     list_domains_paginator: ListDomainsPaginator = client.get_paginator("list_domains")
     list_operations_paginator: ListOperationsPaginator = client.get_paginator("list_operations")
     list_prices_paginator: ListPricesPaginator = client.get_paginator("list_prices")
     view_billing_paginator: ViewBillingPaginator = client.get_paginator("view_billing")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Generic, Iterator, Sequence, TypeVar, Union
+from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import OperationStatusType, OperationTypeType, SortOrderType
 from .type_defs import (
     FilterConditionTypeDef,
     ListDomainsResponseTypeDef,
     ListOperationsResponseTypeDef,
     ListPricesResponseTypeDef,
     PaginatorConfigTypeDef,
     SortConditionTypeDef,
+    TimestampTypeDef,
     ViewBillingResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -85,15 +85,15 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Paginator.ListOperations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/paginators/#listoperationspaginator)
     """
 
     def paginate(
         self,
         *,
-        SubmittedSince: Union[datetime, str] = ...,
+        SubmittedSince: TimestampTypeDef = ...,
         Status: Sequence[OperationStatusType] = ...,
         Type: Sequence[OperationTypeType] = ...,
         SortBy: Literal["SubmittedDate"] = ...,
         SortOrder: SortOrderType = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListOperationsResponseTypeDef]:
         """
@@ -120,15 +120,15 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Paginator.ViewBilling)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/paginators/#viewbillingpaginator)
     """
 
     def paginate(
         self,
         *,
-        Start: Union[datetime, str] = ...,
-        End: Union[datetime, str] = ...,
+        Start: TimestampTypeDef = ...,
+        End: TimestampTypeDef = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ViewBillingResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Paginator.ViewBilling.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/paginators/#viewbillingpaginator)
         """
```

### Comparing `mypy-boto3-route53domains-1.28.15.post1/mypy_boto3_route53domains/type_defs.py` & `mypy-boto3-route53domains-1.28.16/mypy_boto3_route53domains/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_route53domains.type_defs import AcceptDomainTransferFromAnotherAwsAccountRequestRequestTypeDef
 
-    data: AcceptDomainTransferFromAnotherAwsAccountRequestRequestTypeDef = {...}
+    data: AcceptDomainTransferFromAnotherAwsAccountRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -66,29 +66,28 @@
     "GetContactReachabilityStatusRequestRequestTypeDef",
     "GetDomainDetailRequestRequestTypeDef",
     "NameserverOutputTypeDef",
     "GetDomainSuggestionsRequestRequestTypeDef",
     "GetOperationDetailRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "SortConditionTypeDef",
-    "ListOperationsRequestRequestTypeDef",
+    "TimestampTypeDef",
     "OperationSummaryTypeDef",
     "ListPricesRequestRequestTypeDef",
     "ListTagsForDomainRequestRequestTypeDef",
     "TagTypeDef",
     "NameserverTypeDef",
     "PushDomainRequestRequestTypeDef",
     "RejectDomainTransferFromAnotherAwsAccountRequestRequestTypeDef",
     "RenewDomainRequestRequestTypeDef",
     "ResendContactReachabilityEmailRequestRequestTypeDef",
     "ResendOperationAuthorizationRequestRequestTypeDef",
     "RetrieveDomainAuthCodeRequestRequestTypeDef",
     "TransferDomainToAnotherAwsAccountRequestRequestTypeDef",
     "UpdateDomainContactPrivacyRequestRequestTypeDef",
-    "ViewBillingRequestRequestTypeDef",
     "AcceptDomainTransferFromAnotherAwsAccountResponseTypeDef",
     "AssociateDelegationSignerToDomainResponseTypeDef",
     "CancelDomainTransferToAnotherAwsAccountResponseTypeDef",
     "CheckDomainAvailabilityResponseTypeDef",
     "DeleteDomainResponseTypeDef",
     "DisableDomainTransferLockResponseTypeDef",
     "DisassociateDelegationSignerFromDomainResponseTypeDef",
@@ -110,28 +109,32 @@
     "ViewBillingResponseTypeDef",
     "CheckDomainTransferabilityResponseTypeDef",
     "ContactDetailOutputTypeDef",
     "ContactDetailTypeDef",
     "DomainPriceTypeDef",
     "GetDomainSuggestionsResponseTypeDef",
     "ListDomainsResponseTypeDef",
-    "ListOperationsRequestListOperationsPaginateTypeDef",
     "ListPricesRequestListPricesPaginateTypeDef",
-    "ViewBillingRequestViewBillingPaginateTypeDef",
     "ListDomainsRequestListDomainsPaginateTypeDef",
     "ListDomainsRequestRequestTypeDef",
+    "ListOperationsRequestListOperationsPaginateTypeDef",
+    "ListOperationsRequestRequestTypeDef",
+    "ViewBillingRequestRequestTypeDef",
+    "ViewBillingRequestViewBillingPaginateTypeDef",
     "ListOperationsResponseTypeDef",
     "ListTagsForDomainResponseTypeDef",
     "UpdateTagsForDomainRequestRequestTypeDef",
-    "UpdateDomainNameserversRequestRequestTypeDef",
+    "NameserverUnionTypeDef",
     "GetDomainDetailResponseTypeDef",
+    "ContactDetailUnionTypeDef",
     "RegisterDomainRequestRequestTypeDef",
-    "TransferDomainRequestRequestTypeDef",
     "UpdateDomainContactRequestRequestTypeDef",
     "ListPricesResponseTypeDef",
+    "TransferDomainRequestRequestTypeDef",
+    "UpdateDomainNameserversRequestRequestTypeDef",
 )
 
 AcceptDomainTransferFromAnotherAwsAccountRequestRequestTypeDef = TypedDict(
     "AcceptDomainTransferFromAnotherAwsAccountRequestRequestTypeDef",
     {
         "DomainName": str,
         "Password": str,
@@ -412,28 +415,15 @@
     "SortConditionTypeDef",
     {
         "Name": ListDomainsAttributeNameType,
         "SortOrder": SortOrderType,
     },
 )
 
-ListOperationsRequestRequestTypeDef = TypedDict(
-    "ListOperationsRequestRequestTypeDef",
-    {
-        "SubmittedSince": Union[datetime, str],
-        "Marker": str,
-        "MaxItems": int,
-        "Status": Sequence[OperationStatusType],
-        "Type": Sequence[OperationTypeType],
-        "SortBy": Literal["SubmittedDate"],
-        "SortOrder": SortOrderType,
-    },
-    total=False,
-)
-
+TimestampTypeDef = Union[datetime, str]
 OperationSummaryTypeDef = TypedDict(
     "OperationSummaryTypeDef",
     {
         "OperationId": str,
         "Status": OperationStatusType,
         "Type": OperationTypeType,
         "SubmittedDate": datetime,
@@ -577,25 +567,14 @@
 class UpdateDomainContactPrivacyRequestRequestTypeDef(
     _RequiredUpdateDomainContactPrivacyRequestRequestTypeDef,
     _OptionalUpdateDomainContactPrivacyRequestRequestTypeDef,
 ):
     pass
 
 
-ViewBillingRequestRequestTypeDef = TypedDict(
-    "ViewBillingRequestRequestTypeDef",
-    {
-        "Start": Union[datetime, str],
-        "End": Union[datetime, str],
-        "Marker": str,
-        "MaxItems": int,
-    },
-    total=False,
-)
-
 AcceptDomainTransferFromAnotherAwsAccountResponseTypeDef = TypedDict(
     "AcceptDomainTransferFromAnotherAwsAccountResponseTypeDef",
     {
         "OperationId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -863,46 +842,23 @@
     {
         "Domains": List[DomainSummaryTypeDef],
         "NextPageMarker": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListOperationsRequestListOperationsPaginateTypeDef = TypedDict(
-    "ListOperationsRequestListOperationsPaginateTypeDef",
-    {
-        "SubmittedSince": Union[datetime, str],
-        "Status": Sequence[OperationStatusType],
-        "Type": Sequence[OperationTypeType],
-        "SortBy": Literal["SubmittedDate"],
-        "SortOrder": SortOrderType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 ListPricesRequestListPricesPaginateTypeDef = TypedDict(
     "ListPricesRequestListPricesPaginateTypeDef",
     {
         "Tld": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ViewBillingRequestViewBillingPaginateTypeDef = TypedDict(
-    "ViewBillingRequestViewBillingPaginateTypeDef",
-    {
-        "Start": Union[datetime, str],
-        "End": Union[datetime, str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 ListDomainsRequestListDomainsPaginateTypeDef = TypedDict(
     "ListDomainsRequestListDomainsPaginateTypeDef",
     {
         "FilterConditions": Sequence[FilterConditionTypeDef],
         "SortCondition": SortConditionTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
@@ -916,14 +872,62 @@
         "SortCondition": SortConditionTypeDef,
         "Marker": str,
         "MaxItems": int,
     },
     total=False,
 )
 
+ListOperationsRequestListOperationsPaginateTypeDef = TypedDict(
+    "ListOperationsRequestListOperationsPaginateTypeDef",
+    {
+        "SubmittedSince": TimestampTypeDef,
+        "Status": Sequence[OperationStatusType],
+        "Type": Sequence[OperationTypeType],
+        "SortBy": Literal["SubmittedDate"],
+        "SortOrder": SortOrderType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListOperationsRequestRequestTypeDef = TypedDict(
+    "ListOperationsRequestRequestTypeDef",
+    {
+        "SubmittedSince": TimestampTypeDef,
+        "Marker": str,
+        "MaxItems": int,
+        "Status": Sequence[OperationStatusType],
+        "Type": Sequence[OperationTypeType],
+        "SortBy": Literal["SubmittedDate"],
+        "SortOrder": SortOrderType,
+    },
+    total=False,
+)
+
+ViewBillingRequestRequestTypeDef = TypedDict(
+    "ViewBillingRequestRequestTypeDef",
+    {
+        "Start": TimestampTypeDef,
+        "End": TimestampTypeDef,
+        "Marker": str,
+        "MaxItems": int,
+    },
+    total=False,
+)
+
+ViewBillingRequestViewBillingPaginateTypeDef = TypedDict(
+    "ViewBillingRequestViewBillingPaginateTypeDef",
+    {
+        "Start": TimestampTypeDef,
+        "End": TimestampTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 ListOperationsResponseTypeDef = TypedDict(
     "ListOperationsResponseTypeDef",
     {
         "Operations": List[OperationSummaryTypeDef],
         "NextPageMarker": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -955,37 +959,15 @@
 class UpdateTagsForDomainRequestRequestTypeDef(
     _RequiredUpdateTagsForDomainRequestRequestTypeDef,
     _OptionalUpdateTagsForDomainRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredUpdateDomainNameserversRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateDomainNameserversRequestRequestTypeDef",
-    {
-        "DomainName": str,
-        "Nameservers": Sequence[Union[NameserverTypeDef, NameserverOutputTypeDef]],
-    },
-)
-_OptionalUpdateDomainNameserversRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateDomainNameserversRequestRequestTypeDef",
-    {
-        "FIAuthKey": str,
-    },
-    total=False,
-)
-
-
-class UpdateDomainNameserversRequestRequestTypeDef(
-    _RequiredUpdateDomainNameserversRequestRequestTypeDef,
-    _OptionalUpdateDomainNameserversRequestRequestTypeDef,
-):
-    pass
-
-
+NameserverUnionTypeDef = Union[NameserverTypeDef, NameserverOutputTypeDef]
 GetDomainDetailResponseTypeDef = TypedDict(
     "GetDomainDetailResponseTypeDef",
     {
         "DomainName": str,
         "Nameservers": List[NameserverOutputTypeDef],
         "AutoRenew": bool,
         "AdminContact": ContactDetailOutputTypeDef,
@@ -1007,14 +989,15 @@
         "DnsSec": str,
         "StatusList": List[str],
         "DnssecKeys": List[DnssecKeyTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ContactDetailUnionTypeDef = Union[ContactDetailTypeDef, ContactDetailOutputTypeDef]
 _RequiredRegisterDomainRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterDomainRequestRequestTypeDef",
     {
         "DomainName": str,
         "DurationInYears": int,
         "AdminContact": ContactDetailTypeDef,
         "RegistrantContact": ContactDetailTypeDef,
@@ -1036,29 +1019,63 @@
 
 class RegisterDomainRequestRequestTypeDef(
     _RequiredRegisterDomainRequestRequestTypeDef, _OptionalRegisterDomainRequestRequestTypeDef
 ):
     pass
 
 
+_RequiredUpdateDomainContactRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateDomainContactRequestRequestTypeDef",
+    {
+        "DomainName": str,
+    },
+)
+_OptionalUpdateDomainContactRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateDomainContactRequestRequestTypeDef",
+    {
+        "AdminContact": ContactDetailTypeDef,
+        "RegistrantContact": ContactDetailTypeDef,
+        "TechContact": ContactDetailTypeDef,
+        "Consent": ConsentTypeDef,
+    },
+    total=False,
+)
+
+
+class UpdateDomainContactRequestRequestTypeDef(
+    _RequiredUpdateDomainContactRequestRequestTypeDef,
+    _OptionalUpdateDomainContactRequestRequestTypeDef,
+):
+    pass
+
+
+ListPricesResponseTypeDef = TypedDict(
+    "ListPricesResponseTypeDef",
+    {
+        "Prices": List[DomainPriceTypeDef],
+        "NextPageMarker": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredTransferDomainRequestRequestTypeDef = TypedDict(
     "_RequiredTransferDomainRequestRequestTypeDef",
     {
         "DomainName": str,
         "DurationInYears": int,
         "AdminContact": ContactDetailTypeDef,
         "RegistrantContact": ContactDetailTypeDef,
         "TechContact": ContactDetailTypeDef,
     },
 )
 _OptionalTransferDomainRequestRequestTypeDef = TypedDict(
     "_OptionalTransferDomainRequestRequestTypeDef",
     {
         "IdnLangCode": str,
-        "Nameservers": Sequence[Union[NameserverTypeDef, NameserverOutputTypeDef]],
+        "Nameservers": Sequence[NameserverUnionTypeDef],
         "AuthCode": str,
         "AutoRenew": bool,
         "PrivacyProtectAdminContact": bool,
         "PrivacyProtectRegistrantContact": bool,
         "PrivacyProtectTechContact": bool,
     },
     total=False,
@@ -1067,40 +1084,28 @@
 
 class TransferDomainRequestRequestTypeDef(
     _RequiredTransferDomainRequestRequestTypeDef, _OptionalTransferDomainRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredUpdateDomainContactRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateDomainContactRequestRequestTypeDef",
+_RequiredUpdateDomainNameserversRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateDomainNameserversRequestRequestTypeDef",
     {
         "DomainName": str,
+        "Nameservers": Sequence[NameserverUnionTypeDef],
     },
 )
-_OptionalUpdateDomainContactRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateDomainContactRequestRequestTypeDef",
+_OptionalUpdateDomainNameserversRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateDomainNameserversRequestRequestTypeDef",
     {
-        "AdminContact": ContactDetailTypeDef,
-        "RegistrantContact": ContactDetailTypeDef,
-        "TechContact": ContactDetailTypeDef,
-        "Consent": ConsentTypeDef,
+        "FIAuthKey": str,
     },
     total=False,
 )
 
 
-class UpdateDomainContactRequestRequestTypeDef(
-    _RequiredUpdateDomainContactRequestRequestTypeDef,
-    _OptionalUpdateDomainContactRequestRequestTypeDef,
+class UpdateDomainNameserversRequestRequestTypeDef(
+    _RequiredUpdateDomainNameserversRequestRequestTypeDef,
+    _OptionalUpdateDomainNameserversRequestRequestTypeDef,
 ):
     pass
-
-
-ListPricesResponseTypeDef = TypedDict(
-    "ListPricesResponseTypeDef",
-    {
-        "Prices": List[DomainPriceTypeDef],
-        "NextPageMarker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
```

### Comparing `mypy-boto3-route53domains-1.28.15.post1/mypy_boto3_route53domains/type_defs.pyi` & `mypy-boto3-route53domains-1.28.16/mypy_boto3_route53domains/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_route53domains.type_defs import AcceptDomainTransferFromAnotherAwsAccountRequestRequestTypeDef
 
-    data: AcceptDomainTransferFromAnotherAwsAccountRequestRequestTypeDef = {...}
+    data: AcceptDomainTransferFromAnotherAwsAccountRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -65,29 +65,28 @@
     "GetContactReachabilityStatusRequestRequestTypeDef",
     "GetDomainDetailRequestRequestTypeDef",
     "NameserverOutputTypeDef",
     "GetDomainSuggestionsRequestRequestTypeDef",
     "GetOperationDetailRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "SortConditionTypeDef",
-    "ListOperationsRequestRequestTypeDef",
+    "TimestampTypeDef",
     "OperationSummaryTypeDef",
     "ListPricesRequestRequestTypeDef",
     "ListTagsForDomainRequestRequestTypeDef",
     "TagTypeDef",
     "NameserverTypeDef",
     "PushDomainRequestRequestTypeDef",
     "RejectDomainTransferFromAnotherAwsAccountRequestRequestTypeDef",
     "RenewDomainRequestRequestTypeDef",
     "ResendContactReachabilityEmailRequestRequestTypeDef",
     "ResendOperationAuthorizationRequestRequestTypeDef",
     "RetrieveDomainAuthCodeRequestRequestTypeDef",
     "TransferDomainToAnotherAwsAccountRequestRequestTypeDef",
     "UpdateDomainContactPrivacyRequestRequestTypeDef",
-    "ViewBillingRequestRequestTypeDef",
     "AcceptDomainTransferFromAnotherAwsAccountResponseTypeDef",
     "AssociateDelegationSignerToDomainResponseTypeDef",
     "CancelDomainTransferToAnotherAwsAccountResponseTypeDef",
     "CheckDomainAvailabilityResponseTypeDef",
     "DeleteDomainResponseTypeDef",
     "DisableDomainTransferLockResponseTypeDef",
     "DisassociateDelegationSignerFromDomainResponseTypeDef",
@@ -109,28 +108,32 @@
     "ViewBillingResponseTypeDef",
     "CheckDomainTransferabilityResponseTypeDef",
     "ContactDetailOutputTypeDef",
     "ContactDetailTypeDef",
     "DomainPriceTypeDef",
     "GetDomainSuggestionsResponseTypeDef",
     "ListDomainsResponseTypeDef",
-    "ListOperationsRequestListOperationsPaginateTypeDef",
     "ListPricesRequestListPricesPaginateTypeDef",
-    "ViewBillingRequestViewBillingPaginateTypeDef",
     "ListDomainsRequestListDomainsPaginateTypeDef",
     "ListDomainsRequestRequestTypeDef",
+    "ListOperationsRequestListOperationsPaginateTypeDef",
+    "ListOperationsRequestRequestTypeDef",
+    "ViewBillingRequestRequestTypeDef",
+    "ViewBillingRequestViewBillingPaginateTypeDef",
     "ListOperationsResponseTypeDef",
     "ListTagsForDomainResponseTypeDef",
     "UpdateTagsForDomainRequestRequestTypeDef",
-    "UpdateDomainNameserversRequestRequestTypeDef",
+    "NameserverUnionTypeDef",
     "GetDomainDetailResponseTypeDef",
+    "ContactDetailUnionTypeDef",
     "RegisterDomainRequestRequestTypeDef",
-    "TransferDomainRequestRequestTypeDef",
     "UpdateDomainContactRequestRequestTypeDef",
     "ListPricesResponseTypeDef",
+    "TransferDomainRequestRequestTypeDef",
+    "UpdateDomainNameserversRequestRequestTypeDef",
 )
 
 AcceptDomainTransferFromAnotherAwsAccountRequestRequestTypeDef = TypedDict(
     "AcceptDomainTransferFromAnotherAwsAccountRequestRequestTypeDef",
     {
         "DomainName": str,
         "Password": str,
@@ -405,28 +408,15 @@
     "SortConditionTypeDef",
     {
         "Name": ListDomainsAttributeNameType,
         "SortOrder": SortOrderType,
     },
 )
 
-ListOperationsRequestRequestTypeDef = TypedDict(
-    "ListOperationsRequestRequestTypeDef",
-    {
-        "SubmittedSince": Union[datetime, str],
-        "Marker": str,
-        "MaxItems": int,
-        "Status": Sequence[OperationStatusType],
-        "Type": Sequence[OperationTypeType],
-        "SortBy": Literal["SubmittedDate"],
-        "SortOrder": SortOrderType,
-    },
-    total=False,
-)
-
+TimestampTypeDef = Union[datetime, str]
 OperationSummaryTypeDef = TypedDict(
     "OperationSummaryTypeDef",
     {
         "OperationId": str,
         "Status": OperationStatusType,
         "Type": OperationTypeType,
         "SubmittedDate": datetime,
@@ -564,25 +554,14 @@
 
 class UpdateDomainContactPrivacyRequestRequestTypeDef(
     _RequiredUpdateDomainContactPrivacyRequestRequestTypeDef,
     _OptionalUpdateDomainContactPrivacyRequestRequestTypeDef,
 ):
     pass
 
-ViewBillingRequestRequestTypeDef = TypedDict(
-    "ViewBillingRequestRequestTypeDef",
-    {
-        "Start": Union[datetime, str],
-        "End": Union[datetime, str],
-        "Marker": str,
-        "MaxItems": int,
-    },
-    total=False,
-)
-
 AcceptDomainTransferFromAnotherAwsAccountResponseTypeDef = TypedDict(
     "AcceptDomainTransferFromAnotherAwsAccountResponseTypeDef",
     {
         "OperationId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -850,46 +829,23 @@
     {
         "Domains": List[DomainSummaryTypeDef],
         "NextPageMarker": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListOperationsRequestListOperationsPaginateTypeDef = TypedDict(
-    "ListOperationsRequestListOperationsPaginateTypeDef",
-    {
-        "SubmittedSince": Union[datetime, str],
-        "Status": Sequence[OperationStatusType],
-        "Type": Sequence[OperationTypeType],
-        "SortBy": Literal["SubmittedDate"],
-        "SortOrder": SortOrderType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 ListPricesRequestListPricesPaginateTypeDef = TypedDict(
     "ListPricesRequestListPricesPaginateTypeDef",
     {
         "Tld": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ViewBillingRequestViewBillingPaginateTypeDef = TypedDict(
-    "ViewBillingRequestViewBillingPaginateTypeDef",
-    {
-        "Start": Union[datetime, str],
-        "End": Union[datetime, str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 ListDomainsRequestListDomainsPaginateTypeDef = TypedDict(
     "ListDomainsRequestListDomainsPaginateTypeDef",
     {
         "FilterConditions": Sequence[FilterConditionTypeDef],
         "SortCondition": SortConditionTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
@@ -903,14 +859,62 @@
         "SortCondition": SortConditionTypeDef,
         "Marker": str,
         "MaxItems": int,
     },
     total=False,
 )
 
+ListOperationsRequestListOperationsPaginateTypeDef = TypedDict(
+    "ListOperationsRequestListOperationsPaginateTypeDef",
+    {
+        "SubmittedSince": TimestampTypeDef,
+        "Status": Sequence[OperationStatusType],
+        "Type": Sequence[OperationTypeType],
+        "SortBy": Literal["SubmittedDate"],
+        "SortOrder": SortOrderType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListOperationsRequestRequestTypeDef = TypedDict(
+    "ListOperationsRequestRequestTypeDef",
+    {
+        "SubmittedSince": TimestampTypeDef,
+        "Marker": str,
+        "MaxItems": int,
+        "Status": Sequence[OperationStatusType],
+        "Type": Sequence[OperationTypeType],
+        "SortBy": Literal["SubmittedDate"],
+        "SortOrder": SortOrderType,
+    },
+    total=False,
+)
+
+ViewBillingRequestRequestTypeDef = TypedDict(
+    "ViewBillingRequestRequestTypeDef",
+    {
+        "Start": TimestampTypeDef,
+        "End": TimestampTypeDef,
+        "Marker": str,
+        "MaxItems": int,
+    },
+    total=False,
+)
+
+ViewBillingRequestViewBillingPaginateTypeDef = TypedDict(
+    "ViewBillingRequestViewBillingPaginateTypeDef",
+    {
+        "Start": TimestampTypeDef,
+        "End": TimestampTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 ListOperationsResponseTypeDef = TypedDict(
     "ListOperationsResponseTypeDef",
     {
         "Operations": List[OperationSummaryTypeDef],
         "NextPageMarker": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -940,35 +944,15 @@
 
 class UpdateTagsForDomainRequestRequestTypeDef(
     _RequiredUpdateTagsForDomainRequestRequestTypeDef,
     _OptionalUpdateTagsForDomainRequestRequestTypeDef,
 ):
     pass
 
-_RequiredUpdateDomainNameserversRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateDomainNameserversRequestRequestTypeDef",
-    {
-        "DomainName": str,
-        "Nameservers": Sequence[Union[NameserverTypeDef, NameserverOutputTypeDef]],
-    },
-)
-_OptionalUpdateDomainNameserversRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateDomainNameserversRequestRequestTypeDef",
-    {
-        "FIAuthKey": str,
-    },
-    total=False,
-)
-
-class UpdateDomainNameserversRequestRequestTypeDef(
-    _RequiredUpdateDomainNameserversRequestRequestTypeDef,
-    _OptionalUpdateDomainNameserversRequestRequestTypeDef,
-):
-    pass
-
+NameserverUnionTypeDef = Union[NameserverTypeDef, NameserverOutputTypeDef]
 GetDomainDetailResponseTypeDef = TypedDict(
     "GetDomainDetailResponseTypeDef",
     {
         "DomainName": str,
         "Nameservers": List[NameserverOutputTypeDef],
         "AutoRenew": bool,
         "AdminContact": ContactDetailOutputTypeDef,
@@ -990,14 +974,15 @@
         "DnsSec": str,
         "StatusList": List[str],
         "DnssecKeys": List[DnssecKeyTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ContactDetailUnionTypeDef = Union[ContactDetailTypeDef, ContactDetailOutputTypeDef]
 _RequiredRegisterDomainRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterDomainRequestRequestTypeDef",
     {
         "DomainName": str,
         "DurationInYears": int,
         "AdminContact": ContactDetailTypeDef,
         "RegistrantContact": ContactDetailTypeDef,
@@ -1017,67 +1002,88 @@
 )
 
 class RegisterDomainRequestRequestTypeDef(
     _RequiredRegisterDomainRequestRequestTypeDef, _OptionalRegisterDomainRequestRequestTypeDef
 ):
     pass
 
+_RequiredUpdateDomainContactRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateDomainContactRequestRequestTypeDef",
+    {
+        "DomainName": str,
+    },
+)
+_OptionalUpdateDomainContactRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateDomainContactRequestRequestTypeDef",
+    {
+        "AdminContact": ContactDetailTypeDef,
+        "RegistrantContact": ContactDetailTypeDef,
+        "TechContact": ContactDetailTypeDef,
+        "Consent": ConsentTypeDef,
+    },
+    total=False,
+)
+
+class UpdateDomainContactRequestRequestTypeDef(
+    _RequiredUpdateDomainContactRequestRequestTypeDef,
+    _OptionalUpdateDomainContactRequestRequestTypeDef,
+):
+    pass
+
+ListPricesResponseTypeDef = TypedDict(
+    "ListPricesResponseTypeDef",
+    {
+        "Prices": List[DomainPriceTypeDef],
+        "NextPageMarker": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredTransferDomainRequestRequestTypeDef = TypedDict(
     "_RequiredTransferDomainRequestRequestTypeDef",
     {
         "DomainName": str,
         "DurationInYears": int,
         "AdminContact": ContactDetailTypeDef,
         "RegistrantContact": ContactDetailTypeDef,
         "TechContact": ContactDetailTypeDef,
     },
 )
 _OptionalTransferDomainRequestRequestTypeDef = TypedDict(
     "_OptionalTransferDomainRequestRequestTypeDef",
     {
         "IdnLangCode": str,
-        "Nameservers": Sequence[Union[NameserverTypeDef, NameserverOutputTypeDef]],
+        "Nameservers": Sequence[NameserverUnionTypeDef],
         "AuthCode": str,
         "AutoRenew": bool,
         "PrivacyProtectAdminContact": bool,
         "PrivacyProtectRegistrantContact": bool,
         "PrivacyProtectTechContact": bool,
     },
     total=False,
 )
 
 class TransferDomainRequestRequestTypeDef(
     _RequiredTransferDomainRequestRequestTypeDef, _OptionalTransferDomainRequestRequestTypeDef
 ):
     pass
 
-_RequiredUpdateDomainContactRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateDomainContactRequestRequestTypeDef",
+_RequiredUpdateDomainNameserversRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateDomainNameserversRequestRequestTypeDef",
     {
         "DomainName": str,
+        "Nameservers": Sequence[NameserverUnionTypeDef],
     },
 )
-_OptionalUpdateDomainContactRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateDomainContactRequestRequestTypeDef",
+_OptionalUpdateDomainNameserversRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateDomainNameserversRequestRequestTypeDef",
     {
-        "AdminContact": ContactDetailTypeDef,
-        "RegistrantContact": ContactDetailTypeDef,
-        "TechContact": ContactDetailTypeDef,
-        "Consent": ConsentTypeDef,
+        "FIAuthKey": str,
     },
     total=False,
 )
 
-class UpdateDomainContactRequestRequestTypeDef(
-    _RequiredUpdateDomainContactRequestRequestTypeDef,
-    _OptionalUpdateDomainContactRequestRequestTypeDef,
+class UpdateDomainNameserversRequestRequestTypeDef(
+    _RequiredUpdateDomainNameserversRequestRequestTypeDef,
+    _OptionalUpdateDomainNameserversRequestRequestTypeDef,
 ):
     pass
-
-ListPricesResponseTypeDef = TypedDict(
-    "ListPricesResponseTypeDef",
-    {
-        "Prices": List[DomainPriceTypeDef],
-        "NextPageMarker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
```

### Comparing `mypy-boto3-route53domains-1.28.15.post1/mypy_boto3_route53domains.egg-info/PKG-INFO` & `mypy-boto3-route53domains-1.28.16/mypy_boto3_route53domains.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-route53domains
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.Route53Domains 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.Route53Domains 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 route53domains type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 route53domains type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-route53domains.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53domains)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-route53domains)](https://pepy.tech/project/mypy-boto3-route53domains)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Route53Domains 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains)
+[boto3.Route53Domains 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains)
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
 [mypy-boto3-route53domains docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/).
 
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
@@ -335,20 +335,20 @@
 )
 
 
 def check_value(value: ContactTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_route53domains.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_route53domains.type_defs import (
     AcceptDomainTransferFromAnotherAwsAccountRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     DnssecSigningAttributesTypeDef,
     BillingRecordTypeDef,
@@ -373,29 +373,28 @@
     GetContactReachabilityStatusRequestRequestTypeDef,
     GetDomainDetailRequestRequestTypeDef,
     NameserverOutputTypeDef,
     GetDomainSuggestionsRequestRequestTypeDef,
     GetOperationDetailRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     SortConditionTypeDef,
-    ListOperationsRequestRequestTypeDef,
+    TimestampTypeDef,
     OperationSummaryTypeDef,
     ListPricesRequestRequestTypeDef,
     ListTagsForDomainRequestRequestTypeDef,
     TagTypeDef,
     NameserverTypeDef,
     PushDomainRequestRequestTypeDef,
     RejectDomainTransferFromAnotherAwsAccountRequestRequestTypeDef,
     RenewDomainRequestRequestTypeDef,
     ResendContactReachabilityEmailRequestRequestTypeDef,
     ResendOperationAuthorizationRequestRequestTypeDef,
     RetrieveDomainAuthCodeRequestRequestTypeDef,
     TransferDomainToAnotherAwsAccountRequestRequestTypeDef,
     UpdateDomainContactPrivacyRequestRequestTypeDef,
-    ViewBillingRequestRequestTypeDef,
     AcceptDomainTransferFromAnotherAwsAccountResponseTypeDef,
     AssociateDelegationSignerToDomainResponseTypeDef,
     CancelDomainTransferToAnotherAwsAccountResponseTypeDef,
     CheckDomainAvailabilityResponseTypeDef,
     DeleteDomainResponseTypeDef,
     DisableDomainTransferLockResponseTypeDef,
     DisassociateDelegationSignerFromDomainResponseTypeDef,
@@ -417,32 +416,36 @@
     ViewBillingResponseTypeDef,
     CheckDomainTransferabilityResponseTypeDef,
     ContactDetailOutputTypeDef,
     ContactDetailTypeDef,
     DomainPriceTypeDef,
     GetDomainSuggestionsResponseTypeDef,
     ListDomainsResponseTypeDef,
-    ListOperationsRequestListOperationsPaginateTypeDef,
     ListPricesRequestListPricesPaginateTypeDef,
-    ViewBillingRequestViewBillingPaginateTypeDef,
     ListDomainsRequestListDomainsPaginateTypeDef,
     ListDomainsRequestRequestTypeDef,
+    ListOperationsRequestListOperationsPaginateTypeDef,
+    ListOperationsRequestRequestTypeDef,
+    ViewBillingRequestRequestTypeDef,
+    ViewBillingRequestViewBillingPaginateTypeDef,
     ListOperationsResponseTypeDef,
     ListTagsForDomainResponseTypeDef,
     UpdateTagsForDomainRequestRequestTypeDef,
-    UpdateDomainNameserversRequestRequestTypeDef,
+    NameserverUnionTypeDef,
     GetDomainDetailResponseTypeDef,
+    ContactDetailUnionTypeDef,
     RegisterDomainRequestRequestTypeDef,
-    TransferDomainRequestRequestTypeDef,
     UpdateDomainContactRequestRequestTypeDef,
     ListPricesResponseTypeDef,
+    TransferDomainRequestRequestTypeDef,
+    UpdateDomainNameserversRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AcceptDomainTransferFromAnotherAwsAccountRequestRequestTypeDef:
+def get_value() -> AcceptDomainTransferFromAnotherAwsAccountRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-route53domains-1.28.15.post1/mypy_boto3_route53domains.egg-info/SOURCES.txt` & `mypy-boto3-route53domains-1.28.16/mypy_boto3_route53domains.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53domains-1.28.15.post1/setup.py` & `mypy-boto3-route53domains-1.28.16/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-route53domains",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_route53domains"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Route53Domains 1.28.15 service generated with"
-        " mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.Route53Domains 1.28.16 service generated with"
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
-    keywords="boto3 route53domains type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 route53domains type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_route53domains": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

