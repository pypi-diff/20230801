# Comparing `tmp/mypy-boto3-ses-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-ses-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-ses-1.28.15.post1.tar", last modified: Sat Jul 29 10:04:12 2023, max compression
+gzip compressed data, was "mypy-boto3-ses-1.28.16.tar", last modified: Tue Aug  1 11:37:51 2023, max compression
```

## Comparing `mypy-boto3-ses-1.28.15.post1.tar` & `mypy-boto3-ses-1.28.16.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:12.373404 mypy-boto3-ses-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:59:30.000000 mypy-boto3-ses-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20529 2023-07-29 10:04:12.365404 mypy-boto3-ses-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19052 2023-07-29 09:59:30.000000 mypy-boto3-ses-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:12.365404 mypy-boto3-ses-1.28.15.post1/mypy_boto3_ses/
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-07-29 09:59:30.000000 mypy-boto3-ses-1.28.15.post1/mypy_boto3_ses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-07-29 09:59:30.000000 mypy-boto3-ses-1.28.15.post1/mypy_boto3_ses/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-29 09:59:30.000000 mypy-boto3-ses-1.28.15.post1/mypy_boto3_ses/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49503 2023-07-29 09:59:30.000000 mypy-boto3-ses-1.28.15.post1/mypy_boto3_ses/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    49419 2023-07-29 09:59:30.000000 mypy-boto3-ses-1.28.15.post1/mypy_boto3_ses/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10963 2023-07-29 09:59:31.000000 mypy-boto3-ses-1.28.15.post1/mypy_boto3_ses/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10961 2023-07-29 09:59:31.000000 mypy-boto3-ses-1.28.15.post1/mypy_boto3_ses/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6246 2023-07-29 09:59:30.000000 mypy-boto3-ses-1.28.15.post1/mypy_boto3_ses/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6239 2023-07-29 09:59:30.000000 mypy-boto3-ses-1.28.15.post1/mypy_boto3_ses/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:59:30.000000 mypy-boto3-ses-1.28.15.post1/mypy_boto3_ses/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    49427 2023-07-29 09:59:32.000000 mypy-boto3-ses-1.28.15.post1/mypy_boto3_ses/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    49360 2023-07-29 09:59:31.000000 mypy-boto3-ses-1.28.15.post1/mypy_boto3_ses/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:59:30.000000 mypy-boto3-ses-1.28.15.post1/mypy_boto3_ses/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-07-29 09:59:30.000000 mypy-boto3-ses-1.28.15.post1/mypy_boto3_ses/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-07-29 09:59:30.000000 mypy-boto3-ses-1.28.15.post1/mypy_boto3_ses/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:12.365404 mypy-boto3-ses-1.28.15.post1/mypy_boto3_ses.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20529 2023-07-29 10:04:12.000000 mypy-boto3-ses-1.28.15.post1/mypy_boto3_ses.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-29 10:04:12.000000 mypy-boto3-ses-1.28.15.post1/mypy_boto3_ses.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:12.000000 mypy-boto3-ses-1.28.15.post1/mypy_boto3_ses.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:12.000000 mypy-boto3-ses-1.28.15.post1/mypy_boto3_ses.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:04:12.000000 mypy-boto3-ses-1.28.15.post1/mypy_boto3_ses.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-29 10:04:12.000000 mypy-boto3-ses-1.28.15.post1/mypy_boto3_ses.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:04:12.373404 mypy-boto3-ses-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-29 09:59:30.000000 mypy-boto3-ses-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:51.864729 mypy-boto3-ses-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:33:02.000000 mypy-boto3-ses-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20621 2023-08-01 11:37:51.856728 mypy-boto3-ses-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19153 2023-08-01 11:33:02.000000 mypy-boto3-ses-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:51.852728 mypy-boto3-ses-1.28.16/mypy_boto3_ses/
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-08-01 11:33:02.000000 mypy-boto3-ses-1.28.16/mypy_boto3_ses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-08-01 11:33:02.000000 mypy-boto3-ses-1.28.16/mypy_boto3_ses/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-08-01 11:33:02.000000 mypy-boto3-ses-1.28.16/mypy_boto3_ses/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49239 2023-08-01 11:33:03.000000 mypy-boto3-ses-1.28.16/mypy_boto3_ses/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49155 2023-08-01 11:33:02.000000 mypy-boto3-ses-1.28.16/mypy_boto3_ses/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10963 2023-08-01 11:33:03.000000 mypy-boto3-ses-1.28.16/mypy_boto3_ses/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10961 2023-08-01 11:33:03.000000 mypy-boto3-ses-1.28.16/mypy_boto3_ses/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6246 2023-08-01 11:33:03.000000 mypy-boto3-ses-1.28.16/mypy_boto3_ses/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6239 2023-08-01 11:33:03.000000 mypy-boto3-ses-1.28.16/mypy_boto3_ses/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:33:02.000000 mypy-boto3-ses-1.28.16/mypy_boto3_ses/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    49764 2023-08-01 11:33:04.000000 mypy-boto3-ses-1.28.16/mypy_boto3_ses/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49697 2023-08-01 11:33:04.000000 mypy-boto3-ses-1.28.16/mypy_boto3_ses/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:33:02.000000 mypy-boto3-ses-1.28.16/mypy_boto3_ses/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-08-01 11:33:03.000000 mypy-boto3-ses-1.28.16/mypy_boto3_ses/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-08-01 11:33:03.000000 mypy-boto3-ses-1.28.16/mypy_boto3_ses/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:51.856728 mypy-boto3-ses-1.28.16/mypy_boto3_ses.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20621 2023-08-01 11:37:51.000000 mypy-boto3-ses-1.28.16/mypy_boto3_ses.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-08-01 11:37:51.000000 mypy-boto3-ses-1.28.16/mypy_boto3_ses.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:51.000000 mypy-boto3-ses-1.28.16/mypy_boto3_ses.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:51.000000 mypy-boto3-ses-1.28.16/mypy_boto3_ses.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:51.000000 mypy-boto3-ses-1.28.16/mypy_boto3_ses.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-01 11:37:51.000000 mypy-boto3-ses-1.28.16/mypy_boto3_ses.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:51.864729 mypy-boto3-ses-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-08-01 11:33:02.000000 mypy-boto3-ses-1.28.16/setup.py
```

### Comparing `mypy-boto3-ses-1.28.15.post1/LICENSE` & `mypy-boto3-ses-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ses-1.28.15.post1/PKG-INFO` & `mypy-boto3-ses-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ses
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.SES 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.SES 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 ses type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 ses type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ses.svg?color=blue)](https://pypi.org/project/mypy-boto3-ses)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ses)](https://pepy.tech/project/mypy-boto3-ses)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SES 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES)
+[boto3.SES 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES)
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
 [mypy-boto3-ses docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/).
 
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
@@ -366,24 +366,25 @@
 )
 
 
 def check_value(value: BehaviorOnMXFailureType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_ses.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_ses.type_defs import (
     AddHeaderActionTypeDef,
+    BlobTypeDef,
     ContentTypeDef,
     BounceActionTypeDef,
     BulkEmailDestinationStatusTypeDef,
     DestinationTypeDef,
     MessageTagTypeDef,
     CloneReceiptRuleSetRequestRequestTypeDef,
     CloudWatchDimensionConfigurationTypeDef,
@@ -432,16 +433,16 @@
     ListConfigurationSetsRequestRequestTypeDef,
     ListCustomVerificationEmailTemplatesRequestRequestTypeDef,
     ListIdentitiesRequestRequestTypeDef,
     ListIdentityPoliciesRequestRequestTypeDef,
     ListReceiptRuleSetsRequestRequestTypeDef,
     ListTemplatesRequestRequestTypeDef,
     TemplateMetadataTypeDef,
+    TimestampTypeDef,
     PutIdentityPolicyRequestRequestTypeDef,
-    RawMessageTypeDef,
     S3ActionTypeDef,
     SNSActionTypeDef,
     StopActionTypeDef,
     WorkmailActionTypeDef,
     ReceiptIpFilterTypeDef,
     ReorderReceiptRuleSetRequestRequestTypeDef,
     SendCustomVerificationEmailRequestRequestTypeDef,
@@ -457,14 +458,15 @@
     UpdateConfigurationSetReputationMetricsEnabledRequestRequestTypeDef,
     UpdateConfigurationSetSendingEnabledRequestRequestTypeDef,
     UpdateCustomVerificationEmailTemplateRequestRequestTypeDef,
     VerifyDomainDkimRequestRequestTypeDef,
     VerifyDomainIdentityRequestRequestTypeDef,
     VerifyEmailAddressRequestRequestTypeDef,
     VerifyEmailIdentityRequestRequestTypeDef,
+    RawMessageTypeDef,
     BodyTypeDef,
     BulkEmailDestinationTypeDef,
     SendTemplatedEmailRequestRequestTypeDef,
     CloudWatchDestinationOutputTypeDef,
     CloudWatchDestinationTypeDef,
     CreateConfigurationSetRequestRequestTypeDef,
     CreateConfigurationSetTrackingOptionsRequestRequestTypeDef,
@@ -489,54 +491,56 @@
     SendCustomVerificationEmailResponseTypeDef,
     SendEmailResponseTypeDef,
     SendRawEmailResponseTypeDef,
     SendTemplatedEmailResponseTypeDef,
     TestRenderTemplateResponseTypeDef,
     VerifyDomainDkimResponseTypeDef,
     VerifyDomainIdentityResponseTypeDef,
-    MessageDsnTypeDef,
-    RecipientDsnFieldsTypeDef,
     GetIdentityDkimAttributesResponseTypeDef,
     GetIdentityMailFromDomainAttributesResponseTypeDef,
     GetIdentityNotificationAttributesResponseTypeDef,
     GetIdentityVerificationAttributesRequestIdentityExistsWaitTypeDef,
     GetIdentityVerificationAttributesResponseTypeDef,
     GetSendStatisticsResponseTypeDef,
     ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef,
     ListCustomVerificationEmailTemplatesRequestListCustomVerificationEmailTemplatesPaginateTypeDef,
     ListIdentitiesRequestListIdentitiesPaginateTypeDef,
     ListReceiptRuleSetsRequestListReceiptRuleSetsPaginateTypeDef,
     ListTemplatesRequestListTemplatesPaginateTypeDef,
     ListTemplatesResponseTypeDef,
-    SendRawEmailRequestRequestTypeDef,
+    MessageDsnTypeDef,
+    RecipientDsnFieldsTypeDef,
     ReceiptActionTypeDef,
     ReceiptFilterTypeDef,
+    SendRawEmailRequestRequestTypeDef,
     MessageTypeDef,
     SendBulkTemplatedEmailRequestRequestTypeDef,
     EventDestinationOutputTypeDef,
     EventDestinationTypeDef,
     BouncedRecipientInfoTypeDef,
     ReceiptRuleOutputTypeDef,
     ReceiptRuleTypeDef,
     CreateReceiptFilterRequestRequestTypeDef,
     ListReceiptFiltersResponseTypeDef,
     SendEmailRequestRequestTypeDef,
     DescribeConfigurationSetResponseTypeDef,
     CreateConfigurationSetEventDestinationRequestRequestTypeDef,
+    EventDestinationUnionTypeDef,
     UpdateConfigurationSetEventDestinationRequestRequestTypeDef,
     SendBounceRequestRequestTypeDef,
     DescribeActiveReceiptRuleSetResponseTypeDef,
     DescribeReceiptRuleResponseTypeDef,
     DescribeReceiptRuleSetResponseTypeDef,
     CreateReceiptRuleRequestRequestTypeDef,
+    ReceiptRuleUnionTypeDef,
     UpdateReceiptRuleRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AddHeaderActionTypeDef:
+def get_value() -> AddHeaderActionTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-ses-1.28.15.post1/README.md` & `mypy-boto3-ses-1.28.16/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ses.svg?color=blue)](https://pypi.org/project/mypy-boto3-ses)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ses)](https://pepy.tech/project/mypy-boto3-ses)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SES 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES)
+[boto3.SES 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES)
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
 [mypy-boto3-ses docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/).
 
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
@@ -334,24 +334,25 @@
 )
 
 
 def check_value(value: BehaviorOnMXFailureType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_ses.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_ses.type_defs import (
     AddHeaderActionTypeDef,
+    BlobTypeDef,
     ContentTypeDef,
     BounceActionTypeDef,
     BulkEmailDestinationStatusTypeDef,
     DestinationTypeDef,
     MessageTagTypeDef,
     CloneReceiptRuleSetRequestRequestTypeDef,
     CloudWatchDimensionConfigurationTypeDef,
@@ -400,16 +401,16 @@
     ListConfigurationSetsRequestRequestTypeDef,
     ListCustomVerificationEmailTemplatesRequestRequestTypeDef,
     ListIdentitiesRequestRequestTypeDef,
     ListIdentityPoliciesRequestRequestTypeDef,
     ListReceiptRuleSetsRequestRequestTypeDef,
     ListTemplatesRequestRequestTypeDef,
     TemplateMetadataTypeDef,
+    TimestampTypeDef,
     PutIdentityPolicyRequestRequestTypeDef,
-    RawMessageTypeDef,
     S3ActionTypeDef,
     SNSActionTypeDef,
     StopActionTypeDef,
     WorkmailActionTypeDef,
     ReceiptIpFilterTypeDef,
     ReorderReceiptRuleSetRequestRequestTypeDef,
     SendCustomVerificationEmailRequestRequestTypeDef,
@@ -425,14 +426,15 @@
     UpdateConfigurationSetReputationMetricsEnabledRequestRequestTypeDef,
     UpdateConfigurationSetSendingEnabledRequestRequestTypeDef,
     UpdateCustomVerificationEmailTemplateRequestRequestTypeDef,
     VerifyDomainDkimRequestRequestTypeDef,
     VerifyDomainIdentityRequestRequestTypeDef,
     VerifyEmailAddressRequestRequestTypeDef,
     VerifyEmailIdentityRequestRequestTypeDef,
+    RawMessageTypeDef,
     BodyTypeDef,
     BulkEmailDestinationTypeDef,
     SendTemplatedEmailRequestRequestTypeDef,
     CloudWatchDestinationOutputTypeDef,
     CloudWatchDestinationTypeDef,
     CreateConfigurationSetRequestRequestTypeDef,
     CreateConfigurationSetTrackingOptionsRequestRequestTypeDef,
@@ -457,54 +459,56 @@
     SendCustomVerificationEmailResponseTypeDef,
     SendEmailResponseTypeDef,
     SendRawEmailResponseTypeDef,
     SendTemplatedEmailResponseTypeDef,
     TestRenderTemplateResponseTypeDef,
     VerifyDomainDkimResponseTypeDef,
     VerifyDomainIdentityResponseTypeDef,
-    MessageDsnTypeDef,
-    RecipientDsnFieldsTypeDef,
     GetIdentityDkimAttributesResponseTypeDef,
     GetIdentityMailFromDomainAttributesResponseTypeDef,
     GetIdentityNotificationAttributesResponseTypeDef,
     GetIdentityVerificationAttributesRequestIdentityExistsWaitTypeDef,
     GetIdentityVerificationAttributesResponseTypeDef,
     GetSendStatisticsResponseTypeDef,
     ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef,
     ListCustomVerificationEmailTemplatesRequestListCustomVerificationEmailTemplatesPaginateTypeDef,
     ListIdentitiesRequestListIdentitiesPaginateTypeDef,
     ListReceiptRuleSetsRequestListReceiptRuleSetsPaginateTypeDef,
     ListTemplatesRequestListTemplatesPaginateTypeDef,
     ListTemplatesResponseTypeDef,
-    SendRawEmailRequestRequestTypeDef,
+    MessageDsnTypeDef,
+    RecipientDsnFieldsTypeDef,
     ReceiptActionTypeDef,
     ReceiptFilterTypeDef,
+    SendRawEmailRequestRequestTypeDef,
     MessageTypeDef,
     SendBulkTemplatedEmailRequestRequestTypeDef,
     EventDestinationOutputTypeDef,
     EventDestinationTypeDef,
     BouncedRecipientInfoTypeDef,
     ReceiptRuleOutputTypeDef,
     ReceiptRuleTypeDef,
     CreateReceiptFilterRequestRequestTypeDef,
     ListReceiptFiltersResponseTypeDef,
     SendEmailRequestRequestTypeDef,
     DescribeConfigurationSetResponseTypeDef,
     CreateConfigurationSetEventDestinationRequestRequestTypeDef,
+    EventDestinationUnionTypeDef,
     UpdateConfigurationSetEventDestinationRequestRequestTypeDef,
     SendBounceRequestRequestTypeDef,
     DescribeActiveReceiptRuleSetResponseTypeDef,
     DescribeReceiptRuleResponseTypeDef,
     DescribeReceiptRuleSetResponseTypeDef,
     CreateReceiptRuleRequestRequestTypeDef,
+    ReceiptRuleUnionTypeDef,
     UpdateReceiptRuleRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AddHeaderActionTypeDef:
+def get_value() -> AddHeaderActionTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-ses-1.28.15.post1/mypy_boto3_ses/__init__.py` & `mypy-boto3-ses-1.28.16/mypy_boto3_ses/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ses-1.28.15.post1/mypy_boto3_ses/__init__.pyi` & `mypy-boto3-ses-1.28.16/mypy_boto3_ses/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ses-1.28.15.post1/mypy_boto3_ses/__main__.py` & `mypy-boto3-ses-1.28.16/mypy_boto3_ses/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SES 1.28.15\nVersion:         1.28.15.post1\nBuilder version:"
-        " 7.16.2\nDocs:           "
+        "Type annotations for boto3.SES 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES\nOther"
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

### Comparing `mypy-boto3-ses-1.28.15.post1/mypy_boto3_ses/client.py` & `mypy-boto3-ses-1.28.16/mypy_boto3_ses/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_ses.client import SESClient
 
     session = Session()
     client: SESClient = session.client("ses")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     BehaviorOnMXFailureType,
     ConfigurationSetAttributeType,
     IdentityTypeType,
@@ -38,16 +38,15 @@
     DeliveryOptionsTypeDef,
     DescribeActiveReceiptRuleSetResponseTypeDef,
     DescribeConfigurationSetResponseTypeDef,
     DescribeReceiptRuleResponseTypeDef,
     DescribeReceiptRuleSetResponseTypeDef,
     DestinationTypeDef,
     EmptyResponseMetadataTypeDef,
-    EventDestinationOutputTypeDef,
-    EventDestinationTypeDef,
+    EventDestinationUnionTypeDef,
     GetAccountSendingEnabledResponseTypeDef,
     GetCustomVerificationEmailTemplateResponseTypeDef,
     GetIdentityDkimAttributesResponseTypeDef,
     GetIdentityMailFromDomainAttributesResponseTypeDef,
     GetIdentityNotificationAttributesResponseTypeDef,
     GetIdentityPoliciesResponseTypeDef,
     GetIdentityVerificationAttributesResponseTypeDef,
@@ -63,16 +62,15 @@
     ListTemplatesResponseTypeDef,
     ListVerifiedEmailAddressesResponseTypeDef,
     MessageDsnTypeDef,
     MessageTagTypeDef,
     MessageTypeDef,
     RawMessageTypeDef,
     ReceiptFilterTypeDef,
-    ReceiptRuleOutputTypeDef,
-    ReceiptRuleTypeDef,
+    ReceiptRuleUnionTypeDef,
     SendBounceResponseTypeDef,
     SendBulkTemplatedEmailResponseTypeDef,
     SendCustomVerificationEmailResponseTypeDef,
     SendEmailResponseTypeDef,
     SendRawEmailResponseTypeDef,
     SendTemplatedEmailResponseTypeDef,
     TemplateTypeDef,
@@ -188,18 +186,15 @@
         Creates a configuration set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Client.create_configuration_set)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/client/#create_configuration_set)
         """
 
     def create_configuration_set_event_destination(
-        self,
-        *,
-        ConfigurationSetName: str,
-        EventDestination: Union[EventDestinationTypeDef, EventDestinationOutputTypeDef]
+        self, *, ConfigurationSetName: str, EventDestination: EventDestinationUnionTypeDef
     ) -> Dict[str, Any]:
         """
         Creates a configuration set event destination.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Client.create_configuration_set_event_destination)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/client/#create_configuration_set_event_destination)
         """
@@ -237,19 +232,15 @@
         Creates a new IP address filter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Client.create_receipt_filter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/client/#create_receipt_filter)
         """
 
     def create_receipt_rule(
-        self,
-        *,
-        RuleSetName: str,
-        Rule: Union[ReceiptRuleTypeDef, ReceiptRuleOutputTypeDef],
-        After: str = ...
+        self, *, RuleSetName: str, Rule: ReceiptRuleUnionTypeDef, After: str = ...
     ) -> Dict[str, Any]:
         """
         Creates a receipt rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Client.create_receipt_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/client/#create_receipt_rule)
         """
@@ -839,18 +830,15 @@
         current AWS Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Client.update_account_sending_enabled)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/client/#update_account_sending_enabled)
         """
 
     def update_configuration_set_event_destination(
-        self,
-        *,
-        ConfigurationSetName: str,
-        EventDestination: Union[EventDestinationTypeDef, EventDestinationOutputTypeDef]
+        self, *, ConfigurationSetName: str, EventDestination: EventDestinationUnionTypeDef
     ) -> Dict[str, Any]:
         """
         Updates the event destination of a configuration set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Client.update_configuration_set_event_destination)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/client/#update_configuration_set_event_destination)
         """
@@ -902,15 +890,15 @@
         Updates an existing custom verification email template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Client.update_custom_verification_email_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/client/#update_custom_verification_email_template)
         """
 
     def update_receipt_rule(
-        self, *, RuleSetName: str, Rule: Union[ReceiptRuleTypeDef, ReceiptRuleOutputTypeDef]
+        self, *, RuleSetName: str, Rule: ReceiptRuleUnionTypeDef
     ) -> Dict[str, Any]:
         """
         Updates a receipt rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Client.update_receipt_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/client/#update_receipt_rule)
         """
```

### Comparing `mypy-boto3-ses-1.28.15.post1/mypy_boto3_ses/client.pyi` & `mypy-boto3-ses-1.28.16/mypy_boto3_ses/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_ses.client import SESClient
 
     session = Session()
     client: SESClient = session.client("ses")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     BehaviorOnMXFailureType,
     ConfigurationSetAttributeType,
     IdentityTypeType,
@@ -38,16 +38,15 @@
     DeliveryOptionsTypeDef,
     DescribeActiveReceiptRuleSetResponseTypeDef,
     DescribeConfigurationSetResponseTypeDef,
     DescribeReceiptRuleResponseTypeDef,
     DescribeReceiptRuleSetResponseTypeDef,
     DestinationTypeDef,
     EmptyResponseMetadataTypeDef,
-    EventDestinationOutputTypeDef,
-    EventDestinationTypeDef,
+    EventDestinationUnionTypeDef,
     GetAccountSendingEnabledResponseTypeDef,
     GetCustomVerificationEmailTemplateResponseTypeDef,
     GetIdentityDkimAttributesResponseTypeDef,
     GetIdentityMailFromDomainAttributesResponseTypeDef,
     GetIdentityNotificationAttributesResponseTypeDef,
     GetIdentityPoliciesResponseTypeDef,
     GetIdentityVerificationAttributesResponseTypeDef,
@@ -63,16 +62,15 @@
     ListTemplatesResponseTypeDef,
     ListVerifiedEmailAddressesResponseTypeDef,
     MessageDsnTypeDef,
     MessageTagTypeDef,
     MessageTypeDef,
     RawMessageTypeDef,
     ReceiptFilterTypeDef,
-    ReceiptRuleOutputTypeDef,
-    ReceiptRuleTypeDef,
+    ReceiptRuleUnionTypeDef,
     SendBounceResponseTypeDef,
     SendBulkTemplatedEmailResponseTypeDef,
     SendCustomVerificationEmailResponseTypeDef,
     SendEmailResponseTypeDef,
     SendRawEmailResponseTypeDef,
     SendTemplatedEmailResponseTypeDef,
     TemplateTypeDef,
@@ -179,18 +177,15 @@
         """
         Creates a configuration set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Client.create_configuration_set)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/client/#create_configuration_set)
         """
     def create_configuration_set_event_destination(
-        self,
-        *,
-        ConfigurationSetName: str,
-        EventDestination: Union[EventDestinationTypeDef, EventDestinationOutputTypeDef]
+        self, *, ConfigurationSetName: str, EventDestination: EventDestinationUnionTypeDef
     ) -> Dict[str, Any]:
         """
         Creates a configuration set event destination.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Client.create_configuration_set_event_destination)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/client/#create_configuration_set_event_destination)
         """
@@ -224,19 +219,15 @@
         """
         Creates a new IP address filter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Client.create_receipt_filter)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/client/#create_receipt_filter)
         """
     def create_receipt_rule(
-        self,
-        *,
-        RuleSetName: str,
-        Rule: Union[ReceiptRuleTypeDef, ReceiptRuleOutputTypeDef],
-        After: str = ...
+        self, *, RuleSetName: str, Rule: ReceiptRuleUnionTypeDef, After: str = ...
     ) -> Dict[str, Any]:
         """
         Creates a receipt rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Client.create_receipt_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/client/#create_receipt_rule)
         """
@@ -771,18 +762,15 @@
         Enables or disables email sending across your entire Amazon SES account in the
         current AWS Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Client.update_account_sending_enabled)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/client/#update_account_sending_enabled)
         """
     def update_configuration_set_event_destination(
-        self,
-        *,
-        ConfigurationSetName: str,
-        EventDestination: Union[EventDestinationTypeDef, EventDestinationOutputTypeDef]
+        self, *, ConfigurationSetName: str, EventDestination: EventDestinationUnionTypeDef
     ) -> Dict[str, Any]:
         """
         Updates the event destination of a configuration set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Client.update_configuration_set_event_destination)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/client/#update_configuration_set_event_destination)
         """
@@ -829,15 +817,15 @@
         """
         Updates an existing custom verification email template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Client.update_custom_verification_email_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/client/#update_custom_verification_email_template)
         """
     def update_receipt_rule(
-        self, *, RuleSetName: str, Rule: Union[ReceiptRuleTypeDef, ReceiptRuleOutputTypeDef]
+        self, *, RuleSetName: str, Rule: ReceiptRuleUnionTypeDef
     ) -> Dict[str, Any]:
         """
         Updates a receipt rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Client.update_receipt_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/client/#update_receipt_rule)
         """
```

### Comparing `mypy-boto3-ses-1.28.15.post1/mypy_boto3_ses/literals.py` & `mypy-boto3-ses-1.28.16/mypy_boto3_ses/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ses-1.28.15.post1/mypy_boto3_ses/literals.pyi` & `mypy-boto3-ses-1.28.16/mypy_boto3_ses/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ses-1.28.15.post1/mypy_boto3_ses/paginator.py` & `mypy-boto3-ses-1.28.16/mypy_boto3_ses/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ses-1.28.15.post1/mypy_boto3_ses/paginator.pyi` & `mypy-boto3-ses-1.28.16/mypy_boto3_ses/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ses-1.28.15.post1/mypy_boto3_ses/type_defs.py` & `mypy-boto3-ses-1.28.16/mypy_boto3_ses/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_ses.type_defs import AddHeaderActionTypeDef
 
-    data: AddHeaderActionTypeDef = {...}
+    data: AddHeaderActionTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -43,14 +43,15 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AddHeaderActionTypeDef",
+    "BlobTypeDef",
     "ContentTypeDef",
     "BounceActionTypeDef",
     "BulkEmailDestinationStatusTypeDef",
     "DestinationTypeDef",
     "MessageTagTypeDef",
     "CloneReceiptRuleSetRequestRequestTypeDef",
     "CloudWatchDimensionConfigurationTypeDef",
@@ -99,16 +100,16 @@
     "ListConfigurationSetsRequestRequestTypeDef",
     "ListCustomVerificationEmailTemplatesRequestRequestTypeDef",
     "ListIdentitiesRequestRequestTypeDef",
     "ListIdentityPoliciesRequestRequestTypeDef",
     "ListReceiptRuleSetsRequestRequestTypeDef",
     "ListTemplatesRequestRequestTypeDef",
     "TemplateMetadataTypeDef",
+    "TimestampTypeDef",
     "PutIdentityPolicyRequestRequestTypeDef",
-    "RawMessageTypeDef",
     "S3ActionTypeDef",
     "SNSActionTypeDef",
     "StopActionTypeDef",
     "WorkmailActionTypeDef",
     "ReceiptIpFilterTypeDef",
     "ReorderReceiptRuleSetRequestRequestTypeDef",
     "SendCustomVerificationEmailRequestRequestTypeDef",
@@ -124,14 +125,15 @@
     "UpdateConfigurationSetReputationMetricsEnabledRequestRequestTypeDef",
     "UpdateConfigurationSetSendingEnabledRequestRequestTypeDef",
     "UpdateCustomVerificationEmailTemplateRequestRequestTypeDef",
     "VerifyDomainDkimRequestRequestTypeDef",
     "VerifyDomainIdentityRequestRequestTypeDef",
     "VerifyEmailAddressRequestRequestTypeDef",
     "VerifyEmailIdentityRequestRequestTypeDef",
+    "RawMessageTypeDef",
     "BodyTypeDef",
     "BulkEmailDestinationTypeDef",
     "SendTemplatedEmailRequestRequestTypeDef",
     "CloudWatchDestinationOutputTypeDef",
     "CloudWatchDestinationTypeDef",
     "CreateConfigurationSetRequestRequestTypeDef",
     "CreateConfigurationSetTrackingOptionsRequestRequestTypeDef",
@@ -156,60 +158,63 @@
     "SendCustomVerificationEmailResponseTypeDef",
     "SendEmailResponseTypeDef",
     "SendRawEmailResponseTypeDef",
     "SendTemplatedEmailResponseTypeDef",
     "TestRenderTemplateResponseTypeDef",
     "VerifyDomainDkimResponseTypeDef",
     "VerifyDomainIdentityResponseTypeDef",
-    "MessageDsnTypeDef",
-    "RecipientDsnFieldsTypeDef",
     "GetIdentityDkimAttributesResponseTypeDef",
     "GetIdentityMailFromDomainAttributesResponseTypeDef",
     "GetIdentityNotificationAttributesResponseTypeDef",
     "GetIdentityVerificationAttributesRequestIdentityExistsWaitTypeDef",
     "GetIdentityVerificationAttributesResponseTypeDef",
     "GetSendStatisticsResponseTypeDef",
     "ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef",
     "ListCustomVerificationEmailTemplatesRequestListCustomVerificationEmailTemplatesPaginateTypeDef",
     "ListIdentitiesRequestListIdentitiesPaginateTypeDef",
     "ListReceiptRuleSetsRequestListReceiptRuleSetsPaginateTypeDef",
     "ListTemplatesRequestListTemplatesPaginateTypeDef",
     "ListTemplatesResponseTypeDef",
-    "SendRawEmailRequestRequestTypeDef",
+    "MessageDsnTypeDef",
+    "RecipientDsnFieldsTypeDef",
     "ReceiptActionTypeDef",
     "ReceiptFilterTypeDef",
+    "SendRawEmailRequestRequestTypeDef",
     "MessageTypeDef",
     "SendBulkTemplatedEmailRequestRequestTypeDef",
     "EventDestinationOutputTypeDef",
     "EventDestinationTypeDef",
     "BouncedRecipientInfoTypeDef",
     "ReceiptRuleOutputTypeDef",
     "ReceiptRuleTypeDef",
     "CreateReceiptFilterRequestRequestTypeDef",
     "ListReceiptFiltersResponseTypeDef",
     "SendEmailRequestRequestTypeDef",
     "DescribeConfigurationSetResponseTypeDef",
     "CreateConfigurationSetEventDestinationRequestRequestTypeDef",
+    "EventDestinationUnionTypeDef",
     "UpdateConfigurationSetEventDestinationRequestRequestTypeDef",
     "SendBounceRequestRequestTypeDef",
     "DescribeActiveReceiptRuleSetResponseTypeDef",
     "DescribeReceiptRuleResponseTypeDef",
     "DescribeReceiptRuleSetResponseTypeDef",
     "CreateReceiptRuleRequestRequestTypeDef",
+    "ReceiptRuleUnionTypeDef",
     "UpdateReceiptRuleRequestRequestTypeDef",
 )
 
 AddHeaderActionTypeDef = TypedDict(
     "AddHeaderActionTypeDef",
     {
         "HeaderName": str,
         "HeaderValue": str,
     },
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 _RequiredContentTypeDef = TypedDict(
     "_RequiredContentTypeDef",
     {
         "Data": str,
     },
 )
 _OptionalContentTypeDef = TypedDict(
@@ -773,30 +778,24 @@
     {
         "Name": str,
         "CreatedTimestamp": datetime,
     },
     total=False,
 )
 
+TimestampTypeDef = Union[datetime, str]
 PutIdentityPolicyRequestRequestTypeDef = TypedDict(
     "PutIdentityPolicyRequestRequestTypeDef",
     {
         "Identity": str,
         "PolicyName": str,
         "Policy": str,
     },
 )
 
-RawMessageTypeDef = TypedDict(
-    "RawMessageTypeDef",
-    {
-        "Data": Union[str, bytes, IO[Any], StreamingBody],
-    },
-)
-
 _RequiredS3ActionTypeDef = TypedDict(
     "_RequiredS3ActionTypeDef",
     {
         "BucketName": str,
     },
 )
 _OptionalS3ActionTypeDef = TypedDict(
@@ -1094,14 +1093,21 @@
 VerifyEmailIdentityRequestRequestTypeDef = TypedDict(
     "VerifyEmailIdentityRequestRequestTypeDef",
     {
         "EmailAddress": str,
     },
 )
 
+RawMessageTypeDef = TypedDict(
+    "RawMessageTypeDef",
+    {
+        "Data": BlobTypeDef,
+    },
+)
+
 BodyTypeDef = TypedDict(
     "BodyTypeDef",
     {
         "Text": ContentTypeDef,
         "Html": ContentTypeDef,
     },
     total=False,
@@ -1407,60 +1413,14 @@
     "VerifyDomainIdentityResponseTypeDef",
     {
         "VerificationToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredMessageDsnTypeDef = TypedDict(
-    "_RequiredMessageDsnTypeDef",
-    {
-        "ReportingMta": str,
-    },
-)
-_OptionalMessageDsnTypeDef = TypedDict(
-    "_OptionalMessageDsnTypeDef",
-    {
-        "ArrivalDate": Union[datetime, str],
-        "ExtensionFields": Sequence[ExtensionFieldTypeDef],
-    },
-    total=False,
-)
-
-
-class MessageDsnTypeDef(_RequiredMessageDsnTypeDef, _OptionalMessageDsnTypeDef):
-    pass
-
-
-_RequiredRecipientDsnFieldsTypeDef = TypedDict(
-    "_RequiredRecipientDsnFieldsTypeDef",
-    {
-        "Action": DsnActionType,
-        "Status": str,
-    },
-)
-_OptionalRecipientDsnFieldsTypeDef = TypedDict(
-    "_OptionalRecipientDsnFieldsTypeDef",
-    {
-        "FinalRecipient": str,
-        "RemoteMta": str,
-        "DiagnosticCode": str,
-        "LastAttemptDate": Union[datetime, str],
-        "ExtensionFields": Sequence[ExtensionFieldTypeDef],
-    },
-    total=False,
-)
-
-
-class RecipientDsnFieldsTypeDef(
-    _RequiredRecipientDsnFieldsTypeDef, _OptionalRecipientDsnFieldsTypeDef
-):
-    pass
-
-
 GetIdentityDkimAttributesResponseTypeDef = TypedDict(
     "GetIdentityDkimAttributesResponseTypeDef",
     {
         "DkimAttributes": Dict[str, IdentityDkimAttributesTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1565,37 +1525,56 @@
     {
         "TemplatesMetadata": List[TemplateMetadataTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredSendRawEmailRequestRequestTypeDef = TypedDict(
-    "_RequiredSendRawEmailRequestRequestTypeDef",
+_RequiredMessageDsnTypeDef = TypedDict(
+    "_RequiredMessageDsnTypeDef",
     {
-        "RawMessage": RawMessageTypeDef,
+        "ReportingMta": str,
     },
 )
-_OptionalSendRawEmailRequestRequestTypeDef = TypedDict(
-    "_OptionalSendRawEmailRequestRequestTypeDef",
+_OptionalMessageDsnTypeDef = TypedDict(
+    "_OptionalMessageDsnTypeDef",
     {
-        "Source": str,
-        "Destinations": Sequence[str],
-        "FromArn": str,
-        "SourceArn": str,
-        "ReturnPathArn": str,
-        "Tags": Sequence[MessageTagTypeDef],
-        "ConfigurationSetName": str,
+        "ArrivalDate": TimestampTypeDef,
+        "ExtensionFields": Sequence[ExtensionFieldTypeDef],
     },
     total=False,
 )
 
 
-class SendRawEmailRequestRequestTypeDef(
-    _RequiredSendRawEmailRequestRequestTypeDef, _OptionalSendRawEmailRequestRequestTypeDef
+class MessageDsnTypeDef(_RequiredMessageDsnTypeDef, _OptionalMessageDsnTypeDef):
+    pass
+
+
+_RequiredRecipientDsnFieldsTypeDef = TypedDict(
+    "_RequiredRecipientDsnFieldsTypeDef",
+    {
+        "Action": DsnActionType,
+        "Status": str,
+    },
+)
+_OptionalRecipientDsnFieldsTypeDef = TypedDict(
+    "_OptionalRecipientDsnFieldsTypeDef",
+    {
+        "FinalRecipient": str,
+        "RemoteMta": str,
+        "DiagnosticCode": str,
+        "LastAttemptDate": TimestampTypeDef,
+        "ExtensionFields": Sequence[ExtensionFieldTypeDef],
+    },
+    total=False,
+)
+
+
+class RecipientDsnFieldsTypeDef(
+    _RequiredRecipientDsnFieldsTypeDef, _OptionalRecipientDsnFieldsTypeDef
 ):
     pass
 
 
 ReceiptActionTypeDef = TypedDict(
     "ReceiptActionTypeDef",
     {
@@ -1614,14 +1593,41 @@
     "ReceiptFilterTypeDef",
     {
         "Name": str,
         "IpFilter": ReceiptIpFilterTypeDef,
     },
 )
 
+_RequiredSendRawEmailRequestRequestTypeDef = TypedDict(
+    "_RequiredSendRawEmailRequestRequestTypeDef",
+    {
+        "RawMessage": RawMessageTypeDef,
+    },
+)
+_OptionalSendRawEmailRequestRequestTypeDef = TypedDict(
+    "_OptionalSendRawEmailRequestRequestTypeDef",
+    {
+        "Source": str,
+        "Destinations": Sequence[str],
+        "FromArn": str,
+        "SourceArn": str,
+        "ReturnPathArn": str,
+        "Tags": Sequence[MessageTagTypeDef],
+        "ConfigurationSetName": str,
+    },
+    total=False,
+)
+
+
+class SendRawEmailRequestRequestTypeDef(
+    _RequiredSendRawEmailRequestRequestTypeDef, _OptionalSendRawEmailRequestRequestTypeDef
+):
+    pass
+
+
 MessageTypeDef = TypedDict(
     "MessageTypeDef",
     {
         "Subject": ContentTypeDef,
         "Body": BodyTypeDef,
     },
 )
@@ -1835,14 +1841,15 @@
     "CreateConfigurationSetEventDestinationRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
         "EventDestination": EventDestinationTypeDef,
     },
 )
 
+EventDestinationUnionTypeDef = Union[EventDestinationTypeDef, EventDestinationOutputTypeDef]
 UpdateConfigurationSetEventDestinationRequestRequestTypeDef = TypedDict(
     "UpdateConfigurationSetEventDestinationRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
         "EventDestination": EventDestinationTypeDef,
     },
 )
@@ -1916,14 +1923,15 @@
 
 class CreateReceiptRuleRequestRequestTypeDef(
     _RequiredCreateReceiptRuleRequestRequestTypeDef, _OptionalCreateReceiptRuleRequestRequestTypeDef
 ):
     pass
 
 
+ReceiptRuleUnionTypeDef = Union[ReceiptRuleTypeDef, ReceiptRuleOutputTypeDef]
 UpdateReceiptRuleRequestRequestTypeDef = TypedDict(
     "UpdateReceiptRuleRequestRequestTypeDef",
     {
         "RuleSetName": str,
         "Rule": ReceiptRuleTypeDef,
     },
 )
```

### Comparing `mypy-boto3-ses-1.28.15.post1/mypy_boto3_ses/type_defs.pyi` & `mypy-boto3-ses-1.28.16/mypy_boto3_ses/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_ses.type_defs import AddHeaderActionTypeDef
 
-    data: AddHeaderActionTypeDef = {...}
+    data: AddHeaderActionTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -42,14 +42,15 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AddHeaderActionTypeDef",
+    "BlobTypeDef",
     "ContentTypeDef",
     "BounceActionTypeDef",
     "BulkEmailDestinationStatusTypeDef",
     "DestinationTypeDef",
     "MessageTagTypeDef",
     "CloneReceiptRuleSetRequestRequestTypeDef",
     "CloudWatchDimensionConfigurationTypeDef",
@@ -98,16 +99,16 @@
     "ListConfigurationSetsRequestRequestTypeDef",
     "ListCustomVerificationEmailTemplatesRequestRequestTypeDef",
     "ListIdentitiesRequestRequestTypeDef",
     "ListIdentityPoliciesRequestRequestTypeDef",
     "ListReceiptRuleSetsRequestRequestTypeDef",
     "ListTemplatesRequestRequestTypeDef",
     "TemplateMetadataTypeDef",
+    "TimestampTypeDef",
     "PutIdentityPolicyRequestRequestTypeDef",
-    "RawMessageTypeDef",
     "S3ActionTypeDef",
     "SNSActionTypeDef",
     "StopActionTypeDef",
     "WorkmailActionTypeDef",
     "ReceiptIpFilterTypeDef",
     "ReorderReceiptRuleSetRequestRequestTypeDef",
     "SendCustomVerificationEmailRequestRequestTypeDef",
@@ -123,14 +124,15 @@
     "UpdateConfigurationSetReputationMetricsEnabledRequestRequestTypeDef",
     "UpdateConfigurationSetSendingEnabledRequestRequestTypeDef",
     "UpdateCustomVerificationEmailTemplateRequestRequestTypeDef",
     "VerifyDomainDkimRequestRequestTypeDef",
     "VerifyDomainIdentityRequestRequestTypeDef",
     "VerifyEmailAddressRequestRequestTypeDef",
     "VerifyEmailIdentityRequestRequestTypeDef",
+    "RawMessageTypeDef",
     "BodyTypeDef",
     "BulkEmailDestinationTypeDef",
     "SendTemplatedEmailRequestRequestTypeDef",
     "CloudWatchDestinationOutputTypeDef",
     "CloudWatchDestinationTypeDef",
     "CreateConfigurationSetRequestRequestTypeDef",
     "CreateConfigurationSetTrackingOptionsRequestRequestTypeDef",
@@ -155,60 +157,63 @@
     "SendCustomVerificationEmailResponseTypeDef",
     "SendEmailResponseTypeDef",
     "SendRawEmailResponseTypeDef",
     "SendTemplatedEmailResponseTypeDef",
     "TestRenderTemplateResponseTypeDef",
     "VerifyDomainDkimResponseTypeDef",
     "VerifyDomainIdentityResponseTypeDef",
-    "MessageDsnTypeDef",
-    "RecipientDsnFieldsTypeDef",
     "GetIdentityDkimAttributesResponseTypeDef",
     "GetIdentityMailFromDomainAttributesResponseTypeDef",
     "GetIdentityNotificationAttributesResponseTypeDef",
     "GetIdentityVerificationAttributesRequestIdentityExistsWaitTypeDef",
     "GetIdentityVerificationAttributesResponseTypeDef",
     "GetSendStatisticsResponseTypeDef",
     "ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef",
     "ListCustomVerificationEmailTemplatesRequestListCustomVerificationEmailTemplatesPaginateTypeDef",
     "ListIdentitiesRequestListIdentitiesPaginateTypeDef",
     "ListReceiptRuleSetsRequestListReceiptRuleSetsPaginateTypeDef",
     "ListTemplatesRequestListTemplatesPaginateTypeDef",
     "ListTemplatesResponseTypeDef",
-    "SendRawEmailRequestRequestTypeDef",
+    "MessageDsnTypeDef",
+    "RecipientDsnFieldsTypeDef",
     "ReceiptActionTypeDef",
     "ReceiptFilterTypeDef",
+    "SendRawEmailRequestRequestTypeDef",
     "MessageTypeDef",
     "SendBulkTemplatedEmailRequestRequestTypeDef",
     "EventDestinationOutputTypeDef",
     "EventDestinationTypeDef",
     "BouncedRecipientInfoTypeDef",
     "ReceiptRuleOutputTypeDef",
     "ReceiptRuleTypeDef",
     "CreateReceiptFilterRequestRequestTypeDef",
     "ListReceiptFiltersResponseTypeDef",
     "SendEmailRequestRequestTypeDef",
     "DescribeConfigurationSetResponseTypeDef",
     "CreateConfigurationSetEventDestinationRequestRequestTypeDef",
+    "EventDestinationUnionTypeDef",
     "UpdateConfigurationSetEventDestinationRequestRequestTypeDef",
     "SendBounceRequestRequestTypeDef",
     "DescribeActiveReceiptRuleSetResponseTypeDef",
     "DescribeReceiptRuleResponseTypeDef",
     "DescribeReceiptRuleSetResponseTypeDef",
     "CreateReceiptRuleRequestRequestTypeDef",
+    "ReceiptRuleUnionTypeDef",
     "UpdateReceiptRuleRequestRequestTypeDef",
 )
 
 AddHeaderActionTypeDef = TypedDict(
     "AddHeaderActionTypeDef",
     {
         "HeaderName": str,
         "HeaderValue": str,
     },
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 _RequiredContentTypeDef = TypedDict(
     "_RequiredContentTypeDef",
     {
         "Data": str,
     },
 )
 _OptionalContentTypeDef = TypedDict(
@@ -756,30 +761,24 @@
     {
         "Name": str,
         "CreatedTimestamp": datetime,
     },
     total=False,
 )
 
+TimestampTypeDef = Union[datetime, str]
 PutIdentityPolicyRequestRequestTypeDef = TypedDict(
     "PutIdentityPolicyRequestRequestTypeDef",
     {
         "Identity": str,
         "PolicyName": str,
         "Policy": str,
     },
 )
 
-RawMessageTypeDef = TypedDict(
-    "RawMessageTypeDef",
-    {
-        "Data": Union[str, bytes, IO[Any], StreamingBody],
-    },
-)
-
 _RequiredS3ActionTypeDef = TypedDict(
     "_RequiredS3ActionTypeDef",
     {
         "BucketName": str,
     },
 )
 _OptionalS3ActionTypeDef = TypedDict(
@@ -1059,14 +1058,21 @@
 VerifyEmailIdentityRequestRequestTypeDef = TypedDict(
     "VerifyEmailIdentityRequestRequestTypeDef",
     {
         "EmailAddress": str,
     },
 )
 
+RawMessageTypeDef = TypedDict(
+    "RawMessageTypeDef",
+    {
+        "Data": BlobTypeDef,
+    },
+)
+
 BodyTypeDef = TypedDict(
     "BodyTypeDef",
     {
         "Text": ContentTypeDef,
         "Html": ContentTypeDef,
     },
     total=False,
@@ -1366,56 +1372,14 @@
     "VerifyDomainIdentityResponseTypeDef",
     {
         "VerificationToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredMessageDsnTypeDef = TypedDict(
-    "_RequiredMessageDsnTypeDef",
-    {
-        "ReportingMta": str,
-    },
-)
-_OptionalMessageDsnTypeDef = TypedDict(
-    "_OptionalMessageDsnTypeDef",
-    {
-        "ArrivalDate": Union[datetime, str],
-        "ExtensionFields": Sequence[ExtensionFieldTypeDef],
-    },
-    total=False,
-)
-
-class MessageDsnTypeDef(_RequiredMessageDsnTypeDef, _OptionalMessageDsnTypeDef):
-    pass
-
-_RequiredRecipientDsnFieldsTypeDef = TypedDict(
-    "_RequiredRecipientDsnFieldsTypeDef",
-    {
-        "Action": DsnActionType,
-        "Status": str,
-    },
-)
-_OptionalRecipientDsnFieldsTypeDef = TypedDict(
-    "_OptionalRecipientDsnFieldsTypeDef",
-    {
-        "FinalRecipient": str,
-        "RemoteMta": str,
-        "DiagnosticCode": str,
-        "LastAttemptDate": Union[datetime, str],
-        "ExtensionFields": Sequence[ExtensionFieldTypeDef],
-    },
-    total=False,
-)
-
-class RecipientDsnFieldsTypeDef(
-    _RequiredRecipientDsnFieldsTypeDef, _OptionalRecipientDsnFieldsTypeDef
-):
-    pass
-
 GetIdentityDkimAttributesResponseTypeDef = TypedDict(
     "GetIdentityDkimAttributesResponseTypeDef",
     {
         "DkimAttributes": Dict[str, IdentityDkimAttributesTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1518,36 +1482,53 @@
     {
         "TemplatesMetadata": List[TemplateMetadataTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredSendRawEmailRequestRequestTypeDef = TypedDict(
-    "_RequiredSendRawEmailRequestRequestTypeDef",
+_RequiredMessageDsnTypeDef = TypedDict(
+    "_RequiredMessageDsnTypeDef",
     {
-        "RawMessage": RawMessageTypeDef,
+        "ReportingMta": str,
     },
 )
-_OptionalSendRawEmailRequestRequestTypeDef = TypedDict(
-    "_OptionalSendRawEmailRequestRequestTypeDef",
+_OptionalMessageDsnTypeDef = TypedDict(
+    "_OptionalMessageDsnTypeDef",
     {
-        "Source": str,
-        "Destinations": Sequence[str],
-        "FromArn": str,
-        "SourceArn": str,
-        "ReturnPathArn": str,
-        "Tags": Sequence[MessageTagTypeDef],
-        "ConfigurationSetName": str,
+        "ArrivalDate": TimestampTypeDef,
+        "ExtensionFields": Sequence[ExtensionFieldTypeDef],
     },
     total=False,
 )
 
-class SendRawEmailRequestRequestTypeDef(
-    _RequiredSendRawEmailRequestRequestTypeDef, _OptionalSendRawEmailRequestRequestTypeDef
+class MessageDsnTypeDef(_RequiredMessageDsnTypeDef, _OptionalMessageDsnTypeDef):
+    pass
+
+_RequiredRecipientDsnFieldsTypeDef = TypedDict(
+    "_RequiredRecipientDsnFieldsTypeDef",
+    {
+        "Action": DsnActionType,
+        "Status": str,
+    },
+)
+_OptionalRecipientDsnFieldsTypeDef = TypedDict(
+    "_OptionalRecipientDsnFieldsTypeDef",
+    {
+        "FinalRecipient": str,
+        "RemoteMta": str,
+        "DiagnosticCode": str,
+        "LastAttemptDate": TimestampTypeDef,
+        "ExtensionFields": Sequence[ExtensionFieldTypeDef],
+    },
+    total=False,
+)
+
+class RecipientDsnFieldsTypeDef(
+    _RequiredRecipientDsnFieldsTypeDef, _OptionalRecipientDsnFieldsTypeDef
 ):
     pass
 
 ReceiptActionTypeDef = TypedDict(
     "ReceiptActionTypeDef",
     {
         "S3Action": S3ActionTypeDef,
@@ -1565,14 +1546,39 @@
     "ReceiptFilterTypeDef",
     {
         "Name": str,
         "IpFilter": ReceiptIpFilterTypeDef,
     },
 )
 
+_RequiredSendRawEmailRequestRequestTypeDef = TypedDict(
+    "_RequiredSendRawEmailRequestRequestTypeDef",
+    {
+        "RawMessage": RawMessageTypeDef,
+    },
+)
+_OptionalSendRawEmailRequestRequestTypeDef = TypedDict(
+    "_OptionalSendRawEmailRequestRequestTypeDef",
+    {
+        "Source": str,
+        "Destinations": Sequence[str],
+        "FromArn": str,
+        "SourceArn": str,
+        "ReturnPathArn": str,
+        "Tags": Sequence[MessageTagTypeDef],
+        "ConfigurationSetName": str,
+    },
+    total=False,
+)
+
+class SendRawEmailRequestRequestTypeDef(
+    _RequiredSendRawEmailRequestRequestTypeDef, _OptionalSendRawEmailRequestRequestTypeDef
+):
+    pass
+
 MessageTypeDef = TypedDict(
     "MessageTypeDef",
     {
         "Subject": ContentTypeDef,
         "Body": BodyTypeDef,
     },
 )
@@ -1772,14 +1778,15 @@
     "CreateConfigurationSetEventDestinationRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
         "EventDestination": EventDestinationTypeDef,
     },
 )
 
+EventDestinationUnionTypeDef = Union[EventDestinationTypeDef, EventDestinationOutputTypeDef]
 UpdateConfigurationSetEventDestinationRequestRequestTypeDef = TypedDict(
     "UpdateConfigurationSetEventDestinationRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
         "EventDestination": EventDestinationTypeDef,
     },
 )
@@ -1849,14 +1856,15 @@
 )
 
 class CreateReceiptRuleRequestRequestTypeDef(
     _RequiredCreateReceiptRuleRequestRequestTypeDef, _OptionalCreateReceiptRuleRequestRequestTypeDef
 ):
     pass
 
+ReceiptRuleUnionTypeDef = Union[ReceiptRuleTypeDef, ReceiptRuleOutputTypeDef]
 UpdateReceiptRuleRequestRequestTypeDef = TypedDict(
     "UpdateReceiptRuleRequestRequestTypeDef",
     {
         "RuleSetName": str,
         "Rule": ReceiptRuleTypeDef,
     },
 )
```

### Comparing `mypy-boto3-ses-1.28.15.post1/mypy_boto3_ses/waiter.py` & `mypy-boto3-ses-1.28.16/mypy_boto3_ses/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ses-1.28.15.post1/mypy_boto3_ses/waiter.pyi` & `mypy-boto3-ses-1.28.16/mypy_boto3_ses/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ses-1.28.15.post1/mypy_boto3_ses.egg-info/PKG-INFO` & `mypy-boto3-ses-1.28.16/mypy_boto3_ses.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ses
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.SES 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.SES 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 ses type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 ses type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ses.svg?color=blue)](https://pypi.org/project/mypy-boto3-ses)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ses)](https://pepy.tech/project/mypy-boto3-ses)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SES 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES)
+[boto3.SES 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES)
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
 [mypy-boto3-ses docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/).
 
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
@@ -366,24 +366,25 @@
 )
 
 
 def check_value(value: BehaviorOnMXFailureType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_ses.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_ses.type_defs import (
     AddHeaderActionTypeDef,
+    BlobTypeDef,
     ContentTypeDef,
     BounceActionTypeDef,
     BulkEmailDestinationStatusTypeDef,
     DestinationTypeDef,
     MessageTagTypeDef,
     CloneReceiptRuleSetRequestRequestTypeDef,
     CloudWatchDimensionConfigurationTypeDef,
@@ -432,16 +433,16 @@
     ListConfigurationSetsRequestRequestTypeDef,
     ListCustomVerificationEmailTemplatesRequestRequestTypeDef,
     ListIdentitiesRequestRequestTypeDef,
     ListIdentityPoliciesRequestRequestTypeDef,
     ListReceiptRuleSetsRequestRequestTypeDef,
     ListTemplatesRequestRequestTypeDef,
     TemplateMetadataTypeDef,
+    TimestampTypeDef,
     PutIdentityPolicyRequestRequestTypeDef,
-    RawMessageTypeDef,
     S3ActionTypeDef,
     SNSActionTypeDef,
     StopActionTypeDef,
     WorkmailActionTypeDef,
     ReceiptIpFilterTypeDef,
     ReorderReceiptRuleSetRequestRequestTypeDef,
     SendCustomVerificationEmailRequestRequestTypeDef,
@@ -457,14 +458,15 @@
     UpdateConfigurationSetReputationMetricsEnabledRequestRequestTypeDef,
     UpdateConfigurationSetSendingEnabledRequestRequestTypeDef,
     UpdateCustomVerificationEmailTemplateRequestRequestTypeDef,
     VerifyDomainDkimRequestRequestTypeDef,
     VerifyDomainIdentityRequestRequestTypeDef,
     VerifyEmailAddressRequestRequestTypeDef,
     VerifyEmailIdentityRequestRequestTypeDef,
+    RawMessageTypeDef,
     BodyTypeDef,
     BulkEmailDestinationTypeDef,
     SendTemplatedEmailRequestRequestTypeDef,
     CloudWatchDestinationOutputTypeDef,
     CloudWatchDestinationTypeDef,
     CreateConfigurationSetRequestRequestTypeDef,
     CreateConfigurationSetTrackingOptionsRequestRequestTypeDef,
@@ -489,54 +491,56 @@
     SendCustomVerificationEmailResponseTypeDef,
     SendEmailResponseTypeDef,
     SendRawEmailResponseTypeDef,
     SendTemplatedEmailResponseTypeDef,
     TestRenderTemplateResponseTypeDef,
     VerifyDomainDkimResponseTypeDef,
     VerifyDomainIdentityResponseTypeDef,
-    MessageDsnTypeDef,
-    RecipientDsnFieldsTypeDef,
     GetIdentityDkimAttributesResponseTypeDef,
     GetIdentityMailFromDomainAttributesResponseTypeDef,
     GetIdentityNotificationAttributesResponseTypeDef,
     GetIdentityVerificationAttributesRequestIdentityExistsWaitTypeDef,
     GetIdentityVerificationAttributesResponseTypeDef,
     GetSendStatisticsResponseTypeDef,
     ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef,
     ListCustomVerificationEmailTemplatesRequestListCustomVerificationEmailTemplatesPaginateTypeDef,
     ListIdentitiesRequestListIdentitiesPaginateTypeDef,
     ListReceiptRuleSetsRequestListReceiptRuleSetsPaginateTypeDef,
     ListTemplatesRequestListTemplatesPaginateTypeDef,
     ListTemplatesResponseTypeDef,
-    SendRawEmailRequestRequestTypeDef,
+    MessageDsnTypeDef,
+    RecipientDsnFieldsTypeDef,
     ReceiptActionTypeDef,
     ReceiptFilterTypeDef,
+    SendRawEmailRequestRequestTypeDef,
     MessageTypeDef,
     SendBulkTemplatedEmailRequestRequestTypeDef,
     EventDestinationOutputTypeDef,
     EventDestinationTypeDef,
     BouncedRecipientInfoTypeDef,
     ReceiptRuleOutputTypeDef,
     ReceiptRuleTypeDef,
     CreateReceiptFilterRequestRequestTypeDef,
     ListReceiptFiltersResponseTypeDef,
     SendEmailRequestRequestTypeDef,
     DescribeConfigurationSetResponseTypeDef,
     CreateConfigurationSetEventDestinationRequestRequestTypeDef,
+    EventDestinationUnionTypeDef,
     UpdateConfigurationSetEventDestinationRequestRequestTypeDef,
     SendBounceRequestRequestTypeDef,
     DescribeActiveReceiptRuleSetResponseTypeDef,
     DescribeReceiptRuleResponseTypeDef,
     DescribeReceiptRuleSetResponseTypeDef,
     CreateReceiptRuleRequestRequestTypeDef,
+    ReceiptRuleUnionTypeDef,
     UpdateReceiptRuleRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AddHeaderActionTypeDef:
+def get_value() -> AddHeaderActionTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-ses-1.28.15.post1/mypy_boto3_ses.egg-info/SOURCES.txt` & `mypy-boto3-ses-1.28.16/mypy_boto3_ses.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ses-1.28.15.post1/setup.py` & `mypy-boto3-ses-1.28.16/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-ses",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_ses"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.SES 1.28.15 service generated with mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.SES 1.28.16 service generated with mypy-boto3-builder 7.17.1"
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
-    keywords="boto3 ses type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 ses type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_ses": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

