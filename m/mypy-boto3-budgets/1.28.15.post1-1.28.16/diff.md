# Comparing `tmp/mypy-boto3-budgets-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-budgets-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-budgets-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:37 2023, max compression
+gzip compressed data, was "mypy-boto3-budgets-1.28.16.tar", last modified: Tue Aug  1 11:36:18 2023, max compression
```

## Comparing `mypy-boto3-budgets-1.28.15.post1.tar` & `mypy-boto3-budgets-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:37.941035 mypy-boto3-budgets-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:39:09.000000 mypy-boto3-budgets-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17894 2023-07-29 10:02:37.941035 mypy-boto3-budgets-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16401 2023-07-29 09:39:09.000000 mypy-boto3-budgets-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:37.929035 mypy-boto3-budgets-1.28.15.post1/mypy_boto3_budgets/
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-07-29 09:39:09.000000 mypy-boto3-budgets-1.28.15.post1/mypy_boto3_budgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-07-29 09:39:09.000000 mypy-boto3-budgets-1.28.15.post1/mypy_boto3_budgets/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-29 09:39:09.000000 mypy-boto3-budgets-1.28.15.post1/mypy_boto3_budgets/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22253 2023-07-29 09:39:10.000000 mypy-boto3-budgets-1.28.15.post1/mypy_boto3_budgets/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    22215 2023-07-29 09:39:09.000000 mypy-boto3-budgets-1.28.15.post1/mypy_boto3_budgets/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10732 2023-07-29 09:39:10.000000 mypy-boto3-budgets-1.28.15.post1/mypy_boto3_budgets/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10730 2023-07-29 09:39:10.000000 mypy-boto3-budgets-1.28.15.post1/mypy_boto3_budgets/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11083 2023-07-29 09:39:10.000000 mypy-boto3-budgets-1.28.15.post1/mypy_boto3_budgets/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11073 2023-07-29 09:39:10.000000 mypy-boto3-budgets-1.28.15.post1/mypy_boto3_budgets/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:39:09.000000 mypy-boto3-budgets-1.28.15.post1/mypy_boto3_budgets/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    34193 2023-07-29 09:39:12.000000 mypy-boto3-budgets-1.28.15.post1/mypy_boto3_budgets/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    34138 2023-07-29 09:39:11.000000 mypy-boto3-budgets-1.28.15.post1/mypy_boto3_budgets/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:39:09.000000 mypy-boto3-budgets-1.28.15.post1/mypy_boto3_budgets/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:37.941035 mypy-boto3-budgets-1.28.15.post1/mypy_boto3_budgets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17894 2023-07-29 10:02:37.000000 mypy-boto3-budgets-1.28.15.post1/mypy_boto3_budgets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-29 10:02:37.000000 mypy-boto3-budgets-1.28.15.post1/mypy_boto3_budgets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:37.000000 mypy-boto3-budgets-1.28.15.post1/mypy_boto3_budgets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:37.000000 mypy-boto3-budgets-1.28.15.post1/mypy_boto3_budgets.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:37.000000 mypy-boto3-budgets-1.28.15.post1/mypy_boto3_budgets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-29 10:02:37.000000 mypy-boto3-budgets-1.28.15.post1/mypy_boto3_budgets.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:37.941035 mypy-boto3-budgets-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-07-29 09:39:09.000000 mypy-boto3-budgets-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:18.728939 mypy-boto3-budgets-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:11:42.000000 mypy-boto3-budgets-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17986 2023-08-01 11:36:18.724939 mypy-boto3-budgets-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16502 2023-08-01 11:11:42.000000 mypy-boto3-budgets-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:18.720939 mypy-boto3-budgets-1.28.16/mypy_boto3_budgets/
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-08-01 11:11:42.000000 mypy-boto3-budgets-1.28.16/mypy_boto3_budgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-08-01 11:11:42.000000 mypy-boto3-budgets-1.28.16/mypy_boto3_budgets/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-08-01 11:11:42.000000 mypy-boto3-budgets-1.28.16/mypy_boto3_budgets/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22010 2023-08-01 11:11:43.000000 mypy-boto3-budgets-1.28.16/mypy_boto3_budgets/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21972 2023-08-01 11:11:43.000000 mypy-boto3-budgets-1.28.16/mypy_boto3_budgets/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10732 2023-08-01 11:11:44.000000 mypy-boto3-budgets-1.28.16/mypy_boto3_budgets/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10730 2023-08-01 11:11:44.000000 mypy-boto3-budgets-1.28.16/mypy_boto3_budgets/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10998 2023-08-01 11:11:43.000000 mypy-boto3-budgets-1.28.16/mypy_boto3_budgets/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10988 2023-08-01 11:11:43.000000 mypy-boto3-budgets-1.28.16/mypy_boto3_budgets/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:11:42.000000 mypy-boto3-budgets-1.28.16/mypy_boto3_budgets/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    34538 2023-08-01 11:11:45.000000 mypy-boto3-budgets-1.28.16/mypy_boto3_budgets/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34483 2023-08-01 11:11:44.000000 mypy-boto3-budgets-1.28.16/mypy_boto3_budgets/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:11:42.000000 mypy-boto3-budgets-1.28.16/mypy_boto3_budgets/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:18.724939 mypy-boto3-budgets-1.28.16/mypy_boto3_budgets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17986 2023-08-01 11:36:18.000000 mypy-boto3-budgets-1.28.16/mypy_boto3_budgets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-08-01 11:36:18.000000 mypy-boto3-budgets-1.28.16/mypy_boto3_budgets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:18.000000 mypy-boto3-budgets-1.28.16/mypy_boto3_budgets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:18.000000 mypy-boto3-budgets-1.28.16/mypy_boto3_budgets.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:18.000000 mypy-boto3-budgets-1.28.16/mypy_boto3_budgets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-01 11:36:18.000000 mypy-boto3-budgets-1.28.16/mypy_boto3_budgets.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:18.728939 mypy-boto3-budgets-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-08-01 11:11:42.000000 mypy-boto3-budgets-1.28.16/setup.py
```

### Comparing `mypy-boto3-budgets-1.28.15.post1/LICENSE` & `mypy-boto3-budgets-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-budgets-1.28.15.post1/PKG-INFO` & `mypy-boto3-budgets-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-budgets
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.Budgets 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.Budgets 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 budgets type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 budgets type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-budgets.svg?color=blue)](https://pypi.org/project/mypy-boto3-budgets)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-budgets)](https://pepy.tech/project/mypy-boto3-budgets)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Budgets 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets)
+[boto3.Budgets 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets)
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
 [mypy-boto3-budgets docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/).
 
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
@@ -359,31 +359,31 @@
 )
 
 
 def check_value(value: ActionStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_budgets.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_budgets.type_defs import (
     ActionThresholdTypeDef,
     SubscriberTypeDef,
     HistoricalOptionsTypeDef,
+    TimestampTypeDef,
     NotificationTypeDef,
     CostTypesTypeDef,
     SpendTypeDef,
     TimePeriodOutputTypeDef,
-    TimePeriodTypeDef,
     ResponseMetadataTypeDef,
     IamActionDefinitionOutputTypeDef,
     ScpActionDefinitionOutputTypeDef,
     SsmActionDefinitionOutputTypeDef,
     IamActionDefinitionTypeDef,
     ScpActionDefinitionTypeDef,
     SsmActionDefinitionTypeDef,
@@ -396,65 +396,69 @@
     DescribeBudgetNotificationsForAccountRequestRequestTypeDef,
     DescribeBudgetRequestRequestTypeDef,
     DescribeBudgetsRequestRequestTypeDef,
     DescribeNotificationsForBudgetRequestRequestTypeDef,
     ExecuteBudgetActionRequestRequestTypeDef,
     AutoAdjustDataOutputTypeDef,
     AutoAdjustDataTypeDef,
+    TimePeriodTypeDef,
     BudgetNotificationsForAccountTypeDef,
     CreateNotificationRequestRequestTypeDef,
     CreateSubscriberRequestRequestTypeDef,
     DeleteNotificationRequestRequestTypeDef,
     DeleteSubscriberRequestRequestTypeDef,
     DescribeSubscribersForNotificationRequestRequestTypeDef,
     NotificationWithSubscribersTypeDef,
     UpdateNotificationRequestRequestTypeDef,
     UpdateSubscriberRequestRequestTypeDef,
     CalculatedSpendTypeDef,
     BudgetedAndActualAmountsTypeDef,
-    DescribeBudgetActionHistoriesRequestRequestTypeDef,
-    DescribeBudgetPerformanceHistoryRequestRequestTypeDef,
     CreateBudgetActionResponseTypeDef,
     DescribeNotificationsForBudgetResponseTypeDef,
     DescribeSubscribersForNotificationResponseTypeDef,
     ExecuteBudgetActionResponseTypeDef,
     DefinitionOutputTypeDef,
     DefinitionTypeDef,
-    DescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef,
     DescribeBudgetActionsForAccountRequestDescribeBudgetActionsForAccountPaginateTypeDef,
     DescribeBudgetActionsForBudgetRequestDescribeBudgetActionsForBudgetPaginateTypeDef,
     DescribeBudgetNotificationsForAccountRequestDescribeBudgetNotificationsForAccountPaginateTypeDef,
-    DescribeBudgetPerformanceHistoryRequestDescribeBudgetPerformanceHistoryPaginateTypeDef,
     DescribeBudgetsRequestDescribeBudgetsPaginateTypeDef,
     DescribeNotificationsForBudgetRequestDescribeNotificationsForBudgetPaginateTypeDef,
     DescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef,
+    DescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef,
+    DescribeBudgetActionHistoriesRequestRequestTypeDef,
+    DescribeBudgetPerformanceHistoryRequestDescribeBudgetPerformanceHistoryPaginateTypeDef,
+    DescribeBudgetPerformanceHistoryRequestRequestTypeDef,
+    TimePeriodUnionTypeDef,
     DescribeBudgetNotificationsForAccountResponseTypeDef,
     BudgetOutputTypeDef,
     BudgetTypeDef,
     BudgetPerformanceHistoryTypeDef,
     ActionTypeDef,
     CreateBudgetActionRequestRequestTypeDef,
+    DefinitionUnionTypeDef,
     UpdateBudgetActionRequestRequestTypeDef,
     DescribeBudgetResponseTypeDef,
     DescribeBudgetsResponseTypeDef,
+    BudgetUnionTypeDef,
     CreateBudgetRequestRequestTypeDef,
     UpdateBudgetRequestRequestTypeDef,
     DescribeBudgetPerformanceHistoryResponseTypeDef,
     ActionHistoryDetailsTypeDef,
     DeleteBudgetActionResponseTypeDef,
     DescribeBudgetActionResponseTypeDef,
     DescribeBudgetActionsForAccountResponseTypeDef,
     DescribeBudgetActionsForBudgetResponseTypeDef,
     UpdateBudgetActionResponseTypeDef,
     ActionHistoryTypeDef,
     DescribeBudgetActionHistoriesResponseTypeDef,
 )
 
 
-def get_structure() -> ActionThresholdTypeDef:
+def get_value() -> ActionThresholdTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-budgets-1.28.15.post1/README.md` & `mypy-boto3-budgets-1.28.16/mypy_boto3_budgets.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-budgets
+Version: 1.28.16
+Summary: Type annotations for boto3.Budgets 1.28.16 service generated with mypy-boto3-builder 7.17.1
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 budgets type-annotations botocore mypy typeshed autocomplete
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Typing :: Typed
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <a id="mypy-boto3-budgets"></a>
 
 # mypy-boto3-budgets
 
 [![PyPI - mypy-boto3-budgets](https://img.shields.io/pypi/v/mypy-boto3-budgets.svg?color=blue)](https://pypi.org/project/mypy-boto3-budgets)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-budgets.svg?color=blue)](https://pypi.org/project/mypy-boto3-budgets)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-budgets)](https://pepy.tech/project/mypy-boto3-budgets)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Budgets 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets)
+[boto3.Budgets 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets)
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
 [mypy-boto3-budgets docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/).
 
 See how it helps to find and fix potential bugs:
 
@@ -42,15 +74,15 @@
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
@@ -327,31 +359,31 @@
 )
 
 
 def check_value(value: ActionStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_budgets.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_budgets.type_defs import (
     ActionThresholdTypeDef,
     SubscriberTypeDef,
     HistoricalOptionsTypeDef,
+    TimestampTypeDef,
     NotificationTypeDef,
     CostTypesTypeDef,
     SpendTypeDef,
     TimePeriodOutputTypeDef,
-    TimePeriodTypeDef,
     ResponseMetadataTypeDef,
     IamActionDefinitionOutputTypeDef,
     ScpActionDefinitionOutputTypeDef,
     SsmActionDefinitionOutputTypeDef,
     IamActionDefinitionTypeDef,
     ScpActionDefinitionTypeDef,
     SsmActionDefinitionTypeDef,
@@ -364,65 +396,69 @@
     DescribeBudgetNotificationsForAccountRequestRequestTypeDef,
     DescribeBudgetRequestRequestTypeDef,
     DescribeBudgetsRequestRequestTypeDef,
     DescribeNotificationsForBudgetRequestRequestTypeDef,
     ExecuteBudgetActionRequestRequestTypeDef,
     AutoAdjustDataOutputTypeDef,
     AutoAdjustDataTypeDef,
+    TimePeriodTypeDef,
     BudgetNotificationsForAccountTypeDef,
     CreateNotificationRequestRequestTypeDef,
     CreateSubscriberRequestRequestTypeDef,
     DeleteNotificationRequestRequestTypeDef,
     DeleteSubscriberRequestRequestTypeDef,
     DescribeSubscribersForNotificationRequestRequestTypeDef,
     NotificationWithSubscribersTypeDef,
     UpdateNotificationRequestRequestTypeDef,
     UpdateSubscriberRequestRequestTypeDef,
     CalculatedSpendTypeDef,
     BudgetedAndActualAmountsTypeDef,
-    DescribeBudgetActionHistoriesRequestRequestTypeDef,
-    DescribeBudgetPerformanceHistoryRequestRequestTypeDef,
     CreateBudgetActionResponseTypeDef,
     DescribeNotificationsForBudgetResponseTypeDef,
     DescribeSubscribersForNotificationResponseTypeDef,
     ExecuteBudgetActionResponseTypeDef,
     DefinitionOutputTypeDef,
     DefinitionTypeDef,
-    DescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef,
     DescribeBudgetActionsForAccountRequestDescribeBudgetActionsForAccountPaginateTypeDef,
     DescribeBudgetActionsForBudgetRequestDescribeBudgetActionsForBudgetPaginateTypeDef,
     DescribeBudgetNotificationsForAccountRequestDescribeBudgetNotificationsForAccountPaginateTypeDef,
-    DescribeBudgetPerformanceHistoryRequestDescribeBudgetPerformanceHistoryPaginateTypeDef,
     DescribeBudgetsRequestDescribeBudgetsPaginateTypeDef,
     DescribeNotificationsForBudgetRequestDescribeNotificationsForBudgetPaginateTypeDef,
     DescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef,
+    DescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef,
+    DescribeBudgetActionHistoriesRequestRequestTypeDef,
+    DescribeBudgetPerformanceHistoryRequestDescribeBudgetPerformanceHistoryPaginateTypeDef,
+    DescribeBudgetPerformanceHistoryRequestRequestTypeDef,
+    TimePeriodUnionTypeDef,
     DescribeBudgetNotificationsForAccountResponseTypeDef,
     BudgetOutputTypeDef,
     BudgetTypeDef,
     BudgetPerformanceHistoryTypeDef,
     ActionTypeDef,
     CreateBudgetActionRequestRequestTypeDef,
+    DefinitionUnionTypeDef,
     UpdateBudgetActionRequestRequestTypeDef,
     DescribeBudgetResponseTypeDef,
     DescribeBudgetsResponseTypeDef,
+    BudgetUnionTypeDef,
     CreateBudgetRequestRequestTypeDef,
     UpdateBudgetRequestRequestTypeDef,
     DescribeBudgetPerformanceHistoryResponseTypeDef,
     ActionHistoryDetailsTypeDef,
     DeleteBudgetActionResponseTypeDef,
     DescribeBudgetActionResponseTypeDef,
     DescribeBudgetActionsForAccountResponseTypeDef,
     DescribeBudgetActionsForBudgetResponseTypeDef,
     UpdateBudgetActionResponseTypeDef,
     ActionHistoryTypeDef,
     DescribeBudgetActionHistoriesResponseTypeDef,
 )
 
 
-def get_structure() -> ActionThresholdTypeDef:
+def get_value() -> ActionThresholdTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-budgets-1.28.15.post1/mypy_boto3_budgets/__init__.py` & `mypy-boto3-budgets-1.28.16/mypy_boto3_budgets/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-budgets-1.28.15.post1/mypy_boto3_budgets/__init__.pyi` & `mypy-boto3-budgets-1.28.16/mypy_boto3_budgets/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-budgets-1.28.15.post1/mypy_boto3_budgets/__main__.py` & `mypy-boto3-budgets-1.28.16/mypy_boto3_budgets/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Budgets 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.Budgets 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets\nOther"
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

### Comparing `mypy-boto3-budgets-1.28.15.post1/mypy_boto3_budgets/client.py` & `mypy-boto3-budgets-1.28.16/mypy_boto3_budgets/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_budgets.client import BudgetsClient
 
     session = Session()
     client: BudgetsClient = session.client("budgets")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import ActionTypeType, ApprovalModelType, ExecutionTypeType, NotificationTypeType
 from .paginator import (
     DescribeBudgetActionHistoriesPaginator,
     DescribeBudgetActionsForAccountPaginator,
@@ -27,19 +27,17 @@
     DescribeBudgetPerformanceHistoryPaginator,
     DescribeBudgetsPaginator,
     DescribeNotificationsForBudgetPaginator,
     DescribeSubscribersForNotificationPaginator,
 )
 from .type_defs import (
     ActionThresholdTypeDef,
-    BudgetOutputTypeDef,
-    BudgetTypeDef,
+    BudgetUnionTypeDef,
     CreateBudgetActionResponseTypeDef,
-    DefinitionOutputTypeDef,
-    DefinitionTypeDef,
+    DefinitionUnionTypeDef,
     DeleteBudgetActionResponseTypeDef,
     DescribeBudgetActionHistoriesResponseTypeDef,
     DescribeBudgetActionResponseTypeDef,
     DescribeBudgetActionsForAccountResponseTypeDef,
     DescribeBudgetActionsForBudgetResponseTypeDef,
     DescribeBudgetNotificationsForAccountResponseTypeDef,
     DescribeBudgetPerformanceHistoryResponseTypeDef,
@@ -47,16 +45,15 @@
     DescribeBudgetsResponseTypeDef,
     DescribeNotificationsForBudgetResponseTypeDef,
     DescribeSubscribersForNotificationResponseTypeDef,
     ExecuteBudgetActionResponseTypeDef,
     NotificationTypeDef,
     NotificationWithSubscribersTypeDef,
     SubscriberTypeDef,
-    TimePeriodOutputTypeDef,
-    TimePeriodTypeDef,
+    TimePeriodUnionTypeDef,
     UpdateBudgetActionResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -120,15 +117,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/client/#close)
         """
 
     def create_budget(
         self,
         *,
         AccountId: str,
-        Budget: Union[BudgetTypeDef, BudgetOutputTypeDef],
+        Budget: BudgetUnionTypeDef,
         NotificationsWithSubscribers: Sequence[NotificationWithSubscribersTypeDef] = ...
     ) -> Dict[str, Any]:
         """
         Creates a budget and, if included, notifications and subscribers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.create_budget)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/client/#create_budget)
@@ -138,15 +135,15 @@
         self,
         *,
         AccountId: str,
         BudgetName: str,
         NotificationType: NotificationTypeType,
         ActionType: ActionTypeType,
         ActionThreshold: ActionThresholdTypeDef,
-        Definition: Union[DefinitionTypeDef, DefinitionOutputTypeDef],
+        Definition: DefinitionUnionTypeDef,
         ExecutionRoleArn: str,
         ApprovalModel: ApprovalModelType,
         Subscribers: Sequence[SubscriberTypeDef]
     ) -> CreateBudgetActionResponseTypeDef:
         """
         Creates a budget action.
 
@@ -247,15 +244,15 @@
 
     def describe_budget_action_histories(
         self,
         *,
         AccountId: str,
         BudgetName: str,
         ActionId: str,
-        TimePeriod: Union[TimePeriodTypeDef, TimePeriodOutputTypeDef] = ...,
+        TimePeriod: TimePeriodUnionTypeDef = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> DescribeBudgetActionHistoriesResponseTypeDef:
         """
         Describes a budget action history detail.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.describe_budget_action_histories)
@@ -293,15 +290,15 @@
         """
 
     def describe_budget_performance_history(
         self,
         *,
         AccountId: str,
         BudgetName: str,
-        TimePeriod: Union[TimePeriodTypeDef, TimePeriodOutputTypeDef] = ...,
+        TimePeriod: TimePeriodUnionTypeDef = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> DescribeBudgetPerformanceHistoryResponseTypeDef:
         """
         Describes the history for `DAILY`, `MONTHLY`, and `QUARTERLY` budgets.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.describe_budget_performance_history)
@@ -364,17 +361,15 @@
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/client/#generate_presigned_url)
         """
 
-    def update_budget(
-        self, *, AccountId: str, NewBudget: Union[BudgetTypeDef, BudgetOutputTypeDef]
-    ) -> Dict[str, Any]:
+    def update_budget(self, *, AccountId: str, NewBudget: BudgetUnionTypeDef) -> Dict[str, Any]:
         """
         Updates a budget.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.update_budget)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/client/#update_budget)
         """
 
@@ -382,15 +377,15 @@
         self,
         *,
         AccountId: str,
         BudgetName: str,
         ActionId: str,
         NotificationType: NotificationTypeType = ...,
         ActionThreshold: ActionThresholdTypeDef = ...,
-        Definition: Union[DefinitionTypeDef, DefinitionOutputTypeDef] = ...,
+        Definition: DefinitionUnionTypeDef = ...,
         ExecutionRoleArn: str = ...,
         ApprovalModel: ApprovalModelType = ...,
         Subscribers: Sequence[SubscriberTypeDef] = ...
     ) -> UpdateBudgetActionResponseTypeDef:
         """
         Updates a budget action.
```

### Comparing `mypy-boto3-budgets-1.28.15.post1/mypy_boto3_budgets/client.pyi` & `mypy-boto3-budgets-1.28.16/mypy_boto3_budgets/client.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_budgets.client import BudgetsClient
 
     session = Session()
     client: BudgetsClient = session.client("budgets")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import ActionTypeType, ApprovalModelType, ExecutionTypeType, NotificationTypeType
 from .paginator import (
     DescribeBudgetActionHistoriesPaginator,
     DescribeBudgetActionsForAccountPaginator,
@@ -27,19 +27,17 @@
     DescribeBudgetPerformanceHistoryPaginator,
     DescribeBudgetsPaginator,
     DescribeNotificationsForBudgetPaginator,
     DescribeSubscribersForNotificationPaginator,
 )
 from .type_defs import (
     ActionThresholdTypeDef,
-    BudgetOutputTypeDef,
-    BudgetTypeDef,
+    BudgetUnionTypeDef,
     CreateBudgetActionResponseTypeDef,
-    DefinitionOutputTypeDef,
-    DefinitionTypeDef,
+    DefinitionUnionTypeDef,
     DeleteBudgetActionResponseTypeDef,
     DescribeBudgetActionHistoriesResponseTypeDef,
     DescribeBudgetActionResponseTypeDef,
     DescribeBudgetActionsForAccountResponseTypeDef,
     DescribeBudgetActionsForBudgetResponseTypeDef,
     DescribeBudgetNotificationsForAccountResponseTypeDef,
     DescribeBudgetPerformanceHistoryResponseTypeDef,
@@ -47,16 +45,15 @@
     DescribeBudgetsResponseTypeDef,
     DescribeNotificationsForBudgetResponseTypeDef,
     DescribeSubscribersForNotificationResponseTypeDef,
     ExecuteBudgetActionResponseTypeDef,
     NotificationTypeDef,
     NotificationWithSubscribersTypeDef,
     SubscriberTypeDef,
-    TimePeriodOutputTypeDef,
-    TimePeriodTypeDef,
+    TimePeriodUnionTypeDef,
     UpdateBudgetActionResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -113,15 +110,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/client/#close)
         """
     def create_budget(
         self,
         *,
         AccountId: str,
-        Budget: Union[BudgetTypeDef, BudgetOutputTypeDef],
+        Budget: BudgetUnionTypeDef,
         NotificationsWithSubscribers: Sequence[NotificationWithSubscribersTypeDef] = ...
     ) -> Dict[str, Any]:
         """
         Creates a budget and, if included, notifications and subscribers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.create_budget)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/client/#create_budget)
@@ -130,15 +127,15 @@
         self,
         *,
         AccountId: str,
         BudgetName: str,
         NotificationType: NotificationTypeType,
         ActionType: ActionTypeType,
         ActionThreshold: ActionThresholdTypeDef,
-        Definition: Union[DefinitionTypeDef, DefinitionOutputTypeDef],
+        Definition: DefinitionUnionTypeDef,
         ExecutionRoleArn: str,
         ApprovalModel: ApprovalModelType,
         Subscribers: Sequence[SubscriberTypeDef]
     ) -> CreateBudgetActionResponseTypeDef:
         """
         Creates a budget action.
 
@@ -230,15 +227,15 @@
         """
     def describe_budget_action_histories(
         self,
         *,
         AccountId: str,
         BudgetName: str,
         ActionId: str,
-        TimePeriod: Union[TimePeriodTypeDef, TimePeriodOutputTypeDef] = ...,
+        TimePeriod: TimePeriodUnionTypeDef = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> DescribeBudgetActionHistoriesResponseTypeDef:
         """
         Describes a budget action history detail.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.describe_budget_action_histories)
@@ -272,15 +269,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/client/#describe_budget_notifications_for_account)
         """
     def describe_budget_performance_history(
         self,
         *,
         AccountId: str,
         BudgetName: str,
-        TimePeriod: Union[TimePeriodTypeDef, TimePeriodOutputTypeDef] = ...,
+        TimePeriod: TimePeriodUnionTypeDef = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> DescribeBudgetPerformanceHistoryResponseTypeDef:
         """
         Describes the history for `DAILY`, `MONTHLY`, and `QUARTERLY` budgets.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.describe_budget_performance_history)
@@ -337,32 +334,30 @@
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/client/#generate_presigned_url)
         """
-    def update_budget(
-        self, *, AccountId: str, NewBudget: Union[BudgetTypeDef, BudgetOutputTypeDef]
-    ) -> Dict[str, Any]:
+    def update_budget(self, *, AccountId: str, NewBudget: BudgetUnionTypeDef) -> Dict[str, Any]:
         """
         Updates a budget.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.update_budget)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/client/#update_budget)
         """
     def update_budget_action(
         self,
         *,
         AccountId: str,
         BudgetName: str,
         ActionId: str,
         NotificationType: NotificationTypeType = ...,
         ActionThreshold: ActionThresholdTypeDef = ...,
-        Definition: Union[DefinitionTypeDef, DefinitionOutputTypeDef] = ...,
+        Definition: DefinitionUnionTypeDef = ...,
         ExecutionRoleArn: str = ...,
         ApprovalModel: ApprovalModelType = ...,
         Subscribers: Sequence[SubscriberTypeDef] = ...
     ) -> UpdateBudgetActionResponseTypeDef:
         """
         Updates a budget action.
```

### Comparing `mypy-boto3-budgets-1.28.15.post1/mypy_boto3_budgets/literals.py` & `mypy-boto3-budgets-1.28.16/mypy_boto3_budgets/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-budgets-1.28.15.post1/mypy_boto3_budgets/literals.pyi` & `mypy-boto3-budgets-1.28.16/mypy_boto3_budgets/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-budgets-1.28.15.post1/mypy_boto3_budgets/paginator.py` & `mypy-boto3-budgets-1.28.16/mypy_boto3_budgets/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,31 +29,30 @@
     describe_budget_notifications_for_account_paginator: DescribeBudgetNotificationsForAccountPaginator = client.get_paginator("describe_budget_notifications_for_account")
     describe_budget_performance_history_paginator: DescribeBudgetPerformanceHistoryPaginator = client.get_paginator("describe_budget_performance_history")
     describe_budgets_paginator: DescribeBudgetsPaginator = client.get_paginator("describe_budgets")
     describe_notifications_for_budget_paginator: DescribeNotificationsForBudgetPaginator = client.get_paginator("describe_notifications_for_budget")
     describe_subscribers_for_notification_paginator: DescribeSubscribersForNotificationPaginator = client.get_paginator("describe_subscribers_for_notification")
     ```
 """
-from typing import Generic, Iterator, TypeVar, Union
+from typing import Generic, Iterator, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import (
     DescribeBudgetActionHistoriesResponseTypeDef,
     DescribeBudgetActionsForAccountResponseTypeDef,
     DescribeBudgetActionsForBudgetResponseTypeDef,
     DescribeBudgetNotificationsForAccountResponseTypeDef,
     DescribeBudgetPerformanceHistoryResponseTypeDef,
     DescribeBudgetsResponseTypeDef,
     DescribeNotificationsForBudgetResponseTypeDef,
     DescribeSubscribersForNotificationResponseTypeDef,
     NotificationTypeDef,
     PaginatorConfigTypeDef,
-    TimePeriodOutputTypeDef,
-    TimePeriodTypeDef,
+    TimePeriodUnionTypeDef,
 )
 
 __all__ = (
     "DescribeBudgetActionHistoriesPaginator",
     "DescribeBudgetActionsForAccountPaginator",
     "DescribeBudgetActionsForBudgetPaginator",
     "DescribeBudgetNotificationsForAccountPaginator",
@@ -82,15 +81,15 @@
 
     def paginate(
         self,
         *,
         AccountId: str,
         BudgetName: str,
         ActionId: str,
-        TimePeriod: Union[TimePeriodTypeDef, TimePeriodOutputTypeDef] = ...,
+        TimePeriod: TimePeriodUnionTypeDef = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeBudgetActionHistoriesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeBudgetActionHistories.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/paginators/#describebudgetactionhistoriespaginator)
         """
 
@@ -147,15 +146,15 @@
     """
 
     def paginate(
         self,
         *,
         AccountId: str,
         BudgetName: str,
-        TimePeriod: Union[TimePeriodTypeDef, TimePeriodOutputTypeDef] = ...,
+        TimePeriod: TimePeriodUnionTypeDef = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeBudgetPerformanceHistoryResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeBudgetPerformanceHistory.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/paginators/#describebudgetperformancehistorypaginator)
         """
```

### Comparing `mypy-boto3-budgets-1.28.15.post1/mypy_boto3_budgets/paginator.pyi` & `mypy-boto3-budgets-1.28.16/mypy_boto3_budgets/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -29,31 +29,30 @@
     describe_budget_notifications_for_account_paginator: DescribeBudgetNotificationsForAccountPaginator = client.get_paginator("describe_budget_notifications_for_account")
     describe_budget_performance_history_paginator: DescribeBudgetPerformanceHistoryPaginator = client.get_paginator("describe_budget_performance_history")
     describe_budgets_paginator: DescribeBudgetsPaginator = client.get_paginator("describe_budgets")
     describe_notifications_for_budget_paginator: DescribeNotificationsForBudgetPaginator = client.get_paginator("describe_notifications_for_budget")
     describe_subscribers_for_notification_paginator: DescribeSubscribersForNotificationPaginator = client.get_paginator("describe_subscribers_for_notification")
     ```
 """
-from typing import Generic, Iterator, TypeVar, Union
+from typing import Generic, Iterator, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import (
     DescribeBudgetActionHistoriesResponseTypeDef,
     DescribeBudgetActionsForAccountResponseTypeDef,
     DescribeBudgetActionsForBudgetResponseTypeDef,
     DescribeBudgetNotificationsForAccountResponseTypeDef,
     DescribeBudgetPerformanceHistoryResponseTypeDef,
     DescribeBudgetsResponseTypeDef,
     DescribeNotificationsForBudgetResponseTypeDef,
     DescribeSubscribersForNotificationResponseTypeDef,
     NotificationTypeDef,
     PaginatorConfigTypeDef,
-    TimePeriodOutputTypeDef,
-    TimePeriodTypeDef,
+    TimePeriodUnionTypeDef,
 )
 
 __all__ = (
     "DescribeBudgetActionHistoriesPaginator",
     "DescribeBudgetActionsForAccountPaginator",
     "DescribeBudgetActionsForBudgetPaginator",
     "DescribeBudgetNotificationsForAccountPaginator",
@@ -79,15 +78,15 @@
 
     def paginate(
         self,
         *,
         AccountId: str,
         BudgetName: str,
         ActionId: str,
-        TimePeriod: Union[TimePeriodTypeDef, TimePeriodOutputTypeDef] = ...,
+        TimePeriod: TimePeriodUnionTypeDef = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeBudgetActionHistoriesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeBudgetActionHistories.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/paginators/#describebudgetactionhistoriespaginator)
         """
 
@@ -140,15 +139,15 @@
     """
 
     def paginate(
         self,
         *,
         AccountId: str,
         BudgetName: str,
-        TimePeriod: Union[TimePeriodTypeDef, TimePeriodOutputTypeDef] = ...,
+        TimePeriod: TimePeriodUnionTypeDef = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeBudgetPerformanceHistoryResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeBudgetPerformanceHistory.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/paginators/#describebudgetperformancehistorypaginator)
         """
```

### Comparing `mypy-boto3-budgets-1.28.15.post1/mypy_boto3_budgets/type_defs.py` & `mypy-boto3-budgets-1.28.16/mypy_boto3_budgets/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_budgets.type_defs import ActionThresholdTypeDef
 
-    data: ActionThresholdTypeDef = {...}
+    data: ActionThresholdTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -38,19 +38,19 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "ActionThresholdTypeDef",
     "SubscriberTypeDef",
     "HistoricalOptionsTypeDef",
+    "TimestampTypeDef",
     "NotificationTypeDef",
     "CostTypesTypeDef",
     "SpendTypeDef",
     "TimePeriodOutputTypeDef",
-    "TimePeriodTypeDef",
     "ResponseMetadataTypeDef",
     "IamActionDefinitionOutputTypeDef",
     "ScpActionDefinitionOutputTypeDef",
     "SsmActionDefinitionOutputTypeDef",
     "IamActionDefinitionTypeDef",
     "ScpActionDefinitionTypeDef",
     "SsmActionDefinitionTypeDef",
@@ -63,50 +63,54 @@
     "DescribeBudgetNotificationsForAccountRequestRequestTypeDef",
     "DescribeBudgetRequestRequestTypeDef",
     "DescribeBudgetsRequestRequestTypeDef",
     "DescribeNotificationsForBudgetRequestRequestTypeDef",
     "ExecuteBudgetActionRequestRequestTypeDef",
     "AutoAdjustDataOutputTypeDef",
     "AutoAdjustDataTypeDef",
+    "TimePeriodTypeDef",
     "BudgetNotificationsForAccountTypeDef",
     "CreateNotificationRequestRequestTypeDef",
     "CreateSubscriberRequestRequestTypeDef",
     "DeleteNotificationRequestRequestTypeDef",
     "DeleteSubscriberRequestRequestTypeDef",
     "DescribeSubscribersForNotificationRequestRequestTypeDef",
     "NotificationWithSubscribersTypeDef",
     "UpdateNotificationRequestRequestTypeDef",
     "UpdateSubscriberRequestRequestTypeDef",
     "CalculatedSpendTypeDef",
     "BudgetedAndActualAmountsTypeDef",
-    "DescribeBudgetActionHistoriesRequestRequestTypeDef",
-    "DescribeBudgetPerformanceHistoryRequestRequestTypeDef",
     "CreateBudgetActionResponseTypeDef",
     "DescribeNotificationsForBudgetResponseTypeDef",
     "DescribeSubscribersForNotificationResponseTypeDef",
     "ExecuteBudgetActionResponseTypeDef",
     "DefinitionOutputTypeDef",
     "DefinitionTypeDef",
-    "DescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef",
     "DescribeBudgetActionsForAccountRequestDescribeBudgetActionsForAccountPaginateTypeDef",
     "DescribeBudgetActionsForBudgetRequestDescribeBudgetActionsForBudgetPaginateTypeDef",
     "DescribeBudgetNotificationsForAccountRequestDescribeBudgetNotificationsForAccountPaginateTypeDef",
-    "DescribeBudgetPerformanceHistoryRequestDescribeBudgetPerformanceHistoryPaginateTypeDef",
     "DescribeBudgetsRequestDescribeBudgetsPaginateTypeDef",
     "DescribeNotificationsForBudgetRequestDescribeNotificationsForBudgetPaginateTypeDef",
     "DescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef",
+    "DescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef",
+    "DescribeBudgetActionHistoriesRequestRequestTypeDef",
+    "DescribeBudgetPerformanceHistoryRequestDescribeBudgetPerformanceHistoryPaginateTypeDef",
+    "DescribeBudgetPerformanceHistoryRequestRequestTypeDef",
+    "TimePeriodUnionTypeDef",
     "DescribeBudgetNotificationsForAccountResponseTypeDef",
     "BudgetOutputTypeDef",
     "BudgetTypeDef",
     "BudgetPerformanceHistoryTypeDef",
     "ActionTypeDef",
     "CreateBudgetActionRequestRequestTypeDef",
+    "DefinitionUnionTypeDef",
     "UpdateBudgetActionRequestRequestTypeDef",
     "DescribeBudgetResponseTypeDef",
     "DescribeBudgetsResponseTypeDef",
+    "BudgetUnionTypeDef",
     "CreateBudgetRequestRequestTypeDef",
     "UpdateBudgetRequestRequestTypeDef",
     "DescribeBudgetPerformanceHistoryResponseTypeDef",
     "ActionHistoryDetailsTypeDef",
     "DeleteBudgetActionResponseTypeDef",
     "DescribeBudgetActionResponseTypeDef",
     "DescribeBudgetActionsForAccountResponseTypeDef",
@@ -149,14 +153,15 @@
 
 class HistoricalOptionsTypeDef(
     _RequiredHistoricalOptionsTypeDef, _OptionalHistoricalOptionsTypeDef
 ):
     pass
 
 
+TimestampTypeDef = Union[datetime, str]
 _RequiredNotificationTypeDef = TypedDict(
     "_RequiredNotificationTypeDef",
     {
         "NotificationType": NotificationTypeType,
         "ComparisonOperator": ComparisonOperatorType,
         "Threshold": float,
     },
@@ -206,23 +211,14 @@
     {
         "Start": datetime,
         "End": datetime,
     },
     total=False,
 )
 
-TimePeriodTypeDef = TypedDict(
-    "TimePeriodTypeDef",
-    {
-        "Start": Union[datetime, str],
-        "End": Union[datetime, str],
-    },
-    total=False,
-)
-
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -508,24 +504,33 @@
         "AutoAdjustType": AutoAdjustTypeType,
     },
 )
 _OptionalAutoAdjustDataTypeDef = TypedDict(
     "_OptionalAutoAdjustDataTypeDef",
     {
         "HistoricalOptions": HistoricalOptionsTypeDef,
-        "LastAutoAdjustTime": Union[datetime, str],
+        "LastAutoAdjustTime": TimestampTypeDef,
     },
     total=False,
 )
 
 
 class AutoAdjustDataTypeDef(_RequiredAutoAdjustDataTypeDef, _OptionalAutoAdjustDataTypeDef):
     pass
 
 
+TimePeriodTypeDef = TypedDict(
+    "TimePeriodTypeDef",
+    {
+        "Start": TimestampTypeDef,
+        "End": TimestampTypeDef,
+    },
+    total=False,
+)
+
 BudgetNotificationsForAccountTypeDef = TypedDict(
     "BudgetNotificationsForAccountTypeDef",
     {
         "Notifications": List[NotificationTypeDef],
         "BudgetName": str,
     },
     total=False,
@@ -649,65 +654,14 @@
         "BudgetedAmount": SpendTypeDef,
         "ActualAmount": SpendTypeDef,
         "TimePeriod": TimePeriodOutputTypeDef,
     },
     total=False,
 )
 
-_RequiredDescribeBudgetActionHistoriesRequestRequestTypeDef = TypedDict(
-    "_RequiredDescribeBudgetActionHistoriesRequestRequestTypeDef",
-    {
-        "AccountId": str,
-        "BudgetName": str,
-        "ActionId": str,
-    },
-)
-_OptionalDescribeBudgetActionHistoriesRequestRequestTypeDef = TypedDict(
-    "_OptionalDescribeBudgetActionHistoriesRequestRequestTypeDef",
-    {
-        "TimePeriod": TimePeriodTypeDef,
-        "MaxResults": int,
-        "NextToken": str,
-    },
-    total=False,
-)
-
-
-class DescribeBudgetActionHistoriesRequestRequestTypeDef(
-    _RequiredDescribeBudgetActionHistoriesRequestRequestTypeDef,
-    _OptionalDescribeBudgetActionHistoriesRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredDescribeBudgetPerformanceHistoryRequestRequestTypeDef = TypedDict(
-    "_RequiredDescribeBudgetPerformanceHistoryRequestRequestTypeDef",
-    {
-        "AccountId": str,
-        "BudgetName": str,
-    },
-)
-_OptionalDescribeBudgetPerformanceHistoryRequestRequestTypeDef = TypedDict(
-    "_OptionalDescribeBudgetPerformanceHistoryRequestRequestTypeDef",
-    {
-        "TimePeriod": TimePeriodTypeDef,
-        "MaxResults": int,
-        "NextToken": str,
-    },
-    total=False,
-)
-
-
-class DescribeBudgetPerformanceHistoryRequestRequestTypeDef(
-    _RequiredDescribeBudgetPerformanceHistoryRequestRequestTypeDef,
-    _OptionalDescribeBudgetPerformanceHistoryRequestRequestTypeDef,
-):
-    pass
-
-
 CreateBudgetActionResponseTypeDef = TypedDict(
     "CreateBudgetActionResponseTypeDef",
     {
         "AccountId": str,
         "BudgetName": str,
         "ActionId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -759,43 +713,14 @@
         "IamActionDefinition": IamActionDefinitionTypeDef,
         "ScpActionDefinition": ScpActionDefinitionTypeDef,
         "SsmActionDefinition": SsmActionDefinitionTypeDef,
     },
     total=False,
 )
 
-_RequiredDescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef = (
-    TypedDict(
-        "_RequiredDescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef",
-        {
-            "AccountId": str,
-            "BudgetName": str,
-            "ActionId": str,
-        },
-    )
-)
-_OptionalDescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef = (
-    TypedDict(
-        "_OptionalDescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef",
-        {
-            "TimePeriod": TimePeriodTypeDef,
-            "PaginationConfig": PaginatorConfigTypeDef,
-        },
-        total=False,
-    )
-)
-
-
-class DescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef(
-    _RequiredDescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef,
-    _OptionalDescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeBudgetActionsForAccountRequestDescribeBudgetActionsForAccountPaginateTypeDef = TypedDict(
     "_RequiredDescribeBudgetActionsForAccountRequestDescribeBudgetActionsForAccountPaginateTypeDef",
     {
         "AccountId": str,
     },
 )
 _OptionalDescribeBudgetActionsForAccountRequestDescribeBudgetActionsForAccountPaginateTypeDef = TypedDict(
@@ -855,38 +780,14 @@
 class DescribeBudgetNotificationsForAccountRequestDescribeBudgetNotificationsForAccountPaginateTypeDef(
     _RequiredDescribeBudgetNotificationsForAccountRequestDescribeBudgetNotificationsForAccountPaginateTypeDef,
     _OptionalDescribeBudgetNotificationsForAccountRequestDescribeBudgetNotificationsForAccountPaginateTypeDef,
 ):
     pass
 
 
-_RequiredDescribeBudgetPerformanceHistoryRequestDescribeBudgetPerformanceHistoryPaginateTypeDef = TypedDict(
-    "_RequiredDescribeBudgetPerformanceHistoryRequestDescribeBudgetPerformanceHistoryPaginateTypeDef",
-    {
-        "AccountId": str,
-        "BudgetName": str,
-    },
-)
-_OptionalDescribeBudgetPerformanceHistoryRequestDescribeBudgetPerformanceHistoryPaginateTypeDef = TypedDict(
-    "_OptionalDescribeBudgetPerformanceHistoryRequestDescribeBudgetPerformanceHistoryPaginateTypeDef",
-    {
-        "TimePeriod": TimePeriodTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class DescribeBudgetPerformanceHistoryRequestDescribeBudgetPerformanceHistoryPaginateTypeDef(
-    _RequiredDescribeBudgetPerformanceHistoryRequestDescribeBudgetPerformanceHistoryPaginateTypeDef,
-    _OptionalDescribeBudgetPerformanceHistoryRequestDescribeBudgetPerformanceHistoryPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeBudgetsRequestDescribeBudgetsPaginateTypeDef = TypedDict(
     "_RequiredDescribeBudgetsRequestDescribeBudgetsPaginateTypeDef",
     {
         "AccountId": str,
     },
 )
 _OptionalDescribeBudgetsRequestDescribeBudgetsPaginateTypeDef = TypedDict(
@@ -948,14 +849,119 @@
 class DescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef(
     _RequiredDescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef,
     _OptionalDescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef,
 ):
     pass
 
 
+_RequiredDescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef = (
+    TypedDict(
+        "_RequiredDescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef",
+        {
+            "AccountId": str,
+            "BudgetName": str,
+            "ActionId": str,
+        },
+    )
+)
+_OptionalDescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef = (
+    TypedDict(
+        "_OptionalDescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef",
+        {
+            "TimePeriod": TimePeriodTypeDef,
+            "PaginationConfig": PaginatorConfigTypeDef,
+        },
+        total=False,
+    )
+)
+
+
+class DescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef(
+    _RequiredDescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef,
+    _OptionalDescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredDescribeBudgetActionHistoriesRequestRequestTypeDef = TypedDict(
+    "_RequiredDescribeBudgetActionHistoriesRequestRequestTypeDef",
+    {
+        "AccountId": str,
+        "BudgetName": str,
+        "ActionId": str,
+    },
+)
+_OptionalDescribeBudgetActionHistoriesRequestRequestTypeDef = TypedDict(
+    "_OptionalDescribeBudgetActionHistoriesRequestRequestTypeDef",
+    {
+        "TimePeriod": TimePeriodTypeDef,
+        "MaxResults": int,
+        "NextToken": str,
+    },
+    total=False,
+)
+
+
+class DescribeBudgetActionHistoriesRequestRequestTypeDef(
+    _RequiredDescribeBudgetActionHistoriesRequestRequestTypeDef,
+    _OptionalDescribeBudgetActionHistoriesRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredDescribeBudgetPerformanceHistoryRequestDescribeBudgetPerformanceHistoryPaginateTypeDef = TypedDict(
+    "_RequiredDescribeBudgetPerformanceHistoryRequestDescribeBudgetPerformanceHistoryPaginateTypeDef",
+    {
+        "AccountId": str,
+        "BudgetName": str,
+    },
+)
+_OptionalDescribeBudgetPerformanceHistoryRequestDescribeBudgetPerformanceHistoryPaginateTypeDef = TypedDict(
+    "_OptionalDescribeBudgetPerformanceHistoryRequestDescribeBudgetPerformanceHistoryPaginateTypeDef",
+    {
+        "TimePeriod": TimePeriodTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeBudgetPerformanceHistoryRequestDescribeBudgetPerformanceHistoryPaginateTypeDef(
+    _RequiredDescribeBudgetPerformanceHistoryRequestDescribeBudgetPerformanceHistoryPaginateTypeDef,
+    _OptionalDescribeBudgetPerformanceHistoryRequestDescribeBudgetPerformanceHistoryPaginateTypeDef,
+):
+    pass
+
+
+_RequiredDescribeBudgetPerformanceHistoryRequestRequestTypeDef = TypedDict(
+    "_RequiredDescribeBudgetPerformanceHistoryRequestRequestTypeDef",
+    {
+        "AccountId": str,
+        "BudgetName": str,
+    },
+)
+_OptionalDescribeBudgetPerformanceHistoryRequestRequestTypeDef = TypedDict(
+    "_OptionalDescribeBudgetPerformanceHistoryRequestRequestTypeDef",
+    {
+        "TimePeriod": TimePeriodTypeDef,
+        "MaxResults": int,
+        "NextToken": str,
+    },
+    total=False,
+)
+
+
+class DescribeBudgetPerformanceHistoryRequestRequestTypeDef(
+    _RequiredDescribeBudgetPerformanceHistoryRequestRequestTypeDef,
+    _OptionalDescribeBudgetPerformanceHistoryRequestRequestTypeDef,
+):
+    pass
+
+
+TimePeriodUnionTypeDef = Union[TimePeriodTypeDef, TimePeriodOutputTypeDef]
 DescribeBudgetNotificationsForAccountResponseTypeDef = TypedDict(
     "DescribeBudgetNotificationsForAccountResponseTypeDef",
     {
         "BudgetNotificationsForAccount": List[BudgetNotificationsForAccountTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1002,15 +1008,15 @@
     {
         "BudgetLimit": SpendTypeDef,
         "PlannedBudgetLimits": Mapping[str, SpendTypeDef],
         "CostFilters": Mapping[str, Sequence[str]],
         "CostTypes": CostTypesTypeDef,
         "TimePeriod": TimePeriodTypeDef,
         "CalculatedSpend": CalculatedSpendTypeDef,
-        "LastUpdatedTime": Union[datetime, str],
+        "LastUpdatedTime": TimestampTypeDef,
         "AutoAdjustData": AutoAdjustDataTypeDef,
     },
     total=False,
 )
 
 
 class BudgetTypeDef(_RequiredBudgetTypeDef, _OptionalBudgetTypeDef):
@@ -1057,14 +1063,15 @@
         "Definition": DefinitionTypeDef,
         "ExecutionRoleArn": str,
         "ApprovalModel": ApprovalModelType,
         "Subscribers": Sequence[SubscriberTypeDef],
     },
 )
 
+DefinitionUnionTypeDef = Union[DefinitionTypeDef, DefinitionOutputTypeDef]
 _RequiredUpdateBudgetActionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateBudgetActionRequestRequestTypeDef",
     {
         "AccountId": str,
         "BudgetName": str,
         "ActionId": str,
     },
@@ -1103,14 +1110,15 @@
     {
         "Budgets": List[BudgetOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+BudgetUnionTypeDef = Union[BudgetTypeDef, BudgetOutputTypeDef]
 _RequiredCreateBudgetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateBudgetRequestRequestTypeDef",
     {
         "AccountId": str,
         "Budget": BudgetTypeDef,
     },
 )
```

### Comparing `mypy-boto3-budgets-1.28.15.post1/mypy_boto3_budgets/type_defs.pyi` & `mypy-boto3-budgets-1.28.16/mypy_boto3_budgets/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_budgets.type_defs import ActionThresholdTypeDef
 
-    data: ActionThresholdTypeDef = {...}
+    data: ActionThresholdTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -37,19 +37,19 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "ActionThresholdTypeDef",
     "SubscriberTypeDef",
     "HistoricalOptionsTypeDef",
+    "TimestampTypeDef",
     "NotificationTypeDef",
     "CostTypesTypeDef",
     "SpendTypeDef",
     "TimePeriodOutputTypeDef",
-    "TimePeriodTypeDef",
     "ResponseMetadataTypeDef",
     "IamActionDefinitionOutputTypeDef",
     "ScpActionDefinitionOutputTypeDef",
     "SsmActionDefinitionOutputTypeDef",
     "IamActionDefinitionTypeDef",
     "ScpActionDefinitionTypeDef",
     "SsmActionDefinitionTypeDef",
@@ -62,50 +62,54 @@
     "DescribeBudgetNotificationsForAccountRequestRequestTypeDef",
     "DescribeBudgetRequestRequestTypeDef",
     "DescribeBudgetsRequestRequestTypeDef",
     "DescribeNotificationsForBudgetRequestRequestTypeDef",
     "ExecuteBudgetActionRequestRequestTypeDef",
     "AutoAdjustDataOutputTypeDef",
     "AutoAdjustDataTypeDef",
+    "TimePeriodTypeDef",
     "BudgetNotificationsForAccountTypeDef",
     "CreateNotificationRequestRequestTypeDef",
     "CreateSubscriberRequestRequestTypeDef",
     "DeleteNotificationRequestRequestTypeDef",
     "DeleteSubscriberRequestRequestTypeDef",
     "DescribeSubscribersForNotificationRequestRequestTypeDef",
     "NotificationWithSubscribersTypeDef",
     "UpdateNotificationRequestRequestTypeDef",
     "UpdateSubscriberRequestRequestTypeDef",
     "CalculatedSpendTypeDef",
     "BudgetedAndActualAmountsTypeDef",
-    "DescribeBudgetActionHistoriesRequestRequestTypeDef",
-    "DescribeBudgetPerformanceHistoryRequestRequestTypeDef",
     "CreateBudgetActionResponseTypeDef",
     "DescribeNotificationsForBudgetResponseTypeDef",
     "DescribeSubscribersForNotificationResponseTypeDef",
     "ExecuteBudgetActionResponseTypeDef",
     "DefinitionOutputTypeDef",
     "DefinitionTypeDef",
-    "DescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef",
     "DescribeBudgetActionsForAccountRequestDescribeBudgetActionsForAccountPaginateTypeDef",
     "DescribeBudgetActionsForBudgetRequestDescribeBudgetActionsForBudgetPaginateTypeDef",
     "DescribeBudgetNotificationsForAccountRequestDescribeBudgetNotificationsForAccountPaginateTypeDef",
-    "DescribeBudgetPerformanceHistoryRequestDescribeBudgetPerformanceHistoryPaginateTypeDef",
     "DescribeBudgetsRequestDescribeBudgetsPaginateTypeDef",
     "DescribeNotificationsForBudgetRequestDescribeNotificationsForBudgetPaginateTypeDef",
     "DescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef",
+    "DescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef",
+    "DescribeBudgetActionHistoriesRequestRequestTypeDef",
+    "DescribeBudgetPerformanceHistoryRequestDescribeBudgetPerformanceHistoryPaginateTypeDef",
+    "DescribeBudgetPerformanceHistoryRequestRequestTypeDef",
+    "TimePeriodUnionTypeDef",
     "DescribeBudgetNotificationsForAccountResponseTypeDef",
     "BudgetOutputTypeDef",
     "BudgetTypeDef",
     "BudgetPerformanceHistoryTypeDef",
     "ActionTypeDef",
     "CreateBudgetActionRequestRequestTypeDef",
+    "DefinitionUnionTypeDef",
     "UpdateBudgetActionRequestRequestTypeDef",
     "DescribeBudgetResponseTypeDef",
     "DescribeBudgetsResponseTypeDef",
+    "BudgetUnionTypeDef",
     "CreateBudgetRequestRequestTypeDef",
     "UpdateBudgetRequestRequestTypeDef",
     "DescribeBudgetPerformanceHistoryResponseTypeDef",
     "ActionHistoryDetailsTypeDef",
     "DeleteBudgetActionResponseTypeDef",
     "DescribeBudgetActionResponseTypeDef",
     "DescribeBudgetActionsForAccountResponseTypeDef",
@@ -146,14 +150,15 @@
 )
 
 class HistoricalOptionsTypeDef(
     _RequiredHistoricalOptionsTypeDef, _OptionalHistoricalOptionsTypeDef
 ):
     pass
 
+TimestampTypeDef = Union[datetime, str]
 _RequiredNotificationTypeDef = TypedDict(
     "_RequiredNotificationTypeDef",
     {
         "NotificationType": NotificationTypeType,
         "ComparisonOperator": ComparisonOperatorType,
         "Threshold": float,
     },
@@ -201,23 +206,14 @@
     {
         "Start": datetime,
         "End": datetime,
     },
     total=False,
 )
 
-TimePeriodTypeDef = TypedDict(
-    "TimePeriodTypeDef",
-    {
-        "Start": Union[datetime, str],
-        "End": Union[datetime, str],
-    },
-    total=False,
-)
-
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -487,22 +483,31 @@
         "AutoAdjustType": AutoAdjustTypeType,
     },
 )
 _OptionalAutoAdjustDataTypeDef = TypedDict(
     "_OptionalAutoAdjustDataTypeDef",
     {
         "HistoricalOptions": HistoricalOptionsTypeDef,
-        "LastAutoAdjustTime": Union[datetime, str],
+        "LastAutoAdjustTime": TimestampTypeDef,
     },
     total=False,
 )
 
 class AutoAdjustDataTypeDef(_RequiredAutoAdjustDataTypeDef, _OptionalAutoAdjustDataTypeDef):
     pass
 
+TimePeriodTypeDef = TypedDict(
+    "TimePeriodTypeDef",
+    {
+        "Start": TimestampTypeDef,
+        "End": TimestampTypeDef,
+    },
+    total=False,
+)
+
 BudgetNotificationsForAccountTypeDef = TypedDict(
     "BudgetNotificationsForAccountTypeDef",
     {
         "Notifications": List[NotificationTypeDef],
         "BudgetName": str,
     },
     total=False,
@@ -622,61 +627,14 @@
         "BudgetedAmount": SpendTypeDef,
         "ActualAmount": SpendTypeDef,
         "TimePeriod": TimePeriodOutputTypeDef,
     },
     total=False,
 )
 
-_RequiredDescribeBudgetActionHistoriesRequestRequestTypeDef = TypedDict(
-    "_RequiredDescribeBudgetActionHistoriesRequestRequestTypeDef",
-    {
-        "AccountId": str,
-        "BudgetName": str,
-        "ActionId": str,
-    },
-)
-_OptionalDescribeBudgetActionHistoriesRequestRequestTypeDef = TypedDict(
-    "_OptionalDescribeBudgetActionHistoriesRequestRequestTypeDef",
-    {
-        "TimePeriod": TimePeriodTypeDef,
-        "MaxResults": int,
-        "NextToken": str,
-    },
-    total=False,
-)
-
-class DescribeBudgetActionHistoriesRequestRequestTypeDef(
-    _RequiredDescribeBudgetActionHistoriesRequestRequestTypeDef,
-    _OptionalDescribeBudgetActionHistoriesRequestRequestTypeDef,
-):
-    pass
-
-_RequiredDescribeBudgetPerformanceHistoryRequestRequestTypeDef = TypedDict(
-    "_RequiredDescribeBudgetPerformanceHistoryRequestRequestTypeDef",
-    {
-        "AccountId": str,
-        "BudgetName": str,
-    },
-)
-_OptionalDescribeBudgetPerformanceHistoryRequestRequestTypeDef = TypedDict(
-    "_OptionalDescribeBudgetPerformanceHistoryRequestRequestTypeDef",
-    {
-        "TimePeriod": TimePeriodTypeDef,
-        "MaxResults": int,
-        "NextToken": str,
-    },
-    total=False,
-)
-
-class DescribeBudgetPerformanceHistoryRequestRequestTypeDef(
-    _RequiredDescribeBudgetPerformanceHistoryRequestRequestTypeDef,
-    _OptionalDescribeBudgetPerformanceHistoryRequestRequestTypeDef,
-):
-    pass
-
 CreateBudgetActionResponseTypeDef = TypedDict(
     "CreateBudgetActionResponseTypeDef",
     {
         "AccountId": str,
         "BudgetName": str,
         "ActionId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -728,41 +686,14 @@
         "IamActionDefinition": IamActionDefinitionTypeDef,
         "ScpActionDefinition": ScpActionDefinitionTypeDef,
         "SsmActionDefinition": SsmActionDefinitionTypeDef,
     },
     total=False,
 )
 
-_RequiredDescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef = (
-    TypedDict(
-        "_RequiredDescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef",
-        {
-            "AccountId": str,
-            "BudgetName": str,
-            "ActionId": str,
-        },
-    )
-)
-_OptionalDescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef = (
-    TypedDict(
-        "_OptionalDescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef",
-        {
-            "TimePeriod": TimePeriodTypeDef,
-            "PaginationConfig": PaginatorConfigTypeDef,
-        },
-        total=False,
-    )
-)
-
-class DescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef(
-    _RequiredDescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef,
-    _OptionalDescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef,
-):
-    pass
-
 _RequiredDescribeBudgetActionsForAccountRequestDescribeBudgetActionsForAccountPaginateTypeDef = TypedDict(
     "_RequiredDescribeBudgetActionsForAccountRequestDescribeBudgetActionsForAccountPaginateTypeDef",
     {
         "AccountId": str,
     },
 )
 _OptionalDescribeBudgetActionsForAccountRequestDescribeBudgetActionsForAccountPaginateTypeDef = TypedDict(
@@ -816,36 +747,14 @@
 
 class DescribeBudgetNotificationsForAccountRequestDescribeBudgetNotificationsForAccountPaginateTypeDef(
     _RequiredDescribeBudgetNotificationsForAccountRequestDescribeBudgetNotificationsForAccountPaginateTypeDef,
     _OptionalDescribeBudgetNotificationsForAccountRequestDescribeBudgetNotificationsForAccountPaginateTypeDef,
 ):
     pass
 
-_RequiredDescribeBudgetPerformanceHistoryRequestDescribeBudgetPerformanceHistoryPaginateTypeDef = TypedDict(
-    "_RequiredDescribeBudgetPerformanceHistoryRequestDescribeBudgetPerformanceHistoryPaginateTypeDef",
-    {
-        "AccountId": str,
-        "BudgetName": str,
-    },
-)
-_OptionalDescribeBudgetPerformanceHistoryRequestDescribeBudgetPerformanceHistoryPaginateTypeDef = TypedDict(
-    "_OptionalDescribeBudgetPerformanceHistoryRequestDescribeBudgetPerformanceHistoryPaginateTypeDef",
-    {
-        "TimePeriod": TimePeriodTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class DescribeBudgetPerformanceHistoryRequestDescribeBudgetPerformanceHistoryPaginateTypeDef(
-    _RequiredDescribeBudgetPerformanceHistoryRequestDescribeBudgetPerformanceHistoryPaginateTypeDef,
-    _OptionalDescribeBudgetPerformanceHistoryRequestDescribeBudgetPerformanceHistoryPaginateTypeDef,
-):
-    pass
-
 _RequiredDescribeBudgetsRequestDescribeBudgetsPaginateTypeDef = TypedDict(
     "_RequiredDescribeBudgetsRequestDescribeBudgetsPaginateTypeDef",
     {
         "AccountId": str,
     },
 )
 _OptionalDescribeBudgetsRequestDescribeBudgetsPaginateTypeDef = TypedDict(
@@ -901,14 +810,111 @@
 
 class DescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef(
     _RequiredDescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef,
     _OptionalDescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef,
 ):
     pass
 
+_RequiredDescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef = (
+    TypedDict(
+        "_RequiredDescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef",
+        {
+            "AccountId": str,
+            "BudgetName": str,
+            "ActionId": str,
+        },
+    )
+)
+_OptionalDescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef = (
+    TypedDict(
+        "_OptionalDescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef",
+        {
+            "TimePeriod": TimePeriodTypeDef,
+            "PaginationConfig": PaginatorConfigTypeDef,
+        },
+        total=False,
+    )
+)
+
+class DescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef(
+    _RequiredDescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef,
+    _OptionalDescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef,
+):
+    pass
+
+_RequiredDescribeBudgetActionHistoriesRequestRequestTypeDef = TypedDict(
+    "_RequiredDescribeBudgetActionHistoriesRequestRequestTypeDef",
+    {
+        "AccountId": str,
+        "BudgetName": str,
+        "ActionId": str,
+    },
+)
+_OptionalDescribeBudgetActionHistoriesRequestRequestTypeDef = TypedDict(
+    "_OptionalDescribeBudgetActionHistoriesRequestRequestTypeDef",
+    {
+        "TimePeriod": TimePeriodTypeDef,
+        "MaxResults": int,
+        "NextToken": str,
+    },
+    total=False,
+)
+
+class DescribeBudgetActionHistoriesRequestRequestTypeDef(
+    _RequiredDescribeBudgetActionHistoriesRequestRequestTypeDef,
+    _OptionalDescribeBudgetActionHistoriesRequestRequestTypeDef,
+):
+    pass
+
+_RequiredDescribeBudgetPerformanceHistoryRequestDescribeBudgetPerformanceHistoryPaginateTypeDef = TypedDict(
+    "_RequiredDescribeBudgetPerformanceHistoryRequestDescribeBudgetPerformanceHistoryPaginateTypeDef",
+    {
+        "AccountId": str,
+        "BudgetName": str,
+    },
+)
+_OptionalDescribeBudgetPerformanceHistoryRequestDescribeBudgetPerformanceHistoryPaginateTypeDef = TypedDict(
+    "_OptionalDescribeBudgetPerformanceHistoryRequestDescribeBudgetPerformanceHistoryPaginateTypeDef",
+    {
+        "TimePeriod": TimePeriodTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeBudgetPerformanceHistoryRequestDescribeBudgetPerformanceHistoryPaginateTypeDef(
+    _RequiredDescribeBudgetPerformanceHistoryRequestDescribeBudgetPerformanceHistoryPaginateTypeDef,
+    _OptionalDescribeBudgetPerformanceHistoryRequestDescribeBudgetPerformanceHistoryPaginateTypeDef,
+):
+    pass
+
+_RequiredDescribeBudgetPerformanceHistoryRequestRequestTypeDef = TypedDict(
+    "_RequiredDescribeBudgetPerformanceHistoryRequestRequestTypeDef",
+    {
+        "AccountId": str,
+        "BudgetName": str,
+    },
+)
+_OptionalDescribeBudgetPerformanceHistoryRequestRequestTypeDef = TypedDict(
+    "_OptionalDescribeBudgetPerformanceHistoryRequestRequestTypeDef",
+    {
+        "TimePeriod": TimePeriodTypeDef,
+        "MaxResults": int,
+        "NextToken": str,
+    },
+    total=False,
+)
+
+class DescribeBudgetPerformanceHistoryRequestRequestTypeDef(
+    _RequiredDescribeBudgetPerformanceHistoryRequestRequestTypeDef,
+    _OptionalDescribeBudgetPerformanceHistoryRequestRequestTypeDef,
+):
+    pass
+
+TimePeriodUnionTypeDef = Union[TimePeriodTypeDef, TimePeriodOutputTypeDef]
 DescribeBudgetNotificationsForAccountResponseTypeDef = TypedDict(
     "DescribeBudgetNotificationsForAccountResponseTypeDef",
     {
         "BudgetNotificationsForAccount": List[BudgetNotificationsForAccountTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -953,15 +959,15 @@
     {
         "BudgetLimit": SpendTypeDef,
         "PlannedBudgetLimits": Mapping[str, SpendTypeDef],
         "CostFilters": Mapping[str, Sequence[str]],
         "CostTypes": CostTypesTypeDef,
         "TimePeriod": TimePeriodTypeDef,
         "CalculatedSpend": CalculatedSpendTypeDef,
-        "LastUpdatedTime": Union[datetime, str],
+        "LastUpdatedTime": TimestampTypeDef,
         "AutoAdjustData": AutoAdjustDataTypeDef,
     },
     total=False,
 )
 
 class BudgetTypeDef(_RequiredBudgetTypeDef, _OptionalBudgetTypeDef):
     pass
@@ -1006,14 +1012,15 @@
         "Definition": DefinitionTypeDef,
         "ExecutionRoleArn": str,
         "ApprovalModel": ApprovalModelType,
         "Subscribers": Sequence[SubscriberTypeDef],
     },
 )
 
+DefinitionUnionTypeDef = Union[DefinitionTypeDef, DefinitionOutputTypeDef]
 _RequiredUpdateBudgetActionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateBudgetActionRequestRequestTypeDef",
     {
         "AccountId": str,
         "BudgetName": str,
         "ActionId": str,
     },
@@ -1050,14 +1057,15 @@
     {
         "Budgets": List[BudgetOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+BudgetUnionTypeDef = Union[BudgetTypeDef, BudgetOutputTypeDef]
 _RequiredCreateBudgetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateBudgetRequestRequestTypeDef",
     {
         "AccountId": str,
         "Budget": BudgetTypeDef,
     },
 )
```

### Comparing `mypy-boto3-budgets-1.28.15.post1/mypy_boto3_budgets.egg-info/PKG-INFO` & `mypy-boto3-budgets-1.28.16/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,61 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-budgets
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.Budgets 1.28.15 service generated with mypy-boto3-builder 7.16.2
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 budgets type-annotations boto3-stubs mypy typeshed autocomplete
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <a id="mypy-boto3-budgets"></a>
 
 # mypy-boto3-budgets
 
 [![PyPI - mypy-boto3-budgets](https://img.shields.io/pypi/v/mypy-boto3-budgets.svg?color=blue)](https://pypi.org/project/mypy-boto3-budgets)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-budgets.svg?color=blue)](https://pypi.org/project/mypy-boto3-budgets)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-budgets)](https://pepy.tech/project/mypy-boto3-budgets)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Budgets 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets)
+[boto3.Budgets 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets)
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
 [mypy-boto3-budgets docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/).
 
 See how it helps to find and fix potential bugs:
 
@@ -74,15 +42,15 @@
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
@@ -359,31 +327,31 @@
 )
 
 
 def check_value(value: ActionStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_budgets.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_budgets.type_defs import (
     ActionThresholdTypeDef,
     SubscriberTypeDef,
     HistoricalOptionsTypeDef,
+    TimestampTypeDef,
     NotificationTypeDef,
     CostTypesTypeDef,
     SpendTypeDef,
     TimePeriodOutputTypeDef,
-    TimePeriodTypeDef,
     ResponseMetadataTypeDef,
     IamActionDefinitionOutputTypeDef,
     ScpActionDefinitionOutputTypeDef,
     SsmActionDefinitionOutputTypeDef,
     IamActionDefinitionTypeDef,
     ScpActionDefinitionTypeDef,
     SsmActionDefinitionTypeDef,
@@ -396,65 +364,69 @@
     DescribeBudgetNotificationsForAccountRequestRequestTypeDef,
     DescribeBudgetRequestRequestTypeDef,
     DescribeBudgetsRequestRequestTypeDef,
     DescribeNotificationsForBudgetRequestRequestTypeDef,
     ExecuteBudgetActionRequestRequestTypeDef,
     AutoAdjustDataOutputTypeDef,
     AutoAdjustDataTypeDef,
+    TimePeriodTypeDef,
     BudgetNotificationsForAccountTypeDef,
     CreateNotificationRequestRequestTypeDef,
     CreateSubscriberRequestRequestTypeDef,
     DeleteNotificationRequestRequestTypeDef,
     DeleteSubscriberRequestRequestTypeDef,
     DescribeSubscribersForNotificationRequestRequestTypeDef,
     NotificationWithSubscribersTypeDef,
     UpdateNotificationRequestRequestTypeDef,
     UpdateSubscriberRequestRequestTypeDef,
     CalculatedSpendTypeDef,
     BudgetedAndActualAmountsTypeDef,
-    DescribeBudgetActionHistoriesRequestRequestTypeDef,
-    DescribeBudgetPerformanceHistoryRequestRequestTypeDef,
     CreateBudgetActionResponseTypeDef,
     DescribeNotificationsForBudgetResponseTypeDef,
     DescribeSubscribersForNotificationResponseTypeDef,
     ExecuteBudgetActionResponseTypeDef,
     DefinitionOutputTypeDef,
     DefinitionTypeDef,
-    DescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef,
     DescribeBudgetActionsForAccountRequestDescribeBudgetActionsForAccountPaginateTypeDef,
     DescribeBudgetActionsForBudgetRequestDescribeBudgetActionsForBudgetPaginateTypeDef,
     DescribeBudgetNotificationsForAccountRequestDescribeBudgetNotificationsForAccountPaginateTypeDef,
-    DescribeBudgetPerformanceHistoryRequestDescribeBudgetPerformanceHistoryPaginateTypeDef,
     DescribeBudgetsRequestDescribeBudgetsPaginateTypeDef,
     DescribeNotificationsForBudgetRequestDescribeNotificationsForBudgetPaginateTypeDef,
     DescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef,
+    DescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef,
+    DescribeBudgetActionHistoriesRequestRequestTypeDef,
+    DescribeBudgetPerformanceHistoryRequestDescribeBudgetPerformanceHistoryPaginateTypeDef,
+    DescribeBudgetPerformanceHistoryRequestRequestTypeDef,
+    TimePeriodUnionTypeDef,
     DescribeBudgetNotificationsForAccountResponseTypeDef,
     BudgetOutputTypeDef,
     BudgetTypeDef,
     BudgetPerformanceHistoryTypeDef,
     ActionTypeDef,
     CreateBudgetActionRequestRequestTypeDef,
+    DefinitionUnionTypeDef,
     UpdateBudgetActionRequestRequestTypeDef,
     DescribeBudgetResponseTypeDef,
     DescribeBudgetsResponseTypeDef,
+    BudgetUnionTypeDef,
     CreateBudgetRequestRequestTypeDef,
     UpdateBudgetRequestRequestTypeDef,
     DescribeBudgetPerformanceHistoryResponseTypeDef,
     ActionHistoryDetailsTypeDef,
     DeleteBudgetActionResponseTypeDef,
     DescribeBudgetActionResponseTypeDef,
     DescribeBudgetActionsForAccountResponseTypeDef,
     DescribeBudgetActionsForBudgetResponseTypeDef,
     UpdateBudgetActionResponseTypeDef,
     ActionHistoryTypeDef,
     DescribeBudgetActionHistoriesResponseTypeDef,
 )
 
 
-def get_structure() -> ActionThresholdTypeDef:
+def get_value() -> ActionThresholdTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-budgets-1.28.15.post1/mypy_boto3_budgets.egg-info/SOURCES.txt` & `mypy-boto3-budgets-1.28.16/mypy_boto3_budgets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-budgets-1.28.15.post1/setup.py` & `mypy-boto3-budgets-1.28.16/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-budgets",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_budgets"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Budgets 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.2"
+        "Type annotations for boto3.Budgets 1.28.16 service generated with mypy-boto3-builder"
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
-    keywords="boto3 budgets type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 budgets type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_budgets": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

