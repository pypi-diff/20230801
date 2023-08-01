# Comparing `tmp/mypy-boto3-wafv2-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-wafv2-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-wafv2-1.28.15.post1.tar", last modified: Sat Jul 29 10:04:25 2023, max compression
+gzip compressed data, was "mypy-boto3-wafv2-1.28.16.tar", last modified: Tue Aug  1 11:38:04 2023, max compression
```

## Comparing `mypy-boto3-wafv2-1.28.15.post1.tar` & `mypy-boto3-wafv2-1.28.16.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:25.709456 mypy-boto3-wafv2-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 10:01:27.000000 mypy-boto3-wafv2-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21725 2023-07-29 10:04:25.709456 mypy-boto3-wafv2-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20240 2023-07-29 10:01:27.000000 mypy-boto3-wafv2-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:25.701456 mypy-boto3-wafv2-1.28.15.post1/mypy_boto3_wafv2/
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-29 10:01:27.000000 mypy-boto3-wafv2-1.28.15.post1/mypy_boto3_wafv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-29 10:01:27.000000 mypy-boto3-wafv2-1.28.15.post1/mypy_boto3_wafv2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-29 10:01:27.000000 mypy-boto3-wafv2-1.28.15.post1/mypy_boto3_wafv2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37420 2023-07-29 10:01:27.000000 mypy-boto3-wafv2-1.28.15.post1/mypy_boto3_wafv2/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    37361 2023-07-29 10:01:27.000000 mypy-boto3-wafv2-1.28.15.post1/mypy_boto3_wafv2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13531 2023-07-29 10:01:28.000000 mypy-boto3-wafv2-1.28.15.post1/mypy_boto3_wafv2/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13529 2023-07-29 10:01:27.000000 mypy-boto3-wafv2-1.28.15.post1/mypy_boto3_wafv2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 10:01:27.000000 mypy-boto3-wafv2-1.28.15.post1/mypy_boto3_wafv2/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    87884 2023-07-29 10:01:35.000000 mypy-boto3-wafv2-1.28.15.post1/mypy_boto3_wafv2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    87781 2023-07-29 10:01:33.000000 mypy-boto3-wafv2-1.28.15.post1/mypy_boto3_wafv2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 10:01:27.000000 mypy-boto3-wafv2-1.28.15.post1/mypy_boto3_wafv2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:25.709456 mypy-boto3-wafv2-1.28.15.post1/mypy_boto3_wafv2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21725 2023-07-29 10:04:25.000000 mypy-boto3-wafv2-1.28.15.post1/mypy_boto3_wafv2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-29 10:04:25.000000 mypy-boto3-wafv2-1.28.15.post1/mypy_boto3_wafv2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:25.000000 mypy-boto3-wafv2-1.28.15.post1/mypy_boto3_wafv2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:25.000000 mypy-boto3-wafv2-1.28.15.post1/mypy_boto3_wafv2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:04:25.000000 mypy-boto3-wafv2-1.28.15.post1/mypy_boto3_wafv2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-29 10:04:25.000000 mypy-boto3-wafv2-1.28.15.post1/mypy_boto3_wafv2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:04:25.709456 mypy-boto3-wafv2-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-07-29 10:01:27.000000 mypy-boto3-wafv2-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:38:04.512667 mypy-boto3-wafv2-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:35:07.000000 mypy-boto3-wafv2-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21908 2023-08-01 11:38:04.500667 mypy-boto3-wafv2-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20432 2023-08-01 11:35:07.000000 mypy-boto3-wafv2-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:38:04.500667 mypy-boto3-wafv2-1.28.16/mypy_boto3_wafv2/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-08-01 11:35:07.000000 mypy-boto3-wafv2-1.28.16/mypy_boto3_wafv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-08-01 11:35:07.000000 mypy-boto3-wafv2-1.28.16/mypy_boto3_wafv2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-08-01 11:35:07.000000 mypy-boto3-wafv2-1.28.16/mypy_boto3_wafv2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36954 2023-08-01 11:35:12.000000 mypy-boto3-wafv2-1.28.16/mypy_boto3_wafv2/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36895 2023-08-01 11:35:12.000000 mypy-boto3-wafv2-1.28.16/mypy_boto3_wafv2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13531 2023-08-01 11:35:12.000000 mypy-boto3-wafv2-1.28.16/mypy_boto3_wafv2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13529 2023-08-01 11:35:12.000000 mypy-boto3-wafv2-1.28.16/mypy_boto3_wafv2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:35:07.000000 mypy-boto3-wafv2-1.28.16/mypy_boto3_wafv2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    88455 2023-08-01 11:35:15.000000 mypy-boto3-wafv2-1.28.16/mypy_boto3_wafv2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    88352 2023-08-01 11:35:13.000000 mypy-boto3-wafv2-1.28.16/mypy_boto3_wafv2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:35:07.000000 mypy-boto3-wafv2-1.28.16/mypy_boto3_wafv2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:38:04.500667 mypy-boto3-wafv2-1.28.16/mypy_boto3_wafv2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21908 2023-08-01 11:38:04.000000 mypy-boto3-wafv2-1.28.16/mypy_boto3_wafv2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-08-01 11:38:04.000000 mypy-boto3-wafv2-1.28.16/mypy_boto3_wafv2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:38:04.000000 mypy-boto3-wafv2-1.28.16/mypy_boto3_wafv2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:38:04.000000 mypy-boto3-wafv2-1.28.16/mypy_boto3_wafv2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:38:04.000000 mypy-boto3-wafv2-1.28.16/mypy_boto3_wafv2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-01 11:38:04.000000 mypy-boto3-wafv2-1.28.16/mypy_boto3_wafv2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:38:04.512667 mypy-boto3-wafv2-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-08-01 11:35:07.000000 mypy-boto3-wafv2-1.28.16/setup.py
```

### Comparing `mypy-boto3-wafv2-1.28.15.post1/LICENSE` & `mypy-boto3-wafv2-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-wafv2-1.28.15.post1/PKG-INFO` & `mypy-boto3-wafv2-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-wafv2
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.WAFV2 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.WAFV2 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 wafv2 type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 wafv2 type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-wafv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-wafv2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-wafv2)](https://pepy.tech/project/mypy-boto3-wafv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WAFV2 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2)
+[boto3.WAFV2 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2)
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
 [mypy-boto3-wafv2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -73,15 +73,15 @@
     - [Sublime Text](#sublime-text)
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
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
@@ -312,31 +312,32 @@
 )
 
 
 def check_value(value: ActionValueType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_wafv2.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_wafv2.type_defs import (
     APIKeySummaryTypeDef,
     AWSManagedRulesBotControlRuleSetTypeDef,
     ActionConditionTypeDef,
     AddressFieldTypeDef,
     AndStatementOutputTypeDef,
     AndStatementTypeDef,
     AssociateWebACLRequestRequestTypeDef,
     RequestBodyAssociatedResourceTypeConfigTypeDef,
+    BlobTypeDef,
     BodyTypeDef,
     TextTransformationTypeDef,
     ImmunityTimePropertyTypeDef,
     CaptchaResponseTypeDef,
     ChallengeResponseTypeDef,
     ResponseMetadataTypeDef,
     LabelNameConditionTypeDef,
@@ -379,15 +380,14 @@
     GetManagedRuleSetRequestRequestTypeDef,
     GetMobileSdkReleaseRequestRequestTypeDef,
     GetPermissionPolicyRequestRequestTypeDef,
     GetRateBasedStatementManagedKeysRequestRequestTypeDef,
     RateBasedStatementManagedKeysIPSetTypeDef,
     GetRegexPatternSetRequestRequestTypeDef,
     GetRuleGroupRequestRequestTypeDef,
-    TimeWindowTypeDef,
     TimeWindowOutputTypeDef,
     GetWebACLForResourceRequestRequestTypeDef,
     GetWebACLRequestRequestTypeDef,
     HTTPHeaderTypeDef,
     HeaderMatchPatternOutputTypeDef,
     HeaderMatchPatternTypeDef,
     IPSetForwardedIPConfigTypeDef,
@@ -425,17 +425,17 @@
     ResponseInspectionBodyContainsTypeDef,
     ResponseInspectionHeaderOutputTypeDef,
     ResponseInspectionHeaderTypeDef,
     ResponseInspectionJsonOutputTypeDef,
     ResponseInspectionJsonTypeDef,
     ResponseInspectionStatusCodeOutputTypeDef,
     ResponseInspectionStatusCodeTypeDef,
+    TimestampTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateIPSetRequestRequestTypeDef,
-    UpdateManagedRuleSetVersionExpiryDateRequestRequestTypeDef,
     AssociationConfigOutputTypeDef,
     AssociationConfigTypeDef,
     RateLimitCookieOutputTypeDef,
     RateLimitCookieTypeDef,
     RateLimitHeaderOutputTypeDef,
     RateLimitHeaderTypeDef,
     RateLimitQueryArgumentOutputTypeDef,
@@ -484,15 +484,14 @@
     CustomResponseTypeDef,
     DescribeAllManagedProductsResponseTypeDef,
     DescribeManagedProductsByVendorResponseTypeDef,
     GeoMatchStatementOutputTypeDef,
     GeoMatchStatementTypeDef,
     GetIPSetResponseTypeDef,
     GetRateBasedStatementManagedKeysResponseTypeDef,
-    GetSampledRequestsRequestRequestTypeDef,
     HTTPRequestTypeDef,
     HeadersOutputTypeDef,
     HeadersTypeDef,
     IPSetReferenceStatementTypeDef,
     JsonBodyOutputTypeDef,
     JsonBodyTypeDef,
     ListAvailableManagedRuleGroupVersionsResponseTypeDef,
@@ -502,14 +501,17 @@
     RequestInspectionTypeDef,
     ManagedRuleSetTypeDef,
     RequestInspectionACFPOutputTypeDef,
     RequestInspectionACFPTypeDef,
     PutManagedRuleSetVersionsRequestRequestTypeDef,
     ResponseInspectionOutputTypeDef,
     ResponseInspectionTypeDef,
+    TimeWindowTypeDef,
+    UpdateManagedRuleSetVersionExpiryDateRequestRequestTypeDef,
+    AssociationConfigUnionTypeDef,
     RateBasedStatementCustomKeyOutputTypeDef,
     RateBasedStatementCustomKeyTypeDef,
     FilterOutputTypeDef,
     FilterTypeDef,
     GetMobileSdkReleaseResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     GetRegexPatternSetResponseTypeDef,
@@ -527,14 +529,16 @@
     FieldToMatchOutputTypeDef,
     FieldToMatchTypeDef,
     GetManagedRuleSetResponseTypeDef,
     AWSManagedRulesACFPRuleSetOutputTypeDef,
     AWSManagedRulesATPRuleSetOutputTypeDef,
     AWSManagedRulesACFPRuleSetTypeDef,
     AWSManagedRulesATPRuleSetTypeDef,
+    GetSampledRequestsRequestRequestTypeDef,
+    TimeWindowUnionTypeDef,
     RateBasedStatementOutputTypeDef,
     RateBasedStatementTypeDef,
     LoggingFilterOutputTypeDef,
     LoggingFilterTypeDef,
     OverrideActionOutputTypeDef,
     OverrideActionTypeDef,
     DefaultActionOutputTypeDef,
@@ -557,43 +561,46 @@
     ManagedRuleGroupConfigOutputTypeDef,
     ManagedRuleGroupConfigTypeDef,
     LoggingConfigurationOutputTypeDef,
     LoggingConfigurationTypeDef,
     RuleActionOverrideOutputTypeDef,
     RuleOutputTypeDef,
     RuleSummaryTypeDef,
+    DefaultActionUnionTypeDef,
     RuleActionOverrideTypeDef,
     RuleTypeDef,
     GetLoggingConfigurationResponseTypeDef,
     ListLoggingConfigurationsResponseTypeDef,
     PutLoggingConfigurationResponseTypeDef,
+    LoggingConfigurationUnionTypeDef,
     PutLoggingConfigurationRequestRequestTypeDef,
     ManagedRuleGroupStatementOutputTypeDef,
     RuleGroupReferenceStatementOutputTypeDef,
     RuleGroupTypeDef,
     DescribeManagedRuleGroupResponseTypeDef,
     ManagedRuleGroupStatementTypeDef,
     RuleGroupReferenceStatementTypeDef,
+    RuleUnionTypeDef,
+    FirewallManagerStatementTypeDef,
+    StatementOutputTypeDef,
+    GetRuleGroupResponseTypeDef,
+    StatementTypeDef,
     CheckCapacityRequestRequestTypeDef,
     CreateRuleGroupRequestRequestTypeDef,
     CreateWebACLRequestRequestTypeDef,
     UpdateRuleGroupRequestRequestTypeDef,
     UpdateWebACLRequestRequestTypeDef,
-    FirewallManagerStatementTypeDef,
-    StatementOutputTypeDef,
-    GetRuleGroupResponseTypeDef,
-    StatementTypeDef,
     FirewallManagerRuleGroupTypeDef,
     WebACLTypeDef,
     GetWebACLForResourceResponseTypeDef,
     GetWebACLResponseTypeDef,
 )
 
 
-def get_structure() -> APIKeySummaryTypeDef:
+def get_value() -> APIKeySummaryTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-wafv2-1.28.15.post1/README.md` & `mypy-boto3-wafv2-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-wafv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-wafv2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-wafv2)](https://pepy.tech/project/mypy-boto3-wafv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WAFV2 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2)
+[boto3.WAFV2 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2)
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
 [mypy-boto3-wafv2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -41,15 +41,15 @@
     - [Sublime Text](#sublime-text)
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
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
@@ -280,31 +280,32 @@
 )
 
 
 def check_value(value: ActionValueType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_wafv2.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_wafv2.type_defs import (
     APIKeySummaryTypeDef,
     AWSManagedRulesBotControlRuleSetTypeDef,
     ActionConditionTypeDef,
     AddressFieldTypeDef,
     AndStatementOutputTypeDef,
     AndStatementTypeDef,
     AssociateWebACLRequestRequestTypeDef,
     RequestBodyAssociatedResourceTypeConfigTypeDef,
+    BlobTypeDef,
     BodyTypeDef,
     TextTransformationTypeDef,
     ImmunityTimePropertyTypeDef,
     CaptchaResponseTypeDef,
     ChallengeResponseTypeDef,
     ResponseMetadataTypeDef,
     LabelNameConditionTypeDef,
@@ -347,15 +348,14 @@
     GetManagedRuleSetRequestRequestTypeDef,
     GetMobileSdkReleaseRequestRequestTypeDef,
     GetPermissionPolicyRequestRequestTypeDef,
     GetRateBasedStatementManagedKeysRequestRequestTypeDef,
     RateBasedStatementManagedKeysIPSetTypeDef,
     GetRegexPatternSetRequestRequestTypeDef,
     GetRuleGroupRequestRequestTypeDef,
-    TimeWindowTypeDef,
     TimeWindowOutputTypeDef,
     GetWebACLForResourceRequestRequestTypeDef,
     GetWebACLRequestRequestTypeDef,
     HTTPHeaderTypeDef,
     HeaderMatchPatternOutputTypeDef,
     HeaderMatchPatternTypeDef,
     IPSetForwardedIPConfigTypeDef,
@@ -393,17 +393,17 @@
     ResponseInspectionBodyContainsTypeDef,
     ResponseInspectionHeaderOutputTypeDef,
     ResponseInspectionHeaderTypeDef,
     ResponseInspectionJsonOutputTypeDef,
     ResponseInspectionJsonTypeDef,
     ResponseInspectionStatusCodeOutputTypeDef,
     ResponseInspectionStatusCodeTypeDef,
+    TimestampTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateIPSetRequestRequestTypeDef,
-    UpdateManagedRuleSetVersionExpiryDateRequestRequestTypeDef,
     AssociationConfigOutputTypeDef,
     AssociationConfigTypeDef,
     RateLimitCookieOutputTypeDef,
     RateLimitCookieTypeDef,
     RateLimitHeaderOutputTypeDef,
     RateLimitHeaderTypeDef,
     RateLimitQueryArgumentOutputTypeDef,
@@ -452,15 +452,14 @@
     CustomResponseTypeDef,
     DescribeAllManagedProductsResponseTypeDef,
     DescribeManagedProductsByVendorResponseTypeDef,
     GeoMatchStatementOutputTypeDef,
     GeoMatchStatementTypeDef,
     GetIPSetResponseTypeDef,
     GetRateBasedStatementManagedKeysResponseTypeDef,
-    GetSampledRequestsRequestRequestTypeDef,
     HTTPRequestTypeDef,
     HeadersOutputTypeDef,
     HeadersTypeDef,
     IPSetReferenceStatementTypeDef,
     JsonBodyOutputTypeDef,
     JsonBodyTypeDef,
     ListAvailableManagedRuleGroupVersionsResponseTypeDef,
@@ -470,14 +469,17 @@
     RequestInspectionTypeDef,
     ManagedRuleSetTypeDef,
     RequestInspectionACFPOutputTypeDef,
     RequestInspectionACFPTypeDef,
     PutManagedRuleSetVersionsRequestRequestTypeDef,
     ResponseInspectionOutputTypeDef,
     ResponseInspectionTypeDef,
+    TimeWindowTypeDef,
+    UpdateManagedRuleSetVersionExpiryDateRequestRequestTypeDef,
+    AssociationConfigUnionTypeDef,
     RateBasedStatementCustomKeyOutputTypeDef,
     RateBasedStatementCustomKeyTypeDef,
     FilterOutputTypeDef,
     FilterTypeDef,
     GetMobileSdkReleaseResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     GetRegexPatternSetResponseTypeDef,
@@ -495,14 +497,16 @@
     FieldToMatchOutputTypeDef,
     FieldToMatchTypeDef,
     GetManagedRuleSetResponseTypeDef,
     AWSManagedRulesACFPRuleSetOutputTypeDef,
     AWSManagedRulesATPRuleSetOutputTypeDef,
     AWSManagedRulesACFPRuleSetTypeDef,
     AWSManagedRulesATPRuleSetTypeDef,
+    GetSampledRequestsRequestRequestTypeDef,
+    TimeWindowUnionTypeDef,
     RateBasedStatementOutputTypeDef,
     RateBasedStatementTypeDef,
     LoggingFilterOutputTypeDef,
     LoggingFilterTypeDef,
     OverrideActionOutputTypeDef,
     OverrideActionTypeDef,
     DefaultActionOutputTypeDef,
@@ -525,43 +529,46 @@
     ManagedRuleGroupConfigOutputTypeDef,
     ManagedRuleGroupConfigTypeDef,
     LoggingConfigurationOutputTypeDef,
     LoggingConfigurationTypeDef,
     RuleActionOverrideOutputTypeDef,
     RuleOutputTypeDef,
     RuleSummaryTypeDef,
+    DefaultActionUnionTypeDef,
     RuleActionOverrideTypeDef,
     RuleTypeDef,
     GetLoggingConfigurationResponseTypeDef,
     ListLoggingConfigurationsResponseTypeDef,
     PutLoggingConfigurationResponseTypeDef,
+    LoggingConfigurationUnionTypeDef,
     PutLoggingConfigurationRequestRequestTypeDef,
     ManagedRuleGroupStatementOutputTypeDef,
     RuleGroupReferenceStatementOutputTypeDef,
     RuleGroupTypeDef,
     DescribeManagedRuleGroupResponseTypeDef,
     ManagedRuleGroupStatementTypeDef,
     RuleGroupReferenceStatementTypeDef,
+    RuleUnionTypeDef,
+    FirewallManagerStatementTypeDef,
+    StatementOutputTypeDef,
+    GetRuleGroupResponseTypeDef,
+    StatementTypeDef,
     CheckCapacityRequestRequestTypeDef,
     CreateRuleGroupRequestRequestTypeDef,
     CreateWebACLRequestRequestTypeDef,
     UpdateRuleGroupRequestRequestTypeDef,
     UpdateWebACLRequestRequestTypeDef,
-    FirewallManagerStatementTypeDef,
-    StatementOutputTypeDef,
-    GetRuleGroupResponseTypeDef,
-    StatementTypeDef,
     FirewallManagerRuleGroupTypeDef,
     WebACLTypeDef,
     GetWebACLForResourceResponseTypeDef,
     GetWebACLResponseTypeDef,
 )
 
 
-def get_structure() -> APIKeySummaryTypeDef:
+def get_value() -> APIKeySummaryTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-wafv2-1.28.15.post1/mypy_boto3_wafv2/__main__.py` & `mypy-boto3-wafv2-1.28.16/mypy_boto3_wafv2/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.WAFV2 1.28.15\nVersion:         1.28.15.post1\nBuilder version:"
-        " 7.16.2\nDocs:           "
+        "Type annotations for boto3.WAFV2 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2\nOther"
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

### Comparing `mypy-boto3-wafv2-1.28.15.post1/mypy_boto3_wafv2/client.py` & `mypy-boto3-wafv2-1.28.16/mypy_boto3_wafv2/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,34 +9,31 @@
     from boto3.session import Session
     from mypy_boto3_wafv2.client import WAFV2Client
 
     session = Session()
     client: WAFV2Client = session.client("wafv2")
     ```
 """
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import IPAddressVersionType, PlatformType, ResourceTypeType, ScopeType
 from .type_defs import (
-    AssociationConfigOutputTypeDef,
-    AssociationConfigTypeDef,
+    AssociationConfigUnionTypeDef,
     CaptchaConfigTypeDef,
     ChallengeConfigTypeDef,
     CheckCapacityResponseTypeDef,
     CreateAPIKeyResponseTypeDef,
     CreateIPSetResponseTypeDef,
     CreateRegexPatternSetResponseTypeDef,
     CreateRuleGroupResponseTypeDef,
     CreateWebACLResponseTypeDef,
     CustomResponseBodyTypeDef,
-    DefaultActionOutputTypeDef,
-    DefaultActionTypeDef,
+    DefaultActionUnionTypeDef,
     DeleteFirewallManagerRuleGroupsResponseTypeDef,
     DescribeAllManagedProductsResponseTypeDef,
     DescribeManagedProductsByVendorResponseTypeDef,
     DescribeManagedRuleGroupResponseTypeDef,
     GenerateMobileSdkReleaseUrlResponseTypeDef,
     GetDecryptedAPIKeyResponseTypeDef,
     GetIPSetResponseTypeDef,
@@ -58,24 +55,22 @@
     ListManagedRuleSetsResponseTypeDef,
     ListMobileSdkReleasesResponseTypeDef,
     ListRegexPatternSetsResponseTypeDef,
     ListResourcesForWebACLResponseTypeDef,
     ListRuleGroupsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListWebACLsResponseTypeDef,
-    LoggingConfigurationOutputTypeDef,
-    LoggingConfigurationTypeDef,
+    LoggingConfigurationUnionTypeDef,
     PutLoggingConfigurationResponseTypeDef,
     PutManagedRuleSetVersionsResponseTypeDef,
     RegexTypeDef,
-    RuleOutputTypeDef,
-    RuleTypeDef,
+    RuleUnionTypeDef,
     TagTypeDef,
-    TimeWindowOutputTypeDef,
-    TimeWindowTypeDef,
+    TimestampTypeDef,
+    TimeWindowUnionTypeDef,
     UpdateIPSetResponseTypeDef,
     UpdateManagedRuleSetVersionExpiryDateResponseTypeDef,
     UpdateRegexPatternSetResponseTypeDef,
     UpdateRuleGroupResponseTypeDef,
     UpdateWebACLResponseTypeDef,
     VersionToPublishTypeDef,
     VisibilityConfigTypeDef,
@@ -146,15 +141,15 @@
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/client/#can_paginate)
         """
 
     def check_capacity(
-        self, *, Scope: ScopeType, Rules: Sequence[Union[RuleTypeDef, RuleOutputTypeDef]]
+        self, *, Scope: ScopeType, Rules: Sequence[RuleUnionTypeDef]
     ) -> CheckCapacityResponseTypeDef:
         """
         Returns the web ACL capacity unit (WCU) requirements for a specified scope and
         set of rules.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.check_capacity)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/client/#check_capacity)
@@ -218,15 +213,15 @@
         self,
         *,
         Name: str,
         Scope: ScopeType,
         Capacity: int,
         VisibilityConfig: VisibilityConfigTypeDef,
         Description: str = ...,
-        Rules: Sequence[Union[RuleTypeDef, RuleOutputTypeDef]] = ...,
+        Rules: Sequence[RuleUnionTypeDef] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         CustomResponseBodies: Mapping[str, CustomResponseBodyTypeDef] = ...
     ) -> CreateRuleGroupResponseTypeDef:
         """
         Creates a  RuleGroup per the specifications provided.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.create_rule_group)
@@ -234,24 +229,24 @@
         """
 
     def create_web_acl(
         self,
         *,
         Name: str,
         Scope: ScopeType,
-        DefaultAction: Union[DefaultActionTypeDef, DefaultActionOutputTypeDef],
+        DefaultAction: DefaultActionUnionTypeDef,
         VisibilityConfig: VisibilityConfigTypeDef,
         Description: str = ...,
-        Rules: Sequence[Union[RuleTypeDef, RuleOutputTypeDef]] = ...,
+        Rules: Sequence[RuleUnionTypeDef] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         CustomResponseBodies: Mapping[str, CustomResponseBodyTypeDef] = ...,
         CaptchaConfig: CaptchaConfigTypeDef = ...,
         ChallengeConfig: ChallengeConfigTypeDef = ...,
         TokenDomains: Sequence[str] = ...,
-        AssociationConfig: Union[AssociationConfigTypeDef, AssociationConfigOutputTypeDef] = ...
+        AssociationConfig: AssociationConfigUnionTypeDef = ...
     ) -> CreateWebACLResponseTypeDef:
         """
         Creates a  WebACL per the specifications provided.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.create_web_acl)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/client/#create_web_acl)
         """
@@ -485,15 +480,15 @@
 
     def get_sampled_requests(
         self,
         *,
         WebAclArn: str,
         RuleMetricName: str,
         Scope: ScopeType,
-        TimeWindow: Union[TimeWindowTypeDef, TimeWindowOutputTypeDef],
+        TimeWindow: TimeWindowUnionTypeDef,
         MaxItems: int
     ) -> GetSampledRequestsResponseTypeDef:
         """
         Gets detailed information about a specified number of requests--a sample--that
         WAF randomly selects from among the first 5,000 requests that your Amazon Web
         Services resource received during a time range that you choose.
 
@@ -644,17 +639,15 @@
         Retrieves an array of  WebACLSummary objects for the web ACLs that you manage.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.list_web_acls)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/client/#list_web_acls)
         """
 
     def put_logging_configuration(
-        self,
-        *,
-        LoggingConfiguration: Union[LoggingConfigurationTypeDef, LoggingConfigurationOutputTypeDef]
+        self, *, LoggingConfiguration: LoggingConfigurationUnionTypeDef
     ) -> PutLoggingConfigurationResponseTypeDef:
         """
         Enables the specified  LoggingConfiguration, to start logging from a web ACL,
         according to the configuration provided.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.put_logging_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/client/#put_logging_configuration)
@@ -723,15 +716,15 @@
         self,
         *,
         Name: str,
         Scope: ScopeType,
         Id: str,
         LockToken: str,
         VersionToExpire: str,
-        ExpiryTimestamp: Union[datetime, str]
+        ExpiryTimestamp: TimestampTypeDef
     ) -> UpdateManagedRuleSetVersionExpiryDateResponseTypeDef:
         """
         Updates the expiration information for your managed rule set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.update_managed_rule_set_version_expiry_date)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/client/#update_managed_rule_set_version_expiry_date)
         """
@@ -758,15 +751,15 @@
         *,
         Name: str,
         Scope: ScopeType,
         Id: str,
         VisibilityConfig: VisibilityConfigTypeDef,
         LockToken: str,
         Description: str = ...,
-        Rules: Sequence[Union[RuleTypeDef, RuleOutputTypeDef]] = ...,
+        Rules: Sequence[RuleUnionTypeDef] = ...,
         CustomResponseBodies: Mapping[str, CustomResponseBodyTypeDef] = ...
     ) -> UpdateRuleGroupResponseTypeDef:
         """
         Updates the specified  RuleGroup.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.update_rule_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/client/#update_rule_group)
@@ -774,24 +767,24 @@
 
     def update_web_acl(
         self,
         *,
         Name: str,
         Scope: ScopeType,
         Id: str,
-        DefaultAction: Union[DefaultActionTypeDef, DefaultActionOutputTypeDef],
+        DefaultAction: DefaultActionUnionTypeDef,
         VisibilityConfig: VisibilityConfigTypeDef,
         LockToken: str,
         Description: str = ...,
-        Rules: Sequence[Union[RuleTypeDef, RuleOutputTypeDef]] = ...,
+        Rules: Sequence[RuleUnionTypeDef] = ...,
         CustomResponseBodies: Mapping[str, CustomResponseBodyTypeDef] = ...,
         CaptchaConfig: CaptchaConfigTypeDef = ...,
         ChallengeConfig: ChallengeConfigTypeDef = ...,
         TokenDomains: Sequence[str] = ...,
-        AssociationConfig: Union[AssociationConfigTypeDef, AssociationConfigOutputTypeDef] = ...
+        AssociationConfig: AssociationConfigUnionTypeDef = ...
     ) -> UpdateWebACLResponseTypeDef:
         """
         Updates the specified  WebACL.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.update_web_acl)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/client/#update_web_acl)
         """
```

### Comparing `mypy-boto3-wafv2-1.28.15.post1/mypy_boto3_wafv2/client.pyi` & `mypy-boto3-wafv2-1.28.16/mypy_boto3_wafv2/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -9,34 +9,31 @@
     from boto3.session import Session
     from mypy_boto3_wafv2.client import WAFV2Client
 
     session = Session()
     client: WAFV2Client = session.client("wafv2")
     ```
 """
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import IPAddressVersionType, PlatformType, ResourceTypeType, ScopeType
 from .type_defs import (
-    AssociationConfigOutputTypeDef,
-    AssociationConfigTypeDef,
+    AssociationConfigUnionTypeDef,
     CaptchaConfigTypeDef,
     ChallengeConfigTypeDef,
     CheckCapacityResponseTypeDef,
     CreateAPIKeyResponseTypeDef,
     CreateIPSetResponseTypeDef,
     CreateRegexPatternSetResponseTypeDef,
     CreateRuleGroupResponseTypeDef,
     CreateWebACLResponseTypeDef,
     CustomResponseBodyTypeDef,
-    DefaultActionOutputTypeDef,
-    DefaultActionTypeDef,
+    DefaultActionUnionTypeDef,
     DeleteFirewallManagerRuleGroupsResponseTypeDef,
     DescribeAllManagedProductsResponseTypeDef,
     DescribeManagedProductsByVendorResponseTypeDef,
     DescribeManagedRuleGroupResponseTypeDef,
     GenerateMobileSdkReleaseUrlResponseTypeDef,
     GetDecryptedAPIKeyResponseTypeDef,
     GetIPSetResponseTypeDef,
@@ -58,24 +55,22 @@
     ListManagedRuleSetsResponseTypeDef,
     ListMobileSdkReleasesResponseTypeDef,
     ListRegexPatternSetsResponseTypeDef,
     ListResourcesForWebACLResponseTypeDef,
     ListRuleGroupsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListWebACLsResponseTypeDef,
-    LoggingConfigurationOutputTypeDef,
-    LoggingConfigurationTypeDef,
+    LoggingConfigurationUnionTypeDef,
     PutLoggingConfigurationResponseTypeDef,
     PutManagedRuleSetVersionsResponseTypeDef,
     RegexTypeDef,
-    RuleOutputTypeDef,
-    RuleTypeDef,
+    RuleUnionTypeDef,
     TagTypeDef,
-    TimeWindowOutputTypeDef,
-    TimeWindowTypeDef,
+    TimestampTypeDef,
+    TimeWindowUnionTypeDef,
     UpdateIPSetResponseTypeDef,
     UpdateManagedRuleSetVersionExpiryDateResponseTypeDef,
     UpdateRegexPatternSetResponseTypeDef,
     UpdateRuleGroupResponseTypeDef,
     UpdateWebACLResponseTypeDef,
     VersionToPublishTypeDef,
     VisibilityConfigTypeDef,
@@ -140,15 +135,15 @@
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/client/#can_paginate)
         """
     def check_capacity(
-        self, *, Scope: ScopeType, Rules: Sequence[Union[RuleTypeDef, RuleOutputTypeDef]]
+        self, *, Scope: ScopeType, Rules: Sequence[RuleUnionTypeDef]
     ) -> CheckCapacityResponseTypeDef:
         """
         Returns the web ACL capacity unit (WCU) requirements for a specified scope and
         set of rules.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.check_capacity)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/client/#check_capacity)
@@ -207,39 +202,39 @@
         self,
         *,
         Name: str,
         Scope: ScopeType,
         Capacity: int,
         VisibilityConfig: VisibilityConfigTypeDef,
         Description: str = ...,
-        Rules: Sequence[Union[RuleTypeDef, RuleOutputTypeDef]] = ...,
+        Rules: Sequence[RuleUnionTypeDef] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         CustomResponseBodies: Mapping[str, CustomResponseBodyTypeDef] = ...
     ) -> CreateRuleGroupResponseTypeDef:
         """
         Creates a  RuleGroup per the specifications provided.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.create_rule_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/client/#create_rule_group)
         """
     def create_web_acl(
         self,
         *,
         Name: str,
         Scope: ScopeType,
-        DefaultAction: Union[DefaultActionTypeDef, DefaultActionOutputTypeDef],
+        DefaultAction: DefaultActionUnionTypeDef,
         VisibilityConfig: VisibilityConfigTypeDef,
         Description: str = ...,
-        Rules: Sequence[Union[RuleTypeDef, RuleOutputTypeDef]] = ...,
+        Rules: Sequence[RuleUnionTypeDef] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         CustomResponseBodies: Mapping[str, CustomResponseBodyTypeDef] = ...,
         CaptchaConfig: CaptchaConfigTypeDef = ...,
         ChallengeConfig: ChallengeConfigTypeDef = ...,
         TokenDomains: Sequence[str] = ...,
-        AssociationConfig: Union[AssociationConfigTypeDef, AssociationConfigOutputTypeDef] = ...
+        AssociationConfig: AssociationConfigUnionTypeDef = ...
     ) -> CreateWebACLResponseTypeDef:
         """
         Creates a  WebACL per the specifications provided.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.create_web_acl)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/client/#create_web_acl)
         """
@@ -450,15 +445,15 @@
         """
     def get_sampled_requests(
         self,
         *,
         WebAclArn: str,
         RuleMetricName: str,
         Scope: ScopeType,
-        TimeWindow: Union[TimeWindowTypeDef, TimeWindowOutputTypeDef],
+        TimeWindow: TimeWindowUnionTypeDef,
         MaxItems: int
     ) -> GetSampledRequestsResponseTypeDef:
         """
         Gets detailed information about a specified number of requests--a sample--that
         WAF randomly selects from among the first 5,000 requests that your Amazon Web
         Services resource received during a time range that you choose.
 
@@ -594,17 +589,15 @@
         """
         Retrieves an array of  WebACLSummary objects for the web ACLs that you manage.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.list_web_acls)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/client/#list_web_acls)
         """
     def put_logging_configuration(
-        self,
-        *,
-        LoggingConfiguration: Union[LoggingConfigurationTypeDef, LoggingConfigurationOutputTypeDef]
+        self, *, LoggingConfiguration: LoggingConfigurationUnionTypeDef
     ) -> PutLoggingConfigurationResponseTypeDef:
         """
         Enables the specified  LoggingConfiguration, to start logging from a web ACL,
         according to the configuration provided.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.put_logging_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/client/#put_logging_configuration)
@@ -667,15 +660,15 @@
         self,
         *,
         Name: str,
         Scope: ScopeType,
         Id: str,
         LockToken: str,
         VersionToExpire: str,
-        ExpiryTimestamp: Union[datetime, str]
+        ExpiryTimestamp: TimestampTypeDef
     ) -> UpdateManagedRuleSetVersionExpiryDateResponseTypeDef:
         """
         Updates the expiration information for your managed rule set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.update_managed_rule_set_version_expiry_date)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/client/#update_managed_rule_set_version_expiry_date)
         """
@@ -700,39 +693,39 @@
         *,
         Name: str,
         Scope: ScopeType,
         Id: str,
         VisibilityConfig: VisibilityConfigTypeDef,
         LockToken: str,
         Description: str = ...,
-        Rules: Sequence[Union[RuleTypeDef, RuleOutputTypeDef]] = ...,
+        Rules: Sequence[RuleUnionTypeDef] = ...,
         CustomResponseBodies: Mapping[str, CustomResponseBodyTypeDef] = ...
     ) -> UpdateRuleGroupResponseTypeDef:
         """
         Updates the specified  RuleGroup.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.update_rule_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/client/#update_rule_group)
         """
     def update_web_acl(
         self,
         *,
         Name: str,
         Scope: ScopeType,
         Id: str,
-        DefaultAction: Union[DefaultActionTypeDef, DefaultActionOutputTypeDef],
+        DefaultAction: DefaultActionUnionTypeDef,
         VisibilityConfig: VisibilityConfigTypeDef,
         LockToken: str,
         Description: str = ...,
-        Rules: Sequence[Union[RuleTypeDef, RuleOutputTypeDef]] = ...,
+        Rules: Sequence[RuleUnionTypeDef] = ...,
         CustomResponseBodies: Mapping[str, CustomResponseBodyTypeDef] = ...,
         CaptchaConfig: CaptchaConfigTypeDef = ...,
         ChallengeConfig: ChallengeConfigTypeDef = ...,
         TokenDomains: Sequence[str] = ...,
-        AssociationConfig: Union[AssociationConfigTypeDef, AssociationConfigOutputTypeDef] = ...
+        AssociationConfig: AssociationConfigUnionTypeDef = ...
     ) -> UpdateWebACLResponseTypeDef:
         """
         Updates the specified  WebACL.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2.Client.update_web_acl)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/client/#update_web_acl)
         """
```

### Comparing `mypy-boto3-wafv2-1.28.15.post1/mypy_boto3_wafv2/literals.py` & `mypy-boto3-wafv2-1.28.16/mypy_boto3_wafv2/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-wafv2-1.28.15.post1/mypy_boto3_wafv2/literals.pyi` & `mypy-boto3-wafv2-1.28.16/mypy_boto3_wafv2/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-wafv2-1.28.15.post1/mypy_boto3_wafv2/type_defs.py` & `mypy-boto3-wafv2-1.28.16/mypy_boto3_wafv2/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_wafv2.type_defs import APIKeySummaryTypeDef
 
-    data: APIKeySummaryTypeDef = {...}
+    data: APIKeySummaryTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -60,14 +60,15 @@
     "AWSManagedRulesBotControlRuleSetTypeDef",
     "ActionConditionTypeDef",
     "AddressFieldTypeDef",
     "AndStatementOutputTypeDef",
     "AndStatementTypeDef",
     "AssociateWebACLRequestRequestTypeDef",
     "RequestBodyAssociatedResourceTypeConfigTypeDef",
+    "BlobTypeDef",
     "BodyTypeDef",
     "TextTransformationTypeDef",
     "ImmunityTimePropertyTypeDef",
     "CaptchaResponseTypeDef",
     "ChallengeResponseTypeDef",
     "ResponseMetadataTypeDef",
     "LabelNameConditionTypeDef",
@@ -110,15 +111,14 @@
     "GetManagedRuleSetRequestRequestTypeDef",
     "GetMobileSdkReleaseRequestRequestTypeDef",
     "GetPermissionPolicyRequestRequestTypeDef",
     "GetRateBasedStatementManagedKeysRequestRequestTypeDef",
     "RateBasedStatementManagedKeysIPSetTypeDef",
     "GetRegexPatternSetRequestRequestTypeDef",
     "GetRuleGroupRequestRequestTypeDef",
-    "TimeWindowTypeDef",
     "TimeWindowOutputTypeDef",
     "GetWebACLForResourceRequestRequestTypeDef",
     "GetWebACLRequestRequestTypeDef",
     "HTTPHeaderTypeDef",
     "HeaderMatchPatternOutputTypeDef",
     "HeaderMatchPatternTypeDef",
     "IPSetForwardedIPConfigTypeDef",
@@ -156,17 +156,17 @@
     "ResponseInspectionBodyContainsTypeDef",
     "ResponseInspectionHeaderOutputTypeDef",
     "ResponseInspectionHeaderTypeDef",
     "ResponseInspectionJsonOutputTypeDef",
     "ResponseInspectionJsonTypeDef",
     "ResponseInspectionStatusCodeOutputTypeDef",
     "ResponseInspectionStatusCodeTypeDef",
+    "TimestampTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateIPSetRequestRequestTypeDef",
-    "UpdateManagedRuleSetVersionExpiryDateRequestRequestTypeDef",
     "AssociationConfigOutputTypeDef",
     "AssociationConfigTypeDef",
     "RateLimitCookieOutputTypeDef",
     "RateLimitCookieTypeDef",
     "RateLimitHeaderOutputTypeDef",
     "RateLimitHeaderTypeDef",
     "RateLimitQueryArgumentOutputTypeDef",
@@ -215,15 +215,14 @@
     "CustomResponseTypeDef",
     "DescribeAllManagedProductsResponseTypeDef",
     "DescribeManagedProductsByVendorResponseTypeDef",
     "GeoMatchStatementOutputTypeDef",
     "GeoMatchStatementTypeDef",
     "GetIPSetResponseTypeDef",
     "GetRateBasedStatementManagedKeysResponseTypeDef",
-    "GetSampledRequestsRequestRequestTypeDef",
     "HTTPRequestTypeDef",
     "HeadersOutputTypeDef",
     "HeadersTypeDef",
     "IPSetReferenceStatementTypeDef",
     "JsonBodyOutputTypeDef",
     "JsonBodyTypeDef",
     "ListAvailableManagedRuleGroupVersionsResponseTypeDef",
@@ -233,14 +232,17 @@
     "RequestInspectionTypeDef",
     "ManagedRuleSetTypeDef",
     "RequestInspectionACFPOutputTypeDef",
     "RequestInspectionACFPTypeDef",
     "PutManagedRuleSetVersionsRequestRequestTypeDef",
     "ResponseInspectionOutputTypeDef",
     "ResponseInspectionTypeDef",
+    "TimeWindowTypeDef",
+    "UpdateManagedRuleSetVersionExpiryDateRequestRequestTypeDef",
+    "AssociationConfigUnionTypeDef",
     "RateBasedStatementCustomKeyOutputTypeDef",
     "RateBasedStatementCustomKeyTypeDef",
     "FilterOutputTypeDef",
     "FilterTypeDef",
     "GetMobileSdkReleaseResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "GetRegexPatternSetResponseTypeDef",
@@ -258,14 +260,16 @@
     "FieldToMatchOutputTypeDef",
     "FieldToMatchTypeDef",
     "GetManagedRuleSetResponseTypeDef",
     "AWSManagedRulesACFPRuleSetOutputTypeDef",
     "AWSManagedRulesATPRuleSetOutputTypeDef",
     "AWSManagedRulesACFPRuleSetTypeDef",
     "AWSManagedRulesATPRuleSetTypeDef",
+    "GetSampledRequestsRequestRequestTypeDef",
+    "TimeWindowUnionTypeDef",
     "RateBasedStatementOutputTypeDef",
     "RateBasedStatementTypeDef",
     "LoggingFilterOutputTypeDef",
     "LoggingFilterTypeDef",
     "OverrideActionOutputTypeDef",
     "OverrideActionTypeDef",
     "DefaultActionOutputTypeDef",
@@ -288,35 +292,38 @@
     "ManagedRuleGroupConfigOutputTypeDef",
     "ManagedRuleGroupConfigTypeDef",
     "LoggingConfigurationOutputTypeDef",
     "LoggingConfigurationTypeDef",
     "RuleActionOverrideOutputTypeDef",
     "RuleOutputTypeDef",
     "RuleSummaryTypeDef",
+    "DefaultActionUnionTypeDef",
     "RuleActionOverrideTypeDef",
     "RuleTypeDef",
     "GetLoggingConfigurationResponseTypeDef",
     "ListLoggingConfigurationsResponseTypeDef",
     "PutLoggingConfigurationResponseTypeDef",
+    "LoggingConfigurationUnionTypeDef",
     "PutLoggingConfigurationRequestRequestTypeDef",
     "ManagedRuleGroupStatementOutputTypeDef",
     "RuleGroupReferenceStatementOutputTypeDef",
     "RuleGroupTypeDef",
     "DescribeManagedRuleGroupResponseTypeDef",
     "ManagedRuleGroupStatementTypeDef",
     "RuleGroupReferenceStatementTypeDef",
+    "RuleUnionTypeDef",
+    "FirewallManagerStatementTypeDef",
+    "StatementOutputTypeDef",
+    "GetRuleGroupResponseTypeDef",
+    "StatementTypeDef",
     "CheckCapacityRequestRequestTypeDef",
     "CreateRuleGroupRequestRequestTypeDef",
     "CreateWebACLRequestRequestTypeDef",
     "UpdateRuleGroupRequestRequestTypeDef",
     "UpdateWebACLRequestRequestTypeDef",
-    "FirewallManagerStatementTypeDef",
-    "StatementOutputTypeDef",
-    "GetRuleGroupResponseTypeDef",
-    "StatementTypeDef",
     "FirewallManagerRuleGroupTypeDef",
     "WebACLTypeDef",
     "GetWebACLForResourceResponseTypeDef",
     "GetWebACLResponseTypeDef",
 )
 
 APIKeySummaryTypeDef = TypedDict(
@@ -376,14 +383,15 @@
 RequestBodyAssociatedResourceTypeConfigTypeDef = TypedDict(
     "RequestBodyAssociatedResourceTypeConfigTypeDef",
     {
         "DefaultSizeInspectionLimit": SizeInspectionLimitType,
     },
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 BodyTypeDef = TypedDict(
     "BodyTypeDef",
     {
         "OversizeHandling": OversizeHandlingType,
     },
     total=False,
 )
@@ -862,22 +870,14 @@
         "Scope": ScopeType,
         "Id": str,
         "ARN": str,
     },
     total=False,
 )
 
-TimeWindowTypeDef = TypedDict(
-    "TimeWindowTypeDef",
-    {
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-    },
-)
-
 TimeWindowOutputTypeDef = TypedDict(
     "TimeWindowOutputTypeDef",
     {
         "StartTime": datetime,
         "EndTime": datetime,
     },
 )
@@ -1310,29 +1310,29 @@
     },
     total=False,
 )
 
 NotStatementTypeDef = TypedDict(
     "NotStatementTypeDef",
     {
-        "Statement": "StatementOutputTypeDef",
+        "Statement": "StatementTypeDef",
     },
 )
 
 OrStatementOutputTypeDef = TypedDict(
     "OrStatementOutputTypeDef",
     {
         "Statements": List["StatementOutputTypeDef"],
     },
 )
 
 OrStatementTypeDef = TypedDict(
     "OrStatementTypeDef",
     {
-        "Statements": Sequence["StatementTypeDef"],
+        "Statements": Sequence[Dict[str, Any]],
     },
 )
 
 PhoneNumberFieldTypeDef = TypedDict(
     "PhoneNumberFieldTypeDef",
     {
         "Identifier": str,
@@ -1427,14 +1427,15 @@
     "ResponseInspectionStatusCodeTypeDef",
     {
         "SuccessCodes": Sequence[int],
         "FailureCodes": Sequence[int],
     },
 )
 
+TimestampTypeDef = Union[datetime, str]
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -1460,26 +1461,14 @@
 
 class UpdateIPSetRequestRequestTypeDef(
     _RequiredUpdateIPSetRequestRequestTypeDef, _OptionalUpdateIPSetRequestRequestTypeDef
 ):
     pass
 
 
-UpdateManagedRuleSetVersionExpiryDateRequestRequestTypeDef = TypedDict(
-    "UpdateManagedRuleSetVersionExpiryDateRequestRequestTypeDef",
-    {
-        "Name": str,
-        "Scope": ScopeType,
-        "Id": str,
-        "LockToken": str,
-        "VersionToExpire": str,
-        "ExpiryTimestamp": Union[datetime, str],
-    },
-)
-
 AssociationConfigOutputTypeDef = TypedDict(
     "AssociationConfigOutputTypeDef",
     {
         "RequestBody": Dict[Literal["CLOUDFRONT"], RequestBodyAssociatedResourceTypeConfigTypeDef],
     },
     total=False,
 )
@@ -2018,25 +2007,14 @@
     {
         "ManagedKeysIPV4": RateBasedStatementManagedKeysIPSetTypeDef,
         "ManagedKeysIPV6": RateBasedStatementManagedKeysIPSetTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetSampledRequestsRequestRequestTypeDef = TypedDict(
-    "GetSampledRequestsRequestRequestTypeDef",
-    {
-        "WebAclArn": str,
-        "RuleMetricName": str,
-        "Scope": ScopeType,
-        "TimeWindow": TimeWindowTypeDef,
-        "MaxItems": int,
-    },
-)
-
 HTTPRequestTypeDef = TypedDict(
     "HTTPRequestTypeDef",
     {
         "ClientIP": str,
         "Country": str,
         "URI": str,
         "Method": str,
@@ -2291,14 +2269,35 @@
         "Header": ResponseInspectionHeaderTypeDef,
         "BodyContains": ResponseInspectionBodyContainsTypeDef,
         "Json": ResponseInspectionJsonTypeDef,
     },
     total=False,
 )
 
+TimeWindowTypeDef = TypedDict(
+    "TimeWindowTypeDef",
+    {
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+    },
+)
+
+UpdateManagedRuleSetVersionExpiryDateRequestRequestTypeDef = TypedDict(
+    "UpdateManagedRuleSetVersionExpiryDateRequestRequestTypeDef",
+    {
+        "Name": str,
+        "Scope": ScopeType,
+        "Id": str,
+        "LockToken": str,
+        "VersionToExpire": str,
+        "ExpiryTimestamp": TimestampTypeDef,
+    },
+)
+
+AssociationConfigUnionTypeDef = Union[AssociationConfigTypeDef, AssociationConfigOutputTypeDef]
 RateBasedStatementCustomKeyOutputTypeDef = TypedDict(
     "RateBasedStatementCustomKeyOutputTypeDef",
     {
         "Header": RateLimitHeaderOutputTypeDef,
         "Cookie": RateLimitCookieOutputTypeDef,
         "QueryArgument": RateLimitQueryArgumentOutputTypeDef,
         "QueryString": RateLimitQueryStringOutputTypeDef,
@@ -2617,14 +2616,26 @@
 
 class AWSManagedRulesATPRuleSetTypeDef(
     _RequiredAWSManagedRulesATPRuleSetTypeDef, _OptionalAWSManagedRulesATPRuleSetTypeDef
 ):
     pass
 
 
+GetSampledRequestsRequestRequestTypeDef = TypedDict(
+    "GetSampledRequestsRequestRequestTypeDef",
+    {
+        "WebAclArn": str,
+        "RuleMetricName": str,
+        "Scope": ScopeType,
+        "TimeWindow": TimeWindowTypeDef,
+        "MaxItems": int,
+    },
+)
+
+TimeWindowUnionTypeDef = Union[TimeWindowTypeDef, TimeWindowOutputTypeDef]
 _RequiredRateBasedStatementOutputTypeDef = TypedDict(
     "_RequiredRateBasedStatementOutputTypeDef",
     {
         "Limit": int,
         "AggregateKeyType": RateBasedStatementAggregateKeyTypeType,
     },
 )
@@ -2822,15 +2833,15 @@
         "TextTransformations": List[TextTransformationTypeDef],
     },
 )
 
 ByteMatchStatementTypeDef = TypedDict(
     "ByteMatchStatementTypeDef",
     {
-        "SearchString": Union[str, bytes, IO[Any], StreamingBody],
+        "SearchString": BlobTypeDef,
         "FieldToMatch": FieldToMatchTypeDef,
         "TextTransformations": Sequence[TextTransformationTypeDef],
         "PositionalConstraint": PositionalConstraintType,
     },
 )
 
 RegexMatchStatementTypeDef = TypedDict(
@@ -3006,14 +3017,15 @@
     {
         "Name": str,
         "Action": RuleActionOutputTypeDef,
     },
     total=False,
 )
 
+DefaultActionUnionTypeDef = Union[DefaultActionTypeDef, DefaultActionOutputTypeDef]
 RuleActionOverrideTypeDef = TypedDict(
     "RuleActionOverrideTypeDef",
     {
         "Name": str,
         "ActionToUse": RuleActionTypeDef,
     },
 )
@@ -3065,14 +3077,17 @@
     "PutLoggingConfigurationResponseTypeDef",
     {
         "LoggingConfiguration": LoggingConfigurationOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+LoggingConfigurationUnionTypeDef = Union[
+    LoggingConfigurationTypeDef, LoggingConfigurationOutputTypeDef
+]
 PutLoggingConfigurationRequestRequestTypeDef = TypedDict(
     "PutLoggingConfigurationRequestRequestTypeDef",
     {
         "LoggingConfiguration": LoggingConfigurationTypeDef,
     },
 )
 
@@ -3175,15 +3190,15 @@
     },
 )
 _OptionalManagedRuleGroupStatementTypeDef = TypedDict(
     "_OptionalManagedRuleGroupStatementTypeDef",
     {
         "Version": str,
         "ExcludedRules": Sequence[ExcludedRuleTypeDef],
-        "ScopeDownStatement": Dict[str, Any],
+        "ScopeDownStatement": "StatementTypeDef",
         "ManagedRuleGroupConfigs": Sequence[ManagedRuleGroupConfigTypeDef],
         "RuleActionOverrides": Sequence[RuleActionOverrideTypeDef],
     },
     total=False,
 )
 
 
@@ -3211,19 +3226,82 @@
 
 class RuleGroupReferenceStatementTypeDef(
     _RequiredRuleGroupReferenceStatementTypeDef, _OptionalRuleGroupReferenceStatementTypeDef
 ):
     pass
 
 
+RuleUnionTypeDef = Union[RuleTypeDef, RuleOutputTypeDef]
+FirewallManagerStatementTypeDef = TypedDict(
+    "FirewallManagerStatementTypeDef",
+    {
+        "ManagedRuleGroupStatement": ManagedRuleGroupStatementOutputTypeDef,
+        "RuleGroupReferenceStatement": RuleGroupReferenceStatementOutputTypeDef,
+    },
+    total=False,
+)
+
+StatementOutputTypeDef = TypedDict(
+    "StatementOutputTypeDef",
+    {
+        "ByteMatchStatement": ByteMatchStatementOutputTypeDef,
+        "SqliMatchStatement": SqliMatchStatementOutputTypeDef,
+        "XssMatchStatement": XssMatchStatementOutputTypeDef,
+        "SizeConstraintStatement": SizeConstraintStatementOutputTypeDef,
+        "GeoMatchStatement": GeoMatchStatementOutputTypeDef,
+        "RuleGroupReferenceStatement": RuleGroupReferenceStatementOutputTypeDef,
+        "IPSetReferenceStatement": IPSetReferenceStatementTypeDef,
+        "RegexPatternSetReferenceStatement": RegexPatternSetReferenceStatementOutputTypeDef,
+        "RateBasedStatement": Dict[str, Any],
+        "AndStatement": Dict[str, Any],
+        "OrStatement": Dict[str, Any],
+        "NotStatement": NotStatementTypeDef,
+        "ManagedRuleGroupStatement": Dict[str, Any],
+        "LabelMatchStatement": LabelMatchStatementTypeDef,
+        "RegexMatchStatement": RegexMatchStatementOutputTypeDef,
+    },
+    total=False,
+)
+
+GetRuleGroupResponseTypeDef = TypedDict(
+    "GetRuleGroupResponseTypeDef",
+    {
+        "RuleGroup": RuleGroupTypeDef,
+        "LockToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StatementTypeDef = TypedDict(
+    "StatementTypeDef",
+    {
+        "ByteMatchStatement": ByteMatchStatementTypeDef,
+        "SqliMatchStatement": SqliMatchStatementTypeDef,
+        "XssMatchStatement": XssMatchStatementTypeDef,
+        "SizeConstraintStatement": SizeConstraintStatementTypeDef,
+        "GeoMatchStatement": GeoMatchStatementTypeDef,
+        "RuleGroupReferenceStatement": RuleGroupReferenceStatementTypeDef,
+        "IPSetReferenceStatement": IPSetReferenceStatementTypeDef,
+        "RegexPatternSetReferenceStatement": RegexPatternSetReferenceStatementTypeDef,
+        "RateBasedStatement": Dict[str, Any],
+        "AndStatement": Dict[str, Any],
+        "OrStatement": Dict[str, Any],
+        "NotStatement": Dict[str, Any],
+        "ManagedRuleGroupStatement": Dict[str, Any],
+        "LabelMatchStatement": LabelMatchStatementTypeDef,
+        "RegexMatchStatement": RegexMatchStatementTypeDef,
+    },
+    total=False,
+)
+
 CheckCapacityRequestRequestTypeDef = TypedDict(
     "CheckCapacityRequestRequestTypeDef",
     {
         "Scope": ScopeType,
-        "Rules": Sequence[Union[RuleTypeDef, RuleOutputTypeDef]],
+        "Rules": Sequence[RuleUnionTypeDef],
     },
 )
 
 _RequiredCreateRuleGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRuleGroupRequestRequestTypeDef",
     {
         "Name": str,
@@ -3232,15 +3310,15 @@
         "VisibilityConfig": VisibilityConfigTypeDef,
     },
 )
 _OptionalCreateRuleGroupRequestRequestTypeDef = TypedDict(
     "_OptionalCreateRuleGroupRequestRequestTypeDef",
     {
         "Description": str,
-        "Rules": Sequence[Union[RuleTypeDef, RuleOutputTypeDef]],
+        "Rules": Sequence[RuleUnionTypeDef],
         "Tags": Sequence[TagTypeDef],
         "CustomResponseBodies": Mapping[str, CustomResponseBodyTypeDef],
     },
     total=False,
 )
 
 
@@ -3259,15 +3337,15 @@
         "VisibilityConfig": VisibilityConfigTypeDef,
     },
 )
 _OptionalCreateWebACLRequestRequestTypeDef = TypedDict(
     "_OptionalCreateWebACLRequestRequestTypeDef",
     {
         "Description": str,
-        "Rules": Sequence[Union[RuleTypeDef, RuleOutputTypeDef]],
+        "Rules": Sequence[RuleUnionTypeDef],
         "Tags": Sequence[TagTypeDef],
         "CustomResponseBodies": Mapping[str, CustomResponseBodyTypeDef],
         "CaptchaConfig": CaptchaConfigTypeDef,
         "ChallengeConfig": ChallengeConfigTypeDef,
         "TokenDomains": Sequence[str],
         "AssociationConfig": AssociationConfigTypeDef,
     },
@@ -3291,15 +3369,15 @@
         "LockToken": str,
     },
 )
 _OptionalUpdateRuleGroupRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateRuleGroupRequestRequestTypeDef",
     {
         "Description": str,
-        "Rules": Sequence[Union[RuleTypeDef, RuleOutputTypeDef]],
+        "Rules": Sequence[RuleUnionTypeDef],
         "CustomResponseBodies": Mapping[str, CustomResponseBodyTypeDef],
     },
     total=False,
 )
 
 
 class UpdateRuleGroupRequestRequestTypeDef(
@@ -3319,15 +3397,15 @@
         "LockToken": str,
     },
 )
 _OptionalUpdateWebACLRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateWebACLRequestRequestTypeDef",
     {
         "Description": str,
-        "Rules": Sequence[Union[RuleTypeDef, RuleOutputTypeDef]],
+        "Rules": Sequence[RuleUnionTypeDef],
         "CustomResponseBodies": Mapping[str, CustomResponseBodyTypeDef],
         "CaptchaConfig": CaptchaConfigTypeDef,
         "ChallengeConfig": ChallengeConfigTypeDef,
         "TokenDomains": Sequence[str],
         "AssociationConfig": AssociationConfigTypeDef,
     },
     total=False,
@@ -3336,76 +3414,14 @@
 
 class UpdateWebACLRequestRequestTypeDef(
     _RequiredUpdateWebACLRequestRequestTypeDef, _OptionalUpdateWebACLRequestRequestTypeDef
 ):
     pass
 
 
-FirewallManagerStatementTypeDef = TypedDict(
-    "FirewallManagerStatementTypeDef",
-    {
-        "ManagedRuleGroupStatement": ManagedRuleGroupStatementOutputTypeDef,
-        "RuleGroupReferenceStatement": RuleGroupReferenceStatementOutputTypeDef,
-    },
-    total=False,
-)
-
-StatementOutputTypeDef = TypedDict(
-    "StatementOutputTypeDef",
-    {
-        "ByteMatchStatement": ByteMatchStatementOutputTypeDef,
-        "SqliMatchStatement": SqliMatchStatementOutputTypeDef,
-        "XssMatchStatement": XssMatchStatementOutputTypeDef,
-        "SizeConstraintStatement": SizeConstraintStatementOutputTypeDef,
-        "GeoMatchStatement": GeoMatchStatementOutputTypeDef,
-        "RuleGroupReferenceStatement": RuleGroupReferenceStatementOutputTypeDef,
-        "IPSetReferenceStatement": IPSetReferenceStatementTypeDef,
-        "RegexPatternSetReferenceStatement": RegexPatternSetReferenceStatementOutputTypeDef,
-        "RateBasedStatement": Dict[str, Any],
-        "AndStatement": Dict[str, Any],
-        "OrStatement": Dict[str, Any],
-        "NotStatement": Dict[str, Any],
-        "ManagedRuleGroupStatement": Dict[str, Any],
-        "LabelMatchStatement": LabelMatchStatementTypeDef,
-        "RegexMatchStatement": RegexMatchStatementOutputTypeDef,
-    },
-    total=False,
-)
-
-GetRuleGroupResponseTypeDef = TypedDict(
-    "GetRuleGroupResponseTypeDef",
-    {
-        "RuleGroup": RuleGroupTypeDef,
-        "LockToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StatementTypeDef = TypedDict(
-    "StatementTypeDef",
-    {
-        "ByteMatchStatement": ByteMatchStatementTypeDef,
-        "SqliMatchStatement": SqliMatchStatementTypeDef,
-        "XssMatchStatement": XssMatchStatementTypeDef,
-        "SizeConstraintStatement": SizeConstraintStatementTypeDef,
-        "GeoMatchStatement": GeoMatchStatementTypeDef,
-        "RuleGroupReferenceStatement": RuleGroupReferenceStatementTypeDef,
-        "IPSetReferenceStatement": IPSetReferenceStatementTypeDef,
-        "RegexPatternSetReferenceStatement": RegexPatternSetReferenceStatementTypeDef,
-        "RateBasedStatement": Dict[str, Any],
-        "AndStatement": Dict[str, Any],
-        "OrStatement": Dict[str, Any],
-        "NotStatement": NotStatementTypeDef,
-        "ManagedRuleGroupStatement": Dict[str, Any],
-        "LabelMatchStatement": LabelMatchStatementTypeDef,
-        "RegexMatchStatement": RegexMatchStatementTypeDef,
-    },
-    total=False,
-)
-
 FirewallManagerRuleGroupTypeDef = TypedDict(
     "FirewallManagerRuleGroupTypeDef",
     {
         "Name": str,
         "Priority": int,
         "FirewallManagerStatement": FirewallManagerStatementTypeDef,
         "OverrideAction": OverrideActionOutputTypeDef,
```

### Comparing `mypy-boto3-wafv2-1.28.15.post1/mypy_boto3_wafv2/type_defs.pyi` & `mypy-boto3-wafv2-1.28.16/mypy_boto3_wafv2/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_wafv2.type_defs import APIKeySummaryTypeDef
 
-    data: APIKeySummaryTypeDef = {...}
+    data: APIKeySummaryTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -59,14 +59,15 @@
     "AWSManagedRulesBotControlRuleSetTypeDef",
     "ActionConditionTypeDef",
     "AddressFieldTypeDef",
     "AndStatementOutputTypeDef",
     "AndStatementTypeDef",
     "AssociateWebACLRequestRequestTypeDef",
     "RequestBodyAssociatedResourceTypeConfigTypeDef",
+    "BlobTypeDef",
     "BodyTypeDef",
     "TextTransformationTypeDef",
     "ImmunityTimePropertyTypeDef",
     "CaptchaResponseTypeDef",
     "ChallengeResponseTypeDef",
     "ResponseMetadataTypeDef",
     "LabelNameConditionTypeDef",
@@ -109,15 +110,14 @@
     "GetManagedRuleSetRequestRequestTypeDef",
     "GetMobileSdkReleaseRequestRequestTypeDef",
     "GetPermissionPolicyRequestRequestTypeDef",
     "GetRateBasedStatementManagedKeysRequestRequestTypeDef",
     "RateBasedStatementManagedKeysIPSetTypeDef",
     "GetRegexPatternSetRequestRequestTypeDef",
     "GetRuleGroupRequestRequestTypeDef",
-    "TimeWindowTypeDef",
     "TimeWindowOutputTypeDef",
     "GetWebACLForResourceRequestRequestTypeDef",
     "GetWebACLRequestRequestTypeDef",
     "HTTPHeaderTypeDef",
     "HeaderMatchPatternOutputTypeDef",
     "HeaderMatchPatternTypeDef",
     "IPSetForwardedIPConfigTypeDef",
@@ -155,17 +155,17 @@
     "ResponseInspectionBodyContainsTypeDef",
     "ResponseInspectionHeaderOutputTypeDef",
     "ResponseInspectionHeaderTypeDef",
     "ResponseInspectionJsonOutputTypeDef",
     "ResponseInspectionJsonTypeDef",
     "ResponseInspectionStatusCodeOutputTypeDef",
     "ResponseInspectionStatusCodeTypeDef",
+    "TimestampTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateIPSetRequestRequestTypeDef",
-    "UpdateManagedRuleSetVersionExpiryDateRequestRequestTypeDef",
     "AssociationConfigOutputTypeDef",
     "AssociationConfigTypeDef",
     "RateLimitCookieOutputTypeDef",
     "RateLimitCookieTypeDef",
     "RateLimitHeaderOutputTypeDef",
     "RateLimitHeaderTypeDef",
     "RateLimitQueryArgumentOutputTypeDef",
@@ -214,15 +214,14 @@
     "CustomResponseTypeDef",
     "DescribeAllManagedProductsResponseTypeDef",
     "DescribeManagedProductsByVendorResponseTypeDef",
     "GeoMatchStatementOutputTypeDef",
     "GeoMatchStatementTypeDef",
     "GetIPSetResponseTypeDef",
     "GetRateBasedStatementManagedKeysResponseTypeDef",
-    "GetSampledRequestsRequestRequestTypeDef",
     "HTTPRequestTypeDef",
     "HeadersOutputTypeDef",
     "HeadersTypeDef",
     "IPSetReferenceStatementTypeDef",
     "JsonBodyOutputTypeDef",
     "JsonBodyTypeDef",
     "ListAvailableManagedRuleGroupVersionsResponseTypeDef",
@@ -232,14 +231,17 @@
     "RequestInspectionTypeDef",
     "ManagedRuleSetTypeDef",
     "RequestInspectionACFPOutputTypeDef",
     "RequestInspectionACFPTypeDef",
     "PutManagedRuleSetVersionsRequestRequestTypeDef",
     "ResponseInspectionOutputTypeDef",
     "ResponseInspectionTypeDef",
+    "TimeWindowTypeDef",
+    "UpdateManagedRuleSetVersionExpiryDateRequestRequestTypeDef",
+    "AssociationConfigUnionTypeDef",
     "RateBasedStatementCustomKeyOutputTypeDef",
     "RateBasedStatementCustomKeyTypeDef",
     "FilterOutputTypeDef",
     "FilterTypeDef",
     "GetMobileSdkReleaseResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "GetRegexPatternSetResponseTypeDef",
@@ -257,14 +259,16 @@
     "FieldToMatchOutputTypeDef",
     "FieldToMatchTypeDef",
     "GetManagedRuleSetResponseTypeDef",
     "AWSManagedRulesACFPRuleSetOutputTypeDef",
     "AWSManagedRulesATPRuleSetOutputTypeDef",
     "AWSManagedRulesACFPRuleSetTypeDef",
     "AWSManagedRulesATPRuleSetTypeDef",
+    "GetSampledRequestsRequestRequestTypeDef",
+    "TimeWindowUnionTypeDef",
     "RateBasedStatementOutputTypeDef",
     "RateBasedStatementTypeDef",
     "LoggingFilterOutputTypeDef",
     "LoggingFilterTypeDef",
     "OverrideActionOutputTypeDef",
     "OverrideActionTypeDef",
     "DefaultActionOutputTypeDef",
@@ -287,35 +291,38 @@
     "ManagedRuleGroupConfigOutputTypeDef",
     "ManagedRuleGroupConfigTypeDef",
     "LoggingConfigurationOutputTypeDef",
     "LoggingConfigurationTypeDef",
     "RuleActionOverrideOutputTypeDef",
     "RuleOutputTypeDef",
     "RuleSummaryTypeDef",
+    "DefaultActionUnionTypeDef",
     "RuleActionOverrideTypeDef",
     "RuleTypeDef",
     "GetLoggingConfigurationResponseTypeDef",
     "ListLoggingConfigurationsResponseTypeDef",
     "PutLoggingConfigurationResponseTypeDef",
+    "LoggingConfigurationUnionTypeDef",
     "PutLoggingConfigurationRequestRequestTypeDef",
     "ManagedRuleGroupStatementOutputTypeDef",
     "RuleGroupReferenceStatementOutputTypeDef",
     "RuleGroupTypeDef",
     "DescribeManagedRuleGroupResponseTypeDef",
     "ManagedRuleGroupStatementTypeDef",
     "RuleGroupReferenceStatementTypeDef",
+    "RuleUnionTypeDef",
+    "FirewallManagerStatementTypeDef",
+    "StatementOutputTypeDef",
+    "GetRuleGroupResponseTypeDef",
+    "StatementTypeDef",
     "CheckCapacityRequestRequestTypeDef",
     "CreateRuleGroupRequestRequestTypeDef",
     "CreateWebACLRequestRequestTypeDef",
     "UpdateRuleGroupRequestRequestTypeDef",
     "UpdateWebACLRequestRequestTypeDef",
-    "FirewallManagerStatementTypeDef",
-    "StatementOutputTypeDef",
-    "GetRuleGroupResponseTypeDef",
-    "StatementTypeDef",
     "FirewallManagerRuleGroupTypeDef",
     "WebACLTypeDef",
     "GetWebACLForResourceResponseTypeDef",
     "GetWebACLResponseTypeDef",
 )
 
 APIKeySummaryTypeDef = TypedDict(
@@ -375,14 +382,15 @@
 RequestBodyAssociatedResourceTypeConfigTypeDef = TypedDict(
     "RequestBodyAssociatedResourceTypeConfigTypeDef",
     {
         "DefaultSizeInspectionLimit": SizeInspectionLimitType,
     },
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 BodyTypeDef = TypedDict(
     "BodyTypeDef",
     {
         "OversizeHandling": OversizeHandlingType,
     },
     total=False,
 )
@@ -855,22 +863,14 @@
         "Scope": ScopeType,
         "Id": str,
         "ARN": str,
     },
     total=False,
 )
 
-TimeWindowTypeDef = TypedDict(
-    "TimeWindowTypeDef",
-    {
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-    },
-)
-
 TimeWindowOutputTypeDef = TypedDict(
     "TimeWindowOutputTypeDef",
     {
         "StartTime": datetime,
         "EndTime": datetime,
     },
 )
@@ -1279,29 +1279,29 @@
     },
     total=False,
 )
 
 NotStatementTypeDef = TypedDict(
     "NotStatementTypeDef",
     {
-        "Statement": "StatementOutputTypeDef",
+        "Statement": "StatementTypeDef",
     },
 )
 
 OrStatementOutputTypeDef = TypedDict(
     "OrStatementOutputTypeDef",
     {
         "Statements": List["StatementOutputTypeDef"],
     },
 )
 
 OrStatementTypeDef = TypedDict(
     "OrStatementTypeDef",
     {
-        "Statements": Sequence["StatementTypeDef"],
+        "Statements": Sequence[Dict[str, Any]],
     },
 )
 
 PhoneNumberFieldTypeDef = TypedDict(
     "PhoneNumberFieldTypeDef",
     {
         "Identifier": str,
@@ -1396,14 +1396,15 @@
     "ResponseInspectionStatusCodeTypeDef",
     {
         "SuccessCodes": Sequence[int],
         "FailureCodes": Sequence[int],
     },
 )
 
+TimestampTypeDef = Union[datetime, str]
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -1427,26 +1428,14 @@
 )
 
 class UpdateIPSetRequestRequestTypeDef(
     _RequiredUpdateIPSetRequestRequestTypeDef, _OptionalUpdateIPSetRequestRequestTypeDef
 ):
     pass
 
-UpdateManagedRuleSetVersionExpiryDateRequestRequestTypeDef = TypedDict(
-    "UpdateManagedRuleSetVersionExpiryDateRequestRequestTypeDef",
-    {
-        "Name": str,
-        "Scope": ScopeType,
-        "Id": str,
-        "LockToken": str,
-        "VersionToExpire": str,
-        "ExpiryTimestamp": Union[datetime, str],
-    },
-)
-
 AssociationConfigOutputTypeDef = TypedDict(
     "AssociationConfigOutputTypeDef",
     {
         "RequestBody": Dict[Literal["CLOUDFRONT"], RequestBodyAssociatedResourceTypeConfigTypeDef],
     },
     total=False,
 )
@@ -1975,25 +1964,14 @@
     {
         "ManagedKeysIPV4": RateBasedStatementManagedKeysIPSetTypeDef,
         "ManagedKeysIPV6": RateBasedStatementManagedKeysIPSetTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetSampledRequestsRequestRequestTypeDef = TypedDict(
-    "GetSampledRequestsRequestRequestTypeDef",
-    {
-        "WebAclArn": str,
-        "RuleMetricName": str,
-        "Scope": ScopeType,
-        "TimeWindow": TimeWindowTypeDef,
-        "MaxItems": int,
-    },
-)
-
 HTTPRequestTypeDef = TypedDict(
     "HTTPRequestTypeDef",
     {
         "ClientIP": str,
         "Country": str,
         "URI": str,
         "Method": str,
@@ -2234,14 +2212,35 @@
         "Header": ResponseInspectionHeaderTypeDef,
         "BodyContains": ResponseInspectionBodyContainsTypeDef,
         "Json": ResponseInspectionJsonTypeDef,
     },
     total=False,
 )
 
+TimeWindowTypeDef = TypedDict(
+    "TimeWindowTypeDef",
+    {
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+    },
+)
+
+UpdateManagedRuleSetVersionExpiryDateRequestRequestTypeDef = TypedDict(
+    "UpdateManagedRuleSetVersionExpiryDateRequestRequestTypeDef",
+    {
+        "Name": str,
+        "Scope": ScopeType,
+        "Id": str,
+        "LockToken": str,
+        "VersionToExpire": str,
+        "ExpiryTimestamp": TimestampTypeDef,
+    },
+)
+
+AssociationConfigUnionTypeDef = Union[AssociationConfigTypeDef, AssociationConfigOutputTypeDef]
 RateBasedStatementCustomKeyOutputTypeDef = TypedDict(
     "RateBasedStatementCustomKeyOutputTypeDef",
     {
         "Header": RateLimitHeaderOutputTypeDef,
         "Cookie": RateLimitCookieOutputTypeDef,
         "QueryArgument": RateLimitQueryArgumentOutputTypeDef,
         "QueryString": RateLimitQueryStringOutputTypeDef,
@@ -2550,14 +2549,26 @@
 )
 
 class AWSManagedRulesATPRuleSetTypeDef(
     _RequiredAWSManagedRulesATPRuleSetTypeDef, _OptionalAWSManagedRulesATPRuleSetTypeDef
 ):
     pass
 
+GetSampledRequestsRequestRequestTypeDef = TypedDict(
+    "GetSampledRequestsRequestRequestTypeDef",
+    {
+        "WebAclArn": str,
+        "RuleMetricName": str,
+        "Scope": ScopeType,
+        "TimeWindow": TimeWindowTypeDef,
+        "MaxItems": int,
+    },
+)
+
+TimeWindowUnionTypeDef = Union[TimeWindowTypeDef, TimeWindowOutputTypeDef]
 _RequiredRateBasedStatementOutputTypeDef = TypedDict(
     "_RequiredRateBasedStatementOutputTypeDef",
     {
         "Limit": int,
         "AggregateKeyType": RateBasedStatementAggregateKeyTypeType,
     },
 )
@@ -2749,15 +2760,15 @@
         "TextTransformations": List[TextTransformationTypeDef],
     },
 )
 
 ByteMatchStatementTypeDef = TypedDict(
     "ByteMatchStatementTypeDef",
     {
-        "SearchString": Union[str, bytes, IO[Any], StreamingBody],
+        "SearchString": BlobTypeDef,
         "FieldToMatch": FieldToMatchTypeDef,
         "TextTransformations": Sequence[TextTransformationTypeDef],
         "PositionalConstraint": PositionalConstraintType,
     },
 )
 
 RegexMatchStatementTypeDef = TypedDict(
@@ -2925,14 +2936,15 @@
     {
         "Name": str,
         "Action": RuleActionOutputTypeDef,
     },
     total=False,
 )
 
+DefaultActionUnionTypeDef = Union[DefaultActionTypeDef, DefaultActionOutputTypeDef]
 RuleActionOverrideTypeDef = TypedDict(
     "RuleActionOverrideTypeDef",
     {
         "Name": str,
         "ActionToUse": RuleActionTypeDef,
     },
 )
@@ -2982,14 +2994,17 @@
     "PutLoggingConfigurationResponseTypeDef",
     {
         "LoggingConfiguration": LoggingConfigurationOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+LoggingConfigurationUnionTypeDef = Union[
+    LoggingConfigurationTypeDef, LoggingConfigurationOutputTypeDef
+]
 PutLoggingConfigurationRequestRequestTypeDef = TypedDict(
     "PutLoggingConfigurationRequestRequestTypeDef",
     {
         "LoggingConfiguration": LoggingConfigurationTypeDef,
     },
 )
 
@@ -3086,15 +3101,15 @@
     },
 )
 _OptionalManagedRuleGroupStatementTypeDef = TypedDict(
     "_OptionalManagedRuleGroupStatementTypeDef",
     {
         "Version": str,
         "ExcludedRules": Sequence[ExcludedRuleTypeDef],
-        "ScopeDownStatement": Dict[str, Any],
+        "ScopeDownStatement": "StatementTypeDef",
         "ManagedRuleGroupConfigs": Sequence[ManagedRuleGroupConfigTypeDef],
         "RuleActionOverrides": Sequence[RuleActionOverrideTypeDef],
     },
     total=False,
 )
 
 class ManagedRuleGroupStatementTypeDef(
@@ -3118,19 +3133,82 @@
 )
 
 class RuleGroupReferenceStatementTypeDef(
     _RequiredRuleGroupReferenceStatementTypeDef, _OptionalRuleGroupReferenceStatementTypeDef
 ):
     pass
 
+RuleUnionTypeDef = Union[RuleTypeDef, RuleOutputTypeDef]
+FirewallManagerStatementTypeDef = TypedDict(
+    "FirewallManagerStatementTypeDef",
+    {
+        "ManagedRuleGroupStatement": ManagedRuleGroupStatementOutputTypeDef,
+        "RuleGroupReferenceStatement": RuleGroupReferenceStatementOutputTypeDef,
+    },
+    total=False,
+)
+
+StatementOutputTypeDef = TypedDict(
+    "StatementOutputTypeDef",
+    {
+        "ByteMatchStatement": ByteMatchStatementOutputTypeDef,
+        "SqliMatchStatement": SqliMatchStatementOutputTypeDef,
+        "XssMatchStatement": XssMatchStatementOutputTypeDef,
+        "SizeConstraintStatement": SizeConstraintStatementOutputTypeDef,
+        "GeoMatchStatement": GeoMatchStatementOutputTypeDef,
+        "RuleGroupReferenceStatement": RuleGroupReferenceStatementOutputTypeDef,
+        "IPSetReferenceStatement": IPSetReferenceStatementTypeDef,
+        "RegexPatternSetReferenceStatement": RegexPatternSetReferenceStatementOutputTypeDef,
+        "RateBasedStatement": Dict[str, Any],
+        "AndStatement": Dict[str, Any],
+        "OrStatement": Dict[str, Any],
+        "NotStatement": NotStatementTypeDef,
+        "ManagedRuleGroupStatement": Dict[str, Any],
+        "LabelMatchStatement": LabelMatchStatementTypeDef,
+        "RegexMatchStatement": RegexMatchStatementOutputTypeDef,
+    },
+    total=False,
+)
+
+GetRuleGroupResponseTypeDef = TypedDict(
+    "GetRuleGroupResponseTypeDef",
+    {
+        "RuleGroup": RuleGroupTypeDef,
+        "LockToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StatementTypeDef = TypedDict(
+    "StatementTypeDef",
+    {
+        "ByteMatchStatement": ByteMatchStatementTypeDef,
+        "SqliMatchStatement": SqliMatchStatementTypeDef,
+        "XssMatchStatement": XssMatchStatementTypeDef,
+        "SizeConstraintStatement": SizeConstraintStatementTypeDef,
+        "GeoMatchStatement": GeoMatchStatementTypeDef,
+        "RuleGroupReferenceStatement": RuleGroupReferenceStatementTypeDef,
+        "IPSetReferenceStatement": IPSetReferenceStatementTypeDef,
+        "RegexPatternSetReferenceStatement": RegexPatternSetReferenceStatementTypeDef,
+        "RateBasedStatement": Dict[str, Any],
+        "AndStatement": Dict[str, Any],
+        "OrStatement": Dict[str, Any],
+        "NotStatement": Dict[str, Any],
+        "ManagedRuleGroupStatement": Dict[str, Any],
+        "LabelMatchStatement": LabelMatchStatementTypeDef,
+        "RegexMatchStatement": RegexMatchStatementTypeDef,
+    },
+    total=False,
+)
+
 CheckCapacityRequestRequestTypeDef = TypedDict(
     "CheckCapacityRequestRequestTypeDef",
     {
         "Scope": ScopeType,
-        "Rules": Sequence[Union[RuleTypeDef, RuleOutputTypeDef]],
+        "Rules": Sequence[RuleUnionTypeDef],
     },
 )
 
 _RequiredCreateRuleGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRuleGroupRequestRequestTypeDef",
     {
         "Name": str,
@@ -3139,15 +3217,15 @@
         "VisibilityConfig": VisibilityConfigTypeDef,
     },
 )
 _OptionalCreateRuleGroupRequestRequestTypeDef = TypedDict(
     "_OptionalCreateRuleGroupRequestRequestTypeDef",
     {
         "Description": str,
-        "Rules": Sequence[Union[RuleTypeDef, RuleOutputTypeDef]],
+        "Rules": Sequence[RuleUnionTypeDef],
         "Tags": Sequence[TagTypeDef],
         "CustomResponseBodies": Mapping[str, CustomResponseBodyTypeDef],
     },
     total=False,
 )
 
 class CreateRuleGroupRequestRequestTypeDef(
@@ -3164,15 +3242,15 @@
         "VisibilityConfig": VisibilityConfigTypeDef,
     },
 )
 _OptionalCreateWebACLRequestRequestTypeDef = TypedDict(
     "_OptionalCreateWebACLRequestRequestTypeDef",
     {
         "Description": str,
-        "Rules": Sequence[Union[RuleTypeDef, RuleOutputTypeDef]],
+        "Rules": Sequence[RuleUnionTypeDef],
         "Tags": Sequence[TagTypeDef],
         "CustomResponseBodies": Mapping[str, CustomResponseBodyTypeDef],
         "CaptchaConfig": CaptchaConfigTypeDef,
         "ChallengeConfig": ChallengeConfigTypeDef,
         "TokenDomains": Sequence[str],
         "AssociationConfig": AssociationConfigTypeDef,
     },
@@ -3194,15 +3272,15 @@
         "LockToken": str,
     },
 )
 _OptionalUpdateRuleGroupRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateRuleGroupRequestRequestTypeDef",
     {
         "Description": str,
-        "Rules": Sequence[Union[RuleTypeDef, RuleOutputTypeDef]],
+        "Rules": Sequence[RuleUnionTypeDef],
         "CustomResponseBodies": Mapping[str, CustomResponseBodyTypeDef],
     },
     total=False,
 )
 
 class UpdateRuleGroupRequestRequestTypeDef(
     _RequiredUpdateRuleGroupRequestRequestTypeDef, _OptionalUpdateRuleGroupRequestRequestTypeDef
@@ -3220,91 +3298,29 @@
         "LockToken": str,
     },
 )
 _OptionalUpdateWebACLRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateWebACLRequestRequestTypeDef",
     {
         "Description": str,
-        "Rules": Sequence[Union[RuleTypeDef, RuleOutputTypeDef]],
+        "Rules": Sequence[RuleUnionTypeDef],
         "CustomResponseBodies": Mapping[str, CustomResponseBodyTypeDef],
         "CaptchaConfig": CaptchaConfigTypeDef,
         "ChallengeConfig": ChallengeConfigTypeDef,
         "TokenDomains": Sequence[str],
         "AssociationConfig": AssociationConfigTypeDef,
     },
     total=False,
 )
 
 class UpdateWebACLRequestRequestTypeDef(
     _RequiredUpdateWebACLRequestRequestTypeDef, _OptionalUpdateWebACLRequestRequestTypeDef
 ):
     pass
 
-FirewallManagerStatementTypeDef = TypedDict(
-    "FirewallManagerStatementTypeDef",
-    {
-        "ManagedRuleGroupStatement": ManagedRuleGroupStatementOutputTypeDef,
-        "RuleGroupReferenceStatement": RuleGroupReferenceStatementOutputTypeDef,
-    },
-    total=False,
-)
-
-StatementOutputTypeDef = TypedDict(
-    "StatementOutputTypeDef",
-    {
-        "ByteMatchStatement": ByteMatchStatementOutputTypeDef,
-        "SqliMatchStatement": SqliMatchStatementOutputTypeDef,
-        "XssMatchStatement": XssMatchStatementOutputTypeDef,
-        "SizeConstraintStatement": SizeConstraintStatementOutputTypeDef,
-        "GeoMatchStatement": GeoMatchStatementOutputTypeDef,
-        "RuleGroupReferenceStatement": RuleGroupReferenceStatementOutputTypeDef,
-        "IPSetReferenceStatement": IPSetReferenceStatementTypeDef,
-        "RegexPatternSetReferenceStatement": RegexPatternSetReferenceStatementOutputTypeDef,
-        "RateBasedStatement": Dict[str, Any],
-        "AndStatement": Dict[str, Any],
-        "OrStatement": Dict[str, Any],
-        "NotStatement": Dict[str, Any],
-        "ManagedRuleGroupStatement": Dict[str, Any],
-        "LabelMatchStatement": LabelMatchStatementTypeDef,
-        "RegexMatchStatement": RegexMatchStatementOutputTypeDef,
-    },
-    total=False,
-)
-
-GetRuleGroupResponseTypeDef = TypedDict(
-    "GetRuleGroupResponseTypeDef",
-    {
-        "RuleGroup": RuleGroupTypeDef,
-        "LockToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StatementTypeDef = TypedDict(
-    "StatementTypeDef",
-    {
-        "ByteMatchStatement": ByteMatchStatementTypeDef,
-        "SqliMatchStatement": SqliMatchStatementTypeDef,
-        "XssMatchStatement": XssMatchStatementTypeDef,
-        "SizeConstraintStatement": SizeConstraintStatementTypeDef,
-        "GeoMatchStatement": GeoMatchStatementTypeDef,
-        "RuleGroupReferenceStatement": RuleGroupReferenceStatementTypeDef,
-        "IPSetReferenceStatement": IPSetReferenceStatementTypeDef,
-        "RegexPatternSetReferenceStatement": RegexPatternSetReferenceStatementTypeDef,
-        "RateBasedStatement": Dict[str, Any],
-        "AndStatement": Dict[str, Any],
-        "OrStatement": Dict[str, Any],
-        "NotStatement": NotStatementTypeDef,
-        "ManagedRuleGroupStatement": Dict[str, Any],
-        "LabelMatchStatement": LabelMatchStatementTypeDef,
-        "RegexMatchStatement": RegexMatchStatementTypeDef,
-    },
-    total=False,
-)
-
 FirewallManagerRuleGroupTypeDef = TypedDict(
     "FirewallManagerRuleGroupTypeDef",
     {
         "Name": str,
         "Priority": int,
         "FirewallManagerStatement": FirewallManagerStatementTypeDef,
         "OverrideAction": OverrideActionOutputTypeDef,
```

### Comparing `mypy-boto3-wafv2-1.28.15.post1/mypy_boto3_wafv2.egg-info/PKG-INFO` & `mypy-boto3-wafv2-1.28.16/mypy_boto3_wafv2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-wafv2
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.WAFV2 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.WAFV2 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 wafv2 type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 wafv2 type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-wafv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-wafv2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-wafv2)](https://pepy.tech/project/mypy-boto3-wafv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WAFV2 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2)
+[boto3.WAFV2 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2)
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
 [mypy-boto3-wafv2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -73,15 +73,15 @@
     - [Sublime Text](#sublime-text)
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
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
@@ -312,31 +312,32 @@
 )
 
 
 def check_value(value: ActionValueType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_wafv2.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_wafv2.type_defs import (
     APIKeySummaryTypeDef,
     AWSManagedRulesBotControlRuleSetTypeDef,
     ActionConditionTypeDef,
     AddressFieldTypeDef,
     AndStatementOutputTypeDef,
     AndStatementTypeDef,
     AssociateWebACLRequestRequestTypeDef,
     RequestBodyAssociatedResourceTypeConfigTypeDef,
+    BlobTypeDef,
     BodyTypeDef,
     TextTransformationTypeDef,
     ImmunityTimePropertyTypeDef,
     CaptchaResponseTypeDef,
     ChallengeResponseTypeDef,
     ResponseMetadataTypeDef,
     LabelNameConditionTypeDef,
@@ -379,15 +380,14 @@
     GetManagedRuleSetRequestRequestTypeDef,
     GetMobileSdkReleaseRequestRequestTypeDef,
     GetPermissionPolicyRequestRequestTypeDef,
     GetRateBasedStatementManagedKeysRequestRequestTypeDef,
     RateBasedStatementManagedKeysIPSetTypeDef,
     GetRegexPatternSetRequestRequestTypeDef,
     GetRuleGroupRequestRequestTypeDef,
-    TimeWindowTypeDef,
     TimeWindowOutputTypeDef,
     GetWebACLForResourceRequestRequestTypeDef,
     GetWebACLRequestRequestTypeDef,
     HTTPHeaderTypeDef,
     HeaderMatchPatternOutputTypeDef,
     HeaderMatchPatternTypeDef,
     IPSetForwardedIPConfigTypeDef,
@@ -425,17 +425,17 @@
     ResponseInspectionBodyContainsTypeDef,
     ResponseInspectionHeaderOutputTypeDef,
     ResponseInspectionHeaderTypeDef,
     ResponseInspectionJsonOutputTypeDef,
     ResponseInspectionJsonTypeDef,
     ResponseInspectionStatusCodeOutputTypeDef,
     ResponseInspectionStatusCodeTypeDef,
+    TimestampTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateIPSetRequestRequestTypeDef,
-    UpdateManagedRuleSetVersionExpiryDateRequestRequestTypeDef,
     AssociationConfigOutputTypeDef,
     AssociationConfigTypeDef,
     RateLimitCookieOutputTypeDef,
     RateLimitCookieTypeDef,
     RateLimitHeaderOutputTypeDef,
     RateLimitHeaderTypeDef,
     RateLimitQueryArgumentOutputTypeDef,
@@ -484,15 +484,14 @@
     CustomResponseTypeDef,
     DescribeAllManagedProductsResponseTypeDef,
     DescribeManagedProductsByVendorResponseTypeDef,
     GeoMatchStatementOutputTypeDef,
     GeoMatchStatementTypeDef,
     GetIPSetResponseTypeDef,
     GetRateBasedStatementManagedKeysResponseTypeDef,
-    GetSampledRequestsRequestRequestTypeDef,
     HTTPRequestTypeDef,
     HeadersOutputTypeDef,
     HeadersTypeDef,
     IPSetReferenceStatementTypeDef,
     JsonBodyOutputTypeDef,
     JsonBodyTypeDef,
     ListAvailableManagedRuleGroupVersionsResponseTypeDef,
@@ -502,14 +501,17 @@
     RequestInspectionTypeDef,
     ManagedRuleSetTypeDef,
     RequestInspectionACFPOutputTypeDef,
     RequestInspectionACFPTypeDef,
     PutManagedRuleSetVersionsRequestRequestTypeDef,
     ResponseInspectionOutputTypeDef,
     ResponseInspectionTypeDef,
+    TimeWindowTypeDef,
+    UpdateManagedRuleSetVersionExpiryDateRequestRequestTypeDef,
+    AssociationConfigUnionTypeDef,
     RateBasedStatementCustomKeyOutputTypeDef,
     RateBasedStatementCustomKeyTypeDef,
     FilterOutputTypeDef,
     FilterTypeDef,
     GetMobileSdkReleaseResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     GetRegexPatternSetResponseTypeDef,
@@ -527,14 +529,16 @@
     FieldToMatchOutputTypeDef,
     FieldToMatchTypeDef,
     GetManagedRuleSetResponseTypeDef,
     AWSManagedRulesACFPRuleSetOutputTypeDef,
     AWSManagedRulesATPRuleSetOutputTypeDef,
     AWSManagedRulesACFPRuleSetTypeDef,
     AWSManagedRulesATPRuleSetTypeDef,
+    GetSampledRequestsRequestRequestTypeDef,
+    TimeWindowUnionTypeDef,
     RateBasedStatementOutputTypeDef,
     RateBasedStatementTypeDef,
     LoggingFilterOutputTypeDef,
     LoggingFilterTypeDef,
     OverrideActionOutputTypeDef,
     OverrideActionTypeDef,
     DefaultActionOutputTypeDef,
@@ -557,43 +561,46 @@
     ManagedRuleGroupConfigOutputTypeDef,
     ManagedRuleGroupConfigTypeDef,
     LoggingConfigurationOutputTypeDef,
     LoggingConfigurationTypeDef,
     RuleActionOverrideOutputTypeDef,
     RuleOutputTypeDef,
     RuleSummaryTypeDef,
+    DefaultActionUnionTypeDef,
     RuleActionOverrideTypeDef,
     RuleTypeDef,
     GetLoggingConfigurationResponseTypeDef,
     ListLoggingConfigurationsResponseTypeDef,
     PutLoggingConfigurationResponseTypeDef,
+    LoggingConfigurationUnionTypeDef,
     PutLoggingConfigurationRequestRequestTypeDef,
     ManagedRuleGroupStatementOutputTypeDef,
     RuleGroupReferenceStatementOutputTypeDef,
     RuleGroupTypeDef,
     DescribeManagedRuleGroupResponseTypeDef,
     ManagedRuleGroupStatementTypeDef,
     RuleGroupReferenceStatementTypeDef,
+    RuleUnionTypeDef,
+    FirewallManagerStatementTypeDef,
+    StatementOutputTypeDef,
+    GetRuleGroupResponseTypeDef,
+    StatementTypeDef,
     CheckCapacityRequestRequestTypeDef,
     CreateRuleGroupRequestRequestTypeDef,
     CreateWebACLRequestRequestTypeDef,
     UpdateRuleGroupRequestRequestTypeDef,
     UpdateWebACLRequestRequestTypeDef,
-    FirewallManagerStatementTypeDef,
-    StatementOutputTypeDef,
-    GetRuleGroupResponseTypeDef,
-    StatementTypeDef,
     FirewallManagerRuleGroupTypeDef,
     WebACLTypeDef,
     GetWebACLForResourceResponseTypeDef,
     GetWebACLResponseTypeDef,
 )
 
 
-def get_structure() -> APIKeySummaryTypeDef:
+def get_value() -> APIKeySummaryTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-wafv2-1.28.15.post1/mypy_boto3_wafv2.egg-info/SOURCES.txt` & `mypy-boto3-wafv2-1.28.16/mypy_boto3_wafv2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-wafv2-1.28.15.post1/setup.py` & `mypy-boto3-wafv2-1.28.16/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-wafv2",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_wafv2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.WAFV2 1.28.15 service generated with mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.WAFV2 1.28.16 service generated with mypy-boto3-builder 7.17.1"
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
-    keywords="boto3 wafv2 type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 wafv2 type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_wafv2": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

