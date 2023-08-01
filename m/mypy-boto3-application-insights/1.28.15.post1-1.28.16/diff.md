# Comparing `tmp/mypy-boto3-application-insights-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-application-insights-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-application-insights-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:31 2023, max compression
+gzip compressed data, was "mypy-boto3-application-insights-1.28.16.tar", last modified: Tue Aug  1 11:36:11 2023, max compression
```

## Comparing `mypy-boto3-application-insights-1.28.15.post1.tar` & `mypy-boto3-application-insights-1.28.16.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:31.049007 mypy-boto3-application-insights-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:38:15.000000 mypy-boto3-application-insights-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15508 2023-07-29 10:02:31.045007 mypy-boto3-application-insights-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13964 2023-07-29 09:38:15.000000 mypy-boto3-application-insights-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:31.045007 mypy-boto3-application-insights-1.28.15.post1/mypy_boto3_application_insights/
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-29 09:38:16.000000 mypy-boto3-application-insights-1.28.15.post1/mypy_boto3_application_insights/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-29 09:38:16.000000 mypy-boto3-application-insights-1.28.15.post1/mypy_boto3_application_insights/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-07-29 09:38:16.000000 mypy-boto3-application-insights-1.28.15.post1/mypy_boto3_application_insights/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25282 2023-07-29 09:38:16.000000 mypy-boto3-application-insights-1.28.15.post1/mypy_boto3_application_insights/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    25242 2023-07-29 09:38:16.000000 mypy-boto3-application-insights-1.28.15.post1/mypy_boto3_application_insights/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10128 2023-07-29 09:38:16.000000 mypy-boto3-application-insights-1.28.15.post1/mypy_boto3_application_insights/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10126 2023-07-29 09:38:16.000000 mypy-boto3-application-insights-1.28.15.post1/mypy_boto3_application_insights/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:38:16.000000 mypy-boto3-application-insights-1.28.15.post1/mypy_boto3_application_insights/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    27974 2023-07-29 09:38:17.000000 mypy-boto3-application-insights-1.28.15.post1/mypy_boto3_application_insights/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    27935 2023-07-29 09:38:16.000000 mypy-boto3-application-insights-1.28.15.post1/mypy_boto3_application_insights/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:38:15.000000 mypy-boto3-application-insights-1.28.15.post1/mypy_boto3_application_insights/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:31.045007 mypy-boto3-application-insights-1.28.15.post1/mypy_boto3_application_insights.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15508 2023-07-29 10:02:30.000000 mypy-boto3-application-insights-1.28.15.post1/mypy_boto3_application_insights.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-29 10:02:30.000000 mypy-boto3-application-insights-1.28.15.post1/mypy_boto3_application_insights.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:30.000000 mypy-boto3-application-insights-1.28.15.post1/mypy_boto3_application_insights.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:30.000000 mypy-boto3-application-insights-1.28.15.post1/mypy_boto3_application_insights.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:30.000000 mypy-boto3-application-insights-1.28.15.post1/mypy_boto3_application_insights.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-29 10:02:30.000000 mypy-boto3-application-insights-1.28.15.post1/mypy_boto3_application_insights.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:31.049007 mypy-boto3-application-insights-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-07-29 09:38:15.000000 mypy-boto3-application-insights-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:11.772951 mypy-boto3-application-insights-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:10:47.000000 mypy-boto3-application-insights-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15520 2023-08-01 11:36:11.764950 mypy-boto3-application-insights-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13985 2023-08-01 11:10:47.000000 mypy-boto3-application-insights-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:11.756950 mypy-boto3-application-insights-1.28.16/mypy_boto3_application_insights/
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-08-01 11:10:47.000000 mypy-boto3-application-insights-1.28.16/mypy_boto3_application_insights/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-08-01 11:10:47.000000 mypy-boto3-application-insights-1.28.16/mypy_boto3_application_insights/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-08-01 11:10:47.000000 mypy-boto3-application-insights-1.28.16/mypy_boto3_application_insights/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25251 2023-08-01 11:10:47.000000 mypy-boto3-application-insights-1.28.16/mypy_boto3_application_insights/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25211 2023-08-01 11:10:47.000000 mypy-boto3-application-insights-1.28.16/mypy_boto3_application_insights/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10128 2023-08-01 11:10:47.000000 mypy-boto3-application-insights-1.28.16/mypy_boto3_application_insights/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10126 2023-08-01 11:10:47.000000 mypy-boto3-application-insights-1.28.16/mypy_boto3_application_insights/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:10:47.000000 mypy-boto3-application-insights-1.28.16/mypy_boto3_application_insights/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    28020 2023-08-01 11:10:49.000000 mypy-boto3-application-insights-1.28.16/mypy_boto3_application_insights/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27981 2023-08-01 11:10:47.000000 mypy-boto3-application-insights-1.28.16/mypy_boto3_application_insights/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:10:47.000000 mypy-boto3-application-insights-1.28.16/mypy_boto3_application_insights/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:11.764950 mypy-boto3-application-insights-1.28.16/mypy_boto3_application_insights.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15520 2023-08-01 11:36:11.000000 mypy-boto3-application-insights-1.28.16/mypy_boto3_application_insights.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-08-01 11:36:11.000000 mypy-boto3-application-insights-1.28.16/mypy_boto3_application_insights.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:11.000000 mypy-boto3-application-insights-1.28.16/mypy_boto3_application_insights.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:11.000000 mypy-boto3-application-insights-1.28.16/mypy_boto3_application_insights.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:11.000000 mypy-boto3-application-insights-1.28.16/mypy_boto3_application_insights.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-01 11:36:11.000000 mypy-boto3-application-insights-1.28.16/mypy_boto3_application_insights.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:11.772951 mypy-boto3-application-insights-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-08-01 11:10:46.000000 mypy-boto3-application-insights-1.28.16/setup.py
```

### Comparing `mypy-boto3-application-insights-1.28.15.post1/LICENSE` & `mypy-boto3-application-insights-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-application-insights-1.28.15.post1/PKG-INFO` & `mypy-boto3-application-insights-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-application-insights
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.ApplicationInsights 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.ApplicationInsights 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 application-insights type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 application-insights type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-application-insights.svg?color=blue)](https://pypi.org/project/mypy-boto3-application-insights)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-application-insights)](https://pepy.tech/project/mypy-boto3-application-insights)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ApplicationInsights 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights)
+[boto3.ApplicationInsights 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights)
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
 [mypy-boto3-application-insights docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/).
 
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
@@ -304,20 +304,20 @@
 )
 
 
 def check_value(value: CloudWatchEventSourceType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_application_insights.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_application_insights.type_defs import (
     WorkloadConfigurationTypeDef,
     ResponseMetadataTypeDef,
     ApplicationComponentTypeDef,
     ApplicationInfoTypeDef,
@@ -338,18 +338,17 @@
     ObservationTypeDef,
     DescribeProblemObservationsRequestRequestTypeDef,
     DescribeProblemRequestRequestTypeDef,
     ProblemTypeDef,
     DescribeWorkloadRequestRequestTypeDef,
     ListApplicationsRequestRequestTypeDef,
     ListComponentsRequestRequestTypeDef,
-    ListConfigurationHistoryRequestRequestTypeDef,
+    TimestampTypeDef,
     ListLogPatternSetsRequestRequestTypeDef,
     ListLogPatternsRequestRequestTypeDef,
-    ListProblemsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListWorkloadsRequestRequestTypeDef,
     WorkloadTypeDef,
     RemoveWorkloadRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateApplicationRequestRequestTypeDef,
     UpdateComponentConfigurationRequestRequestTypeDef,
@@ -378,20 +377,22 @@
     DescribeLogPatternResponseTypeDef,
     ListLogPatternsResponseTypeDef,
     UpdateLogPatternResponseTypeDef,
     DescribeObservationResponseTypeDef,
     RelatedObservationsTypeDef,
     DescribeProblemResponseTypeDef,
     ListProblemsResponseTypeDef,
+    ListConfigurationHistoryRequestRequestTypeDef,
+    ListProblemsRequestRequestTypeDef,
     ListWorkloadsResponseTypeDef,
     DescribeProblemObservationsResponseTypeDef,
 )
 
 
-def get_structure() -> WorkloadConfigurationTypeDef:
+def get_value() -> WorkloadConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-application-insights-1.28.15.post1/README.md` & `mypy-boto3-application-insights-1.28.16/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-application-insights.svg?color=blue)](https://pypi.org/project/mypy-boto3-application-insights)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-application-insights)](https://pepy.tech/project/mypy-boto3-application-insights)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ApplicationInsights 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights)
+[boto3.ApplicationInsights 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights)
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
 [mypy-boto3-application-insights docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/).
 
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
@@ -272,20 +272,20 @@
 )
 
 
 def check_value(value: CloudWatchEventSourceType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_application_insights.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_application_insights.type_defs import (
     WorkloadConfigurationTypeDef,
     ResponseMetadataTypeDef,
     ApplicationComponentTypeDef,
     ApplicationInfoTypeDef,
@@ -306,18 +306,17 @@
     ObservationTypeDef,
     DescribeProblemObservationsRequestRequestTypeDef,
     DescribeProblemRequestRequestTypeDef,
     ProblemTypeDef,
     DescribeWorkloadRequestRequestTypeDef,
     ListApplicationsRequestRequestTypeDef,
     ListComponentsRequestRequestTypeDef,
-    ListConfigurationHistoryRequestRequestTypeDef,
+    TimestampTypeDef,
     ListLogPatternSetsRequestRequestTypeDef,
     ListLogPatternsRequestRequestTypeDef,
-    ListProblemsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListWorkloadsRequestRequestTypeDef,
     WorkloadTypeDef,
     RemoveWorkloadRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateApplicationRequestRequestTypeDef,
     UpdateComponentConfigurationRequestRequestTypeDef,
@@ -346,20 +345,22 @@
     DescribeLogPatternResponseTypeDef,
     ListLogPatternsResponseTypeDef,
     UpdateLogPatternResponseTypeDef,
     DescribeObservationResponseTypeDef,
     RelatedObservationsTypeDef,
     DescribeProblemResponseTypeDef,
     ListProblemsResponseTypeDef,
+    ListConfigurationHistoryRequestRequestTypeDef,
+    ListProblemsRequestRequestTypeDef,
     ListWorkloadsResponseTypeDef,
     DescribeProblemObservationsResponseTypeDef,
 )
 
 
-def get_structure() -> WorkloadConfigurationTypeDef:
+def get_value() -> WorkloadConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-application-insights-1.28.15.post1/mypy_boto3_application_insights/__main__.py` & `mypy-boto3-application-insights-1.28.16/mypy_boto3_application_insights/__main__.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ApplicationInsights 1.28.15\nVersion:        "
-        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.ApplicationInsights 1.28.16\nVersion:         1.28.16\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights//\nBoto3 docs:"
         "     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights\nOther"
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

### Comparing `mypy-boto3-application-insights-1.28.15.post1/mypy_boto3_application_insights/client.py` & `mypy-boto3-application-insights-1.28.16/mypy_boto3_application_insights/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from mypy_boto3_application_insights.client import ApplicationInsightsClient
 
     session = Session()
     client: ApplicationInsightsClient = session.client("application-insights")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import ConfigurationEventStatusType, RecommendationTypeType, TierType, VisibilityType
 from .type_defs import (
     AddWorkloadResponseTypeDef,
     CreateApplicationResponseTypeDef,
@@ -38,14 +37,15 @@
     ListConfigurationHistoryResponseTypeDef,
     ListLogPatternSetsResponseTypeDef,
     ListLogPatternsResponseTypeDef,
     ListProblemsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListWorkloadsResponseTypeDef,
     TagTypeDef,
+    TimestampTypeDef,
     UpdateApplicationResponseTypeDef,
     UpdateLogPatternResponseTypeDef,
     UpdateWorkloadResponseTypeDef,
     WorkloadConfigurationTypeDef,
 )
 
 if sys.version_info >= (3, 9):
@@ -330,16 +330,16 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/client/#list_components)
         """
 
     def list_configuration_history(
         self,
         *,
         ResourceGroupName: str = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         EventStatus: ConfigurationEventStatusType = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
         AccountId: str = ...
     ) -> ListConfigurationHistoryResponseTypeDef:
         """
         Lists the INFO, WARN, and ERROR events for periodic configuration updates
@@ -381,16 +381,16 @@
         """
 
     def list_problems(
         self,
         *,
         AccountId: str = ...,
         ResourceGroupName: str = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
         ComponentName: str = ...,
         Visibility: VisibilityType = ...
     ) -> ListProblemsResponseTypeDef:
         """
         Lists the problems with your application.
```

### Comparing `mypy-boto3-application-insights-1.28.15.post1/mypy_boto3_application_insights/client.pyi` & `mypy-boto3-application-insights-1.28.16/mypy_boto3_application_insights/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from mypy_boto3_application_insights.client import ApplicationInsightsClient
 
     session = Session()
     client: ApplicationInsightsClient = session.client("application-insights")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import ConfigurationEventStatusType, RecommendationTypeType, TierType, VisibilityType
 from .type_defs import (
     AddWorkloadResponseTypeDef,
     CreateApplicationResponseTypeDef,
@@ -38,14 +37,15 @@
     ListConfigurationHistoryResponseTypeDef,
     ListLogPatternSetsResponseTypeDef,
     ListLogPatternsResponseTypeDef,
     ListProblemsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListWorkloadsResponseTypeDef,
     TagTypeDef,
+    TimestampTypeDef,
     UpdateApplicationResponseTypeDef,
     UpdateLogPatternResponseTypeDef,
     UpdateWorkloadResponseTypeDef,
     WorkloadConfigurationTypeDef,
 )
 
 if sys.version_info >= (3, 9):
@@ -304,16 +304,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.list_components)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/client/#list_components)
         """
     def list_configuration_history(
         self,
         *,
         ResourceGroupName: str = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         EventStatus: ConfigurationEventStatusType = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
         AccountId: str = ...
     ) -> ListConfigurationHistoryResponseTypeDef:
         """
         Lists the INFO, WARN, and ERROR events for periodic configuration updates
@@ -352,16 +352,16 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/client/#list_log_patterns)
         """
     def list_problems(
         self,
         *,
         AccountId: str = ...,
         ResourceGroupName: str = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
         ComponentName: str = ...,
         Visibility: VisibilityType = ...
     ) -> ListProblemsResponseTypeDef:
         """
         Lists the problems with your application.
```

### Comparing `mypy-boto3-application-insights-1.28.15.post1/mypy_boto3_application_insights/literals.py` & `mypy-boto3-application-insights-1.28.16/mypy_boto3_application_insights/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-application-insights-1.28.15.post1/mypy_boto3_application_insights/literals.pyi` & `mypy-boto3-application-insights-1.28.16/mypy_boto3_application_insights/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-application-insights-1.28.15.post1/mypy_boto3_application_insights/type_defs.py` & `mypy-boto3-application-insights-1.28.16/mypy_boto3_application_insights/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_application_insights.type_defs import WorkloadConfigurationTypeDef
 
-    data: WorkloadConfigurationTypeDef = {...}
+    data: WorkloadConfigurationTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -63,18 +63,17 @@
     "ObservationTypeDef",
     "DescribeProblemObservationsRequestRequestTypeDef",
     "DescribeProblemRequestRequestTypeDef",
     "ProblemTypeDef",
     "DescribeWorkloadRequestRequestTypeDef",
     "ListApplicationsRequestRequestTypeDef",
     "ListComponentsRequestRequestTypeDef",
-    "ListConfigurationHistoryRequestRequestTypeDef",
+    "TimestampTypeDef",
     "ListLogPatternSetsRequestRequestTypeDef",
     "ListLogPatternsRequestRequestTypeDef",
-    "ListProblemsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListWorkloadsRequestRequestTypeDef",
     "WorkloadTypeDef",
     "RemoveWorkloadRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateApplicationRequestRequestTypeDef",
     "UpdateComponentConfigurationRequestRequestTypeDef",
@@ -103,14 +102,16 @@
     "DescribeLogPatternResponseTypeDef",
     "ListLogPatternsResponseTypeDef",
     "UpdateLogPatternResponseTypeDef",
     "DescribeObservationResponseTypeDef",
     "RelatedObservationsTypeDef",
     "DescribeProblemResponseTypeDef",
     "ListProblemsResponseTypeDef",
+    "ListConfigurationHistoryRequestRequestTypeDef",
+    "ListProblemsRequestRequestTypeDef",
     "ListWorkloadsResponseTypeDef",
     "DescribeProblemObservationsResponseTypeDef",
 )
 
 WorkloadConfigurationTypeDef = TypedDict(
     "WorkloadConfigurationTypeDef",
     {
@@ -546,28 +547,15 @@
 
 class ListComponentsRequestRequestTypeDef(
     _RequiredListComponentsRequestRequestTypeDef, _OptionalListComponentsRequestRequestTypeDef
 ):
     pass
 
 
-ListConfigurationHistoryRequestRequestTypeDef = TypedDict(
-    "ListConfigurationHistoryRequestRequestTypeDef",
-    {
-        "ResourceGroupName": str,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "EventStatus": ConfigurationEventStatusType,
-        "MaxResults": int,
-        "NextToken": str,
-        "AccountId": str,
-    },
-    total=False,
-)
-
+TimestampTypeDef = Union[datetime, str]
 _RequiredListLogPatternSetsRequestRequestTypeDef = TypedDict(
     "_RequiredListLogPatternSetsRequestRequestTypeDef",
     {
         "ResourceGroupName": str,
     },
 )
 _OptionalListLogPatternSetsRequestRequestTypeDef = TypedDict(
@@ -608,29 +596,14 @@
 
 class ListLogPatternsRequestRequestTypeDef(
     _RequiredListLogPatternsRequestRequestTypeDef, _OptionalListLogPatternsRequestRequestTypeDef
 ):
     pass
 
 
-ListProblemsRequestRequestTypeDef = TypedDict(
-    "ListProblemsRequestRequestTypeDef",
-    {
-        "AccountId": str,
-        "ResourceGroupName": str,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "MaxResults": int,
-        "NextToken": str,
-        "ComponentName": str,
-        "Visibility": VisibilityType,
-    },
-    total=False,
-)
-
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
     },
 )
 
@@ -1057,14 +1030,43 @@
         "NextToken": str,
         "ResourceGroupName": str,
         "AccountId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListConfigurationHistoryRequestRequestTypeDef = TypedDict(
+    "ListConfigurationHistoryRequestRequestTypeDef",
+    {
+        "ResourceGroupName": str,
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "EventStatus": ConfigurationEventStatusType,
+        "MaxResults": int,
+        "NextToken": str,
+        "AccountId": str,
+    },
+    total=False,
+)
+
+ListProblemsRequestRequestTypeDef = TypedDict(
+    "ListProblemsRequestRequestTypeDef",
+    {
+        "AccountId": str,
+        "ResourceGroupName": str,
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "MaxResults": int,
+        "NextToken": str,
+        "ComponentName": str,
+        "Visibility": VisibilityType,
+    },
+    total=False,
+)
+
 ListWorkloadsResponseTypeDef = TypedDict(
     "ListWorkloadsResponseTypeDef",
     {
         "WorkloadList": List[WorkloadTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-application-insights-1.28.15.post1/mypy_boto3_application_insights/type_defs.pyi` & `mypy-boto3-application-insights-1.28.16/mypy_boto3_application_insights/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_application_insights.type_defs import WorkloadConfigurationTypeDef
 
-    data: WorkloadConfigurationTypeDef = {...}
+    data: WorkloadConfigurationTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -62,18 +62,17 @@
     "ObservationTypeDef",
     "DescribeProblemObservationsRequestRequestTypeDef",
     "DescribeProblemRequestRequestTypeDef",
     "ProblemTypeDef",
     "DescribeWorkloadRequestRequestTypeDef",
     "ListApplicationsRequestRequestTypeDef",
     "ListComponentsRequestRequestTypeDef",
-    "ListConfigurationHistoryRequestRequestTypeDef",
+    "TimestampTypeDef",
     "ListLogPatternSetsRequestRequestTypeDef",
     "ListLogPatternsRequestRequestTypeDef",
-    "ListProblemsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListWorkloadsRequestRequestTypeDef",
     "WorkloadTypeDef",
     "RemoveWorkloadRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateApplicationRequestRequestTypeDef",
     "UpdateComponentConfigurationRequestRequestTypeDef",
@@ -102,14 +101,16 @@
     "DescribeLogPatternResponseTypeDef",
     "ListLogPatternsResponseTypeDef",
     "UpdateLogPatternResponseTypeDef",
     "DescribeObservationResponseTypeDef",
     "RelatedObservationsTypeDef",
     "DescribeProblemResponseTypeDef",
     "ListProblemsResponseTypeDef",
+    "ListConfigurationHistoryRequestRequestTypeDef",
+    "ListProblemsRequestRequestTypeDef",
     "ListWorkloadsResponseTypeDef",
     "DescribeProblemObservationsResponseTypeDef",
 )
 
 WorkloadConfigurationTypeDef = TypedDict(
     "WorkloadConfigurationTypeDef",
     {
@@ -525,28 +526,15 @@
 )
 
 class ListComponentsRequestRequestTypeDef(
     _RequiredListComponentsRequestRequestTypeDef, _OptionalListComponentsRequestRequestTypeDef
 ):
     pass
 
-ListConfigurationHistoryRequestRequestTypeDef = TypedDict(
-    "ListConfigurationHistoryRequestRequestTypeDef",
-    {
-        "ResourceGroupName": str,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "EventStatus": ConfigurationEventStatusType,
-        "MaxResults": int,
-        "NextToken": str,
-        "AccountId": str,
-    },
-    total=False,
-)
-
+TimestampTypeDef = Union[datetime, str]
 _RequiredListLogPatternSetsRequestRequestTypeDef = TypedDict(
     "_RequiredListLogPatternSetsRequestRequestTypeDef",
     {
         "ResourceGroupName": str,
     },
 )
 _OptionalListLogPatternSetsRequestRequestTypeDef = TypedDict(
@@ -583,29 +571,14 @@
 )
 
 class ListLogPatternsRequestRequestTypeDef(
     _RequiredListLogPatternsRequestRequestTypeDef, _OptionalListLogPatternsRequestRequestTypeDef
 ):
     pass
 
-ListProblemsRequestRequestTypeDef = TypedDict(
-    "ListProblemsRequestRequestTypeDef",
-    {
-        "AccountId": str,
-        "ResourceGroupName": str,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "MaxResults": int,
-        "NextToken": str,
-        "ComponentName": str,
-        "Visibility": VisibilityType,
-    },
-    total=False,
-)
-
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
     },
 )
 
@@ -1018,14 +991,43 @@
         "NextToken": str,
         "ResourceGroupName": str,
         "AccountId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListConfigurationHistoryRequestRequestTypeDef = TypedDict(
+    "ListConfigurationHistoryRequestRequestTypeDef",
+    {
+        "ResourceGroupName": str,
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "EventStatus": ConfigurationEventStatusType,
+        "MaxResults": int,
+        "NextToken": str,
+        "AccountId": str,
+    },
+    total=False,
+)
+
+ListProblemsRequestRequestTypeDef = TypedDict(
+    "ListProblemsRequestRequestTypeDef",
+    {
+        "AccountId": str,
+        "ResourceGroupName": str,
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "MaxResults": int,
+        "NextToken": str,
+        "ComponentName": str,
+        "Visibility": VisibilityType,
+    },
+    total=False,
+)
+
 ListWorkloadsResponseTypeDef = TypedDict(
     "ListWorkloadsResponseTypeDef",
     {
         "WorkloadList": List[WorkloadTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-application-insights-1.28.15.post1/mypy_boto3_application_insights.egg-info/PKG-INFO` & `mypy-boto3-application-insights-1.28.16/mypy_boto3_application_insights.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-application-insights
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.ApplicationInsights 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.ApplicationInsights 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 application-insights type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 application-insights type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-application-insights.svg?color=blue)](https://pypi.org/project/mypy-boto3-application-insights)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-application-insights)](https://pepy.tech/project/mypy-boto3-application-insights)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ApplicationInsights 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights)
+[boto3.ApplicationInsights 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights)
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
 [mypy-boto3-application-insights docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/).
 
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
@@ -304,20 +304,20 @@
 )
 
 
 def check_value(value: CloudWatchEventSourceType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_application_insights.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_application_insights.type_defs import (
     WorkloadConfigurationTypeDef,
     ResponseMetadataTypeDef,
     ApplicationComponentTypeDef,
     ApplicationInfoTypeDef,
@@ -338,18 +338,17 @@
     ObservationTypeDef,
     DescribeProblemObservationsRequestRequestTypeDef,
     DescribeProblemRequestRequestTypeDef,
     ProblemTypeDef,
     DescribeWorkloadRequestRequestTypeDef,
     ListApplicationsRequestRequestTypeDef,
     ListComponentsRequestRequestTypeDef,
-    ListConfigurationHistoryRequestRequestTypeDef,
+    TimestampTypeDef,
     ListLogPatternSetsRequestRequestTypeDef,
     ListLogPatternsRequestRequestTypeDef,
-    ListProblemsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListWorkloadsRequestRequestTypeDef,
     WorkloadTypeDef,
     RemoveWorkloadRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateApplicationRequestRequestTypeDef,
     UpdateComponentConfigurationRequestRequestTypeDef,
@@ -378,20 +377,22 @@
     DescribeLogPatternResponseTypeDef,
     ListLogPatternsResponseTypeDef,
     UpdateLogPatternResponseTypeDef,
     DescribeObservationResponseTypeDef,
     RelatedObservationsTypeDef,
     DescribeProblemResponseTypeDef,
     ListProblemsResponseTypeDef,
+    ListConfigurationHistoryRequestRequestTypeDef,
+    ListProblemsRequestRequestTypeDef,
     ListWorkloadsResponseTypeDef,
     DescribeProblemObservationsResponseTypeDef,
 )
 
 
-def get_structure() -> WorkloadConfigurationTypeDef:
+def get_value() -> WorkloadConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-application-insights-1.28.15.post1/mypy_boto3_application_insights.egg-info/SOURCES.txt` & `mypy-boto3-application-insights-1.28.16/mypy_boto3_application_insights.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-application-insights-1.28.15.post1/setup.py` & `mypy-boto3-application-insights-1.28.16/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-application-insights",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_application_insights"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ApplicationInsights 1.28.15 service generated with"
-        " mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.ApplicationInsights 1.28.16 service generated with"
+        " mypy-boto3-builder 7.17.1"
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
-    keywords="boto3 application-insights type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 application-insights type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_application_insights": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/"
```

