# Comparing `tmp/mypy-boto3-swf-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-swf-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-swf-1.28.15.post1.tar", last modified: Sat Jul 29 10:04:20 2023, max compression
+gzip compressed data, was "mypy-boto3-swf-1.28.16.tar", last modified: Tue Aug  1 11:37:59 2023, max compression
```

## Comparing `mypy-boto3-swf-1.28.15.post1.tar` & `mypy-boto3-swf-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:20.169435 mypy-boto3-swf-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 10:00:38.000000 mypy-boto3-swf-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21452 2023-07-29 10:04:20.161435 mypy-boto3-swf-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19975 2023-07-29 10:00:38.000000 mypy-boto3-swf-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:20.157435 mypy-boto3-swf-1.28.15.post1/mypy_boto3_swf/
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-07-29 10:00:38.000000 mypy-boto3-swf-1.28.15.post1/mypy_boto3_swf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-29 10:00:38.000000 mypy-boto3-swf-1.28.15.post1/mypy_boto3_swf/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-29 10:00:38.000000 mypy-boto3-swf-1.28.15.post1/mypy_boto3_swf/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31022 2023-07-29 10:00:38.000000 mypy-boto3-swf-1.28.15.post1/mypy_boto3_swf/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    30971 2023-07-29 10:00:38.000000 mypy-boto3-swf-1.28.15.post1/mypy_boto3_swf/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    16078 2023-07-29 10:00:38.000000 mypy-boto3-swf-1.28.15.post1/mypy_boto3_swf/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    16076 2023-07-29 10:00:38.000000 mypy-boto3-swf-1.28.15.post1/mypy_boto3_swf/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9713 2023-07-29 10:00:38.000000 mypy-boto3-swf-1.28.15.post1/mypy_boto3_swf/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9704 2023-07-29 10:00:38.000000 mypy-boto3-swf-1.28.15.post1/mypy_boto3_swf/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 10:00:38.000000 mypy-boto3-swf-1.28.15.post1/mypy_boto3_swf/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    83888 2023-07-29 10:00:40.000000 mypy-boto3-swf-1.28.15.post1/mypy_boto3_swf/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    83731 2023-07-29 10:00:39.000000 mypy-boto3-swf-1.28.15.post1/mypy_boto3_swf/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 10:00:38.000000 mypy-boto3-swf-1.28.15.post1/mypy_boto3_swf/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:20.161435 mypy-boto3-swf-1.28.15.post1/mypy_boto3_swf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21452 2023-07-29 10:04:19.000000 mypy-boto3-swf-1.28.15.post1/mypy_boto3_swf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-29 10:04:19.000000 mypy-boto3-swf-1.28.15.post1/mypy_boto3_swf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:19.000000 mypy-boto3-swf-1.28.15.post1/mypy_boto3_swf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:19.000000 mypy-boto3-swf-1.28.15.post1/mypy_boto3_swf.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:04:19.000000 mypy-boto3-swf-1.28.15.post1/mypy_boto3_swf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-29 10:04:19.000000 mypy-boto3-swf-1.28.15.post1/mypy_boto3_swf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:04:20.169435 mypy-boto3-swf-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-29 10:00:38.000000 mypy-boto3-swf-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:59.512709 mypy-boto3-swf-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:34:14.000000 mypy-boto3-swf-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21464 2023-08-01 11:37:59.512709 mypy-boto3-swf-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19996 2023-08-01 11:34:14.000000 mypy-boto3-swf-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:59.512709 mypy-boto3-swf-1.28.16/mypy_boto3_swf/
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-08-01 11:34:14.000000 mypy-boto3-swf-1.28.16/mypy_boto3_swf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-08-01 11:34:14.000000 mypy-boto3-swf-1.28.16/mypy_boto3_swf/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-08-01 11:34:14.000000 mypy-boto3-swf-1.28.16/mypy_boto3_swf/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31022 2023-08-01 11:34:14.000000 mypy-boto3-swf-1.28.16/mypy_boto3_swf/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30971 2023-08-01 11:34:14.000000 mypy-boto3-swf-1.28.16/mypy_boto3_swf/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    16078 2023-08-01 11:34:15.000000 mypy-boto3-swf-1.28.16/mypy_boto3_swf/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16076 2023-08-01 11:34:15.000000 mypy-boto3-swf-1.28.16/mypy_boto3_swf/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9713 2023-08-01 11:34:15.000000 mypy-boto3-swf-1.28.16/mypy_boto3_swf/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9704 2023-08-01 11:34:14.000000 mypy-boto3-swf-1.28.16/mypy_boto3_swf/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:34:14.000000 mypy-boto3-swf-1.28.16/mypy_boto3_swf/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    83942 2023-08-01 11:34:21.000000 mypy-boto3-swf-1.28.16/mypy_boto3_swf/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83785 2023-08-01 11:34:16.000000 mypy-boto3-swf-1.28.16/mypy_boto3_swf/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:34:14.000000 mypy-boto3-swf-1.28.16/mypy_boto3_swf/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:59.512709 mypy-boto3-swf-1.28.16/mypy_boto3_swf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21464 2023-08-01 11:37:59.000000 mypy-boto3-swf-1.28.16/mypy_boto3_swf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-08-01 11:37:59.000000 mypy-boto3-swf-1.28.16/mypy_boto3_swf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:59.000000 mypy-boto3-swf-1.28.16/mypy_boto3_swf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:59.000000 mypy-boto3-swf-1.28.16/mypy_boto3_swf.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:59.000000 mypy-boto3-swf-1.28.16/mypy_boto3_swf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-01 11:37:59.000000 mypy-boto3-swf-1.28.16/mypy_boto3_swf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:59.512709 mypy-boto3-swf-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-08-01 11:34:14.000000 mypy-boto3-swf-1.28.16/setup.py
```

### Comparing `mypy-boto3-swf-1.28.15.post1/LICENSE` & `mypy-boto3-swf-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-swf-1.28.15.post1/PKG-INFO` & `mypy-boto3-swf-1.28.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-swf
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.SWF 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.SWF 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_swf/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 swf type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 swf type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-swf.svg?color=blue)](https://pypi.org/project/mypy-boto3-swf)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_swf/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-swf)](https://pepy.tech/project/mypy-boto3-swf)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SWF 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF)
+[boto3.SWF 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF)
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
 [mypy-boto3-swf docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_swf/).
 
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
@@ -366,20 +366,20 @@
 )
 
 
 def check_value(value: ActivityTaskTimeoutTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_swf.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_swf.type_defs import (
     ActivityTaskCancelRequestedEventAttributesTypeDef,
     ActivityTaskCanceledEventAttributesTypeDef,
     ActivityTaskCompletedEventAttributesTypeDef,
     ActivityTaskFailedEventAttributesTypeDef,
@@ -394,15 +394,14 @@
     CancelWorkflowExecutionDecisionAttributesTypeDef,
     CancelWorkflowExecutionFailedEventAttributesTypeDef,
     WorkflowTypeTypeDef,
     CloseStatusFilterTypeDef,
     CompleteWorkflowExecutionDecisionAttributesTypeDef,
     CompleteWorkflowExecutionFailedEventAttributesTypeDef,
     ContinueAsNewWorkflowExecutionFailedEventAttributesTypeDef,
-    ExecutionTimeFilterTypeDef,
     TagFilterTypeDef,
     WorkflowExecutionFilterTypeDef,
     WorkflowTypeFilterTypeDef,
     DecisionTaskCompletedEventAttributesTypeDef,
     DecisionTaskStartedEventAttributesTypeDef,
     DecisionTaskTimedOutEventAttributesTypeDef,
     FailWorkflowExecutionDecisionAttributesTypeDef,
@@ -412,14 +411,15 @@
     ScheduleLambdaFunctionDecisionAttributesTypeDef,
     SignalExternalWorkflowExecutionDecisionAttributesTypeDef,
     StartTimerDecisionAttributesTypeDef,
     DeprecateDomainInputRequestTypeDef,
     DescribeDomainInputRequestTypeDef,
     DomainConfigurationTypeDef,
     DomainInfoTypeDef,
+    TimestampTypeDef,
     FailWorkflowExecutionFailedEventAttributesTypeDef,
     PaginatorConfigTypeDef,
     LambdaFunctionCompletedEventAttributesTypeDef,
     LambdaFunctionFailedEventAttributesTypeDef,
     LambdaFunctionScheduledEventAttributesTypeDef,
     LambdaFunctionStartedEventAttributesTypeDef,
     LambdaFunctionTimedOutEventAttributesTypeDef,
@@ -499,45 +499,46 @@
     StartChildWorkflowExecutionInitiatedEventAttributesTypeDef,
     StartWorkflowExecutionInputRequestTypeDef,
     UndeprecateWorkflowTypeInputRequestTypeDef,
     WorkflowExecutionContinuedAsNewEventAttributesTypeDef,
     WorkflowExecutionInfoTypeDef,
     WorkflowExecutionStartedEventAttributesTypeDef,
     WorkflowTypeInfoTypeDef,
-    CountClosedWorkflowExecutionsInputRequestTypeDef,
-    CountOpenWorkflowExecutionsInputRequestTypeDef,
-    ListClosedWorkflowExecutionsInputRequestTypeDef,
-    ListOpenWorkflowExecutionsInputRequestTypeDef,
     DomainDetailTypeDef,
     DomainInfosTypeDef,
+    ExecutionTimeFilterTypeDef,
     GetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef,
     ListActivityTypesInputListActivityTypesPaginateTypeDef,
-    ListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef,
     ListDomainsInputListDomainsPaginateTypeDef,
-    ListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef,
     ListWorkflowTypesInputListWorkflowTypesPaginateTypeDef,
     PollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef,
     ListTagsForResourceOutputTypeDef,
     RegisterDomainInputRequestTypeDef,
     TagResourceInputRequestTypeDef,
     ActivityTypeInfosTypeDef,
     ActivityTypeDetailTypeDef,
     DecisionTypeDef,
     WorkflowExecutionDetailTypeDef,
     WorkflowExecutionInfosTypeDef,
     HistoryEventTypeDef,
     WorkflowTypeDetailTypeDef,
     WorkflowTypeInfosTypeDef,
+    CountClosedWorkflowExecutionsInputRequestTypeDef,
+    CountOpenWorkflowExecutionsInputRequestTypeDef,
+    ListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef,
+    ListClosedWorkflowExecutionsInputRequestTypeDef,
+    ListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef,
+    ListOpenWorkflowExecutionsInputRequestTypeDef,
     RespondDecisionTaskCompletedInputRequestTypeDef,
     DecisionTaskTypeDef,
     HistoryTypeDef,
 )
 
 
-def get_structure() -> ActivityTaskCancelRequestedEventAttributesTypeDef:
+def get_value() -> ActivityTaskCancelRequestedEventAttributesTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-swf-1.28.15.post1/README.md` & `mypy-boto3-swf-1.28.16/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-swf.svg?color=blue)](https://pypi.org/project/mypy-boto3-swf)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_swf/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-swf)](https://pepy.tech/project/mypy-boto3-swf)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SWF 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF)
+[boto3.SWF 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF)
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
 [mypy-boto3-swf docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_swf/).
 
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
@@ -334,20 +334,20 @@
 )
 
 
 def check_value(value: ActivityTaskTimeoutTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_swf.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_swf.type_defs import (
     ActivityTaskCancelRequestedEventAttributesTypeDef,
     ActivityTaskCanceledEventAttributesTypeDef,
     ActivityTaskCompletedEventAttributesTypeDef,
     ActivityTaskFailedEventAttributesTypeDef,
@@ -362,15 +362,14 @@
     CancelWorkflowExecutionDecisionAttributesTypeDef,
     CancelWorkflowExecutionFailedEventAttributesTypeDef,
     WorkflowTypeTypeDef,
     CloseStatusFilterTypeDef,
     CompleteWorkflowExecutionDecisionAttributesTypeDef,
     CompleteWorkflowExecutionFailedEventAttributesTypeDef,
     ContinueAsNewWorkflowExecutionFailedEventAttributesTypeDef,
-    ExecutionTimeFilterTypeDef,
     TagFilterTypeDef,
     WorkflowExecutionFilterTypeDef,
     WorkflowTypeFilterTypeDef,
     DecisionTaskCompletedEventAttributesTypeDef,
     DecisionTaskStartedEventAttributesTypeDef,
     DecisionTaskTimedOutEventAttributesTypeDef,
     FailWorkflowExecutionDecisionAttributesTypeDef,
@@ -380,14 +379,15 @@
     ScheduleLambdaFunctionDecisionAttributesTypeDef,
     SignalExternalWorkflowExecutionDecisionAttributesTypeDef,
     StartTimerDecisionAttributesTypeDef,
     DeprecateDomainInputRequestTypeDef,
     DescribeDomainInputRequestTypeDef,
     DomainConfigurationTypeDef,
     DomainInfoTypeDef,
+    TimestampTypeDef,
     FailWorkflowExecutionFailedEventAttributesTypeDef,
     PaginatorConfigTypeDef,
     LambdaFunctionCompletedEventAttributesTypeDef,
     LambdaFunctionFailedEventAttributesTypeDef,
     LambdaFunctionScheduledEventAttributesTypeDef,
     LambdaFunctionStartedEventAttributesTypeDef,
     LambdaFunctionTimedOutEventAttributesTypeDef,
@@ -467,45 +467,46 @@
     StartChildWorkflowExecutionInitiatedEventAttributesTypeDef,
     StartWorkflowExecutionInputRequestTypeDef,
     UndeprecateWorkflowTypeInputRequestTypeDef,
     WorkflowExecutionContinuedAsNewEventAttributesTypeDef,
     WorkflowExecutionInfoTypeDef,
     WorkflowExecutionStartedEventAttributesTypeDef,
     WorkflowTypeInfoTypeDef,
-    CountClosedWorkflowExecutionsInputRequestTypeDef,
-    CountOpenWorkflowExecutionsInputRequestTypeDef,
-    ListClosedWorkflowExecutionsInputRequestTypeDef,
-    ListOpenWorkflowExecutionsInputRequestTypeDef,
     DomainDetailTypeDef,
     DomainInfosTypeDef,
+    ExecutionTimeFilterTypeDef,
     GetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef,
     ListActivityTypesInputListActivityTypesPaginateTypeDef,
-    ListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef,
     ListDomainsInputListDomainsPaginateTypeDef,
-    ListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef,
     ListWorkflowTypesInputListWorkflowTypesPaginateTypeDef,
     PollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef,
     ListTagsForResourceOutputTypeDef,
     RegisterDomainInputRequestTypeDef,
     TagResourceInputRequestTypeDef,
     ActivityTypeInfosTypeDef,
     ActivityTypeDetailTypeDef,
     DecisionTypeDef,
     WorkflowExecutionDetailTypeDef,
     WorkflowExecutionInfosTypeDef,
     HistoryEventTypeDef,
     WorkflowTypeDetailTypeDef,
     WorkflowTypeInfosTypeDef,
+    CountClosedWorkflowExecutionsInputRequestTypeDef,
+    CountOpenWorkflowExecutionsInputRequestTypeDef,
+    ListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef,
+    ListClosedWorkflowExecutionsInputRequestTypeDef,
+    ListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef,
+    ListOpenWorkflowExecutionsInputRequestTypeDef,
     RespondDecisionTaskCompletedInputRequestTypeDef,
     DecisionTaskTypeDef,
     HistoryTypeDef,
 )
 
 
-def get_structure() -> ActivityTaskCancelRequestedEventAttributesTypeDef:
+def get_value() -> ActivityTaskCancelRequestedEventAttributesTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-swf-1.28.15.post1/mypy_boto3_swf/__init__.py` & `mypy-boto3-swf-1.28.16/mypy_boto3_swf/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-swf-1.28.15.post1/mypy_boto3_swf/__init__.pyi` & `mypy-boto3-swf-1.28.16/mypy_boto3_swf/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-swf-1.28.15.post1/mypy_boto3_swf/__main__.py` & `mypy-boto3-swf-1.28.16/mypy_boto3_swf/__main__.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SWF 1.28.15\nVersion:         1.28.15.post1\nBuilder version:"
-        " 7.16.2\nDocs:           "
+        "Type annotations for boto3.SWF 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_swf//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF\nOther"
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

### Comparing `mypy-boto3-swf-1.28.15.post1/mypy_boto3_swf/client.py` & `mypy-boto3-swf-1.28.16/mypy_boto3_swf/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-swf-1.28.15.post1/mypy_boto3_swf/client.pyi` & `mypy-boto3-swf-1.28.16/mypy_boto3_swf/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-swf-1.28.15.post1/mypy_boto3_swf/literals.py` & `mypy-boto3-swf-1.28.16/mypy_boto3_swf/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-swf-1.28.15.post1/mypy_boto3_swf/literals.pyi` & `mypy-boto3-swf-1.28.16/mypy_boto3_swf/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-swf-1.28.15.post1/mypy_boto3_swf/paginator.py` & `mypy-boto3-swf-1.28.16/mypy_boto3_swf/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-swf-1.28.15.post1/mypy_boto3_swf/paginator.pyi` & `mypy-boto3-swf-1.28.16/mypy_boto3_swf/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-swf-1.28.15.post1/mypy_boto3_swf/type_defs.py` & `mypy-boto3-swf-1.28.16/mypy_boto3_swf/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_swf/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_swf.type_defs import ActivityTaskCancelRequestedEventAttributesTypeDef
 
-    data: ActivityTaskCancelRequestedEventAttributesTypeDef = {...}
+    data: ActivityTaskCancelRequestedEventAttributesTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -64,15 +64,14 @@
     "CancelWorkflowExecutionDecisionAttributesTypeDef",
     "CancelWorkflowExecutionFailedEventAttributesTypeDef",
     "WorkflowTypeTypeDef",
     "CloseStatusFilterTypeDef",
     "CompleteWorkflowExecutionDecisionAttributesTypeDef",
     "CompleteWorkflowExecutionFailedEventAttributesTypeDef",
     "ContinueAsNewWorkflowExecutionFailedEventAttributesTypeDef",
-    "ExecutionTimeFilterTypeDef",
     "TagFilterTypeDef",
     "WorkflowExecutionFilterTypeDef",
     "WorkflowTypeFilterTypeDef",
     "DecisionTaskCompletedEventAttributesTypeDef",
     "DecisionTaskStartedEventAttributesTypeDef",
     "DecisionTaskTimedOutEventAttributesTypeDef",
     "FailWorkflowExecutionDecisionAttributesTypeDef",
@@ -82,14 +81,15 @@
     "ScheduleLambdaFunctionDecisionAttributesTypeDef",
     "SignalExternalWorkflowExecutionDecisionAttributesTypeDef",
     "StartTimerDecisionAttributesTypeDef",
     "DeprecateDomainInputRequestTypeDef",
     "DescribeDomainInputRequestTypeDef",
     "DomainConfigurationTypeDef",
     "DomainInfoTypeDef",
+    "TimestampTypeDef",
     "FailWorkflowExecutionFailedEventAttributesTypeDef",
     "PaginatorConfigTypeDef",
     "LambdaFunctionCompletedEventAttributesTypeDef",
     "LambdaFunctionFailedEventAttributesTypeDef",
     "LambdaFunctionScheduledEventAttributesTypeDef",
     "LambdaFunctionStartedEventAttributesTypeDef",
     "LambdaFunctionTimedOutEventAttributesTypeDef",
@@ -169,38 +169,39 @@
     "StartChildWorkflowExecutionInitiatedEventAttributesTypeDef",
     "StartWorkflowExecutionInputRequestTypeDef",
     "UndeprecateWorkflowTypeInputRequestTypeDef",
     "WorkflowExecutionContinuedAsNewEventAttributesTypeDef",
     "WorkflowExecutionInfoTypeDef",
     "WorkflowExecutionStartedEventAttributesTypeDef",
     "WorkflowTypeInfoTypeDef",
-    "CountClosedWorkflowExecutionsInputRequestTypeDef",
-    "CountOpenWorkflowExecutionsInputRequestTypeDef",
-    "ListClosedWorkflowExecutionsInputRequestTypeDef",
-    "ListOpenWorkflowExecutionsInputRequestTypeDef",
     "DomainDetailTypeDef",
     "DomainInfosTypeDef",
+    "ExecutionTimeFilterTypeDef",
     "GetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef",
     "ListActivityTypesInputListActivityTypesPaginateTypeDef",
-    "ListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef",
     "ListDomainsInputListDomainsPaginateTypeDef",
-    "ListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef",
     "ListWorkflowTypesInputListWorkflowTypesPaginateTypeDef",
     "PollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef",
     "ListTagsForResourceOutputTypeDef",
     "RegisterDomainInputRequestTypeDef",
     "TagResourceInputRequestTypeDef",
     "ActivityTypeInfosTypeDef",
     "ActivityTypeDetailTypeDef",
     "DecisionTypeDef",
     "WorkflowExecutionDetailTypeDef",
     "WorkflowExecutionInfosTypeDef",
     "HistoryEventTypeDef",
     "WorkflowTypeDetailTypeDef",
     "WorkflowTypeInfosTypeDef",
+    "CountClosedWorkflowExecutionsInputRequestTypeDef",
+    "CountOpenWorkflowExecutionsInputRequestTypeDef",
+    "ListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef",
+    "ListClosedWorkflowExecutionsInputRequestTypeDef",
+    "ListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef",
+    "ListOpenWorkflowExecutionsInputRequestTypeDef",
     "RespondDecisionTaskCompletedInputRequestTypeDef",
     "DecisionTaskTypeDef",
     "HistoryTypeDef",
 )
 
 ActivityTaskCancelRequestedEventAttributesTypeDef = TypedDict(
     "ActivityTaskCancelRequestedEventAttributesTypeDef",
@@ -428,35 +429,14 @@
     "ContinueAsNewWorkflowExecutionFailedEventAttributesTypeDef",
     {
         "cause": ContinueAsNewWorkflowExecutionFailedCauseType,
         "decisionTaskCompletedEventId": int,
     },
 )
 
-_RequiredExecutionTimeFilterTypeDef = TypedDict(
-    "_RequiredExecutionTimeFilterTypeDef",
-    {
-        "oldestDate": Union[datetime, str],
-    },
-)
-_OptionalExecutionTimeFilterTypeDef = TypedDict(
-    "_OptionalExecutionTimeFilterTypeDef",
-    {
-        "latestDate": Union[datetime, str],
-    },
-    total=False,
-)
-
-
-class ExecutionTimeFilterTypeDef(
-    _RequiredExecutionTimeFilterTypeDef, _OptionalExecutionTimeFilterTypeDef
-):
-    pass
-
-
 TagFilterTypeDef = TypedDict(
     "TagFilterTypeDef",
     {
         "tag": str,
     },
 )
 
@@ -712,14 +692,15 @@
 )
 
 
 class DomainInfoTypeDef(_RequiredDomainInfoTypeDef, _OptionalDomainInfoTypeDef):
     pass
 
 
+TimestampTypeDef = Union[datetime, str]
 FailWorkflowExecutionFailedEventAttributesTypeDef = TypedDict(
     "FailWorkflowExecutionFailedEventAttributesTypeDef",
     {
         "cause": FailWorkflowExecutionFailedCauseType,
         "decisionTaskCompletedEventId": int,
     },
 )
@@ -2275,142 +2256,53 @@
 )
 
 
 class WorkflowTypeInfoTypeDef(_RequiredWorkflowTypeInfoTypeDef, _OptionalWorkflowTypeInfoTypeDef):
     pass
 
 
-_RequiredCountClosedWorkflowExecutionsInputRequestTypeDef = TypedDict(
-    "_RequiredCountClosedWorkflowExecutionsInputRequestTypeDef",
-    {
-        "domain": str,
-    },
-)
-_OptionalCountClosedWorkflowExecutionsInputRequestTypeDef = TypedDict(
-    "_OptionalCountClosedWorkflowExecutionsInputRequestTypeDef",
-    {
-        "startTimeFilter": ExecutionTimeFilterTypeDef,
-        "closeTimeFilter": ExecutionTimeFilterTypeDef,
-        "executionFilter": WorkflowExecutionFilterTypeDef,
-        "typeFilter": WorkflowTypeFilterTypeDef,
-        "tagFilter": TagFilterTypeDef,
-        "closeStatusFilter": CloseStatusFilterTypeDef,
-    },
-    total=False,
-)
-
-
-class CountClosedWorkflowExecutionsInputRequestTypeDef(
-    _RequiredCountClosedWorkflowExecutionsInputRequestTypeDef,
-    _OptionalCountClosedWorkflowExecutionsInputRequestTypeDef,
-):
-    pass
-
-
-_RequiredCountOpenWorkflowExecutionsInputRequestTypeDef = TypedDict(
-    "_RequiredCountOpenWorkflowExecutionsInputRequestTypeDef",
-    {
-        "domain": str,
-        "startTimeFilter": ExecutionTimeFilterTypeDef,
-    },
-)
-_OptionalCountOpenWorkflowExecutionsInputRequestTypeDef = TypedDict(
-    "_OptionalCountOpenWorkflowExecutionsInputRequestTypeDef",
+DomainDetailTypeDef = TypedDict(
+    "DomainDetailTypeDef",
     {
-        "typeFilter": WorkflowTypeFilterTypeDef,
-        "tagFilter": TagFilterTypeDef,
-        "executionFilter": WorkflowExecutionFilterTypeDef,
+        "domainInfo": DomainInfoTypeDef,
+        "configuration": DomainConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-
-class CountOpenWorkflowExecutionsInputRequestTypeDef(
-    _RequiredCountOpenWorkflowExecutionsInputRequestTypeDef,
-    _OptionalCountOpenWorkflowExecutionsInputRequestTypeDef,
-):
-    pass
-
-
-_RequiredListClosedWorkflowExecutionsInputRequestTypeDef = TypedDict(
-    "_RequiredListClosedWorkflowExecutionsInputRequestTypeDef",
-    {
-        "domain": str,
-    },
-)
-_OptionalListClosedWorkflowExecutionsInputRequestTypeDef = TypedDict(
-    "_OptionalListClosedWorkflowExecutionsInputRequestTypeDef",
+DomainInfosTypeDef = TypedDict(
+    "DomainInfosTypeDef",
     {
-        "startTimeFilter": ExecutionTimeFilterTypeDef,
-        "closeTimeFilter": ExecutionTimeFilterTypeDef,
-        "executionFilter": WorkflowExecutionFilterTypeDef,
-        "closeStatusFilter": CloseStatusFilterTypeDef,
-        "typeFilter": WorkflowTypeFilterTypeDef,
-        "tagFilter": TagFilterTypeDef,
+        "domainInfos": List[DomainInfoTypeDef],
         "nextPageToken": str,
-        "maximumPageSize": int,
-        "reverseOrder": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-
-class ListClosedWorkflowExecutionsInputRequestTypeDef(
-    _RequiredListClosedWorkflowExecutionsInputRequestTypeDef,
-    _OptionalListClosedWorkflowExecutionsInputRequestTypeDef,
-):
-    pass
-
-
-_RequiredListOpenWorkflowExecutionsInputRequestTypeDef = TypedDict(
-    "_RequiredListOpenWorkflowExecutionsInputRequestTypeDef",
+_RequiredExecutionTimeFilterTypeDef = TypedDict(
+    "_RequiredExecutionTimeFilterTypeDef",
     {
-        "domain": str,
-        "startTimeFilter": ExecutionTimeFilterTypeDef,
+        "oldestDate": TimestampTypeDef,
     },
 )
-_OptionalListOpenWorkflowExecutionsInputRequestTypeDef = TypedDict(
-    "_OptionalListOpenWorkflowExecutionsInputRequestTypeDef",
+_OptionalExecutionTimeFilterTypeDef = TypedDict(
+    "_OptionalExecutionTimeFilterTypeDef",
     {
-        "typeFilter": WorkflowTypeFilterTypeDef,
-        "tagFilter": TagFilterTypeDef,
-        "nextPageToken": str,
-        "maximumPageSize": int,
-        "reverseOrder": bool,
-        "executionFilter": WorkflowExecutionFilterTypeDef,
+        "latestDate": TimestampTypeDef,
     },
     total=False,
 )
 
 
-class ListOpenWorkflowExecutionsInputRequestTypeDef(
-    _RequiredListOpenWorkflowExecutionsInputRequestTypeDef,
-    _OptionalListOpenWorkflowExecutionsInputRequestTypeDef,
+class ExecutionTimeFilterTypeDef(
+    _RequiredExecutionTimeFilterTypeDef, _OptionalExecutionTimeFilterTypeDef
 ):
     pass
 
 
-DomainDetailTypeDef = TypedDict(
-    "DomainDetailTypeDef",
-    {
-        "domainInfo": DomainInfoTypeDef,
-        "configuration": DomainConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DomainInfosTypeDef = TypedDict(
-    "DomainInfosTypeDef",
-    {
-        "domainInfos": List[DomainInfoTypeDef],
-        "nextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredGetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef = TypedDict(
     "_RequiredGetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef",
     {
         "domain": str,
         "execution": WorkflowExecutionTypeDef,
     },
 )
@@ -2452,43 +2344,14 @@
 class ListActivityTypesInputListActivityTypesPaginateTypeDef(
     _RequiredListActivityTypesInputListActivityTypesPaginateTypeDef,
     _OptionalListActivityTypesInputListActivityTypesPaginateTypeDef,
 ):
     pass
 
 
-_RequiredListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef = TypedDict(
-    "_RequiredListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef",
-    {
-        "domain": str,
-    },
-)
-_OptionalListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef = TypedDict(
-    "_OptionalListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef",
-    {
-        "startTimeFilter": ExecutionTimeFilterTypeDef,
-        "closeTimeFilter": ExecutionTimeFilterTypeDef,
-        "executionFilter": WorkflowExecutionFilterTypeDef,
-        "closeStatusFilter": CloseStatusFilterTypeDef,
-        "typeFilter": WorkflowTypeFilterTypeDef,
-        "tagFilter": TagFilterTypeDef,
-        "reverseOrder": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef(
-    _RequiredListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef,
-    _OptionalListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListDomainsInputListDomainsPaginateTypeDef = TypedDict(
     "_RequiredListDomainsInputListDomainsPaginateTypeDef",
     {
         "registrationStatus": RegistrationStatusType,
     },
 )
 _OptionalListDomainsInputListDomainsPaginateTypeDef = TypedDict(
@@ -2504,41 +2367,14 @@
 class ListDomainsInputListDomainsPaginateTypeDef(
     _RequiredListDomainsInputListDomainsPaginateTypeDef,
     _OptionalListDomainsInputListDomainsPaginateTypeDef,
 ):
     pass
 
 
-_RequiredListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef = TypedDict(
-    "_RequiredListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef",
-    {
-        "domain": str,
-        "startTimeFilter": ExecutionTimeFilterTypeDef,
-    },
-)
-_OptionalListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef = TypedDict(
-    "_OptionalListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef",
-    {
-        "typeFilter": WorkflowTypeFilterTypeDef,
-        "tagFilter": TagFilterTypeDef,
-        "reverseOrder": bool,
-        "executionFilter": WorkflowExecutionFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef(
-    _RequiredListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef,
-    _OptionalListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListWorkflowTypesInputListWorkflowTypesPaginateTypeDef = TypedDict(
     "_RequiredListWorkflowTypesInputListWorkflowTypesPaginateTypeDef",
     {
         "domain": str,
         "registrationStatus": RegistrationStatusType,
     },
 )
@@ -2849,14 +2685,180 @@
     {
         "typeInfos": List[WorkflowTypeInfoTypeDef],
         "nextPageToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredCountClosedWorkflowExecutionsInputRequestTypeDef = TypedDict(
+    "_RequiredCountClosedWorkflowExecutionsInputRequestTypeDef",
+    {
+        "domain": str,
+    },
+)
+_OptionalCountClosedWorkflowExecutionsInputRequestTypeDef = TypedDict(
+    "_OptionalCountClosedWorkflowExecutionsInputRequestTypeDef",
+    {
+        "startTimeFilter": ExecutionTimeFilterTypeDef,
+        "closeTimeFilter": ExecutionTimeFilterTypeDef,
+        "executionFilter": WorkflowExecutionFilterTypeDef,
+        "typeFilter": WorkflowTypeFilterTypeDef,
+        "tagFilter": TagFilterTypeDef,
+        "closeStatusFilter": CloseStatusFilterTypeDef,
+    },
+    total=False,
+)
+
+
+class CountClosedWorkflowExecutionsInputRequestTypeDef(
+    _RequiredCountClosedWorkflowExecutionsInputRequestTypeDef,
+    _OptionalCountClosedWorkflowExecutionsInputRequestTypeDef,
+):
+    pass
+
+
+_RequiredCountOpenWorkflowExecutionsInputRequestTypeDef = TypedDict(
+    "_RequiredCountOpenWorkflowExecutionsInputRequestTypeDef",
+    {
+        "domain": str,
+        "startTimeFilter": ExecutionTimeFilterTypeDef,
+    },
+)
+_OptionalCountOpenWorkflowExecutionsInputRequestTypeDef = TypedDict(
+    "_OptionalCountOpenWorkflowExecutionsInputRequestTypeDef",
+    {
+        "typeFilter": WorkflowTypeFilterTypeDef,
+        "tagFilter": TagFilterTypeDef,
+        "executionFilter": WorkflowExecutionFilterTypeDef,
+    },
+    total=False,
+)
+
+
+class CountOpenWorkflowExecutionsInputRequestTypeDef(
+    _RequiredCountOpenWorkflowExecutionsInputRequestTypeDef,
+    _OptionalCountOpenWorkflowExecutionsInputRequestTypeDef,
+):
+    pass
+
+
+_RequiredListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef = TypedDict(
+    "_RequiredListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef",
+    {
+        "domain": str,
+    },
+)
+_OptionalListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef = TypedDict(
+    "_OptionalListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef",
+    {
+        "startTimeFilter": ExecutionTimeFilterTypeDef,
+        "closeTimeFilter": ExecutionTimeFilterTypeDef,
+        "executionFilter": WorkflowExecutionFilterTypeDef,
+        "closeStatusFilter": CloseStatusFilterTypeDef,
+        "typeFilter": WorkflowTypeFilterTypeDef,
+        "tagFilter": TagFilterTypeDef,
+        "reverseOrder": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef(
+    _RequiredListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef,
+    _OptionalListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListClosedWorkflowExecutionsInputRequestTypeDef = TypedDict(
+    "_RequiredListClosedWorkflowExecutionsInputRequestTypeDef",
+    {
+        "domain": str,
+    },
+)
+_OptionalListClosedWorkflowExecutionsInputRequestTypeDef = TypedDict(
+    "_OptionalListClosedWorkflowExecutionsInputRequestTypeDef",
+    {
+        "startTimeFilter": ExecutionTimeFilterTypeDef,
+        "closeTimeFilter": ExecutionTimeFilterTypeDef,
+        "executionFilter": WorkflowExecutionFilterTypeDef,
+        "closeStatusFilter": CloseStatusFilterTypeDef,
+        "typeFilter": WorkflowTypeFilterTypeDef,
+        "tagFilter": TagFilterTypeDef,
+        "nextPageToken": str,
+        "maximumPageSize": int,
+        "reverseOrder": bool,
+    },
+    total=False,
+)
+
+
+class ListClosedWorkflowExecutionsInputRequestTypeDef(
+    _RequiredListClosedWorkflowExecutionsInputRequestTypeDef,
+    _OptionalListClosedWorkflowExecutionsInputRequestTypeDef,
+):
+    pass
+
+
+_RequiredListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef = TypedDict(
+    "_RequiredListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef",
+    {
+        "domain": str,
+        "startTimeFilter": ExecutionTimeFilterTypeDef,
+    },
+)
+_OptionalListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef = TypedDict(
+    "_OptionalListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef",
+    {
+        "typeFilter": WorkflowTypeFilterTypeDef,
+        "tagFilter": TagFilterTypeDef,
+        "reverseOrder": bool,
+        "executionFilter": WorkflowExecutionFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef(
+    _RequiredListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef,
+    _OptionalListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListOpenWorkflowExecutionsInputRequestTypeDef = TypedDict(
+    "_RequiredListOpenWorkflowExecutionsInputRequestTypeDef",
+    {
+        "domain": str,
+        "startTimeFilter": ExecutionTimeFilterTypeDef,
+    },
+)
+_OptionalListOpenWorkflowExecutionsInputRequestTypeDef = TypedDict(
+    "_OptionalListOpenWorkflowExecutionsInputRequestTypeDef",
+    {
+        "typeFilter": WorkflowTypeFilterTypeDef,
+        "tagFilter": TagFilterTypeDef,
+        "nextPageToken": str,
+        "maximumPageSize": int,
+        "reverseOrder": bool,
+        "executionFilter": WorkflowExecutionFilterTypeDef,
+    },
+    total=False,
+)
+
+
+class ListOpenWorkflowExecutionsInputRequestTypeDef(
+    _RequiredListOpenWorkflowExecutionsInputRequestTypeDef,
+    _OptionalListOpenWorkflowExecutionsInputRequestTypeDef,
+):
+    pass
+
+
 _RequiredRespondDecisionTaskCompletedInputRequestTypeDef = TypedDict(
     "_RequiredRespondDecisionTaskCompletedInputRequestTypeDef",
     {
         "taskToken": str,
     },
 )
 _OptionalRespondDecisionTaskCompletedInputRequestTypeDef = TypedDict(
```

### Comparing `mypy-boto3-swf-1.28.15.post1/mypy_boto3_swf/type_defs.pyi` & `mypy-boto3-swf-1.28.16/mypy_boto3_swf/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_swf/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_swf.type_defs import ActivityTaskCancelRequestedEventAttributesTypeDef
 
-    data: ActivityTaskCancelRequestedEventAttributesTypeDef = {...}
+    data: ActivityTaskCancelRequestedEventAttributesTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -63,15 +63,14 @@
     "CancelWorkflowExecutionDecisionAttributesTypeDef",
     "CancelWorkflowExecutionFailedEventAttributesTypeDef",
     "WorkflowTypeTypeDef",
     "CloseStatusFilterTypeDef",
     "CompleteWorkflowExecutionDecisionAttributesTypeDef",
     "CompleteWorkflowExecutionFailedEventAttributesTypeDef",
     "ContinueAsNewWorkflowExecutionFailedEventAttributesTypeDef",
-    "ExecutionTimeFilterTypeDef",
     "TagFilterTypeDef",
     "WorkflowExecutionFilterTypeDef",
     "WorkflowTypeFilterTypeDef",
     "DecisionTaskCompletedEventAttributesTypeDef",
     "DecisionTaskStartedEventAttributesTypeDef",
     "DecisionTaskTimedOutEventAttributesTypeDef",
     "FailWorkflowExecutionDecisionAttributesTypeDef",
@@ -81,14 +80,15 @@
     "ScheduleLambdaFunctionDecisionAttributesTypeDef",
     "SignalExternalWorkflowExecutionDecisionAttributesTypeDef",
     "StartTimerDecisionAttributesTypeDef",
     "DeprecateDomainInputRequestTypeDef",
     "DescribeDomainInputRequestTypeDef",
     "DomainConfigurationTypeDef",
     "DomainInfoTypeDef",
+    "TimestampTypeDef",
     "FailWorkflowExecutionFailedEventAttributesTypeDef",
     "PaginatorConfigTypeDef",
     "LambdaFunctionCompletedEventAttributesTypeDef",
     "LambdaFunctionFailedEventAttributesTypeDef",
     "LambdaFunctionScheduledEventAttributesTypeDef",
     "LambdaFunctionStartedEventAttributesTypeDef",
     "LambdaFunctionTimedOutEventAttributesTypeDef",
@@ -168,38 +168,39 @@
     "StartChildWorkflowExecutionInitiatedEventAttributesTypeDef",
     "StartWorkflowExecutionInputRequestTypeDef",
     "UndeprecateWorkflowTypeInputRequestTypeDef",
     "WorkflowExecutionContinuedAsNewEventAttributesTypeDef",
     "WorkflowExecutionInfoTypeDef",
     "WorkflowExecutionStartedEventAttributesTypeDef",
     "WorkflowTypeInfoTypeDef",
-    "CountClosedWorkflowExecutionsInputRequestTypeDef",
-    "CountOpenWorkflowExecutionsInputRequestTypeDef",
-    "ListClosedWorkflowExecutionsInputRequestTypeDef",
-    "ListOpenWorkflowExecutionsInputRequestTypeDef",
     "DomainDetailTypeDef",
     "DomainInfosTypeDef",
+    "ExecutionTimeFilterTypeDef",
     "GetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef",
     "ListActivityTypesInputListActivityTypesPaginateTypeDef",
-    "ListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef",
     "ListDomainsInputListDomainsPaginateTypeDef",
-    "ListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef",
     "ListWorkflowTypesInputListWorkflowTypesPaginateTypeDef",
     "PollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef",
     "ListTagsForResourceOutputTypeDef",
     "RegisterDomainInputRequestTypeDef",
     "TagResourceInputRequestTypeDef",
     "ActivityTypeInfosTypeDef",
     "ActivityTypeDetailTypeDef",
     "DecisionTypeDef",
     "WorkflowExecutionDetailTypeDef",
     "WorkflowExecutionInfosTypeDef",
     "HistoryEventTypeDef",
     "WorkflowTypeDetailTypeDef",
     "WorkflowTypeInfosTypeDef",
+    "CountClosedWorkflowExecutionsInputRequestTypeDef",
+    "CountOpenWorkflowExecutionsInputRequestTypeDef",
+    "ListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef",
+    "ListClosedWorkflowExecutionsInputRequestTypeDef",
+    "ListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef",
+    "ListOpenWorkflowExecutionsInputRequestTypeDef",
     "RespondDecisionTaskCompletedInputRequestTypeDef",
     "DecisionTaskTypeDef",
     "HistoryTypeDef",
 )
 
 ActivityTaskCancelRequestedEventAttributesTypeDef = TypedDict(
     "ActivityTaskCancelRequestedEventAttributesTypeDef",
@@ -417,33 +418,14 @@
     "ContinueAsNewWorkflowExecutionFailedEventAttributesTypeDef",
     {
         "cause": ContinueAsNewWorkflowExecutionFailedCauseType,
         "decisionTaskCompletedEventId": int,
     },
 )
 
-_RequiredExecutionTimeFilterTypeDef = TypedDict(
-    "_RequiredExecutionTimeFilterTypeDef",
-    {
-        "oldestDate": Union[datetime, str],
-    },
-)
-_OptionalExecutionTimeFilterTypeDef = TypedDict(
-    "_OptionalExecutionTimeFilterTypeDef",
-    {
-        "latestDate": Union[datetime, str],
-    },
-    total=False,
-)
-
-class ExecutionTimeFilterTypeDef(
-    _RequiredExecutionTimeFilterTypeDef, _OptionalExecutionTimeFilterTypeDef
-):
-    pass
-
 TagFilterTypeDef = TypedDict(
     "TagFilterTypeDef",
     {
         "tag": str,
     },
 )
 
@@ -681,14 +663,15 @@
     },
     total=False,
 )
 
 class DomainInfoTypeDef(_RequiredDomainInfoTypeDef, _OptionalDomainInfoTypeDef):
     pass
 
+TimestampTypeDef = Union[datetime, str]
 FailWorkflowExecutionFailedEventAttributesTypeDef = TypedDict(
     "FailWorkflowExecutionFailedEventAttributesTypeDef",
     {
         "cause": FailWorkflowExecutionFailedCauseType,
         "decisionTaskCompletedEventId": int,
     },
 )
@@ -2148,134 +2131,51 @@
     },
     total=False,
 )
 
 class WorkflowTypeInfoTypeDef(_RequiredWorkflowTypeInfoTypeDef, _OptionalWorkflowTypeInfoTypeDef):
     pass
 
-_RequiredCountClosedWorkflowExecutionsInputRequestTypeDef = TypedDict(
-    "_RequiredCountClosedWorkflowExecutionsInputRequestTypeDef",
-    {
-        "domain": str,
-    },
-)
-_OptionalCountClosedWorkflowExecutionsInputRequestTypeDef = TypedDict(
-    "_OptionalCountClosedWorkflowExecutionsInputRequestTypeDef",
-    {
-        "startTimeFilter": ExecutionTimeFilterTypeDef,
-        "closeTimeFilter": ExecutionTimeFilterTypeDef,
-        "executionFilter": WorkflowExecutionFilterTypeDef,
-        "typeFilter": WorkflowTypeFilterTypeDef,
-        "tagFilter": TagFilterTypeDef,
-        "closeStatusFilter": CloseStatusFilterTypeDef,
-    },
-    total=False,
-)
-
-class CountClosedWorkflowExecutionsInputRequestTypeDef(
-    _RequiredCountClosedWorkflowExecutionsInputRequestTypeDef,
-    _OptionalCountClosedWorkflowExecutionsInputRequestTypeDef,
-):
-    pass
-
-_RequiredCountOpenWorkflowExecutionsInputRequestTypeDef = TypedDict(
-    "_RequiredCountOpenWorkflowExecutionsInputRequestTypeDef",
-    {
-        "domain": str,
-        "startTimeFilter": ExecutionTimeFilterTypeDef,
-    },
-)
-_OptionalCountOpenWorkflowExecutionsInputRequestTypeDef = TypedDict(
-    "_OptionalCountOpenWorkflowExecutionsInputRequestTypeDef",
+DomainDetailTypeDef = TypedDict(
+    "DomainDetailTypeDef",
     {
-        "typeFilter": WorkflowTypeFilterTypeDef,
-        "tagFilter": TagFilterTypeDef,
-        "executionFilter": WorkflowExecutionFilterTypeDef,
+        "domainInfo": DomainInfoTypeDef,
+        "configuration": DomainConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class CountOpenWorkflowExecutionsInputRequestTypeDef(
-    _RequiredCountOpenWorkflowExecutionsInputRequestTypeDef,
-    _OptionalCountOpenWorkflowExecutionsInputRequestTypeDef,
-):
-    pass
-
-_RequiredListClosedWorkflowExecutionsInputRequestTypeDef = TypedDict(
-    "_RequiredListClosedWorkflowExecutionsInputRequestTypeDef",
-    {
-        "domain": str,
-    },
-)
-_OptionalListClosedWorkflowExecutionsInputRequestTypeDef = TypedDict(
-    "_OptionalListClosedWorkflowExecutionsInputRequestTypeDef",
+DomainInfosTypeDef = TypedDict(
+    "DomainInfosTypeDef",
     {
-        "startTimeFilter": ExecutionTimeFilterTypeDef,
-        "closeTimeFilter": ExecutionTimeFilterTypeDef,
-        "executionFilter": WorkflowExecutionFilterTypeDef,
-        "closeStatusFilter": CloseStatusFilterTypeDef,
-        "typeFilter": WorkflowTypeFilterTypeDef,
-        "tagFilter": TagFilterTypeDef,
+        "domainInfos": List[DomainInfoTypeDef],
         "nextPageToken": str,
-        "maximumPageSize": int,
-        "reverseOrder": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class ListClosedWorkflowExecutionsInputRequestTypeDef(
-    _RequiredListClosedWorkflowExecutionsInputRequestTypeDef,
-    _OptionalListClosedWorkflowExecutionsInputRequestTypeDef,
-):
-    pass
-
-_RequiredListOpenWorkflowExecutionsInputRequestTypeDef = TypedDict(
-    "_RequiredListOpenWorkflowExecutionsInputRequestTypeDef",
+_RequiredExecutionTimeFilterTypeDef = TypedDict(
+    "_RequiredExecutionTimeFilterTypeDef",
     {
-        "domain": str,
-        "startTimeFilter": ExecutionTimeFilterTypeDef,
+        "oldestDate": TimestampTypeDef,
     },
 )
-_OptionalListOpenWorkflowExecutionsInputRequestTypeDef = TypedDict(
-    "_OptionalListOpenWorkflowExecutionsInputRequestTypeDef",
+_OptionalExecutionTimeFilterTypeDef = TypedDict(
+    "_OptionalExecutionTimeFilterTypeDef",
     {
-        "typeFilter": WorkflowTypeFilterTypeDef,
-        "tagFilter": TagFilterTypeDef,
-        "nextPageToken": str,
-        "maximumPageSize": int,
-        "reverseOrder": bool,
-        "executionFilter": WorkflowExecutionFilterTypeDef,
+        "latestDate": TimestampTypeDef,
     },
     total=False,
 )
 
-class ListOpenWorkflowExecutionsInputRequestTypeDef(
-    _RequiredListOpenWorkflowExecutionsInputRequestTypeDef,
-    _OptionalListOpenWorkflowExecutionsInputRequestTypeDef,
+class ExecutionTimeFilterTypeDef(
+    _RequiredExecutionTimeFilterTypeDef, _OptionalExecutionTimeFilterTypeDef
 ):
     pass
 
-DomainDetailTypeDef = TypedDict(
-    "DomainDetailTypeDef",
-    {
-        "domainInfo": DomainInfoTypeDef,
-        "configuration": DomainConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DomainInfosTypeDef = TypedDict(
-    "DomainInfosTypeDef",
-    {
-        "domainInfos": List[DomainInfoTypeDef],
-        "nextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredGetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef = TypedDict(
     "_RequiredGetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef",
     {
         "domain": str,
         "execution": WorkflowExecutionTypeDef,
     },
 )
@@ -2313,41 +2213,14 @@
 
 class ListActivityTypesInputListActivityTypesPaginateTypeDef(
     _RequiredListActivityTypesInputListActivityTypesPaginateTypeDef,
     _OptionalListActivityTypesInputListActivityTypesPaginateTypeDef,
 ):
     pass
 
-_RequiredListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef = TypedDict(
-    "_RequiredListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef",
-    {
-        "domain": str,
-    },
-)
-_OptionalListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef = TypedDict(
-    "_OptionalListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef",
-    {
-        "startTimeFilter": ExecutionTimeFilterTypeDef,
-        "closeTimeFilter": ExecutionTimeFilterTypeDef,
-        "executionFilter": WorkflowExecutionFilterTypeDef,
-        "closeStatusFilter": CloseStatusFilterTypeDef,
-        "typeFilter": WorkflowTypeFilterTypeDef,
-        "tagFilter": TagFilterTypeDef,
-        "reverseOrder": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef(
-    _RequiredListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef,
-    _OptionalListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef,
-):
-    pass
-
 _RequiredListDomainsInputListDomainsPaginateTypeDef = TypedDict(
     "_RequiredListDomainsInputListDomainsPaginateTypeDef",
     {
         "registrationStatus": RegistrationStatusType,
     },
 )
 _OptionalListDomainsInputListDomainsPaginateTypeDef = TypedDict(
@@ -2361,39 +2234,14 @@
 
 class ListDomainsInputListDomainsPaginateTypeDef(
     _RequiredListDomainsInputListDomainsPaginateTypeDef,
     _OptionalListDomainsInputListDomainsPaginateTypeDef,
 ):
     pass
 
-_RequiredListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef = TypedDict(
-    "_RequiredListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef",
-    {
-        "domain": str,
-        "startTimeFilter": ExecutionTimeFilterTypeDef,
-    },
-)
-_OptionalListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef = TypedDict(
-    "_OptionalListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef",
-    {
-        "typeFilter": WorkflowTypeFilterTypeDef,
-        "tagFilter": TagFilterTypeDef,
-        "reverseOrder": bool,
-        "executionFilter": WorkflowExecutionFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef(
-    _RequiredListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef,
-    _OptionalListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef,
-):
-    pass
-
 _RequiredListWorkflowTypesInputListWorkflowTypesPaginateTypeDef = TypedDict(
     "_RequiredListWorkflowTypesInputListWorkflowTypesPaginateTypeDef",
     {
         "domain": str,
         "registrationStatus": RegistrationStatusType,
     },
 )
@@ -2694,14 +2542,168 @@
     {
         "typeInfos": List[WorkflowTypeInfoTypeDef],
         "nextPageToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredCountClosedWorkflowExecutionsInputRequestTypeDef = TypedDict(
+    "_RequiredCountClosedWorkflowExecutionsInputRequestTypeDef",
+    {
+        "domain": str,
+    },
+)
+_OptionalCountClosedWorkflowExecutionsInputRequestTypeDef = TypedDict(
+    "_OptionalCountClosedWorkflowExecutionsInputRequestTypeDef",
+    {
+        "startTimeFilter": ExecutionTimeFilterTypeDef,
+        "closeTimeFilter": ExecutionTimeFilterTypeDef,
+        "executionFilter": WorkflowExecutionFilterTypeDef,
+        "typeFilter": WorkflowTypeFilterTypeDef,
+        "tagFilter": TagFilterTypeDef,
+        "closeStatusFilter": CloseStatusFilterTypeDef,
+    },
+    total=False,
+)
+
+class CountClosedWorkflowExecutionsInputRequestTypeDef(
+    _RequiredCountClosedWorkflowExecutionsInputRequestTypeDef,
+    _OptionalCountClosedWorkflowExecutionsInputRequestTypeDef,
+):
+    pass
+
+_RequiredCountOpenWorkflowExecutionsInputRequestTypeDef = TypedDict(
+    "_RequiredCountOpenWorkflowExecutionsInputRequestTypeDef",
+    {
+        "domain": str,
+        "startTimeFilter": ExecutionTimeFilterTypeDef,
+    },
+)
+_OptionalCountOpenWorkflowExecutionsInputRequestTypeDef = TypedDict(
+    "_OptionalCountOpenWorkflowExecutionsInputRequestTypeDef",
+    {
+        "typeFilter": WorkflowTypeFilterTypeDef,
+        "tagFilter": TagFilterTypeDef,
+        "executionFilter": WorkflowExecutionFilterTypeDef,
+    },
+    total=False,
+)
+
+class CountOpenWorkflowExecutionsInputRequestTypeDef(
+    _RequiredCountOpenWorkflowExecutionsInputRequestTypeDef,
+    _OptionalCountOpenWorkflowExecutionsInputRequestTypeDef,
+):
+    pass
+
+_RequiredListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef = TypedDict(
+    "_RequiredListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef",
+    {
+        "domain": str,
+    },
+)
+_OptionalListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef = TypedDict(
+    "_OptionalListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef",
+    {
+        "startTimeFilter": ExecutionTimeFilterTypeDef,
+        "closeTimeFilter": ExecutionTimeFilterTypeDef,
+        "executionFilter": WorkflowExecutionFilterTypeDef,
+        "closeStatusFilter": CloseStatusFilterTypeDef,
+        "typeFilter": WorkflowTypeFilterTypeDef,
+        "tagFilter": TagFilterTypeDef,
+        "reverseOrder": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef(
+    _RequiredListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef,
+    _OptionalListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef,
+):
+    pass
+
+_RequiredListClosedWorkflowExecutionsInputRequestTypeDef = TypedDict(
+    "_RequiredListClosedWorkflowExecutionsInputRequestTypeDef",
+    {
+        "domain": str,
+    },
+)
+_OptionalListClosedWorkflowExecutionsInputRequestTypeDef = TypedDict(
+    "_OptionalListClosedWorkflowExecutionsInputRequestTypeDef",
+    {
+        "startTimeFilter": ExecutionTimeFilterTypeDef,
+        "closeTimeFilter": ExecutionTimeFilterTypeDef,
+        "executionFilter": WorkflowExecutionFilterTypeDef,
+        "closeStatusFilter": CloseStatusFilterTypeDef,
+        "typeFilter": WorkflowTypeFilterTypeDef,
+        "tagFilter": TagFilterTypeDef,
+        "nextPageToken": str,
+        "maximumPageSize": int,
+        "reverseOrder": bool,
+    },
+    total=False,
+)
+
+class ListClosedWorkflowExecutionsInputRequestTypeDef(
+    _RequiredListClosedWorkflowExecutionsInputRequestTypeDef,
+    _OptionalListClosedWorkflowExecutionsInputRequestTypeDef,
+):
+    pass
+
+_RequiredListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef = TypedDict(
+    "_RequiredListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef",
+    {
+        "domain": str,
+        "startTimeFilter": ExecutionTimeFilterTypeDef,
+    },
+)
+_OptionalListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef = TypedDict(
+    "_OptionalListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef",
+    {
+        "typeFilter": WorkflowTypeFilterTypeDef,
+        "tagFilter": TagFilterTypeDef,
+        "reverseOrder": bool,
+        "executionFilter": WorkflowExecutionFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef(
+    _RequiredListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef,
+    _OptionalListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef,
+):
+    pass
+
+_RequiredListOpenWorkflowExecutionsInputRequestTypeDef = TypedDict(
+    "_RequiredListOpenWorkflowExecutionsInputRequestTypeDef",
+    {
+        "domain": str,
+        "startTimeFilter": ExecutionTimeFilterTypeDef,
+    },
+)
+_OptionalListOpenWorkflowExecutionsInputRequestTypeDef = TypedDict(
+    "_OptionalListOpenWorkflowExecutionsInputRequestTypeDef",
+    {
+        "typeFilter": WorkflowTypeFilterTypeDef,
+        "tagFilter": TagFilterTypeDef,
+        "nextPageToken": str,
+        "maximumPageSize": int,
+        "reverseOrder": bool,
+        "executionFilter": WorkflowExecutionFilterTypeDef,
+    },
+    total=False,
+)
+
+class ListOpenWorkflowExecutionsInputRequestTypeDef(
+    _RequiredListOpenWorkflowExecutionsInputRequestTypeDef,
+    _OptionalListOpenWorkflowExecutionsInputRequestTypeDef,
+):
+    pass
+
 _RequiredRespondDecisionTaskCompletedInputRequestTypeDef = TypedDict(
     "_RequiredRespondDecisionTaskCompletedInputRequestTypeDef",
     {
         "taskToken": str,
     },
 )
 _OptionalRespondDecisionTaskCompletedInputRequestTypeDef = TypedDict(
```

### Comparing `mypy-boto3-swf-1.28.15.post1/mypy_boto3_swf.egg-info/PKG-INFO` & `mypy-boto3-swf-1.28.16/mypy_boto3_swf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-swf
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.SWF 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.SWF 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_swf/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 swf type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 swf type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-swf.svg?color=blue)](https://pypi.org/project/mypy-boto3-swf)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_swf/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-swf)](https://pepy.tech/project/mypy-boto3-swf)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SWF 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF)
+[boto3.SWF 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF)
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
 [mypy-boto3-swf docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_swf/).
 
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
@@ -366,20 +366,20 @@
 )
 
 
 def check_value(value: ActivityTaskTimeoutTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_swf.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_swf.type_defs import (
     ActivityTaskCancelRequestedEventAttributesTypeDef,
     ActivityTaskCanceledEventAttributesTypeDef,
     ActivityTaskCompletedEventAttributesTypeDef,
     ActivityTaskFailedEventAttributesTypeDef,
@@ -394,15 +394,14 @@
     CancelWorkflowExecutionDecisionAttributesTypeDef,
     CancelWorkflowExecutionFailedEventAttributesTypeDef,
     WorkflowTypeTypeDef,
     CloseStatusFilterTypeDef,
     CompleteWorkflowExecutionDecisionAttributesTypeDef,
     CompleteWorkflowExecutionFailedEventAttributesTypeDef,
     ContinueAsNewWorkflowExecutionFailedEventAttributesTypeDef,
-    ExecutionTimeFilterTypeDef,
     TagFilterTypeDef,
     WorkflowExecutionFilterTypeDef,
     WorkflowTypeFilterTypeDef,
     DecisionTaskCompletedEventAttributesTypeDef,
     DecisionTaskStartedEventAttributesTypeDef,
     DecisionTaskTimedOutEventAttributesTypeDef,
     FailWorkflowExecutionDecisionAttributesTypeDef,
@@ -412,14 +411,15 @@
     ScheduleLambdaFunctionDecisionAttributesTypeDef,
     SignalExternalWorkflowExecutionDecisionAttributesTypeDef,
     StartTimerDecisionAttributesTypeDef,
     DeprecateDomainInputRequestTypeDef,
     DescribeDomainInputRequestTypeDef,
     DomainConfigurationTypeDef,
     DomainInfoTypeDef,
+    TimestampTypeDef,
     FailWorkflowExecutionFailedEventAttributesTypeDef,
     PaginatorConfigTypeDef,
     LambdaFunctionCompletedEventAttributesTypeDef,
     LambdaFunctionFailedEventAttributesTypeDef,
     LambdaFunctionScheduledEventAttributesTypeDef,
     LambdaFunctionStartedEventAttributesTypeDef,
     LambdaFunctionTimedOutEventAttributesTypeDef,
@@ -499,45 +499,46 @@
     StartChildWorkflowExecutionInitiatedEventAttributesTypeDef,
     StartWorkflowExecutionInputRequestTypeDef,
     UndeprecateWorkflowTypeInputRequestTypeDef,
     WorkflowExecutionContinuedAsNewEventAttributesTypeDef,
     WorkflowExecutionInfoTypeDef,
     WorkflowExecutionStartedEventAttributesTypeDef,
     WorkflowTypeInfoTypeDef,
-    CountClosedWorkflowExecutionsInputRequestTypeDef,
-    CountOpenWorkflowExecutionsInputRequestTypeDef,
-    ListClosedWorkflowExecutionsInputRequestTypeDef,
-    ListOpenWorkflowExecutionsInputRequestTypeDef,
     DomainDetailTypeDef,
     DomainInfosTypeDef,
+    ExecutionTimeFilterTypeDef,
     GetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef,
     ListActivityTypesInputListActivityTypesPaginateTypeDef,
-    ListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef,
     ListDomainsInputListDomainsPaginateTypeDef,
-    ListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef,
     ListWorkflowTypesInputListWorkflowTypesPaginateTypeDef,
     PollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef,
     ListTagsForResourceOutputTypeDef,
     RegisterDomainInputRequestTypeDef,
     TagResourceInputRequestTypeDef,
     ActivityTypeInfosTypeDef,
     ActivityTypeDetailTypeDef,
     DecisionTypeDef,
     WorkflowExecutionDetailTypeDef,
     WorkflowExecutionInfosTypeDef,
     HistoryEventTypeDef,
     WorkflowTypeDetailTypeDef,
     WorkflowTypeInfosTypeDef,
+    CountClosedWorkflowExecutionsInputRequestTypeDef,
+    CountOpenWorkflowExecutionsInputRequestTypeDef,
+    ListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef,
+    ListClosedWorkflowExecutionsInputRequestTypeDef,
+    ListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef,
+    ListOpenWorkflowExecutionsInputRequestTypeDef,
     RespondDecisionTaskCompletedInputRequestTypeDef,
     DecisionTaskTypeDef,
     HistoryTypeDef,
 )
 
 
-def get_structure() -> ActivityTaskCancelRequestedEventAttributesTypeDef:
+def get_value() -> ActivityTaskCancelRequestedEventAttributesTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-swf-1.28.15.post1/mypy_boto3_swf.egg-info/SOURCES.txt` & `mypy-boto3-swf-1.28.16/mypy_boto3_swf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-swf-1.28.15.post1/setup.py` & `mypy-boto3-swf-1.28.16/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-swf",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_swf"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.SWF 1.28.15 service generated with mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.SWF 1.28.16 service generated with mypy-boto3-builder 7.17.1"
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
-    keywords="boto3 swf type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 swf type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_swf": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_swf/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

