# Comparing `tmp/mypy-boto3-databrew-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-databrew-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-databrew-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:54 2023, max compression
+gzip compressed data, was "mypy-boto3-databrew-1.28.16.tar", last modified: Tue Aug  1 11:36:35 2023, max compression
```

## Comparing `mypy-boto3-databrew-1.28.15.post1.tar` & `mypy-boto3-databrew-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:54.829097 mypy-boto3-databrew-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:41:55.000000 mypy-boto3-databrew-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19482 2023-07-29 10:02:54.829097 mypy-boto3-databrew-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17981 2023-07-29 09:41:55.000000 mypy-boto3-databrew-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:54.817097 mypy-boto3-databrew-1.28.15.post1/mypy_boto3_databrew/
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-07-29 09:41:55.000000 mypy-boto3-databrew-1.28.15.post1/mypy_boto3_databrew/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-07-29 09:41:55.000000 mypy-boto3-databrew-1.28.15.post1/mypy_boto3_databrew/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-29 09:41:55.000000 mypy-boto3-databrew-1.28.15.post1/mypy_boto3_databrew/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34421 2023-07-29 09:41:55.000000 mypy-boto3-databrew-1.28.15.post1/mypy_boto3_databrew/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    34362 2023-07-29 09:41:55.000000 mypy-boto3-databrew-1.28.15.post1/mypy_boto3_databrew/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10736 2023-07-29 09:41:56.000000 mypy-boto3-databrew-1.28.15.post1/mypy_boto3_databrew/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10734 2023-07-29 09:41:56.000000 mypy-boto3-databrew-1.28.15.post1/mypy_boto3_databrew/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9045 2023-07-29 09:41:55.000000 mypy-boto3-databrew-1.28.15.post1/mypy_boto3_databrew/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9035 2023-07-29 09:41:55.000000 mypy-boto3-databrew-1.28.15.post1/mypy_boto3_databrew/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:41:55.000000 mypy-boto3-databrew-1.28.15.post1/mypy_boto3_databrew/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    59707 2023-07-29 09:41:59.000000 mypy-boto3-databrew-1.28.15.post1/mypy_boto3_databrew/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    59597 2023-07-29 09:41:58.000000 mypy-boto3-databrew-1.28.15.post1/mypy_boto3_databrew/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:41:55.000000 mypy-boto3-databrew-1.28.15.post1/mypy_boto3_databrew/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:54.829097 mypy-boto3-databrew-1.28.15.post1/mypy_boto3_databrew.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19482 2023-07-29 10:02:54.000000 mypy-boto3-databrew-1.28.15.post1/mypy_boto3_databrew.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-29 10:02:54.000000 mypy-boto3-databrew-1.28.15.post1/mypy_boto3_databrew.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:54.000000 mypy-boto3-databrew-1.28.15.post1/mypy_boto3_databrew.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:54.000000 mypy-boto3-databrew-1.28.15.post1/mypy_boto3_databrew.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:54.000000 mypy-boto3-databrew-1.28.15.post1/mypy_boto3_databrew.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-29 10:02:54.000000 mypy-boto3-databrew-1.28.15.post1/mypy_boto3_databrew.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:54.829097 mypy-boto3-databrew-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-07-29 09:41:55.000000 mypy-boto3-databrew-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:35.280913 mypy-boto3-databrew-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:14:28.000000 mypy-boto3-databrew-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19638 2023-08-01 11:36:35.280913 mypy-boto3-databrew-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18146 2023-08-01 11:14:28.000000 mypy-boto3-databrew-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:35.272913 mypy-boto3-databrew-1.28.16/mypy_boto3_databrew/
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-08-01 11:14:28.000000 mypy-boto3-databrew-1.28.16/mypy_boto3_databrew/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-08-01 11:14:28.000000 mypy-boto3-databrew-1.28.16/mypy_boto3_databrew/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-08-01 11:14:28.000000 mypy-boto3-databrew-1.28.16/mypy_boto3_databrew/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33862 2023-08-01 11:14:28.000000 mypy-boto3-databrew-1.28.16/mypy_boto3_databrew/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33803 2023-08-01 11:14:28.000000 mypy-boto3-databrew-1.28.16/mypy_boto3_databrew/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10736 2023-08-01 11:14:30.000000 mypy-boto3-databrew-1.28.16/mypy_boto3_databrew/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10734 2023-08-01 11:14:29.000000 mypy-boto3-databrew-1.28.16/mypy_boto3_databrew/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9045 2023-08-01 11:14:29.000000 mypy-boto3-databrew-1.28.16/mypy_boto3_databrew/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9035 2023-08-01 11:14:29.000000 mypy-boto3-databrew-1.28.16/mypy_boto3_databrew/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:14:28.000000 mypy-boto3-databrew-1.28.16/mypy_boto3_databrew/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    60193 2023-08-01 11:14:31.000000 mypy-boto3-databrew-1.28.16/mypy_boto3_databrew/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60083 2023-08-01 11:14:30.000000 mypy-boto3-databrew-1.28.16/mypy_boto3_databrew/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:14:28.000000 mypy-boto3-databrew-1.28.16/mypy_boto3_databrew/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:35.280913 mypy-boto3-databrew-1.28.16/mypy_boto3_databrew.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19638 2023-08-01 11:36:35.000000 mypy-boto3-databrew-1.28.16/mypy_boto3_databrew.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-08-01 11:36:35.000000 mypy-boto3-databrew-1.28.16/mypy_boto3_databrew.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:35.000000 mypy-boto3-databrew-1.28.16/mypy_boto3_databrew.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:35.000000 mypy-boto3-databrew-1.28.16/mypy_boto3_databrew.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:35.000000 mypy-boto3-databrew-1.28.16/mypy_boto3_databrew.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-01 11:36:35.000000 mypy-boto3-databrew-1.28.16/mypy_boto3_databrew.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:35.280913 mypy-boto3-databrew-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-08-01 11:14:27.000000 mypy-boto3-databrew-1.28.16/setup.py
```

### Comparing `mypy-boto3-databrew-1.28.15.post1/LICENSE` & `mypy-boto3-databrew-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-databrew-1.28.15.post1/PKG-INFO` & `mypy-boto3-databrew-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-databrew
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.GlueDataBrew 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.GlueDataBrew 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 databrew type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 databrew type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-databrew.svg?color=blue)](https://pypi.org/project/mypy-boto3-databrew)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-databrew)](https://pepy.tech/project/mypy-boto3-databrew)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.GlueDataBrew 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew)
+[boto3.GlueDataBrew 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew)
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
 [mypy-boto3-databrew docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/).
 
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
@@ -353,20 +353,20 @@
 )
 
 
 def check_value(value: AnalyticsModeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_databrew.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_databrew.type_defs import (
     AllowedStatisticsOutputTypeDef,
     AllowedStatisticsTypeDef,
     BatchDeleteRecipeVersionRequestRequestTypeDef,
     RecipeVersionErrorDetailTypeDef,
@@ -489,47 +489,53 @@
     InputTypeDef,
     DatabaseOutputTypeDef,
     DataCatalogOutputTypeDef,
     ListProjectsResponseTypeDef,
     OutputTypeDef,
     PathOptionsOutputTypeDef,
     PathOptionsTypeDef,
+    FormatOptionsUnionTypeDef,
     DescribeRecipeResponseTypeDef,
     RecipeTypeDef,
-    CreateRecipeRequestRequestTypeDef,
+    RecipeStepUnionTypeDef,
     SendProjectSessionActionRequestRequestTypeDef,
-    UpdateRecipeRequestRequestTypeDef,
     DescribeRulesetResponseTypeDef,
-    CreateRulesetRequestRequestTypeDef,
-    UpdateRulesetRequestRequestTypeDef,
+    RuleUnionTypeDef,
     ColumnStatisticsConfigurationOutputTypeDef,
     ColumnStatisticsConfigurationTypeDef,
-    CreateRecipeJobRequestRequestTypeDef,
     JobRunTypeDef,
     JobTypeDef,
-    UpdateRecipeJobRequestRequestTypeDef,
+    UnionTypeDef,
     DatasetTypeDef,
     DescribeDatasetResponseTypeDef,
     CreateDatasetRequestRequestTypeDef,
+    PathOptionsUnionTypeDef,
     UpdateDatasetRequestRequestTypeDef,
     ListRecipeVersionsResponseTypeDef,
     ListRecipesResponseTypeDef,
+    CreateRecipeRequestRequestTypeDef,
+    UpdateRecipeRequestRequestTypeDef,
+    CreateRulesetRequestRequestTypeDef,
+    UpdateRulesetRequestRequestTypeDef,
     ProfileConfigurationOutputTypeDef,
     ProfileConfigurationTypeDef,
     ListJobRunsResponseTypeDef,
     ListJobsResponseTypeDef,
+    CreateRecipeJobRequestRequestTypeDef,
+    UpdateRecipeJobRequestRequestTypeDef,
     ListDatasetsResponseTypeDef,
     DescribeJobResponseTypeDef,
     DescribeJobRunResponseTypeDef,
     CreateProfileJobRequestRequestTypeDef,
+    ProfileConfigurationUnionTypeDef,
     UpdateProfileJobRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AllowedStatisticsOutputTypeDef:
+def get_value() -> AllowedStatisticsOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-databrew-1.28.15.post1/README.md` & `mypy-boto3-databrew-1.28.16/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-databrew.svg?color=blue)](https://pypi.org/project/mypy-boto3-databrew)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-databrew)](https://pepy.tech/project/mypy-boto3-databrew)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.GlueDataBrew 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew)
+[boto3.GlueDataBrew 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew)
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
 [mypy-boto3-databrew docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/).
 
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
@@ -321,20 +321,20 @@
 )
 
 
 def check_value(value: AnalyticsModeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_databrew.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_databrew.type_defs import (
     AllowedStatisticsOutputTypeDef,
     AllowedStatisticsTypeDef,
     BatchDeleteRecipeVersionRequestRequestTypeDef,
     RecipeVersionErrorDetailTypeDef,
@@ -457,47 +457,53 @@
     InputTypeDef,
     DatabaseOutputTypeDef,
     DataCatalogOutputTypeDef,
     ListProjectsResponseTypeDef,
     OutputTypeDef,
     PathOptionsOutputTypeDef,
     PathOptionsTypeDef,
+    FormatOptionsUnionTypeDef,
     DescribeRecipeResponseTypeDef,
     RecipeTypeDef,
-    CreateRecipeRequestRequestTypeDef,
+    RecipeStepUnionTypeDef,
     SendProjectSessionActionRequestRequestTypeDef,
-    UpdateRecipeRequestRequestTypeDef,
     DescribeRulesetResponseTypeDef,
-    CreateRulesetRequestRequestTypeDef,
-    UpdateRulesetRequestRequestTypeDef,
+    RuleUnionTypeDef,
     ColumnStatisticsConfigurationOutputTypeDef,
     ColumnStatisticsConfigurationTypeDef,
-    CreateRecipeJobRequestRequestTypeDef,
     JobRunTypeDef,
     JobTypeDef,
-    UpdateRecipeJobRequestRequestTypeDef,
+    UnionTypeDef,
     DatasetTypeDef,
     DescribeDatasetResponseTypeDef,
     CreateDatasetRequestRequestTypeDef,
+    PathOptionsUnionTypeDef,
     UpdateDatasetRequestRequestTypeDef,
     ListRecipeVersionsResponseTypeDef,
     ListRecipesResponseTypeDef,
+    CreateRecipeRequestRequestTypeDef,
+    UpdateRecipeRequestRequestTypeDef,
+    CreateRulesetRequestRequestTypeDef,
+    UpdateRulesetRequestRequestTypeDef,
     ProfileConfigurationOutputTypeDef,
     ProfileConfigurationTypeDef,
     ListJobRunsResponseTypeDef,
     ListJobsResponseTypeDef,
+    CreateRecipeJobRequestRequestTypeDef,
+    UpdateRecipeJobRequestRequestTypeDef,
     ListDatasetsResponseTypeDef,
     DescribeJobResponseTypeDef,
     DescribeJobRunResponseTypeDef,
     CreateProfileJobRequestRequestTypeDef,
+    ProfileConfigurationUnionTypeDef,
     UpdateProfileJobRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AllowedStatisticsOutputTypeDef:
+def get_value() -> AllowedStatisticsOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-databrew-1.28.15.post1/mypy_boto3_databrew/__init__.py` & `mypy-boto3-databrew-1.28.16/mypy_boto3_databrew/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-databrew-1.28.15.post1/mypy_boto3_databrew/__init__.pyi` & `mypy-boto3-databrew-1.28.16/mypy_boto3_databrew/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-databrew-1.28.15.post1/mypy_boto3_databrew/__main__.py` & `mypy-boto3-databrew-1.28.16/mypy_boto3_databrew/__main__.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.GlueDataBrew 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.GlueDataBrew 1.28.16\nVersion:         1.28.16\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew\nOther"
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

### Comparing `mypy-boto3-databrew-1.28.15.post1/mypy_boto3_databrew/client.py` & `mypy-boto3-databrew-1.28.16/mypy_boto3_databrew/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_databrew.client import GlueDataBrewClient
 
     session = Session()
     client: GlueDataBrewClient = session.client("databrew")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import EncryptionModeType, InputFormatType, LogSubscriptionType
 from .paginator import (
     ListDatasetsPaginator,
     ListJobRunsPaginator,
@@ -49,44 +49,39 @@
     DescribeDatasetResponseTypeDef,
     DescribeJobResponseTypeDef,
     DescribeJobRunResponseTypeDef,
     DescribeProjectResponseTypeDef,
     DescribeRecipeResponseTypeDef,
     DescribeRulesetResponseTypeDef,
     DescribeScheduleResponseTypeDef,
-    FormatOptionsOutputTypeDef,
-    FormatOptionsTypeDef,
+    FormatOptionsUnionTypeDef,
     InputTypeDef,
     JobSampleTypeDef,
     ListDatasetsResponseTypeDef,
     ListJobRunsResponseTypeDef,
     ListJobsResponseTypeDef,
     ListProjectsResponseTypeDef,
     ListRecipesResponseTypeDef,
     ListRecipeVersionsResponseTypeDef,
     ListRulesetsResponseTypeDef,
     ListSchedulesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    OutputTypeDef,
-    PathOptionsOutputTypeDef,
-    PathOptionsTypeDef,
-    ProfileConfigurationOutputTypeDef,
-    ProfileConfigurationTypeDef,
+    PathOptionsUnionTypeDef,
+    ProfileConfigurationUnionTypeDef,
     PublishRecipeResponseTypeDef,
     RecipeReferenceTypeDef,
-    RecipeStepOutputTypeDef,
-    RecipeStepTypeDef,
-    RuleOutputTypeDef,
-    RuleTypeDef,
+    RecipeStepUnionTypeDef,
+    RuleUnionTypeDef,
     S3LocationTypeDef,
     SampleTypeDef,
     SendProjectSessionActionResponseTypeDef,
     StartJobRunResponseTypeDef,
     StartProjectSessionResponseTypeDef,
     StopJobRunResponseTypeDef,
+    UnionTypeDef,
     UpdateDatasetResponseTypeDef,
     UpdateProfileJobResponseTypeDef,
     UpdateProjectResponseTypeDef,
     UpdateRecipeJobResponseTypeDef,
     UpdateRecipeResponseTypeDef,
     UpdateRulesetResponseTypeDef,
     UpdateScheduleResponseTypeDef,
@@ -166,16 +161,16 @@
 
     def create_dataset(
         self,
         *,
         Name: str,
         Input: InputTypeDef,
         Format: InputFormatType = ...,
-        FormatOptions: Union[FormatOptionsTypeDef, FormatOptionsOutputTypeDef] = ...,
-        PathOptions: Union[PathOptionsTypeDef, PathOptionsOutputTypeDef] = ...,
+        FormatOptions: FormatOptionsUnionTypeDef = ...,
+        PathOptions: PathOptionsUnionTypeDef = ...,
         Tags: Mapping[str, str] = ...
     ) -> CreateDatasetResponseTypeDef:
         """
         Creates a new DataBrew dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Client.create_dataset)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/client/#create_dataset)
@@ -189,15 +184,15 @@
         OutputLocation: S3LocationTypeDef,
         RoleArn: str,
         EncryptionKeyArn: str = ...,
         EncryptionMode: EncryptionModeType = ...,
         LogSubscription: LogSubscriptionType = ...,
         MaxCapacity: int = ...,
         MaxRetries: int = ...,
-        Configuration: Union[ProfileConfigurationTypeDef, ProfileConfigurationOutputTypeDef] = ...,
+        Configuration: ProfileConfigurationUnionTypeDef = ...,
         ValidationConfigurations: Sequence[ValidationConfigurationTypeDef] = ...,
         Tags: Mapping[str, str] = ...,
         Timeout: int = ...,
         JobSample: JobSampleTypeDef = ...
     ) -> CreateProfileJobResponseTypeDef:
         """
         Creates a new job to analyze a dataset and create its data profile.
@@ -223,15 +218,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/client/#create_project)
         """
 
     def create_recipe(
         self,
         *,
         Name: str,
-        Steps: Sequence[Union[RecipeStepTypeDef, RecipeStepOutputTypeDef]],
+        Steps: Sequence[RecipeStepUnionTypeDef],
         Description: str = ...,
         Tags: Mapping[str, str] = ...
     ) -> CreateRecipeResponseTypeDef:
         """
         Creates a new DataBrew recipe.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Client.create_recipe)
@@ -245,15 +240,15 @@
         RoleArn: str,
         DatasetName: str = ...,
         EncryptionKeyArn: str = ...,
         EncryptionMode: EncryptionModeType = ...,
         LogSubscription: LogSubscriptionType = ...,
         MaxCapacity: int = ...,
         MaxRetries: int = ...,
-        Outputs: Sequence[Union[OutputTypeDef, OutputTypeDef]] = ...,
+        Outputs: Sequence[UnionTypeDef] = ...,
         DataCatalogOutputs: Sequence[DataCatalogOutputTypeDef] = ...,
         DatabaseOutputs: Sequence[DatabaseOutputTypeDef] = ...,
         ProjectName: str = ...,
         RecipeReference: RecipeReferenceTypeDef = ...,
         Tags: Mapping[str, str] = ...,
         Timeout: int = ...
     ) -> CreateRecipeJobResponseTypeDef:
@@ -267,15 +262,15 @@
         """
 
     def create_ruleset(
         self,
         *,
         Name: str,
         TargetArn: str,
-        Rules: Sequence[Union[RuleTypeDef, RuleOutputTypeDef]],
+        Rules: Sequence[RuleUnionTypeDef],
         Description: str = ...,
         Tags: Mapping[str, str] = ...
     ) -> CreateRulesetResponseTypeDef:
         """
         Creates a new ruleset that can be used in a profile job to validate the data
         quality of a dataset.
 
@@ -524,15 +519,15 @@
         """
 
     def send_project_session_action(
         self,
         *,
         Name: str,
         Preview: bool = ...,
-        RecipeStep: Union[RecipeStepTypeDef, RecipeStepOutputTypeDef] = ...,
+        RecipeStep: RecipeStepUnionTypeDef = ...,
         StepIndex: int = ...,
         ClientSessionId: str = ...,
         ViewFrame: ViewFrameTypeDef = ...
     ) -> SendProjectSessionActionResponseTypeDef:
         """
         Performs a recipe step within an interactive DataBrew session that's currently
         open.
@@ -587,31 +582,31 @@
 
     def update_dataset(
         self,
         *,
         Name: str,
         Input: InputTypeDef,
         Format: InputFormatType = ...,
-        FormatOptions: Union[FormatOptionsTypeDef, FormatOptionsOutputTypeDef] = ...,
-        PathOptions: Union[PathOptionsTypeDef, PathOptionsOutputTypeDef] = ...
+        FormatOptions: FormatOptionsUnionTypeDef = ...,
+        PathOptions: PathOptionsUnionTypeDef = ...
     ) -> UpdateDatasetResponseTypeDef:
         """
         Modifies the definition of an existing DataBrew dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Client.update_dataset)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/client/#update_dataset)
         """
 
     def update_profile_job(
         self,
         *,
         Name: str,
         OutputLocation: S3LocationTypeDef,
         RoleArn: str,
-        Configuration: Union[ProfileConfigurationTypeDef, ProfileConfigurationOutputTypeDef] = ...,
+        Configuration: ProfileConfigurationUnionTypeDef = ...,
         EncryptionKeyArn: str = ...,
         EncryptionMode: EncryptionModeType = ...,
         LogSubscription: LogSubscriptionType = ...,
         MaxCapacity: int = ...,
         MaxRetries: int = ...,
         ValidationConfigurations: Sequence[ValidationConfigurationTypeDef] = ...,
         Timeout: int = ...,
@@ -631,19 +626,15 @@
         Modifies the definition of an existing DataBrew project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Client.update_project)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/client/#update_project)
         """
 
     def update_recipe(
-        self,
-        *,
-        Name: str,
-        Description: str = ...,
-        Steps: Sequence[Union[RecipeStepTypeDef, RecipeStepOutputTypeDef]] = ...
+        self, *, Name: str, Description: str = ..., Steps: Sequence[RecipeStepUnionTypeDef] = ...
     ) -> UpdateRecipeResponseTypeDef:
         """
         Modifies the definition of the `LATEST_WORKING` version of a DataBrew recipe.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Client.update_recipe)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/client/#update_recipe)
         """
@@ -654,32 +645,28 @@
         Name: str,
         RoleArn: str,
         EncryptionKeyArn: str = ...,
         EncryptionMode: EncryptionModeType = ...,
         LogSubscription: LogSubscriptionType = ...,
         MaxCapacity: int = ...,
         MaxRetries: int = ...,
-        Outputs: Sequence[Union[OutputTypeDef, OutputTypeDef]] = ...,
+        Outputs: Sequence[UnionTypeDef] = ...,
         DataCatalogOutputs: Sequence[DataCatalogOutputTypeDef] = ...,
         DatabaseOutputs: Sequence[DatabaseOutputTypeDef] = ...,
         Timeout: int = ...
     ) -> UpdateRecipeJobResponseTypeDef:
         """
         Modifies the definition of an existing DataBrew recipe job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Client.update_recipe_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/client/#update_recipe_job)
         """
 
     def update_ruleset(
-        self,
-        *,
-        Name: str,
-        Rules: Sequence[Union[RuleTypeDef, RuleOutputTypeDef]],
-        Description: str = ...
+        self, *, Name: str, Rules: Sequence[RuleUnionTypeDef], Description: str = ...
     ) -> UpdateRulesetResponseTypeDef:
         """
         Updates specified ruleset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Client.update_ruleset)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/client/#update_ruleset)
         """
```

### Comparing `mypy-boto3-databrew-1.28.15.post1/mypy_boto3_databrew/client.pyi` & `mypy-boto3-databrew-1.28.16/mypy_boto3_databrew/client.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_databrew.client import GlueDataBrewClient
 
     session = Session()
     client: GlueDataBrewClient = session.client("databrew")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import EncryptionModeType, InputFormatType, LogSubscriptionType
 from .paginator import (
     ListDatasetsPaginator,
     ListJobRunsPaginator,
@@ -49,44 +49,39 @@
     DescribeDatasetResponseTypeDef,
     DescribeJobResponseTypeDef,
     DescribeJobRunResponseTypeDef,
     DescribeProjectResponseTypeDef,
     DescribeRecipeResponseTypeDef,
     DescribeRulesetResponseTypeDef,
     DescribeScheduleResponseTypeDef,
-    FormatOptionsOutputTypeDef,
-    FormatOptionsTypeDef,
+    FormatOptionsUnionTypeDef,
     InputTypeDef,
     JobSampleTypeDef,
     ListDatasetsResponseTypeDef,
     ListJobRunsResponseTypeDef,
     ListJobsResponseTypeDef,
     ListProjectsResponseTypeDef,
     ListRecipesResponseTypeDef,
     ListRecipeVersionsResponseTypeDef,
     ListRulesetsResponseTypeDef,
     ListSchedulesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    OutputTypeDef,
-    PathOptionsOutputTypeDef,
-    PathOptionsTypeDef,
-    ProfileConfigurationOutputTypeDef,
-    ProfileConfigurationTypeDef,
+    PathOptionsUnionTypeDef,
+    ProfileConfigurationUnionTypeDef,
     PublishRecipeResponseTypeDef,
     RecipeReferenceTypeDef,
-    RecipeStepOutputTypeDef,
-    RecipeStepTypeDef,
-    RuleOutputTypeDef,
-    RuleTypeDef,
+    RecipeStepUnionTypeDef,
+    RuleUnionTypeDef,
     S3LocationTypeDef,
     SampleTypeDef,
     SendProjectSessionActionResponseTypeDef,
     StartJobRunResponseTypeDef,
     StartProjectSessionResponseTypeDef,
     StopJobRunResponseTypeDef,
+    UnionTypeDef,
     UpdateDatasetResponseTypeDef,
     UpdateProfileJobResponseTypeDef,
     UpdateProjectResponseTypeDef,
     UpdateRecipeJobResponseTypeDef,
     UpdateRecipeResponseTypeDef,
     UpdateRulesetResponseTypeDef,
     UpdateScheduleResponseTypeDef,
@@ -158,16 +153,16 @@
         """
     def create_dataset(
         self,
         *,
         Name: str,
         Input: InputTypeDef,
         Format: InputFormatType = ...,
-        FormatOptions: Union[FormatOptionsTypeDef, FormatOptionsOutputTypeDef] = ...,
-        PathOptions: Union[PathOptionsTypeDef, PathOptionsOutputTypeDef] = ...,
+        FormatOptions: FormatOptionsUnionTypeDef = ...,
+        PathOptions: PathOptionsUnionTypeDef = ...,
         Tags: Mapping[str, str] = ...
     ) -> CreateDatasetResponseTypeDef:
         """
         Creates a new DataBrew dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Client.create_dataset)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/client/#create_dataset)
@@ -180,15 +175,15 @@
         OutputLocation: S3LocationTypeDef,
         RoleArn: str,
         EncryptionKeyArn: str = ...,
         EncryptionMode: EncryptionModeType = ...,
         LogSubscription: LogSubscriptionType = ...,
         MaxCapacity: int = ...,
         MaxRetries: int = ...,
-        Configuration: Union[ProfileConfigurationTypeDef, ProfileConfigurationOutputTypeDef] = ...,
+        Configuration: ProfileConfigurationUnionTypeDef = ...,
         ValidationConfigurations: Sequence[ValidationConfigurationTypeDef] = ...,
         Tags: Mapping[str, str] = ...,
         Timeout: int = ...,
         JobSample: JobSampleTypeDef = ...
     ) -> CreateProfileJobResponseTypeDef:
         """
         Creates a new job to analyze a dataset and create its data profile.
@@ -212,15 +207,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Client.create_project)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/client/#create_project)
         """
     def create_recipe(
         self,
         *,
         Name: str,
-        Steps: Sequence[Union[RecipeStepTypeDef, RecipeStepOutputTypeDef]],
+        Steps: Sequence[RecipeStepUnionTypeDef],
         Description: str = ...,
         Tags: Mapping[str, str] = ...
     ) -> CreateRecipeResponseTypeDef:
         """
         Creates a new DataBrew recipe.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Client.create_recipe)
@@ -233,15 +228,15 @@
         RoleArn: str,
         DatasetName: str = ...,
         EncryptionKeyArn: str = ...,
         EncryptionMode: EncryptionModeType = ...,
         LogSubscription: LogSubscriptionType = ...,
         MaxCapacity: int = ...,
         MaxRetries: int = ...,
-        Outputs: Sequence[Union[OutputTypeDef, OutputTypeDef]] = ...,
+        Outputs: Sequence[UnionTypeDef] = ...,
         DataCatalogOutputs: Sequence[DataCatalogOutputTypeDef] = ...,
         DatabaseOutputs: Sequence[DatabaseOutputTypeDef] = ...,
         ProjectName: str = ...,
         RecipeReference: RecipeReferenceTypeDef = ...,
         Tags: Mapping[str, str] = ...,
         Timeout: int = ...
     ) -> CreateRecipeJobResponseTypeDef:
@@ -254,15 +249,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/client/#create_recipe_job)
         """
     def create_ruleset(
         self,
         *,
         Name: str,
         TargetArn: str,
-        Rules: Sequence[Union[RuleTypeDef, RuleOutputTypeDef]],
+        Rules: Sequence[RuleUnionTypeDef],
         Description: str = ...,
         Tags: Mapping[str, str] = ...
     ) -> CreateRulesetResponseTypeDef:
         """
         Creates a new ruleset that can be used in a profile job to validate the data
         quality of a dataset.
 
@@ -485,15 +480,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/client/#publish_recipe)
         """
     def send_project_session_action(
         self,
         *,
         Name: str,
         Preview: bool = ...,
-        RecipeStep: Union[RecipeStepTypeDef, RecipeStepOutputTypeDef] = ...,
+        RecipeStep: RecipeStepUnionTypeDef = ...,
         StepIndex: int = ...,
         ClientSessionId: str = ...,
         ViewFrame: ViewFrameTypeDef = ...
     ) -> SendProjectSessionActionResponseTypeDef:
         """
         Performs a recipe step within an interactive DataBrew session that's currently
         open.
@@ -542,30 +537,30 @@
         """
     def update_dataset(
         self,
         *,
         Name: str,
         Input: InputTypeDef,
         Format: InputFormatType = ...,
-        FormatOptions: Union[FormatOptionsTypeDef, FormatOptionsOutputTypeDef] = ...,
-        PathOptions: Union[PathOptionsTypeDef, PathOptionsOutputTypeDef] = ...
+        FormatOptions: FormatOptionsUnionTypeDef = ...,
+        PathOptions: PathOptionsUnionTypeDef = ...
     ) -> UpdateDatasetResponseTypeDef:
         """
         Modifies the definition of an existing DataBrew dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Client.update_dataset)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/client/#update_dataset)
         """
     def update_profile_job(
         self,
         *,
         Name: str,
         OutputLocation: S3LocationTypeDef,
         RoleArn: str,
-        Configuration: Union[ProfileConfigurationTypeDef, ProfileConfigurationOutputTypeDef] = ...,
+        Configuration: ProfileConfigurationUnionTypeDef = ...,
         EncryptionKeyArn: str = ...,
         EncryptionMode: EncryptionModeType = ...,
         LogSubscription: LogSubscriptionType = ...,
         MaxCapacity: int = ...,
         MaxRetries: int = ...,
         ValidationConfigurations: Sequence[ValidationConfigurationTypeDef] = ...,
         Timeout: int = ...,
@@ -583,19 +578,15 @@
         """
         Modifies the definition of an existing DataBrew project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Client.update_project)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/client/#update_project)
         """
     def update_recipe(
-        self,
-        *,
-        Name: str,
-        Description: str = ...,
-        Steps: Sequence[Union[RecipeStepTypeDef, RecipeStepOutputTypeDef]] = ...
+        self, *, Name: str, Description: str = ..., Steps: Sequence[RecipeStepUnionTypeDef] = ...
     ) -> UpdateRecipeResponseTypeDef:
         """
         Modifies the definition of the `LATEST_WORKING` version of a DataBrew recipe.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Client.update_recipe)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/client/#update_recipe)
         """
@@ -605,31 +596,27 @@
         Name: str,
         RoleArn: str,
         EncryptionKeyArn: str = ...,
         EncryptionMode: EncryptionModeType = ...,
         LogSubscription: LogSubscriptionType = ...,
         MaxCapacity: int = ...,
         MaxRetries: int = ...,
-        Outputs: Sequence[Union[OutputTypeDef, OutputTypeDef]] = ...,
+        Outputs: Sequence[UnionTypeDef] = ...,
         DataCatalogOutputs: Sequence[DataCatalogOutputTypeDef] = ...,
         DatabaseOutputs: Sequence[DatabaseOutputTypeDef] = ...,
         Timeout: int = ...
     ) -> UpdateRecipeJobResponseTypeDef:
         """
         Modifies the definition of an existing DataBrew recipe job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Client.update_recipe_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/client/#update_recipe_job)
         """
     def update_ruleset(
-        self,
-        *,
-        Name: str,
-        Rules: Sequence[Union[RuleTypeDef, RuleOutputTypeDef]],
-        Description: str = ...
+        self, *, Name: str, Rules: Sequence[RuleUnionTypeDef], Description: str = ...
     ) -> UpdateRulesetResponseTypeDef:
         """
         Updates specified ruleset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Client.update_ruleset)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/client/#update_ruleset)
         """
```

### Comparing `mypy-boto3-databrew-1.28.15.post1/mypy_boto3_databrew/literals.py` & `mypy-boto3-databrew-1.28.16/mypy_boto3_databrew/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-databrew-1.28.15.post1/mypy_boto3_databrew/literals.pyi` & `mypy-boto3-databrew-1.28.16/mypy_boto3_databrew/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-databrew-1.28.15.post1/mypy_boto3_databrew/paginator.py` & `mypy-boto3-databrew-1.28.16/mypy_boto3_databrew/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-databrew-1.28.15.post1/mypy_boto3_databrew/paginator.pyi` & `mypy-boto3-databrew-1.28.16/mypy_boto3_databrew/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-databrew-1.28.15.post1/mypy_boto3_databrew/type_defs.py` & `mypy-boto3-databrew-1.28.16/mypy_boto3_databrew/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_databrew.type_defs import AllowedStatisticsOutputTypeDef
 
-    data: AllowedStatisticsOutputTypeDef = {...}
+    data: AllowedStatisticsOutputTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -39,15 +39,14 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AllowedStatisticsOutputTypeDef",
     "AllowedStatisticsTypeDef",
     "BatchDeleteRecipeVersionRequestRequestTypeDef",
     "RecipeVersionErrorDetailTypeDef",
     "ResponseMetadataTypeDef",
     "ColumnSelectorTypeDef",
@@ -168,42 +167,48 @@
     "InputTypeDef",
     "DatabaseOutputTypeDef",
     "DataCatalogOutputTypeDef",
     "ListProjectsResponseTypeDef",
     "OutputTypeDef",
     "PathOptionsOutputTypeDef",
     "PathOptionsTypeDef",
+    "FormatOptionsUnionTypeDef",
     "DescribeRecipeResponseTypeDef",
     "RecipeTypeDef",
-    "CreateRecipeRequestRequestTypeDef",
+    "RecipeStepUnionTypeDef",
     "SendProjectSessionActionRequestRequestTypeDef",
-    "UpdateRecipeRequestRequestTypeDef",
     "DescribeRulesetResponseTypeDef",
-    "CreateRulesetRequestRequestTypeDef",
-    "UpdateRulesetRequestRequestTypeDef",
+    "RuleUnionTypeDef",
     "ColumnStatisticsConfigurationOutputTypeDef",
     "ColumnStatisticsConfigurationTypeDef",
-    "CreateRecipeJobRequestRequestTypeDef",
     "JobRunTypeDef",
     "JobTypeDef",
-    "UpdateRecipeJobRequestRequestTypeDef",
+    "UnionTypeDef",
     "DatasetTypeDef",
     "DescribeDatasetResponseTypeDef",
     "CreateDatasetRequestRequestTypeDef",
+    "PathOptionsUnionTypeDef",
     "UpdateDatasetRequestRequestTypeDef",
     "ListRecipeVersionsResponseTypeDef",
     "ListRecipesResponseTypeDef",
+    "CreateRecipeRequestRequestTypeDef",
+    "UpdateRecipeRequestRequestTypeDef",
+    "CreateRulesetRequestRequestTypeDef",
+    "UpdateRulesetRequestRequestTypeDef",
     "ProfileConfigurationOutputTypeDef",
     "ProfileConfigurationTypeDef",
     "ListJobRunsResponseTypeDef",
     "ListJobsResponseTypeDef",
+    "CreateRecipeJobRequestRequestTypeDef",
+    "UpdateRecipeJobRequestRequestTypeDef",
     "ListDatasetsResponseTypeDef",
     "DescribeJobResponseTypeDef",
     "DescribeJobRunResponseTypeDef",
     "CreateProfileJobRequestRequestTypeDef",
+    "ProfileConfigurationUnionTypeDef",
     "UpdateProfileJobRequestRequestTypeDef",
 )
 
 AllowedStatisticsOutputTypeDef = TypedDict(
     "AllowedStatisticsOutputTypeDef",
     {
         "Statistics": List[str],
@@ -266,21 +271,19 @@
     "_OptionalConditionExpressionTypeDef",
     {
         "Value": str,
     },
     total=False,
 )
 
-
 class ConditionExpressionTypeDef(
     _RequiredConditionExpressionTypeDef, _OptionalConditionExpressionTypeDef
 ):
     pass
 
-
 JobSampleTypeDef = TypedDict(
     "JobSampleTypeDef",
     {
         "Mode": SampleModeType,
         "Size": int,
     },
     total=False,
@@ -297,78 +300,70 @@
     {
         "Key": str,
         "BucketOwner": str,
     },
     total=False,
 )
 
-
 class S3LocationTypeDef(_RequiredS3LocationTypeDef, _OptionalS3LocationTypeDef):
     pass
 
-
 _RequiredValidationConfigurationTypeDef = TypedDict(
     "_RequiredValidationConfigurationTypeDef",
     {
         "RulesetArn": str,
     },
 )
 _OptionalValidationConfigurationTypeDef = TypedDict(
     "_OptionalValidationConfigurationTypeDef",
     {
         "ValidationMode": Literal["CHECK_ALL"],
     },
     total=False,
 )
 
-
 class ValidationConfigurationTypeDef(
     _RequiredValidationConfigurationTypeDef, _OptionalValidationConfigurationTypeDef
 ):
     pass
 
-
 _RequiredSampleTypeDef = TypedDict(
     "_RequiredSampleTypeDef",
     {
         "Type": SampleTypeType,
     },
 )
 _OptionalSampleTypeDef = TypedDict(
     "_OptionalSampleTypeDef",
     {
         "Size": int,
     },
     total=False,
 )
 
-
 class SampleTypeDef(_RequiredSampleTypeDef, _OptionalSampleTypeDef):
     pass
 
-
 _RequiredRecipeReferenceTypeDef = TypedDict(
     "_RequiredRecipeReferenceTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalRecipeReferenceTypeDef = TypedDict(
     "_OptionalRecipeReferenceTypeDef",
     {
         "RecipeVersion": str,
     },
     total=False,
 )
 
-
 class RecipeReferenceTypeDef(_RequiredRecipeReferenceTypeDef, _OptionalRecipeReferenceTypeDef):
     pass
 
-
 _RequiredCreateScheduleRequestRequestTypeDef = TypedDict(
     "_RequiredCreateScheduleRequestRequestTypeDef",
     {
         "CronExpression": str,
         "Name": str,
     },
 )
@@ -377,21 +372,19 @@
     {
         "JobNames": Sequence[str],
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateScheduleRequestRequestTypeDef(
     _RequiredCreateScheduleRequestRequestTypeDef, _OptionalCreateScheduleRequestRequestTypeDef
 ):
     pass
 
-
 CsvOptionsTypeDef = TypedDict(
     "CsvOptionsTypeDef",
     {
         "Delimiter": str,
         "HeaderRow": bool,
     },
     total=False,
@@ -416,19 +409,17 @@
     {
         "TimezoneOffset": str,
         "LocaleCode": str,
     },
     total=False,
 )
 
-
 class DatetimeOptionsTypeDef(_RequiredDatetimeOptionsTypeDef, _OptionalDatetimeOptionsTypeDef):
     pass
 
-
 FilterExpressionOutputTypeDef = TypedDict(
     "FilterExpressionOutputTypeDef",
     {
         "Expression": str,
         "ValuesMap": Dict[str, str],
     },
 )
@@ -523,21 +514,19 @@
     "_OptionalDescribeRecipeRequestRequestTypeDef",
     {
         "RecipeVersion": str,
     },
     total=False,
 )
 
-
 class DescribeRecipeRequestRequestTypeDef(
     _RequiredDescribeRecipeRequestRequestTypeDef, _OptionalDescribeRecipeRequestRequestTypeDef
 ):
     pass
 
-
 DescribeRulesetRequestRequestTypeDef = TypedDict(
     "DescribeRulesetRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -579,19 +568,17 @@
     {
         "OrderedBy": Literal["LAST_MODIFIED_DATE"],
         "Order": OrderType,
     },
     total=False,
 )
 
-
 class FilesLimitTypeDef(_RequiredFilesLimitTypeDef, _OptionalFilesLimitTypeDef):
     pass
 
-
 JsonOptionsTypeDef = TypedDict(
     "JsonOptionsTypeDef",
     {
         "MultiLine": bool,
     },
     total=False,
 )
@@ -634,21 +621,19 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListJobRunsRequestRequestTypeDef(
     _RequiredListJobRunsRequestRequestTypeDef, _OptionalListJobRunsRequestRequestTypeDef
 ):
     pass
 
-
 ListJobsRequestRequestTypeDef = TypedDict(
     "ListJobsRequestRequestTypeDef",
     {
         "DatasetName": str,
         "MaxResults": int,
         "NextToken": str,
         "ProjectName": str,
@@ -676,22 +661,20 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListRecipeVersionsRequestRequestTypeDef(
     _RequiredListRecipeVersionsRequestRequestTypeDef,
     _OptionalListRecipeVersionsRequestRequestTypeDef,
 ):
     pass
 
-
 ListRecipesRequestRequestTypeDef = TypedDict(
     "ListRecipesRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "RecipeVersion": str,
     },
@@ -727,19 +710,17 @@
         "ResourceArn": str,
         "RuleCount": int,
         "Tags": Dict[str, str],
     },
     total=False,
 )
 
-
 class RulesetItemTypeDef(_RequiredRulesetItemTypeDef, _OptionalRulesetItemTypeDef):
     pass
 
-
 ListSchedulesRequestRequestTypeDef = TypedDict(
     "ListSchedulesRequestRequestTypeDef",
     {
         "JobName": str,
         "MaxResults": int,
         "NextToken": str,
     },
@@ -764,19 +745,17 @@
         "ResourceArn": str,
         "CronExpression": str,
         "Tags": Dict[str, str],
     },
     total=False,
 )
 
-
 class ScheduleTypeDef(_RequiredScheduleTypeDef, _OptionalScheduleTypeDef):
     pass
 
-
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
@@ -790,61 +769,55 @@
     "_OptionalPublishRecipeRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
-
 class PublishRecipeRequestRequestTypeDef(
     _RequiredPublishRecipeRequestRequestTypeDef, _OptionalPublishRecipeRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredRecipeActionOutputTypeDef = TypedDict(
     "_RequiredRecipeActionOutputTypeDef",
     {
         "Operation": str,
     },
 )
 _OptionalRecipeActionOutputTypeDef = TypedDict(
     "_OptionalRecipeActionOutputTypeDef",
     {
         "Parameters": Dict[str, str],
     },
     total=False,
 )
 
-
 class RecipeActionOutputTypeDef(
     _RequiredRecipeActionOutputTypeDef, _OptionalRecipeActionOutputTypeDef
 ):
     pass
 
-
 _RequiredRecipeActionTypeDef = TypedDict(
     "_RequiredRecipeActionTypeDef",
     {
         "Operation": str,
     },
 )
 _OptionalRecipeActionTypeDef = TypedDict(
     "_OptionalRecipeActionTypeDef",
     {
         "Parameters": Mapping[str, str],
     },
     total=False,
 )
 
-
 class RecipeActionTypeDef(_RequiredRecipeActionTypeDef, _OptionalRecipeActionTypeDef):
     pass
 
-
 _RequiredThresholdTypeDef = TypedDict(
     "_RequiredThresholdTypeDef",
     {
         "Value": float,
     },
 )
 _OptionalThresholdTypeDef = TypedDict(
@@ -852,19 +825,17 @@
     {
         "Type": ThresholdTypeType,
         "Unit": ThresholdUnitType,
     },
     total=False,
 )
 
-
 class ThresholdTypeDef(_RequiredThresholdTypeDef, _OptionalThresholdTypeDef):
     pass
 
-
 _RequiredViewFrameTypeDef = TypedDict(
     "_RequiredViewFrameTypeDef",
     {
         "StartColumnIndex": int,
     },
 )
 _OptionalViewFrameTypeDef = TypedDict(
@@ -875,19 +846,17 @@
         "StartRowIndex": int,
         "RowRange": int,
         "Analytics": AnalyticsModeType,
     },
     total=False,
 )
 
-
 class ViewFrameTypeDef(_RequiredViewFrameTypeDef, _OptionalViewFrameTypeDef):
     pass
 
-
 StartJobRunRequestRequestTypeDef = TypedDict(
     "StartJobRunRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -901,22 +870,20 @@
     "_OptionalStartProjectSessionRequestRequestTypeDef",
     {
         "AssumeControl": bool,
     },
     total=False,
 )
 
-
 class StartProjectSessionRequestRequestTypeDef(
     _RequiredStartProjectSessionRequestRequestTypeDef,
     _OptionalStartProjectSessionRequestRequestTypeDef,
 ):
     pass
 
-
 StatisticOverrideOutputTypeDef = TypedDict(
     "StatisticOverrideOutputTypeDef",
     {
         "Statistic": str,
         "Parameters": Dict[str, str],
     },
 )
@@ -964,64 +931,58 @@
     "_OptionalUpdateScheduleRequestRequestTypeDef",
     {
         "JobNames": Sequence[str],
     },
     total=False,
 )
 
-
 class UpdateScheduleRequestRequestTypeDef(
     _RequiredUpdateScheduleRequestRequestTypeDef, _OptionalUpdateScheduleRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredEntityDetectorConfigurationOutputTypeDef = TypedDict(
     "_RequiredEntityDetectorConfigurationOutputTypeDef",
     {
         "EntityTypes": List[str],
     },
 )
 _OptionalEntityDetectorConfigurationOutputTypeDef = TypedDict(
     "_OptionalEntityDetectorConfigurationOutputTypeDef",
     {
         "AllowedStatistics": List[AllowedStatisticsOutputTypeDef],
     },
     total=False,
 )
 
-
 class EntityDetectorConfigurationOutputTypeDef(
     _RequiredEntityDetectorConfigurationOutputTypeDef,
     _OptionalEntityDetectorConfigurationOutputTypeDef,
 ):
     pass
 
-
 _RequiredEntityDetectorConfigurationTypeDef = TypedDict(
     "_RequiredEntityDetectorConfigurationTypeDef",
     {
         "EntityTypes": Sequence[str],
     },
 )
 _OptionalEntityDetectorConfigurationTypeDef = TypedDict(
     "_OptionalEntityDetectorConfigurationTypeDef",
     {
         "AllowedStatistics": Sequence[AllowedStatisticsTypeDef],
     },
     total=False,
 )
 
-
 class EntityDetectorConfigurationTypeDef(
     _RequiredEntityDetectorConfigurationTypeDef, _OptionalEntityDetectorConfigurationTypeDef
 ):
     pass
 
-
 BatchDeleteRecipeVersionResponseTypeDef = TypedDict(
     "BatchDeleteRecipeVersionResponseTypeDef",
     {
         "Name": str,
         "Errors": List[RecipeVersionErrorDetailTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1268,21 +1229,19 @@
     {
         "CatalogId": str,
         "TempDirectory": S3LocationTypeDef,
     },
     total=False,
 )
 
-
 class DataCatalogInputDefinitionTypeDef(
     _RequiredDataCatalogInputDefinitionTypeDef, _OptionalDataCatalogInputDefinitionTypeDef
 ):
     pass
 
-
 _RequiredDatabaseInputDefinitionTypeDef = TypedDict(
     "_RequiredDatabaseInputDefinitionTypeDef",
     {
         "GlueConnectionName": str,
     },
 )
 _OptionalDatabaseInputDefinitionTypeDef = TypedDict(
@@ -1291,42 +1250,38 @@
         "DatabaseTableName": str,
         "TempDirectory": S3LocationTypeDef,
         "QueryString": str,
     },
     total=False,
 )
 
-
 class DatabaseInputDefinitionTypeDef(
     _RequiredDatabaseInputDefinitionTypeDef, _OptionalDatabaseInputDefinitionTypeDef
 ):
     pass
 
-
 _RequiredDatabaseTableOutputOptionsTypeDef = TypedDict(
     "_RequiredDatabaseTableOutputOptionsTypeDef",
     {
         "TableName": str,
     },
 )
 _OptionalDatabaseTableOutputOptionsTypeDef = TypedDict(
     "_OptionalDatabaseTableOutputOptionsTypeDef",
     {
         "TempDirectory": S3LocationTypeDef,
     },
     total=False,
 )
 
-
 class DatabaseTableOutputOptionsTypeDef(
     _RequiredDatabaseTableOutputOptionsTypeDef, _OptionalDatabaseTableOutputOptionsTypeDef
 ):
     pass
 
-
 S3TableOutputOptionsTypeDef = TypedDict(
     "S3TableOutputOptionsTypeDef",
     {
         "Location": S3LocationTypeDef,
     },
 )
 
@@ -1344,21 +1299,19 @@
     {
         "Sample": SampleTypeDef,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateProjectRequestRequestTypeDef(
     _RequiredCreateProjectRequestRequestTypeDef, _OptionalCreateProjectRequestRequestTypeDef
 ):
     pass
 
-
 DescribeProjectResponseTypeDef = TypedDict(
     "DescribeProjectResponseTypeDef",
     {
         "CreateDate": datetime,
         "CreatedBy": str,
         "DatasetName": str,
         "LastModifiedDate": datetime,
@@ -1398,19 +1351,17 @@
         "RoleArn": str,
         "OpenedBy": str,
         "OpenDate": datetime,
     },
     total=False,
 )
 
-
 class ProjectTypeDef(_RequiredProjectTypeDef, _OptionalProjectTypeDef):
     pass
 
-
 _RequiredUpdateProjectRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateProjectRequestRequestTypeDef",
     {
         "RoleArn": str,
         "Name": str,
     },
 )
@@ -1418,21 +1369,19 @@
     "_OptionalUpdateProjectRequestRequestTypeDef",
     {
         "Sample": SampleTypeDef,
     },
     total=False,
 )
 
-
 class UpdateProjectRequestRequestTypeDef(
     _RequiredUpdateProjectRequestRequestTypeDef, _OptionalUpdateProjectRequestRequestTypeDef
 ):
     pass
 
-
 OutputFormatOptionsTypeDef = TypedDict(
     "OutputFormatOptionsTypeDef",
     {
         "Csv": CsvOutputOptionsTypeDef,
     },
     total=False,
 )
@@ -1450,21 +1399,19 @@
         "DatetimeOptions": DatetimeOptionsTypeDef,
         "CreateColumn": bool,
         "Filter": FilterExpressionOutputTypeDef,
     },
     total=False,
 )
 
-
 class DatasetParameterOutputTypeDef(
     _RequiredDatasetParameterOutputTypeDef, _OptionalDatasetParameterOutputTypeDef
 ):
     pass
 
-
 _RequiredDatasetParameterTypeDef = TypedDict(
     "_RequiredDatasetParameterTypeDef",
     {
         "Name": str,
         "Type": ParameterTypeType,
     },
 )
@@ -1474,19 +1421,17 @@
         "DatetimeOptions": DatetimeOptionsTypeDef,
         "CreateColumn": bool,
         "Filter": FilterExpressionTypeDef,
     },
     total=False,
 )
 
-
 class DatasetParameterTypeDef(_RequiredDatasetParameterTypeDef, _OptionalDatasetParameterTypeDef):
     pass
 
-
 FormatOptionsOutputTypeDef = TypedDict(
     "FormatOptionsOutputTypeDef",
     {
         "Json": JsonOptionsTypeDef,
         "Excel": ExcelOptionsOutputTypeDef,
         "Csv": CsvOptionsTypeDef,
     },
@@ -1521,22 +1466,20 @@
     "_OptionalListJobRunsRequestListJobRunsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListJobRunsRequestListJobRunsPaginateTypeDef(
     _RequiredListJobRunsRequestListJobRunsPaginateTypeDef,
     _OptionalListJobRunsRequestListJobRunsPaginateTypeDef,
 ):
     pass
 
-
 ListJobsRequestListJobsPaginateTypeDef = TypedDict(
     "ListJobsRequestListJobsPaginateTypeDef",
     {
         "DatasetName": str,
         "ProjectName": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
@@ -1561,22 +1504,20 @@
     "_OptionalListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef(
     _RequiredListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef,
     _OptionalListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef,
 ):
     pass
 
-
 ListRecipesRequestListRecipesPaginateTypeDef = TypedDict(
     "ListRecipesRequestListRecipesPaginateTypeDef",
     {
         "RecipeVersion": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -1628,38 +1569,34 @@
     "_OptionalRecipeStepOutputTypeDef",
     {
         "ConditionExpressions": List[ConditionExpressionTypeDef],
     },
     total=False,
 )
 
-
 class RecipeStepOutputTypeDef(_RequiredRecipeStepOutputTypeDef, _OptionalRecipeStepOutputTypeDef):
     pass
 
-
 _RequiredRecipeStepTypeDef = TypedDict(
     "_RequiredRecipeStepTypeDef",
     {
         "Action": RecipeActionTypeDef,
     },
 )
 _OptionalRecipeStepTypeDef = TypedDict(
     "_OptionalRecipeStepTypeDef",
     {
         "ConditionExpressions": Sequence[ConditionExpressionTypeDef],
     },
     total=False,
 )
 
-
 class RecipeStepTypeDef(_RequiredRecipeStepTypeDef, _OptionalRecipeStepTypeDef):
     pass
 
-
 _RequiredRuleOutputTypeDef = TypedDict(
     "_RequiredRuleOutputTypeDef",
     {
         "Name": str,
         "CheckExpression": str,
     },
 )
@@ -1670,19 +1607,17 @@
         "SubstitutionMap": Dict[str, str],
         "Threshold": ThresholdTypeDef,
         "ColumnSelectors": List[ColumnSelectorTypeDef],
     },
     total=False,
 )
 
-
 class RuleOutputTypeDef(_RequiredRuleOutputTypeDef, _OptionalRuleOutputTypeDef):
     pass
 
-
 _RequiredRuleTypeDef = TypedDict(
     "_RequiredRuleTypeDef",
     {
         "Name": str,
         "CheckExpression": str,
     },
 )
@@ -1693,19 +1628,17 @@
         "SubstitutionMap": Mapping[str, str],
         "Threshold": ThresholdTypeDef,
         "ColumnSelectors": Sequence[ColumnSelectorTypeDef],
     },
     total=False,
 )
 
-
 class RuleTypeDef(_RequiredRuleTypeDef, _OptionalRuleTypeDef):
     pass
 
-
 StatisticsConfigurationOutputTypeDef = TypedDict(
     "StatisticsConfigurationOutputTypeDef",
     {
         "IncludedStatistics": List[str],
         "Overrides": List[StatisticOverrideOutputTypeDef],
     },
     total=False,
@@ -1742,19 +1675,17 @@
     "_OptionalDatabaseOutputTypeDef",
     {
         "DatabaseOutputMode": Literal["NEW_TABLE"],
     },
     total=False,
 )
 
-
 class DatabaseOutputTypeDef(_RequiredDatabaseOutputTypeDef, _OptionalDatabaseOutputTypeDef):
     pass
 
-
 _RequiredDataCatalogOutputTypeDef = TypedDict(
     "_RequiredDataCatalogOutputTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
     },
 )
@@ -1765,21 +1696,19 @@
         "S3Options": S3TableOutputOptionsTypeDef,
         "DatabaseOptions": DatabaseTableOutputOptionsTypeDef,
         "Overwrite": bool,
     },
     total=False,
 )
 
-
 class DataCatalogOutputTypeDef(
     _RequiredDataCatalogOutputTypeDef, _OptionalDataCatalogOutputTypeDef
 ):
     pass
 
-
 ListProjectsResponseTypeDef = TypedDict(
     "ListProjectsResponseTypeDef",
     {
         "Projects": List[ProjectTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1792,27 +1721,25 @@
     },
 )
 _OptionalOutputTypeDef = TypedDict(
     "_OptionalOutputTypeDef",
     {
         "CompressionFormat": CompressionFormatType,
         "Format": OutputFormatType,
-        "PartitionColumns": Sequence[str],
+        "PartitionColumns": List[str],
         "Overwrite": bool,
         "FormatOptions": OutputFormatOptionsTypeDef,
         "MaxOutputFiles": int,
     },
     total=False,
 )
 
-
 class OutputTypeDef(_RequiredOutputTypeDef, _OptionalOutputTypeDef):
     pass
 
-
 PathOptionsOutputTypeDef = TypedDict(
     "PathOptionsOutputTypeDef",
     {
         "LastModifiedDateCondition": FilterExpressionOutputTypeDef,
         "FilesLimit": FilesLimitTypeDef,
         "Parameters": Dict[str, DatasetParameterOutputTypeDef],
     },
@@ -1825,14 +1752,15 @@
         "LastModifiedDateCondition": FilterExpressionTypeDef,
         "FilesLimit": FilesLimitTypeDef,
         "Parameters": Mapping[str, DatasetParameterTypeDef],
     },
     total=False,
 )
 
+FormatOptionsUnionTypeDef = Union[FormatOptionsTypeDef, FormatOptionsOutputTypeDef]
 DescribeRecipeResponseTypeDef = TypedDict(
     "DescribeRecipeResponseTypeDef",
     {
         "CreatedBy": str,
         "CreateDate": datetime,
         "LastModifiedBy": str,
         "LastModifiedDate": datetime,
@@ -1870,42 +1798,18 @@
         "Steps": List[RecipeStepOutputTypeDef],
         "Tags": Dict[str, str],
         "RecipeVersion": str,
     },
     total=False,
 )
 
-
 class RecipeTypeDef(_RequiredRecipeTypeDef, _OptionalRecipeTypeDef):
     pass
 
-
-_RequiredCreateRecipeRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateRecipeRequestRequestTypeDef",
-    {
-        "Name": str,
-        "Steps": Sequence[Union[RecipeStepTypeDef, RecipeStepOutputTypeDef]],
-    },
-)
-_OptionalCreateRecipeRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateRecipeRequestRequestTypeDef",
-    {
-        "Description": str,
-        "Tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-
-class CreateRecipeRequestRequestTypeDef(
-    _RequiredCreateRecipeRequestRequestTypeDef, _OptionalCreateRecipeRequestRequestTypeDef
-):
-    pass
-
-
+RecipeStepUnionTypeDef = Union[RecipeStepTypeDef, RecipeStepOutputTypeDef]
 _RequiredSendProjectSessionActionRequestRequestTypeDef = TypedDict(
     "_RequiredSendProjectSessionActionRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalSendProjectSessionActionRequestRequestTypeDef = TypedDict(
@@ -1916,44 +1820,20 @@
         "StepIndex": int,
         "ClientSessionId": str,
         "ViewFrame": ViewFrameTypeDef,
     },
     total=False,
 )
 
-
 class SendProjectSessionActionRequestRequestTypeDef(
     _RequiredSendProjectSessionActionRequestRequestTypeDef,
     _OptionalSendProjectSessionActionRequestRequestTypeDef,
 ):
     pass
 
-
-_RequiredUpdateRecipeRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateRecipeRequestRequestTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalUpdateRecipeRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateRecipeRequestRequestTypeDef",
-    {
-        "Description": str,
-        "Steps": Sequence[Union[RecipeStepTypeDef, RecipeStepOutputTypeDef]],
-    },
-    total=False,
-)
-
-
-class UpdateRecipeRequestRequestTypeDef(
-    _RequiredUpdateRecipeRequestRequestTypeDef, _OptionalUpdateRecipeRequestRequestTypeDef
-):
-    pass
-
-
 DescribeRulesetResponseTypeDef = TypedDict(
     "DescribeRulesetResponseTypeDef",
     {
         "Name": str,
         "Description": str,
         "TargetArn": str,
         "Rules": List[RuleOutputTypeDef],
@@ -1963,137 +1843,54 @@
         "LastModifiedDate": datetime,
         "ResourceArn": str,
         "Tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateRulesetRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateRulesetRequestRequestTypeDef",
-    {
-        "Name": str,
-        "TargetArn": str,
-        "Rules": Sequence[Union[RuleTypeDef, RuleOutputTypeDef]],
-    },
-)
-_OptionalCreateRulesetRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateRulesetRequestRequestTypeDef",
-    {
-        "Description": str,
-        "Tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-
-class CreateRulesetRequestRequestTypeDef(
-    _RequiredCreateRulesetRequestRequestTypeDef, _OptionalCreateRulesetRequestRequestTypeDef
-):
-    pass
-
-
-_RequiredUpdateRulesetRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateRulesetRequestRequestTypeDef",
-    {
-        "Name": str,
-        "Rules": Sequence[Union[RuleTypeDef, RuleOutputTypeDef]],
-    },
-)
-_OptionalUpdateRulesetRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateRulesetRequestRequestTypeDef",
-    {
-        "Description": str,
-    },
-    total=False,
-)
-
-
-class UpdateRulesetRequestRequestTypeDef(
-    _RequiredUpdateRulesetRequestRequestTypeDef, _OptionalUpdateRulesetRequestRequestTypeDef
-):
-    pass
-
-
+RuleUnionTypeDef = Union[RuleTypeDef, RuleOutputTypeDef]
 _RequiredColumnStatisticsConfigurationOutputTypeDef = TypedDict(
     "_RequiredColumnStatisticsConfigurationOutputTypeDef",
     {
         "Statistics": StatisticsConfigurationOutputTypeDef,
     },
 )
 _OptionalColumnStatisticsConfigurationOutputTypeDef = TypedDict(
     "_OptionalColumnStatisticsConfigurationOutputTypeDef",
     {
         "Selectors": List[ColumnSelectorTypeDef],
     },
     total=False,
 )
 
-
 class ColumnStatisticsConfigurationOutputTypeDef(
     _RequiredColumnStatisticsConfigurationOutputTypeDef,
     _OptionalColumnStatisticsConfigurationOutputTypeDef,
 ):
     pass
 
-
 _RequiredColumnStatisticsConfigurationTypeDef = TypedDict(
     "_RequiredColumnStatisticsConfigurationTypeDef",
     {
         "Statistics": StatisticsConfigurationTypeDef,
     },
 )
 _OptionalColumnStatisticsConfigurationTypeDef = TypedDict(
     "_OptionalColumnStatisticsConfigurationTypeDef",
     {
         "Selectors": Sequence[ColumnSelectorTypeDef],
     },
     total=False,
 )
 
-
 class ColumnStatisticsConfigurationTypeDef(
     _RequiredColumnStatisticsConfigurationTypeDef, _OptionalColumnStatisticsConfigurationTypeDef
 ):
     pass
 
-
-_RequiredCreateRecipeJobRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateRecipeJobRequestRequestTypeDef",
-    {
-        "Name": str,
-        "RoleArn": str,
-    },
-)
-_OptionalCreateRecipeJobRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateRecipeJobRequestRequestTypeDef",
-    {
-        "DatasetName": str,
-        "EncryptionKeyArn": str,
-        "EncryptionMode": EncryptionModeType,
-        "LogSubscription": LogSubscriptionType,
-        "MaxCapacity": int,
-        "MaxRetries": int,
-        "Outputs": Sequence[Union[OutputTypeDef, OutputTypeDef]],
-        "DataCatalogOutputs": Sequence[DataCatalogOutputTypeDef],
-        "DatabaseOutputs": Sequence[DatabaseOutputTypeDef],
-        "ProjectName": str,
-        "RecipeReference": RecipeReferenceTypeDef,
-        "Tags": Mapping[str, str],
-        "Timeout": int,
-    },
-    total=False,
-)
-
-
-class CreateRecipeJobRequestRequestTypeDef(
-    _RequiredCreateRecipeJobRequestRequestTypeDef, _OptionalCreateRecipeJobRequestRequestTypeDef
-):
-    pass
-
-
 JobRunTypeDef = TypedDict(
     "JobRunTypeDef",
     {
         "Attempt": int,
         "CompletedOn": datetime,
         "DatasetName": str,
         "ErrorMessage": str,
@@ -2147,49 +1944,18 @@
         "Tags": Dict[str, str],
         "JobSample": JobSampleTypeDef,
         "ValidationConfigurations": List[ValidationConfigurationTypeDef],
     },
     total=False,
 )
 
-
 class JobTypeDef(_RequiredJobTypeDef, _OptionalJobTypeDef):
     pass
 
-
-_RequiredUpdateRecipeJobRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateRecipeJobRequestRequestTypeDef",
-    {
-        "Name": str,
-        "RoleArn": str,
-    },
-)
-_OptionalUpdateRecipeJobRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateRecipeJobRequestRequestTypeDef",
-    {
-        "EncryptionKeyArn": str,
-        "EncryptionMode": EncryptionModeType,
-        "LogSubscription": LogSubscriptionType,
-        "MaxCapacity": int,
-        "MaxRetries": int,
-        "Outputs": Sequence[Union[OutputTypeDef, OutputTypeDef]],
-        "DataCatalogOutputs": Sequence[DataCatalogOutputTypeDef],
-        "DatabaseOutputs": Sequence[DatabaseOutputTypeDef],
-        "Timeout": int,
-    },
-    total=False,
-)
-
-
-class UpdateRecipeJobRequestRequestTypeDef(
-    _RequiredUpdateRecipeJobRequestRequestTypeDef, _OptionalUpdateRecipeJobRequestRequestTypeDef
-):
-    pass
-
-
+UnionTypeDef = Union[OutputTypeDef, OutputTypeDef]
 _RequiredDatasetTypeDef = TypedDict(
     "_RequiredDatasetTypeDef",
     {
         "Name": str,
         "Input": InputTypeDef,
     },
 )
@@ -2207,19 +1973,17 @@
         "PathOptions": PathOptionsOutputTypeDef,
         "Tags": Dict[str, str],
         "ResourceArn": str,
     },
     total=False,
 )
 
-
 class DatasetTypeDef(_RequiredDatasetTypeDef, _OptionalDatasetTypeDef):
     pass
 
-
 DescribeDatasetResponseTypeDef = TypedDict(
     "DescribeDatasetResponseTypeDef",
     {
         "CreatedBy": str,
         "CreateDate": datetime,
         "Name": str,
         "Format": InputFormatType,
@@ -2249,21 +2013,20 @@
         "FormatOptions": FormatOptionsTypeDef,
         "PathOptions": PathOptionsTypeDef,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateDatasetRequestRequestTypeDef(
     _RequiredCreateDatasetRequestRequestTypeDef, _OptionalCreateDatasetRequestRequestTypeDef
 ):
     pass
 
-
+PathOptionsUnionTypeDef = Union[PathOptionsTypeDef, PathOptionsOutputTypeDef]
 _RequiredUpdateDatasetRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDatasetRequestRequestTypeDef",
     {
         "Name": str,
         "Input": InputTypeDef,
     },
 )
@@ -2273,21 +2036,19 @@
         "Format": InputFormatType,
         "FormatOptions": FormatOptionsTypeDef,
         "PathOptions": PathOptionsTypeDef,
     },
     total=False,
 )
 
-
 class UpdateDatasetRequestRequestTypeDef(
     _RequiredUpdateDatasetRequestRequestTypeDef, _OptionalUpdateDatasetRequestRequestTypeDef
 ):
     pass
 
-
 ListRecipeVersionsResponseTypeDef = TypedDict(
     "ListRecipeVersionsResponseTypeDef",
     {
         "NextToken": str,
         "Recipes": List[RecipeTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2298,14 +2059,97 @@
     {
         "Recipes": List[RecipeTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredCreateRecipeRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateRecipeRequestRequestTypeDef",
+    {
+        "Name": str,
+        "Steps": Sequence[RecipeStepUnionTypeDef],
+    },
+)
+_OptionalCreateRecipeRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateRecipeRequestRequestTypeDef",
+    {
+        "Description": str,
+        "Tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+class CreateRecipeRequestRequestTypeDef(
+    _RequiredCreateRecipeRequestRequestTypeDef, _OptionalCreateRecipeRequestRequestTypeDef
+):
+    pass
+
+_RequiredUpdateRecipeRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateRecipeRequestRequestTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalUpdateRecipeRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateRecipeRequestRequestTypeDef",
+    {
+        "Description": str,
+        "Steps": Sequence[RecipeStepUnionTypeDef],
+    },
+    total=False,
+)
+
+class UpdateRecipeRequestRequestTypeDef(
+    _RequiredUpdateRecipeRequestRequestTypeDef, _OptionalUpdateRecipeRequestRequestTypeDef
+):
+    pass
+
+_RequiredCreateRulesetRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateRulesetRequestRequestTypeDef",
+    {
+        "Name": str,
+        "TargetArn": str,
+        "Rules": Sequence[RuleUnionTypeDef],
+    },
+)
+_OptionalCreateRulesetRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateRulesetRequestRequestTypeDef",
+    {
+        "Description": str,
+        "Tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+class CreateRulesetRequestRequestTypeDef(
+    _RequiredCreateRulesetRequestRequestTypeDef, _OptionalCreateRulesetRequestRequestTypeDef
+):
+    pass
+
+_RequiredUpdateRulesetRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateRulesetRequestRequestTypeDef",
+    {
+        "Name": str,
+        "Rules": Sequence[RuleUnionTypeDef],
+    },
+)
+_OptionalUpdateRulesetRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateRulesetRequestRequestTypeDef",
+    {
+        "Description": str,
+    },
+    total=False,
+)
+
+class UpdateRulesetRequestRequestTypeDef(
+    _RequiredUpdateRulesetRequestRequestTypeDef, _OptionalUpdateRulesetRequestRequestTypeDef
+):
+    pass
+
 ProfileConfigurationOutputTypeDef = TypedDict(
     "ProfileConfigurationOutputTypeDef",
     {
         "DatasetStatisticsConfiguration": StatisticsConfigurationOutputTypeDef,
         "ProfileColumns": List[ColumnSelectorTypeDef],
         "ColumnStatisticsConfigurations": List[ColumnStatisticsConfigurationOutputTypeDef],
         "EntityDetectorConfiguration": EntityDetectorConfigurationOutputTypeDef,
@@ -2338,14 +2182,74 @@
     {
         "Jobs": List[JobTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredCreateRecipeJobRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateRecipeJobRequestRequestTypeDef",
+    {
+        "Name": str,
+        "RoleArn": str,
+    },
+)
+_OptionalCreateRecipeJobRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateRecipeJobRequestRequestTypeDef",
+    {
+        "DatasetName": str,
+        "EncryptionKeyArn": str,
+        "EncryptionMode": EncryptionModeType,
+        "LogSubscription": LogSubscriptionType,
+        "MaxCapacity": int,
+        "MaxRetries": int,
+        "Outputs": Sequence[UnionTypeDef],
+        "DataCatalogOutputs": Sequence[DataCatalogOutputTypeDef],
+        "DatabaseOutputs": Sequence[DatabaseOutputTypeDef],
+        "ProjectName": str,
+        "RecipeReference": RecipeReferenceTypeDef,
+        "Tags": Mapping[str, str],
+        "Timeout": int,
+    },
+    total=False,
+)
+
+class CreateRecipeJobRequestRequestTypeDef(
+    _RequiredCreateRecipeJobRequestRequestTypeDef, _OptionalCreateRecipeJobRequestRequestTypeDef
+):
+    pass
+
+_RequiredUpdateRecipeJobRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateRecipeJobRequestRequestTypeDef",
+    {
+        "Name": str,
+        "RoleArn": str,
+    },
+)
+_OptionalUpdateRecipeJobRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateRecipeJobRequestRequestTypeDef",
+    {
+        "EncryptionKeyArn": str,
+        "EncryptionMode": EncryptionModeType,
+        "LogSubscription": LogSubscriptionType,
+        "MaxCapacity": int,
+        "MaxRetries": int,
+        "Outputs": Sequence[UnionTypeDef],
+        "DataCatalogOutputs": Sequence[DataCatalogOutputTypeDef],
+        "DatabaseOutputs": Sequence[DatabaseOutputTypeDef],
+        "Timeout": int,
+    },
+    total=False,
+)
+
+class UpdateRecipeJobRequestRequestTypeDef(
+    _RequiredUpdateRecipeJobRequestRequestTypeDef, _OptionalUpdateRecipeJobRequestRequestTypeDef
+):
+    pass
+
 ListDatasetsResponseTypeDef = TypedDict(
     "ListDatasetsResponseTypeDef",
     {
         "Datasets": List[DatasetTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2430,21 +2334,22 @@
         "Tags": Mapping[str, str],
         "Timeout": int,
         "JobSample": JobSampleTypeDef,
     },
     total=False,
 )
 
-
 class CreateProfileJobRequestRequestTypeDef(
     _RequiredCreateProfileJobRequestRequestTypeDef, _OptionalCreateProfileJobRequestRequestTypeDef
 ):
     pass
 
-
+ProfileConfigurationUnionTypeDef = Union[
+    ProfileConfigurationTypeDef, ProfileConfigurationOutputTypeDef
+]
 _RequiredUpdateProfileJobRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateProfileJobRequestRequestTypeDef",
     {
         "Name": str,
         "OutputLocation": S3LocationTypeDef,
         "RoleArn": str,
     },
@@ -2461,12 +2366,11 @@
         "ValidationConfigurations": Sequence[ValidationConfigurationTypeDef],
         "Timeout": int,
         "JobSample": JobSampleTypeDef,
     },
     total=False,
 )
 
-
 class UpdateProfileJobRequestRequestTypeDef(
     _RequiredUpdateProfileJobRequestRequestTypeDef, _OptionalUpdateProfileJobRequestRequestTypeDef
 ):
     pass
```

### Comparing `mypy-boto3-databrew-1.28.15.post1/mypy_boto3_databrew/type_defs.pyi` & `mypy-boto3-databrew-1.28.16/mypy_boto3_databrew/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_databrew.type_defs import AllowedStatisticsOutputTypeDef
 
-    data: AllowedStatisticsOutputTypeDef = {...}
+    data: AllowedStatisticsOutputTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -39,14 +39,15 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AllowedStatisticsOutputTypeDef",
     "AllowedStatisticsTypeDef",
     "BatchDeleteRecipeVersionRequestRequestTypeDef",
     "RecipeVersionErrorDetailTypeDef",
     "ResponseMetadataTypeDef",
     "ColumnSelectorTypeDef",
@@ -167,42 +168,48 @@
     "InputTypeDef",
     "DatabaseOutputTypeDef",
     "DataCatalogOutputTypeDef",
     "ListProjectsResponseTypeDef",
     "OutputTypeDef",
     "PathOptionsOutputTypeDef",
     "PathOptionsTypeDef",
+    "FormatOptionsUnionTypeDef",
     "DescribeRecipeResponseTypeDef",
     "RecipeTypeDef",
-    "CreateRecipeRequestRequestTypeDef",
+    "RecipeStepUnionTypeDef",
     "SendProjectSessionActionRequestRequestTypeDef",
-    "UpdateRecipeRequestRequestTypeDef",
     "DescribeRulesetResponseTypeDef",
-    "CreateRulesetRequestRequestTypeDef",
-    "UpdateRulesetRequestRequestTypeDef",
+    "RuleUnionTypeDef",
     "ColumnStatisticsConfigurationOutputTypeDef",
     "ColumnStatisticsConfigurationTypeDef",
-    "CreateRecipeJobRequestRequestTypeDef",
     "JobRunTypeDef",
     "JobTypeDef",
-    "UpdateRecipeJobRequestRequestTypeDef",
+    "UnionTypeDef",
     "DatasetTypeDef",
     "DescribeDatasetResponseTypeDef",
     "CreateDatasetRequestRequestTypeDef",
+    "PathOptionsUnionTypeDef",
     "UpdateDatasetRequestRequestTypeDef",
     "ListRecipeVersionsResponseTypeDef",
     "ListRecipesResponseTypeDef",
+    "CreateRecipeRequestRequestTypeDef",
+    "UpdateRecipeRequestRequestTypeDef",
+    "CreateRulesetRequestRequestTypeDef",
+    "UpdateRulesetRequestRequestTypeDef",
     "ProfileConfigurationOutputTypeDef",
     "ProfileConfigurationTypeDef",
     "ListJobRunsResponseTypeDef",
     "ListJobsResponseTypeDef",
+    "CreateRecipeJobRequestRequestTypeDef",
+    "UpdateRecipeJobRequestRequestTypeDef",
     "ListDatasetsResponseTypeDef",
     "DescribeJobResponseTypeDef",
     "DescribeJobRunResponseTypeDef",
     "CreateProfileJobRequestRequestTypeDef",
+    "ProfileConfigurationUnionTypeDef",
     "UpdateProfileJobRequestRequestTypeDef",
 )
 
 AllowedStatisticsOutputTypeDef = TypedDict(
     "AllowedStatisticsOutputTypeDef",
     {
         "Statistics": List[str],
@@ -265,19 +272,21 @@
     "_OptionalConditionExpressionTypeDef",
     {
         "Value": str,
     },
     total=False,
 )
 
+
 class ConditionExpressionTypeDef(
     _RequiredConditionExpressionTypeDef, _OptionalConditionExpressionTypeDef
 ):
     pass
 
+
 JobSampleTypeDef = TypedDict(
     "JobSampleTypeDef",
     {
         "Mode": SampleModeType,
         "Size": int,
     },
     total=False,
@@ -294,70 +303,78 @@
     {
         "Key": str,
         "BucketOwner": str,
     },
     total=False,
 )
 
+
 class S3LocationTypeDef(_RequiredS3LocationTypeDef, _OptionalS3LocationTypeDef):
     pass
 
+
 _RequiredValidationConfigurationTypeDef = TypedDict(
     "_RequiredValidationConfigurationTypeDef",
     {
         "RulesetArn": str,
     },
 )
 _OptionalValidationConfigurationTypeDef = TypedDict(
     "_OptionalValidationConfigurationTypeDef",
     {
         "ValidationMode": Literal["CHECK_ALL"],
     },
     total=False,
 )
 
+
 class ValidationConfigurationTypeDef(
     _RequiredValidationConfigurationTypeDef, _OptionalValidationConfigurationTypeDef
 ):
     pass
 
+
 _RequiredSampleTypeDef = TypedDict(
     "_RequiredSampleTypeDef",
     {
         "Type": SampleTypeType,
     },
 )
 _OptionalSampleTypeDef = TypedDict(
     "_OptionalSampleTypeDef",
     {
         "Size": int,
     },
     total=False,
 )
 
+
 class SampleTypeDef(_RequiredSampleTypeDef, _OptionalSampleTypeDef):
     pass
 
+
 _RequiredRecipeReferenceTypeDef = TypedDict(
     "_RequiredRecipeReferenceTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalRecipeReferenceTypeDef = TypedDict(
     "_OptionalRecipeReferenceTypeDef",
     {
         "RecipeVersion": str,
     },
     total=False,
 )
 
+
 class RecipeReferenceTypeDef(_RequiredRecipeReferenceTypeDef, _OptionalRecipeReferenceTypeDef):
     pass
 
+
 _RequiredCreateScheduleRequestRequestTypeDef = TypedDict(
     "_RequiredCreateScheduleRequestRequestTypeDef",
     {
         "CronExpression": str,
         "Name": str,
     },
 )
@@ -366,19 +383,21 @@
     {
         "JobNames": Sequence[str],
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateScheduleRequestRequestTypeDef(
     _RequiredCreateScheduleRequestRequestTypeDef, _OptionalCreateScheduleRequestRequestTypeDef
 ):
     pass
 
+
 CsvOptionsTypeDef = TypedDict(
     "CsvOptionsTypeDef",
     {
         "Delimiter": str,
         "HeaderRow": bool,
     },
     total=False,
@@ -403,17 +422,19 @@
     {
         "TimezoneOffset": str,
         "LocaleCode": str,
     },
     total=False,
 )
 
+
 class DatetimeOptionsTypeDef(_RequiredDatetimeOptionsTypeDef, _OptionalDatetimeOptionsTypeDef):
     pass
 
+
 FilterExpressionOutputTypeDef = TypedDict(
     "FilterExpressionOutputTypeDef",
     {
         "Expression": str,
         "ValuesMap": Dict[str, str],
     },
 )
@@ -508,19 +529,21 @@
     "_OptionalDescribeRecipeRequestRequestTypeDef",
     {
         "RecipeVersion": str,
     },
     total=False,
 )
 
+
 class DescribeRecipeRequestRequestTypeDef(
     _RequiredDescribeRecipeRequestRequestTypeDef, _OptionalDescribeRecipeRequestRequestTypeDef
 ):
     pass
 
+
 DescribeRulesetRequestRequestTypeDef = TypedDict(
     "DescribeRulesetRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -562,17 +585,19 @@
     {
         "OrderedBy": Literal["LAST_MODIFIED_DATE"],
         "Order": OrderType,
     },
     total=False,
 )
 
+
 class FilesLimitTypeDef(_RequiredFilesLimitTypeDef, _OptionalFilesLimitTypeDef):
     pass
 
+
 JsonOptionsTypeDef = TypedDict(
     "JsonOptionsTypeDef",
     {
         "MultiLine": bool,
     },
     total=False,
 )
@@ -615,19 +640,21 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListJobRunsRequestRequestTypeDef(
     _RequiredListJobRunsRequestRequestTypeDef, _OptionalListJobRunsRequestRequestTypeDef
 ):
     pass
 
+
 ListJobsRequestRequestTypeDef = TypedDict(
     "ListJobsRequestRequestTypeDef",
     {
         "DatasetName": str,
         "MaxResults": int,
         "NextToken": str,
         "ProjectName": str,
@@ -655,20 +682,22 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListRecipeVersionsRequestRequestTypeDef(
     _RequiredListRecipeVersionsRequestRequestTypeDef,
     _OptionalListRecipeVersionsRequestRequestTypeDef,
 ):
     pass
 
+
 ListRecipesRequestRequestTypeDef = TypedDict(
     "ListRecipesRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "RecipeVersion": str,
     },
@@ -704,17 +733,19 @@
         "ResourceArn": str,
         "RuleCount": int,
         "Tags": Dict[str, str],
     },
     total=False,
 )
 
+
 class RulesetItemTypeDef(_RequiredRulesetItemTypeDef, _OptionalRulesetItemTypeDef):
     pass
 
+
 ListSchedulesRequestRequestTypeDef = TypedDict(
     "ListSchedulesRequestRequestTypeDef",
     {
         "JobName": str,
         "MaxResults": int,
         "NextToken": str,
     },
@@ -739,17 +770,19 @@
         "ResourceArn": str,
         "CronExpression": str,
         "Tags": Dict[str, str],
     },
     total=False,
 )
 
+
 class ScheduleTypeDef(_RequiredScheduleTypeDef, _OptionalScheduleTypeDef):
     pass
 
+
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
@@ -763,55 +796,61 @@
     "_OptionalPublishRecipeRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
+
 class PublishRecipeRequestRequestTypeDef(
     _RequiredPublishRecipeRequestRequestTypeDef, _OptionalPublishRecipeRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredRecipeActionOutputTypeDef = TypedDict(
     "_RequiredRecipeActionOutputTypeDef",
     {
         "Operation": str,
     },
 )
 _OptionalRecipeActionOutputTypeDef = TypedDict(
     "_OptionalRecipeActionOutputTypeDef",
     {
         "Parameters": Dict[str, str],
     },
     total=False,
 )
 
+
 class RecipeActionOutputTypeDef(
     _RequiredRecipeActionOutputTypeDef, _OptionalRecipeActionOutputTypeDef
 ):
     pass
 
+
 _RequiredRecipeActionTypeDef = TypedDict(
     "_RequiredRecipeActionTypeDef",
     {
         "Operation": str,
     },
 )
 _OptionalRecipeActionTypeDef = TypedDict(
     "_OptionalRecipeActionTypeDef",
     {
         "Parameters": Mapping[str, str],
     },
     total=False,
 )
 
+
 class RecipeActionTypeDef(_RequiredRecipeActionTypeDef, _OptionalRecipeActionTypeDef):
     pass
 
+
 _RequiredThresholdTypeDef = TypedDict(
     "_RequiredThresholdTypeDef",
     {
         "Value": float,
     },
 )
 _OptionalThresholdTypeDef = TypedDict(
@@ -819,17 +858,19 @@
     {
         "Type": ThresholdTypeType,
         "Unit": ThresholdUnitType,
     },
     total=False,
 )
 
+
 class ThresholdTypeDef(_RequiredThresholdTypeDef, _OptionalThresholdTypeDef):
     pass
 
+
 _RequiredViewFrameTypeDef = TypedDict(
     "_RequiredViewFrameTypeDef",
     {
         "StartColumnIndex": int,
     },
 )
 _OptionalViewFrameTypeDef = TypedDict(
@@ -840,17 +881,19 @@
         "StartRowIndex": int,
         "RowRange": int,
         "Analytics": AnalyticsModeType,
     },
     total=False,
 )
 
+
 class ViewFrameTypeDef(_RequiredViewFrameTypeDef, _OptionalViewFrameTypeDef):
     pass
 
+
 StartJobRunRequestRequestTypeDef = TypedDict(
     "StartJobRunRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -864,20 +907,22 @@
     "_OptionalStartProjectSessionRequestRequestTypeDef",
     {
         "AssumeControl": bool,
     },
     total=False,
 )
 
+
 class StartProjectSessionRequestRequestTypeDef(
     _RequiredStartProjectSessionRequestRequestTypeDef,
     _OptionalStartProjectSessionRequestRequestTypeDef,
 ):
     pass
 
+
 StatisticOverrideOutputTypeDef = TypedDict(
     "StatisticOverrideOutputTypeDef",
     {
         "Statistic": str,
         "Parameters": Dict[str, str],
     },
 )
@@ -925,58 +970,64 @@
     "_OptionalUpdateScheduleRequestRequestTypeDef",
     {
         "JobNames": Sequence[str],
     },
     total=False,
 )
 
+
 class UpdateScheduleRequestRequestTypeDef(
     _RequiredUpdateScheduleRequestRequestTypeDef, _OptionalUpdateScheduleRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredEntityDetectorConfigurationOutputTypeDef = TypedDict(
     "_RequiredEntityDetectorConfigurationOutputTypeDef",
     {
         "EntityTypes": List[str],
     },
 )
 _OptionalEntityDetectorConfigurationOutputTypeDef = TypedDict(
     "_OptionalEntityDetectorConfigurationOutputTypeDef",
     {
         "AllowedStatistics": List[AllowedStatisticsOutputTypeDef],
     },
     total=False,
 )
 
+
 class EntityDetectorConfigurationOutputTypeDef(
     _RequiredEntityDetectorConfigurationOutputTypeDef,
     _OptionalEntityDetectorConfigurationOutputTypeDef,
 ):
     pass
 
+
 _RequiredEntityDetectorConfigurationTypeDef = TypedDict(
     "_RequiredEntityDetectorConfigurationTypeDef",
     {
         "EntityTypes": Sequence[str],
     },
 )
 _OptionalEntityDetectorConfigurationTypeDef = TypedDict(
     "_OptionalEntityDetectorConfigurationTypeDef",
     {
         "AllowedStatistics": Sequence[AllowedStatisticsTypeDef],
     },
     total=False,
 )
 
+
 class EntityDetectorConfigurationTypeDef(
     _RequiredEntityDetectorConfigurationTypeDef, _OptionalEntityDetectorConfigurationTypeDef
 ):
     pass
 
+
 BatchDeleteRecipeVersionResponseTypeDef = TypedDict(
     "BatchDeleteRecipeVersionResponseTypeDef",
     {
         "Name": str,
         "Errors": List[RecipeVersionErrorDetailTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1223,19 +1274,21 @@
     {
         "CatalogId": str,
         "TempDirectory": S3LocationTypeDef,
     },
     total=False,
 )
 
+
 class DataCatalogInputDefinitionTypeDef(
     _RequiredDataCatalogInputDefinitionTypeDef, _OptionalDataCatalogInputDefinitionTypeDef
 ):
     pass
 
+
 _RequiredDatabaseInputDefinitionTypeDef = TypedDict(
     "_RequiredDatabaseInputDefinitionTypeDef",
     {
         "GlueConnectionName": str,
     },
 )
 _OptionalDatabaseInputDefinitionTypeDef = TypedDict(
@@ -1244,38 +1297,42 @@
         "DatabaseTableName": str,
         "TempDirectory": S3LocationTypeDef,
         "QueryString": str,
     },
     total=False,
 )
 
+
 class DatabaseInputDefinitionTypeDef(
     _RequiredDatabaseInputDefinitionTypeDef, _OptionalDatabaseInputDefinitionTypeDef
 ):
     pass
 
+
 _RequiredDatabaseTableOutputOptionsTypeDef = TypedDict(
     "_RequiredDatabaseTableOutputOptionsTypeDef",
     {
         "TableName": str,
     },
 )
 _OptionalDatabaseTableOutputOptionsTypeDef = TypedDict(
     "_OptionalDatabaseTableOutputOptionsTypeDef",
     {
         "TempDirectory": S3LocationTypeDef,
     },
     total=False,
 )
 
+
 class DatabaseTableOutputOptionsTypeDef(
     _RequiredDatabaseTableOutputOptionsTypeDef, _OptionalDatabaseTableOutputOptionsTypeDef
 ):
     pass
 
+
 S3TableOutputOptionsTypeDef = TypedDict(
     "S3TableOutputOptionsTypeDef",
     {
         "Location": S3LocationTypeDef,
     },
 )
 
@@ -1293,19 +1350,21 @@
     {
         "Sample": SampleTypeDef,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateProjectRequestRequestTypeDef(
     _RequiredCreateProjectRequestRequestTypeDef, _OptionalCreateProjectRequestRequestTypeDef
 ):
     pass
 
+
 DescribeProjectResponseTypeDef = TypedDict(
     "DescribeProjectResponseTypeDef",
     {
         "CreateDate": datetime,
         "CreatedBy": str,
         "DatasetName": str,
         "LastModifiedDate": datetime,
@@ -1345,17 +1404,19 @@
         "RoleArn": str,
         "OpenedBy": str,
         "OpenDate": datetime,
     },
     total=False,
 )
 
+
 class ProjectTypeDef(_RequiredProjectTypeDef, _OptionalProjectTypeDef):
     pass
 
+
 _RequiredUpdateProjectRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateProjectRequestRequestTypeDef",
     {
         "RoleArn": str,
         "Name": str,
     },
 )
@@ -1363,19 +1424,21 @@
     "_OptionalUpdateProjectRequestRequestTypeDef",
     {
         "Sample": SampleTypeDef,
     },
     total=False,
 )
 
+
 class UpdateProjectRequestRequestTypeDef(
     _RequiredUpdateProjectRequestRequestTypeDef, _OptionalUpdateProjectRequestRequestTypeDef
 ):
     pass
 
+
 OutputFormatOptionsTypeDef = TypedDict(
     "OutputFormatOptionsTypeDef",
     {
         "Csv": CsvOutputOptionsTypeDef,
     },
     total=False,
 )
@@ -1393,19 +1456,21 @@
         "DatetimeOptions": DatetimeOptionsTypeDef,
         "CreateColumn": bool,
         "Filter": FilterExpressionOutputTypeDef,
     },
     total=False,
 )
 
+
 class DatasetParameterOutputTypeDef(
     _RequiredDatasetParameterOutputTypeDef, _OptionalDatasetParameterOutputTypeDef
 ):
     pass
 
+
 _RequiredDatasetParameterTypeDef = TypedDict(
     "_RequiredDatasetParameterTypeDef",
     {
         "Name": str,
         "Type": ParameterTypeType,
     },
 )
@@ -1415,17 +1480,19 @@
         "DatetimeOptions": DatetimeOptionsTypeDef,
         "CreateColumn": bool,
         "Filter": FilterExpressionTypeDef,
     },
     total=False,
 )
 
+
 class DatasetParameterTypeDef(_RequiredDatasetParameterTypeDef, _OptionalDatasetParameterTypeDef):
     pass
 
+
 FormatOptionsOutputTypeDef = TypedDict(
     "FormatOptionsOutputTypeDef",
     {
         "Json": JsonOptionsTypeDef,
         "Excel": ExcelOptionsOutputTypeDef,
         "Csv": CsvOptionsTypeDef,
     },
@@ -1460,20 +1527,22 @@
     "_OptionalListJobRunsRequestListJobRunsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListJobRunsRequestListJobRunsPaginateTypeDef(
     _RequiredListJobRunsRequestListJobRunsPaginateTypeDef,
     _OptionalListJobRunsRequestListJobRunsPaginateTypeDef,
 ):
     pass
 
+
 ListJobsRequestListJobsPaginateTypeDef = TypedDict(
     "ListJobsRequestListJobsPaginateTypeDef",
     {
         "DatasetName": str,
         "ProjectName": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
@@ -1498,20 +1567,22 @@
     "_OptionalListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef(
     _RequiredListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef,
     _OptionalListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef,
 ):
     pass
 
+
 ListRecipesRequestListRecipesPaginateTypeDef = TypedDict(
     "ListRecipesRequestListRecipesPaginateTypeDef",
     {
         "RecipeVersion": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -1563,34 +1634,38 @@
     "_OptionalRecipeStepOutputTypeDef",
     {
         "ConditionExpressions": List[ConditionExpressionTypeDef],
     },
     total=False,
 )
 
+
 class RecipeStepOutputTypeDef(_RequiredRecipeStepOutputTypeDef, _OptionalRecipeStepOutputTypeDef):
     pass
 
+
 _RequiredRecipeStepTypeDef = TypedDict(
     "_RequiredRecipeStepTypeDef",
     {
         "Action": RecipeActionTypeDef,
     },
 )
 _OptionalRecipeStepTypeDef = TypedDict(
     "_OptionalRecipeStepTypeDef",
     {
         "ConditionExpressions": Sequence[ConditionExpressionTypeDef],
     },
     total=False,
 )
 
+
 class RecipeStepTypeDef(_RequiredRecipeStepTypeDef, _OptionalRecipeStepTypeDef):
     pass
 
+
 _RequiredRuleOutputTypeDef = TypedDict(
     "_RequiredRuleOutputTypeDef",
     {
         "Name": str,
         "CheckExpression": str,
     },
 )
@@ -1601,17 +1676,19 @@
         "SubstitutionMap": Dict[str, str],
         "Threshold": ThresholdTypeDef,
         "ColumnSelectors": List[ColumnSelectorTypeDef],
     },
     total=False,
 )
 
+
 class RuleOutputTypeDef(_RequiredRuleOutputTypeDef, _OptionalRuleOutputTypeDef):
     pass
 
+
 _RequiredRuleTypeDef = TypedDict(
     "_RequiredRuleTypeDef",
     {
         "Name": str,
         "CheckExpression": str,
     },
 )
@@ -1622,17 +1699,19 @@
         "SubstitutionMap": Mapping[str, str],
         "Threshold": ThresholdTypeDef,
         "ColumnSelectors": Sequence[ColumnSelectorTypeDef],
     },
     total=False,
 )
 
+
 class RuleTypeDef(_RequiredRuleTypeDef, _OptionalRuleTypeDef):
     pass
 
+
 StatisticsConfigurationOutputTypeDef = TypedDict(
     "StatisticsConfigurationOutputTypeDef",
     {
         "IncludedStatistics": List[str],
         "Overrides": List[StatisticOverrideOutputTypeDef],
     },
     total=False,
@@ -1669,17 +1748,19 @@
     "_OptionalDatabaseOutputTypeDef",
     {
         "DatabaseOutputMode": Literal["NEW_TABLE"],
     },
     total=False,
 )
 
+
 class DatabaseOutputTypeDef(_RequiredDatabaseOutputTypeDef, _OptionalDatabaseOutputTypeDef):
     pass
 
+
 _RequiredDataCatalogOutputTypeDef = TypedDict(
     "_RequiredDataCatalogOutputTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
     },
 )
@@ -1690,19 +1771,21 @@
         "S3Options": S3TableOutputOptionsTypeDef,
         "DatabaseOptions": DatabaseTableOutputOptionsTypeDef,
         "Overwrite": bool,
     },
     total=False,
 )
 
+
 class DataCatalogOutputTypeDef(
     _RequiredDataCatalogOutputTypeDef, _OptionalDataCatalogOutputTypeDef
 ):
     pass
 
+
 ListProjectsResponseTypeDef = TypedDict(
     "ListProjectsResponseTypeDef",
     {
         "Projects": List[ProjectTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1715,25 +1798,27 @@
     },
 )
 _OptionalOutputTypeDef = TypedDict(
     "_OptionalOutputTypeDef",
     {
         "CompressionFormat": CompressionFormatType,
         "Format": OutputFormatType,
-        "PartitionColumns": Sequence[str],
+        "PartitionColumns": List[str],
         "Overwrite": bool,
         "FormatOptions": OutputFormatOptionsTypeDef,
         "MaxOutputFiles": int,
     },
     total=False,
 )
 
+
 class OutputTypeDef(_RequiredOutputTypeDef, _OptionalOutputTypeDef):
     pass
 
+
 PathOptionsOutputTypeDef = TypedDict(
     "PathOptionsOutputTypeDef",
     {
         "LastModifiedDateCondition": FilterExpressionOutputTypeDef,
         "FilesLimit": FilesLimitTypeDef,
         "Parameters": Dict[str, DatasetParameterOutputTypeDef],
     },
@@ -1746,14 +1831,15 @@
         "LastModifiedDateCondition": FilterExpressionTypeDef,
         "FilesLimit": FilesLimitTypeDef,
         "Parameters": Mapping[str, DatasetParameterTypeDef],
     },
     total=False,
 )
 
+FormatOptionsUnionTypeDef = Union[FormatOptionsTypeDef, FormatOptionsOutputTypeDef]
 DescribeRecipeResponseTypeDef = TypedDict(
     "DescribeRecipeResponseTypeDef",
     {
         "CreatedBy": str,
         "CreateDate": datetime,
         "LastModifiedBy": str,
         "LastModifiedDate": datetime,
@@ -1791,38 +1877,20 @@
         "Steps": List[RecipeStepOutputTypeDef],
         "Tags": Dict[str, str],
         "RecipeVersion": str,
     },
     total=False,
 )
 
+
 class RecipeTypeDef(_RequiredRecipeTypeDef, _OptionalRecipeTypeDef):
     pass
 
-_RequiredCreateRecipeRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateRecipeRequestRequestTypeDef",
-    {
-        "Name": str,
-        "Steps": Sequence[Union[RecipeStepTypeDef, RecipeStepOutputTypeDef]],
-    },
-)
-_OptionalCreateRecipeRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateRecipeRequestRequestTypeDef",
-    {
-        "Description": str,
-        "Tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-class CreateRecipeRequestRequestTypeDef(
-    _RequiredCreateRecipeRequestRequestTypeDef, _OptionalCreateRecipeRequestRequestTypeDef
-):
-    pass
 
+RecipeStepUnionTypeDef = Union[RecipeStepTypeDef, RecipeStepOutputTypeDef]
 _RequiredSendProjectSessionActionRequestRequestTypeDef = TypedDict(
     "_RequiredSendProjectSessionActionRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalSendProjectSessionActionRequestRequestTypeDef = TypedDict(
@@ -1833,39 +1901,21 @@
         "StepIndex": int,
         "ClientSessionId": str,
         "ViewFrame": ViewFrameTypeDef,
     },
     total=False,
 )
 
+
 class SendProjectSessionActionRequestRequestTypeDef(
     _RequiredSendProjectSessionActionRequestRequestTypeDef,
     _OptionalSendProjectSessionActionRequestRequestTypeDef,
 ):
     pass
 
-_RequiredUpdateRecipeRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateRecipeRequestRequestTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalUpdateRecipeRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateRecipeRequestRequestTypeDef",
-    {
-        "Description": str,
-        "Steps": Sequence[Union[RecipeStepTypeDef, RecipeStepOutputTypeDef]],
-    },
-    total=False,
-)
-
-class UpdateRecipeRequestRequestTypeDef(
-    _RequiredUpdateRecipeRequestRequestTypeDef, _OptionalUpdateRecipeRequestRequestTypeDef
-):
-    pass
 
 DescribeRulesetResponseTypeDef = TypedDict(
     "DescribeRulesetResponseTypeDef",
     {
         "Name": str,
         "Description": str,
         "TargetArn": str,
@@ -1876,126 +1926,57 @@
         "LastModifiedDate": datetime,
         "ResourceArn": str,
         "Tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateRulesetRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateRulesetRequestRequestTypeDef",
-    {
-        "Name": str,
-        "TargetArn": str,
-        "Rules": Sequence[Union[RuleTypeDef, RuleOutputTypeDef]],
-    },
-)
-_OptionalCreateRulesetRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateRulesetRequestRequestTypeDef",
-    {
-        "Description": str,
-        "Tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-class CreateRulesetRequestRequestTypeDef(
-    _RequiredCreateRulesetRequestRequestTypeDef, _OptionalCreateRulesetRequestRequestTypeDef
-):
-    pass
-
-_RequiredUpdateRulesetRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateRulesetRequestRequestTypeDef",
-    {
-        "Name": str,
-        "Rules": Sequence[Union[RuleTypeDef, RuleOutputTypeDef]],
-    },
-)
-_OptionalUpdateRulesetRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateRulesetRequestRequestTypeDef",
-    {
-        "Description": str,
-    },
-    total=False,
-)
-
-class UpdateRulesetRequestRequestTypeDef(
-    _RequiredUpdateRulesetRequestRequestTypeDef, _OptionalUpdateRulesetRequestRequestTypeDef
-):
-    pass
-
+RuleUnionTypeDef = Union[RuleTypeDef, RuleOutputTypeDef]
 _RequiredColumnStatisticsConfigurationOutputTypeDef = TypedDict(
     "_RequiredColumnStatisticsConfigurationOutputTypeDef",
     {
         "Statistics": StatisticsConfigurationOutputTypeDef,
     },
 )
 _OptionalColumnStatisticsConfigurationOutputTypeDef = TypedDict(
     "_OptionalColumnStatisticsConfigurationOutputTypeDef",
     {
         "Selectors": List[ColumnSelectorTypeDef],
     },
     total=False,
 )
 
+
 class ColumnStatisticsConfigurationOutputTypeDef(
     _RequiredColumnStatisticsConfigurationOutputTypeDef,
     _OptionalColumnStatisticsConfigurationOutputTypeDef,
 ):
     pass
 
+
 _RequiredColumnStatisticsConfigurationTypeDef = TypedDict(
     "_RequiredColumnStatisticsConfigurationTypeDef",
     {
         "Statistics": StatisticsConfigurationTypeDef,
     },
 )
 _OptionalColumnStatisticsConfigurationTypeDef = TypedDict(
     "_OptionalColumnStatisticsConfigurationTypeDef",
     {
         "Selectors": Sequence[ColumnSelectorTypeDef],
     },
     total=False,
 )
 
+
 class ColumnStatisticsConfigurationTypeDef(
     _RequiredColumnStatisticsConfigurationTypeDef, _OptionalColumnStatisticsConfigurationTypeDef
 ):
     pass
 
-_RequiredCreateRecipeJobRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateRecipeJobRequestRequestTypeDef",
-    {
-        "Name": str,
-        "RoleArn": str,
-    },
-)
-_OptionalCreateRecipeJobRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateRecipeJobRequestRequestTypeDef",
-    {
-        "DatasetName": str,
-        "EncryptionKeyArn": str,
-        "EncryptionMode": EncryptionModeType,
-        "LogSubscription": LogSubscriptionType,
-        "MaxCapacity": int,
-        "MaxRetries": int,
-        "Outputs": Sequence[Union[OutputTypeDef, OutputTypeDef]],
-        "DataCatalogOutputs": Sequence[DataCatalogOutputTypeDef],
-        "DatabaseOutputs": Sequence[DatabaseOutputTypeDef],
-        "ProjectName": str,
-        "RecipeReference": RecipeReferenceTypeDef,
-        "Tags": Mapping[str, str],
-        "Timeout": int,
-    },
-    total=False,
-)
-
-class CreateRecipeJobRequestRequestTypeDef(
-    _RequiredCreateRecipeJobRequestRequestTypeDef, _OptionalCreateRecipeJobRequestRequestTypeDef
-):
-    pass
 
 JobRunTypeDef = TypedDict(
     "JobRunTypeDef",
     {
         "Attempt": int,
         "CompletedOn": datetime,
         "DatasetName": str,
@@ -2050,45 +2031,20 @@
         "Tags": Dict[str, str],
         "JobSample": JobSampleTypeDef,
         "ValidationConfigurations": List[ValidationConfigurationTypeDef],
     },
     total=False,
 )
 
+
 class JobTypeDef(_RequiredJobTypeDef, _OptionalJobTypeDef):
     pass
 
-_RequiredUpdateRecipeJobRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateRecipeJobRequestRequestTypeDef",
-    {
-        "Name": str,
-        "RoleArn": str,
-    },
-)
-_OptionalUpdateRecipeJobRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateRecipeJobRequestRequestTypeDef",
-    {
-        "EncryptionKeyArn": str,
-        "EncryptionMode": EncryptionModeType,
-        "LogSubscription": LogSubscriptionType,
-        "MaxCapacity": int,
-        "MaxRetries": int,
-        "Outputs": Sequence[Union[OutputTypeDef, OutputTypeDef]],
-        "DataCatalogOutputs": Sequence[DataCatalogOutputTypeDef],
-        "DatabaseOutputs": Sequence[DatabaseOutputTypeDef],
-        "Timeout": int,
-    },
-    total=False,
-)
-
-class UpdateRecipeJobRequestRequestTypeDef(
-    _RequiredUpdateRecipeJobRequestRequestTypeDef, _OptionalUpdateRecipeJobRequestRequestTypeDef
-):
-    pass
 
+UnionTypeDef = Union[OutputTypeDef, OutputTypeDef]
 _RequiredDatasetTypeDef = TypedDict(
     "_RequiredDatasetTypeDef",
     {
         "Name": str,
         "Input": InputTypeDef,
     },
 )
@@ -2106,17 +2062,19 @@
         "PathOptions": PathOptionsOutputTypeDef,
         "Tags": Dict[str, str],
         "ResourceArn": str,
     },
     total=False,
 )
 
+
 class DatasetTypeDef(_RequiredDatasetTypeDef, _OptionalDatasetTypeDef):
     pass
 
+
 DescribeDatasetResponseTypeDef = TypedDict(
     "DescribeDatasetResponseTypeDef",
     {
         "CreatedBy": str,
         "CreateDate": datetime,
         "Name": str,
         "Format": InputFormatType,
@@ -2146,19 +2104,22 @@
         "FormatOptions": FormatOptionsTypeDef,
         "PathOptions": PathOptionsTypeDef,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateDatasetRequestRequestTypeDef(
     _RequiredCreateDatasetRequestRequestTypeDef, _OptionalCreateDatasetRequestRequestTypeDef
 ):
     pass
 
+
+PathOptionsUnionTypeDef = Union[PathOptionsTypeDef, PathOptionsOutputTypeDef]
 _RequiredUpdateDatasetRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDatasetRequestRequestTypeDef",
     {
         "Name": str,
         "Input": InputTypeDef,
     },
 )
@@ -2168,19 +2129,21 @@
         "Format": InputFormatType,
         "FormatOptions": FormatOptionsTypeDef,
         "PathOptions": PathOptionsTypeDef,
     },
     total=False,
 )
 
+
 class UpdateDatasetRequestRequestTypeDef(
     _RequiredUpdateDatasetRequestRequestTypeDef, _OptionalUpdateDatasetRequestRequestTypeDef
 ):
     pass
 
+
 ListRecipeVersionsResponseTypeDef = TypedDict(
     "ListRecipeVersionsResponseTypeDef",
     {
         "NextToken": str,
         "Recipes": List[RecipeTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2191,14 +2154,105 @@
     {
         "Recipes": List[RecipeTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredCreateRecipeRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateRecipeRequestRequestTypeDef",
+    {
+        "Name": str,
+        "Steps": Sequence[RecipeStepUnionTypeDef],
+    },
+)
+_OptionalCreateRecipeRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateRecipeRequestRequestTypeDef",
+    {
+        "Description": str,
+        "Tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+
+class CreateRecipeRequestRequestTypeDef(
+    _RequiredCreateRecipeRequestRequestTypeDef, _OptionalCreateRecipeRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredUpdateRecipeRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateRecipeRequestRequestTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalUpdateRecipeRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateRecipeRequestRequestTypeDef",
+    {
+        "Description": str,
+        "Steps": Sequence[RecipeStepUnionTypeDef],
+    },
+    total=False,
+)
+
+
+class UpdateRecipeRequestRequestTypeDef(
+    _RequiredUpdateRecipeRequestRequestTypeDef, _OptionalUpdateRecipeRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredCreateRulesetRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateRulesetRequestRequestTypeDef",
+    {
+        "Name": str,
+        "TargetArn": str,
+        "Rules": Sequence[RuleUnionTypeDef],
+    },
+)
+_OptionalCreateRulesetRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateRulesetRequestRequestTypeDef",
+    {
+        "Description": str,
+        "Tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+
+class CreateRulesetRequestRequestTypeDef(
+    _RequiredCreateRulesetRequestRequestTypeDef, _OptionalCreateRulesetRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredUpdateRulesetRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateRulesetRequestRequestTypeDef",
+    {
+        "Name": str,
+        "Rules": Sequence[RuleUnionTypeDef],
+    },
+)
+_OptionalUpdateRulesetRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateRulesetRequestRequestTypeDef",
+    {
+        "Description": str,
+    },
+    total=False,
+)
+
+
+class UpdateRulesetRequestRequestTypeDef(
+    _RequiredUpdateRulesetRequestRequestTypeDef, _OptionalUpdateRulesetRequestRequestTypeDef
+):
+    pass
+
+
 ProfileConfigurationOutputTypeDef = TypedDict(
     "ProfileConfigurationOutputTypeDef",
     {
         "DatasetStatisticsConfiguration": StatisticsConfigurationOutputTypeDef,
         "ProfileColumns": List[ColumnSelectorTypeDef],
         "ColumnStatisticsConfigurations": List[ColumnStatisticsConfigurationOutputTypeDef],
         "EntityDetectorConfiguration": EntityDetectorConfigurationOutputTypeDef,
@@ -2231,14 +2285,78 @@
     {
         "Jobs": List[JobTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredCreateRecipeJobRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateRecipeJobRequestRequestTypeDef",
+    {
+        "Name": str,
+        "RoleArn": str,
+    },
+)
+_OptionalCreateRecipeJobRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateRecipeJobRequestRequestTypeDef",
+    {
+        "DatasetName": str,
+        "EncryptionKeyArn": str,
+        "EncryptionMode": EncryptionModeType,
+        "LogSubscription": LogSubscriptionType,
+        "MaxCapacity": int,
+        "MaxRetries": int,
+        "Outputs": Sequence[UnionTypeDef],
+        "DataCatalogOutputs": Sequence[DataCatalogOutputTypeDef],
+        "DatabaseOutputs": Sequence[DatabaseOutputTypeDef],
+        "ProjectName": str,
+        "RecipeReference": RecipeReferenceTypeDef,
+        "Tags": Mapping[str, str],
+        "Timeout": int,
+    },
+    total=False,
+)
+
+
+class CreateRecipeJobRequestRequestTypeDef(
+    _RequiredCreateRecipeJobRequestRequestTypeDef, _OptionalCreateRecipeJobRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredUpdateRecipeJobRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateRecipeJobRequestRequestTypeDef",
+    {
+        "Name": str,
+        "RoleArn": str,
+    },
+)
+_OptionalUpdateRecipeJobRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateRecipeJobRequestRequestTypeDef",
+    {
+        "EncryptionKeyArn": str,
+        "EncryptionMode": EncryptionModeType,
+        "LogSubscription": LogSubscriptionType,
+        "MaxCapacity": int,
+        "MaxRetries": int,
+        "Outputs": Sequence[UnionTypeDef],
+        "DataCatalogOutputs": Sequence[DataCatalogOutputTypeDef],
+        "DatabaseOutputs": Sequence[DatabaseOutputTypeDef],
+        "Timeout": int,
+    },
+    total=False,
+)
+
+
+class UpdateRecipeJobRequestRequestTypeDef(
+    _RequiredUpdateRecipeJobRequestRequestTypeDef, _OptionalUpdateRecipeJobRequestRequestTypeDef
+):
+    pass
+
+
 ListDatasetsResponseTypeDef = TypedDict(
     "ListDatasetsResponseTypeDef",
     {
         "Datasets": List[DatasetTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2323,19 +2441,24 @@
         "Tags": Mapping[str, str],
         "Timeout": int,
         "JobSample": JobSampleTypeDef,
     },
     total=False,
 )
 
+
 class CreateProfileJobRequestRequestTypeDef(
     _RequiredCreateProfileJobRequestRequestTypeDef, _OptionalCreateProfileJobRequestRequestTypeDef
 ):
     pass
 
+
+ProfileConfigurationUnionTypeDef = Union[
+    ProfileConfigurationTypeDef, ProfileConfigurationOutputTypeDef
+]
 _RequiredUpdateProfileJobRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateProfileJobRequestRequestTypeDef",
     {
         "Name": str,
         "OutputLocation": S3LocationTypeDef,
         "RoleArn": str,
     },
@@ -2352,11 +2475,12 @@
         "ValidationConfigurations": Sequence[ValidationConfigurationTypeDef],
         "Timeout": int,
         "JobSample": JobSampleTypeDef,
     },
     total=False,
 )
 
+
 class UpdateProfileJobRequestRequestTypeDef(
     _RequiredUpdateProfileJobRequestRequestTypeDef, _OptionalUpdateProfileJobRequestRequestTypeDef
 ):
     pass
```

### Comparing `mypy-boto3-databrew-1.28.15.post1/mypy_boto3_databrew.egg-info/PKG-INFO` & `mypy-boto3-databrew-1.28.16/mypy_boto3_databrew.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-databrew
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.GlueDataBrew 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.GlueDataBrew 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 databrew type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 databrew type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-databrew.svg?color=blue)](https://pypi.org/project/mypy-boto3-databrew)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-databrew)](https://pepy.tech/project/mypy-boto3-databrew)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.GlueDataBrew 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew)
+[boto3.GlueDataBrew 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew)
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
 [mypy-boto3-databrew docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/).
 
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
@@ -353,20 +353,20 @@
 )
 
 
 def check_value(value: AnalyticsModeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_databrew.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_databrew.type_defs import (
     AllowedStatisticsOutputTypeDef,
     AllowedStatisticsTypeDef,
     BatchDeleteRecipeVersionRequestRequestTypeDef,
     RecipeVersionErrorDetailTypeDef,
@@ -489,47 +489,53 @@
     InputTypeDef,
     DatabaseOutputTypeDef,
     DataCatalogOutputTypeDef,
     ListProjectsResponseTypeDef,
     OutputTypeDef,
     PathOptionsOutputTypeDef,
     PathOptionsTypeDef,
+    FormatOptionsUnionTypeDef,
     DescribeRecipeResponseTypeDef,
     RecipeTypeDef,
-    CreateRecipeRequestRequestTypeDef,
+    RecipeStepUnionTypeDef,
     SendProjectSessionActionRequestRequestTypeDef,
-    UpdateRecipeRequestRequestTypeDef,
     DescribeRulesetResponseTypeDef,
-    CreateRulesetRequestRequestTypeDef,
-    UpdateRulesetRequestRequestTypeDef,
+    RuleUnionTypeDef,
     ColumnStatisticsConfigurationOutputTypeDef,
     ColumnStatisticsConfigurationTypeDef,
-    CreateRecipeJobRequestRequestTypeDef,
     JobRunTypeDef,
     JobTypeDef,
-    UpdateRecipeJobRequestRequestTypeDef,
+    UnionTypeDef,
     DatasetTypeDef,
     DescribeDatasetResponseTypeDef,
     CreateDatasetRequestRequestTypeDef,
+    PathOptionsUnionTypeDef,
     UpdateDatasetRequestRequestTypeDef,
     ListRecipeVersionsResponseTypeDef,
     ListRecipesResponseTypeDef,
+    CreateRecipeRequestRequestTypeDef,
+    UpdateRecipeRequestRequestTypeDef,
+    CreateRulesetRequestRequestTypeDef,
+    UpdateRulesetRequestRequestTypeDef,
     ProfileConfigurationOutputTypeDef,
     ProfileConfigurationTypeDef,
     ListJobRunsResponseTypeDef,
     ListJobsResponseTypeDef,
+    CreateRecipeJobRequestRequestTypeDef,
+    UpdateRecipeJobRequestRequestTypeDef,
     ListDatasetsResponseTypeDef,
     DescribeJobResponseTypeDef,
     DescribeJobRunResponseTypeDef,
     CreateProfileJobRequestRequestTypeDef,
+    ProfileConfigurationUnionTypeDef,
     UpdateProfileJobRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AllowedStatisticsOutputTypeDef:
+def get_value() -> AllowedStatisticsOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-databrew-1.28.15.post1/mypy_boto3_databrew.egg-info/SOURCES.txt` & `mypy-boto3-databrew-1.28.16/mypy_boto3_databrew.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-databrew-1.28.15.post1/setup.py` & `mypy-boto3-databrew-1.28.16/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-databrew",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_databrew"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.GlueDataBrew 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.2"
+        "Type annotations for boto3.GlueDataBrew 1.28.16 service generated with mypy-boto3-builder"
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
-    keywords="boto3 databrew type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 databrew type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_databrew": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

