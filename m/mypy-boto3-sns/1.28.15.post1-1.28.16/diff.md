# Comparing `tmp/mypy-boto3-sns-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-sns-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-sns-1.28.15.post1.tar", last modified: Sat Jul 29 10:04:15 2023, max compression
+gzip compressed data, was "mypy-boto3-sns-1.28.16.tar", last modified: Tue Aug  1 11:37:54 2023, max compression
```

## Comparing `mypy-boto3-sns-1.28.15.post1.tar` & `mypy-boto3-sns-1.28.16.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:15.573417 mypy-boto3-sns-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:59:51.000000 mypy-boto3-sns-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20738 2023-07-29 10:04:15.569417 mypy-boto3-sns-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19261 2023-07-29 09:59:51.000000 mypy-boto3-sns-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:15.561417 mypy-boto3-sns-1.28.15.post1/mypy_boto3_sns/
--rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-07-29 09:59:51.000000 mypy-boto3-sns-1.28.15.post1/mypy_boto3_sns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-07-29 09:59:51.000000 mypy-boto3-sns-1.28.15.post1/mypy_boto3_sns/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-29 09:59:51.000000 mypy-boto3-sns-1.28.15.post1/mypy_boto3_sns/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33218 2023-07-29 09:59:51.000000 mypy-boto3-sns-1.28.15.post1/mypy_boto3_sns/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    33161 2023-07-29 09:59:51.000000 mypy-boto3-sns-1.28.15.post1/mypy_boto3_sns/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9936 2023-07-29 09:59:51.000000 mypy-boto3-sns-1.28.15.post1/mypy_boto3_sns/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9934 2023-07-29 09:59:51.000000 mypy-boto3-sns-1.28.15.post1/mypy_boto3_sns/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9594 2023-07-29 09:59:51.000000 mypy-boto3-sns-1.28.15.post1/mypy_boto3_sns/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9584 2023-07-29 09:59:51.000000 mypy-boto3-sns-1.28.15.post1/mypy_boto3_sns/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:59:51.000000 mypy-boto3-sns-1.28.15.post1/mypy_boto3_sns/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    33864 2023-07-29 09:59:51.000000 mypy-boto3-sns-1.28.15.post1/mypy_boto3_sns/service_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    33795 2023-07-29 09:59:51.000000 mypy-boto3-sns-1.28.15.post1/mypy_boto3_sns/service_resource.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    34544 2023-07-29 09:59:57.000000 mypy-boto3-sns-1.28.15.post1/mypy_boto3_sns/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    34497 2023-07-29 09:59:52.000000 mypy-boto3-sns-1.28.15.post1/mypy_boto3_sns/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:59:51.000000 mypy-boto3-sns-1.28.15.post1/mypy_boto3_sns/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:15.565417 mypy-boto3-sns-1.28.15.post1/mypy_boto3_sns.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20738 2023-07-29 10:04:15.000000 mypy-boto3-sns-1.28.15.post1/mypy_boto3_sns.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-29 10:04:15.000000 mypy-boto3-sns-1.28.15.post1/mypy_boto3_sns.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:15.000000 mypy-boto3-sns-1.28.15.post1/mypy_boto3_sns.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:15.000000 mypy-boto3-sns-1.28.15.post1/mypy_boto3_sns.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:04:15.000000 mypy-boto3-sns-1.28.15.post1/mypy_boto3_sns.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-29 10:04:15.000000 mypy-boto3-sns-1.28.15.post1/mypy_boto3_sns.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:04:15.573417 mypy-boto3-sns-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-29 09:59:50.000000 mypy-boto3-sns-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:54.968721 mypy-boto3-sns-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:33:25.000000 mypy-boto3-sns-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20745 2023-08-01 11:37:54.964721 mypy-boto3-sns-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19277 2023-08-01 11:33:25.000000 mypy-boto3-sns-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:54.964721 mypy-boto3-sns-1.28.16/mypy_boto3_sns/
+-rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-08-01 11:33:25.000000 mypy-boto3-sns-1.28.16/mypy_boto3_sns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-08-01 11:33:25.000000 mypy-boto3-sns-1.28.16/mypy_boto3_sns/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-08-01 11:33:25.000000 mypy-boto3-sns-1.28.16/mypy_boto3_sns/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33218 2023-08-01 11:33:25.000000 mypy-boto3-sns-1.28.16/mypy_boto3_sns/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33161 2023-08-01 11:33:25.000000 mypy-boto3-sns-1.28.16/mypy_boto3_sns/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9936 2023-08-01 11:33:30.000000 mypy-boto3-sns-1.28.16/mypy_boto3_sns/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9934 2023-08-01 11:33:30.000000 mypy-boto3-sns-1.28.16/mypy_boto3_sns/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9594 2023-08-01 11:33:29.000000 mypy-boto3-sns-1.28.16/mypy_boto3_sns/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9584 2023-08-01 11:33:29.000000 mypy-boto3-sns-1.28.16/mypy_boto3_sns/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:33:25.000000 mypy-boto3-sns-1.28.16/mypy_boto3_sns/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    33864 2023-08-01 11:33:29.000000 mypy-boto3-sns-1.28.16/mypy_boto3_sns/service_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33795 2023-08-01 11:33:25.000000 mypy-boto3-sns-1.28.16/mypy_boto3_sns/service_resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    34587 2023-08-01 11:33:31.000000 mypy-boto3-sns-1.28.16/mypy_boto3_sns/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34540 2023-08-01 11:33:30.000000 mypy-boto3-sns-1.28.16/mypy_boto3_sns/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:33:25.000000 mypy-boto3-sns-1.28.16/mypy_boto3_sns/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:54.964721 mypy-boto3-sns-1.28.16/mypy_boto3_sns.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20745 2023-08-01 11:37:54.000000 mypy-boto3-sns-1.28.16/mypy_boto3_sns.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-08-01 11:37:54.000000 mypy-boto3-sns-1.28.16/mypy_boto3_sns.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:54.000000 mypy-boto3-sns-1.28.16/mypy_boto3_sns.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:54.000000 mypy-boto3-sns-1.28.16/mypy_boto3_sns.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:54.000000 mypy-boto3-sns-1.28.16/mypy_boto3_sns.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-01 11:37:54.000000 mypy-boto3-sns-1.28.16/mypy_boto3_sns.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:54.968721 mypy-boto3-sns-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-08-01 11:33:24.000000 mypy-boto3-sns-1.28.16/setup.py
```

### Comparing `mypy-boto3-sns-1.28.15.post1/LICENSE` & `mypy-boto3-sns-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sns-1.28.15.post1/PKG-INFO` & `mypy-boto3-sns-1.28.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sns
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.SNS 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.SNS 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 sns type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 sns type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sns.svg?color=blue)](https://pypi.org/project/mypy-boto3-sns)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sns)](https://pepy.tech/project/mypy-boto3-sns)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SNS 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS)
+[boto3.SNS 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS)
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
 [mypy-boto3-sns docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/).
 
 See how it helps to find and fix potential bugs:
 
@@ -77,15 +77,15 @@
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Service Resource annotations](#service-resource-annotations)
     - [Other resources annotations](#other-resources-annotations)
     - [Collections annotations](#collections-annotations)
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
@@ -424,26 +424,27 @@
 )
 
 
 def check_value(value: LanguageCodeStringType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_sns.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_sns.type_defs import (
     AddPermissionInputRequestTypeDef,
     AddPermissionInputTopicAddPermissionTypeDef,
     BatchResultErrorEntryTypeDef,
+    BlobTypeDef,
     CheckIfPhoneNumberIsOptedOutInputRequestTypeDef,
     ResponseMetadataTypeDef,
     ConfirmSubscriptionInputRequestTypeDef,
     ConfirmSubscriptionInputTopicConfirmSubscriptionTypeDef,
     CreatePlatformApplicationInputRequestTypeDef,
     CreatePlatformApplicationInputServiceResourceCreatePlatformApplicationTypeDef,
     CreatePlatformEndpointInputPlatformApplicationCreatePlatformEndpointTypeDef,
@@ -472,15 +473,14 @@
     SMSSandboxPhoneNumberTypeDef,
     ListSubscriptionsByTopicInputRequestTypeDef,
     SubscriptionTypeDef,
     ListSubscriptionsInputRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTopicsInputRequestTypeDef,
     TopicTypeDef,
-    MessageAttributeValueTypeDef,
     OptInPhoneNumberInputRequestTypeDef,
     PublishBatchResultEntryTypeDef,
     PutDataProtectionPolicyInputRequestTypeDef,
     RemovePermissionInputRequestTypeDef,
     RemovePermissionInputTopicRemovePermissionTypeDef,
     SetEndpointAttributesInputPlatformEndpointSetAttributesTypeDef,
     SetEndpointAttributesInputRequestTypeDef,
@@ -492,14 +492,15 @@
     SetTopicAttributesInputRequestTypeDef,
     SetTopicAttributesInputTopicSetAttributesTypeDef,
     SubscribeInputRequestTypeDef,
     SubscribeInputTopicSubscribeTypeDef,
     UnsubscribeInputRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     VerifySMSSandboxPhoneNumberInputRequestTypeDef,
+    MessageAttributeValueTypeDef,
     CheckIfPhoneNumberIsOptedOutResponseTypeDef,
     ConfirmSubscriptionResponseTypeDef,
     CreateEndpointResponseTypeDef,
     CreatePlatformApplicationResponseTypeDef,
     CreateTopicResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetDataProtectionPolicyResponseTypeDef,
@@ -527,24 +528,24 @@
     ListTopicsInputListTopicsPaginateTypeDef,
     ListOriginationNumbersResultTypeDef,
     ListPlatformApplicationsResponseTypeDef,
     ListSMSSandboxPhoneNumbersResultTypeDef,
     ListSubscriptionsByTopicResponseTypeDef,
     ListSubscriptionsResponseTypeDef,
     ListTopicsResponseTypeDef,
+    PublishBatchResponseTypeDef,
     PublishBatchRequestEntryTypeDef,
     PublishInputPlatformEndpointPublishTypeDef,
     PublishInputRequestTypeDef,
     PublishInputTopicPublishTypeDef,
-    PublishBatchResponseTypeDef,
     PublishBatchInputRequestTypeDef,
 )
 
 
-def get_structure() -> AddPermissionInputRequestTypeDef:
+def get_value() -> AddPermissionInputRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-sns-1.28.15.post1/README.md` & `mypy-boto3-sns-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sns.svg?color=blue)](https://pypi.org/project/mypy-boto3-sns)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sns)](https://pepy.tech/project/mypy-boto3-sns)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SNS 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS)
+[boto3.SNS 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS)
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
 [mypy-boto3-sns docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/).
 
 See how it helps to find and fix potential bugs:
 
@@ -45,15 +45,15 @@
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Service Resource annotations](#service-resource-annotations)
     - [Other resources annotations](#other-resources-annotations)
     - [Collections annotations](#collections-annotations)
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
@@ -392,26 +392,27 @@
 )
 
 
 def check_value(value: LanguageCodeStringType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_sns.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_sns.type_defs import (
     AddPermissionInputRequestTypeDef,
     AddPermissionInputTopicAddPermissionTypeDef,
     BatchResultErrorEntryTypeDef,
+    BlobTypeDef,
     CheckIfPhoneNumberIsOptedOutInputRequestTypeDef,
     ResponseMetadataTypeDef,
     ConfirmSubscriptionInputRequestTypeDef,
     ConfirmSubscriptionInputTopicConfirmSubscriptionTypeDef,
     CreatePlatformApplicationInputRequestTypeDef,
     CreatePlatformApplicationInputServiceResourceCreatePlatformApplicationTypeDef,
     CreatePlatformEndpointInputPlatformApplicationCreatePlatformEndpointTypeDef,
@@ -440,15 +441,14 @@
     SMSSandboxPhoneNumberTypeDef,
     ListSubscriptionsByTopicInputRequestTypeDef,
     SubscriptionTypeDef,
     ListSubscriptionsInputRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTopicsInputRequestTypeDef,
     TopicTypeDef,
-    MessageAttributeValueTypeDef,
     OptInPhoneNumberInputRequestTypeDef,
     PublishBatchResultEntryTypeDef,
     PutDataProtectionPolicyInputRequestTypeDef,
     RemovePermissionInputRequestTypeDef,
     RemovePermissionInputTopicRemovePermissionTypeDef,
     SetEndpointAttributesInputPlatformEndpointSetAttributesTypeDef,
     SetEndpointAttributesInputRequestTypeDef,
@@ -460,14 +460,15 @@
     SetTopicAttributesInputRequestTypeDef,
     SetTopicAttributesInputTopicSetAttributesTypeDef,
     SubscribeInputRequestTypeDef,
     SubscribeInputTopicSubscribeTypeDef,
     UnsubscribeInputRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     VerifySMSSandboxPhoneNumberInputRequestTypeDef,
+    MessageAttributeValueTypeDef,
     CheckIfPhoneNumberIsOptedOutResponseTypeDef,
     ConfirmSubscriptionResponseTypeDef,
     CreateEndpointResponseTypeDef,
     CreatePlatformApplicationResponseTypeDef,
     CreateTopicResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetDataProtectionPolicyResponseTypeDef,
@@ -495,24 +496,24 @@
     ListTopicsInputListTopicsPaginateTypeDef,
     ListOriginationNumbersResultTypeDef,
     ListPlatformApplicationsResponseTypeDef,
     ListSMSSandboxPhoneNumbersResultTypeDef,
     ListSubscriptionsByTopicResponseTypeDef,
     ListSubscriptionsResponseTypeDef,
     ListTopicsResponseTypeDef,
+    PublishBatchResponseTypeDef,
     PublishBatchRequestEntryTypeDef,
     PublishInputPlatformEndpointPublishTypeDef,
     PublishInputRequestTypeDef,
     PublishInputTopicPublishTypeDef,
-    PublishBatchResponseTypeDef,
     PublishBatchInputRequestTypeDef,
 )
 
 
-def get_structure() -> AddPermissionInputRequestTypeDef:
+def get_value() -> AddPermissionInputRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-sns-1.28.15.post1/mypy_boto3_sns/__init__.py` & `mypy-boto3-sns-1.28.16/mypy_boto3_sns/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sns-1.28.15.post1/mypy_boto3_sns/__init__.pyi` & `mypy-boto3-sns-1.28.16/mypy_boto3_sns/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sns-1.28.15.post1/mypy_boto3_sns/__main__.py` & `mypy-boto3-sns-1.28.16/mypy_boto3_sns/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SNS 1.28.15\nVersion:         1.28.15.post1\nBuilder version:"
-        " 7.16.2\nDocs:           "
+        "Type annotations for boto3.SNS 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS\nOther"
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

### Comparing `mypy-boto3-sns-1.28.15.post1/mypy_boto3_sns/client.py` & `mypy-boto3-sns-1.28.16/mypy_boto3_sns/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sns-1.28.15.post1/mypy_boto3_sns/client.pyi` & `mypy-boto3-sns-1.28.16/mypy_boto3_sns/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sns-1.28.15.post1/mypy_boto3_sns/literals.py` & `mypy-boto3-sns-1.28.16/mypy_boto3_sns/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sns-1.28.15.post1/mypy_boto3_sns/literals.pyi` & `mypy-boto3-sns-1.28.16/mypy_boto3_sns/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sns-1.28.15.post1/mypy_boto3_sns/paginator.py` & `mypy-boto3-sns-1.28.16/mypy_boto3_sns/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sns-1.28.15.post1/mypy_boto3_sns/paginator.pyi` & `mypy-boto3-sns-1.28.16/mypy_boto3_sns/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sns-1.28.15.post1/mypy_boto3_sns/service_resource.py` & `mypy-boto3-sns-1.28.16/mypy_boto3_sns/service_resource.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sns-1.28.15.post1/mypy_boto3_sns/service_resource.pyi` & `mypy-boto3-sns-1.28.16/mypy_boto3_sns/service_resource.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sns-1.28.15.post1/mypy_boto3_sns/type_defs.py` & `mypy-boto3-sns-1.28.16/mypy_boto3_sns/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_sns.type_defs import AddPermissionInputRequestTypeDef
 
-    data: AddPermissionInputRequestTypeDef = {...}
+    data: AddPermissionInputRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -30,14 +30,15 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AddPermissionInputRequestTypeDef",
     "AddPermissionInputTopicAddPermissionTypeDef",
     "BatchResultErrorEntryTypeDef",
+    "BlobTypeDef",
     "CheckIfPhoneNumberIsOptedOutInputRequestTypeDef",
     "ResponseMetadataTypeDef",
     "ConfirmSubscriptionInputRequestTypeDef",
     "ConfirmSubscriptionInputTopicConfirmSubscriptionTypeDef",
     "CreatePlatformApplicationInputRequestTypeDef",
     "CreatePlatformApplicationInputServiceResourceCreatePlatformApplicationTypeDef",
     "CreatePlatformEndpointInputPlatformApplicationCreatePlatformEndpointTypeDef",
@@ -66,15 +67,14 @@
     "SMSSandboxPhoneNumberTypeDef",
     "ListSubscriptionsByTopicInputRequestTypeDef",
     "SubscriptionTypeDef",
     "ListSubscriptionsInputRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListTopicsInputRequestTypeDef",
     "TopicTypeDef",
-    "MessageAttributeValueTypeDef",
     "OptInPhoneNumberInputRequestTypeDef",
     "PublishBatchResultEntryTypeDef",
     "PutDataProtectionPolicyInputRequestTypeDef",
     "RemovePermissionInputRequestTypeDef",
     "RemovePermissionInputTopicRemovePermissionTypeDef",
     "SetEndpointAttributesInputPlatformEndpointSetAttributesTypeDef",
     "SetEndpointAttributesInputRequestTypeDef",
@@ -86,14 +86,15 @@
     "SetTopicAttributesInputRequestTypeDef",
     "SetTopicAttributesInputTopicSetAttributesTypeDef",
     "SubscribeInputRequestTypeDef",
     "SubscribeInputTopicSubscribeTypeDef",
     "UnsubscribeInputRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "VerifySMSSandboxPhoneNumberInputRequestTypeDef",
+    "MessageAttributeValueTypeDef",
     "CheckIfPhoneNumberIsOptedOutResponseTypeDef",
     "ConfirmSubscriptionResponseTypeDef",
     "CreateEndpointResponseTypeDef",
     "CreatePlatformApplicationResponseTypeDef",
     "CreateTopicResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetDataProtectionPolicyResponseTypeDef",
@@ -121,19 +122,19 @@
     "ListTopicsInputListTopicsPaginateTypeDef",
     "ListOriginationNumbersResultTypeDef",
     "ListPlatformApplicationsResponseTypeDef",
     "ListSMSSandboxPhoneNumbersResultTypeDef",
     "ListSubscriptionsByTopicResponseTypeDef",
     "ListSubscriptionsResponseTypeDef",
     "ListTopicsResponseTypeDef",
+    "PublishBatchResponseTypeDef",
     "PublishBatchRequestEntryTypeDef",
     "PublishInputPlatformEndpointPublishTypeDef",
     "PublishInputRequestTypeDef",
     "PublishInputTopicPublishTypeDef",
-    "PublishBatchResponseTypeDef",
     "PublishBatchInputRequestTypeDef",
 )
 
 AddPermissionInputRequestTypeDef = TypedDict(
     "AddPermissionInputRequestTypeDef",
     {
         "TopicArn": str,
@@ -171,14 +172,15 @@
 
 class BatchResultErrorEntryTypeDef(
     _RequiredBatchResultErrorEntryTypeDef, _OptionalBatchResultErrorEntryTypeDef
 ):
     pass
 
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 CheckIfPhoneNumberIsOptedOutInputRequestTypeDef = TypedDict(
     "CheckIfPhoneNumberIsOptedOutInputRequestTypeDef",
     {
         "phoneNumber": str,
     },
 )
 
@@ -570,36 +572,14 @@
     "TopicTypeDef",
     {
         "TopicArn": str,
     },
     total=False,
 )
 
-_RequiredMessageAttributeValueTypeDef = TypedDict(
-    "_RequiredMessageAttributeValueTypeDef",
-    {
-        "DataType": str,
-    },
-)
-_OptionalMessageAttributeValueTypeDef = TypedDict(
-    "_OptionalMessageAttributeValueTypeDef",
-    {
-        "StringValue": str,
-        "BinaryValue": Union[str, bytes, IO[Any], StreamingBody],
-    },
-    total=False,
-)
-
-
-class MessageAttributeValueTypeDef(
-    _RequiredMessageAttributeValueTypeDef, _OptionalMessageAttributeValueTypeDef
-):
-    pass
-
-
 OptInPhoneNumberInputRequestTypeDef = TypedDict(
     "OptInPhoneNumberInputRequestTypeDef",
     {
         "phoneNumber": str,
     },
 )
 
@@ -828,14 +808,36 @@
     "VerifySMSSandboxPhoneNumberInputRequestTypeDef",
     {
         "PhoneNumber": str,
         "OneTimePassword": str,
     },
 )
 
+_RequiredMessageAttributeValueTypeDef = TypedDict(
+    "_RequiredMessageAttributeValueTypeDef",
+    {
+        "DataType": str,
+    },
+)
+_OptionalMessageAttributeValueTypeDef = TypedDict(
+    "_OptionalMessageAttributeValueTypeDef",
+    {
+        "StringValue": str,
+        "BinaryValue": BlobTypeDef,
+    },
+    total=False,
+)
+
+
+class MessageAttributeValueTypeDef(
+    _RequiredMessageAttributeValueTypeDef, _OptionalMessageAttributeValueTypeDef
+):
+    pass
+
+
 CheckIfPhoneNumberIsOptedOutResponseTypeDef = TypedDict(
     "CheckIfPhoneNumberIsOptedOutResponseTypeDef",
     {
         "isOptedOut": bool,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1175,14 +1177,23 @@
     {
         "Topics": List[TopicTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+PublishBatchResponseTypeDef = TypedDict(
+    "PublishBatchResponseTypeDef",
+    {
+        "Successful": List[PublishBatchResultEntryTypeDef],
+        "Failed": List[BatchResultErrorEntryTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredPublishBatchRequestEntryTypeDef = TypedDict(
     "_RequiredPublishBatchRequestEntryTypeDef",
     {
         "Id": str,
         "Message": str,
     },
 )
@@ -1284,23 +1295,14 @@
 
 class PublishInputTopicPublishTypeDef(
     _RequiredPublishInputTopicPublishTypeDef, _OptionalPublishInputTopicPublishTypeDef
 ):
     pass
 
 
-PublishBatchResponseTypeDef = TypedDict(
-    "PublishBatchResponseTypeDef",
-    {
-        "Successful": List[PublishBatchResultEntryTypeDef],
-        "Failed": List[BatchResultErrorEntryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 PublishBatchInputRequestTypeDef = TypedDict(
     "PublishBatchInputRequestTypeDef",
     {
         "TopicArn": str,
         "PublishBatchRequestEntries": Sequence[PublishBatchRequestEntryTypeDef],
     },
 )
```

### Comparing `mypy-boto3-sns-1.28.15.post1/mypy_boto3_sns/type_defs.pyi` & `mypy-boto3-sns-1.28.16/mypy_boto3_sns/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_sns.type_defs import AddPermissionInputRequestTypeDef
 
-    data: AddPermissionInputRequestTypeDef = {...}
+    data: AddPermissionInputRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -29,14 +29,15 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AddPermissionInputRequestTypeDef",
     "AddPermissionInputTopicAddPermissionTypeDef",
     "BatchResultErrorEntryTypeDef",
+    "BlobTypeDef",
     "CheckIfPhoneNumberIsOptedOutInputRequestTypeDef",
     "ResponseMetadataTypeDef",
     "ConfirmSubscriptionInputRequestTypeDef",
     "ConfirmSubscriptionInputTopicConfirmSubscriptionTypeDef",
     "CreatePlatformApplicationInputRequestTypeDef",
     "CreatePlatformApplicationInputServiceResourceCreatePlatformApplicationTypeDef",
     "CreatePlatformEndpointInputPlatformApplicationCreatePlatformEndpointTypeDef",
@@ -65,15 +66,14 @@
     "SMSSandboxPhoneNumberTypeDef",
     "ListSubscriptionsByTopicInputRequestTypeDef",
     "SubscriptionTypeDef",
     "ListSubscriptionsInputRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListTopicsInputRequestTypeDef",
     "TopicTypeDef",
-    "MessageAttributeValueTypeDef",
     "OptInPhoneNumberInputRequestTypeDef",
     "PublishBatchResultEntryTypeDef",
     "PutDataProtectionPolicyInputRequestTypeDef",
     "RemovePermissionInputRequestTypeDef",
     "RemovePermissionInputTopicRemovePermissionTypeDef",
     "SetEndpointAttributesInputPlatformEndpointSetAttributesTypeDef",
     "SetEndpointAttributesInputRequestTypeDef",
@@ -85,14 +85,15 @@
     "SetTopicAttributesInputRequestTypeDef",
     "SetTopicAttributesInputTopicSetAttributesTypeDef",
     "SubscribeInputRequestTypeDef",
     "SubscribeInputTopicSubscribeTypeDef",
     "UnsubscribeInputRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "VerifySMSSandboxPhoneNumberInputRequestTypeDef",
+    "MessageAttributeValueTypeDef",
     "CheckIfPhoneNumberIsOptedOutResponseTypeDef",
     "ConfirmSubscriptionResponseTypeDef",
     "CreateEndpointResponseTypeDef",
     "CreatePlatformApplicationResponseTypeDef",
     "CreateTopicResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetDataProtectionPolicyResponseTypeDef",
@@ -120,19 +121,19 @@
     "ListTopicsInputListTopicsPaginateTypeDef",
     "ListOriginationNumbersResultTypeDef",
     "ListPlatformApplicationsResponseTypeDef",
     "ListSMSSandboxPhoneNumbersResultTypeDef",
     "ListSubscriptionsByTopicResponseTypeDef",
     "ListSubscriptionsResponseTypeDef",
     "ListTopicsResponseTypeDef",
+    "PublishBatchResponseTypeDef",
     "PublishBatchRequestEntryTypeDef",
     "PublishInputPlatformEndpointPublishTypeDef",
     "PublishInputRequestTypeDef",
     "PublishInputTopicPublishTypeDef",
-    "PublishBatchResponseTypeDef",
     "PublishBatchInputRequestTypeDef",
 )
 
 AddPermissionInputRequestTypeDef = TypedDict(
     "AddPermissionInputRequestTypeDef",
     {
         "TopicArn": str,
@@ -168,14 +169,15 @@
 )
 
 class BatchResultErrorEntryTypeDef(
     _RequiredBatchResultErrorEntryTypeDef, _OptionalBatchResultErrorEntryTypeDef
 ):
     pass
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 CheckIfPhoneNumberIsOptedOutInputRequestTypeDef = TypedDict(
     "CheckIfPhoneNumberIsOptedOutInputRequestTypeDef",
     {
         "phoneNumber": str,
     },
 )
 
@@ -553,34 +555,14 @@
     "TopicTypeDef",
     {
         "TopicArn": str,
     },
     total=False,
 )
 
-_RequiredMessageAttributeValueTypeDef = TypedDict(
-    "_RequiredMessageAttributeValueTypeDef",
-    {
-        "DataType": str,
-    },
-)
-_OptionalMessageAttributeValueTypeDef = TypedDict(
-    "_OptionalMessageAttributeValueTypeDef",
-    {
-        "StringValue": str,
-        "BinaryValue": Union[str, bytes, IO[Any], StreamingBody],
-    },
-    total=False,
-)
-
-class MessageAttributeValueTypeDef(
-    _RequiredMessageAttributeValueTypeDef, _OptionalMessageAttributeValueTypeDef
-):
-    pass
-
 OptInPhoneNumberInputRequestTypeDef = TypedDict(
     "OptInPhoneNumberInputRequestTypeDef",
     {
         "phoneNumber": str,
     },
 )
 
@@ -797,14 +779,34 @@
     "VerifySMSSandboxPhoneNumberInputRequestTypeDef",
     {
         "PhoneNumber": str,
         "OneTimePassword": str,
     },
 )
 
+_RequiredMessageAttributeValueTypeDef = TypedDict(
+    "_RequiredMessageAttributeValueTypeDef",
+    {
+        "DataType": str,
+    },
+)
+_OptionalMessageAttributeValueTypeDef = TypedDict(
+    "_OptionalMessageAttributeValueTypeDef",
+    {
+        "StringValue": str,
+        "BinaryValue": BlobTypeDef,
+    },
+    total=False,
+)
+
+class MessageAttributeValueTypeDef(
+    _RequiredMessageAttributeValueTypeDef, _OptionalMessageAttributeValueTypeDef
+):
+    pass
+
 CheckIfPhoneNumberIsOptedOutResponseTypeDef = TypedDict(
     "CheckIfPhoneNumberIsOptedOutResponseTypeDef",
     {
         "isOptedOut": bool,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1136,14 +1138,23 @@
     {
         "Topics": List[TopicTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+PublishBatchResponseTypeDef = TypedDict(
+    "PublishBatchResponseTypeDef",
+    {
+        "Successful": List[PublishBatchResultEntryTypeDef],
+        "Failed": List[BatchResultErrorEntryTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredPublishBatchRequestEntryTypeDef = TypedDict(
     "_RequiredPublishBatchRequestEntryTypeDef",
     {
         "Id": str,
         "Message": str,
     },
 )
@@ -1237,23 +1248,14 @@
 )
 
 class PublishInputTopicPublishTypeDef(
     _RequiredPublishInputTopicPublishTypeDef, _OptionalPublishInputTopicPublishTypeDef
 ):
     pass
 
-PublishBatchResponseTypeDef = TypedDict(
-    "PublishBatchResponseTypeDef",
-    {
-        "Successful": List[PublishBatchResultEntryTypeDef],
-        "Failed": List[BatchResultErrorEntryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 PublishBatchInputRequestTypeDef = TypedDict(
     "PublishBatchInputRequestTypeDef",
     {
         "TopicArn": str,
         "PublishBatchRequestEntries": Sequence[PublishBatchRequestEntryTypeDef],
     },
 )
```

### Comparing `mypy-boto3-sns-1.28.15.post1/mypy_boto3_sns.egg-info/PKG-INFO` & `mypy-boto3-sns-1.28.16/mypy_boto3_sns.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sns
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.SNS 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.SNS 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 sns type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 sns type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sns.svg?color=blue)](https://pypi.org/project/mypy-boto3-sns)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sns)](https://pepy.tech/project/mypy-boto3-sns)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SNS 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS)
+[boto3.SNS 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS)
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
 [mypy-boto3-sns docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/).
 
 See how it helps to find and fix potential bugs:
 
@@ -77,15 +77,15 @@
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Service Resource annotations](#service-resource-annotations)
     - [Other resources annotations](#other-resources-annotations)
     - [Collections annotations](#collections-annotations)
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
@@ -424,26 +424,27 @@
 )
 
 
 def check_value(value: LanguageCodeStringType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_sns.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_sns.type_defs import (
     AddPermissionInputRequestTypeDef,
     AddPermissionInputTopicAddPermissionTypeDef,
     BatchResultErrorEntryTypeDef,
+    BlobTypeDef,
     CheckIfPhoneNumberIsOptedOutInputRequestTypeDef,
     ResponseMetadataTypeDef,
     ConfirmSubscriptionInputRequestTypeDef,
     ConfirmSubscriptionInputTopicConfirmSubscriptionTypeDef,
     CreatePlatformApplicationInputRequestTypeDef,
     CreatePlatformApplicationInputServiceResourceCreatePlatformApplicationTypeDef,
     CreatePlatformEndpointInputPlatformApplicationCreatePlatformEndpointTypeDef,
@@ -472,15 +473,14 @@
     SMSSandboxPhoneNumberTypeDef,
     ListSubscriptionsByTopicInputRequestTypeDef,
     SubscriptionTypeDef,
     ListSubscriptionsInputRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTopicsInputRequestTypeDef,
     TopicTypeDef,
-    MessageAttributeValueTypeDef,
     OptInPhoneNumberInputRequestTypeDef,
     PublishBatchResultEntryTypeDef,
     PutDataProtectionPolicyInputRequestTypeDef,
     RemovePermissionInputRequestTypeDef,
     RemovePermissionInputTopicRemovePermissionTypeDef,
     SetEndpointAttributesInputPlatformEndpointSetAttributesTypeDef,
     SetEndpointAttributesInputRequestTypeDef,
@@ -492,14 +492,15 @@
     SetTopicAttributesInputRequestTypeDef,
     SetTopicAttributesInputTopicSetAttributesTypeDef,
     SubscribeInputRequestTypeDef,
     SubscribeInputTopicSubscribeTypeDef,
     UnsubscribeInputRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     VerifySMSSandboxPhoneNumberInputRequestTypeDef,
+    MessageAttributeValueTypeDef,
     CheckIfPhoneNumberIsOptedOutResponseTypeDef,
     ConfirmSubscriptionResponseTypeDef,
     CreateEndpointResponseTypeDef,
     CreatePlatformApplicationResponseTypeDef,
     CreateTopicResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetDataProtectionPolicyResponseTypeDef,
@@ -527,24 +528,24 @@
     ListTopicsInputListTopicsPaginateTypeDef,
     ListOriginationNumbersResultTypeDef,
     ListPlatformApplicationsResponseTypeDef,
     ListSMSSandboxPhoneNumbersResultTypeDef,
     ListSubscriptionsByTopicResponseTypeDef,
     ListSubscriptionsResponseTypeDef,
     ListTopicsResponseTypeDef,
+    PublishBatchResponseTypeDef,
     PublishBatchRequestEntryTypeDef,
     PublishInputPlatformEndpointPublishTypeDef,
     PublishInputRequestTypeDef,
     PublishInputTopicPublishTypeDef,
-    PublishBatchResponseTypeDef,
     PublishBatchInputRequestTypeDef,
 )
 
 
-def get_structure() -> AddPermissionInputRequestTypeDef:
+def get_value() -> AddPermissionInputRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-sns-1.28.15.post1/mypy_boto3_sns.egg-info/SOURCES.txt` & `mypy-boto3-sns-1.28.16/mypy_boto3_sns.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sns-1.28.15.post1/setup.py` & `mypy-boto3-sns-1.28.16/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-sns",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_sns"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.SNS 1.28.15 service generated with mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.SNS 1.28.16 service generated with mypy-boto3-builder 7.17.1"
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
-    keywords="boto3 sns type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 sns type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_sns": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

