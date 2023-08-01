# Comparing `tmp/mypy-boto3-waf-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-waf-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-waf-1.28.15.post1.tar", last modified: Sat Jul 29 10:04:23 2023, max compression
+gzip compressed data, was "mypy-boto3-waf-1.28.16.tar", last modified: Tue Aug  1 11:38:03 2023, max compression
```

## Comparing `mypy-boto3-waf-1.28.15.post1.tar` & `mypy-boto3-waf-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:23.941450 mypy-boto3-waf-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 10:01:12.000000 mypy-boto3-waf-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    24366 2023-07-29 10:04:23.937450 mypy-boto3-waf-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22889 2023-07-29 10:01:12.000000 mypy-boto3-waf-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:23.929450 mypy-boto3-waf-1.28.15.post1/mypy_boto3_waf/
--rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-07-29 10:01:12.000000 mypy-boto3-waf-1.28.15.post1/mypy_boto3_waf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3943 2023-07-29 10:01:12.000000 mypy-boto3-waf-1.28.15.post1/mypy_boto3_waf/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-29 10:01:12.000000 mypy-boto3-waf-1.28.15.post1/mypy_boto3_waf/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49647 2023-07-29 10:01:13.000000 mypy-boto3-waf-1.28.15.post1/mypy_boto3_waf/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    49547 2023-07-29 10:01:12.000000 mypy-boto3-waf-1.28.15.post1/mypy_boto3_waf/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13754 2023-07-29 10:01:13.000000 mypy-boto3-waf-1.28.15.post1/mypy_boto3_waf/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13752 2023-07-29 10:01:13.000000 mypy-boto3-waf-1.28.15.post1/mypy_boto3_waf/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    17639 2023-07-29 10:01:13.000000 mypy-boto3-waf-1.28.15.post1/mypy_boto3_waf/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    17621 2023-07-29 10:01:13.000000 mypy-boto3-waf-1.28.15.post1/mypy_boto3_waf/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 10:01:12.000000 mypy-boto3-waf-1.28.15.post1/mypy_boto3_waf/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    60886 2023-07-29 10:01:15.000000 mypy-boto3-waf-1.28.15.post1/mypy_boto3_waf/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    60835 2023-07-29 10:01:14.000000 mypy-boto3-waf-1.28.15.post1/mypy_boto3_waf/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 10:01:12.000000 mypy-boto3-waf-1.28.15.post1/mypy_boto3_waf/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:23.937450 mypy-boto3-waf-1.28.15.post1/mypy_boto3_waf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    24366 2023-07-29 10:04:23.000000 mypy-boto3-waf-1.28.15.post1/mypy_boto3_waf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-29 10:04:23.000000 mypy-boto3-waf-1.28.15.post1/mypy_boto3_waf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:23.000000 mypy-boto3-waf-1.28.15.post1/mypy_boto3_waf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:23.000000 mypy-boto3-waf-1.28.15.post1/mypy_boto3_waf.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:04:23.000000 mypy-boto3-waf-1.28.15.post1/mypy_boto3_waf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-29 10:04:23.000000 mypy-boto3-waf-1.28.15.post1/mypy_boto3_waf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:04:23.941450 mypy-boto3-waf-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-29 10:01:12.000000 mypy-boto3-waf-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:38:03.720675 mypy-boto3-waf-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:34:51.000000 mypy-boto3-waf-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    24461 2023-08-01 11:38:03.700675 mypy-boto3-waf-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22993 2023-08-01 11:34:51.000000 mypy-boto3-waf-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:38:03.700675 mypy-boto3-waf-1.28.16/mypy_boto3_waf/
+-rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-08-01 11:34:51.000000 mypy-boto3-waf-1.28.16/mypy_boto3_waf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3943 2023-08-01 11:34:51.000000 mypy-boto3-waf-1.28.16/mypy_boto3_waf/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-08-01 11:34:51.000000 mypy-boto3-waf-1.28.16/mypy_boto3_waf/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49462 2023-08-01 11:34:52.000000 mypy-boto3-waf-1.28.16/mypy_boto3_waf/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49362 2023-08-01 11:34:51.000000 mypy-boto3-waf-1.28.16/mypy_boto3_waf/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13754 2023-08-01 11:34:52.000000 mypy-boto3-waf-1.28.16/mypy_boto3_waf/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13752 2023-08-01 11:34:52.000000 mypy-boto3-waf-1.28.16/mypy_boto3_waf/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    17639 2023-08-01 11:34:52.000000 mypy-boto3-waf-1.28.16/mypy_boto3_waf/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17621 2023-08-01 11:34:52.000000 mypy-boto3-waf-1.28.16/mypy_boto3_waf/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:34:51.000000 mypy-boto3-waf-1.28.16/mypy_boto3_waf/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    61241 2023-08-01 11:34:58.000000 mypy-boto3-waf-1.28.16/mypy_boto3_waf/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61190 2023-08-01 11:34:57.000000 mypy-boto3-waf-1.28.16/mypy_boto3_waf/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:34:51.000000 mypy-boto3-waf-1.28.16/mypy_boto3_waf/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:38:03.700675 mypy-boto3-waf-1.28.16/mypy_boto3_waf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    24461 2023-08-01 11:38:03.000000 mypy-boto3-waf-1.28.16/mypy_boto3_waf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-08-01 11:38:03.000000 mypy-boto3-waf-1.28.16/mypy_boto3_waf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:38:03.000000 mypy-boto3-waf-1.28.16/mypy_boto3_waf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:38:03.000000 mypy-boto3-waf-1.28.16/mypy_boto3_waf.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:38:03.000000 mypy-boto3-waf-1.28.16/mypy_boto3_waf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-01 11:38:03.000000 mypy-boto3-waf-1.28.16/mypy_boto3_waf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:38:03.720675 mypy-boto3-waf-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-08-01 11:34:51.000000 mypy-boto3-waf-1.28.16/setup.py
```

### Comparing `mypy-boto3-waf-1.28.15.post1/LICENSE` & `mypy-boto3-waf-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-waf-1.28.15.post1/PKG-INFO` & `mypy-boto3-waf-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-waf
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.WAF 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.WAF 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 waf type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 waf type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-waf.svg?color=blue)](https://pypi.org/project/mypy-boto3-waf)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-waf)](https://pepy.tech/project/mypy-boto3-waf)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WAF 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF)
+[boto3.WAF 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF)
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
 [mypy-boto3-waf docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/).
 
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
@@ -392,26 +392,27 @@
 )
 
 
 def check_value(value: ChangeActionType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_waf.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_waf.type_defs import (
     ExcludedRuleTypeDef,
     WafActionTypeDef,
     WafOverrideActionTypeDef,
+    BlobTypeDef,
     ByteMatchSetSummaryTypeDef,
     FieldToMatchTypeDef,
     CreateByteMatchSetRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     CreateGeoMatchSetRequestRequestTypeDef,
     CreateIPSetRequestRequestTypeDef,
     TagTypeDef,
@@ -448,15 +449,14 @@
     PaginatorConfigTypeDef,
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
     GetWebACLRequestRequestTypeDef,
     GetXssMatchSetRequestRequestTypeDef,
     HTTPHeaderTypeDef,
     IPSetDescriptorTypeDef,
@@ -485,14 +485,15 @@
     ListWebACLsRequestRequestTypeDef,
     WebACLSummaryTypeDef,
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
@@ -555,15 +556,14 @@
     ListRuleGroupsRequestListRuleGroupsPaginateTypeDef,
     ListRulesRequestListRulesPaginateTypeDef,
     ListSizeConstraintSetsRequestListSizeConstraintSetsPaginateTypeDef,
     ListSqlInjectionMatchSetsRequestListSqlInjectionMatchSetsPaginateTypeDef,
     ListSubscribedRuleGroupsRequestListSubscribedRuleGroupsPaginateTypeDef,
     ListWebACLsRequestListWebACLsPaginateTypeDef,
     ListXssMatchSetsRequestListXssMatchSetsPaginateTypeDef,
-    GetSampledRequestsRequestRequestTypeDef,
     HTTPRequestTypeDef,
     IPSetTypeDef,
     IPSetUpdateTypeDef,
     ListIPSetsResponseTypeDef,
     ListRateBasedRulesResponseTypeDef,
     ListRulesResponseTypeDef,
     ListRegexMatchSetsResponseTypeDef,
@@ -574,23 +574,25 @@
     ListSubscribedRuleGroupsResponseTypeDef,
     ListWebACLsResponseTypeDef,
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
@@ -606,14 +608,16 @@
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
@@ -629,15 +633,15 @@
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

### Comparing `mypy-boto3-waf-1.28.15.post1/README.md` & `mypy-boto3-waf-1.28.16/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-waf.svg?color=blue)](https://pypi.org/project/mypy-boto3-waf)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-waf)](https://pepy.tech/project/mypy-boto3-waf)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WAF 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF)
+[boto3.WAF 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF)
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
 [mypy-boto3-waf docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/).
 
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
@@ -360,26 +360,27 @@
 )
 
 
 def check_value(value: ChangeActionType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_waf.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_waf.type_defs import (
     ExcludedRuleTypeDef,
     WafActionTypeDef,
     WafOverrideActionTypeDef,
+    BlobTypeDef,
     ByteMatchSetSummaryTypeDef,
     FieldToMatchTypeDef,
     CreateByteMatchSetRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     CreateGeoMatchSetRequestRequestTypeDef,
     CreateIPSetRequestRequestTypeDef,
     TagTypeDef,
@@ -416,15 +417,14 @@
     PaginatorConfigTypeDef,
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
     GetWebACLRequestRequestTypeDef,
     GetXssMatchSetRequestRequestTypeDef,
     HTTPHeaderTypeDef,
     IPSetDescriptorTypeDef,
@@ -453,14 +453,15 @@
     ListWebACLsRequestRequestTypeDef,
     WebACLSummaryTypeDef,
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
@@ -523,15 +524,14 @@
     ListRuleGroupsRequestListRuleGroupsPaginateTypeDef,
     ListRulesRequestListRulesPaginateTypeDef,
     ListSizeConstraintSetsRequestListSizeConstraintSetsPaginateTypeDef,
     ListSqlInjectionMatchSetsRequestListSqlInjectionMatchSetsPaginateTypeDef,
     ListSubscribedRuleGroupsRequestListSubscribedRuleGroupsPaginateTypeDef,
     ListWebACLsRequestListWebACLsPaginateTypeDef,
     ListXssMatchSetsRequestListXssMatchSetsPaginateTypeDef,
-    GetSampledRequestsRequestRequestTypeDef,
     HTTPRequestTypeDef,
     IPSetTypeDef,
     IPSetUpdateTypeDef,
     ListIPSetsResponseTypeDef,
     ListRateBasedRulesResponseTypeDef,
     ListRulesResponseTypeDef,
     ListRegexMatchSetsResponseTypeDef,
@@ -542,23 +542,25 @@
     ListSubscribedRuleGroupsResponseTypeDef,
     ListWebACLsResponseTypeDef,
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
@@ -574,14 +576,16 @@
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
@@ -597,15 +601,15 @@
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

### Comparing `mypy-boto3-waf-1.28.15.post1/mypy_boto3_waf/__init__.py` & `mypy-boto3-waf-1.28.16/mypy_boto3_waf/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-waf-1.28.15.post1/mypy_boto3_waf/__init__.pyi` & `mypy-boto3-waf-1.28.16/mypy_boto3_waf/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-waf-1.28.15.post1/mypy_boto3_waf/__main__.py` & `mypy-boto3-waf-1.28.16/mypy_boto3_waf/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.WAF 1.28.15\nVersion:         1.28.15.post1\nBuilder version:"
-        " 7.16.2\nDocs:           "
+        "Type annotations for boto3.WAF 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF\nOther"
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

### Comparing `mypy-boto3-waf-1.28.15.post1/mypy_boto3_waf/client.py` & `mypy-boto3-waf-1.28.16/mypy_boto3_waf/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_waf.client import WAFClient
 
     session = Session()
     client: WAFClient = session.client("waf")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .paginator import (
     GetRateBasedRuleManagedKeysPaginator,
     ListActivatedRulesInRuleGroupPaginator,
     ListByteMatchSetsPaginator,
@@ -95,26 +95,24 @@
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
@@ -592,20 +590,15 @@
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.get_rule_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/client/#get_rule_group)
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
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.get_sampled_requests)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/client/#get_sampled_requests)
         """
@@ -799,17 +792,15 @@
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.list_xss_match_sets)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/client/#list_xss_match_sets)
         """
 
     def put_logging_configuration(
-        self,
-        *,
-        LoggingConfiguration: Union[LoggingConfigurationTypeDef, LoggingConfigurationOutputTypeDef]
+        self, *, LoggingConfiguration: LoggingConfigurationUnionTypeDef
     ) -> PutLoggingConfigurationResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.put_logging_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/client/#put_logging_configuration)
         """
```

### Comparing `mypy-boto3-waf-1.28.15.post1/mypy_boto3_waf/client.pyi` & `mypy-boto3-waf-1.28.16/mypy_boto3_waf/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_waf.client import WAFClient
 
     session = Session()
     client: WAFClient = session.client("waf")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .paginator import (
     GetRateBasedRuleManagedKeysPaginator,
     ListActivatedRulesInRuleGroupPaginator,
     ListByteMatchSetsPaginator,
@@ -95,26 +95,24 @@
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
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.get_rule_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/client/#get_rule_group)
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
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.get_sampled_requests)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/client/#get_sampled_requests)
         """
@@ -730,17 +723,15 @@
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.list_xss_match_sets)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/client/#list_xss_match_sets)
         """
     def put_logging_configuration(
-        self,
-        *,
-        LoggingConfiguration: Union[LoggingConfigurationTypeDef, LoggingConfigurationOutputTypeDef]
+        self, *, LoggingConfiguration: LoggingConfigurationUnionTypeDef
     ) -> PutLoggingConfigurationResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF.Client.put_logging_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/client/#put_logging_configuration)
         """
```

### Comparing `mypy-boto3-waf-1.28.15.post1/mypy_boto3_waf/literals.py` & `mypy-boto3-waf-1.28.16/mypy_boto3_waf/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-waf-1.28.15.post1/mypy_boto3_waf/literals.pyi` & `mypy-boto3-waf-1.28.16/mypy_boto3_waf/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-waf-1.28.15.post1/mypy_boto3_waf/paginator.py` & `mypy-boto3-waf-1.28.16/mypy_boto3_waf/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-waf-1.28.15.post1/mypy_boto3_waf/paginator.pyi` & `mypy-boto3-waf-1.28.16/mypy_boto3_waf/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-waf-1.28.15.post1/mypy_boto3_waf/type_defs.py` & `mypy-boto3-waf-1.28.16/mypy_boto3_waf/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_waf.type_defs import ExcludedRuleTypeDef
 
-    data: ExcludedRuleTypeDef = {...}
+    data: ExcludedRuleTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -42,14 +42,15 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "ExcludedRuleTypeDef",
     "WafActionTypeDef",
     "WafOverrideActionTypeDef",
+    "BlobTypeDef",
     "ByteMatchSetSummaryTypeDef",
     "FieldToMatchTypeDef",
     "CreateByteMatchSetRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "CreateGeoMatchSetRequestRequestTypeDef",
     "CreateIPSetRequestRequestTypeDef",
     "TagTypeDef",
@@ -86,15 +87,14 @@
     "PaginatorConfigTypeDef",
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
     "GetWebACLRequestRequestTypeDef",
     "GetXssMatchSetRequestRequestTypeDef",
     "HTTPHeaderTypeDef",
     "IPSetDescriptorTypeDef",
@@ -123,14 +123,15 @@
     "ListWebACLsRequestRequestTypeDef",
     "WebACLSummaryTypeDef",
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
@@ -193,15 +194,14 @@
     "ListRuleGroupsRequestListRuleGroupsPaginateTypeDef",
     "ListRulesRequestListRulesPaginateTypeDef",
     "ListSizeConstraintSetsRequestListSizeConstraintSetsPaginateTypeDef",
     "ListSqlInjectionMatchSetsRequestListSqlInjectionMatchSetsPaginateTypeDef",
     "ListSubscribedRuleGroupsRequestListSubscribedRuleGroupsPaginateTypeDef",
     "ListWebACLsRequestListWebACLsPaginateTypeDef",
     "ListXssMatchSetsRequestListXssMatchSetsPaginateTypeDef",
-    "GetSampledRequestsRequestRequestTypeDef",
     "HTTPRequestTypeDef",
     "IPSetTypeDef",
     "IPSetUpdateTypeDef",
     "ListIPSetsResponseTypeDef",
     "ListRateBasedRulesResponseTypeDef",
     "ListRulesResponseTypeDef",
     "ListRegexMatchSetsResponseTypeDef",
@@ -212,23 +212,25 @@
     "ListSubscribedRuleGroupsResponseTypeDef",
     "ListWebACLsResponseTypeDef",
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
@@ -244,14 +246,16 @@
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
@@ -287,14 +291,15 @@
 WafOverrideActionTypeDef = TypedDict(
     "WafOverrideActionTypeDef",
     {
         "Type": WafOverrideActionTypeType,
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
@@ -681,22 +686,14 @@
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
@@ -1007,14 +1004,15 @@
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
@@ -1077,15 +1075,15 @@
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
@@ -1731,24 +1729,14 @@
     "ListXssMatchSetsRequestListXssMatchSetsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
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
 HTTPRequestTypeDef = TypedDict(
     "HTTPRequestTypeDef",
     {
         "ClientIP": str,
         "Country": str,
         "URI": str,
         "Method": str,
@@ -1942,14 +1930,22 @@
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
@@ -2043,14 +2039,17 @@
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
 
@@ -2294,14 +2293,25 @@
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

### Comparing `mypy-boto3-waf-1.28.15.post1/mypy_boto3_waf/type_defs.pyi` & `mypy-boto3-waf-1.28.16/mypy_boto3_waf/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_waf.type_defs import ExcludedRuleTypeDef
 
-    data: ExcludedRuleTypeDef = {...}
+    data: ExcludedRuleTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -41,14 +41,15 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "ExcludedRuleTypeDef",
     "WafActionTypeDef",
     "WafOverrideActionTypeDef",
+    "BlobTypeDef",
     "ByteMatchSetSummaryTypeDef",
     "FieldToMatchTypeDef",
     "CreateByteMatchSetRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "CreateGeoMatchSetRequestRequestTypeDef",
     "CreateIPSetRequestRequestTypeDef",
     "TagTypeDef",
@@ -85,15 +86,14 @@
     "PaginatorConfigTypeDef",
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
     "GetWebACLRequestRequestTypeDef",
     "GetXssMatchSetRequestRequestTypeDef",
     "HTTPHeaderTypeDef",
     "IPSetDescriptorTypeDef",
@@ -122,14 +122,15 @@
     "ListWebACLsRequestRequestTypeDef",
     "WebACLSummaryTypeDef",
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
@@ -192,15 +193,14 @@
     "ListRuleGroupsRequestListRuleGroupsPaginateTypeDef",
     "ListRulesRequestListRulesPaginateTypeDef",
     "ListSizeConstraintSetsRequestListSizeConstraintSetsPaginateTypeDef",
     "ListSqlInjectionMatchSetsRequestListSqlInjectionMatchSetsPaginateTypeDef",
     "ListSubscribedRuleGroupsRequestListSubscribedRuleGroupsPaginateTypeDef",
     "ListWebACLsRequestListWebACLsPaginateTypeDef",
     "ListXssMatchSetsRequestListXssMatchSetsPaginateTypeDef",
-    "GetSampledRequestsRequestRequestTypeDef",
     "HTTPRequestTypeDef",
     "IPSetTypeDef",
     "IPSetUpdateTypeDef",
     "ListIPSetsResponseTypeDef",
     "ListRateBasedRulesResponseTypeDef",
     "ListRulesResponseTypeDef",
     "ListRegexMatchSetsResponseTypeDef",
@@ -211,23 +211,25 @@
     "ListSubscribedRuleGroupsResponseTypeDef",
     "ListWebACLsResponseTypeDef",
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
@@ -243,14 +245,16 @@
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
@@ -286,14 +290,15 @@
 WafOverrideActionTypeDef = TypedDict(
     "WafOverrideActionTypeDef",
     {
         "Type": WafOverrideActionTypeType,
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
@@ -672,22 +677,14 @@
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
@@ -996,14 +993,15 @@
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
@@ -1062,15 +1060,15 @@
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
@@ -1700,24 +1698,14 @@
     "ListXssMatchSetsRequestListXssMatchSetsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
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
 HTTPRequestTypeDef = TypedDict(
     "HTTPRequestTypeDef",
     {
         "ClientIP": str,
         "Country": str,
         "URI": str,
         "Method": str,
@@ -1905,14 +1893,22 @@
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
@@ -2002,14 +1998,17 @@
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
 
@@ -2245,14 +2244,25 @@
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

### Comparing `mypy-boto3-waf-1.28.15.post1/mypy_boto3_waf.egg-info/PKG-INFO` & `mypy-boto3-waf-1.28.16/mypy_boto3_waf.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-waf
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.WAF 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.WAF 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 waf type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 waf type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-waf.svg?color=blue)](https://pypi.org/project/mypy-boto3-waf)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-waf)](https://pepy.tech/project/mypy-boto3-waf)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WAF 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF)
+[boto3.WAF 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#WAF)
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
 [mypy-boto3-waf docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/).
 
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
@@ -392,26 +392,27 @@
 )
 
 
 def check_value(value: ChangeActionType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_waf.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_waf.type_defs import (
     ExcludedRuleTypeDef,
     WafActionTypeDef,
     WafOverrideActionTypeDef,
+    BlobTypeDef,
     ByteMatchSetSummaryTypeDef,
     FieldToMatchTypeDef,
     CreateByteMatchSetRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     CreateGeoMatchSetRequestRequestTypeDef,
     CreateIPSetRequestRequestTypeDef,
     TagTypeDef,
@@ -448,15 +449,14 @@
     PaginatorConfigTypeDef,
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
     GetWebACLRequestRequestTypeDef,
     GetXssMatchSetRequestRequestTypeDef,
     HTTPHeaderTypeDef,
     IPSetDescriptorTypeDef,
@@ -485,14 +485,15 @@
     ListWebACLsRequestRequestTypeDef,
     WebACLSummaryTypeDef,
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
@@ -555,15 +556,14 @@
     ListRuleGroupsRequestListRuleGroupsPaginateTypeDef,
     ListRulesRequestListRulesPaginateTypeDef,
     ListSizeConstraintSetsRequestListSizeConstraintSetsPaginateTypeDef,
     ListSqlInjectionMatchSetsRequestListSqlInjectionMatchSetsPaginateTypeDef,
     ListSubscribedRuleGroupsRequestListSubscribedRuleGroupsPaginateTypeDef,
     ListWebACLsRequestListWebACLsPaginateTypeDef,
     ListXssMatchSetsRequestListXssMatchSetsPaginateTypeDef,
-    GetSampledRequestsRequestRequestTypeDef,
     HTTPRequestTypeDef,
     IPSetTypeDef,
     IPSetUpdateTypeDef,
     ListIPSetsResponseTypeDef,
     ListRateBasedRulesResponseTypeDef,
     ListRulesResponseTypeDef,
     ListRegexMatchSetsResponseTypeDef,
@@ -574,23 +574,25 @@
     ListSubscribedRuleGroupsResponseTypeDef,
     ListWebACLsResponseTypeDef,
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
@@ -606,14 +608,16 @@
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
@@ -629,15 +633,15 @@
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

### Comparing `mypy-boto3-waf-1.28.15.post1/mypy_boto3_waf.egg-info/SOURCES.txt` & `mypy-boto3-waf-1.28.16/mypy_boto3_waf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-waf-1.28.15.post1/setup.py` & `mypy-boto3-waf-1.28.16/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-waf",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_waf"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.WAF 1.28.15 service generated with mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.WAF 1.28.16 service generated with mypy-boto3-builder 7.17.1"
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
-    keywords="boto3 waf type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 waf type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_waf": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

