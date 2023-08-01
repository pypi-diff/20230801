# Comparing `tmp/mypy-boto3-shield-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-shield-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-shield-1.28.15.post1.tar", last modified: Sat Jul 29 10:04:12 2023, max compression
+gzip compressed data, was "mypy-boto3-shield-1.28.16.tar", last modified: Tue Aug  1 11:37:51 2023, max compression
```

## Comparing `mypy-boto3-shield-1.28.15.post1.tar` & `mypy-boto3-shield-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:12.497405 mypy-boto3-shield-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:59:40.000000 mypy-boto3-shield-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15821 2023-07-29 10:04:12.497405 mypy-boto3-shield-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14332 2023-07-29 09:59:40.000000 mypy-boto3-shield-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:12.477405 mypy-boto3-shield-1.28.15.post1/mypy_boto3_shield/
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-29 09:59:40.000000 mypy-boto3-shield-1.28.15.post1/mypy_boto3_shield/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-29 09:59:40.000000 mypy-boto3-shield-1.28.15.post1/mypy_boto3_shield/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-29 09:59:40.000000 mypy-boto3-shield-1.28.15.post1/mypy_boto3_shield/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25777 2023-07-29 09:59:40.000000 mypy-boto3-shield-1.28.15.post1/mypy_boto3_shield/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    25732 2023-07-29 09:59:40.000000 mypy-boto3-shield-1.28.15.post1/mypy_boto3_shield/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9245 2023-07-29 09:59:41.000000 mypy-boto3-shield-1.28.15.post1/mypy_boto3_shield/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9243 2023-07-29 09:59:40.000000 mypy-boto3-shield-1.28.15.post1/mypy_boto3_shield/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-07-29 09:59:40.000000 mypy-boto3-shield-1.28.15.post1/mypy_boto3_shield/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-07-29 09:59:40.000000 mypy-boto3-shield-1.28.15.post1/mypy_boto3_shield/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:59:40.000000 mypy-boto3-shield-1.28.15.post1/mypy_boto3_shield/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    22632 2023-07-29 09:59:41.000000 mypy-boto3-shield-1.28.15.post1/mypy_boto3_shield/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    22613 2023-07-29 09:59:41.000000 mypy-boto3-shield-1.28.15.post1/mypy_boto3_shield/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:59:40.000000 mypy-boto3-shield-1.28.15.post1/mypy_boto3_shield/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:12.497405 mypy-boto3-shield-1.28.15.post1/mypy_boto3_shield.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15821 2023-07-29 10:04:12.000000 mypy-boto3-shield-1.28.15.post1/mypy_boto3_shield.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-29 10:04:12.000000 mypy-boto3-shield-1.28.15.post1/mypy_boto3_shield.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:12.000000 mypy-boto3-shield-1.28.15.post1/mypy_boto3_shield.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:12.000000 mypy-boto3-shield-1.28.15.post1/mypy_boto3_shield.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:04:12.000000 mypy-boto3-shield-1.28.15.post1/mypy_boto3_shield.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-29 10:04:12.000000 mypy-boto3-shield-1.28.15.post1/mypy_boto3_shield.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:04:12.497405 mypy-boto3-shield-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-29 09:59:40.000000 mypy-boto3-shield-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:51.988728 mypy-boto3-shield-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:33:13.000000 mypy-boto3-shield-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15892 2023-08-01 11:37:51.980728 mypy-boto3-shield-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14412 2023-08-01 11:33:13.000000 mypy-boto3-shield-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:51.972728 mypy-boto3-shield-1.28.16/mypy_boto3_shield/
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-08-01 11:33:13.000000 mypy-boto3-shield-1.28.16/mypy_boto3_shield/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-08-01 11:33:13.000000 mypy-boto3-shield-1.28.16/mypy_boto3_shield/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-08-01 11:33:13.000000 mypy-boto3-shield-1.28.16/mypy_boto3_shield/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25605 2023-08-01 11:33:13.000000 mypy-boto3-shield-1.28.16/mypy_boto3_shield/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25560 2023-08-01 11:33:13.000000 mypy-boto3-shield-1.28.16/mypy_boto3_shield/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9245 2023-08-01 11:33:13.000000 mypy-boto3-shield-1.28.16/mypy_boto3_shield/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9243 2023-08-01 11:33:13.000000 mypy-boto3-shield-1.28.16/mypy_boto3_shield/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-08-01 11:33:13.000000 mypy-boto3-shield-1.28.16/mypy_boto3_shield/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-08-01 11:33:13.000000 mypy-boto3-shield-1.28.16/mypy_boto3_shield/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:33:13.000000 mypy-boto3-shield-1.28.16/mypy_boto3_shield/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    22908 2023-08-01 11:33:14.000000 mypy-boto3-shield-1.28.16/mypy_boto3_shield/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22889 2023-08-01 11:33:14.000000 mypy-boto3-shield-1.28.16/mypy_boto3_shield/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:33:13.000000 mypy-boto3-shield-1.28.16/mypy_boto3_shield/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:51.980728 mypy-boto3-shield-1.28.16/mypy_boto3_shield.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15892 2023-08-01 11:37:51.000000 mypy-boto3-shield-1.28.16/mypy_boto3_shield.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-08-01 11:37:51.000000 mypy-boto3-shield-1.28.16/mypy_boto3_shield.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:51.000000 mypy-boto3-shield-1.28.16/mypy_boto3_shield.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:51.000000 mypy-boto3-shield-1.28.16/mypy_boto3_shield.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:51.000000 mypy-boto3-shield-1.28.16/mypy_boto3_shield.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-01 11:37:51.000000 mypy-boto3-shield-1.28.16/mypy_boto3_shield.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:51.988728 mypy-boto3-shield-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-08-01 11:33:13.000000 mypy-boto3-shield-1.28.16/setup.py
```

### Comparing `mypy-boto3-shield-1.28.15.post1/LICENSE` & `mypy-boto3-shield-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-shield-1.28.15.post1/PKG-INFO` & `mypy-boto3-shield-1.28.16/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-shield
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.Shield 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.Shield 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 shield type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 shield type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-shield.svg?color=blue)](https://pypi.org/project/mypy-boto3-shield)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-shield)](https://pepy.tech/project/mypy-boto3-shield)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Shield 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield)
+[boto3.Shield 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield)
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
 [mypy-boto3-shield docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield/).
 
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
@@ -321,20 +321,20 @@
 )
 
 
 def check_value(value: ApplicationLayerAutomaticResponseStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_shield.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_shield.type_defs import (
     ResponseActionOutputTypeDef,
     AssociateDRTLogBucketRequestRequestTypeDef,
     AssociateDRTRoleRequestRequestTypeDef,
     AssociateHealthCheckRequestRequestTypeDef,
@@ -357,18 +357,18 @@
     DisassociateDRTLogBucketRequestRequestTypeDef,
     DisassociateHealthCheckRequestRequestTypeDef,
     ResponseActionTypeDef,
     InclusionProtectionFiltersTypeDef,
     InclusionProtectionGroupFiltersTypeDef,
     LimitTypeDef,
     PaginatorConfigTypeDef,
-    TimeRangeTypeDef,
     ListResourcesInProtectionGroupRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ProtectionGroupArbitraryPatternLimitsTypeDef,
+    TimestampTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateProtectionGroupRequestRequestTypeDef,
     UpdateSubscriptionRequestRequestTypeDef,
     ApplicationLayerAutomaticResponseConfigurationTypeDef,
     AssociateProactiveEngagementDetailsRequestRequestTypeDef,
     UpdateEmergencyContactSettingsRequestRequestTypeDef,
     SummarizedAttackVectorTypeDef,
@@ -383,39 +383,42 @@
     DescribeEmergencyContactSettingsResponseTypeDef,
     GetSubscriptionStateResponseTypeDef,
     ListResourcesInProtectionGroupResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     DescribeProtectionGroupResponseTypeDef,
     ListProtectionGroupsResponseTypeDef,
     EnableApplicationLayerAutomaticResponseRequestRequestTypeDef,
+    ResponseActionUnionTypeDef,
     UpdateApplicationLayerAutomaticResponseRequestRequestTypeDef,
     ListProtectionsRequestRequestTypeDef,
     ListProtectionGroupsRequestRequestTypeDef,
     ProtectionLimitsTypeDef,
     ListProtectionsRequestListProtectionsPaginateTypeDef,
-    ListAttacksRequestListAttacksPaginateTypeDef,
-    ListAttacksRequestRequestTypeDef,
     ProtectionGroupPatternTypeLimitsTypeDef,
+    TimeRangeTypeDef,
     ProtectionTypeDef,
     SubResourceSummaryTypeDef,
     ListAttacksResponseTypeDef,
     AttackStatisticsDataItemTypeDef,
     ProtectionGroupLimitsTypeDef,
+    ListAttacksRequestListAttacksPaginateTypeDef,
+    ListAttacksRequestRequestTypeDef,
+    TimeRangeUnionTypeDef,
     DescribeProtectionResponseTypeDef,
     ListProtectionsResponseTypeDef,
     AttackDetailTypeDef,
     DescribeAttackStatisticsResponseTypeDef,
     SubscriptionLimitsTypeDef,
     DescribeAttackResponseTypeDef,
     SubscriptionTypeDef,
     DescribeSubscriptionResponseTypeDef,
 )
 
 
-def get_structure() -> ResponseActionOutputTypeDef:
+def get_value() -> ResponseActionOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-shield-1.28.15.post1/README.md` & `mypy-boto3-shield-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-shield.svg?color=blue)](https://pypi.org/project/mypy-boto3-shield)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-shield)](https://pepy.tech/project/mypy-boto3-shield)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Shield 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield)
+[boto3.Shield 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield)
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
 [mypy-boto3-shield docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield/).
 
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
@@ -289,20 +289,20 @@
 )
 
 
 def check_value(value: ApplicationLayerAutomaticResponseStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_shield.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_shield.type_defs import (
     ResponseActionOutputTypeDef,
     AssociateDRTLogBucketRequestRequestTypeDef,
     AssociateDRTRoleRequestRequestTypeDef,
     AssociateHealthCheckRequestRequestTypeDef,
@@ -325,18 +325,18 @@
     DisassociateDRTLogBucketRequestRequestTypeDef,
     DisassociateHealthCheckRequestRequestTypeDef,
     ResponseActionTypeDef,
     InclusionProtectionFiltersTypeDef,
     InclusionProtectionGroupFiltersTypeDef,
     LimitTypeDef,
     PaginatorConfigTypeDef,
-    TimeRangeTypeDef,
     ListResourcesInProtectionGroupRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ProtectionGroupArbitraryPatternLimitsTypeDef,
+    TimestampTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateProtectionGroupRequestRequestTypeDef,
     UpdateSubscriptionRequestRequestTypeDef,
     ApplicationLayerAutomaticResponseConfigurationTypeDef,
     AssociateProactiveEngagementDetailsRequestRequestTypeDef,
     UpdateEmergencyContactSettingsRequestRequestTypeDef,
     SummarizedAttackVectorTypeDef,
@@ -351,39 +351,42 @@
     DescribeEmergencyContactSettingsResponseTypeDef,
     GetSubscriptionStateResponseTypeDef,
     ListResourcesInProtectionGroupResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     DescribeProtectionGroupResponseTypeDef,
     ListProtectionGroupsResponseTypeDef,
     EnableApplicationLayerAutomaticResponseRequestRequestTypeDef,
+    ResponseActionUnionTypeDef,
     UpdateApplicationLayerAutomaticResponseRequestRequestTypeDef,
     ListProtectionsRequestRequestTypeDef,
     ListProtectionGroupsRequestRequestTypeDef,
     ProtectionLimitsTypeDef,
     ListProtectionsRequestListProtectionsPaginateTypeDef,
-    ListAttacksRequestListAttacksPaginateTypeDef,
-    ListAttacksRequestRequestTypeDef,
     ProtectionGroupPatternTypeLimitsTypeDef,
+    TimeRangeTypeDef,
     ProtectionTypeDef,
     SubResourceSummaryTypeDef,
     ListAttacksResponseTypeDef,
     AttackStatisticsDataItemTypeDef,
     ProtectionGroupLimitsTypeDef,
+    ListAttacksRequestListAttacksPaginateTypeDef,
+    ListAttacksRequestRequestTypeDef,
+    TimeRangeUnionTypeDef,
     DescribeProtectionResponseTypeDef,
     ListProtectionsResponseTypeDef,
     AttackDetailTypeDef,
     DescribeAttackStatisticsResponseTypeDef,
     SubscriptionLimitsTypeDef,
     DescribeAttackResponseTypeDef,
     SubscriptionTypeDef,
     DescribeSubscriptionResponseTypeDef,
 )
 
 
-def get_structure() -> ResponseActionOutputTypeDef:
+def get_value() -> ResponseActionOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-shield-1.28.15.post1/mypy_boto3_shield/__init__.py` & `mypy-boto3-shield-1.28.16/mypy_boto3_shield/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-shield-1.28.15.post1/mypy_boto3_shield/__init__.pyi` & `mypy-boto3-shield-1.28.16/mypy_boto3_shield/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-shield-1.28.15.post1/mypy_boto3_shield/__main__.py` & `mypy-boto3-shield-1.28.16/mypy_boto3_shield/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Shield 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.Shield 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield\nOther"
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

### Comparing `mypy-boto3-shield-1.28.15.post1/mypy_boto3_shield/client.py` & `mypy-boto3-shield-1.28.16/mypy_boto3_shield/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_shield.client import ShieldClient
 
     session = Session()
     client: ShieldClient = session.client("shield")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AutoRenewType,
     ProtectedResourceTypeType,
     ProtectionGroupAggregationType,
@@ -39,19 +39,17 @@
     InclusionProtectionFiltersTypeDef,
     InclusionProtectionGroupFiltersTypeDef,
     ListAttacksResponseTypeDef,
     ListProtectionGroupsResponseTypeDef,
     ListProtectionsResponseTypeDef,
     ListResourcesInProtectionGroupResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    ResponseActionOutputTypeDef,
-    ResponseActionTypeDef,
+    ResponseActionUnionTypeDef,
     TagTypeDef,
-    TimeRangeOutputTypeDef,
-    TimeRangeTypeDef,
+    TimeRangeUnionTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -328,15 +326,15 @@
         resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield.Client.disassociate_health_check)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield/client/#disassociate_health_check)
         """
 
     def enable_application_layer_automatic_response(
-        self, *, ResourceArn: str, Action: Union[ResponseActionTypeDef, ResponseActionOutputTypeDef]
+        self, *, ResourceArn: str, Action: ResponseActionUnionTypeDef
     ) -> Dict[str, Any]:
         """
         Enable the Shield Advanced automatic application layer DDoS mitigation for the
         protected resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield.Client.enable_application_layer_automatic_response)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield/client/#enable_application_layer_automatic_response)
@@ -374,16 +372,16 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield/client/#get_subscription_state)
         """
 
     def list_attacks(
         self,
         *,
         ResourceArns: Sequence[str] = ...,
-        StartTime: Union[TimeRangeTypeDef, TimeRangeOutputTypeDef] = ...,
-        EndTime: Union[TimeRangeTypeDef, TimeRangeOutputTypeDef] = ...,
+        StartTime: TimeRangeUnionTypeDef = ...,
+        EndTime: TimeRangeUnionTypeDef = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListAttacksResponseTypeDef:
         """
         Returns all ongoing DDoS attacks or all DDoS attacks during a specified time
         period.
 
@@ -451,15 +449,15 @@
         Removes tags from a resource in Shield.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield/client/#untag_resource)
         """
 
     def update_application_layer_automatic_response(
-        self, *, ResourceArn: str, Action: Union[ResponseActionTypeDef, ResponseActionOutputTypeDef]
+        self, *, ResourceArn: str, Action: ResponseActionUnionTypeDef
     ) -> Dict[str, Any]:
         """
         Updates an existing Shield Advanced automatic application layer DDoS mitigation
         configuration for the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield.Client.update_application_layer_automatic_response)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield/client/#update_application_layer_automatic_response)
```

### Comparing `mypy-boto3-shield-1.28.15.post1/mypy_boto3_shield/client.pyi` & `mypy-boto3-shield-1.28.16/mypy_boto3_shield/client.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_shield.client import ShieldClient
 
     session = Session()
     client: ShieldClient = session.client("shield")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AutoRenewType,
     ProtectedResourceTypeType,
     ProtectionGroupAggregationType,
@@ -39,19 +39,17 @@
     InclusionProtectionFiltersTypeDef,
     InclusionProtectionGroupFiltersTypeDef,
     ListAttacksResponseTypeDef,
     ListProtectionGroupsResponseTypeDef,
     ListProtectionsResponseTypeDef,
     ListResourcesInProtectionGroupResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    ResponseActionOutputTypeDef,
-    ResponseActionTypeDef,
+    ResponseActionUnionTypeDef,
     TagTypeDef,
-    TimeRangeOutputTypeDef,
-    TimeRangeTypeDef,
+    TimeRangeUnionTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -299,15 +297,15 @@
         Removes health-based detection from the Shield Advanced protection for a
         resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield.Client.disassociate_health_check)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield/client/#disassociate_health_check)
         """
     def enable_application_layer_automatic_response(
-        self, *, ResourceArn: str, Action: Union[ResponseActionTypeDef, ResponseActionOutputTypeDef]
+        self, *, ResourceArn: str, Action: ResponseActionUnionTypeDef
     ) -> Dict[str, Any]:
         """
         Enable the Shield Advanced automatic application layer DDoS mitigation for the
         protected resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield.Client.enable_application_layer_automatic_response)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield/client/#enable_application_layer_automatic_response)
@@ -341,16 +339,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield.Client.get_subscription_state)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield/client/#get_subscription_state)
         """
     def list_attacks(
         self,
         *,
         ResourceArns: Sequence[str] = ...,
-        StartTime: Union[TimeRangeTypeDef, TimeRangeOutputTypeDef] = ...,
-        EndTime: Union[TimeRangeTypeDef, TimeRangeOutputTypeDef] = ...,
+        StartTime: TimeRangeUnionTypeDef = ...,
+        EndTime: TimeRangeUnionTypeDef = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListAttacksResponseTypeDef:
         """
         Returns all ongoing DDoS attacks or all DDoS attacks during a specified time
         period.
 
@@ -411,15 +409,15 @@
         """
         Removes tags from a resource in Shield.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield/client/#untag_resource)
         """
     def update_application_layer_automatic_response(
-        self, *, ResourceArn: str, Action: Union[ResponseActionTypeDef, ResponseActionOutputTypeDef]
+        self, *, ResourceArn: str, Action: ResponseActionUnionTypeDef
     ) -> Dict[str, Any]:
         """
         Updates an existing Shield Advanced automatic application layer DDoS mitigation
         configuration for the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield.Client.update_application_layer_automatic_response)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield/client/#update_application_layer_automatic_response)
```

### Comparing `mypy-boto3-shield-1.28.15.post1/mypy_boto3_shield/literals.py` & `mypy-boto3-shield-1.28.16/mypy_boto3_shield/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-shield-1.28.15.post1/mypy_boto3_shield/literals.pyi` & `mypy-boto3-shield-1.28.16/mypy_boto3_shield/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-shield-1.28.15.post1/mypy_boto3_shield/paginator.py` & `mypy-boto3-shield-1.28.16/mypy_boto3_shield/paginator.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -17,60 +17,55 @@
     session = Session()
     client: ShieldClient = session.client("shield")
 
     list_attacks_paginator: ListAttacksPaginator = client.get_paginator("list_attacks")
     list_protections_paginator: ListProtectionsPaginator = client.get_paginator("list_protections")
     ```
 """
-from typing import Generic, Iterator, Sequence, TypeVar, Union
+from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import (
     InclusionProtectionFiltersTypeDef,
     ListAttacksResponseTypeDef,
     ListProtectionsResponseTypeDef,
     PaginatorConfigTypeDef,
-    TimeRangeOutputTypeDef,
-    TimeRangeTypeDef,
+    TimeRangeUnionTypeDef,
 )
 
 __all__ = ("ListAttacksPaginator", "ListProtectionsPaginator")
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class ListAttacksPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield.Paginator.ListAttacks)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield/paginators/#listattackspaginator)
     """
 
     def paginate(
         self,
         *,
         ResourceArns: Sequence[str] = ...,
-        StartTime: Union[TimeRangeTypeDef, TimeRangeOutputTypeDef] = ...,
-        EndTime: Union[TimeRangeTypeDef, TimeRangeOutputTypeDef] = ...,
+        StartTime: TimeRangeUnionTypeDef = ...,
+        EndTime: TimeRangeUnionTypeDef = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAttacksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield.Paginator.ListAttacks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield/paginators/#listattackspaginator)
         """
 
-
 class ListProtectionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield.Paginator.ListProtections)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield/paginators/#listprotectionspaginator)
     """
 
     def paginate(
```

### Comparing `mypy-boto3-shield-1.28.15.post1/mypy_boto3_shield/paginator.pyi` & `mypy-boto3-shield-1.28.16/mypy_boto3_shield/paginator.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,56 +17,59 @@
     session = Session()
     client: ShieldClient = session.client("shield")
 
     list_attacks_paginator: ListAttacksPaginator = client.get_paginator("list_attacks")
     list_protections_paginator: ListProtectionsPaginator = client.get_paginator("list_protections")
     ```
 """
-from typing import Generic, Iterator, Sequence, TypeVar, Union
+from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import (
     InclusionProtectionFiltersTypeDef,
     ListAttacksResponseTypeDef,
     ListProtectionsResponseTypeDef,
     PaginatorConfigTypeDef,
-    TimeRangeOutputTypeDef,
-    TimeRangeTypeDef,
+    TimeRangeUnionTypeDef,
 )
 
 __all__ = ("ListAttacksPaginator", "ListProtectionsPaginator")
 
+
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class ListAttacksPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield.Paginator.ListAttacks)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield/paginators/#listattackspaginator)
     """
 
     def paginate(
         self,
         *,
         ResourceArns: Sequence[str] = ...,
-        StartTime: Union[TimeRangeTypeDef, TimeRangeOutputTypeDef] = ...,
-        EndTime: Union[TimeRangeTypeDef, TimeRangeOutputTypeDef] = ...,
+        StartTime: TimeRangeUnionTypeDef = ...,
+        EndTime: TimeRangeUnionTypeDef = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAttacksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield.Paginator.ListAttacks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield/paginators/#listattackspaginator)
         """
 
+
 class ListProtectionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield.Paginator.ListProtections)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield/paginators/#listprotectionspaginator)
     """
 
     def paginate(
```

### Comparing `mypy-boto3-shield-1.28.15.post1/mypy_boto3_shield/type_defs.py` & `mypy-boto3-shield-1.28.16/mypy_boto3_shield/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_shield.type_defs import ResponseActionOutputTypeDef
 
-    data: ResponseActionOutputTypeDef = {...}
+    data: ResponseActionOutputTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -59,18 +59,18 @@
     "DisassociateDRTLogBucketRequestRequestTypeDef",
     "DisassociateHealthCheckRequestRequestTypeDef",
     "ResponseActionTypeDef",
     "InclusionProtectionFiltersTypeDef",
     "InclusionProtectionGroupFiltersTypeDef",
     "LimitTypeDef",
     "PaginatorConfigTypeDef",
-    "TimeRangeTypeDef",
     "ListResourcesInProtectionGroupRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ProtectionGroupArbitraryPatternLimitsTypeDef",
+    "TimestampTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateProtectionGroupRequestRequestTypeDef",
     "UpdateSubscriptionRequestRequestTypeDef",
     "ApplicationLayerAutomaticResponseConfigurationTypeDef",
     "AssociateProactiveEngagementDetailsRequestRequestTypeDef",
     "UpdateEmergencyContactSettingsRequestRequestTypeDef",
     "SummarizedAttackVectorTypeDef",
@@ -85,27 +85,30 @@
     "DescribeEmergencyContactSettingsResponseTypeDef",
     "GetSubscriptionStateResponseTypeDef",
     "ListResourcesInProtectionGroupResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "DescribeProtectionGroupResponseTypeDef",
     "ListProtectionGroupsResponseTypeDef",
     "EnableApplicationLayerAutomaticResponseRequestRequestTypeDef",
+    "ResponseActionUnionTypeDef",
     "UpdateApplicationLayerAutomaticResponseRequestRequestTypeDef",
     "ListProtectionsRequestRequestTypeDef",
     "ListProtectionGroupsRequestRequestTypeDef",
     "ProtectionLimitsTypeDef",
     "ListProtectionsRequestListProtectionsPaginateTypeDef",
-    "ListAttacksRequestListAttacksPaginateTypeDef",
-    "ListAttacksRequestRequestTypeDef",
     "ProtectionGroupPatternTypeLimitsTypeDef",
+    "TimeRangeTypeDef",
     "ProtectionTypeDef",
     "SubResourceSummaryTypeDef",
     "ListAttacksResponseTypeDef",
     "AttackStatisticsDataItemTypeDef",
     "ProtectionGroupLimitsTypeDef",
+    "ListAttacksRequestListAttacksPaginateTypeDef",
+    "ListAttacksRequestRequestTypeDef",
+    "TimeRangeUnionTypeDef",
     "DescribeProtectionResponseTypeDef",
     "ListProtectionsResponseTypeDef",
     "AttackDetailTypeDef",
     "DescribeAttackStatisticsResponseTypeDef",
     "SubscriptionLimitsTypeDef",
     "DescribeAttackResponseTypeDef",
     "SubscriptionTypeDef",
@@ -363,23 +366,14 @@
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
-TimeRangeTypeDef = TypedDict(
-    "TimeRangeTypeDef",
-    {
-        "FromInclusive": Union[datetime, str],
-        "ToExclusive": Union[datetime, str],
-    },
-    total=False,
-)
-
 _RequiredListResourcesInProtectionGroupRequestRequestTypeDef = TypedDict(
     "_RequiredListResourcesInProtectionGroupRequestRequestTypeDef",
     {
         "ProtectionGroupId": str,
     },
 )
 _OptionalListResourcesInProtectionGroupRequestRequestTypeDef = TypedDict(
@@ -409,14 +403,15 @@
 ProtectionGroupArbitraryPatternLimitsTypeDef = TypedDict(
     "ProtectionGroupArbitraryPatternLimitsTypeDef",
     {
         "MaxMembers": int,
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
@@ -659,14 +654,15 @@
     "EnableApplicationLayerAutomaticResponseRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Action": ResponseActionTypeDef,
     },
 )
 
+ResponseActionUnionTypeDef = Union[ResponseActionTypeDef, ResponseActionOutputTypeDef]
 UpdateApplicationLayerAutomaticResponseRequestRequestTypeDef = TypedDict(
     "UpdateApplicationLayerAutomaticResponseRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Action": ResponseActionTypeDef,
     },
 )
@@ -703,44 +699,30 @@
     {
         "InclusionFilters": InclusionProtectionFiltersTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListAttacksRequestListAttacksPaginateTypeDef = TypedDict(
-    "ListAttacksRequestListAttacksPaginateTypeDef",
+ProtectionGroupPatternTypeLimitsTypeDef = TypedDict(
+    "ProtectionGroupPatternTypeLimitsTypeDef",
     {
-        "ResourceArns": Sequence[str],
-        "StartTime": TimeRangeTypeDef,
-        "EndTime": TimeRangeTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "ArbitraryPatternLimits": ProtectionGroupArbitraryPatternLimitsTypeDef,
     },
-    total=False,
 )
 
-ListAttacksRequestRequestTypeDef = TypedDict(
-    "ListAttacksRequestRequestTypeDef",
+TimeRangeTypeDef = TypedDict(
+    "TimeRangeTypeDef",
     {
-        "ResourceArns": Sequence[str],
-        "StartTime": TimeRangeTypeDef,
-        "EndTime": TimeRangeTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
+        "FromInclusive": TimestampTypeDef,
+        "ToExclusive": TimestampTypeDef,
     },
     total=False,
 )
 
-ProtectionGroupPatternTypeLimitsTypeDef = TypedDict(
-    "ProtectionGroupPatternTypeLimitsTypeDef",
-    {
-        "ArbitraryPatternLimits": ProtectionGroupArbitraryPatternLimitsTypeDef,
-    },
-)
-
 ProtectionTypeDef = TypedDict(
     "ProtectionTypeDef",
     {
         "Id": str,
         "Name": str,
         "ResourceArn": str,
         "HealthCheckIds": List[str],
@@ -797,14 +779,38 @@
     "ProtectionGroupLimitsTypeDef",
     {
         "MaxProtectionGroups": int,
         "PatternTypeLimits": ProtectionGroupPatternTypeLimitsTypeDef,
     },
 )
 
+ListAttacksRequestListAttacksPaginateTypeDef = TypedDict(
+    "ListAttacksRequestListAttacksPaginateTypeDef",
+    {
+        "ResourceArns": Sequence[str],
+        "StartTime": TimeRangeTypeDef,
+        "EndTime": TimeRangeTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListAttacksRequestRequestTypeDef = TypedDict(
+    "ListAttacksRequestRequestTypeDef",
+    {
+        "ResourceArns": Sequence[str],
+        "StartTime": TimeRangeTypeDef,
+        "EndTime": TimeRangeTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+TimeRangeUnionTypeDef = Union[TimeRangeTypeDef, TimeRangeOutputTypeDef]
 DescribeProtectionResponseTypeDef = TypedDict(
     "DescribeProtectionResponseTypeDef",
     {
         "Protection": ProtectionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-shield-1.28.15.post1/mypy_boto3_shield/type_defs.pyi` & `mypy-boto3-shield-1.28.16/mypy_boto3_shield/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_shield.type_defs import ResponseActionOutputTypeDef
 
-    data: ResponseActionOutputTypeDef = {...}
+    data: ResponseActionOutputTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -58,18 +58,18 @@
     "DisassociateDRTLogBucketRequestRequestTypeDef",
     "DisassociateHealthCheckRequestRequestTypeDef",
     "ResponseActionTypeDef",
     "InclusionProtectionFiltersTypeDef",
     "InclusionProtectionGroupFiltersTypeDef",
     "LimitTypeDef",
     "PaginatorConfigTypeDef",
-    "TimeRangeTypeDef",
     "ListResourcesInProtectionGroupRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ProtectionGroupArbitraryPatternLimitsTypeDef",
+    "TimestampTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateProtectionGroupRequestRequestTypeDef",
     "UpdateSubscriptionRequestRequestTypeDef",
     "ApplicationLayerAutomaticResponseConfigurationTypeDef",
     "AssociateProactiveEngagementDetailsRequestRequestTypeDef",
     "UpdateEmergencyContactSettingsRequestRequestTypeDef",
     "SummarizedAttackVectorTypeDef",
@@ -84,27 +84,30 @@
     "DescribeEmergencyContactSettingsResponseTypeDef",
     "GetSubscriptionStateResponseTypeDef",
     "ListResourcesInProtectionGroupResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "DescribeProtectionGroupResponseTypeDef",
     "ListProtectionGroupsResponseTypeDef",
     "EnableApplicationLayerAutomaticResponseRequestRequestTypeDef",
+    "ResponseActionUnionTypeDef",
     "UpdateApplicationLayerAutomaticResponseRequestRequestTypeDef",
     "ListProtectionsRequestRequestTypeDef",
     "ListProtectionGroupsRequestRequestTypeDef",
     "ProtectionLimitsTypeDef",
     "ListProtectionsRequestListProtectionsPaginateTypeDef",
-    "ListAttacksRequestListAttacksPaginateTypeDef",
-    "ListAttacksRequestRequestTypeDef",
     "ProtectionGroupPatternTypeLimitsTypeDef",
+    "TimeRangeTypeDef",
     "ProtectionTypeDef",
     "SubResourceSummaryTypeDef",
     "ListAttacksResponseTypeDef",
     "AttackStatisticsDataItemTypeDef",
     "ProtectionGroupLimitsTypeDef",
+    "ListAttacksRequestListAttacksPaginateTypeDef",
+    "ListAttacksRequestRequestTypeDef",
+    "TimeRangeUnionTypeDef",
     "DescribeProtectionResponseTypeDef",
     "ListProtectionsResponseTypeDef",
     "AttackDetailTypeDef",
     "DescribeAttackStatisticsResponseTypeDef",
     "SubscriptionLimitsTypeDef",
     "DescribeAttackResponseTypeDef",
     "SubscriptionTypeDef",
@@ -358,23 +361,14 @@
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
-TimeRangeTypeDef = TypedDict(
-    "TimeRangeTypeDef",
-    {
-        "FromInclusive": Union[datetime, str],
-        "ToExclusive": Union[datetime, str],
-    },
-    total=False,
-)
-
 _RequiredListResourcesInProtectionGroupRequestRequestTypeDef = TypedDict(
     "_RequiredListResourcesInProtectionGroupRequestRequestTypeDef",
     {
         "ProtectionGroupId": str,
     },
 )
 _OptionalListResourcesInProtectionGroupRequestRequestTypeDef = TypedDict(
@@ -402,14 +396,15 @@
 ProtectionGroupArbitraryPatternLimitsTypeDef = TypedDict(
     "ProtectionGroupArbitraryPatternLimitsTypeDef",
     {
         "MaxMembers": int,
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
@@ -644,14 +639,15 @@
     "EnableApplicationLayerAutomaticResponseRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Action": ResponseActionTypeDef,
     },
 )
 
+ResponseActionUnionTypeDef = Union[ResponseActionTypeDef, ResponseActionOutputTypeDef]
 UpdateApplicationLayerAutomaticResponseRequestRequestTypeDef = TypedDict(
     "UpdateApplicationLayerAutomaticResponseRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Action": ResponseActionTypeDef,
     },
 )
@@ -688,44 +684,30 @@
     {
         "InclusionFilters": InclusionProtectionFiltersTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListAttacksRequestListAttacksPaginateTypeDef = TypedDict(
-    "ListAttacksRequestListAttacksPaginateTypeDef",
+ProtectionGroupPatternTypeLimitsTypeDef = TypedDict(
+    "ProtectionGroupPatternTypeLimitsTypeDef",
     {
-        "ResourceArns": Sequence[str],
-        "StartTime": TimeRangeTypeDef,
-        "EndTime": TimeRangeTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "ArbitraryPatternLimits": ProtectionGroupArbitraryPatternLimitsTypeDef,
     },
-    total=False,
 )
 
-ListAttacksRequestRequestTypeDef = TypedDict(
-    "ListAttacksRequestRequestTypeDef",
+TimeRangeTypeDef = TypedDict(
+    "TimeRangeTypeDef",
     {
-        "ResourceArns": Sequence[str],
-        "StartTime": TimeRangeTypeDef,
-        "EndTime": TimeRangeTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
+        "FromInclusive": TimestampTypeDef,
+        "ToExclusive": TimestampTypeDef,
     },
     total=False,
 )
 
-ProtectionGroupPatternTypeLimitsTypeDef = TypedDict(
-    "ProtectionGroupPatternTypeLimitsTypeDef",
-    {
-        "ArbitraryPatternLimits": ProtectionGroupArbitraryPatternLimitsTypeDef,
-    },
-)
-
 ProtectionTypeDef = TypedDict(
     "ProtectionTypeDef",
     {
         "Id": str,
         "Name": str,
         "ResourceArn": str,
         "HealthCheckIds": List[str],
@@ -780,14 +762,38 @@
     "ProtectionGroupLimitsTypeDef",
     {
         "MaxProtectionGroups": int,
         "PatternTypeLimits": ProtectionGroupPatternTypeLimitsTypeDef,
     },
 )
 
+ListAttacksRequestListAttacksPaginateTypeDef = TypedDict(
+    "ListAttacksRequestListAttacksPaginateTypeDef",
+    {
+        "ResourceArns": Sequence[str],
+        "StartTime": TimeRangeTypeDef,
+        "EndTime": TimeRangeTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListAttacksRequestRequestTypeDef = TypedDict(
+    "ListAttacksRequestRequestTypeDef",
+    {
+        "ResourceArns": Sequence[str],
+        "StartTime": TimeRangeTypeDef,
+        "EndTime": TimeRangeTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+TimeRangeUnionTypeDef = Union[TimeRangeTypeDef, TimeRangeOutputTypeDef]
 DescribeProtectionResponseTypeDef = TypedDict(
     "DescribeProtectionResponseTypeDef",
     {
         "Protection": ProtectionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-shield-1.28.15.post1/mypy_boto3_shield.egg-info/PKG-INFO` & `mypy-boto3-shield-1.28.16/mypy_boto3_shield.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-shield
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.Shield 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.Shield 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 shield type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 shield type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-shield.svg?color=blue)](https://pypi.org/project/mypy-boto3-shield)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-shield)](https://pepy.tech/project/mypy-boto3-shield)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Shield 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield)
+[boto3.Shield 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield)
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
 [mypy-boto3-shield docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield/).
 
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
@@ -321,20 +321,20 @@
 )
 
 
 def check_value(value: ApplicationLayerAutomaticResponseStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_shield.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_shield.type_defs import (
     ResponseActionOutputTypeDef,
     AssociateDRTLogBucketRequestRequestTypeDef,
     AssociateDRTRoleRequestRequestTypeDef,
     AssociateHealthCheckRequestRequestTypeDef,
@@ -357,18 +357,18 @@
     DisassociateDRTLogBucketRequestRequestTypeDef,
     DisassociateHealthCheckRequestRequestTypeDef,
     ResponseActionTypeDef,
     InclusionProtectionFiltersTypeDef,
     InclusionProtectionGroupFiltersTypeDef,
     LimitTypeDef,
     PaginatorConfigTypeDef,
-    TimeRangeTypeDef,
     ListResourcesInProtectionGroupRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ProtectionGroupArbitraryPatternLimitsTypeDef,
+    TimestampTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateProtectionGroupRequestRequestTypeDef,
     UpdateSubscriptionRequestRequestTypeDef,
     ApplicationLayerAutomaticResponseConfigurationTypeDef,
     AssociateProactiveEngagementDetailsRequestRequestTypeDef,
     UpdateEmergencyContactSettingsRequestRequestTypeDef,
     SummarizedAttackVectorTypeDef,
@@ -383,39 +383,42 @@
     DescribeEmergencyContactSettingsResponseTypeDef,
     GetSubscriptionStateResponseTypeDef,
     ListResourcesInProtectionGroupResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     DescribeProtectionGroupResponseTypeDef,
     ListProtectionGroupsResponseTypeDef,
     EnableApplicationLayerAutomaticResponseRequestRequestTypeDef,
+    ResponseActionUnionTypeDef,
     UpdateApplicationLayerAutomaticResponseRequestRequestTypeDef,
     ListProtectionsRequestRequestTypeDef,
     ListProtectionGroupsRequestRequestTypeDef,
     ProtectionLimitsTypeDef,
     ListProtectionsRequestListProtectionsPaginateTypeDef,
-    ListAttacksRequestListAttacksPaginateTypeDef,
-    ListAttacksRequestRequestTypeDef,
     ProtectionGroupPatternTypeLimitsTypeDef,
+    TimeRangeTypeDef,
     ProtectionTypeDef,
     SubResourceSummaryTypeDef,
     ListAttacksResponseTypeDef,
     AttackStatisticsDataItemTypeDef,
     ProtectionGroupLimitsTypeDef,
+    ListAttacksRequestListAttacksPaginateTypeDef,
+    ListAttacksRequestRequestTypeDef,
+    TimeRangeUnionTypeDef,
     DescribeProtectionResponseTypeDef,
     ListProtectionsResponseTypeDef,
     AttackDetailTypeDef,
     DescribeAttackStatisticsResponseTypeDef,
     SubscriptionLimitsTypeDef,
     DescribeAttackResponseTypeDef,
     SubscriptionTypeDef,
     DescribeSubscriptionResponseTypeDef,
 )
 
 
-def get_structure() -> ResponseActionOutputTypeDef:
+def get_value() -> ResponseActionOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-shield-1.28.15.post1/mypy_boto3_shield.egg-info/SOURCES.txt` & `mypy-boto3-shield-1.28.16/mypy_boto3_shield.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-shield-1.28.15.post1/setup.py` & `mypy-boto3-shield-1.28.16/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-shield",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_shield"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Shield 1.28.15 service generated with mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.Shield 1.28.16 service generated with mypy-boto3-builder 7.17.1"
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
-    keywords="boto3 shield type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 shield type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_shield": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

