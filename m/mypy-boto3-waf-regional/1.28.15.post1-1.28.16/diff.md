# Comparing `tmp/mypy-boto3-waf-regional-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-waf-regional-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-waf-regional-1.28.15.post1.tar", last modified: Sat Jul 29 10:04:25 2023, max compression
+gzip compressed data, was "mypy-boto3-waf-regional-1.28.16.tar", last modified: Tue Aug  1 11:38:04 2023, max compression
```

## Comparing `mypy-boto3-waf-regional-1.28.15.post1.tar` & `mypy-boto3-waf-regional-1.28.16.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:25.273455 mypy-boto3-waf-regional-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 10:01:16.000000 mypy-boto3-waf-regional-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20545 2023-07-29 10:04:25.269455 mypy-boto3-waf-regional-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19033 2023-07-29 10:01:16.000000 mypy-boto3-waf-regional-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:25.261455 mypy-boto3-waf-regional-1.28.15.post1/mypy_boto3_waf_regional/
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-29 10:01:16.000000 mypy-boto3-waf-regional-1.28.15.post1/mypy_boto3_waf_regional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-29 10:01:16.000000 mypy-boto3-waf-regional-1.28.15.post1/mypy_boto3_waf_regional/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-29 10:01:16.000000 mypy-boto3-waf-regional-1.28.15.post1/mypy_boto3_waf_regional/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    46413 2023-07-29 10:01:21.000000 mypy-boto3-waf-regional-1.28.15.post1/mypy_boto3_waf_regional/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    46325 2023-07-29 10:01:20.000000 mypy-boto3-waf-regional-1.28.15.post1/mypy_boto3_waf_regional/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12198 2023-07-29 10:01:21.000000 mypy-boto3-waf-regional-1.28.15.post1/mypy_boto3_waf_regional/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12196 2023-07-29 10:01:21.000000 mypy-boto3-waf-regional-1.28.15.post1/mypy_boto3_waf_regional/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 10:01:16.000000 mypy-boto3-waf-regional-1.28.15.post1/mypy_boto3_waf_regional/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    57158 2023-07-29 10:01:23.000000 mypy-boto3-waf-regional-1.28.15.post1/mypy_boto3_waf_regional/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    57107 2023-07-29 10:01:22.000000 mypy-boto3-waf-regional-1.28.15.post1/mypy_boto3_waf_regional/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 10:01:16.000000 mypy-boto3-waf-regional-1.28.15.post1/mypy_boto3_waf_regional/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:25.269455 mypy-boto3-waf-regional-1.28.15.post1/mypy_boto3_waf_regional.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20545 2023-07-29 10:04:25.000000 mypy-boto3-waf-regional-1.28.15.post1/mypy_boto3_waf_regional.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-29 10:04:25.000000 mypy-boto3-waf-regional-1.28.15.post1/mypy_boto3_waf_regional.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:25.000000 mypy-boto3-waf-regional-1.28.15.post1/mypy_boto3_waf_regional.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:25.000000 mypy-boto3-waf-regional-1.28.15.post1/mypy_boto3_waf_regional.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:04:25.000000 mypy-boto3-waf-regional-1.28.15.post1/mypy_boto3_waf_regional.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-29 10:04:25.000000 mypy-boto3-waf-regional-1.28.15.post1/mypy_boto3_waf_regional.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:04:25.273455 mypy-boto3-waf-regional-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-07-29 10:01:16.000000 mypy-boto3-waf-regional-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:38:04.076671 mypy-boto3-waf-regional-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:34:59.000000 mypy-boto3-waf-regional-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20640 2023-08-01 11:38:04.072671 mypy-boto3-waf-regional-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19137 2023-08-01 11:34:59.000000 mypy-boto3-waf-regional-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:38:04.064671 mypy-boto3-waf-regional-1.28.16/mypy_boto3_waf_regional/
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-08-01 11:34:59.000000 mypy-boto3-waf-regional-1.28.16/mypy_boto3_waf_regional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-08-01 11:34:59.000000 mypy-boto3-waf-regional-1.28.16/mypy_boto3_waf_regional/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-08-01 11:34:59.000000 mypy-boto3-waf-regional-1.28.16/mypy_boto3_waf_regional/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46228 2023-08-01 11:35:00.000000 mypy-boto3-waf-regional-1.28.16/mypy_boto3_waf_regional/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46140 2023-08-01 11:34:59.000000 mypy-boto3-waf-regional-1.28.16/mypy_boto3_waf_regional/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12198 2023-08-01 11:35:00.000000 mypy-boto3-waf-regional-1.28.16/mypy_boto3_waf_regional/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12196 2023-08-01 11:35:00.000000 mypy-boto3-waf-regional-1.28.16/mypy_boto3_waf_regional/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:34:59.000000 mypy-boto3-waf-regional-1.28.16/mypy_boto3_waf_regional/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    57513 2023-08-01 11:35:02.000000 mypy-boto3-waf-regional-1.28.16/mypy_boto3_waf_regional/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57462 2023-08-01 11:35:01.000000 mypy-boto3-waf-regional-1.28.16/mypy_boto3_waf_regional/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:34:59.000000 mypy-boto3-waf-regional-1.28.16/mypy_boto3_waf_regional/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:38:04.072671 mypy-boto3-waf-regional-1.28.16/mypy_boto3_waf_regional.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20640 2023-08-01 11:38:03.000000 mypy-boto3-waf-regional-1.28.16/mypy_boto3_waf_regional.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-08-01 11:38:03.000000 mypy-boto3-waf-regional-1.28.16/mypy_boto3_waf_regional.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:38:03.000000 mypy-boto3-waf-regional-1.28.16/mypy_boto3_waf_regional.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:38:03.000000 mypy-boto3-waf-regional-1.28.16/mypy_boto3_waf_regional.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:38:03.000000 mypy-boto3-waf-regional-1.28.16/mypy_boto3_waf_regional.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-01 11:38:03.000000 mypy-boto3-waf-regional-1.28.16/mypy_boto3_waf_regional.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:38:04.076671 mypy-boto3-waf-regional-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-08-01 11:34:59.000000 mypy-boto3-waf-regional-1.28.16/setup.py
```

### Comparing `mypy-boto3-waf-regional-1.28.15.post1/LICENSE` & `mypy-boto3-waf-regional-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-waf-regional-1.28.15.post1/PKG-INFO` & `mypy-boto3-waf-regional-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-waf-regional
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.WAFRegional 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.WAFRegional 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf_regional/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 waf-regional type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 waf-regional type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-waf-regional.svg?color=blue)](https://pypi.org/project/mypy-boto3-waf-regional)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf_regional/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-waf-regional)](https://pepy.tech/project/mypy-boto3-waf-regional)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WAFRegional 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional)
+[boto3.WAFRegional 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional)
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
 [mypy-boto3-waf-regional docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf_regional/).
 
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
@@ -302,27 +302,28 @@
 )
 
 
 def check_value(value: ChangeActionType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_waf_regional.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_waf_regional.type_defs import (
     ExcludedRuleTypeDef,
     WafActionTypeDef,
     WafOverrideActionTypeDef,
     AssociateWebACLRequestRequestTypeDef,
+    BlobTypeDef,
     ByteMatchSetSummaryTypeDef,
     FieldToMatchTypeDef,
     CreateByteMatchSetRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     CreateGeoMatchSetRequestRequestTypeDef,
     CreateIPSetRequestRequestTypeDef,
     TagTypeDef,
@@ -359,15 +360,14 @@
     GetPermissionPolicyRequestRequestTypeDef,
     GetRateBasedRuleManagedKeysRequestRequestTypeDef,
     GetRateBasedRuleRequestRequestTypeDef,
     GetRegexMatchSetRequestRequestTypeDef,
     GetRegexPatternSetRequestRequestTypeDef,
     GetRuleGroupRequestRequestTypeDef,
     GetRuleRequestRequestTypeDef,
-    TimeWindowTypeDef,
     TimeWindowOutputTypeDef,
     GetSizeConstraintSetRequestRequestTypeDef,
     GetSqlInjectionMatchSetRequestRequestTypeDef,
     GetWebACLForResourceRequestRequestTypeDef,
     WebACLSummaryTypeDef,
     GetWebACLRequestRequestTypeDef,
     GetXssMatchSetRequestRequestTypeDef,
@@ -398,14 +398,15 @@
     ListTagsForResourceRequestRequestTypeDef,
     ListWebACLsRequestRequestTypeDef,
     ListXssMatchSetsRequestRequestTypeDef,
     XssMatchSetSummaryTypeDef,
     PredicateTypeDef,
     PutPermissionPolicyRequestRequestTypeDef,
     RegexPatternSetUpdateTypeDef,
+    TimestampTypeDef,
     UntagResourceRequestRequestTypeDef,
     ActivatedRuleOutputTypeDef,
     ActivatedRuleTypeDef,
     ByteMatchTupleOutputTypeDef,
     ByteMatchTupleTypeDef,
     LoggingConfigurationOutputTypeDef,
     LoggingConfigurationTypeDef,
@@ -453,15 +454,14 @@
     CreateRegexPatternSetResponseTypeDef,
     GetRegexPatternSetResponseTypeDef,
     CreateRuleGroupResponseTypeDef,
     GetRuleGroupResponseTypeDef,
     GeoMatchSetTypeDef,
     GeoMatchSetUpdateTypeDef,
     ListGeoMatchSetsResponseTypeDef,
-    GetSampledRequestsRequestRequestTypeDef,
     GetWebACLForResourceResponseTypeDef,
     ListWebACLsResponseTypeDef,
     HTTPRequestTypeDef,
     IPSetTypeDef,
     IPSetUpdateTypeDef,
     ListIPSetsResponseTypeDef,
     ListRateBasedRulesResponseTypeDef,
@@ -473,23 +473,25 @@
     ListSqlInjectionMatchSetsResponseTypeDef,
     ListSubscribedRuleGroupsResponseTypeDef,
     ListXssMatchSetsResponseTypeDef,
     RateBasedRuleTypeDef,
     RuleTypeDef,
     RuleUpdateTypeDef,
     UpdateRegexPatternSetRequestRequestTypeDef,
+    TimeWindowTypeDef,
     ListActivatedRulesInRuleGroupResponseTypeDef,
     WebACLTypeDef,
     RuleGroupUpdateTypeDef,
     WebACLUpdateTypeDef,
     ByteMatchSetTypeDef,
     ByteMatchSetUpdateTypeDef,
     GetLoggingConfigurationResponseTypeDef,
     ListLoggingConfigurationsResponseTypeDef,
     PutLoggingConfigurationResponseTypeDef,
+    LoggingConfigurationUnionTypeDef,
     PutLoggingConfigurationRequestRequestTypeDef,
     RegexMatchSetTypeDef,
     RegexMatchSetUpdateTypeDef,
     SizeConstraintSetTypeDef,
     SizeConstraintSetUpdateTypeDef,
     SqlInjectionMatchSetTypeDef,
     SqlInjectionMatchSetUpdateTypeDef,
@@ -505,14 +507,16 @@
     UpdateIPSetRequestRequestTypeDef,
     CreateRateBasedRuleResponseTypeDef,
     GetRateBasedRuleResponseTypeDef,
     CreateRuleResponseTypeDef,
     GetRuleResponseTypeDef,
     UpdateRateBasedRuleRequestRequestTypeDef,
     UpdateRuleRequestRequestTypeDef,
+    GetSampledRequestsRequestRequestTypeDef,
+    TimeWindowUnionTypeDef,
     CreateWebACLResponseTypeDef,
     GetWebACLResponseTypeDef,
     UpdateRuleGroupRequestRequestTypeDef,
     UpdateWebACLRequestRequestTypeDef,
     CreateByteMatchSetResponseTypeDef,
     GetByteMatchSetResponseTypeDef,
     UpdateByteMatchSetRequestRequestTypeDef,
@@ -528,15 +532,15 @@
     CreateXssMatchSetResponseTypeDef,
     GetXssMatchSetResponseTypeDef,
     UpdateXssMatchSetRequestRequestTypeDef,
     GetSampledRequestsResponseTypeDef,
 )
 
 
-def get_structure() -> ExcludedRuleTypeDef:
+def get_value() -> ExcludedRuleTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-waf-regional-1.28.15.post1/README.md` & `mypy-boto3-waf-regional-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-waf-regional.svg?color=blue)](https://pypi.org/project/mypy-boto3-waf-regional)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf_regional/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-waf-regional)](https://pepy.tech/project/mypy-boto3-waf-regional)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WAFRegional 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional)
+[boto3.WAFRegional 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional)
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
 [mypy-boto3-waf-regional docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf_regional/).
 
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
@@ -270,27 +270,28 @@
 )
 
 
 def check_value(value: ChangeActionType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_waf_regional.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_waf_regional.type_defs import (
     ExcludedRuleTypeDef,
     WafActionTypeDef,
     WafOverrideActionTypeDef,
     AssociateWebACLRequestRequestTypeDef,
+    BlobTypeDef,
     ByteMatchSetSummaryTypeDef,
     FieldToMatchTypeDef,
     CreateByteMatchSetRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     CreateGeoMatchSetRequestRequestTypeDef,
     CreateIPSetRequestRequestTypeDef,
     TagTypeDef,
@@ -327,15 +328,14 @@
     GetPermissionPolicyRequestRequestTypeDef,
     GetRateBasedRuleManagedKeysRequestRequestTypeDef,
     GetRateBasedRuleRequestRequestTypeDef,
     GetRegexMatchSetRequestRequestTypeDef,
     GetRegexPatternSetRequestRequestTypeDef,
     GetRuleGroupRequestRequestTypeDef,
     GetRuleRequestRequestTypeDef,
-    TimeWindowTypeDef,
     TimeWindowOutputTypeDef,
     GetSizeConstraintSetRequestRequestTypeDef,
     GetSqlInjectionMatchSetRequestRequestTypeDef,
     GetWebACLForResourceRequestRequestTypeDef,
     WebACLSummaryTypeDef,
     GetWebACLRequestRequestTypeDef,
     GetXssMatchSetRequestRequestTypeDef,
@@ -366,14 +366,15 @@
     ListTagsForResourceRequestRequestTypeDef,
     ListWebACLsRequestRequestTypeDef,
     ListXssMatchSetsRequestRequestTypeDef,
     XssMatchSetSummaryTypeDef,
     PredicateTypeDef,
     PutPermissionPolicyRequestRequestTypeDef,
     RegexPatternSetUpdateTypeDef,
+    TimestampTypeDef,
     UntagResourceRequestRequestTypeDef,
     ActivatedRuleOutputTypeDef,
     ActivatedRuleTypeDef,
     ByteMatchTupleOutputTypeDef,
     ByteMatchTupleTypeDef,
     LoggingConfigurationOutputTypeDef,
     LoggingConfigurationTypeDef,
@@ -421,15 +422,14 @@
     CreateRegexPatternSetResponseTypeDef,
     GetRegexPatternSetResponseTypeDef,
     CreateRuleGroupResponseTypeDef,
     GetRuleGroupResponseTypeDef,
     GeoMatchSetTypeDef,
     GeoMatchSetUpdateTypeDef,
     ListGeoMatchSetsResponseTypeDef,
-    GetSampledRequestsRequestRequestTypeDef,
     GetWebACLForResourceResponseTypeDef,
     ListWebACLsResponseTypeDef,
     HTTPRequestTypeDef,
     IPSetTypeDef,
     IPSetUpdateTypeDef,
     ListIPSetsResponseTypeDef,
     ListRateBasedRulesResponseTypeDef,
@@ -441,23 +441,25 @@
     ListSqlInjectionMatchSetsResponseTypeDef,
     ListSubscribedRuleGroupsResponseTypeDef,
     ListXssMatchSetsResponseTypeDef,
     RateBasedRuleTypeDef,
     RuleTypeDef,
     RuleUpdateTypeDef,
     UpdateRegexPatternSetRequestRequestTypeDef,
+    TimeWindowTypeDef,
     ListActivatedRulesInRuleGroupResponseTypeDef,
     WebACLTypeDef,
     RuleGroupUpdateTypeDef,
     WebACLUpdateTypeDef,
     ByteMatchSetTypeDef,
     ByteMatchSetUpdateTypeDef,
     GetLoggingConfigurationResponseTypeDef,
     ListLoggingConfigurationsResponseTypeDef,
     PutLoggingConfigurationResponseTypeDef,
+    LoggingConfigurationUnionTypeDef,
     PutLoggingConfigurationRequestRequestTypeDef,
     RegexMatchSetTypeDef,
     RegexMatchSetUpdateTypeDef,
     SizeConstraintSetTypeDef,
     SizeConstraintSetUpdateTypeDef,
     SqlInjectionMatchSetTypeDef,
     SqlInjectionMatchSetUpdateTypeDef,
@@ -473,14 +475,16 @@
     UpdateIPSetRequestRequestTypeDef,
     CreateRateBasedRuleResponseTypeDef,
     GetRateBasedRuleResponseTypeDef,
     CreateRuleResponseTypeDef,
     GetRuleResponseTypeDef,
     UpdateRateBasedRuleRequestRequestTypeDef,
     UpdateRuleRequestRequestTypeDef,
+    GetSampledRequestsRequestRequestTypeDef,
+    TimeWindowUnionTypeDef,
     CreateWebACLResponseTypeDef,
     GetWebACLResponseTypeDef,
     UpdateRuleGroupRequestRequestTypeDef,
     UpdateWebACLRequestRequestTypeDef,
     CreateByteMatchSetResponseTypeDef,
     GetByteMatchSetResponseTypeDef,
     UpdateByteMatchSetRequestRequestTypeDef,
@@ -496,15 +500,15 @@
     CreateXssMatchSetResponseTypeDef,
     GetXssMatchSetResponseTypeDef,
     UpdateXssMatchSetRequestRequestTypeDef,
     GetSampledRequestsResponseTypeDef,
 )
 
 
-def get_structure() -> ExcludedRuleTypeDef:
+def get_value() -> ExcludedRuleTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-waf-regional-1.28.15.post1/mypy_boto3_waf_regional/__main__.py` & `mypy-boto3-waf-regional-1.28.16/mypy_boto3_waf_regional/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.WAFRegional 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.WAFRegional 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf_regional//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional\nOther"
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

### Comparing `mypy-boto3-waf-regional-1.28.15.post1/mypy_boto3_waf_regional/client.py` & `mypy-boto3-waf-regional-1.28.16/mypy_boto3_waf_regional/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_waf_regional.client import WAFRegionalClient
 
     session = Session()
     client: WAFRegionalClient = session.client("waf-regional")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import ResourceTypeType
 from .type_defs import (
     ByteMatchSetUpdateTypeDef,
     CreateByteMatchSetResponseTypeDef,
@@ -80,26 +80,24 @@
     ListRulesResponseTypeDef,
     ListSizeConstraintSetsResponseTypeDef,
     ListSqlInjectionMatchSetsResponseTypeDef,
     ListSubscribedRuleGroupsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListWebACLsResponseTypeDef,
     ListXssMatchSetsResponseTypeDef,
-    LoggingConfigurationOutputTypeDef,
-    LoggingConfigurationTypeDef,
+    LoggingConfigurationUnionTypeDef,
     PutLoggingConfigurationResponseTypeDef,
     RegexMatchSetUpdateTypeDef,
     RegexPatternSetUpdateTypeDef,
     RuleGroupUpdateTypeDef,
     RuleUpdateTypeDef,
     SizeConstraintSetUpdateTypeDef,
     SqlInjectionMatchSetUpdateTypeDef,
     TagTypeDef,
-    TimeWindowOutputTypeDef,
-    TimeWindowTypeDef,
+    TimeWindowUnionTypeDef,
     UpdateByteMatchSetResponseTypeDef,
     UpdateGeoMatchSetResponseTypeDef,
     UpdateIPSetResponseTypeDef,
     UpdateRateBasedRuleResponseTypeDef,
     UpdateRegexMatchSetResponseTypeDef,
     UpdateRegexPatternSetResponseTypeDef,
     UpdateRuleGroupResponseTypeDef,
@@ -594,20 +592,15 @@
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.get_rule_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf_regional/client/#get_rule_group)
         """
 
     def get_sampled_requests(
-        self,
-        *,
-        WebAclId: str,
-        RuleId: str,
-        TimeWindow: Union[TimeWindowTypeDef, TimeWindowOutputTypeDef],
-        MaxItems: int
+        self, *, WebAclId: str, RuleId: str, TimeWindow: TimeWindowUnionTypeDef, MaxItems: int
     ) -> GetSampledRequestsResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.get_sampled_requests)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf_regional/client/#get_sampled_requests)
         """
@@ -819,17 +812,15 @@
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.list_xss_match_sets)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf_regional/client/#list_xss_match_sets)
         """
 
     def put_logging_configuration(
-        self,
-        *,
-        LoggingConfiguration: Union[LoggingConfigurationTypeDef, LoggingConfigurationOutputTypeDef]
+        self, *, LoggingConfiguration: LoggingConfigurationUnionTypeDef
     ) -> PutLoggingConfigurationResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.put_logging_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf_regional/client/#put_logging_configuration)
         """
```

### Comparing `mypy-boto3-waf-regional-1.28.15.post1/mypy_boto3_waf_regional/client.pyi` & `mypy-boto3-waf-regional-1.28.16/mypy_boto3_waf_regional/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_waf_regional.client import WAFRegionalClient
 
     session = Session()
     client: WAFRegionalClient = session.client("waf-regional")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import ResourceTypeType
 from .type_defs import (
     ByteMatchSetUpdateTypeDef,
     CreateByteMatchSetResponseTypeDef,
@@ -80,26 +80,24 @@
     ListRulesResponseTypeDef,
     ListSizeConstraintSetsResponseTypeDef,
     ListSqlInjectionMatchSetsResponseTypeDef,
     ListSubscribedRuleGroupsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListWebACLsResponseTypeDef,
     ListXssMatchSetsResponseTypeDef,
-    LoggingConfigurationOutputTypeDef,
-    LoggingConfigurationTypeDef,
+    LoggingConfigurationUnionTypeDef,
     PutLoggingConfigurationResponseTypeDef,
     RegexMatchSetUpdateTypeDef,
     RegexPatternSetUpdateTypeDef,
     RuleGroupUpdateTypeDef,
     RuleUpdateTypeDef,
     SizeConstraintSetUpdateTypeDef,
     SqlInjectionMatchSetUpdateTypeDef,
     TagTypeDef,
-    TimeWindowOutputTypeDef,
-    TimeWindowTypeDef,
+    TimeWindowUnionTypeDef,
     UpdateByteMatchSetResponseTypeDef,
     UpdateGeoMatchSetResponseTypeDef,
     UpdateIPSetResponseTypeDef,
     UpdateRateBasedRuleResponseTypeDef,
     UpdateRegexMatchSetResponseTypeDef,
     UpdateRegexPatternSetResponseTypeDef,
     UpdateRuleGroupResponseTypeDef,
@@ -544,20 +542,15 @@
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.get_rule_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf_regional/client/#get_rule_group)
         """
     def get_sampled_requests(
-        self,
-        *,
-        WebAclId: str,
-        RuleId: str,
-        TimeWindow: Union[TimeWindowTypeDef, TimeWindowOutputTypeDef],
-        MaxItems: int
+        self, *, WebAclId: str, RuleId: str, TimeWindow: TimeWindowUnionTypeDef, MaxItems: int
     ) -> GetSampledRequestsResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.get_sampled_requests)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf_regional/client/#get_sampled_requests)
         """
@@ -746,17 +739,15 @@
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.list_xss_match_sets)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf_regional/client/#list_xss_match_sets)
         """
     def put_logging_configuration(
-        self,
-        *,
-        LoggingConfiguration: Union[LoggingConfigurationTypeDef, LoggingConfigurationOutputTypeDef]
+        self, *, LoggingConfiguration: LoggingConfigurationUnionTypeDef
     ) -> PutLoggingConfigurationResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional.Client.put_logging_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf_regional/client/#put_logging_configuration)
         """
```

### Comparing `mypy-boto3-waf-regional-1.28.15.post1/mypy_boto3_waf_regional/literals.py` & `mypy-boto3-waf-regional-1.28.16/mypy_boto3_waf_regional/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-waf-regional-1.28.15.post1/mypy_boto3_waf_regional/literals.pyi` & `mypy-boto3-waf-regional-1.28.16/mypy_boto3_waf_regional/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-waf-regional-1.28.15.post1/mypy_boto3_waf_regional/type_defs.py` & `mypy-boto3-waf-regional-1.28.16/mypy_boto3_waf_regional/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf_regional/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_waf_regional.type_defs import ExcludedRuleTypeDef
 
-    data: ExcludedRuleTypeDef = {...}
+    data: ExcludedRuleTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -44,14 +44,15 @@
 
 
 __all__ = (
     "ExcludedRuleTypeDef",
     "WafActionTypeDef",
     "WafOverrideActionTypeDef",
     "AssociateWebACLRequestRequestTypeDef",
+    "BlobTypeDef",
     "ByteMatchSetSummaryTypeDef",
     "FieldToMatchTypeDef",
     "CreateByteMatchSetRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "CreateGeoMatchSetRequestRequestTypeDef",
     "CreateIPSetRequestRequestTypeDef",
     "TagTypeDef",
@@ -88,15 +89,14 @@
     "GetPermissionPolicyRequestRequestTypeDef",
     "GetRateBasedRuleManagedKeysRequestRequestTypeDef",
     "GetRateBasedRuleRequestRequestTypeDef",
     "GetRegexMatchSetRequestRequestTypeDef",
     "GetRegexPatternSetRequestRequestTypeDef",
     "GetRuleGroupRequestRequestTypeDef",
     "GetRuleRequestRequestTypeDef",
-    "TimeWindowTypeDef",
     "TimeWindowOutputTypeDef",
     "GetSizeConstraintSetRequestRequestTypeDef",
     "GetSqlInjectionMatchSetRequestRequestTypeDef",
     "GetWebACLForResourceRequestRequestTypeDef",
     "WebACLSummaryTypeDef",
     "GetWebACLRequestRequestTypeDef",
     "GetXssMatchSetRequestRequestTypeDef",
@@ -127,14 +127,15 @@
     "ListTagsForResourceRequestRequestTypeDef",
     "ListWebACLsRequestRequestTypeDef",
     "ListXssMatchSetsRequestRequestTypeDef",
     "XssMatchSetSummaryTypeDef",
     "PredicateTypeDef",
     "PutPermissionPolicyRequestRequestTypeDef",
     "RegexPatternSetUpdateTypeDef",
+    "TimestampTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "ActivatedRuleOutputTypeDef",
     "ActivatedRuleTypeDef",
     "ByteMatchTupleOutputTypeDef",
     "ByteMatchTupleTypeDef",
     "LoggingConfigurationOutputTypeDef",
     "LoggingConfigurationTypeDef",
@@ -182,15 +183,14 @@
     "CreateRegexPatternSetResponseTypeDef",
     "GetRegexPatternSetResponseTypeDef",
     "CreateRuleGroupResponseTypeDef",
     "GetRuleGroupResponseTypeDef",
     "GeoMatchSetTypeDef",
     "GeoMatchSetUpdateTypeDef",
     "ListGeoMatchSetsResponseTypeDef",
-    "GetSampledRequestsRequestRequestTypeDef",
     "GetWebACLForResourceResponseTypeDef",
     "ListWebACLsResponseTypeDef",
     "HTTPRequestTypeDef",
     "IPSetTypeDef",
     "IPSetUpdateTypeDef",
     "ListIPSetsResponseTypeDef",
     "ListRateBasedRulesResponseTypeDef",
@@ -202,23 +202,25 @@
     "ListSqlInjectionMatchSetsResponseTypeDef",
     "ListSubscribedRuleGroupsResponseTypeDef",
     "ListXssMatchSetsResponseTypeDef",
     "RateBasedRuleTypeDef",
     "RuleTypeDef",
     "RuleUpdateTypeDef",
     "UpdateRegexPatternSetRequestRequestTypeDef",
+    "TimeWindowTypeDef",
     "ListActivatedRulesInRuleGroupResponseTypeDef",
     "WebACLTypeDef",
     "RuleGroupUpdateTypeDef",
     "WebACLUpdateTypeDef",
     "ByteMatchSetTypeDef",
     "ByteMatchSetUpdateTypeDef",
     "GetLoggingConfigurationResponseTypeDef",
     "ListLoggingConfigurationsResponseTypeDef",
     "PutLoggingConfigurationResponseTypeDef",
+    "LoggingConfigurationUnionTypeDef",
     "PutLoggingConfigurationRequestRequestTypeDef",
     "RegexMatchSetTypeDef",
     "RegexMatchSetUpdateTypeDef",
     "SizeConstraintSetTypeDef",
     "SizeConstraintSetUpdateTypeDef",
     "SqlInjectionMatchSetTypeDef",
     "SqlInjectionMatchSetUpdateTypeDef",
@@ -234,14 +236,16 @@
     "UpdateIPSetRequestRequestTypeDef",
     "CreateRateBasedRuleResponseTypeDef",
     "GetRateBasedRuleResponseTypeDef",
     "CreateRuleResponseTypeDef",
     "GetRuleResponseTypeDef",
     "UpdateRateBasedRuleRequestRequestTypeDef",
     "UpdateRuleRequestRequestTypeDef",
+    "GetSampledRequestsRequestRequestTypeDef",
+    "TimeWindowUnionTypeDef",
     "CreateWebACLResponseTypeDef",
     "GetWebACLResponseTypeDef",
     "UpdateRuleGroupRequestRequestTypeDef",
     "UpdateWebACLRequestRequestTypeDef",
     "CreateByteMatchSetResponseTypeDef",
     "GetByteMatchSetResponseTypeDef",
     "UpdateByteMatchSetRequestRequestTypeDef",
@@ -285,14 +289,15 @@
     "AssociateWebACLRequestRequestTypeDef",
     {
         "WebACLId": str,
         "ResourceArn": str,
     },
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 ByteMatchSetSummaryTypeDef = TypedDict(
     "ByteMatchSetSummaryTypeDef",
     {
         "ByteMatchSetId": str,
         "Name": str,
     },
 )
@@ -676,22 +681,14 @@
 GetRuleRequestRequestTypeDef = TypedDict(
     "GetRuleRequestRequestTypeDef",
     {
         "RuleId": str,
     },
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
@@ -1031,14 +1028,15 @@
     "RegexPatternSetUpdateTypeDef",
     {
         "Action": ChangeActionType,
         "RegexPatternString": str,
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
@@ -1101,15 +1099,15 @@
     },
 )
 
 ByteMatchTupleTypeDef = TypedDict(
     "ByteMatchTupleTypeDef",
     {
         "FieldToMatch": FieldToMatchTypeDef,
-        "TargetString": Union[str, bytes, IO[Any], StreamingBody],
+        "TargetString": BlobTypeDef,
         "TextTransformation": TextTransformationType,
         "PositionalConstraint": PositionalConstraintType,
     },
 )
 
 _RequiredLoggingConfigurationOutputTypeDef = TypedDict(
     "_RequiredLoggingConfigurationOutputTypeDef",
@@ -1620,24 +1618,14 @@
     {
         "NextMarker": str,
         "GeoMatchSets": List[GeoMatchSetSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetSampledRequestsRequestRequestTypeDef = TypedDict(
-    "GetSampledRequestsRequestRequestTypeDef",
-    {
-        "WebAclId": str,
-        "RuleId": str,
-        "TimeWindow": TimeWindowTypeDef,
-        "MaxItems": int,
-    },
-)
-
 GetWebACLForResourceResponseTypeDef = TypedDict(
     "GetWebACLForResourceResponseTypeDef",
     {
         "WebACLSummary": WebACLSummaryTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1839,14 +1827,22 @@
     {
         "RegexPatternSetId": str,
         "Updates": Sequence[RegexPatternSetUpdateTypeDef],
         "ChangeToken": str,
     },
 )
 
+TimeWindowTypeDef = TypedDict(
+    "TimeWindowTypeDef",
+    {
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+    },
+)
+
 ListActivatedRulesInRuleGroupResponseTypeDef = TypedDict(
     "ListActivatedRulesInRuleGroupResponseTypeDef",
     {
         "NextMarker": str,
         "ActivatedRules": List[ActivatedRuleOutputTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1940,14 +1936,17 @@
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
 
@@ -2191,14 +2190,25 @@
     {
         "RuleId": str,
         "ChangeToken": str,
         "Updates": Sequence[RuleUpdateTypeDef],
     },
 )
 
+GetSampledRequestsRequestRequestTypeDef = TypedDict(
+    "GetSampledRequestsRequestRequestTypeDef",
+    {
+        "WebAclId": str,
+        "RuleId": str,
+        "TimeWindow": TimeWindowTypeDef,
+        "MaxItems": int,
+    },
+)
+
+TimeWindowUnionTypeDef = Union[TimeWindowTypeDef, TimeWindowOutputTypeDef]
 CreateWebACLResponseTypeDef = TypedDict(
     "CreateWebACLResponseTypeDef",
     {
         "WebACL": WebACLTypeDef,
         "ChangeToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-waf-regional-1.28.15.post1/mypy_boto3_waf_regional/type_defs.pyi` & `mypy-boto3-waf-regional-1.28.16/mypy_boto3_waf_regional/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf_regional/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_waf_regional.type_defs import ExcludedRuleTypeDef
 
-    data: ExcludedRuleTypeDef = {...}
+    data: ExcludedRuleTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -43,14 +43,15 @@
     from typing_extensions import TypedDict
 
 __all__ = (
     "ExcludedRuleTypeDef",
     "WafActionTypeDef",
     "WafOverrideActionTypeDef",
     "AssociateWebACLRequestRequestTypeDef",
+    "BlobTypeDef",
     "ByteMatchSetSummaryTypeDef",
     "FieldToMatchTypeDef",
     "CreateByteMatchSetRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "CreateGeoMatchSetRequestRequestTypeDef",
     "CreateIPSetRequestRequestTypeDef",
     "TagTypeDef",
@@ -87,15 +88,14 @@
     "GetPermissionPolicyRequestRequestTypeDef",
     "GetRateBasedRuleManagedKeysRequestRequestTypeDef",
     "GetRateBasedRuleRequestRequestTypeDef",
     "GetRegexMatchSetRequestRequestTypeDef",
     "GetRegexPatternSetRequestRequestTypeDef",
     "GetRuleGroupRequestRequestTypeDef",
     "GetRuleRequestRequestTypeDef",
-    "TimeWindowTypeDef",
     "TimeWindowOutputTypeDef",
     "GetSizeConstraintSetRequestRequestTypeDef",
     "GetSqlInjectionMatchSetRequestRequestTypeDef",
     "GetWebACLForResourceRequestRequestTypeDef",
     "WebACLSummaryTypeDef",
     "GetWebACLRequestRequestTypeDef",
     "GetXssMatchSetRequestRequestTypeDef",
@@ -126,14 +126,15 @@
     "ListTagsForResourceRequestRequestTypeDef",
     "ListWebACLsRequestRequestTypeDef",
     "ListXssMatchSetsRequestRequestTypeDef",
     "XssMatchSetSummaryTypeDef",
     "PredicateTypeDef",
     "PutPermissionPolicyRequestRequestTypeDef",
     "RegexPatternSetUpdateTypeDef",
+    "TimestampTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "ActivatedRuleOutputTypeDef",
     "ActivatedRuleTypeDef",
     "ByteMatchTupleOutputTypeDef",
     "ByteMatchTupleTypeDef",
     "LoggingConfigurationOutputTypeDef",
     "LoggingConfigurationTypeDef",
@@ -181,15 +182,14 @@
     "CreateRegexPatternSetResponseTypeDef",
     "GetRegexPatternSetResponseTypeDef",
     "CreateRuleGroupResponseTypeDef",
     "GetRuleGroupResponseTypeDef",
     "GeoMatchSetTypeDef",
     "GeoMatchSetUpdateTypeDef",
     "ListGeoMatchSetsResponseTypeDef",
-    "GetSampledRequestsRequestRequestTypeDef",
     "GetWebACLForResourceResponseTypeDef",
     "ListWebACLsResponseTypeDef",
     "HTTPRequestTypeDef",
     "IPSetTypeDef",
     "IPSetUpdateTypeDef",
     "ListIPSetsResponseTypeDef",
     "ListRateBasedRulesResponseTypeDef",
@@ -201,23 +201,25 @@
     "ListSqlInjectionMatchSetsResponseTypeDef",
     "ListSubscribedRuleGroupsResponseTypeDef",
     "ListXssMatchSetsResponseTypeDef",
     "RateBasedRuleTypeDef",
     "RuleTypeDef",
     "RuleUpdateTypeDef",
     "UpdateRegexPatternSetRequestRequestTypeDef",
+    "TimeWindowTypeDef",
     "ListActivatedRulesInRuleGroupResponseTypeDef",
     "WebACLTypeDef",
     "RuleGroupUpdateTypeDef",
     "WebACLUpdateTypeDef",
     "ByteMatchSetTypeDef",
     "ByteMatchSetUpdateTypeDef",
     "GetLoggingConfigurationResponseTypeDef",
     "ListLoggingConfigurationsResponseTypeDef",
     "PutLoggingConfigurationResponseTypeDef",
+    "LoggingConfigurationUnionTypeDef",
     "PutLoggingConfigurationRequestRequestTypeDef",
     "RegexMatchSetTypeDef",
     "RegexMatchSetUpdateTypeDef",
     "SizeConstraintSetTypeDef",
     "SizeConstraintSetUpdateTypeDef",
     "SqlInjectionMatchSetTypeDef",
     "SqlInjectionMatchSetUpdateTypeDef",
@@ -233,14 +235,16 @@
     "UpdateIPSetRequestRequestTypeDef",
     "CreateRateBasedRuleResponseTypeDef",
     "GetRateBasedRuleResponseTypeDef",
     "CreateRuleResponseTypeDef",
     "GetRuleResponseTypeDef",
     "UpdateRateBasedRuleRequestRequestTypeDef",
     "UpdateRuleRequestRequestTypeDef",
+    "GetSampledRequestsRequestRequestTypeDef",
+    "TimeWindowUnionTypeDef",
     "CreateWebACLResponseTypeDef",
     "GetWebACLResponseTypeDef",
     "UpdateRuleGroupRequestRequestTypeDef",
     "UpdateWebACLRequestRequestTypeDef",
     "CreateByteMatchSetResponseTypeDef",
     "GetByteMatchSetResponseTypeDef",
     "UpdateByteMatchSetRequestRequestTypeDef",
@@ -284,14 +288,15 @@
     "AssociateWebACLRequestRequestTypeDef",
     {
         "WebACLId": str,
         "ResourceArn": str,
     },
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 ByteMatchSetSummaryTypeDef = TypedDict(
     "ByteMatchSetSummaryTypeDef",
     {
         "ByteMatchSetId": str,
         "Name": str,
     },
 )
@@ -667,22 +672,14 @@
 GetRuleRequestRequestTypeDef = TypedDict(
     "GetRuleRequestRequestTypeDef",
     {
         "RuleId": str,
     },
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
@@ -1018,14 +1015,15 @@
     "RegexPatternSetUpdateTypeDef",
     {
         "Action": ChangeActionType,
         "RegexPatternString": str,
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
@@ -1084,15 +1082,15 @@
     },
 )
 
 ByteMatchTupleTypeDef = TypedDict(
     "ByteMatchTupleTypeDef",
     {
         "FieldToMatch": FieldToMatchTypeDef,
-        "TargetString": Union[str, bytes, IO[Any], StreamingBody],
+        "TargetString": BlobTypeDef,
         "TextTransformation": TextTransformationType,
         "PositionalConstraint": PositionalConstraintType,
     },
 )
 
 _RequiredLoggingConfigurationOutputTypeDef = TypedDict(
     "_RequiredLoggingConfigurationOutputTypeDef",
@@ -1589,24 +1587,14 @@
     {
         "NextMarker": str,
         "GeoMatchSets": List[GeoMatchSetSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetSampledRequestsRequestRequestTypeDef = TypedDict(
-    "GetSampledRequestsRequestRequestTypeDef",
-    {
-        "WebAclId": str,
-        "RuleId": str,
-        "TimeWindow": TimeWindowTypeDef,
-        "MaxItems": int,
-    },
-)
-
 GetWebACLForResourceResponseTypeDef = TypedDict(
     "GetWebACLForResourceResponseTypeDef",
     {
         "WebACLSummary": WebACLSummaryTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1802,14 +1790,22 @@
     {
         "RegexPatternSetId": str,
         "Updates": Sequence[RegexPatternSetUpdateTypeDef],
         "ChangeToken": str,
     },
 )
 
+TimeWindowTypeDef = TypedDict(
+    "TimeWindowTypeDef",
+    {
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+    },
+)
+
 ListActivatedRulesInRuleGroupResponseTypeDef = TypedDict(
     "ListActivatedRulesInRuleGroupResponseTypeDef",
     {
         "NextMarker": str,
         "ActivatedRules": List[ActivatedRuleOutputTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1899,14 +1895,17 @@
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
 
@@ -2142,14 +2141,25 @@
     {
         "RuleId": str,
         "ChangeToken": str,
         "Updates": Sequence[RuleUpdateTypeDef],
     },
 )
 
+GetSampledRequestsRequestRequestTypeDef = TypedDict(
+    "GetSampledRequestsRequestRequestTypeDef",
+    {
+        "WebAclId": str,
+        "RuleId": str,
+        "TimeWindow": TimeWindowTypeDef,
+        "MaxItems": int,
+    },
+)
+
+TimeWindowUnionTypeDef = Union[TimeWindowTypeDef, TimeWindowOutputTypeDef]
 CreateWebACLResponseTypeDef = TypedDict(
     "CreateWebACLResponseTypeDef",
     {
         "WebACL": WebACLTypeDef,
         "ChangeToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-waf-regional-1.28.15.post1/mypy_boto3_waf_regional.egg-info/PKG-INFO` & `mypy-boto3-waf-regional-1.28.16/mypy_boto3_waf_regional.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-waf-regional
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.WAFRegional 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.WAFRegional 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf_regional/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 waf-regional type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 waf-regional type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-waf-regional.svg?color=blue)](https://pypi.org/project/mypy-boto3-waf-regional)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf_regional/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-waf-regional)](https://pepy.tech/project/mypy-boto3-waf-regional)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WAFRegional 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional)
+[boto3.WAFRegional 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional)
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
 [mypy-boto3-waf-regional docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf_regional/).
 
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
@@ -302,27 +302,28 @@
 )
 
 
 def check_value(value: ChangeActionType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_waf_regional.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_waf_regional.type_defs import (
     ExcludedRuleTypeDef,
     WafActionTypeDef,
     WafOverrideActionTypeDef,
     AssociateWebACLRequestRequestTypeDef,
+    BlobTypeDef,
     ByteMatchSetSummaryTypeDef,
     FieldToMatchTypeDef,
     CreateByteMatchSetRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     CreateGeoMatchSetRequestRequestTypeDef,
     CreateIPSetRequestRequestTypeDef,
     TagTypeDef,
@@ -359,15 +360,14 @@
     GetPermissionPolicyRequestRequestTypeDef,
     GetRateBasedRuleManagedKeysRequestRequestTypeDef,
     GetRateBasedRuleRequestRequestTypeDef,
     GetRegexMatchSetRequestRequestTypeDef,
     GetRegexPatternSetRequestRequestTypeDef,
     GetRuleGroupRequestRequestTypeDef,
     GetRuleRequestRequestTypeDef,
-    TimeWindowTypeDef,
     TimeWindowOutputTypeDef,
     GetSizeConstraintSetRequestRequestTypeDef,
     GetSqlInjectionMatchSetRequestRequestTypeDef,
     GetWebACLForResourceRequestRequestTypeDef,
     WebACLSummaryTypeDef,
     GetWebACLRequestRequestTypeDef,
     GetXssMatchSetRequestRequestTypeDef,
@@ -398,14 +398,15 @@
     ListTagsForResourceRequestRequestTypeDef,
     ListWebACLsRequestRequestTypeDef,
     ListXssMatchSetsRequestRequestTypeDef,
     XssMatchSetSummaryTypeDef,
     PredicateTypeDef,
     PutPermissionPolicyRequestRequestTypeDef,
     RegexPatternSetUpdateTypeDef,
+    TimestampTypeDef,
     UntagResourceRequestRequestTypeDef,
     ActivatedRuleOutputTypeDef,
     ActivatedRuleTypeDef,
     ByteMatchTupleOutputTypeDef,
     ByteMatchTupleTypeDef,
     LoggingConfigurationOutputTypeDef,
     LoggingConfigurationTypeDef,
@@ -453,15 +454,14 @@
     CreateRegexPatternSetResponseTypeDef,
     GetRegexPatternSetResponseTypeDef,
     CreateRuleGroupResponseTypeDef,
     GetRuleGroupResponseTypeDef,
     GeoMatchSetTypeDef,
     GeoMatchSetUpdateTypeDef,
     ListGeoMatchSetsResponseTypeDef,
-    GetSampledRequestsRequestRequestTypeDef,
     GetWebACLForResourceResponseTypeDef,
     ListWebACLsResponseTypeDef,
     HTTPRequestTypeDef,
     IPSetTypeDef,
     IPSetUpdateTypeDef,
     ListIPSetsResponseTypeDef,
     ListRateBasedRulesResponseTypeDef,
@@ -473,23 +473,25 @@
     ListSqlInjectionMatchSetsResponseTypeDef,
     ListSubscribedRuleGroupsResponseTypeDef,
     ListXssMatchSetsResponseTypeDef,
     RateBasedRuleTypeDef,
     RuleTypeDef,
     RuleUpdateTypeDef,
     UpdateRegexPatternSetRequestRequestTypeDef,
+    TimeWindowTypeDef,
     ListActivatedRulesInRuleGroupResponseTypeDef,
     WebACLTypeDef,
     RuleGroupUpdateTypeDef,
     WebACLUpdateTypeDef,
     ByteMatchSetTypeDef,
     ByteMatchSetUpdateTypeDef,
     GetLoggingConfigurationResponseTypeDef,
     ListLoggingConfigurationsResponseTypeDef,
     PutLoggingConfigurationResponseTypeDef,
+    LoggingConfigurationUnionTypeDef,
     PutLoggingConfigurationRequestRequestTypeDef,
     RegexMatchSetTypeDef,
     RegexMatchSetUpdateTypeDef,
     SizeConstraintSetTypeDef,
     SizeConstraintSetUpdateTypeDef,
     SqlInjectionMatchSetTypeDef,
     SqlInjectionMatchSetUpdateTypeDef,
@@ -505,14 +507,16 @@
     UpdateIPSetRequestRequestTypeDef,
     CreateRateBasedRuleResponseTypeDef,
     GetRateBasedRuleResponseTypeDef,
     CreateRuleResponseTypeDef,
     GetRuleResponseTypeDef,
     UpdateRateBasedRuleRequestRequestTypeDef,
     UpdateRuleRequestRequestTypeDef,
+    GetSampledRequestsRequestRequestTypeDef,
+    TimeWindowUnionTypeDef,
     CreateWebACLResponseTypeDef,
     GetWebACLResponseTypeDef,
     UpdateRuleGroupRequestRequestTypeDef,
     UpdateWebACLRequestRequestTypeDef,
     CreateByteMatchSetResponseTypeDef,
     GetByteMatchSetResponseTypeDef,
     UpdateByteMatchSetRequestRequestTypeDef,
@@ -528,15 +532,15 @@
     CreateXssMatchSetResponseTypeDef,
     GetXssMatchSetResponseTypeDef,
     UpdateXssMatchSetRequestRequestTypeDef,
     GetSampledRequestsResponseTypeDef,
 )
 
 
-def get_structure() -> ExcludedRuleTypeDef:
+def get_value() -> ExcludedRuleTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-waf-regional-1.28.15.post1/mypy_boto3_waf_regional.egg-info/SOURCES.txt` & `mypy-boto3-waf-regional-1.28.16/mypy_boto3_waf_regional.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-waf-regional-1.28.15.post1/setup.py` & `mypy-boto3-waf-regional-1.28.16/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-waf-regional",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_waf_regional"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.WAFRegional 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.2"
+        "Type annotations for boto3.WAFRegional 1.28.16 service generated with mypy-boto3-builder"
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
-    keywords="boto3 waf-regional type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 waf-regional type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_waf_regional": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf_regional/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

