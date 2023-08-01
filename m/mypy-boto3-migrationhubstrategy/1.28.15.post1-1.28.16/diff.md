# Comparing `tmp/mypy-boto3-migrationhubstrategy-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-migrationhubstrategy-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-migrationhubstrategy-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:44 2023, max compression
+gzip compressed data, was "mypy-boto3-migrationhubstrategy-1.28.16.tar", last modified: Tue Aug  1 11:37:24 2023, max compression
```

## Comparing `mypy-boto3-migrationhubstrategy-1.28.15.post1.tar` & `mypy-boto3-migrationhubstrategy-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:44.229300 mypy-boto3-migrationhubstrategy-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:51:46.000000 mypy-boto3-migrationhubstrategy-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19272 2023-07-29 10:03:44.221300 mypy-boto3-migrationhubstrategy-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17712 2023-07-29 09:51:46.000000 mypy-boto3-migrationhubstrategy-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:44.209300 mypy-boto3-migrationhubstrategy-1.28.15.post1/mypy_boto3_migrationhubstrategy/
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-07-29 09:51:46.000000 mypy-boto3-migrationhubstrategy-1.28.15.post1/mypy_boto3_migrationhubstrategy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-07-29 09:51:46.000000 mypy-boto3-migrationhubstrategy-1.28.15.post1/mypy_boto3_migrationhubstrategy/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-29 09:51:46.000000 mypy-boto3-migrationhubstrategy-1.28.15.post1/mypy_boto3_migrationhubstrategy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21098 2023-07-29 09:51:46.000000 mypy-boto3-migrationhubstrategy-1.28.15.post1/mypy_boto3_migrationhubstrategy/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    21065 2023-07-29 09:51:46.000000 mypy-boto3-migrationhubstrategy-1.28.15.post1/mypy_boto3_migrationhubstrategy/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15739 2023-07-29 09:51:47.000000 mypy-boto3-migrationhubstrategy-1.28.15.post1/mypy_boto3_migrationhubstrategy/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    15737 2023-07-29 09:51:46.000000 mypy-boto3-migrationhubstrategy-1.28.15.post1/mypy_boto3_migrationhubstrategy/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7255 2023-07-29 09:51:46.000000 mypy-boto3-migrationhubstrategy-1.28.15.post1/mypy_boto3_migrationhubstrategy/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7248 2023-07-29 09:51:46.000000 mypy-boto3-migrationhubstrategy-1.28.15.post1/mypy_boto3_migrationhubstrategy/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:51:46.000000 mypy-boto3-migrationhubstrategy-1.28.15.post1/mypy_boto3_migrationhubstrategy/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    34575 2023-07-29 09:51:47.000000 mypy-boto3-migrationhubstrategy-1.28.15.post1/mypy_boto3_migrationhubstrategy/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    34564 2023-07-29 09:51:47.000000 mypy-boto3-migrationhubstrategy-1.28.15.post1/mypy_boto3_migrationhubstrategy/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:51:46.000000 mypy-boto3-migrationhubstrategy-1.28.15.post1/mypy_boto3_migrationhubstrategy/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:44.221300 mypy-boto3-migrationhubstrategy-1.28.15.post1/mypy_boto3_migrationhubstrategy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19272 2023-07-29 10:03:43.000000 mypy-boto3-migrationhubstrategy-1.28.15.post1/mypy_boto3_migrationhubstrategy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-29 10:03:44.000000 mypy-boto3-migrationhubstrategy-1.28.15.post1/mypy_boto3_migrationhubstrategy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:43.000000 mypy-boto3-migrationhubstrategy-1.28.15.post1/mypy_boto3_migrationhubstrategy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:43.000000 mypy-boto3-migrationhubstrategy-1.28.15.post1/mypy_boto3_migrationhubstrategy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:43.000000 mypy-boto3-migrationhubstrategy-1.28.15.post1/mypy_boto3_migrationhubstrategy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-29 10:03:43.000000 mypy-boto3-migrationhubstrategy-1.28.15.post1/mypy_boto3_migrationhubstrategy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:44.229300 mypy-boto3-migrationhubstrategy-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-07-29 09:51:46.000000 mypy-boto3-migrationhubstrategy-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:24.084812 mypy-boto3-migrationhubstrategy-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:24:43.000000 mypy-boto3-migrationhubstrategy-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19373 2023-08-01 11:37:24.084812 mypy-boto3-migrationhubstrategy-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17822 2023-08-01 11:24:43.000000 mypy-boto3-migrationhubstrategy-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:24.064812 mypy-boto3-migrationhubstrategy-1.28.16/mypy_boto3_migrationhubstrategy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-08-01 11:24:43.000000 mypy-boto3-migrationhubstrategy-1.28.16/mypy_boto3_migrationhubstrategy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-08-01 11:24:43.000000 mypy-boto3-migrationhubstrategy-1.28.16/mypy_boto3_migrationhubstrategy/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-08-01 11:24:43.000000 mypy-boto3-migrationhubstrategy-1.28.16/mypy_boto3_migrationhubstrategy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20818 2023-08-01 11:24:43.000000 mypy-boto3-migrationhubstrategy-1.28.16/mypy_boto3_migrationhubstrategy/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20785 2023-08-01 11:24:43.000000 mypy-boto3-migrationhubstrategy-1.28.16/mypy_boto3_migrationhubstrategy/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15739 2023-08-01 11:24:44.000000 mypy-boto3-migrationhubstrategy-1.28.16/mypy_boto3_migrationhubstrategy/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15737 2023-08-01 11:24:44.000000 mypy-boto3-migrationhubstrategy-1.28.16/mypy_boto3_migrationhubstrategy/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7255 2023-08-01 11:24:43.000000 mypy-boto3-migrationhubstrategy-1.28.16/mypy_boto3_migrationhubstrategy/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7248 2023-08-01 11:24:43.000000 mypy-boto3-migrationhubstrategy-1.28.16/mypy_boto3_migrationhubstrategy/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:24:43.000000 mypy-boto3-migrationhubstrategy-1.28.16/mypy_boto3_migrationhubstrategy/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    34953 2023-08-01 11:24:45.000000 mypy-boto3-migrationhubstrategy-1.28.16/mypy_boto3_migrationhubstrategy/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34942 2023-08-01 11:24:44.000000 mypy-boto3-migrationhubstrategy-1.28.16/mypy_boto3_migrationhubstrategy/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:24:43.000000 mypy-boto3-migrationhubstrategy-1.28.16/mypy_boto3_migrationhubstrategy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:24.084812 mypy-boto3-migrationhubstrategy-1.28.16/mypy_boto3_migrationhubstrategy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19373 2023-08-01 11:37:23.000000 mypy-boto3-migrationhubstrategy-1.28.16/mypy_boto3_migrationhubstrategy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-08-01 11:37:23.000000 mypy-boto3-migrationhubstrategy-1.28.16/mypy_boto3_migrationhubstrategy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:23.000000 mypy-boto3-migrationhubstrategy-1.28.16/mypy_boto3_migrationhubstrategy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:23.000000 mypy-boto3-migrationhubstrategy-1.28.16/mypy_boto3_migrationhubstrategy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:23.000000 mypy-boto3-migrationhubstrategy-1.28.16/mypy_boto3_migrationhubstrategy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-01 11:37:23.000000 mypy-boto3-migrationhubstrategy-1.28.16/mypy_boto3_migrationhubstrategy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:24.084812 mypy-boto3-migrationhubstrategy-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-08-01 11:24:43.000000 mypy-boto3-migrationhubstrategy-1.28.16/setup.py
```

### Comparing `mypy-boto3-migrationhubstrategy-1.28.15.post1/LICENSE` & `mypy-boto3-migrationhubstrategy-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migrationhubstrategy-1.28.15.post1/PKG-INFO` & `mypy-boto3-migrationhubstrategy-1.28.16/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,61 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-migrationhubstrategy
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.MigrationHubStrategyRecommendations 1.28.15 service generated with mypy-boto3-builder 7.16.2
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhubstrategy/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 migrationhubstrategy type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-migrationhubstrategy"></a>
 
 # mypy-boto3-migrationhubstrategy
 
 [![PyPI - mypy-boto3-migrationhubstrategy](https://img.shields.io/pypi/v/mypy-boto3-migrationhubstrategy.svg?color=blue)](https://pypi.org/project/mypy-boto3-migrationhubstrategy)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-migrationhubstrategy.svg?color=blue)](https://pypi.org/project/mypy-boto3-migrationhubstrategy)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhubstrategy/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-migrationhubstrategy)](https://pepy.tech/project/mypy-boto3-migrationhubstrategy)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MigrationHubStrategyRecommendations 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations)
+[boto3.MigrationHubStrategyRecommendations 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations)
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
 [mypy-boto3-migrationhubstrategy docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhubstrategy/).
 
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
@@ -373,20 +341,20 @@
 )
 
 
 def check_value(value: AnalysisTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_migrationhubstrategy.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_migrationhubstrategy.type_defs import (
     AnalysisStatusUnionTypeDef,
     AnalyzerNameUnionTypeDef,
     S3ObjectTypeDef,
     AntipatternSeveritySummaryTypeDef,
@@ -439,15 +407,15 @@
     TransformationToolTypeDef,
     ServerErrorTypeDef,
     SourceCodeTypeDef,
     StopAssessmentRequestRequestTypeDef,
     StrategyOptionTypeDef,
     AntipatternReportResultTypeDef,
     AssessmentSummaryTypeDef,
-    StartAssessmentRequestRequestTypeDef,
+    AssessmentTargetUnionTypeDef,
     PrioritizeBusinessGoalsTypeDef,
     ConfigurationSummaryTypeDef,
     DatabaseMigrationPreferenceOutputTypeDef,
     DatabaseMigrationPreferenceTypeDef,
     GetAssessmentResponseTypeDef,
     GetImportFileTaskResponseTypeDef,
     GetLatestAssessmentIdResponseTypeDef,
@@ -469,36 +437,39 @@
     ManagementPreferenceTypeDef,
     SystemInfoTypeDef,
     RecommendationSetTypeDef,
     UpdateApplicationComponentConfigRequestRequestTypeDef,
     UpdateServerConfigRequestRequestTypeDef,
     ResultTypeDef,
     GetPortfolioSummaryResponseTypeDef,
+    StartAssessmentRequestRequestTypeDef,
     CollectorTypeDef,
     DatabasePreferencesOutputTypeDef,
     DatabasePreferencesTypeDef,
     ApplicationPreferencesOutputTypeDef,
     ApplicationPreferencesTypeDef,
     ApplicationComponentStrategyTypeDef,
     ServerDetailTypeDef,
     ServerStrategyTypeDef,
     ApplicationComponentDetailTypeDef,
     ListCollectorsResponseTypeDef,
+    DatabasePreferencesUnionTypeDef,
     GetPortfolioPreferencesResponseTypeDef,
+    ApplicationPreferencesUnionTypeDef,
     PutPortfolioPreferencesRequestRequestTypeDef,
     GetApplicationComponentStrategiesResponseTypeDef,
     GetServerDetailsResponseTypeDef,
     ListServersResponseTypeDef,
     GetServerStrategiesResponseTypeDef,
     GetApplicationComponentDetailsResponseTypeDef,
     ListApplicationComponentsResponseTypeDef,
 )
 
 
-def get_structure() -> AnalysisStatusUnionTypeDef:
+def get_value() -> AnalysisStatusUnionTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-migrationhubstrategy-1.28.15.post1/README.md` & `mypy-boto3-migrationhubstrategy-1.28.16/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-migrationhubstrategy
+Version: 1.28.16
+Summary: Type annotations for boto3.MigrationHubStrategyRecommendations 1.28.16 service generated with mypy-boto3-builder 7.17.1
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhubstrategy/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 migrationhubstrategy type-annotations botocore mypy typeshed autocomplete
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
 <a id="mypy-boto3-migrationhubstrategy"></a>
 
 # mypy-boto3-migrationhubstrategy
 
 [![PyPI - mypy-boto3-migrationhubstrategy](https://img.shields.io/pypi/v/mypy-boto3-migrationhubstrategy.svg?color=blue)](https://pypi.org/project/mypy-boto3-migrationhubstrategy)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-migrationhubstrategy.svg?color=blue)](https://pypi.org/project/mypy-boto3-migrationhubstrategy)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhubstrategy/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-migrationhubstrategy)](https://pepy.tech/project/mypy-boto3-migrationhubstrategy)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MigrationHubStrategyRecommendations 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations)
+[boto3.MigrationHubStrategyRecommendations 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations)
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
 [mypy-boto3-migrationhubstrategy docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhubstrategy/).
 
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
@@ -341,20 +373,20 @@
 )
 
 
 def check_value(value: AnalysisTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_migrationhubstrategy.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_migrationhubstrategy.type_defs import (
     AnalysisStatusUnionTypeDef,
     AnalyzerNameUnionTypeDef,
     S3ObjectTypeDef,
     AntipatternSeveritySummaryTypeDef,
@@ -407,15 +439,15 @@
     TransformationToolTypeDef,
     ServerErrorTypeDef,
     SourceCodeTypeDef,
     StopAssessmentRequestRequestTypeDef,
     StrategyOptionTypeDef,
     AntipatternReportResultTypeDef,
     AssessmentSummaryTypeDef,
-    StartAssessmentRequestRequestTypeDef,
+    AssessmentTargetUnionTypeDef,
     PrioritizeBusinessGoalsTypeDef,
     ConfigurationSummaryTypeDef,
     DatabaseMigrationPreferenceOutputTypeDef,
     DatabaseMigrationPreferenceTypeDef,
     GetAssessmentResponseTypeDef,
     GetImportFileTaskResponseTypeDef,
     GetLatestAssessmentIdResponseTypeDef,
@@ -437,36 +469,39 @@
     ManagementPreferenceTypeDef,
     SystemInfoTypeDef,
     RecommendationSetTypeDef,
     UpdateApplicationComponentConfigRequestRequestTypeDef,
     UpdateServerConfigRequestRequestTypeDef,
     ResultTypeDef,
     GetPortfolioSummaryResponseTypeDef,
+    StartAssessmentRequestRequestTypeDef,
     CollectorTypeDef,
     DatabasePreferencesOutputTypeDef,
     DatabasePreferencesTypeDef,
     ApplicationPreferencesOutputTypeDef,
     ApplicationPreferencesTypeDef,
     ApplicationComponentStrategyTypeDef,
     ServerDetailTypeDef,
     ServerStrategyTypeDef,
     ApplicationComponentDetailTypeDef,
     ListCollectorsResponseTypeDef,
+    DatabasePreferencesUnionTypeDef,
     GetPortfolioPreferencesResponseTypeDef,
+    ApplicationPreferencesUnionTypeDef,
     PutPortfolioPreferencesRequestRequestTypeDef,
     GetApplicationComponentStrategiesResponseTypeDef,
     GetServerDetailsResponseTypeDef,
     ListServersResponseTypeDef,
     GetServerStrategiesResponseTypeDef,
     GetApplicationComponentDetailsResponseTypeDef,
     ListApplicationComponentsResponseTypeDef,
 )
 
 
-def get_structure() -> AnalysisStatusUnionTypeDef:
+def get_value() -> AnalysisStatusUnionTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-migrationhubstrategy-1.28.15.post1/mypy_boto3_migrationhubstrategy/__init__.py` & `mypy-boto3-migrationhubstrategy-1.28.16/mypy_boto3_migrationhubstrategy/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migrationhubstrategy-1.28.15.post1/mypy_boto3_migrationhubstrategy/__init__.pyi` & `mypy-boto3-migrationhubstrategy-1.28.16/mypy_boto3_migrationhubstrategy/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migrationhubstrategy-1.28.15.post1/mypy_boto3_migrationhubstrategy/__main__.py` & `mypy-boto3-migrationhubstrategy-1.28.16/mypy_boto3_migrationhubstrategy/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.MigrationHubStrategyRecommendations 1.28.15\nVersion:        "
-        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.MigrationHubStrategyRecommendations 1.28.16\nVersion:        "
+        " 1.28.16\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhubstrategy//\nBoto3 docs:"
         "     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations\nOther"
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

### Comparing `mypy-boto3-migrationhubstrategy-1.28.15.post1/mypy_boto3_migrationhubstrategy/client.py` & `mypy-boto3-migrationhubstrategy-1.28.16/mypy_boto3_migrationhubstrategy/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_migrationhubstrategy.client import MigrationHubStrategyRecommendationsClient
 
     session = Session()
     client: MigrationHubStrategyRecommendationsClient = session.client("migrationhubstrategy")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     ApplicationComponentCriteriaType,
     ApplicationModeType,
     AppTypeType,
@@ -32,20 +32,17 @@
     GetServerDetailsPaginator,
     ListApplicationComponentsPaginator,
     ListCollectorsPaginator,
     ListImportFileTaskPaginator,
     ListServersPaginator,
 )
 from .type_defs import (
-    ApplicationPreferencesOutputTypeDef,
-    ApplicationPreferencesTypeDef,
-    AssessmentTargetOutputTypeDef,
-    AssessmentTargetTypeDef,
-    DatabasePreferencesOutputTypeDef,
-    DatabasePreferencesTypeDef,
+    ApplicationPreferencesUnionTypeDef,
+    AssessmentTargetUnionTypeDef,
+    DatabasePreferencesUnionTypeDef,
     GetApplicationComponentDetailsResponseTypeDef,
     GetApplicationComponentStrategiesResponseTypeDef,
     GetAssessmentResponseTypeDef,
     GetImportFileTaskResponseTypeDef,
     GetLatestAssessmentIdResponseTypeDef,
     GetPortfolioPreferencesResponseTypeDef,
     GetPortfolioSummaryResponseTypeDef,
@@ -286,35 +283,29 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhubstrategy/client/#list_servers)
         """
 
     def put_portfolio_preferences(
         self,
         *,
         applicationMode: ApplicationModeType = ...,
-        applicationPreferences: Union[
-            ApplicationPreferencesTypeDef, ApplicationPreferencesOutputTypeDef
-        ] = ...,
-        databasePreferences: Union[
-            DatabasePreferencesTypeDef, DatabasePreferencesOutputTypeDef
-        ] = ...,
+        applicationPreferences: ApplicationPreferencesUnionTypeDef = ...,
+        databasePreferences: DatabasePreferencesUnionTypeDef = ...,
         prioritizeBusinessGoals: PrioritizeBusinessGoalsTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Saves the specified migration and modernization preferences.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations.Client.put_portfolio_preferences)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhubstrategy/client/#put_portfolio_preferences)
         """
 
     def start_assessment(
         self,
         *,
-        assessmentTargets: Sequence[
-            Union[AssessmentTargetTypeDef, AssessmentTargetOutputTypeDef]
-        ] = ...,
+        assessmentTargets: Sequence[AssessmentTargetUnionTypeDef] = ...,
         s3bucketForAnalysisData: str = ...,
         s3bucketForReportData: str = ...
     ) -> StartAssessmentResponseTypeDef:
         """
         Starts the assessment of an on-premises environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations.Client.start_assessment)
```

### Comparing `mypy-boto3-migrationhubstrategy-1.28.15.post1/mypy_boto3_migrationhubstrategy/client.pyi` & `mypy-boto3-migrationhubstrategy-1.28.16/mypy_boto3_migrationhubstrategy/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_migrationhubstrategy.client import MigrationHubStrategyRecommendationsClient
 
     session = Session()
     client: MigrationHubStrategyRecommendationsClient = session.client("migrationhubstrategy")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     ApplicationComponentCriteriaType,
     ApplicationModeType,
     AppTypeType,
@@ -32,20 +32,17 @@
     GetServerDetailsPaginator,
     ListApplicationComponentsPaginator,
     ListCollectorsPaginator,
     ListImportFileTaskPaginator,
     ListServersPaginator,
 )
 from .type_defs import (
-    ApplicationPreferencesOutputTypeDef,
-    ApplicationPreferencesTypeDef,
-    AssessmentTargetOutputTypeDef,
-    AssessmentTargetTypeDef,
-    DatabasePreferencesOutputTypeDef,
-    DatabasePreferencesTypeDef,
+    ApplicationPreferencesUnionTypeDef,
+    AssessmentTargetUnionTypeDef,
+    DatabasePreferencesUnionTypeDef,
     GetApplicationComponentDetailsResponseTypeDef,
     GetApplicationComponentStrategiesResponseTypeDef,
     GetAssessmentResponseTypeDef,
     GetImportFileTaskResponseTypeDef,
     GetLatestAssessmentIdResponseTypeDef,
     GetPortfolioPreferencesResponseTypeDef,
     GetPortfolioSummaryResponseTypeDef,
@@ -264,34 +261,28 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations.Client.list_servers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhubstrategy/client/#list_servers)
         """
     def put_portfolio_preferences(
         self,
         *,
         applicationMode: ApplicationModeType = ...,
-        applicationPreferences: Union[
-            ApplicationPreferencesTypeDef, ApplicationPreferencesOutputTypeDef
-        ] = ...,
-        databasePreferences: Union[
-            DatabasePreferencesTypeDef, DatabasePreferencesOutputTypeDef
-        ] = ...,
+        applicationPreferences: ApplicationPreferencesUnionTypeDef = ...,
+        databasePreferences: DatabasePreferencesUnionTypeDef = ...,
         prioritizeBusinessGoals: PrioritizeBusinessGoalsTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Saves the specified migration and modernization preferences.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations.Client.put_portfolio_preferences)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhubstrategy/client/#put_portfolio_preferences)
         """
     def start_assessment(
         self,
         *,
-        assessmentTargets: Sequence[
-            Union[AssessmentTargetTypeDef, AssessmentTargetOutputTypeDef]
-        ] = ...,
+        assessmentTargets: Sequence[AssessmentTargetUnionTypeDef] = ...,
         s3bucketForAnalysisData: str = ...,
         s3bucketForReportData: str = ...
     ) -> StartAssessmentResponseTypeDef:
         """
         Starts the assessment of an on-premises environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations.Client.start_assessment)
```

### Comparing `mypy-boto3-migrationhubstrategy-1.28.15.post1/mypy_boto3_migrationhubstrategy/literals.py` & `mypy-boto3-migrationhubstrategy-1.28.16/mypy_boto3_migrationhubstrategy/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migrationhubstrategy-1.28.15.post1/mypy_boto3_migrationhubstrategy/literals.pyi` & `mypy-boto3-migrationhubstrategy-1.28.16/mypy_boto3_migrationhubstrategy/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migrationhubstrategy-1.28.15.post1/mypy_boto3_migrationhubstrategy/paginator.py` & `mypy-boto3-migrationhubstrategy-1.28.16/mypy_boto3_migrationhubstrategy/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migrationhubstrategy-1.28.15.post1/mypy_boto3_migrationhubstrategy/paginator.pyi` & `mypy-boto3-migrationhubstrategy-1.28.16/mypy_boto3_migrationhubstrategy/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migrationhubstrategy-1.28.15.post1/mypy_boto3_migrationhubstrategy/type_defs.py` & `mypy-boto3-migrationhubstrategy-1.28.16/mypy_boto3_migrationhubstrategy/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhubstrategy/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_migrationhubstrategy.type_defs import AnalysisStatusUnionTypeDef
 
-    data: AnalysisStatusUnionTypeDef = {...}
+    data: AnalysisStatusUnionTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -123,15 +123,15 @@
     "TransformationToolTypeDef",
     "ServerErrorTypeDef",
     "SourceCodeTypeDef",
     "StopAssessmentRequestRequestTypeDef",
     "StrategyOptionTypeDef",
     "AntipatternReportResultTypeDef",
     "AssessmentSummaryTypeDef",
-    "StartAssessmentRequestRequestTypeDef",
+    "AssessmentTargetUnionTypeDef",
     "PrioritizeBusinessGoalsTypeDef",
     "ConfigurationSummaryTypeDef",
     "DatabaseMigrationPreferenceOutputTypeDef",
     "DatabaseMigrationPreferenceTypeDef",
     "GetAssessmentResponseTypeDef",
     "GetImportFileTaskResponseTypeDef",
     "GetLatestAssessmentIdResponseTypeDef",
@@ -153,25 +153,28 @@
     "ManagementPreferenceTypeDef",
     "SystemInfoTypeDef",
     "RecommendationSetTypeDef",
     "UpdateApplicationComponentConfigRequestRequestTypeDef",
     "UpdateServerConfigRequestRequestTypeDef",
     "ResultTypeDef",
     "GetPortfolioSummaryResponseTypeDef",
+    "StartAssessmentRequestRequestTypeDef",
     "CollectorTypeDef",
     "DatabasePreferencesOutputTypeDef",
     "DatabasePreferencesTypeDef",
     "ApplicationPreferencesOutputTypeDef",
     "ApplicationPreferencesTypeDef",
     "ApplicationComponentStrategyTypeDef",
     "ServerDetailTypeDef",
     "ServerStrategyTypeDef",
     "ApplicationComponentDetailTypeDef",
     "ListCollectorsResponseTypeDef",
+    "DatabasePreferencesUnionTypeDef",
     "GetPortfolioPreferencesResponseTypeDef",
+    "ApplicationPreferencesUnionTypeDef",
     "PutPortfolioPreferencesRequestRequestTypeDef",
     "GetApplicationComponentStrategiesResponseTypeDef",
     "GetServerDetailsResponseTypeDef",
     "ListServersResponseTypeDef",
     "GetServerStrategiesResponseTypeDef",
     "GetApplicationComponentDetailsResponseTypeDef",
     "ListApplicationComponentsResponseTypeDef",
@@ -704,26 +707,15 @@
         "listServerStatusSummary": List[ServerStatusSummaryTypeDef],
         "listServerStrategySummary": List[StrategySummaryTypeDef],
         "listServerSummary": List[ServerSummaryTypeDef],
     },
     total=False,
 )
 
-StartAssessmentRequestRequestTypeDef = TypedDict(
-    "StartAssessmentRequestRequestTypeDef",
-    {
-        "assessmentTargets": Sequence[
-            Union[AssessmentTargetTypeDef, AssessmentTargetOutputTypeDef]
-        ],
-        "s3bucketForAnalysisData": str,
-        "s3bucketForReportData": str,
-    },
-    total=False,
-)
-
+AssessmentTargetUnionTypeDef = Union[AssessmentTargetTypeDef, AssessmentTargetOutputTypeDef]
 PrioritizeBusinessGoalsTypeDef = TypedDict(
     "PrioritizeBusinessGoalsTypeDef",
     {
         "businessGoals": BusinessGoalsTypeDef,
     },
     total=False,
 )
@@ -1066,14 +1058,24 @@
     "GetPortfolioSummaryResponseTypeDef",
     {
         "assessmentSummary": AssessmentSummaryTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+StartAssessmentRequestRequestTypeDef = TypedDict(
+    "StartAssessmentRequestRequestTypeDef",
+    {
+        "assessmentTargets": Sequence[AssessmentTargetUnionTypeDef],
+        "s3bucketForAnalysisData": str,
+        "s3bucketForReportData": str,
+    },
+    total=False,
+)
+
 CollectorTypeDef = TypedDict(
     "CollectorTypeDef",
     {
         "collectorHealth": CollectorHealthType,
         "collectorId": str,
         "collectorVersion": str,
         "configurationSummary": ConfigurationSummaryTypeDef,
@@ -1196,25 +1198,31 @@
     {
         "Collectors": List[CollectorTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DatabasePreferencesUnionTypeDef = Union[
+    DatabasePreferencesTypeDef, DatabasePreferencesOutputTypeDef
+]
 GetPortfolioPreferencesResponseTypeDef = TypedDict(
     "GetPortfolioPreferencesResponseTypeDef",
     {
         "applicationMode": ApplicationModeType,
         "applicationPreferences": ApplicationPreferencesOutputTypeDef,
         "databasePreferences": DatabasePreferencesOutputTypeDef,
         "prioritizeBusinessGoals": PrioritizeBusinessGoalsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ApplicationPreferencesUnionTypeDef = Union[
+    ApplicationPreferencesTypeDef, ApplicationPreferencesOutputTypeDef
+]
 PutPortfolioPreferencesRequestRequestTypeDef = TypedDict(
     "PutPortfolioPreferencesRequestRequestTypeDef",
     {
         "applicationMode": ApplicationModeType,
         "applicationPreferences": ApplicationPreferencesTypeDef,
         "databasePreferences": DatabasePreferencesTypeDef,
         "prioritizeBusinessGoals": PrioritizeBusinessGoalsTypeDef,
```

### Comparing `mypy-boto3-migrationhubstrategy-1.28.15.post1/mypy_boto3_migrationhubstrategy/type_defs.pyi` & `mypy-boto3-migrationhubstrategy-1.28.16/mypy_boto3_migrationhubstrategy/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhubstrategy/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_migrationhubstrategy.type_defs import AnalysisStatusUnionTypeDef
 
-    data: AnalysisStatusUnionTypeDef = {...}
+    data: AnalysisStatusUnionTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -122,15 +122,15 @@
     "TransformationToolTypeDef",
     "ServerErrorTypeDef",
     "SourceCodeTypeDef",
     "StopAssessmentRequestRequestTypeDef",
     "StrategyOptionTypeDef",
     "AntipatternReportResultTypeDef",
     "AssessmentSummaryTypeDef",
-    "StartAssessmentRequestRequestTypeDef",
+    "AssessmentTargetUnionTypeDef",
     "PrioritizeBusinessGoalsTypeDef",
     "ConfigurationSummaryTypeDef",
     "DatabaseMigrationPreferenceOutputTypeDef",
     "DatabaseMigrationPreferenceTypeDef",
     "GetAssessmentResponseTypeDef",
     "GetImportFileTaskResponseTypeDef",
     "GetLatestAssessmentIdResponseTypeDef",
@@ -152,25 +152,28 @@
     "ManagementPreferenceTypeDef",
     "SystemInfoTypeDef",
     "RecommendationSetTypeDef",
     "UpdateApplicationComponentConfigRequestRequestTypeDef",
     "UpdateServerConfigRequestRequestTypeDef",
     "ResultTypeDef",
     "GetPortfolioSummaryResponseTypeDef",
+    "StartAssessmentRequestRequestTypeDef",
     "CollectorTypeDef",
     "DatabasePreferencesOutputTypeDef",
     "DatabasePreferencesTypeDef",
     "ApplicationPreferencesOutputTypeDef",
     "ApplicationPreferencesTypeDef",
     "ApplicationComponentStrategyTypeDef",
     "ServerDetailTypeDef",
     "ServerStrategyTypeDef",
     "ApplicationComponentDetailTypeDef",
     "ListCollectorsResponseTypeDef",
+    "DatabasePreferencesUnionTypeDef",
     "GetPortfolioPreferencesResponseTypeDef",
+    "ApplicationPreferencesUnionTypeDef",
     "PutPortfolioPreferencesRequestRequestTypeDef",
     "GetApplicationComponentStrategiesResponseTypeDef",
     "GetServerDetailsResponseTypeDef",
     "ListServersResponseTypeDef",
     "GetServerStrategiesResponseTypeDef",
     "GetApplicationComponentDetailsResponseTypeDef",
     "ListApplicationComponentsResponseTypeDef",
@@ -701,26 +704,15 @@
         "listServerStatusSummary": List[ServerStatusSummaryTypeDef],
         "listServerStrategySummary": List[StrategySummaryTypeDef],
         "listServerSummary": List[ServerSummaryTypeDef],
     },
     total=False,
 )
 
-StartAssessmentRequestRequestTypeDef = TypedDict(
-    "StartAssessmentRequestRequestTypeDef",
-    {
-        "assessmentTargets": Sequence[
-            Union[AssessmentTargetTypeDef, AssessmentTargetOutputTypeDef]
-        ],
-        "s3bucketForAnalysisData": str,
-        "s3bucketForReportData": str,
-    },
-    total=False,
-)
-
+AssessmentTargetUnionTypeDef = Union[AssessmentTargetTypeDef, AssessmentTargetOutputTypeDef]
 PrioritizeBusinessGoalsTypeDef = TypedDict(
     "PrioritizeBusinessGoalsTypeDef",
     {
         "businessGoals": BusinessGoalsTypeDef,
     },
     total=False,
 )
@@ -1055,14 +1047,24 @@
     "GetPortfolioSummaryResponseTypeDef",
     {
         "assessmentSummary": AssessmentSummaryTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+StartAssessmentRequestRequestTypeDef = TypedDict(
+    "StartAssessmentRequestRequestTypeDef",
+    {
+        "assessmentTargets": Sequence[AssessmentTargetUnionTypeDef],
+        "s3bucketForAnalysisData": str,
+        "s3bucketForReportData": str,
+    },
+    total=False,
+)
+
 CollectorTypeDef = TypedDict(
     "CollectorTypeDef",
     {
         "collectorHealth": CollectorHealthType,
         "collectorId": str,
         "collectorVersion": str,
         "configurationSummary": ConfigurationSummaryTypeDef,
@@ -1185,25 +1187,31 @@
     {
         "Collectors": List[CollectorTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DatabasePreferencesUnionTypeDef = Union[
+    DatabasePreferencesTypeDef, DatabasePreferencesOutputTypeDef
+]
 GetPortfolioPreferencesResponseTypeDef = TypedDict(
     "GetPortfolioPreferencesResponseTypeDef",
     {
         "applicationMode": ApplicationModeType,
         "applicationPreferences": ApplicationPreferencesOutputTypeDef,
         "databasePreferences": DatabasePreferencesOutputTypeDef,
         "prioritizeBusinessGoals": PrioritizeBusinessGoalsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ApplicationPreferencesUnionTypeDef = Union[
+    ApplicationPreferencesTypeDef, ApplicationPreferencesOutputTypeDef
+]
 PutPortfolioPreferencesRequestRequestTypeDef = TypedDict(
     "PutPortfolioPreferencesRequestRequestTypeDef",
     {
         "applicationMode": ApplicationModeType,
         "applicationPreferences": ApplicationPreferencesTypeDef,
         "databasePreferences": DatabasePreferencesTypeDef,
         "prioritizeBusinessGoals": PrioritizeBusinessGoalsTypeDef,
```

### Comparing `mypy-boto3-migrationhubstrategy-1.28.15.post1/mypy_boto3_migrationhubstrategy.egg-info/PKG-INFO` & `mypy-boto3-migrationhubstrategy-1.28.16/mypy_boto3_migrationhubstrategy.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-migrationhubstrategy
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.MigrationHubStrategyRecommendations 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.MigrationHubStrategyRecommendations 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhubstrategy/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 migrationhubstrategy type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 migrationhubstrategy type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-migrationhubstrategy.svg?color=blue)](https://pypi.org/project/mypy-boto3-migrationhubstrategy)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhubstrategy/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-migrationhubstrategy)](https://pepy.tech/project/mypy-boto3-migrationhubstrategy)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MigrationHubStrategyRecommendations 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations)
+[boto3.MigrationHubStrategyRecommendations 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations)
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
 [mypy-boto3-migrationhubstrategy docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhubstrategy/).
 
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
@@ -373,20 +373,20 @@
 )
 
 
 def check_value(value: AnalysisTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_migrationhubstrategy.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_migrationhubstrategy.type_defs import (
     AnalysisStatusUnionTypeDef,
     AnalyzerNameUnionTypeDef,
     S3ObjectTypeDef,
     AntipatternSeveritySummaryTypeDef,
@@ -439,15 +439,15 @@
     TransformationToolTypeDef,
     ServerErrorTypeDef,
     SourceCodeTypeDef,
     StopAssessmentRequestRequestTypeDef,
     StrategyOptionTypeDef,
     AntipatternReportResultTypeDef,
     AssessmentSummaryTypeDef,
-    StartAssessmentRequestRequestTypeDef,
+    AssessmentTargetUnionTypeDef,
     PrioritizeBusinessGoalsTypeDef,
     ConfigurationSummaryTypeDef,
     DatabaseMigrationPreferenceOutputTypeDef,
     DatabaseMigrationPreferenceTypeDef,
     GetAssessmentResponseTypeDef,
     GetImportFileTaskResponseTypeDef,
     GetLatestAssessmentIdResponseTypeDef,
@@ -469,36 +469,39 @@
     ManagementPreferenceTypeDef,
     SystemInfoTypeDef,
     RecommendationSetTypeDef,
     UpdateApplicationComponentConfigRequestRequestTypeDef,
     UpdateServerConfigRequestRequestTypeDef,
     ResultTypeDef,
     GetPortfolioSummaryResponseTypeDef,
+    StartAssessmentRequestRequestTypeDef,
     CollectorTypeDef,
     DatabasePreferencesOutputTypeDef,
     DatabasePreferencesTypeDef,
     ApplicationPreferencesOutputTypeDef,
     ApplicationPreferencesTypeDef,
     ApplicationComponentStrategyTypeDef,
     ServerDetailTypeDef,
     ServerStrategyTypeDef,
     ApplicationComponentDetailTypeDef,
     ListCollectorsResponseTypeDef,
+    DatabasePreferencesUnionTypeDef,
     GetPortfolioPreferencesResponseTypeDef,
+    ApplicationPreferencesUnionTypeDef,
     PutPortfolioPreferencesRequestRequestTypeDef,
     GetApplicationComponentStrategiesResponseTypeDef,
     GetServerDetailsResponseTypeDef,
     ListServersResponseTypeDef,
     GetServerStrategiesResponseTypeDef,
     GetApplicationComponentDetailsResponseTypeDef,
     ListApplicationComponentsResponseTypeDef,
 )
 
 
-def get_structure() -> AnalysisStatusUnionTypeDef:
+def get_value() -> AnalysisStatusUnionTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-migrationhubstrategy-1.28.15.post1/mypy_boto3_migrationhubstrategy.egg-info/SOURCES.txt` & `mypy-boto3-migrationhubstrategy-1.28.16/mypy_boto3_migrationhubstrategy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migrationhubstrategy-1.28.15.post1/setup.py` & `mypy-boto3-migrationhubstrategy-1.28.16/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-migrationhubstrategy",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_migrationhubstrategy"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.MigrationHubStrategyRecommendations 1.28.15 service generated"
-        " with mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.MigrationHubStrategyRecommendations 1.28.16 service generated"
+        " with mypy-boto3-builder 7.17.1"
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
-    keywords="boto3 migrationhubstrategy type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 migrationhubstrategy type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_migrationhubstrategy": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhubstrategy/"
```

