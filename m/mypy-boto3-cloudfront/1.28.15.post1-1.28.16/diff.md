# Comparing `tmp/mypy-boto3-cloudfront-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-cloudfront-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-cloudfront-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:41 2023, max compression
+gzip compressed data, was "mypy-boto3-cloudfront-1.28.16.tar", last modified: Tue Aug  1 11:36:22 2023, max compression
```

## Comparing `mypy-boto3-cloudfront-1.28.15.post1.tar` & `mypy-boto3-cloudfront-1.28.16.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:41.625051 mypy-boto3-cloudfront-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:40:00.000000 mypy-boto3-cloudfront-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    33224 2023-07-29 10:02:41.621050 mypy-boto3-cloudfront-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    31719 2023-07-29 09:40:00.000000 mypy-boto3-cloudfront-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:41.617051 mypy-boto3-cloudfront-1.28.15.post1/mypy_boto3_cloudfront/
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-07-29 09:40:00.000000 mypy-boto3-cloudfront-1.28.15.post1/mypy_boto3_cloudfront/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-07-29 09:40:00.000000 mypy-boto3-cloudfront-1.28.15.post1/mypy_boto3_cloudfront/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-29 09:40:00.000000 mypy-boto3-cloudfront-1.28.15.post1/mypy_boto3_cloudfront/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    81323 2023-07-29 09:40:02.000000 mypy-boto3-cloudfront-1.28.15.post1/mypy_boto3_cloudfront/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    81203 2023-07-29 09:40:01.000000 mypy-boto3-cloudfront-1.28.15.post1/mypy_boto3_cloudfront/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12568 2023-07-29 09:40:02.000000 mypy-boto3-cloudfront-1.28.15.post1/mypy_boto3_cloudfront/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-07-29 09:40:02.000000 mypy-boto3-cloudfront-1.28.15.post1/mypy_boto3_cloudfront/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-07-29 09:40:02.000000 mypy-boto3-cloudfront-1.28.15.post1/mypy_boto3_cloudfront/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5454 2023-07-29 09:40:02.000000 mypy-boto3-cloudfront-1.28.15.post1/mypy_boto3_cloudfront/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:40:00.000000 mypy-boto3-cloudfront-1.28.15.post1/mypy_boto3_cloudfront/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   172819 2023-07-29 09:40:07.000000 mypy-boto3-cloudfront-1.28.15.post1/mypy_boto3_cloudfront/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   172458 2023-07-29 09:40:04.000000 mypy-boto3-cloudfront-1.28.15.post1/mypy_boto3_cloudfront/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:40:00.000000 mypy-boto3-cloudfront-1.28.15.post1/mypy_boto3_cloudfront/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-07-29 09:40:02.000000 mypy-boto3-cloudfront-1.28.15.post1/mypy_boto3_cloudfront/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-07-29 09:40:02.000000 mypy-boto3-cloudfront-1.28.15.post1/mypy_boto3_cloudfront/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:41.621050 mypy-boto3-cloudfront-1.28.15.post1/mypy_boto3_cloudfront.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    33224 2023-07-29 10:02:41.000000 mypy-boto3-cloudfront-1.28.15.post1/mypy_boto3_cloudfront.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-29 10:02:41.000000 mypy-boto3-cloudfront-1.28.15.post1/mypy_boto3_cloudfront.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:41.000000 mypy-boto3-cloudfront-1.28.15.post1/mypy_boto3_cloudfront.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:41.000000 mypy-boto3-cloudfront-1.28.15.post1/mypy_boto3_cloudfront.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:41.000000 mypy-boto3-cloudfront-1.28.15.post1/mypy_boto3_cloudfront.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-29 10:02:41.000000 mypy-boto3-cloudfront-1.28.15.post1/mypy_boto3_cloudfront.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:41.625051 mypy-boto3-cloudfront-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-07-29 09:40:00.000000 mypy-boto3-cloudfront-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:22.240934 mypy-boto3-cloudfront-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:12:34.000000 mypy-boto3-cloudfront-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    33669 2023-08-01 11:36:22.224934 mypy-boto3-cloudfront-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    32173 2023-08-01 11:12:34.000000 mypy-boto3-cloudfront-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:22.220934 mypy-boto3-cloudfront-1.28.16/mypy_boto3_cloudfront/
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-08-01 11:12:34.000000 mypy-boto3-cloudfront-1.28.16/mypy_boto3_cloudfront/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-08-01 11:12:34.000000 mypy-boto3-cloudfront-1.28.16/mypy_boto3_cloudfront/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-08-01 11:12:34.000000 mypy-boto3-cloudfront-1.28.16/mypy_boto3_cloudfront/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79434 2023-08-01 11:12:34.000000 mypy-boto3-cloudfront-1.28.16/mypy_boto3_cloudfront/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79314 2023-08-01 11:12:34.000000 mypy-boto3-cloudfront-1.28.16/mypy_boto3_cloudfront/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12568 2023-08-01 11:12:35.000000 mypy-boto3-cloudfront-1.28.16/mypy_boto3_cloudfront/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-08-01 11:12:35.000000 mypy-boto3-cloudfront-1.28.16/mypy_boto3_cloudfront/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-08-01 11:12:34.000000 mypy-boto3-cloudfront-1.28.16/mypy_boto3_cloudfront/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5454 2023-08-01 11:12:34.000000 mypy-boto3-cloudfront-1.28.16/mypy_boto3_cloudfront/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:12:34.000000 mypy-boto3-cloudfront-1.28.16/mypy_boto3_cloudfront/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   174513 2023-08-01 11:12:40.000000 mypy-boto3-cloudfront-1.28.16/mypy_boto3_cloudfront/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   174152 2023-08-01 11:12:38.000000 mypy-boto3-cloudfront-1.28.16/mypy_boto3_cloudfront/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:12:34.000000 mypy-boto3-cloudfront-1.28.16/mypy_boto3_cloudfront/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-08-01 11:12:34.000000 mypy-boto3-cloudfront-1.28.16/mypy_boto3_cloudfront/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-08-01 11:12:34.000000 mypy-boto3-cloudfront-1.28.16/mypy_boto3_cloudfront/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:22.224934 mypy-boto3-cloudfront-1.28.16/mypy_boto3_cloudfront.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    33669 2023-08-01 11:36:21.000000 mypy-boto3-cloudfront-1.28.16/mypy_boto3_cloudfront.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-01 11:36:22.000000 mypy-boto3-cloudfront-1.28.16/mypy_boto3_cloudfront.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:21.000000 mypy-boto3-cloudfront-1.28.16/mypy_boto3_cloudfront.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:21.000000 mypy-boto3-cloudfront-1.28.16/mypy_boto3_cloudfront.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:21.000000 mypy-boto3-cloudfront-1.28.16/mypy_boto3_cloudfront.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-01 11:36:21.000000 mypy-boto3-cloudfront-1.28.16/mypy_boto3_cloudfront.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:22.240934 mypy-boto3-cloudfront-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-08-01 11:12:34.000000 mypy-boto3-cloudfront-1.28.16/setup.py
```

### Comparing `mypy-boto3-cloudfront-1.28.15.post1/LICENSE` & `mypy-boto3-cloudfront-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudfront-1.28.15.post1/PKG-INFO` & `mypy-boto3-cloudfront-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cloudfront
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.CloudFront 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.CloudFront 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 cloudfront type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 cloudfront type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudfront.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudfront)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cloudfront)](https://pepy.tech/project/mypy-boto3-cloudfront)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudFront 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront)
+[boto3.CloudFront 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront)
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
 [mypy-boto3-cloudfront docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/).
 
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
@@ -397,29 +397,30 @@
 )
 
 
 def check_value(value: CachePolicyCookieBehaviorType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_cloudfront.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_cloudfront.type_defs import (
     AliasICPRecordalTypeDef,
     AliasesOutputTypeDef,
     AliasesTypeDef,
     CachedMethodsOutputTypeDef,
     CachedMethodsTypeDef,
     AssociateAliasRequestRequestTypeDef,
+    BlobTypeDef,
     TrustedKeyGroupsOutputTypeDef,
     TrustedSignersOutputTypeDef,
     TrustedKeyGroupsTypeDef,
     TrustedSignersTypeDef,
     CookieNamesOutputTypeDef,
     CookieNamesTypeDef,
     HeadersOutputTypeDef,
@@ -558,18 +559,18 @@
     ResponseHeadersPolicyRemoveHeaderTypeDef,
     ResponseHeadersPolicyStrictTransportSecurityTypeDef,
     ResponseHeadersPolicyXSSProtectionTypeDef,
     S3OriginTypeDef,
     StreamingLoggingConfigTypeDef,
     TagKeysTypeDef,
     TagTypeDef,
-    TestFunctionRequestRequestTypeDef,
     UpdateDistributionWithStagingConfigRequestRequestTypeDef,
     AllowedMethodsOutputTypeDef,
     AllowedMethodsTypeDef,
+    TestFunctionRequestRequestTypeDef,
     CachePolicyCookiesConfigOutputTypeDef,
     CookiePreferenceOutputTypeDef,
     OriginRequestPolicyCookiesConfigOutputTypeDef,
     CachePolicyCookiesConfigTypeDef,
     CookiePreferenceTypeDef,
     OriginRequestPolicyCookiesConfigTypeDef,
     CachePolicyHeadersConfigOutputTypeDef,
@@ -621,14 +622,15 @@
     FunctionSummaryTypeDef,
     RestrictionsOutputTypeDef,
     RestrictionsTypeDef,
     GetDistributionRequestDistributionDeployedWaitTypeDef,
     GetInvalidationRequestInvalidationCompletedWaitTypeDef,
     GetStreamingDistributionRequestStreamingDistributionDeployedWaitTypeDef,
     GetKeyGroupConfigResultTypeDef,
+    KeyGroupConfigUnionTypeDef,
     KeyGroupTypeDef,
     InvalidationBatchOutputTypeDef,
     InvalidationBatchTypeDef,
     InvalidationListTypeDef,
     KGKeyPairIdsTypeDef,
     SignerTypeDef,
     LambdaFunctionAssociationsOutputTypeDef,
@@ -694,14 +696,15 @@
     UpdateFunctionResultTypeDef,
     CreateKeyGroupResultTypeDef,
     GetKeyGroupResultTypeDef,
     KeyGroupSummaryTypeDef,
     UpdateKeyGroupResultTypeDef,
     InvalidationTypeDef,
     CreateInvalidationRequestRequestTypeDef,
+    InvalidationBatchUnionTypeDef,
     ListInvalidationsResultTypeDef,
     ActiveTrustedKeyGroupsTypeDef,
     ActiveTrustedSignersTypeDef,
     CreateMonitoringSubscriptionRequestRequestTypeDef,
     CreateMonitoringSubscriptionResultTypeDef,
     GetMonitoringSubscriptionResultTypeDef,
     ListOriginAccessControlsResultTypeDef,
@@ -711,27 +714,30 @@
     QueryArgProfileConfigOutputTypeDef,
     QueryArgProfileConfigTypeDef,
     ResponseHeadersPolicyConfigOutputTypeDef,
     ResponseHeadersPolicyConfigTypeDef,
     StreamingDistributionListTypeDef,
     GetStreamingDistributionConfigResultTypeDef,
     CreateStreamingDistributionRequestRequestTypeDef,
+    StreamingDistributionConfigUnionTypeDef,
     UpdateStreamingDistributionRequestRequestTypeDef,
     ListTagsForResourceResultTypeDef,
     StreamingDistributionConfigWithTagsTypeDef,
     TagResourceRequestRequestTypeDef,
+    TagsUnionTypeDef,
     CacheBehaviorOutputTypeDef,
     DefaultCacheBehaviorOutputTypeDef,
     CacheBehaviorTypeDef,
     DefaultCacheBehaviorTypeDef,
     CachePolicyConfigOutputTypeDef,
     GetOriginRequestPolicyConfigResultTypeDef,
     OriginRequestPolicyTypeDef,
     CachePolicyConfigTypeDef,
     CreateOriginRequestPolicyRequestRequestTypeDef,
+    OriginRequestPolicyConfigUnionTypeDef,
     UpdateOriginRequestPolicyRequestRequestTypeDef,
     ContinuousDeploymentPolicyConfigOutputTypeDef,
     ContinuousDeploymentPolicyConfigTypeDef,
     OriginsOutputTypeDef,
     OriginsTypeDef,
     FieldLevelEncryptionProfileConfigOutputTypeDef,
     FieldLevelEncryptionProfileSummaryTypeDef,
@@ -750,46 +756,51 @@
     OriginGroupsTypeDef,
     FieldLevelEncryptionConfigOutputTypeDef,
     FieldLevelEncryptionSummaryTypeDef,
     FieldLevelEncryptionConfigTypeDef,
     GetResponseHeadersPolicyConfigResultTypeDef,
     ResponseHeadersPolicyTypeDef,
     CreateResponseHeadersPolicyRequestRequestTypeDef,
+    ResponseHeadersPolicyConfigUnionTypeDef,
     UpdateResponseHeadersPolicyRequestRequestTypeDef,
     ListStreamingDistributionsResultTypeDef,
     CreateStreamingDistributionWithTagsRequestRequestTypeDef,
     CacheBehaviorsOutputTypeDef,
     CacheBehaviorsTypeDef,
     CachePolicyTypeDef,
     GetCachePolicyConfigResultTypeDef,
     CreateOriginRequestPolicyResultTypeDef,
     GetOriginRequestPolicyResultTypeDef,
     OriginRequestPolicySummaryTypeDef,
     UpdateOriginRequestPolicyResultTypeDef,
+    CachePolicyConfigUnionTypeDef,
     CreateCachePolicyRequestRequestTypeDef,
     UpdateCachePolicyRequestRequestTypeDef,
     ContinuousDeploymentPolicyTypeDef,
     GetContinuousDeploymentPolicyConfigResultTypeDef,
+    ContinuousDeploymentPolicyConfigUnionTypeDef,
     CreateContinuousDeploymentPolicyRequestRequestTypeDef,
     UpdateContinuousDeploymentPolicyRequestRequestTypeDef,
     FieldLevelEncryptionProfileTypeDef,
     GetFieldLevelEncryptionProfileConfigResultTypeDef,
     FieldLevelEncryptionProfileListTypeDef,
     CreateFieldLevelEncryptionProfileRequestRequestTypeDef,
+    FieldLevelEncryptionProfileConfigUnionTypeDef,
     UpdateFieldLevelEncryptionProfileRequestRequestTypeDef,
     ListRealtimeLogConfigsResultTypeDef,
     ListKeyGroupsResultTypeDef,
     CreateStreamingDistributionResultTypeDef,
     CreateStreamingDistributionWithTagsResultTypeDef,
     GetStreamingDistributionResultTypeDef,
     UpdateStreamingDistributionResultTypeDef,
     FieldLevelEncryptionTypeDef,
     GetFieldLevelEncryptionConfigResultTypeDef,
     FieldLevelEncryptionListTypeDef,
     CreateFieldLevelEncryptionConfigRequestRequestTypeDef,
+    FieldLevelEncryptionConfigUnionTypeDef,
     UpdateFieldLevelEncryptionConfigRequestRequestTypeDef,
     CreateResponseHeadersPolicyResultTypeDef,
     GetResponseHeadersPolicyResultTypeDef,
     ResponseHeadersPolicySummaryTypeDef,
     UpdateResponseHeadersPolicyResultTypeDef,
     DistributionConfigOutputTypeDef,
     DistributionSummaryTypeDef,
@@ -812,14 +823,15 @@
     UpdateFieldLevelEncryptionConfigResultTypeDef,
     ListFieldLevelEncryptionConfigsResultTypeDef,
     ResponseHeadersPolicyListTypeDef,
     DistributionTypeDef,
     GetDistributionConfigResultTypeDef,
     DistributionListTypeDef,
     CreateDistributionRequestRequestTypeDef,
+    DistributionConfigUnionTypeDef,
     DistributionConfigWithTagsTypeDef,
     UpdateDistributionRequestRequestTypeDef,
     CachePolicyListTypeDef,
     ListOriginRequestPoliciesResultTypeDef,
     ContinuousDeploymentPolicyListTypeDef,
     ListResponseHeadersPoliciesResultTypeDef,
     CopyDistributionResultTypeDef,
@@ -833,15 +845,15 @@
     ListDistributionsResultTypeDef,
     CreateDistributionWithTagsRequestRequestTypeDef,
     ListCachePoliciesResultTypeDef,
     ListContinuousDeploymentPoliciesResultTypeDef,
 )
 
 
-def get_structure() -> AliasICPRecordalTypeDef:
+def get_value() -> AliasICPRecordalTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-cloudfront-1.28.15.post1/README.md` & `mypy-boto3-cloudfront-1.28.16/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudfront.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudfront)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cloudfront)](https://pepy.tech/project/mypy-boto3-cloudfront)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudFront 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront)
+[boto3.CloudFront 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront)
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
 [mypy-boto3-cloudfront docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/).
 
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
@@ -365,29 +365,30 @@
 )
 
 
 def check_value(value: CachePolicyCookieBehaviorType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_cloudfront.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_cloudfront.type_defs import (
     AliasICPRecordalTypeDef,
     AliasesOutputTypeDef,
     AliasesTypeDef,
     CachedMethodsOutputTypeDef,
     CachedMethodsTypeDef,
     AssociateAliasRequestRequestTypeDef,
+    BlobTypeDef,
     TrustedKeyGroupsOutputTypeDef,
     TrustedSignersOutputTypeDef,
     TrustedKeyGroupsTypeDef,
     TrustedSignersTypeDef,
     CookieNamesOutputTypeDef,
     CookieNamesTypeDef,
     HeadersOutputTypeDef,
@@ -526,18 +527,18 @@
     ResponseHeadersPolicyRemoveHeaderTypeDef,
     ResponseHeadersPolicyStrictTransportSecurityTypeDef,
     ResponseHeadersPolicyXSSProtectionTypeDef,
     S3OriginTypeDef,
     StreamingLoggingConfigTypeDef,
     TagKeysTypeDef,
     TagTypeDef,
-    TestFunctionRequestRequestTypeDef,
     UpdateDistributionWithStagingConfigRequestRequestTypeDef,
     AllowedMethodsOutputTypeDef,
     AllowedMethodsTypeDef,
+    TestFunctionRequestRequestTypeDef,
     CachePolicyCookiesConfigOutputTypeDef,
     CookiePreferenceOutputTypeDef,
     OriginRequestPolicyCookiesConfigOutputTypeDef,
     CachePolicyCookiesConfigTypeDef,
     CookiePreferenceTypeDef,
     OriginRequestPolicyCookiesConfigTypeDef,
     CachePolicyHeadersConfigOutputTypeDef,
@@ -589,14 +590,15 @@
     FunctionSummaryTypeDef,
     RestrictionsOutputTypeDef,
     RestrictionsTypeDef,
     GetDistributionRequestDistributionDeployedWaitTypeDef,
     GetInvalidationRequestInvalidationCompletedWaitTypeDef,
     GetStreamingDistributionRequestStreamingDistributionDeployedWaitTypeDef,
     GetKeyGroupConfigResultTypeDef,
+    KeyGroupConfigUnionTypeDef,
     KeyGroupTypeDef,
     InvalidationBatchOutputTypeDef,
     InvalidationBatchTypeDef,
     InvalidationListTypeDef,
     KGKeyPairIdsTypeDef,
     SignerTypeDef,
     LambdaFunctionAssociationsOutputTypeDef,
@@ -662,14 +664,15 @@
     UpdateFunctionResultTypeDef,
     CreateKeyGroupResultTypeDef,
     GetKeyGroupResultTypeDef,
     KeyGroupSummaryTypeDef,
     UpdateKeyGroupResultTypeDef,
     InvalidationTypeDef,
     CreateInvalidationRequestRequestTypeDef,
+    InvalidationBatchUnionTypeDef,
     ListInvalidationsResultTypeDef,
     ActiveTrustedKeyGroupsTypeDef,
     ActiveTrustedSignersTypeDef,
     CreateMonitoringSubscriptionRequestRequestTypeDef,
     CreateMonitoringSubscriptionResultTypeDef,
     GetMonitoringSubscriptionResultTypeDef,
     ListOriginAccessControlsResultTypeDef,
@@ -679,27 +682,30 @@
     QueryArgProfileConfigOutputTypeDef,
     QueryArgProfileConfigTypeDef,
     ResponseHeadersPolicyConfigOutputTypeDef,
     ResponseHeadersPolicyConfigTypeDef,
     StreamingDistributionListTypeDef,
     GetStreamingDistributionConfigResultTypeDef,
     CreateStreamingDistributionRequestRequestTypeDef,
+    StreamingDistributionConfigUnionTypeDef,
     UpdateStreamingDistributionRequestRequestTypeDef,
     ListTagsForResourceResultTypeDef,
     StreamingDistributionConfigWithTagsTypeDef,
     TagResourceRequestRequestTypeDef,
+    TagsUnionTypeDef,
     CacheBehaviorOutputTypeDef,
     DefaultCacheBehaviorOutputTypeDef,
     CacheBehaviorTypeDef,
     DefaultCacheBehaviorTypeDef,
     CachePolicyConfigOutputTypeDef,
     GetOriginRequestPolicyConfigResultTypeDef,
     OriginRequestPolicyTypeDef,
     CachePolicyConfigTypeDef,
     CreateOriginRequestPolicyRequestRequestTypeDef,
+    OriginRequestPolicyConfigUnionTypeDef,
     UpdateOriginRequestPolicyRequestRequestTypeDef,
     ContinuousDeploymentPolicyConfigOutputTypeDef,
     ContinuousDeploymentPolicyConfigTypeDef,
     OriginsOutputTypeDef,
     OriginsTypeDef,
     FieldLevelEncryptionProfileConfigOutputTypeDef,
     FieldLevelEncryptionProfileSummaryTypeDef,
@@ -718,46 +724,51 @@
     OriginGroupsTypeDef,
     FieldLevelEncryptionConfigOutputTypeDef,
     FieldLevelEncryptionSummaryTypeDef,
     FieldLevelEncryptionConfigTypeDef,
     GetResponseHeadersPolicyConfigResultTypeDef,
     ResponseHeadersPolicyTypeDef,
     CreateResponseHeadersPolicyRequestRequestTypeDef,
+    ResponseHeadersPolicyConfigUnionTypeDef,
     UpdateResponseHeadersPolicyRequestRequestTypeDef,
     ListStreamingDistributionsResultTypeDef,
     CreateStreamingDistributionWithTagsRequestRequestTypeDef,
     CacheBehaviorsOutputTypeDef,
     CacheBehaviorsTypeDef,
     CachePolicyTypeDef,
     GetCachePolicyConfigResultTypeDef,
     CreateOriginRequestPolicyResultTypeDef,
     GetOriginRequestPolicyResultTypeDef,
     OriginRequestPolicySummaryTypeDef,
     UpdateOriginRequestPolicyResultTypeDef,
+    CachePolicyConfigUnionTypeDef,
     CreateCachePolicyRequestRequestTypeDef,
     UpdateCachePolicyRequestRequestTypeDef,
     ContinuousDeploymentPolicyTypeDef,
     GetContinuousDeploymentPolicyConfigResultTypeDef,
+    ContinuousDeploymentPolicyConfigUnionTypeDef,
     CreateContinuousDeploymentPolicyRequestRequestTypeDef,
     UpdateContinuousDeploymentPolicyRequestRequestTypeDef,
     FieldLevelEncryptionProfileTypeDef,
     GetFieldLevelEncryptionProfileConfigResultTypeDef,
     FieldLevelEncryptionProfileListTypeDef,
     CreateFieldLevelEncryptionProfileRequestRequestTypeDef,
+    FieldLevelEncryptionProfileConfigUnionTypeDef,
     UpdateFieldLevelEncryptionProfileRequestRequestTypeDef,
     ListRealtimeLogConfigsResultTypeDef,
     ListKeyGroupsResultTypeDef,
     CreateStreamingDistributionResultTypeDef,
     CreateStreamingDistributionWithTagsResultTypeDef,
     GetStreamingDistributionResultTypeDef,
     UpdateStreamingDistributionResultTypeDef,
     FieldLevelEncryptionTypeDef,
     GetFieldLevelEncryptionConfigResultTypeDef,
     FieldLevelEncryptionListTypeDef,
     CreateFieldLevelEncryptionConfigRequestRequestTypeDef,
+    FieldLevelEncryptionConfigUnionTypeDef,
     UpdateFieldLevelEncryptionConfigRequestRequestTypeDef,
     CreateResponseHeadersPolicyResultTypeDef,
     GetResponseHeadersPolicyResultTypeDef,
     ResponseHeadersPolicySummaryTypeDef,
     UpdateResponseHeadersPolicyResultTypeDef,
     DistributionConfigOutputTypeDef,
     DistributionSummaryTypeDef,
@@ -780,14 +791,15 @@
     UpdateFieldLevelEncryptionConfigResultTypeDef,
     ListFieldLevelEncryptionConfigsResultTypeDef,
     ResponseHeadersPolicyListTypeDef,
     DistributionTypeDef,
     GetDistributionConfigResultTypeDef,
     DistributionListTypeDef,
     CreateDistributionRequestRequestTypeDef,
+    DistributionConfigUnionTypeDef,
     DistributionConfigWithTagsTypeDef,
     UpdateDistributionRequestRequestTypeDef,
     CachePolicyListTypeDef,
     ListOriginRequestPoliciesResultTypeDef,
     ContinuousDeploymentPolicyListTypeDef,
     ListResponseHeadersPoliciesResultTypeDef,
     CopyDistributionResultTypeDef,
@@ -801,15 +813,15 @@
     ListDistributionsResultTypeDef,
     CreateDistributionWithTagsRequestRequestTypeDef,
     ListCachePoliciesResultTypeDef,
     ListContinuousDeploymentPoliciesResultTypeDef,
 )
 
 
-def get_structure() -> AliasICPRecordalTypeDef:
+def get_value() -> AliasICPRecordalTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-cloudfront-1.28.15.post1/mypy_boto3_cloudfront/__init__.py` & `mypy-boto3-cloudfront-1.28.16/mypy_boto3_cloudfront/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudfront-1.28.15.post1/mypy_boto3_cloudfront/__init__.pyi` & `mypy-boto3-cloudfront-1.28.16/mypy_boto3_cloudfront/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudfront-1.28.15.post1/mypy_boto3_cloudfront/__main__.py` & `mypy-boto3-cloudfront-1.28.16/mypy_boto3_cloudfront/__main__.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CloudFront 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.CloudFront 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront\nOther"
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

### Comparing `mypy-boto3-cloudfront-1.28.15.post1/mypy_boto3_cloudfront/client.py` & `mypy-boto3-cloudfront-1.28.16/mypy_boto3_cloudfront/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,37 +10,35 @@
     from mypy_boto3_cloudfront.client import CloudFrontClient
 
     session = Session()
     client: CloudFrontClient = session.client("cloudfront")
     ```
 """
 import sys
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
-from botocore.response import StreamingBody
 
 from .literals import (
     CachePolicyTypeType,
     FunctionStageType,
     OriginRequestPolicyTypeType,
     ResponseHeadersPolicyTypeType,
 )
 from .paginator import (
     ListCloudFrontOriginAccessIdentitiesPaginator,
     ListDistributionsPaginator,
     ListInvalidationsPaginator,
     ListStreamingDistributionsPaginator,
 )
 from .type_defs import (
-    CachePolicyConfigOutputTypeDef,
-    CachePolicyConfigTypeDef,
+    BlobTypeDef,
+    CachePolicyConfigUnionTypeDef,
     CloudFrontOriginAccessIdentityConfigTypeDef,
-    ContinuousDeploymentPolicyConfigOutputTypeDef,
-    ContinuousDeploymentPolicyConfigTypeDef,
+    ContinuousDeploymentPolicyConfigUnionTypeDef,
     CopyDistributionResultTypeDef,
     CreateCachePolicyResultTypeDef,
     CreateCloudFrontOriginAccessIdentityResultTypeDef,
     CreateContinuousDeploymentPolicyResultTypeDef,
     CreateDistributionResultTypeDef,
     CreateDistributionWithTagsResultTypeDef,
     CreateFieldLevelEncryptionConfigResultTypeDef,
@@ -53,23 +51,20 @@
     CreateOriginRequestPolicyResultTypeDef,
     CreatePublicKeyResultTypeDef,
     CreateRealtimeLogConfigResultTypeDef,
     CreateResponseHeadersPolicyResultTypeDef,
     CreateStreamingDistributionResultTypeDef,
     CreateStreamingDistributionWithTagsResultTypeDef,
     DescribeFunctionResultTypeDef,
-    DistributionConfigOutputTypeDef,
-    DistributionConfigTypeDef,
+    DistributionConfigUnionTypeDef,
     DistributionConfigWithTagsTypeDef,
     EmptyResponseMetadataTypeDef,
     EndPointTypeDef,
-    FieldLevelEncryptionConfigOutputTypeDef,
-    FieldLevelEncryptionConfigTypeDef,
-    FieldLevelEncryptionProfileConfigOutputTypeDef,
-    FieldLevelEncryptionProfileConfigTypeDef,
+    FieldLevelEncryptionConfigUnionTypeDef,
+    FieldLevelEncryptionProfileConfigUnionTypeDef,
     FunctionConfigTypeDef,
     GetCachePolicyConfigResultTypeDef,
     GetCachePolicyResultTypeDef,
     GetCloudFrontOriginAccessIdentityConfigResultTypeDef,
     GetCloudFrontOriginAccessIdentityResultTypeDef,
     GetContinuousDeploymentPolicyConfigResultTypeDef,
     GetContinuousDeploymentPolicyResultTypeDef,
@@ -91,18 +86,16 @@
     GetPublicKeyConfigResultTypeDef,
     GetPublicKeyResultTypeDef,
     GetRealtimeLogConfigResultTypeDef,
     GetResponseHeadersPolicyConfigResultTypeDef,
     GetResponseHeadersPolicyResultTypeDef,
     GetStreamingDistributionConfigResultTypeDef,
     GetStreamingDistributionResultTypeDef,
-    InvalidationBatchOutputTypeDef,
-    InvalidationBatchTypeDef,
-    KeyGroupConfigOutputTypeDef,
-    KeyGroupConfigTypeDef,
+    InvalidationBatchUnionTypeDef,
+    KeyGroupConfigUnionTypeDef,
     ListCachePoliciesResultTypeDef,
     ListCloudFrontOriginAccessIdentitiesResultTypeDef,
     ListConflictingAliasesResultTypeDef,
     ListContinuousDeploymentPoliciesResultTypeDef,
     ListDistributionsByCachePolicyIdResultTypeDef,
     ListDistributionsByKeyGroupResultTypeDef,
     ListDistributionsByOriginRequestPolicyIdResultTypeDef,
@@ -120,26 +113,22 @@
     ListPublicKeysResultTypeDef,
     ListRealtimeLogConfigsResultTypeDef,
     ListResponseHeadersPoliciesResultTypeDef,
     ListStreamingDistributionsResultTypeDef,
     ListTagsForResourceResultTypeDef,
     MonitoringSubscriptionTypeDef,
     OriginAccessControlConfigTypeDef,
-    OriginRequestPolicyConfigOutputTypeDef,
-    OriginRequestPolicyConfigTypeDef,
+    OriginRequestPolicyConfigUnionTypeDef,
     PublicKeyConfigTypeDef,
     PublishFunctionResultTypeDef,
-    ResponseHeadersPolicyConfigOutputTypeDef,
-    ResponseHeadersPolicyConfigTypeDef,
-    StreamingDistributionConfigOutputTypeDef,
-    StreamingDistributionConfigTypeDef,
+    ResponseHeadersPolicyConfigUnionTypeDef,
+    StreamingDistributionConfigUnionTypeDef,
     StreamingDistributionConfigWithTagsTypeDef,
     TagKeysTypeDef,
-    TagsOutputTypeDef,
-    TagsTypeDef,
+    TagsUnionTypeDef,
     TestFunctionResultTypeDef,
     UpdateCachePolicyResultTypeDef,
     UpdateCloudFrontOriginAccessIdentityResultTypeDef,
     UpdateContinuousDeploymentPolicyResultTypeDef,
     UpdateDistributionResultTypeDef,
     UpdateDistributionWithStagingConfigResultTypeDef,
     UpdateFieldLevelEncryptionConfigResultTypeDef,
@@ -382,15 +371,15 @@
         distribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.copy_distribution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#copy_distribution)
         """
 
     def create_cache_policy(
-        self, *, CachePolicyConfig: Union[CachePolicyConfigTypeDef, CachePolicyConfigOutputTypeDef]
+        self, *, CachePolicyConfig: CachePolicyConfigUnionTypeDef
     ) -> CreateCachePolicyResultTypeDef:
         """
         Creates a cache policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_cache_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_cache_policy)
         """
@@ -402,32 +391,26 @@
         Creates a new origin access identity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_cloud_front_origin_access_identity)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_cloud_front_origin_access_identity)
         """
 
     def create_continuous_deployment_policy(
-        self,
-        *,
-        ContinuousDeploymentPolicyConfig: Union[
-            ContinuousDeploymentPolicyConfigTypeDef, ContinuousDeploymentPolicyConfigOutputTypeDef
-        ]
+        self, *, ContinuousDeploymentPolicyConfig: ContinuousDeploymentPolicyConfigUnionTypeDef
     ) -> CreateContinuousDeploymentPolicyResultTypeDef:
         """
         Creates a continuous deployment policy that distributes traffic for a custom
         domain name to two different CloudFront distributions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_continuous_deployment_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_continuous_deployment_policy)
         """
 
     def create_distribution(
-        self,
-        *,
-        DistributionConfig: Union[DistributionConfigTypeDef, DistributionConfigOutputTypeDef]
+        self, *, DistributionConfig: DistributionConfigUnionTypeDef
     ) -> CreateDistributionResultTypeDef:
         """
         Creates a CloudFront distribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_distribution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_distribution)
         """
@@ -439,70 +422,55 @@
         Create a new distribution with tags.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_distribution_with_tags)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_distribution_with_tags)
         """
 
     def create_field_level_encryption_config(
-        self,
-        *,
-        FieldLevelEncryptionConfig: Union[
-            FieldLevelEncryptionConfigTypeDef, FieldLevelEncryptionConfigOutputTypeDef
-        ]
+        self, *, FieldLevelEncryptionConfig: FieldLevelEncryptionConfigUnionTypeDef
     ) -> CreateFieldLevelEncryptionConfigResultTypeDef:
         """
         Create a new field-level encryption configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_field_level_encryption_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_field_level_encryption_config)
         """
 
     def create_field_level_encryption_profile(
-        self,
-        *,
-        FieldLevelEncryptionProfileConfig: Union[
-            FieldLevelEncryptionProfileConfigTypeDef, FieldLevelEncryptionProfileConfigOutputTypeDef
-        ]
+        self, *, FieldLevelEncryptionProfileConfig: FieldLevelEncryptionProfileConfigUnionTypeDef
     ) -> CreateFieldLevelEncryptionProfileResultTypeDef:
         """
         Create a field-level encryption profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_field_level_encryption_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_field_level_encryption_profile)
         """
 
     def create_function(
-        self,
-        *,
-        Name: str,
-        FunctionConfig: FunctionConfigTypeDef,
-        FunctionCode: Union[str, bytes, IO[Any], StreamingBody]
+        self, *, Name: str, FunctionConfig: FunctionConfigTypeDef, FunctionCode: BlobTypeDef
     ) -> CreateFunctionResultTypeDef:
         """
         Creates a CloudFront function.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_function)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_function)
         """
 
     def create_invalidation(
-        self,
-        *,
-        DistributionId: str,
-        InvalidationBatch: Union[InvalidationBatchTypeDef, InvalidationBatchOutputTypeDef]
+        self, *, DistributionId: str, InvalidationBatch: InvalidationBatchUnionTypeDef
     ) -> CreateInvalidationResultTypeDef:
         """
         Create a new invalidation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_invalidation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_invalidation)
         """
 
     def create_key_group(
-        self, *, KeyGroupConfig: Union[KeyGroupConfigTypeDef, KeyGroupConfigOutputTypeDef]
+        self, *, KeyGroupConfig: KeyGroupConfigUnionTypeDef
     ) -> CreateKeyGroupResultTypeDef:
         """
         Creates a key group that you can use with [CloudFront signed URLs and signed
         cookies](https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/PrivateContent.html)_.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_key_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_key_group)
@@ -525,19 +493,15 @@
         Creates a new origin access control in CloudFront.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_origin_access_control)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_origin_access_control)
         """
 
     def create_origin_request_policy(
-        self,
-        *,
-        OriginRequestPolicyConfig: Union[
-            OriginRequestPolicyConfigTypeDef, OriginRequestPolicyConfigOutputTypeDef
-        ]
+        self, *, OriginRequestPolicyConfig: OriginRequestPolicyConfigUnionTypeDef
     ) -> CreateOriginRequestPolicyResultTypeDef:
         """
         Creates an origin request policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_origin_request_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_origin_request_policy)
         """
@@ -568,33 +532,25 @@
         Creates a real-time log configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_realtime_log_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_realtime_log_config)
         """
 
     def create_response_headers_policy(
-        self,
-        *,
-        ResponseHeadersPolicyConfig: Union[
-            ResponseHeadersPolicyConfigTypeDef, ResponseHeadersPolicyConfigOutputTypeDef
-        ]
+        self, *, ResponseHeadersPolicyConfig: ResponseHeadersPolicyConfigUnionTypeDef
     ) -> CreateResponseHeadersPolicyResultTypeDef:
         """
         Creates a response headers policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_response_headers_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_response_headers_policy)
         """
 
     def create_streaming_distribution(
-        self,
-        *,
-        StreamingDistributionConfig: Union[
-            StreamingDistributionConfigTypeDef, StreamingDistributionConfigOutputTypeDef
-        ]
+        self, *, StreamingDistributionConfig: StreamingDistributionConfigUnionTypeDef
     ) -> CreateStreamingDistributionResultTypeDef:
         """
         This API is deprecated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_streaming_distribution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_streaming_distribution)
         """
@@ -1282,30 +1238,25 @@
         `DEVELOPMENT` stage to `LIVE`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.publish_function)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#publish_function)
         """
 
     def tag_resource(
-        self, *, Resource: str, Tags: Union[TagsTypeDef, TagsOutputTypeDef]
+        self, *, Resource: str, Tags: TagsUnionTypeDef
     ) -> EmptyResponseMetadataTypeDef:
         """
         Add tags to a CloudFront resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#tag_resource)
         """
 
     def test_function(
-        self,
-        *,
-        Name: str,
-        IfMatch: str,
-        EventObject: Union[str, bytes, IO[Any], StreamingBody],
-        Stage: FunctionStageType = ...
+        self, *, Name: str, IfMatch: str, EventObject: BlobTypeDef, Stage: FunctionStageType = ...
     ) -> TestFunctionResultTypeDef:
         """
         Tests a CloudFront function.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.test_function)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#test_function)
         """
@@ -1317,19 +1268,15 @@
         Remove tags from a CloudFront resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#untag_resource)
         """
 
     def update_cache_policy(
-        self,
-        *,
-        CachePolicyConfig: Union[CachePolicyConfigTypeDef, CachePolicyConfigOutputTypeDef],
-        Id: str,
-        IfMatch: str = ...
+        self, *, CachePolicyConfig: CachePolicyConfigUnionTypeDef, Id: str, IfMatch: str = ...
     ) -> UpdateCachePolicyResultTypeDef:
         """
         Updates a cache policy configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_cache_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_cache_policy)
         """
@@ -1347,33 +1294,27 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_cloud_front_origin_access_identity)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_cloud_front_origin_access_identity)
         """
 
     def update_continuous_deployment_policy(
         self,
         *,
-        ContinuousDeploymentPolicyConfig: Union[
-            ContinuousDeploymentPolicyConfigTypeDef, ContinuousDeploymentPolicyConfigOutputTypeDef
-        ],
+        ContinuousDeploymentPolicyConfig: ContinuousDeploymentPolicyConfigUnionTypeDef,
         Id: str,
         IfMatch: str = ...
     ) -> UpdateContinuousDeploymentPolicyResultTypeDef:
         """
         Updates a continuous deployment policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_continuous_deployment_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_continuous_deployment_policy)
         """
 
     def update_distribution(
-        self,
-        *,
-        DistributionConfig: Union[DistributionConfigTypeDef, DistributionConfigOutputTypeDef],
-        Id: str,
-        IfMatch: str = ...
+        self, *, DistributionConfig: DistributionConfigUnionTypeDef, Id: str, IfMatch: str = ...
     ) -> UpdateDistributionResultTypeDef:
         """
         Updates the configuration for a CloudFront distribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_distribution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_distribution)
         """
@@ -1388,33 +1329,29 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_distribution_with_staging_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_distribution_with_staging_config)
         """
 
     def update_field_level_encryption_config(
         self,
         *,
-        FieldLevelEncryptionConfig: Union[
-            FieldLevelEncryptionConfigTypeDef, FieldLevelEncryptionConfigOutputTypeDef
-        ],
+        FieldLevelEncryptionConfig: FieldLevelEncryptionConfigUnionTypeDef,
         Id: str,
         IfMatch: str = ...
     ) -> UpdateFieldLevelEncryptionConfigResultTypeDef:
         """
         Update a field-level encryption configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_field_level_encryption_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_field_level_encryption_config)
         """
 
     def update_field_level_encryption_profile(
         self,
         *,
-        FieldLevelEncryptionProfileConfig: Union[
-            FieldLevelEncryptionProfileConfigTypeDef, FieldLevelEncryptionProfileConfigOutputTypeDef
-        ],
+        FieldLevelEncryptionProfileConfig: FieldLevelEncryptionProfileConfigUnionTypeDef,
         Id: str,
         IfMatch: str = ...
     ) -> UpdateFieldLevelEncryptionProfileResultTypeDef:
         """
         Update a field-level encryption profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_field_level_encryption_profile)
@@ -1423,29 +1360,25 @@
 
     def update_function(
         self,
         *,
         Name: str,
         IfMatch: str,
         FunctionConfig: FunctionConfigTypeDef,
-        FunctionCode: Union[str, bytes, IO[Any], StreamingBody]
+        FunctionCode: BlobTypeDef
     ) -> UpdateFunctionResultTypeDef:
         """
         Updates a CloudFront function.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_function)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_function)
         """
 
     def update_key_group(
-        self,
-        *,
-        KeyGroupConfig: Union[KeyGroupConfigTypeDef, KeyGroupConfigOutputTypeDef],
-        Id: str,
-        IfMatch: str = ...
+        self, *, KeyGroupConfig: KeyGroupConfigUnionTypeDef, Id: str, IfMatch: str = ...
     ) -> UpdateKeyGroupResultTypeDef:
         """
         Updates a key group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_key_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_key_group)
         """
@@ -1463,17 +1396,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_origin_access_control)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_origin_access_control)
         """
 
     def update_origin_request_policy(
         self,
         *,
-        OriginRequestPolicyConfig: Union[
-            OriginRequestPolicyConfigTypeDef, OriginRequestPolicyConfigOutputTypeDef
-        ],
+        OriginRequestPolicyConfig: OriginRequestPolicyConfigUnionTypeDef,
         Id: str,
         IfMatch: str = ...
     ) -> UpdateOriginRequestPolicyResultTypeDef:
         """
         Updates an origin request policy configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_origin_request_policy)
@@ -1505,33 +1436,29 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_realtime_log_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_realtime_log_config)
         """
 
     def update_response_headers_policy(
         self,
         *,
-        ResponseHeadersPolicyConfig: Union[
-            ResponseHeadersPolicyConfigTypeDef, ResponseHeadersPolicyConfigOutputTypeDef
-        ],
+        ResponseHeadersPolicyConfig: ResponseHeadersPolicyConfigUnionTypeDef,
         Id: str,
         IfMatch: str = ...
     ) -> UpdateResponseHeadersPolicyResultTypeDef:
         """
         Updates a response headers policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_response_headers_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_response_headers_policy)
         """
 
     def update_streaming_distribution(
         self,
         *,
-        StreamingDistributionConfig: Union[
-            StreamingDistributionConfigTypeDef, StreamingDistributionConfigOutputTypeDef
-        ],
+        StreamingDistributionConfig: StreamingDistributionConfigUnionTypeDef,
         Id: str,
         IfMatch: str = ...
     ) -> UpdateStreamingDistributionResultTypeDef:
         """
         Update a streaming distribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_streaming_distribution)
```

### Comparing `mypy-boto3-cloudfront-1.28.15.post1/mypy_boto3_cloudfront/client.pyi` & `mypy-boto3-cloudfront-1.28.16/mypy_boto3_cloudfront/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -10,37 +10,35 @@
     from mypy_boto3_cloudfront.client import CloudFrontClient
 
     session = Session()
     client: CloudFrontClient = session.client("cloudfront")
     ```
 """
 import sys
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
-from botocore.response import StreamingBody
 
 from .literals import (
     CachePolicyTypeType,
     FunctionStageType,
     OriginRequestPolicyTypeType,
     ResponseHeadersPolicyTypeType,
 )
 from .paginator import (
     ListCloudFrontOriginAccessIdentitiesPaginator,
     ListDistributionsPaginator,
     ListInvalidationsPaginator,
     ListStreamingDistributionsPaginator,
 )
 from .type_defs import (
-    CachePolicyConfigOutputTypeDef,
-    CachePolicyConfigTypeDef,
+    BlobTypeDef,
+    CachePolicyConfigUnionTypeDef,
     CloudFrontOriginAccessIdentityConfigTypeDef,
-    ContinuousDeploymentPolicyConfigOutputTypeDef,
-    ContinuousDeploymentPolicyConfigTypeDef,
+    ContinuousDeploymentPolicyConfigUnionTypeDef,
     CopyDistributionResultTypeDef,
     CreateCachePolicyResultTypeDef,
     CreateCloudFrontOriginAccessIdentityResultTypeDef,
     CreateContinuousDeploymentPolicyResultTypeDef,
     CreateDistributionResultTypeDef,
     CreateDistributionWithTagsResultTypeDef,
     CreateFieldLevelEncryptionConfigResultTypeDef,
@@ -53,23 +51,20 @@
     CreateOriginRequestPolicyResultTypeDef,
     CreatePublicKeyResultTypeDef,
     CreateRealtimeLogConfigResultTypeDef,
     CreateResponseHeadersPolicyResultTypeDef,
     CreateStreamingDistributionResultTypeDef,
     CreateStreamingDistributionWithTagsResultTypeDef,
     DescribeFunctionResultTypeDef,
-    DistributionConfigOutputTypeDef,
-    DistributionConfigTypeDef,
+    DistributionConfigUnionTypeDef,
     DistributionConfigWithTagsTypeDef,
     EmptyResponseMetadataTypeDef,
     EndPointTypeDef,
-    FieldLevelEncryptionConfigOutputTypeDef,
-    FieldLevelEncryptionConfigTypeDef,
-    FieldLevelEncryptionProfileConfigOutputTypeDef,
-    FieldLevelEncryptionProfileConfigTypeDef,
+    FieldLevelEncryptionConfigUnionTypeDef,
+    FieldLevelEncryptionProfileConfigUnionTypeDef,
     FunctionConfigTypeDef,
     GetCachePolicyConfigResultTypeDef,
     GetCachePolicyResultTypeDef,
     GetCloudFrontOriginAccessIdentityConfigResultTypeDef,
     GetCloudFrontOriginAccessIdentityResultTypeDef,
     GetContinuousDeploymentPolicyConfigResultTypeDef,
     GetContinuousDeploymentPolicyResultTypeDef,
@@ -91,18 +86,16 @@
     GetPublicKeyConfigResultTypeDef,
     GetPublicKeyResultTypeDef,
     GetRealtimeLogConfigResultTypeDef,
     GetResponseHeadersPolicyConfigResultTypeDef,
     GetResponseHeadersPolicyResultTypeDef,
     GetStreamingDistributionConfigResultTypeDef,
     GetStreamingDistributionResultTypeDef,
-    InvalidationBatchOutputTypeDef,
-    InvalidationBatchTypeDef,
-    KeyGroupConfigOutputTypeDef,
-    KeyGroupConfigTypeDef,
+    InvalidationBatchUnionTypeDef,
+    KeyGroupConfigUnionTypeDef,
     ListCachePoliciesResultTypeDef,
     ListCloudFrontOriginAccessIdentitiesResultTypeDef,
     ListConflictingAliasesResultTypeDef,
     ListContinuousDeploymentPoliciesResultTypeDef,
     ListDistributionsByCachePolicyIdResultTypeDef,
     ListDistributionsByKeyGroupResultTypeDef,
     ListDistributionsByOriginRequestPolicyIdResultTypeDef,
@@ -120,26 +113,22 @@
     ListPublicKeysResultTypeDef,
     ListRealtimeLogConfigsResultTypeDef,
     ListResponseHeadersPoliciesResultTypeDef,
     ListStreamingDistributionsResultTypeDef,
     ListTagsForResourceResultTypeDef,
     MonitoringSubscriptionTypeDef,
     OriginAccessControlConfigTypeDef,
-    OriginRequestPolicyConfigOutputTypeDef,
-    OriginRequestPolicyConfigTypeDef,
+    OriginRequestPolicyConfigUnionTypeDef,
     PublicKeyConfigTypeDef,
     PublishFunctionResultTypeDef,
-    ResponseHeadersPolicyConfigOutputTypeDef,
-    ResponseHeadersPolicyConfigTypeDef,
-    StreamingDistributionConfigOutputTypeDef,
-    StreamingDistributionConfigTypeDef,
+    ResponseHeadersPolicyConfigUnionTypeDef,
+    StreamingDistributionConfigUnionTypeDef,
     StreamingDistributionConfigWithTagsTypeDef,
     TagKeysTypeDef,
-    TagsOutputTypeDef,
-    TagsTypeDef,
+    TagsUnionTypeDef,
     TestFunctionResultTypeDef,
     UpdateCachePolicyResultTypeDef,
     UpdateCloudFrontOriginAccessIdentityResultTypeDef,
     UpdateContinuousDeploymentPolicyResultTypeDef,
     UpdateDistributionResultTypeDef,
     UpdateDistributionWithStagingConfigResultTypeDef,
     UpdateFieldLevelEncryptionConfigResultTypeDef,
@@ -373,15 +362,15 @@
         Creates a staging distribution using the configuration of the provided primary
         distribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.copy_distribution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#copy_distribution)
         """
     def create_cache_policy(
-        self, *, CachePolicyConfig: Union[CachePolicyConfigTypeDef, CachePolicyConfigOutputTypeDef]
+        self, *, CachePolicyConfig: CachePolicyConfigUnionTypeDef
     ) -> CreateCachePolicyResultTypeDef:
         """
         Creates a cache policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_cache_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_cache_policy)
         """
@@ -391,31 +380,25 @@
         """
         Creates a new origin access identity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_cloud_front_origin_access_identity)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_cloud_front_origin_access_identity)
         """
     def create_continuous_deployment_policy(
-        self,
-        *,
-        ContinuousDeploymentPolicyConfig: Union[
-            ContinuousDeploymentPolicyConfigTypeDef, ContinuousDeploymentPolicyConfigOutputTypeDef
-        ]
+        self, *, ContinuousDeploymentPolicyConfig: ContinuousDeploymentPolicyConfigUnionTypeDef
     ) -> CreateContinuousDeploymentPolicyResultTypeDef:
         """
         Creates a continuous deployment policy that distributes traffic for a custom
         domain name to two different CloudFront distributions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_continuous_deployment_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_continuous_deployment_policy)
         """
     def create_distribution(
-        self,
-        *,
-        DistributionConfig: Union[DistributionConfigTypeDef, DistributionConfigOutputTypeDef]
+        self, *, DistributionConfig: DistributionConfigUnionTypeDef
     ) -> CreateDistributionResultTypeDef:
         """
         Creates a CloudFront distribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_distribution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_distribution)
         """
@@ -425,66 +408,51 @@
         """
         Create a new distribution with tags.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_distribution_with_tags)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_distribution_with_tags)
         """
     def create_field_level_encryption_config(
-        self,
-        *,
-        FieldLevelEncryptionConfig: Union[
-            FieldLevelEncryptionConfigTypeDef, FieldLevelEncryptionConfigOutputTypeDef
-        ]
+        self, *, FieldLevelEncryptionConfig: FieldLevelEncryptionConfigUnionTypeDef
     ) -> CreateFieldLevelEncryptionConfigResultTypeDef:
         """
         Create a new field-level encryption configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_field_level_encryption_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_field_level_encryption_config)
         """
     def create_field_level_encryption_profile(
-        self,
-        *,
-        FieldLevelEncryptionProfileConfig: Union[
-            FieldLevelEncryptionProfileConfigTypeDef, FieldLevelEncryptionProfileConfigOutputTypeDef
-        ]
+        self, *, FieldLevelEncryptionProfileConfig: FieldLevelEncryptionProfileConfigUnionTypeDef
     ) -> CreateFieldLevelEncryptionProfileResultTypeDef:
         """
         Create a field-level encryption profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_field_level_encryption_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_field_level_encryption_profile)
         """
     def create_function(
-        self,
-        *,
-        Name: str,
-        FunctionConfig: FunctionConfigTypeDef,
-        FunctionCode: Union[str, bytes, IO[Any], StreamingBody]
+        self, *, Name: str, FunctionConfig: FunctionConfigTypeDef, FunctionCode: BlobTypeDef
     ) -> CreateFunctionResultTypeDef:
         """
         Creates a CloudFront function.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_function)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_function)
         """
     def create_invalidation(
-        self,
-        *,
-        DistributionId: str,
-        InvalidationBatch: Union[InvalidationBatchTypeDef, InvalidationBatchOutputTypeDef]
+        self, *, DistributionId: str, InvalidationBatch: InvalidationBatchUnionTypeDef
     ) -> CreateInvalidationResultTypeDef:
         """
         Create a new invalidation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_invalidation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_invalidation)
         """
     def create_key_group(
-        self, *, KeyGroupConfig: Union[KeyGroupConfigTypeDef, KeyGroupConfigOutputTypeDef]
+        self, *, KeyGroupConfig: KeyGroupConfigUnionTypeDef
     ) -> CreateKeyGroupResultTypeDef:
         """
         Creates a key group that you can use with [CloudFront signed URLs and signed
         cookies](https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/PrivateContent.html)_.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_key_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_key_group)
@@ -504,19 +472,15 @@
         """
         Creates a new origin access control in CloudFront.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_origin_access_control)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_origin_access_control)
         """
     def create_origin_request_policy(
-        self,
-        *,
-        OriginRequestPolicyConfig: Union[
-            OriginRequestPolicyConfigTypeDef, OriginRequestPolicyConfigOutputTypeDef
-        ]
+        self, *, OriginRequestPolicyConfig: OriginRequestPolicyConfigUnionTypeDef
     ) -> CreateOriginRequestPolicyResultTypeDef:
         """
         Creates an origin request policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_origin_request_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_origin_request_policy)
         """
@@ -544,32 +508,24 @@
         """
         Creates a real-time log configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_realtime_log_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_realtime_log_config)
         """
     def create_response_headers_policy(
-        self,
-        *,
-        ResponseHeadersPolicyConfig: Union[
-            ResponseHeadersPolicyConfigTypeDef, ResponseHeadersPolicyConfigOutputTypeDef
-        ]
+        self, *, ResponseHeadersPolicyConfig: ResponseHeadersPolicyConfigUnionTypeDef
     ) -> CreateResponseHeadersPolicyResultTypeDef:
         """
         Creates a response headers policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_response_headers_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_response_headers_policy)
         """
     def create_streaming_distribution(
-        self,
-        *,
-        StreamingDistributionConfig: Union[
-            StreamingDistributionConfigTypeDef, StreamingDistributionConfigOutputTypeDef
-        ]
+        self, *, StreamingDistributionConfig: StreamingDistributionConfigUnionTypeDef
     ) -> CreateStreamingDistributionResultTypeDef:
         """
         This API is deprecated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_streaming_distribution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_streaming_distribution)
         """
@@ -1186,29 +1142,24 @@
         Publishes a CloudFront function by copying the function code from the
         `DEVELOPMENT` stage to `LIVE`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.publish_function)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#publish_function)
         """
     def tag_resource(
-        self, *, Resource: str, Tags: Union[TagsTypeDef, TagsOutputTypeDef]
+        self, *, Resource: str, Tags: TagsUnionTypeDef
     ) -> EmptyResponseMetadataTypeDef:
         """
         Add tags to a CloudFront resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#tag_resource)
         """
     def test_function(
-        self,
-        *,
-        Name: str,
-        IfMatch: str,
-        EventObject: Union[str, bytes, IO[Any], StreamingBody],
-        Stage: FunctionStageType = ...
+        self, *, Name: str, IfMatch: str, EventObject: BlobTypeDef, Stage: FunctionStageType = ...
     ) -> TestFunctionResultTypeDef:
         """
         Tests a CloudFront function.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.test_function)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#test_function)
         """
@@ -1218,19 +1169,15 @@
         """
         Remove tags from a CloudFront resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#untag_resource)
         """
     def update_cache_policy(
-        self,
-        *,
-        CachePolicyConfig: Union[CachePolicyConfigTypeDef, CachePolicyConfigOutputTypeDef],
-        Id: str,
-        IfMatch: str = ...
+        self, *, CachePolicyConfig: CachePolicyConfigUnionTypeDef, Id: str, IfMatch: str = ...
     ) -> UpdateCachePolicyResultTypeDef:
         """
         Updates a cache policy configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_cache_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_cache_policy)
         """
@@ -1246,32 +1193,26 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_cloud_front_origin_access_identity)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_cloud_front_origin_access_identity)
         """
     def update_continuous_deployment_policy(
         self,
         *,
-        ContinuousDeploymentPolicyConfig: Union[
-            ContinuousDeploymentPolicyConfigTypeDef, ContinuousDeploymentPolicyConfigOutputTypeDef
-        ],
+        ContinuousDeploymentPolicyConfig: ContinuousDeploymentPolicyConfigUnionTypeDef,
         Id: str,
         IfMatch: str = ...
     ) -> UpdateContinuousDeploymentPolicyResultTypeDef:
         """
         Updates a continuous deployment policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_continuous_deployment_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_continuous_deployment_policy)
         """
     def update_distribution(
-        self,
-        *,
-        DistributionConfig: Union[DistributionConfigTypeDef, DistributionConfigOutputTypeDef],
-        Id: str,
-        IfMatch: str = ...
+        self, *, DistributionConfig: DistributionConfigUnionTypeDef, Id: str, IfMatch: str = ...
     ) -> UpdateDistributionResultTypeDef:
         """
         Updates the configuration for a CloudFront distribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_distribution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_distribution)
         """
@@ -1284,32 +1225,28 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_distribution_with_staging_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_distribution_with_staging_config)
         """
     def update_field_level_encryption_config(
         self,
         *,
-        FieldLevelEncryptionConfig: Union[
-            FieldLevelEncryptionConfigTypeDef, FieldLevelEncryptionConfigOutputTypeDef
-        ],
+        FieldLevelEncryptionConfig: FieldLevelEncryptionConfigUnionTypeDef,
         Id: str,
         IfMatch: str = ...
     ) -> UpdateFieldLevelEncryptionConfigResultTypeDef:
         """
         Update a field-level encryption configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_field_level_encryption_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_field_level_encryption_config)
         """
     def update_field_level_encryption_profile(
         self,
         *,
-        FieldLevelEncryptionProfileConfig: Union[
-            FieldLevelEncryptionProfileConfigTypeDef, FieldLevelEncryptionProfileConfigOutputTypeDef
-        ],
+        FieldLevelEncryptionProfileConfig: FieldLevelEncryptionProfileConfigUnionTypeDef,
         Id: str,
         IfMatch: str = ...
     ) -> UpdateFieldLevelEncryptionProfileResultTypeDef:
         """
         Update a field-level encryption profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_field_level_encryption_profile)
@@ -1317,28 +1254,24 @@
         """
     def update_function(
         self,
         *,
         Name: str,
         IfMatch: str,
         FunctionConfig: FunctionConfigTypeDef,
-        FunctionCode: Union[str, bytes, IO[Any], StreamingBody]
+        FunctionCode: BlobTypeDef
     ) -> UpdateFunctionResultTypeDef:
         """
         Updates a CloudFront function.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_function)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_function)
         """
     def update_key_group(
-        self,
-        *,
-        KeyGroupConfig: Union[KeyGroupConfigTypeDef, KeyGroupConfigOutputTypeDef],
-        Id: str,
-        IfMatch: str = ...
+        self, *, KeyGroupConfig: KeyGroupConfigUnionTypeDef, Id: str, IfMatch: str = ...
     ) -> UpdateKeyGroupResultTypeDef:
         """
         Updates a key group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_key_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_key_group)
         """
@@ -1354,17 +1287,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_origin_access_control)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_origin_access_control)
         """
     def update_origin_request_policy(
         self,
         *,
-        OriginRequestPolicyConfig: Union[
-            OriginRequestPolicyConfigTypeDef, OriginRequestPolicyConfigOutputTypeDef
-        ],
+        OriginRequestPolicyConfig: OriginRequestPolicyConfigUnionTypeDef,
         Id: str,
         IfMatch: str = ...
     ) -> UpdateOriginRequestPolicyResultTypeDef:
         """
         Updates an origin request policy configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_origin_request_policy)
@@ -1393,32 +1324,28 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_realtime_log_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_realtime_log_config)
         """
     def update_response_headers_policy(
         self,
         *,
-        ResponseHeadersPolicyConfig: Union[
-            ResponseHeadersPolicyConfigTypeDef, ResponseHeadersPolicyConfigOutputTypeDef
-        ],
+        ResponseHeadersPolicyConfig: ResponseHeadersPolicyConfigUnionTypeDef,
         Id: str,
         IfMatch: str = ...
     ) -> UpdateResponseHeadersPolicyResultTypeDef:
         """
         Updates a response headers policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_response_headers_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_response_headers_policy)
         """
     def update_streaming_distribution(
         self,
         *,
-        StreamingDistributionConfig: Union[
-            StreamingDistributionConfigTypeDef, StreamingDistributionConfigOutputTypeDef
-        ],
+        StreamingDistributionConfig: StreamingDistributionConfigUnionTypeDef,
         Id: str,
         IfMatch: str = ...
     ) -> UpdateStreamingDistributionResultTypeDef:
         """
         Update a streaming distribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_streaming_distribution)
```

### Comparing `mypy-boto3-cloudfront-1.28.15.post1/mypy_boto3_cloudfront/literals.py` & `mypy-boto3-cloudfront-1.28.16/mypy_boto3_cloudfront/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudfront-1.28.15.post1/mypy_boto3_cloudfront/literals.pyi` & `mypy-boto3-cloudfront-1.28.16/mypy_boto3_cloudfront/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudfront-1.28.15.post1/mypy_boto3_cloudfront/paginator.py` & `mypy-boto3-cloudfront-1.28.16/mypy_boto3_cloudfront/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudfront-1.28.15.post1/mypy_boto3_cloudfront/paginator.pyi` & `mypy-boto3-cloudfront-1.28.16/mypy_boto3_cloudfront/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudfront-1.28.15.post1/mypy_boto3_cloudfront/type_defs.py` & `mypy-boto3-cloudfront-1.28.16/mypy_boto3_cloudfront/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_cloudfront.type_defs import AliasICPRecordalTypeDef
 
-    data: AliasICPRecordalTypeDef = {...}
+    data: AliasICPRecordalTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -64,14 +64,15 @@
 __all__ = (
     "AliasICPRecordalTypeDef",
     "AliasesOutputTypeDef",
     "AliasesTypeDef",
     "CachedMethodsOutputTypeDef",
     "CachedMethodsTypeDef",
     "AssociateAliasRequestRequestTypeDef",
+    "BlobTypeDef",
     "TrustedKeyGroupsOutputTypeDef",
     "TrustedSignersOutputTypeDef",
     "TrustedKeyGroupsTypeDef",
     "TrustedSignersTypeDef",
     "CookieNamesOutputTypeDef",
     "CookieNamesTypeDef",
     "HeadersOutputTypeDef",
@@ -210,18 +211,18 @@
     "ResponseHeadersPolicyRemoveHeaderTypeDef",
     "ResponseHeadersPolicyStrictTransportSecurityTypeDef",
     "ResponseHeadersPolicyXSSProtectionTypeDef",
     "S3OriginTypeDef",
     "StreamingLoggingConfigTypeDef",
     "TagKeysTypeDef",
     "TagTypeDef",
-    "TestFunctionRequestRequestTypeDef",
     "UpdateDistributionWithStagingConfigRequestRequestTypeDef",
     "AllowedMethodsOutputTypeDef",
     "AllowedMethodsTypeDef",
+    "TestFunctionRequestRequestTypeDef",
     "CachePolicyCookiesConfigOutputTypeDef",
     "CookiePreferenceOutputTypeDef",
     "OriginRequestPolicyCookiesConfigOutputTypeDef",
     "CachePolicyCookiesConfigTypeDef",
     "CookiePreferenceTypeDef",
     "OriginRequestPolicyCookiesConfigTypeDef",
     "CachePolicyHeadersConfigOutputTypeDef",
@@ -273,14 +274,15 @@
     "FunctionSummaryTypeDef",
     "RestrictionsOutputTypeDef",
     "RestrictionsTypeDef",
     "GetDistributionRequestDistributionDeployedWaitTypeDef",
     "GetInvalidationRequestInvalidationCompletedWaitTypeDef",
     "GetStreamingDistributionRequestStreamingDistributionDeployedWaitTypeDef",
     "GetKeyGroupConfigResultTypeDef",
+    "KeyGroupConfigUnionTypeDef",
     "KeyGroupTypeDef",
     "InvalidationBatchOutputTypeDef",
     "InvalidationBatchTypeDef",
     "InvalidationListTypeDef",
     "KGKeyPairIdsTypeDef",
     "SignerTypeDef",
     "LambdaFunctionAssociationsOutputTypeDef",
@@ -346,14 +348,15 @@
     "UpdateFunctionResultTypeDef",
     "CreateKeyGroupResultTypeDef",
     "GetKeyGroupResultTypeDef",
     "KeyGroupSummaryTypeDef",
     "UpdateKeyGroupResultTypeDef",
     "InvalidationTypeDef",
     "CreateInvalidationRequestRequestTypeDef",
+    "InvalidationBatchUnionTypeDef",
     "ListInvalidationsResultTypeDef",
     "ActiveTrustedKeyGroupsTypeDef",
     "ActiveTrustedSignersTypeDef",
     "CreateMonitoringSubscriptionRequestRequestTypeDef",
     "CreateMonitoringSubscriptionResultTypeDef",
     "GetMonitoringSubscriptionResultTypeDef",
     "ListOriginAccessControlsResultTypeDef",
@@ -363,27 +366,30 @@
     "QueryArgProfileConfigOutputTypeDef",
     "QueryArgProfileConfigTypeDef",
     "ResponseHeadersPolicyConfigOutputTypeDef",
     "ResponseHeadersPolicyConfigTypeDef",
     "StreamingDistributionListTypeDef",
     "GetStreamingDistributionConfigResultTypeDef",
     "CreateStreamingDistributionRequestRequestTypeDef",
+    "StreamingDistributionConfigUnionTypeDef",
     "UpdateStreamingDistributionRequestRequestTypeDef",
     "ListTagsForResourceResultTypeDef",
     "StreamingDistributionConfigWithTagsTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "TagsUnionTypeDef",
     "CacheBehaviorOutputTypeDef",
     "DefaultCacheBehaviorOutputTypeDef",
     "CacheBehaviorTypeDef",
     "DefaultCacheBehaviorTypeDef",
     "CachePolicyConfigOutputTypeDef",
     "GetOriginRequestPolicyConfigResultTypeDef",
     "OriginRequestPolicyTypeDef",
     "CachePolicyConfigTypeDef",
     "CreateOriginRequestPolicyRequestRequestTypeDef",
+    "OriginRequestPolicyConfigUnionTypeDef",
     "UpdateOriginRequestPolicyRequestRequestTypeDef",
     "ContinuousDeploymentPolicyConfigOutputTypeDef",
     "ContinuousDeploymentPolicyConfigTypeDef",
     "OriginsOutputTypeDef",
     "OriginsTypeDef",
     "FieldLevelEncryptionProfileConfigOutputTypeDef",
     "FieldLevelEncryptionProfileSummaryTypeDef",
@@ -402,46 +408,51 @@
     "OriginGroupsTypeDef",
     "FieldLevelEncryptionConfigOutputTypeDef",
     "FieldLevelEncryptionSummaryTypeDef",
     "FieldLevelEncryptionConfigTypeDef",
     "GetResponseHeadersPolicyConfigResultTypeDef",
     "ResponseHeadersPolicyTypeDef",
     "CreateResponseHeadersPolicyRequestRequestTypeDef",
+    "ResponseHeadersPolicyConfigUnionTypeDef",
     "UpdateResponseHeadersPolicyRequestRequestTypeDef",
     "ListStreamingDistributionsResultTypeDef",
     "CreateStreamingDistributionWithTagsRequestRequestTypeDef",
     "CacheBehaviorsOutputTypeDef",
     "CacheBehaviorsTypeDef",
     "CachePolicyTypeDef",
     "GetCachePolicyConfigResultTypeDef",
     "CreateOriginRequestPolicyResultTypeDef",
     "GetOriginRequestPolicyResultTypeDef",
     "OriginRequestPolicySummaryTypeDef",
     "UpdateOriginRequestPolicyResultTypeDef",
+    "CachePolicyConfigUnionTypeDef",
     "CreateCachePolicyRequestRequestTypeDef",
     "UpdateCachePolicyRequestRequestTypeDef",
     "ContinuousDeploymentPolicyTypeDef",
     "GetContinuousDeploymentPolicyConfigResultTypeDef",
+    "ContinuousDeploymentPolicyConfigUnionTypeDef",
     "CreateContinuousDeploymentPolicyRequestRequestTypeDef",
     "UpdateContinuousDeploymentPolicyRequestRequestTypeDef",
     "FieldLevelEncryptionProfileTypeDef",
     "GetFieldLevelEncryptionProfileConfigResultTypeDef",
     "FieldLevelEncryptionProfileListTypeDef",
     "CreateFieldLevelEncryptionProfileRequestRequestTypeDef",
+    "FieldLevelEncryptionProfileConfigUnionTypeDef",
     "UpdateFieldLevelEncryptionProfileRequestRequestTypeDef",
     "ListRealtimeLogConfigsResultTypeDef",
     "ListKeyGroupsResultTypeDef",
     "CreateStreamingDistributionResultTypeDef",
     "CreateStreamingDistributionWithTagsResultTypeDef",
     "GetStreamingDistributionResultTypeDef",
     "UpdateStreamingDistributionResultTypeDef",
     "FieldLevelEncryptionTypeDef",
     "GetFieldLevelEncryptionConfigResultTypeDef",
     "FieldLevelEncryptionListTypeDef",
     "CreateFieldLevelEncryptionConfigRequestRequestTypeDef",
+    "FieldLevelEncryptionConfigUnionTypeDef",
     "UpdateFieldLevelEncryptionConfigRequestRequestTypeDef",
     "CreateResponseHeadersPolicyResultTypeDef",
     "GetResponseHeadersPolicyResultTypeDef",
     "ResponseHeadersPolicySummaryTypeDef",
     "UpdateResponseHeadersPolicyResultTypeDef",
     "DistributionConfigOutputTypeDef",
     "DistributionSummaryTypeDef",
@@ -464,14 +475,15 @@
     "UpdateFieldLevelEncryptionConfigResultTypeDef",
     "ListFieldLevelEncryptionConfigsResultTypeDef",
     "ResponseHeadersPolicyListTypeDef",
     "DistributionTypeDef",
     "GetDistributionConfigResultTypeDef",
     "DistributionListTypeDef",
     "CreateDistributionRequestRequestTypeDef",
+    "DistributionConfigUnionTypeDef",
     "DistributionConfigWithTagsTypeDef",
     "UpdateDistributionRequestRequestTypeDef",
     "CachePolicyListTypeDef",
     "ListOriginRequestPoliciesResultTypeDef",
     "ContinuousDeploymentPolicyListTypeDef",
     "ListResponseHeadersPoliciesResultTypeDef",
     "CopyDistributionResultTypeDef",
@@ -555,14 +567,15 @@
     "AssociateAliasRequestRequestTypeDef",
     {
         "TargetDistributionId": str,
         "Alias": str,
     },
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 _RequiredTrustedKeyGroupsOutputTypeDef = TypedDict(
     "_RequiredTrustedKeyGroupsOutputTypeDef",
     {
         "Enabled": bool,
         "Quantity": int,
     },
 )
@@ -2546,37 +2559,14 @@
 )
 
 
 class TagTypeDef(_RequiredTagTypeDef, _OptionalTagTypeDef):
     pass
 
 
-_RequiredTestFunctionRequestRequestTypeDef = TypedDict(
-    "_RequiredTestFunctionRequestRequestTypeDef",
-    {
-        "Name": str,
-        "IfMatch": str,
-        "EventObject": Union[str, bytes, IO[Any], StreamingBody],
-    },
-)
-_OptionalTestFunctionRequestRequestTypeDef = TypedDict(
-    "_OptionalTestFunctionRequestRequestTypeDef",
-    {
-        "Stage": FunctionStageType,
-    },
-    total=False,
-)
-
-
-class TestFunctionRequestRequestTypeDef(
-    _RequiredTestFunctionRequestRequestTypeDef, _OptionalTestFunctionRequestRequestTypeDef
-):
-    pass
-
-
 _RequiredUpdateDistributionWithStagingConfigRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDistributionWithStagingConfigRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalUpdateDistributionWithStagingConfigRequestRequestTypeDef = TypedDict(
@@ -2634,14 +2624,37 @@
 )
 
 
 class AllowedMethodsTypeDef(_RequiredAllowedMethodsTypeDef, _OptionalAllowedMethodsTypeDef):
     pass
 
 
+_RequiredTestFunctionRequestRequestTypeDef = TypedDict(
+    "_RequiredTestFunctionRequestRequestTypeDef",
+    {
+        "Name": str,
+        "IfMatch": str,
+        "EventObject": BlobTypeDef,
+    },
+)
+_OptionalTestFunctionRequestRequestTypeDef = TypedDict(
+    "_OptionalTestFunctionRequestRequestTypeDef",
+    {
+        "Stage": FunctionStageType,
+    },
+    total=False,
+)
+
+
+class TestFunctionRequestRequestTypeDef(
+    _RequiredTestFunctionRequestRequestTypeDef, _OptionalTestFunctionRequestRequestTypeDef
+):
+    pass
+
+
 _RequiredCachePolicyCookiesConfigOutputTypeDef = TypedDict(
     "_RequiredCachePolicyCookiesConfigOutputTypeDef",
     {
         "CookieBehavior": CachePolicyCookieBehaviorType,
     },
 )
 _OptionalCachePolicyCookiesConfigOutputTypeDef = TypedDict(
@@ -3117,25 +3130,25 @@
 )
 
 CreateFunctionRequestRequestTypeDef = TypedDict(
     "CreateFunctionRequestRequestTypeDef",
     {
         "Name": str,
         "FunctionConfig": FunctionConfigTypeDef,
-        "FunctionCode": Union[str, bytes, IO[Any], StreamingBody],
+        "FunctionCode": BlobTypeDef,
     },
 )
 
 UpdateFunctionRequestRequestTypeDef = TypedDict(
     "UpdateFunctionRequestRequestTypeDef",
     {
         "Name": str,
         "IfMatch": str,
         "FunctionConfig": FunctionConfigTypeDef,
-        "FunctionCode": Union[str, bytes, IO[Any], StreamingBody],
+        "FunctionCode": BlobTypeDef,
     },
 )
 
 CreateKeyGroupRequestRequestTypeDef = TypedDict(
     "CreateKeyGroupRequestRequestTypeDef",
     {
         "KeyGroupConfig": KeyGroupConfigTypeDef,
@@ -3621,14 +3634,15 @@
     {
         "KeyGroupConfig": KeyGroupConfigOutputTypeDef,
         "ETag": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+KeyGroupConfigUnionTypeDef = Union[KeyGroupConfigTypeDef, KeyGroupConfigOutputTypeDef]
 KeyGroupTypeDef = TypedDict(
     "KeyGroupTypeDef",
     {
         "Id": str,
         "LastModifiedTime": datetime,
         "KeyGroupConfig": KeyGroupConfigOutputTypeDef,
     },
@@ -4705,14 +4719,15 @@
     "CreateInvalidationRequestRequestTypeDef",
     {
         "DistributionId": str,
         "InvalidationBatch": InvalidationBatchTypeDef,
     },
 )
 
+InvalidationBatchUnionTypeDef = Union[InvalidationBatchTypeDef, InvalidationBatchOutputTypeDef]
 ListInvalidationsResultTypeDef = TypedDict(
     "ListInvalidationsResultTypeDef",
     {
         "InvalidationList": InvalidationListTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -4951,14 +4966,17 @@
 CreateStreamingDistributionRequestRequestTypeDef = TypedDict(
     "CreateStreamingDistributionRequestRequestTypeDef",
     {
         "StreamingDistributionConfig": StreamingDistributionConfigTypeDef,
     },
 )
 
+StreamingDistributionConfigUnionTypeDef = Union[
+    StreamingDistributionConfigTypeDef, StreamingDistributionConfigOutputTypeDef
+]
 _RequiredUpdateStreamingDistributionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateStreamingDistributionRequestRequestTypeDef",
     {
         "StreamingDistributionConfig": StreamingDistributionConfigTypeDef,
         "Id": str,
     },
 )
@@ -4998,14 +5016,15 @@
     "TagResourceRequestRequestTypeDef",
     {
         "Resource": str,
         "Tags": TagsTypeDef,
     },
 )
 
+TagsUnionTypeDef = Union[TagsTypeDef, TagsOutputTypeDef]
 _RequiredCacheBehaviorOutputTypeDef = TypedDict(
     "_RequiredCacheBehaviorOutputTypeDef",
     {
         "PathPattern": str,
         "TargetOriginId": str,
         "ViewerProtocolPolicy": ViewerProtocolPolicyType,
     },
@@ -5223,14 +5242,17 @@
 CreateOriginRequestPolicyRequestRequestTypeDef = TypedDict(
     "CreateOriginRequestPolicyRequestRequestTypeDef",
     {
         "OriginRequestPolicyConfig": OriginRequestPolicyConfigTypeDef,
     },
 )
 
+OriginRequestPolicyConfigUnionTypeDef = Union[
+    OriginRequestPolicyConfigTypeDef, OriginRequestPolicyConfigOutputTypeDef
+]
 _RequiredUpdateOriginRequestPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateOriginRequestPolicyRequestRequestTypeDef",
     {
         "OriginRequestPolicyConfig": OriginRequestPolicyConfigTypeDef,
         "Id": str,
     },
 )
@@ -5645,14 +5667,17 @@
 CreateResponseHeadersPolicyRequestRequestTypeDef = TypedDict(
     "CreateResponseHeadersPolicyRequestRequestTypeDef",
     {
         "ResponseHeadersPolicyConfig": ResponseHeadersPolicyConfigTypeDef,
     },
 )
 
+ResponseHeadersPolicyConfigUnionTypeDef = Union[
+    ResponseHeadersPolicyConfigTypeDef, ResponseHeadersPolicyConfigOutputTypeDef
+]
 _RequiredUpdateResponseHeadersPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateResponseHeadersPolicyRequestRequestTypeDef",
     {
         "ResponseHeadersPolicyConfig": ResponseHeadersPolicyConfigTypeDef,
         "Id": str,
     },
 )
@@ -5777,14 +5802,15 @@
     {
         "OriginRequestPolicy": OriginRequestPolicyTypeDef,
         "ETag": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+CachePolicyConfigUnionTypeDef = Union[CachePolicyConfigTypeDef, CachePolicyConfigOutputTypeDef]
 CreateCachePolicyRequestRequestTypeDef = TypedDict(
     "CreateCachePolicyRequestRequestTypeDef",
     {
         "CachePolicyConfig": CachePolicyConfigTypeDef,
     },
 )
 
@@ -5824,14 +5850,17 @@
     {
         "ContinuousDeploymentPolicyConfig": ContinuousDeploymentPolicyConfigOutputTypeDef,
         "ETag": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ContinuousDeploymentPolicyConfigUnionTypeDef = Union[
+    ContinuousDeploymentPolicyConfigTypeDef, ContinuousDeploymentPolicyConfigOutputTypeDef
+]
 CreateContinuousDeploymentPolicyRequestRequestTypeDef = TypedDict(
     "CreateContinuousDeploymentPolicyRequestRequestTypeDef",
     {
         "ContinuousDeploymentPolicyConfig": ContinuousDeploymentPolicyConfigTypeDef,
     },
 )
 
@@ -5902,14 +5931,17 @@
 CreateFieldLevelEncryptionProfileRequestRequestTypeDef = TypedDict(
     "CreateFieldLevelEncryptionProfileRequestRequestTypeDef",
     {
         "FieldLevelEncryptionProfileConfig": FieldLevelEncryptionProfileConfigTypeDef,
     },
 )
 
+FieldLevelEncryptionProfileConfigUnionTypeDef = Union[
+    FieldLevelEncryptionProfileConfigTypeDef, FieldLevelEncryptionProfileConfigOutputTypeDef
+]
 _RequiredUpdateFieldLevelEncryptionProfileRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFieldLevelEncryptionProfileRequestRequestTypeDef",
     {
         "FieldLevelEncryptionProfileConfig": FieldLevelEncryptionProfileConfigTypeDef,
         "Id": str,
     },
 )
@@ -6027,14 +6059,17 @@
 CreateFieldLevelEncryptionConfigRequestRequestTypeDef = TypedDict(
     "CreateFieldLevelEncryptionConfigRequestRequestTypeDef",
     {
         "FieldLevelEncryptionConfig": FieldLevelEncryptionConfigTypeDef,
     },
 )
 
+FieldLevelEncryptionConfigUnionTypeDef = Union[
+    FieldLevelEncryptionConfigTypeDef, FieldLevelEncryptionConfigOutputTypeDef
+]
 _RequiredUpdateFieldLevelEncryptionConfigRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFieldLevelEncryptionConfigRequestRequestTypeDef",
     {
         "FieldLevelEncryptionConfig": FieldLevelEncryptionConfigTypeDef,
         "Id": str,
     },
 )
@@ -6457,14 +6492,15 @@
 CreateDistributionRequestRequestTypeDef = TypedDict(
     "CreateDistributionRequestRequestTypeDef",
     {
         "DistributionConfig": DistributionConfigTypeDef,
     },
 )
 
+DistributionConfigUnionTypeDef = Union[DistributionConfigTypeDef, DistributionConfigOutputTypeDef]
 DistributionConfigWithTagsTypeDef = TypedDict(
     "DistributionConfigWithTagsTypeDef",
     {
         "DistributionConfig": DistributionConfigTypeDef,
         "Tags": TagsTypeDef,
     },
 )
```

### Comparing `mypy-boto3-cloudfront-1.28.15.post1/mypy_boto3_cloudfront/type_defs.pyi` & `mypy-boto3-cloudfront-1.28.16/mypy_boto3_cloudfront/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_cloudfront.type_defs import AliasICPRecordalTypeDef
 
-    data: AliasICPRecordalTypeDef = {...}
+    data: AliasICPRecordalTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -63,14 +63,15 @@
 __all__ = (
     "AliasICPRecordalTypeDef",
     "AliasesOutputTypeDef",
     "AliasesTypeDef",
     "CachedMethodsOutputTypeDef",
     "CachedMethodsTypeDef",
     "AssociateAliasRequestRequestTypeDef",
+    "BlobTypeDef",
     "TrustedKeyGroupsOutputTypeDef",
     "TrustedSignersOutputTypeDef",
     "TrustedKeyGroupsTypeDef",
     "TrustedSignersTypeDef",
     "CookieNamesOutputTypeDef",
     "CookieNamesTypeDef",
     "HeadersOutputTypeDef",
@@ -209,18 +210,18 @@
     "ResponseHeadersPolicyRemoveHeaderTypeDef",
     "ResponseHeadersPolicyStrictTransportSecurityTypeDef",
     "ResponseHeadersPolicyXSSProtectionTypeDef",
     "S3OriginTypeDef",
     "StreamingLoggingConfigTypeDef",
     "TagKeysTypeDef",
     "TagTypeDef",
-    "TestFunctionRequestRequestTypeDef",
     "UpdateDistributionWithStagingConfigRequestRequestTypeDef",
     "AllowedMethodsOutputTypeDef",
     "AllowedMethodsTypeDef",
+    "TestFunctionRequestRequestTypeDef",
     "CachePolicyCookiesConfigOutputTypeDef",
     "CookiePreferenceOutputTypeDef",
     "OriginRequestPolicyCookiesConfigOutputTypeDef",
     "CachePolicyCookiesConfigTypeDef",
     "CookiePreferenceTypeDef",
     "OriginRequestPolicyCookiesConfigTypeDef",
     "CachePolicyHeadersConfigOutputTypeDef",
@@ -272,14 +273,15 @@
     "FunctionSummaryTypeDef",
     "RestrictionsOutputTypeDef",
     "RestrictionsTypeDef",
     "GetDistributionRequestDistributionDeployedWaitTypeDef",
     "GetInvalidationRequestInvalidationCompletedWaitTypeDef",
     "GetStreamingDistributionRequestStreamingDistributionDeployedWaitTypeDef",
     "GetKeyGroupConfigResultTypeDef",
+    "KeyGroupConfigUnionTypeDef",
     "KeyGroupTypeDef",
     "InvalidationBatchOutputTypeDef",
     "InvalidationBatchTypeDef",
     "InvalidationListTypeDef",
     "KGKeyPairIdsTypeDef",
     "SignerTypeDef",
     "LambdaFunctionAssociationsOutputTypeDef",
@@ -345,14 +347,15 @@
     "UpdateFunctionResultTypeDef",
     "CreateKeyGroupResultTypeDef",
     "GetKeyGroupResultTypeDef",
     "KeyGroupSummaryTypeDef",
     "UpdateKeyGroupResultTypeDef",
     "InvalidationTypeDef",
     "CreateInvalidationRequestRequestTypeDef",
+    "InvalidationBatchUnionTypeDef",
     "ListInvalidationsResultTypeDef",
     "ActiveTrustedKeyGroupsTypeDef",
     "ActiveTrustedSignersTypeDef",
     "CreateMonitoringSubscriptionRequestRequestTypeDef",
     "CreateMonitoringSubscriptionResultTypeDef",
     "GetMonitoringSubscriptionResultTypeDef",
     "ListOriginAccessControlsResultTypeDef",
@@ -362,27 +365,30 @@
     "QueryArgProfileConfigOutputTypeDef",
     "QueryArgProfileConfigTypeDef",
     "ResponseHeadersPolicyConfigOutputTypeDef",
     "ResponseHeadersPolicyConfigTypeDef",
     "StreamingDistributionListTypeDef",
     "GetStreamingDistributionConfigResultTypeDef",
     "CreateStreamingDistributionRequestRequestTypeDef",
+    "StreamingDistributionConfigUnionTypeDef",
     "UpdateStreamingDistributionRequestRequestTypeDef",
     "ListTagsForResourceResultTypeDef",
     "StreamingDistributionConfigWithTagsTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "TagsUnionTypeDef",
     "CacheBehaviorOutputTypeDef",
     "DefaultCacheBehaviorOutputTypeDef",
     "CacheBehaviorTypeDef",
     "DefaultCacheBehaviorTypeDef",
     "CachePolicyConfigOutputTypeDef",
     "GetOriginRequestPolicyConfigResultTypeDef",
     "OriginRequestPolicyTypeDef",
     "CachePolicyConfigTypeDef",
     "CreateOriginRequestPolicyRequestRequestTypeDef",
+    "OriginRequestPolicyConfigUnionTypeDef",
     "UpdateOriginRequestPolicyRequestRequestTypeDef",
     "ContinuousDeploymentPolicyConfigOutputTypeDef",
     "ContinuousDeploymentPolicyConfigTypeDef",
     "OriginsOutputTypeDef",
     "OriginsTypeDef",
     "FieldLevelEncryptionProfileConfigOutputTypeDef",
     "FieldLevelEncryptionProfileSummaryTypeDef",
@@ -401,46 +407,51 @@
     "OriginGroupsTypeDef",
     "FieldLevelEncryptionConfigOutputTypeDef",
     "FieldLevelEncryptionSummaryTypeDef",
     "FieldLevelEncryptionConfigTypeDef",
     "GetResponseHeadersPolicyConfigResultTypeDef",
     "ResponseHeadersPolicyTypeDef",
     "CreateResponseHeadersPolicyRequestRequestTypeDef",
+    "ResponseHeadersPolicyConfigUnionTypeDef",
     "UpdateResponseHeadersPolicyRequestRequestTypeDef",
     "ListStreamingDistributionsResultTypeDef",
     "CreateStreamingDistributionWithTagsRequestRequestTypeDef",
     "CacheBehaviorsOutputTypeDef",
     "CacheBehaviorsTypeDef",
     "CachePolicyTypeDef",
     "GetCachePolicyConfigResultTypeDef",
     "CreateOriginRequestPolicyResultTypeDef",
     "GetOriginRequestPolicyResultTypeDef",
     "OriginRequestPolicySummaryTypeDef",
     "UpdateOriginRequestPolicyResultTypeDef",
+    "CachePolicyConfigUnionTypeDef",
     "CreateCachePolicyRequestRequestTypeDef",
     "UpdateCachePolicyRequestRequestTypeDef",
     "ContinuousDeploymentPolicyTypeDef",
     "GetContinuousDeploymentPolicyConfigResultTypeDef",
+    "ContinuousDeploymentPolicyConfigUnionTypeDef",
     "CreateContinuousDeploymentPolicyRequestRequestTypeDef",
     "UpdateContinuousDeploymentPolicyRequestRequestTypeDef",
     "FieldLevelEncryptionProfileTypeDef",
     "GetFieldLevelEncryptionProfileConfigResultTypeDef",
     "FieldLevelEncryptionProfileListTypeDef",
     "CreateFieldLevelEncryptionProfileRequestRequestTypeDef",
+    "FieldLevelEncryptionProfileConfigUnionTypeDef",
     "UpdateFieldLevelEncryptionProfileRequestRequestTypeDef",
     "ListRealtimeLogConfigsResultTypeDef",
     "ListKeyGroupsResultTypeDef",
     "CreateStreamingDistributionResultTypeDef",
     "CreateStreamingDistributionWithTagsResultTypeDef",
     "GetStreamingDistributionResultTypeDef",
     "UpdateStreamingDistributionResultTypeDef",
     "FieldLevelEncryptionTypeDef",
     "GetFieldLevelEncryptionConfigResultTypeDef",
     "FieldLevelEncryptionListTypeDef",
     "CreateFieldLevelEncryptionConfigRequestRequestTypeDef",
+    "FieldLevelEncryptionConfigUnionTypeDef",
     "UpdateFieldLevelEncryptionConfigRequestRequestTypeDef",
     "CreateResponseHeadersPolicyResultTypeDef",
     "GetResponseHeadersPolicyResultTypeDef",
     "ResponseHeadersPolicySummaryTypeDef",
     "UpdateResponseHeadersPolicyResultTypeDef",
     "DistributionConfigOutputTypeDef",
     "DistributionSummaryTypeDef",
@@ -463,14 +474,15 @@
     "UpdateFieldLevelEncryptionConfigResultTypeDef",
     "ListFieldLevelEncryptionConfigsResultTypeDef",
     "ResponseHeadersPolicyListTypeDef",
     "DistributionTypeDef",
     "GetDistributionConfigResultTypeDef",
     "DistributionListTypeDef",
     "CreateDistributionRequestRequestTypeDef",
+    "DistributionConfigUnionTypeDef",
     "DistributionConfigWithTagsTypeDef",
     "UpdateDistributionRequestRequestTypeDef",
     "CachePolicyListTypeDef",
     "ListOriginRequestPoliciesResultTypeDef",
     "ContinuousDeploymentPolicyListTypeDef",
     "ListResponseHeadersPoliciesResultTypeDef",
     "CopyDistributionResultTypeDef",
@@ -550,14 +562,15 @@
     "AssociateAliasRequestRequestTypeDef",
     {
         "TargetDistributionId": str,
         "Alias": str,
     },
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 _RequiredTrustedKeyGroupsOutputTypeDef = TypedDict(
     "_RequiredTrustedKeyGroupsOutputTypeDef",
     {
         "Enabled": bool,
         "Quantity": int,
     },
 )
@@ -2421,35 +2434,14 @@
     },
     total=False,
 )
 
 class TagTypeDef(_RequiredTagTypeDef, _OptionalTagTypeDef):
     pass
 
-_RequiredTestFunctionRequestRequestTypeDef = TypedDict(
-    "_RequiredTestFunctionRequestRequestTypeDef",
-    {
-        "Name": str,
-        "IfMatch": str,
-        "EventObject": Union[str, bytes, IO[Any], StreamingBody],
-    },
-)
-_OptionalTestFunctionRequestRequestTypeDef = TypedDict(
-    "_OptionalTestFunctionRequestRequestTypeDef",
-    {
-        "Stage": FunctionStageType,
-    },
-    total=False,
-)
-
-class TestFunctionRequestRequestTypeDef(
-    _RequiredTestFunctionRequestRequestTypeDef, _OptionalTestFunctionRequestRequestTypeDef
-):
-    pass
-
 _RequiredUpdateDistributionWithStagingConfigRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDistributionWithStagingConfigRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalUpdateDistributionWithStagingConfigRequestRequestTypeDef = TypedDict(
@@ -2501,14 +2493,35 @@
     },
     total=False,
 )
 
 class AllowedMethodsTypeDef(_RequiredAllowedMethodsTypeDef, _OptionalAllowedMethodsTypeDef):
     pass
 
+_RequiredTestFunctionRequestRequestTypeDef = TypedDict(
+    "_RequiredTestFunctionRequestRequestTypeDef",
+    {
+        "Name": str,
+        "IfMatch": str,
+        "EventObject": BlobTypeDef,
+    },
+)
+_OptionalTestFunctionRequestRequestTypeDef = TypedDict(
+    "_OptionalTestFunctionRequestRequestTypeDef",
+    {
+        "Stage": FunctionStageType,
+    },
+    total=False,
+)
+
+class TestFunctionRequestRequestTypeDef(
+    _RequiredTestFunctionRequestRequestTypeDef, _OptionalTestFunctionRequestRequestTypeDef
+):
+    pass
+
 _RequiredCachePolicyCookiesConfigOutputTypeDef = TypedDict(
     "_RequiredCachePolicyCookiesConfigOutputTypeDef",
     {
         "CookieBehavior": CachePolicyCookieBehaviorType,
     },
 )
 _OptionalCachePolicyCookiesConfigOutputTypeDef = TypedDict(
@@ -2944,25 +2957,25 @@
 )
 
 CreateFunctionRequestRequestTypeDef = TypedDict(
     "CreateFunctionRequestRequestTypeDef",
     {
         "Name": str,
         "FunctionConfig": FunctionConfigTypeDef,
-        "FunctionCode": Union[str, bytes, IO[Any], StreamingBody],
+        "FunctionCode": BlobTypeDef,
     },
 )
 
 UpdateFunctionRequestRequestTypeDef = TypedDict(
     "UpdateFunctionRequestRequestTypeDef",
     {
         "Name": str,
         "IfMatch": str,
         "FunctionConfig": FunctionConfigTypeDef,
-        "FunctionCode": Union[str, bytes, IO[Any], StreamingBody],
+        "FunctionCode": BlobTypeDef,
     },
 )
 
 CreateKeyGroupRequestRequestTypeDef = TypedDict(
     "CreateKeyGroupRequestRequestTypeDef",
     {
         "KeyGroupConfig": KeyGroupConfigTypeDef,
@@ -3414,14 +3427,15 @@
     {
         "KeyGroupConfig": KeyGroupConfigOutputTypeDef,
         "ETag": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+KeyGroupConfigUnionTypeDef = Union[KeyGroupConfigTypeDef, KeyGroupConfigOutputTypeDef]
 KeyGroupTypeDef = TypedDict(
     "KeyGroupTypeDef",
     {
         "Id": str,
         "LastModifiedTime": datetime,
         "KeyGroupConfig": KeyGroupConfigOutputTypeDef,
     },
@@ -4438,14 +4452,15 @@
     "CreateInvalidationRequestRequestTypeDef",
     {
         "DistributionId": str,
         "InvalidationBatch": InvalidationBatchTypeDef,
     },
 )
 
+InvalidationBatchUnionTypeDef = Union[InvalidationBatchTypeDef, InvalidationBatchOutputTypeDef]
 ListInvalidationsResultTypeDef = TypedDict(
     "ListInvalidationsResultTypeDef",
     {
         "InvalidationList": InvalidationListTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -4670,14 +4685,17 @@
 CreateStreamingDistributionRequestRequestTypeDef = TypedDict(
     "CreateStreamingDistributionRequestRequestTypeDef",
     {
         "StreamingDistributionConfig": StreamingDistributionConfigTypeDef,
     },
 )
 
+StreamingDistributionConfigUnionTypeDef = Union[
+    StreamingDistributionConfigTypeDef, StreamingDistributionConfigOutputTypeDef
+]
 _RequiredUpdateStreamingDistributionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateStreamingDistributionRequestRequestTypeDef",
     {
         "StreamingDistributionConfig": StreamingDistributionConfigTypeDef,
         "Id": str,
     },
 )
@@ -4715,14 +4733,15 @@
     "TagResourceRequestRequestTypeDef",
     {
         "Resource": str,
         "Tags": TagsTypeDef,
     },
 )
 
+TagsUnionTypeDef = Union[TagsTypeDef, TagsOutputTypeDef]
 _RequiredCacheBehaviorOutputTypeDef = TypedDict(
     "_RequiredCacheBehaviorOutputTypeDef",
     {
         "PathPattern": str,
         "TargetOriginId": str,
         "ViewerProtocolPolicy": ViewerProtocolPolicyType,
     },
@@ -4928,14 +4947,17 @@
 CreateOriginRequestPolicyRequestRequestTypeDef = TypedDict(
     "CreateOriginRequestPolicyRequestRequestTypeDef",
     {
         "OriginRequestPolicyConfig": OriginRequestPolicyConfigTypeDef,
     },
 )
 
+OriginRequestPolicyConfigUnionTypeDef = Union[
+    OriginRequestPolicyConfigTypeDef, OriginRequestPolicyConfigOutputTypeDef
+]
 _RequiredUpdateOriginRequestPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateOriginRequestPolicyRequestRequestTypeDef",
     {
         "OriginRequestPolicyConfig": OriginRequestPolicyConfigTypeDef,
         "Id": str,
     },
 )
@@ -5322,14 +5344,17 @@
 CreateResponseHeadersPolicyRequestRequestTypeDef = TypedDict(
     "CreateResponseHeadersPolicyRequestRequestTypeDef",
     {
         "ResponseHeadersPolicyConfig": ResponseHeadersPolicyConfigTypeDef,
     },
 )
 
+ResponseHeadersPolicyConfigUnionTypeDef = Union[
+    ResponseHeadersPolicyConfigTypeDef, ResponseHeadersPolicyConfigOutputTypeDef
+]
 _RequiredUpdateResponseHeadersPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateResponseHeadersPolicyRequestRequestTypeDef",
     {
         "ResponseHeadersPolicyConfig": ResponseHeadersPolicyConfigTypeDef,
         "Id": str,
     },
 )
@@ -5448,14 +5473,15 @@
     {
         "OriginRequestPolicy": OriginRequestPolicyTypeDef,
         "ETag": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+CachePolicyConfigUnionTypeDef = Union[CachePolicyConfigTypeDef, CachePolicyConfigOutputTypeDef]
 CreateCachePolicyRequestRequestTypeDef = TypedDict(
     "CreateCachePolicyRequestRequestTypeDef",
     {
         "CachePolicyConfig": CachePolicyConfigTypeDef,
     },
 )
 
@@ -5493,14 +5519,17 @@
     {
         "ContinuousDeploymentPolicyConfig": ContinuousDeploymentPolicyConfigOutputTypeDef,
         "ETag": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ContinuousDeploymentPolicyConfigUnionTypeDef = Union[
+    ContinuousDeploymentPolicyConfigTypeDef, ContinuousDeploymentPolicyConfigOutputTypeDef
+]
 CreateContinuousDeploymentPolicyRequestRequestTypeDef = TypedDict(
     "CreateContinuousDeploymentPolicyRequestRequestTypeDef",
     {
         "ContinuousDeploymentPolicyConfig": ContinuousDeploymentPolicyConfigTypeDef,
     },
 )
 
@@ -5567,14 +5596,17 @@
 CreateFieldLevelEncryptionProfileRequestRequestTypeDef = TypedDict(
     "CreateFieldLevelEncryptionProfileRequestRequestTypeDef",
     {
         "FieldLevelEncryptionProfileConfig": FieldLevelEncryptionProfileConfigTypeDef,
     },
 )
 
+FieldLevelEncryptionProfileConfigUnionTypeDef = Union[
+    FieldLevelEncryptionProfileConfigTypeDef, FieldLevelEncryptionProfileConfigOutputTypeDef
+]
 _RequiredUpdateFieldLevelEncryptionProfileRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFieldLevelEncryptionProfileRequestRequestTypeDef",
     {
         "FieldLevelEncryptionProfileConfig": FieldLevelEncryptionProfileConfigTypeDef,
         "Id": str,
     },
 )
@@ -5688,14 +5720,17 @@
 CreateFieldLevelEncryptionConfigRequestRequestTypeDef = TypedDict(
     "CreateFieldLevelEncryptionConfigRequestRequestTypeDef",
     {
         "FieldLevelEncryptionConfig": FieldLevelEncryptionConfigTypeDef,
     },
 )
 
+FieldLevelEncryptionConfigUnionTypeDef = Union[
+    FieldLevelEncryptionConfigTypeDef, FieldLevelEncryptionConfigOutputTypeDef
+]
 _RequiredUpdateFieldLevelEncryptionConfigRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFieldLevelEncryptionConfigRequestRequestTypeDef",
     {
         "FieldLevelEncryptionConfig": FieldLevelEncryptionConfigTypeDef,
         "Id": str,
     },
 )
@@ -6102,14 +6137,15 @@
 CreateDistributionRequestRequestTypeDef = TypedDict(
     "CreateDistributionRequestRequestTypeDef",
     {
         "DistributionConfig": DistributionConfigTypeDef,
     },
 )
 
+DistributionConfigUnionTypeDef = Union[DistributionConfigTypeDef, DistributionConfigOutputTypeDef]
 DistributionConfigWithTagsTypeDef = TypedDict(
     "DistributionConfigWithTagsTypeDef",
     {
         "DistributionConfig": DistributionConfigTypeDef,
         "Tags": TagsTypeDef,
     },
 )
```

### Comparing `mypy-boto3-cloudfront-1.28.15.post1/mypy_boto3_cloudfront/waiter.py` & `mypy-boto3-cloudfront-1.28.16/mypy_boto3_cloudfront/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudfront-1.28.15.post1/mypy_boto3_cloudfront/waiter.pyi` & `mypy-boto3-cloudfront-1.28.16/mypy_boto3_cloudfront/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudfront-1.28.15.post1/mypy_boto3_cloudfront.egg-info/PKG-INFO` & `mypy-boto3-cloudfront-1.28.16/mypy_boto3_cloudfront.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cloudfront
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.CloudFront 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.CloudFront 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 cloudfront type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 cloudfront type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudfront.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudfront)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cloudfront)](https://pepy.tech/project/mypy-boto3-cloudfront)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudFront 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront)
+[boto3.CloudFront 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront)
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
 [mypy-boto3-cloudfront docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/).
 
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
@@ -397,29 +397,30 @@
 )
 
 
 def check_value(value: CachePolicyCookieBehaviorType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_cloudfront.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_cloudfront.type_defs import (
     AliasICPRecordalTypeDef,
     AliasesOutputTypeDef,
     AliasesTypeDef,
     CachedMethodsOutputTypeDef,
     CachedMethodsTypeDef,
     AssociateAliasRequestRequestTypeDef,
+    BlobTypeDef,
     TrustedKeyGroupsOutputTypeDef,
     TrustedSignersOutputTypeDef,
     TrustedKeyGroupsTypeDef,
     TrustedSignersTypeDef,
     CookieNamesOutputTypeDef,
     CookieNamesTypeDef,
     HeadersOutputTypeDef,
@@ -558,18 +559,18 @@
     ResponseHeadersPolicyRemoveHeaderTypeDef,
     ResponseHeadersPolicyStrictTransportSecurityTypeDef,
     ResponseHeadersPolicyXSSProtectionTypeDef,
     S3OriginTypeDef,
     StreamingLoggingConfigTypeDef,
     TagKeysTypeDef,
     TagTypeDef,
-    TestFunctionRequestRequestTypeDef,
     UpdateDistributionWithStagingConfigRequestRequestTypeDef,
     AllowedMethodsOutputTypeDef,
     AllowedMethodsTypeDef,
+    TestFunctionRequestRequestTypeDef,
     CachePolicyCookiesConfigOutputTypeDef,
     CookiePreferenceOutputTypeDef,
     OriginRequestPolicyCookiesConfigOutputTypeDef,
     CachePolicyCookiesConfigTypeDef,
     CookiePreferenceTypeDef,
     OriginRequestPolicyCookiesConfigTypeDef,
     CachePolicyHeadersConfigOutputTypeDef,
@@ -621,14 +622,15 @@
     FunctionSummaryTypeDef,
     RestrictionsOutputTypeDef,
     RestrictionsTypeDef,
     GetDistributionRequestDistributionDeployedWaitTypeDef,
     GetInvalidationRequestInvalidationCompletedWaitTypeDef,
     GetStreamingDistributionRequestStreamingDistributionDeployedWaitTypeDef,
     GetKeyGroupConfigResultTypeDef,
+    KeyGroupConfigUnionTypeDef,
     KeyGroupTypeDef,
     InvalidationBatchOutputTypeDef,
     InvalidationBatchTypeDef,
     InvalidationListTypeDef,
     KGKeyPairIdsTypeDef,
     SignerTypeDef,
     LambdaFunctionAssociationsOutputTypeDef,
@@ -694,14 +696,15 @@
     UpdateFunctionResultTypeDef,
     CreateKeyGroupResultTypeDef,
     GetKeyGroupResultTypeDef,
     KeyGroupSummaryTypeDef,
     UpdateKeyGroupResultTypeDef,
     InvalidationTypeDef,
     CreateInvalidationRequestRequestTypeDef,
+    InvalidationBatchUnionTypeDef,
     ListInvalidationsResultTypeDef,
     ActiveTrustedKeyGroupsTypeDef,
     ActiveTrustedSignersTypeDef,
     CreateMonitoringSubscriptionRequestRequestTypeDef,
     CreateMonitoringSubscriptionResultTypeDef,
     GetMonitoringSubscriptionResultTypeDef,
     ListOriginAccessControlsResultTypeDef,
@@ -711,27 +714,30 @@
     QueryArgProfileConfigOutputTypeDef,
     QueryArgProfileConfigTypeDef,
     ResponseHeadersPolicyConfigOutputTypeDef,
     ResponseHeadersPolicyConfigTypeDef,
     StreamingDistributionListTypeDef,
     GetStreamingDistributionConfigResultTypeDef,
     CreateStreamingDistributionRequestRequestTypeDef,
+    StreamingDistributionConfigUnionTypeDef,
     UpdateStreamingDistributionRequestRequestTypeDef,
     ListTagsForResourceResultTypeDef,
     StreamingDistributionConfigWithTagsTypeDef,
     TagResourceRequestRequestTypeDef,
+    TagsUnionTypeDef,
     CacheBehaviorOutputTypeDef,
     DefaultCacheBehaviorOutputTypeDef,
     CacheBehaviorTypeDef,
     DefaultCacheBehaviorTypeDef,
     CachePolicyConfigOutputTypeDef,
     GetOriginRequestPolicyConfigResultTypeDef,
     OriginRequestPolicyTypeDef,
     CachePolicyConfigTypeDef,
     CreateOriginRequestPolicyRequestRequestTypeDef,
+    OriginRequestPolicyConfigUnionTypeDef,
     UpdateOriginRequestPolicyRequestRequestTypeDef,
     ContinuousDeploymentPolicyConfigOutputTypeDef,
     ContinuousDeploymentPolicyConfigTypeDef,
     OriginsOutputTypeDef,
     OriginsTypeDef,
     FieldLevelEncryptionProfileConfigOutputTypeDef,
     FieldLevelEncryptionProfileSummaryTypeDef,
@@ -750,46 +756,51 @@
     OriginGroupsTypeDef,
     FieldLevelEncryptionConfigOutputTypeDef,
     FieldLevelEncryptionSummaryTypeDef,
     FieldLevelEncryptionConfigTypeDef,
     GetResponseHeadersPolicyConfigResultTypeDef,
     ResponseHeadersPolicyTypeDef,
     CreateResponseHeadersPolicyRequestRequestTypeDef,
+    ResponseHeadersPolicyConfigUnionTypeDef,
     UpdateResponseHeadersPolicyRequestRequestTypeDef,
     ListStreamingDistributionsResultTypeDef,
     CreateStreamingDistributionWithTagsRequestRequestTypeDef,
     CacheBehaviorsOutputTypeDef,
     CacheBehaviorsTypeDef,
     CachePolicyTypeDef,
     GetCachePolicyConfigResultTypeDef,
     CreateOriginRequestPolicyResultTypeDef,
     GetOriginRequestPolicyResultTypeDef,
     OriginRequestPolicySummaryTypeDef,
     UpdateOriginRequestPolicyResultTypeDef,
+    CachePolicyConfigUnionTypeDef,
     CreateCachePolicyRequestRequestTypeDef,
     UpdateCachePolicyRequestRequestTypeDef,
     ContinuousDeploymentPolicyTypeDef,
     GetContinuousDeploymentPolicyConfigResultTypeDef,
+    ContinuousDeploymentPolicyConfigUnionTypeDef,
     CreateContinuousDeploymentPolicyRequestRequestTypeDef,
     UpdateContinuousDeploymentPolicyRequestRequestTypeDef,
     FieldLevelEncryptionProfileTypeDef,
     GetFieldLevelEncryptionProfileConfigResultTypeDef,
     FieldLevelEncryptionProfileListTypeDef,
     CreateFieldLevelEncryptionProfileRequestRequestTypeDef,
+    FieldLevelEncryptionProfileConfigUnionTypeDef,
     UpdateFieldLevelEncryptionProfileRequestRequestTypeDef,
     ListRealtimeLogConfigsResultTypeDef,
     ListKeyGroupsResultTypeDef,
     CreateStreamingDistributionResultTypeDef,
     CreateStreamingDistributionWithTagsResultTypeDef,
     GetStreamingDistributionResultTypeDef,
     UpdateStreamingDistributionResultTypeDef,
     FieldLevelEncryptionTypeDef,
     GetFieldLevelEncryptionConfigResultTypeDef,
     FieldLevelEncryptionListTypeDef,
     CreateFieldLevelEncryptionConfigRequestRequestTypeDef,
+    FieldLevelEncryptionConfigUnionTypeDef,
     UpdateFieldLevelEncryptionConfigRequestRequestTypeDef,
     CreateResponseHeadersPolicyResultTypeDef,
     GetResponseHeadersPolicyResultTypeDef,
     ResponseHeadersPolicySummaryTypeDef,
     UpdateResponseHeadersPolicyResultTypeDef,
     DistributionConfigOutputTypeDef,
     DistributionSummaryTypeDef,
@@ -812,14 +823,15 @@
     UpdateFieldLevelEncryptionConfigResultTypeDef,
     ListFieldLevelEncryptionConfigsResultTypeDef,
     ResponseHeadersPolicyListTypeDef,
     DistributionTypeDef,
     GetDistributionConfigResultTypeDef,
     DistributionListTypeDef,
     CreateDistributionRequestRequestTypeDef,
+    DistributionConfigUnionTypeDef,
     DistributionConfigWithTagsTypeDef,
     UpdateDistributionRequestRequestTypeDef,
     CachePolicyListTypeDef,
     ListOriginRequestPoliciesResultTypeDef,
     ContinuousDeploymentPolicyListTypeDef,
     ListResponseHeadersPoliciesResultTypeDef,
     CopyDistributionResultTypeDef,
@@ -833,15 +845,15 @@
     ListDistributionsResultTypeDef,
     CreateDistributionWithTagsRequestRequestTypeDef,
     ListCachePoliciesResultTypeDef,
     ListContinuousDeploymentPoliciesResultTypeDef,
 )
 
 
-def get_structure() -> AliasICPRecordalTypeDef:
+def get_value() -> AliasICPRecordalTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-cloudfront-1.28.15.post1/mypy_boto3_cloudfront.egg-info/SOURCES.txt` & `mypy-boto3-cloudfront-1.28.16/mypy_boto3_cloudfront.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudfront-1.28.15.post1/setup.py` & `mypy-boto3-cloudfront-1.28.16/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-cloudfront",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_cloudfront"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CloudFront 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.2"
+        "Type annotations for boto3.CloudFront 1.28.16 service generated with mypy-boto3-builder"
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
-    keywords="boto3 cloudfront type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 cloudfront type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_cloudfront": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

