# Comparing `tmp/mypy-boto3-events-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-events-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-events-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:07 2023, max compression
+gzip compressed data, was "mypy-boto3-events-1.28.16.tar", last modified: Tue Aug  1 11:36:47 2023, max compression
```

## Comparing `mypy-boto3-events-1.28.15.post1.tar` & `mypy-boto3-events-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:07.281147 mypy-boto3-events-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:45:10.000000 mypy-boto3-events-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20194 2023-07-29 10:03:07.281147 mypy-boto3-events-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18700 2023-07-29 09:45:10.000000 mypy-boto3-events-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:07.273147 mypy-boto3-events-1.28.15.post1/mypy_boto3_events/
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-29 09:45:10.000000 mypy-boto3-events-1.28.15.post1/mypy_boto3_events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-29 09:45:10.000000 mypy-boto3-events-1.28.15.post1/mypy_boto3_events/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-29 09:45:10.000000 mypy-boto3-events-1.28.15.post1/mypy_boto3_events/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37939 2023-07-29 09:45:11.000000 mypy-boto3-events-1.28.15.post1/mypy_boto3_events/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    37873 2023-07-29 09:45:11.000000 mypy-boto3-events-1.28.15.post1/mypy_boto3_events/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10281 2023-07-29 09:45:11.000000 mypy-boto3-events-1.28.15.post1/mypy_boto3_events/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10279 2023-07-29 09:45:11.000000 mypy-boto3-events-1.28.15.post1/mypy_boto3_events/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-07-29 09:45:11.000000 mypy-boto3-events-1.28.15.post1/mypy_boto3_events/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-07-29 09:45:11.000000 mypy-boto3-events-1.28.15.post1/mypy_boto3_events/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:45:10.000000 mypy-boto3-events-1.28.15.post1/mypy_boto3_events/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    64866 2023-07-29 09:45:15.000000 mypy-boto3-events-1.28.15.post1/mypy_boto3_events/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    64785 2023-07-29 09:45:12.000000 mypy-boto3-events-1.28.15.post1/mypy_boto3_events/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:45:10.000000 mypy-boto3-events-1.28.15.post1/mypy_boto3_events/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:07.281147 mypy-boto3-events-1.28.15.post1/mypy_boto3_events.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20194 2023-07-29 10:03:06.000000 mypy-boto3-events-1.28.15.post1/mypy_boto3_events.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-29 10:03:07.000000 mypy-boto3-events-1.28.15.post1/mypy_boto3_events.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:07.000000 mypy-boto3-events-1.28.15.post1/mypy_boto3_events.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:06.000000 mypy-boto3-events-1.28.15.post1/mypy_boto3_events.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:07.000000 mypy-boto3-events-1.28.15.post1/mypy_boto3_events.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-29 10:03:07.000000 mypy-boto3-events-1.28.15.post1/mypy_boto3_events.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:07.281147 mypy-boto3-events-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-07-29 09:45:10.000000 mypy-boto3-events-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:47.292891 mypy-boto3-events-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:17:47.000000 mypy-boto3-events-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20265 2023-08-01 11:36:47.292891 mypy-boto3-events-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18780 2023-08-01 11:17:47.000000 mypy-boto3-events-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:47.280892 mypy-boto3-events-1.28.16/mypy_boto3_events/
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-08-01 11:17:47.000000 mypy-boto3-events-1.28.16/mypy_boto3_events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-08-01 11:17:47.000000 mypy-boto3-events-1.28.16/mypy_boto3_events/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-08-01 11:17:47.000000 mypy-boto3-events-1.28.16/mypy_boto3_events/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37776 2023-08-01 11:17:47.000000 mypy-boto3-events-1.28.16/mypy_boto3_events/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37710 2023-08-01 11:17:47.000000 mypy-boto3-events-1.28.16/mypy_boto3_events/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10281 2023-08-01 11:17:48.000000 mypy-boto3-events-1.28.16/mypy_boto3_events/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10279 2023-08-01 11:17:48.000000 mypy-boto3-events-1.28.16/mypy_boto3_events/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-08-01 11:17:47.000000 mypy-boto3-events-1.28.16/mypy_boto3_events/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-08-01 11:17:47.000000 mypy-boto3-events-1.28.16/mypy_boto3_events/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:17:47.000000 mypy-boto3-events-1.28.16/mypy_boto3_events/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    65110 2023-08-01 11:17:51.000000 mypy-boto3-events-1.28.16/mypy_boto3_events/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65030 2023-08-01 11:17:50.000000 mypy-boto3-events-1.28.16/mypy_boto3_events/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:17:47.000000 mypy-boto3-events-1.28.16/mypy_boto3_events/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:47.292891 mypy-boto3-events-1.28.16/mypy_boto3_events.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20265 2023-08-01 11:36:47.000000 mypy-boto3-events-1.28.16/mypy_boto3_events.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-08-01 11:36:47.000000 mypy-boto3-events-1.28.16/mypy_boto3_events.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:47.000000 mypy-boto3-events-1.28.16/mypy_boto3_events.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:47.000000 mypy-boto3-events-1.28.16/mypy_boto3_events.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:47.000000 mypy-boto3-events-1.28.16/mypy_boto3_events.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-01 11:36:47.000000 mypy-boto3-events-1.28.16/mypy_boto3_events.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:47.292891 mypy-boto3-events-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-08-01 11:17:47.000000 mypy-boto3-events-1.28.16/setup.py
```

### Comparing `mypy-boto3-events-1.28.15.post1/LICENSE` & `mypy-boto3-events-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-events-1.28.15.post1/PKG-INFO` & `mypy-boto3-events-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-events
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.EventBridge 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.EventBridge 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_events/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 events type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 events type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-events.svg?color=blue)](https://pypi.org/project/mypy-boto3-events)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_events/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-events)](https://pepy.tech/project/mypy-boto3-events)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EventBridge 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge)
+[boto3.EventBridge 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge)
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
 [mypy-boto3-events docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_events/).
 
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
@@ -337,20 +337,20 @@
 )
 
 
 def check_value(value: ApiDestinationHttpMethodType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_events.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_events.type_defs import (
     ActivateEventSourceRequestRequestTypeDef,
     ApiDestinationTypeDef,
     ArchiveTypeDef,
     AwsVpcConfigurationOutputTypeDef,
@@ -424,17 +424,16 @@
     ReplayTypeDef,
     PaginatorConfigTypeDef,
     ListRuleNamesByTargetRequestRequestTypeDef,
     ListRulesRequestRequestTypeDef,
     RuleTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTargetsByRuleRequestRequestTypeDef,
-    PutEventsRequestEntryTypeDef,
+    TimestampTypeDef,
     PutEventsResultEntryTypeDef,
-    PutPartnerEventsRequestEntryTypeDef,
     PutPartnerEventsResultEntryTypeDef,
     PutTargetsResultEntryTypeDef,
     RedshiftDataParametersOutputTypeDef,
     RedshiftDataParametersTypeDef,
     RemovePermissionRequestRequestTypeDef,
     RemoveTargetsRequestRequestTypeDef,
     RemoveTargetsResultEntryTypeDef,
@@ -493,52 +492,56 @@
     ListPartnerEventSourceAccountsResponseTypeDef,
     ListPartnerEventSourcesResponseTypeDef,
     ListReplaysResponseTypeDef,
     ListRuleNamesByTargetRequestListRuleNamesByTargetPaginateTypeDef,
     ListRulesRequestListRulesPaginateTypeDef,
     ListTargetsByRuleRequestListTargetsByRulePaginateTypeDef,
     ListRulesResponseTypeDef,
-    PutEventsRequestRequestTypeDef,
+    PutEventsRequestEntryTypeDef,
+    PutPartnerEventsRequestEntryTypeDef,
     PutEventsResponseTypeDef,
-    PutPartnerEventsRequestRequestTypeDef,
     PutPartnerEventsResponseTypeDef,
     PutTargetsResponseTypeDef,
     RemoveTargetsResponseTypeDef,
+    ReplayDestinationUnionTypeDef,
     StartReplayRequestRequestTypeDef,
     RunCommandParametersOutputTypeDef,
     RunCommandParametersTypeDef,
     SageMakerPipelineParametersOutputTypeDef,
     SageMakerPipelineParametersTypeDef,
     EcsParametersOutputTypeDef,
     EcsParametersTypeDef,
     ConnectionOAuthResponseParametersTypeDef,
     CreateConnectionOAuthRequestParametersTypeDef,
     UpdateConnectionOAuthRequestParametersTypeDef,
     RoutingConfigTypeDef,
+    PutEventsRequestRequestTypeDef,
+    PutPartnerEventsRequestRequestTypeDef,
     TargetOutputTypeDef,
     TargetTypeDef,
     ConnectionAuthResponseParametersTypeDef,
     CreateConnectionAuthRequestParametersTypeDef,
     UpdateConnectionAuthRequestParametersTypeDef,
     CreateEndpointRequestRequestTypeDef,
     CreateEndpointResponseTypeDef,
     DescribeEndpointResponseTypeDef,
     EndpointTypeDef,
     UpdateEndpointRequestRequestTypeDef,
     UpdateEndpointResponseTypeDef,
     ListTargetsByRuleResponseTypeDef,
-    PutTargetsRequestRequestTypeDef,
+    TargetUnionTypeDef,
     DescribeConnectionResponseTypeDef,
     CreateConnectionRequestRequestTypeDef,
     UpdateConnectionRequestRequestTypeDef,
     ListEndpointsResponseTypeDef,
+    PutTargetsRequestRequestTypeDef,
 )
 
 
-def get_structure() -> ActivateEventSourceRequestRequestTypeDef:
+def get_value() -> ActivateEventSourceRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-events-1.28.15.post1/README.md` & `mypy-boto3-events-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-events.svg?color=blue)](https://pypi.org/project/mypy-boto3-events)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_events/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-events)](https://pepy.tech/project/mypy-boto3-events)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EventBridge 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge)
+[boto3.EventBridge 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge)
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
 [mypy-boto3-events docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_events/).
 
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
@@ -305,20 +305,20 @@
 )
 
 
 def check_value(value: ApiDestinationHttpMethodType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_events.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_events.type_defs import (
     ActivateEventSourceRequestRequestTypeDef,
     ApiDestinationTypeDef,
     ArchiveTypeDef,
     AwsVpcConfigurationOutputTypeDef,
@@ -392,17 +392,16 @@
     ReplayTypeDef,
     PaginatorConfigTypeDef,
     ListRuleNamesByTargetRequestRequestTypeDef,
     ListRulesRequestRequestTypeDef,
     RuleTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTargetsByRuleRequestRequestTypeDef,
-    PutEventsRequestEntryTypeDef,
+    TimestampTypeDef,
     PutEventsResultEntryTypeDef,
-    PutPartnerEventsRequestEntryTypeDef,
     PutPartnerEventsResultEntryTypeDef,
     PutTargetsResultEntryTypeDef,
     RedshiftDataParametersOutputTypeDef,
     RedshiftDataParametersTypeDef,
     RemovePermissionRequestRequestTypeDef,
     RemoveTargetsRequestRequestTypeDef,
     RemoveTargetsResultEntryTypeDef,
@@ -461,52 +460,56 @@
     ListPartnerEventSourceAccountsResponseTypeDef,
     ListPartnerEventSourcesResponseTypeDef,
     ListReplaysResponseTypeDef,
     ListRuleNamesByTargetRequestListRuleNamesByTargetPaginateTypeDef,
     ListRulesRequestListRulesPaginateTypeDef,
     ListTargetsByRuleRequestListTargetsByRulePaginateTypeDef,
     ListRulesResponseTypeDef,
-    PutEventsRequestRequestTypeDef,
+    PutEventsRequestEntryTypeDef,
+    PutPartnerEventsRequestEntryTypeDef,
     PutEventsResponseTypeDef,
-    PutPartnerEventsRequestRequestTypeDef,
     PutPartnerEventsResponseTypeDef,
     PutTargetsResponseTypeDef,
     RemoveTargetsResponseTypeDef,
+    ReplayDestinationUnionTypeDef,
     StartReplayRequestRequestTypeDef,
     RunCommandParametersOutputTypeDef,
     RunCommandParametersTypeDef,
     SageMakerPipelineParametersOutputTypeDef,
     SageMakerPipelineParametersTypeDef,
     EcsParametersOutputTypeDef,
     EcsParametersTypeDef,
     ConnectionOAuthResponseParametersTypeDef,
     CreateConnectionOAuthRequestParametersTypeDef,
     UpdateConnectionOAuthRequestParametersTypeDef,
     RoutingConfigTypeDef,
+    PutEventsRequestRequestTypeDef,
+    PutPartnerEventsRequestRequestTypeDef,
     TargetOutputTypeDef,
     TargetTypeDef,
     ConnectionAuthResponseParametersTypeDef,
     CreateConnectionAuthRequestParametersTypeDef,
     UpdateConnectionAuthRequestParametersTypeDef,
     CreateEndpointRequestRequestTypeDef,
     CreateEndpointResponseTypeDef,
     DescribeEndpointResponseTypeDef,
     EndpointTypeDef,
     UpdateEndpointRequestRequestTypeDef,
     UpdateEndpointResponseTypeDef,
     ListTargetsByRuleResponseTypeDef,
-    PutTargetsRequestRequestTypeDef,
+    TargetUnionTypeDef,
     DescribeConnectionResponseTypeDef,
     CreateConnectionRequestRequestTypeDef,
     UpdateConnectionRequestRequestTypeDef,
     ListEndpointsResponseTypeDef,
+    PutTargetsRequestRequestTypeDef,
 )
 
 
-def get_structure() -> ActivateEventSourceRequestRequestTypeDef:
+def get_value() -> ActivateEventSourceRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-events-1.28.15.post1/mypy_boto3_events/__init__.py` & `mypy-boto3-events-1.28.16/mypy_boto3_events/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-events-1.28.15.post1/mypy_boto3_events/__init__.pyi` & `mypy-boto3-events-1.28.16/mypy_boto3_events/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-events-1.28.15.post1/mypy_boto3_events/__main__.py` & `mypy-boto3-events-1.28.16/mypy_boto3_events/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.EventBridge 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.EventBridge 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_events//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge\nOther"
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

### Comparing `mypy-boto3-events-1.28.15.post1/mypy_boto3_events/client.py` & `mypy-boto3-events-1.28.16/mypy_boto3_events/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from mypy_boto3_events.client import EventBridgeClient
 
     session = Session()
     client: EventBridgeClient = session.client("events")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     ApiDestinationHttpMethodType,
     ArchiveStateType,
     ConnectionAuthorizationTypeType,
@@ -71,23 +70,22 @@
     PutEventsRequestEntryTypeDef,
     PutEventsResponseTypeDef,
     PutPartnerEventsRequestEntryTypeDef,
     PutPartnerEventsResponseTypeDef,
     PutRuleResponseTypeDef,
     PutTargetsResponseTypeDef,
     RemoveTargetsResponseTypeDef,
-    ReplayDestinationOutputTypeDef,
-    ReplayDestinationTypeDef,
+    ReplayDestinationUnionTypeDef,
     ReplicationConfigTypeDef,
     RoutingConfigTypeDef,
     StartReplayResponseTypeDef,
     TagTypeDef,
-    TargetOutputTypeDef,
-    TargetTypeDef,
+    TargetUnionTypeDef,
     TestEventPatternResponseTypeDef,
+    TimestampTypeDef,
     UpdateApiDestinationResponseTypeDef,
     UpdateArchiveResponseTypeDef,
     UpdateConnectionAuthRequestParametersTypeDef,
     UpdateConnectionResponseTypeDef,
     UpdateEndpointResponseTypeDef,
 )
 
@@ -661,19 +659,15 @@
         Creates or updates the specified rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.put_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_events/client/#put_rule)
         """
 
     def put_targets(
-        self,
-        *,
-        Rule: str,
-        Targets: Sequence[Union[TargetTypeDef, TargetOutputTypeDef]],
-        EventBusName: str = ...
+        self, *, Rule: str, Targets: Sequence[TargetUnionTypeDef], EventBusName: str = ...
     ) -> PutTargetsResponseTypeDef:
         """
         Adds the specified targets to the specified rule, or updates the targets if they
         are already associated with the rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.put_targets)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_events/client/#put_targets)
@@ -701,17 +695,17 @@
         """
 
     def start_replay(
         self,
         *,
         ReplayName: str,
         EventSourceArn: str,
-        EventStartTime: Union[datetime, str],
-        EventEndTime: Union[datetime, str],
-        Destination: Union[ReplayDestinationTypeDef, ReplayDestinationOutputTypeDef],
+        EventStartTime: TimestampTypeDef,
+        EventEndTime: TimestampTypeDef,
+        Destination: ReplayDestinationUnionTypeDef,
         Description: str = ...
     ) -> StartReplayResponseTypeDef:
         """
         Starts the specified replay.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.start_replay)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_events/client/#start_replay)
```

### Comparing `mypy-boto3-events-1.28.15.post1/mypy_boto3_events/client.pyi` & `mypy-boto3-events-1.28.16/mypy_boto3_events/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from mypy_boto3_events.client import EventBridgeClient
 
     session = Session()
     client: EventBridgeClient = session.client("events")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     ApiDestinationHttpMethodType,
     ArchiveStateType,
     ConnectionAuthorizationTypeType,
@@ -71,23 +70,22 @@
     PutEventsRequestEntryTypeDef,
     PutEventsResponseTypeDef,
     PutPartnerEventsRequestEntryTypeDef,
     PutPartnerEventsResponseTypeDef,
     PutRuleResponseTypeDef,
     PutTargetsResponseTypeDef,
     RemoveTargetsResponseTypeDef,
-    ReplayDestinationOutputTypeDef,
-    ReplayDestinationTypeDef,
+    ReplayDestinationUnionTypeDef,
     ReplicationConfigTypeDef,
     RoutingConfigTypeDef,
     StartReplayResponseTypeDef,
     TagTypeDef,
-    TargetOutputTypeDef,
-    TargetTypeDef,
+    TargetUnionTypeDef,
     TestEventPatternResponseTypeDef,
+    TimestampTypeDef,
     UpdateApiDestinationResponseTypeDef,
     UpdateArchiveResponseTypeDef,
     UpdateConnectionAuthRequestParametersTypeDef,
     UpdateConnectionResponseTypeDef,
     UpdateEndpointResponseTypeDef,
 )
 
@@ -608,19 +606,15 @@
         """
         Creates or updates the specified rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.put_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_events/client/#put_rule)
         """
     def put_targets(
-        self,
-        *,
-        Rule: str,
-        Targets: Sequence[Union[TargetTypeDef, TargetOutputTypeDef]],
-        EventBusName: str = ...
+        self, *, Rule: str, Targets: Sequence[TargetUnionTypeDef], EventBusName: str = ...
     ) -> PutTargetsResponseTypeDef:
         """
         Adds the specified targets to the specified rule, or updates the targets if they
         are already associated with the rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.put_targets)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_events/client/#put_targets)
@@ -645,17 +639,17 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_events/client/#remove_targets)
         """
     def start_replay(
         self,
         *,
         ReplayName: str,
         EventSourceArn: str,
-        EventStartTime: Union[datetime, str],
-        EventEndTime: Union[datetime, str],
-        Destination: Union[ReplayDestinationTypeDef, ReplayDestinationOutputTypeDef],
+        EventStartTime: TimestampTypeDef,
+        EventEndTime: TimestampTypeDef,
+        Destination: ReplayDestinationUnionTypeDef,
         Description: str = ...
     ) -> StartReplayResponseTypeDef:
         """
         Starts the specified replay.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.start_replay)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_events/client/#start_replay)
```

### Comparing `mypy-boto3-events-1.28.15.post1/mypy_boto3_events/literals.py` & `mypy-boto3-events-1.28.16/mypy_boto3_events/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-events-1.28.15.post1/mypy_boto3_events/literals.pyi` & `mypy-boto3-events-1.28.16/mypy_boto3_events/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-events-1.28.15.post1/mypy_boto3_events/paginator.py` & `mypy-boto3-events-1.28.16/mypy_boto3_events/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-events-1.28.15.post1/mypy_boto3_events/paginator.pyi` & `mypy-boto3-events-1.28.16/mypy_boto3_events/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-events-1.28.15.post1/mypy_boto3_events/type_defs.py` & `mypy-boto3-events-1.28.16/mypy_boto3_events/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_events/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_events.type_defs import ActivateEventSourceRequestRequestTypeDef
 
-    data: ActivateEventSourceRequestRequestTypeDef = {...}
+    data: ActivateEventSourceRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -118,17 +118,16 @@
     "ReplayTypeDef",
     "PaginatorConfigTypeDef",
     "ListRuleNamesByTargetRequestRequestTypeDef",
     "ListRulesRequestRequestTypeDef",
     "RuleTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListTargetsByRuleRequestRequestTypeDef",
-    "PutEventsRequestEntryTypeDef",
+    "TimestampTypeDef",
     "PutEventsResultEntryTypeDef",
-    "PutPartnerEventsRequestEntryTypeDef",
     "PutPartnerEventsResultEntryTypeDef",
     "PutTargetsResultEntryTypeDef",
     "RedshiftDataParametersOutputTypeDef",
     "RedshiftDataParametersTypeDef",
     "RemovePermissionRequestRequestTypeDef",
     "RemoveTargetsRequestRequestTypeDef",
     "RemoveTargetsResultEntryTypeDef",
@@ -187,48 +186,52 @@
     "ListPartnerEventSourceAccountsResponseTypeDef",
     "ListPartnerEventSourcesResponseTypeDef",
     "ListReplaysResponseTypeDef",
     "ListRuleNamesByTargetRequestListRuleNamesByTargetPaginateTypeDef",
     "ListRulesRequestListRulesPaginateTypeDef",
     "ListTargetsByRuleRequestListTargetsByRulePaginateTypeDef",
     "ListRulesResponseTypeDef",
-    "PutEventsRequestRequestTypeDef",
+    "PutEventsRequestEntryTypeDef",
+    "PutPartnerEventsRequestEntryTypeDef",
     "PutEventsResponseTypeDef",
-    "PutPartnerEventsRequestRequestTypeDef",
     "PutPartnerEventsResponseTypeDef",
     "PutTargetsResponseTypeDef",
     "RemoveTargetsResponseTypeDef",
+    "ReplayDestinationUnionTypeDef",
     "StartReplayRequestRequestTypeDef",
     "RunCommandParametersOutputTypeDef",
     "RunCommandParametersTypeDef",
     "SageMakerPipelineParametersOutputTypeDef",
     "SageMakerPipelineParametersTypeDef",
     "EcsParametersOutputTypeDef",
     "EcsParametersTypeDef",
     "ConnectionOAuthResponseParametersTypeDef",
     "CreateConnectionOAuthRequestParametersTypeDef",
     "UpdateConnectionOAuthRequestParametersTypeDef",
     "RoutingConfigTypeDef",
+    "PutEventsRequestRequestTypeDef",
+    "PutPartnerEventsRequestRequestTypeDef",
     "TargetOutputTypeDef",
     "TargetTypeDef",
     "ConnectionAuthResponseParametersTypeDef",
     "CreateConnectionAuthRequestParametersTypeDef",
     "UpdateConnectionAuthRequestParametersTypeDef",
     "CreateEndpointRequestRequestTypeDef",
     "CreateEndpointResponseTypeDef",
     "DescribeEndpointResponseTypeDef",
     "EndpointTypeDef",
     "UpdateEndpointRequestRequestTypeDef",
     "UpdateEndpointResponseTypeDef",
     "ListTargetsByRuleResponseTypeDef",
-    "PutTargetsRequestRequestTypeDef",
+    "TargetUnionTypeDef",
     "DescribeConnectionResponseTypeDef",
     "CreateConnectionRequestRequestTypeDef",
     "UpdateConnectionRequestRequestTypeDef",
     "ListEndpointsResponseTypeDef",
+    "PutTargetsRequestRequestTypeDef",
 )
 
 ActivateEventSourceRequestRequestTypeDef = TypedDict(
     "ActivateEventSourceRequestRequestTypeDef",
     {
         "Name": str,
     },
@@ -1158,50 +1161,25 @@
 
 class ListTargetsByRuleRequestRequestTypeDef(
     _RequiredListTargetsByRuleRequestRequestTypeDef, _OptionalListTargetsByRuleRequestRequestTypeDef
 ):
     pass
 
 
-PutEventsRequestEntryTypeDef = TypedDict(
-    "PutEventsRequestEntryTypeDef",
-    {
-        "Time": Union[datetime, str],
-        "Source": str,
-        "Resources": Sequence[str],
-        "DetailType": str,
-        "Detail": str,
-        "EventBusName": str,
-        "TraceHeader": str,
-    },
-    total=False,
-)
-
+TimestampTypeDef = Union[datetime, str]
 PutEventsResultEntryTypeDef = TypedDict(
     "PutEventsResultEntryTypeDef",
     {
         "EventId": str,
         "ErrorCode": str,
         "ErrorMessage": str,
     },
     total=False,
 )
 
-PutPartnerEventsRequestEntryTypeDef = TypedDict(
-    "PutPartnerEventsRequestEntryTypeDef",
-    {
-        "Time": Union[datetime, str],
-        "Source": str,
-        "Resources": Sequence[str],
-        "DetailType": str,
-        "Detail": str,
-    },
-    total=False,
-)
-
 PutPartnerEventsResultEntryTypeDef = TypedDict(
     "PutPartnerEventsResultEntryTypeDef",
     {
         "EventId": str,
         "ErrorCode": str,
         "ErrorMessage": str,
     },
@@ -2006,51 +1984,49 @@
     {
         "Rules": List[RuleTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredPutEventsRequestRequestTypeDef = TypedDict(
-    "_RequiredPutEventsRequestRequestTypeDef",
+PutEventsRequestEntryTypeDef = TypedDict(
+    "PutEventsRequestEntryTypeDef",
     {
-        "Entries": Sequence[PutEventsRequestEntryTypeDef],
+        "Time": TimestampTypeDef,
+        "Source": str,
+        "Resources": Sequence[str],
+        "DetailType": str,
+        "Detail": str,
+        "EventBusName": str,
+        "TraceHeader": str,
     },
+    total=False,
 )
-_OptionalPutEventsRequestRequestTypeDef = TypedDict(
-    "_OptionalPutEventsRequestRequestTypeDef",
+
+PutPartnerEventsRequestEntryTypeDef = TypedDict(
+    "PutPartnerEventsRequestEntryTypeDef",
     {
-        "EndpointId": str,
+        "Time": TimestampTypeDef,
+        "Source": str,
+        "Resources": Sequence[str],
+        "DetailType": str,
+        "Detail": str,
     },
     total=False,
 )
 
-
-class PutEventsRequestRequestTypeDef(
-    _RequiredPutEventsRequestRequestTypeDef, _OptionalPutEventsRequestRequestTypeDef
-):
-    pass
-
-
 PutEventsResponseTypeDef = TypedDict(
     "PutEventsResponseTypeDef",
     {
         "FailedEntryCount": int,
         "Entries": List[PutEventsResultEntryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutPartnerEventsRequestRequestTypeDef = TypedDict(
-    "PutPartnerEventsRequestRequestTypeDef",
-    {
-        "Entries": Sequence[PutPartnerEventsRequestEntryTypeDef],
-    },
-)
-
 PutPartnerEventsResponseTypeDef = TypedDict(
     "PutPartnerEventsResponseTypeDef",
     {
         "FailedEntryCount": int,
         "Entries": List[PutPartnerEventsResultEntryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2070,21 +2046,22 @@
     {
         "FailedEntryCount": int,
         "FailedEntries": List[RemoveTargetsResultEntryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ReplayDestinationUnionTypeDef = Union[ReplayDestinationTypeDef, ReplayDestinationOutputTypeDef]
 _RequiredStartReplayRequestRequestTypeDef = TypedDict(
     "_RequiredStartReplayRequestRequestTypeDef",
     {
         "ReplayName": str,
         "EventSourceArn": str,
-        "EventStartTime": Union[datetime, str],
-        "EventEndTime": Union[datetime, str],
+        "EventStartTime": TimestampTypeDef,
+        "EventEndTime": TimestampTypeDef,
         "Destination": ReplayDestinationTypeDef,
     },
 )
 _OptionalStartReplayRequestRequestTypeDef = TypedDict(
     "_OptionalStartReplayRequestRequestTypeDef",
     {
         "Description": str,
@@ -2242,14 +2219,42 @@
 RoutingConfigTypeDef = TypedDict(
     "RoutingConfigTypeDef",
     {
         "FailoverConfig": FailoverConfigTypeDef,
     },
 )
 
+_RequiredPutEventsRequestRequestTypeDef = TypedDict(
+    "_RequiredPutEventsRequestRequestTypeDef",
+    {
+        "Entries": Sequence[PutEventsRequestEntryTypeDef],
+    },
+)
+_OptionalPutEventsRequestRequestTypeDef = TypedDict(
+    "_OptionalPutEventsRequestRequestTypeDef",
+    {
+        "EndpointId": str,
+    },
+    total=False,
+)
+
+
+class PutEventsRequestRequestTypeDef(
+    _RequiredPutEventsRequestRequestTypeDef, _OptionalPutEventsRequestRequestTypeDef
+):
+    pass
+
+
+PutPartnerEventsRequestRequestTypeDef = TypedDict(
+    "PutPartnerEventsRequestRequestTypeDef",
+    {
+        "Entries": Sequence[PutPartnerEventsRequestEntryTypeDef],
+    },
+)
+
 _RequiredTargetOutputTypeDef = TypedDict(
     "_RequiredTargetOutputTypeDef",
     {
         "Id": str,
         "Arn": str,
     },
 )
@@ -2470,36 +2475,15 @@
     {
         "Targets": List[TargetOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredPutTargetsRequestRequestTypeDef = TypedDict(
-    "_RequiredPutTargetsRequestRequestTypeDef",
-    {
-        "Rule": str,
-        "Targets": Sequence[Union[TargetTypeDef, TargetOutputTypeDef]],
-    },
-)
-_OptionalPutTargetsRequestRequestTypeDef = TypedDict(
-    "_OptionalPutTargetsRequestRequestTypeDef",
-    {
-        "EventBusName": str,
-    },
-    total=False,
-)
-
-
-class PutTargetsRequestRequestTypeDef(
-    _RequiredPutTargetsRequestRequestTypeDef, _OptionalPutTargetsRequestRequestTypeDef
-):
-    pass
-
-
+TargetUnionTypeDef = Union[TargetTypeDef, TargetOutputTypeDef]
 DescribeConnectionResponseTypeDef = TypedDict(
     "DescribeConnectionResponseTypeDef",
     {
         "ConnectionArn": str,
         "Name": str,
         "Description": str,
         "ConnectionState": ConnectionStateType,
@@ -2564,7 +2548,28 @@
     "ListEndpointsResponseTypeDef",
     {
         "Endpoints": List[EndpointTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+
+_RequiredPutTargetsRequestRequestTypeDef = TypedDict(
+    "_RequiredPutTargetsRequestRequestTypeDef",
+    {
+        "Rule": str,
+        "Targets": Sequence[TargetUnionTypeDef],
+    },
+)
+_OptionalPutTargetsRequestRequestTypeDef = TypedDict(
+    "_OptionalPutTargetsRequestRequestTypeDef",
+    {
+        "EventBusName": str,
+    },
+    total=False,
+)
+
+
+class PutTargetsRequestRequestTypeDef(
+    _RequiredPutTargetsRequestRequestTypeDef, _OptionalPutTargetsRequestRequestTypeDef
+):
+    pass
```

### Comparing `mypy-boto3-events-1.28.15.post1/mypy_boto3_events/type_defs.pyi` & `mypy-boto3-events-1.28.16/mypy_boto3_events/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_events/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_events.type_defs import ActivateEventSourceRequestRequestTypeDef
 
-    data: ActivateEventSourceRequestRequestTypeDef = {...}
+    data: ActivateEventSourceRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -117,17 +117,16 @@
     "ReplayTypeDef",
     "PaginatorConfigTypeDef",
     "ListRuleNamesByTargetRequestRequestTypeDef",
     "ListRulesRequestRequestTypeDef",
     "RuleTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListTargetsByRuleRequestRequestTypeDef",
-    "PutEventsRequestEntryTypeDef",
+    "TimestampTypeDef",
     "PutEventsResultEntryTypeDef",
-    "PutPartnerEventsRequestEntryTypeDef",
     "PutPartnerEventsResultEntryTypeDef",
     "PutTargetsResultEntryTypeDef",
     "RedshiftDataParametersOutputTypeDef",
     "RedshiftDataParametersTypeDef",
     "RemovePermissionRequestRequestTypeDef",
     "RemoveTargetsRequestRequestTypeDef",
     "RemoveTargetsResultEntryTypeDef",
@@ -186,48 +185,52 @@
     "ListPartnerEventSourceAccountsResponseTypeDef",
     "ListPartnerEventSourcesResponseTypeDef",
     "ListReplaysResponseTypeDef",
     "ListRuleNamesByTargetRequestListRuleNamesByTargetPaginateTypeDef",
     "ListRulesRequestListRulesPaginateTypeDef",
     "ListTargetsByRuleRequestListTargetsByRulePaginateTypeDef",
     "ListRulesResponseTypeDef",
-    "PutEventsRequestRequestTypeDef",
+    "PutEventsRequestEntryTypeDef",
+    "PutPartnerEventsRequestEntryTypeDef",
     "PutEventsResponseTypeDef",
-    "PutPartnerEventsRequestRequestTypeDef",
     "PutPartnerEventsResponseTypeDef",
     "PutTargetsResponseTypeDef",
     "RemoveTargetsResponseTypeDef",
+    "ReplayDestinationUnionTypeDef",
     "StartReplayRequestRequestTypeDef",
     "RunCommandParametersOutputTypeDef",
     "RunCommandParametersTypeDef",
     "SageMakerPipelineParametersOutputTypeDef",
     "SageMakerPipelineParametersTypeDef",
     "EcsParametersOutputTypeDef",
     "EcsParametersTypeDef",
     "ConnectionOAuthResponseParametersTypeDef",
     "CreateConnectionOAuthRequestParametersTypeDef",
     "UpdateConnectionOAuthRequestParametersTypeDef",
     "RoutingConfigTypeDef",
+    "PutEventsRequestRequestTypeDef",
+    "PutPartnerEventsRequestRequestTypeDef",
     "TargetOutputTypeDef",
     "TargetTypeDef",
     "ConnectionAuthResponseParametersTypeDef",
     "CreateConnectionAuthRequestParametersTypeDef",
     "UpdateConnectionAuthRequestParametersTypeDef",
     "CreateEndpointRequestRequestTypeDef",
     "CreateEndpointResponseTypeDef",
     "DescribeEndpointResponseTypeDef",
     "EndpointTypeDef",
     "UpdateEndpointRequestRequestTypeDef",
     "UpdateEndpointResponseTypeDef",
     "ListTargetsByRuleResponseTypeDef",
-    "PutTargetsRequestRequestTypeDef",
+    "TargetUnionTypeDef",
     "DescribeConnectionResponseTypeDef",
     "CreateConnectionRequestRequestTypeDef",
     "UpdateConnectionRequestRequestTypeDef",
     "ListEndpointsResponseTypeDef",
+    "PutTargetsRequestRequestTypeDef",
 )
 
 ActivateEventSourceRequestRequestTypeDef = TypedDict(
     "ActivateEventSourceRequestRequestTypeDef",
     {
         "Name": str,
     },
@@ -1123,50 +1126,25 @@
 )
 
 class ListTargetsByRuleRequestRequestTypeDef(
     _RequiredListTargetsByRuleRequestRequestTypeDef, _OptionalListTargetsByRuleRequestRequestTypeDef
 ):
     pass
 
-PutEventsRequestEntryTypeDef = TypedDict(
-    "PutEventsRequestEntryTypeDef",
-    {
-        "Time": Union[datetime, str],
-        "Source": str,
-        "Resources": Sequence[str],
-        "DetailType": str,
-        "Detail": str,
-        "EventBusName": str,
-        "TraceHeader": str,
-    },
-    total=False,
-)
-
+TimestampTypeDef = Union[datetime, str]
 PutEventsResultEntryTypeDef = TypedDict(
     "PutEventsResultEntryTypeDef",
     {
         "EventId": str,
         "ErrorCode": str,
         "ErrorMessage": str,
     },
     total=False,
 )
 
-PutPartnerEventsRequestEntryTypeDef = TypedDict(
-    "PutPartnerEventsRequestEntryTypeDef",
-    {
-        "Time": Union[datetime, str],
-        "Source": str,
-        "Resources": Sequence[str],
-        "DetailType": str,
-        "Detail": str,
-    },
-    total=False,
-)
-
 PutPartnerEventsResultEntryTypeDef = TypedDict(
     "PutPartnerEventsResultEntryTypeDef",
     {
         "EventId": str,
         "ErrorCode": str,
         "ErrorMessage": str,
     },
@@ -1949,49 +1927,49 @@
     {
         "Rules": List[RuleTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredPutEventsRequestRequestTypeDef = TypedDict(
-    "_RequiredPutEventsRequestRequestTypeDef",
+PutEventsRequestEntryTypeDef = TypedDict(
+    "PutEventsRequestEntryTypeDef",
     {
-        "Entries": Sequence[PutEventsRequestEntryTypeDef],
+        "Time": TimestampTypeDef,
+        "Source": str,
+        "Resources": Sequence[str],
+        "DetailType": str,
+        "Detail": str,
+        "EventBusName": str,
+        "TraceHeader": str,
     },
+    total=False,
 )
-_OptionalPutEventsRequestRequestTypeDef = TypedDict(
-    "_OptionalPutEventsRequestRequestTypeDef",
+
+PutPartnerEventsRequestEntryTypeDef = TypedDict(
+    "PutPartnerEventsRequestEntryTypeDef",
     {
-        "EndpointId": str,
+        "Time": TimestampTypeDef,
+        "Source": str,
+        "Resources": Sequence[str],
+        "DetailType": str,
+        "Detail": str,
     },
     total=False,
 )
 
-class PutEventsRequestRequestTypeDef(
-    _RequiredPutEventsRequestRequestTypeDef, _OptionalPutEventsRequestRequestTypeDef
-):
-    pass
-
 PutEventsResponseTypeDef = TypedDict(
     "PutEventsResponseTypeDef",
     {
         "FailedEntryCount": int,
         "Entries": List[PutEventsResultEntryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutPartnerEventsRequestRequestTypeDef = TypedDict(
-    "PutPartnerEventsRequestRequestTypeDef",
-    {
-        "Entries": Sequence[PutPartnerEventsRequestEntryTypeDef],
-    },
-)
-
 PutPartnerEventsResponseTypeDef = TypedDict(
     "PutPartnerEventsResponseTypeDef",
     {
         "FailedEntryCount": int,
         "Entries": List[PutPartnerEventsResultEntryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2011,21 +1989,22 @@
     {
         "FailedEntryCount": int,
         "FailedEntries": List[RemoveTargetsResultEntryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ReplayDestinationUnionTypeDef = Union[ReplayDestinationTypeDef, ReplayDestinationOutputTypeDef]
 _RequiredStartReplayRequestRequestTypeDef = TypedDict(
     "_RequiredStartReplayRequestRequestTypeDef",
     {
         "ReplayName": str,
         "EventSourceArn": str,
-        "EventStartTime": Union[datetime, str],
-        "EventEndTime": Union[datetime, str],
+        "EventStartTime": TimestampTypeDef,
+        "EventEndTime": TimestampTypeDef,
         "Destination": ReplayDestinationTypeDef,
     },
 )
 _OptionalStartReplayRequestRequestTypeDef = TypedDict(
     "_OptionalStartReplayRequestRequestTypeDef",
     {
         "Description": str,
@@ -2175,14 +2154,40 @@
 RoutingConfigTypeDef = TypedDict(
     "RoutingConfigTypeDef",
     {
         "FailoverConfig": FailoverConfigTypeDef,
     },
 )
 
+_RequiredPutEventsRequestRequestTypeDef = TypedDict(
+    "_RequiredPutEventsRequestRequestTypeDef",
+    {
+        "Entries": Sequence[PutEventsRequestEntryTypeDef],
+    },
+)
+_OptionalPutEventsRequestRequestTypeDef = TypedDict(
+    "_OptionalPutEventsRequestRequestTypeDef",
+    {
+        "EndpointId": str,
+    },
+    total=False,
+)
+
+class PutEventsRequestRequestTypeDef(
+    _RequiredPutEventsRequestRequestTypeDef, _OptionalPutEventsRequestRequestTypeDef
+):
+    pass
+
+PutPartnerEventsRequestRequestTypeDef = TypedDict(
+    "PutPartnerEventsRequestRequestTypeDef",
+    {
+        "Entries": Sequence[PutPartnerEventsRequestEntryTypeDef],
+    },
+)
+
 _RequiredTargetOutputTypeDef = TypedDict(
     "_RequiredTargetOutputTypeDef",
     {
         "Id": str,
         "Arn": str,
     },
 )
@@ -2395,34 +2400,15 @@
     {
         "Targets": List[TargetOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredPutTargetsRequestRequestTypeDef = TypedDict(
-    "_RequiredPutTargetsRequestRequestTypeDef",
-    {
-        "Rule": str,
-        "Targets": Sequence[Union[TargetTypeDef, TargetOutputTypeDef]],
-    },
-)
-_OptionalPutTargetsRequestRequestTypeDef = TypedDict(
-    "_OptionalPutTargetsRequestRequestTypeDef",
-    {
-        "EventBusName": str,
-    },
-    total=False,
-)
-
-class PutTargetsRequestRequestTypeDef(
-    _RequiredPutTargetsRequestRequestTypeDef, _OptionalPutTargetsRequestRequestTypeDef
-):
-    pass
-
+TargetUnionTypeDef = Union[TargetTypeDef, TargetOutputTypeDef]
 DescribeConnectionResponseTypeDef = TypedDict(
     "DescribeConnectionResponseTypeDef",
     {
         "ConnectionArn": str,
         "Name": str,
         "Description": str,
         "ConnectionState": ConnectionStateType,
@@ -2483,7 +2469,27 @@
     "ListEndpointsResponseTypeDef",
     {
         "Endpoints": List[EndpointTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+
+_RequiredPutTargetsRequestRequestTypeDef = TypedDict(
+    "_RequiredPutTargetsRequestRequestTypeDef",
+    {
+        "Rule": str,
+        "Targets": Sequence[TargetUnionTypeDef],
+    },
+)
+_OptionalPutTargetsRequestRequestTypeDef = TypedDict(
+    "_OptionalPutTargetsRequestRequestTypeDef",
+    {
+        "EventBusName": str,
+    },
+    total=False,
+)
+
+class PutTargetsRequestRequestTypeDef(
+    _RequiredPutTargetsRequestRequestTypeDef, _OptionalPutTargetsRequestRequestTypeDef
+):
+    pass
```

### Comparing `mypy-boto3-events-1.28.15.post1/mypy_boto3_events.egg-info/PKG-INFO` & `mypy-boto3-events-1.28.16/mypy_boto3_events.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-events
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.EventBridge 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.EventBridge 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_events/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 events type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 events type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-events.svg?color=blue)](https://pypi.org/project/mypy-boto3-events)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_events/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-events)](https://pepy.tech/project/mypy-boto3-events)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EventBridge 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge)
+[boto3.EventBridge 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge)
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
 [mypy-boto3-events docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_events/).
 
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
@@ -337,20 +337,20 @@
 )
 
 
 def check_value(value: ApiDestinationHttpMethodType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_events.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_events.type_defs import (
     ActivateEventSourceRequestRequestTypeDef,
     ApiDestinationTypeDef,
     ArchiveTypeDef,
     AwsVpcConfigurationOutputTypeDef,
@@ -424,17 +424,16 @@
     ReplayTypeDef,
     PaginatorConfigTypeDef,
     ListRuleNamesByTargetRequestRequestTypeDef,
     ListRulesRequestRequestTypeDef,
     RuleTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTargetsByRuleRequestRequestTypeDef,
-    PutEventsRequestEntryTypeDef,
+    TimestampTypeDef,
     PutEventsResultEntryTypeDef,
-    PutPartnerEventsRequestEntryTypeDef,
     PutPartnerEventsResultEntryTypeDef,
     PutTargetsResultEntryTypeDef,
     RedshiftDataParametersOutputTypeDef,
     RedshiftDataParametersTypeDef,
     RemovePermissionRequestRequestTypeDef,
     RemoveTargetsRequestRequestTypeDef,
     RemoveTargetsResultEntryTypeDef,
@@ -493,52 +492,56 @@
     ListPartnerEventSourceAccountsResponseTypeDef,
     ListPartnerEventSourcesResponseTypeDef,
     ListReplaysResponseTypeDef,
     ListRuleNamesByTargetRequestListRuleNamesByTargetPaginateTypeDef,
     ListRulesRequestListRulesPaginateTypeDef,
     ListTargetsByRuleRequestListTargetsByRulePaginateTypeDef,
     ListRulesResponseTypeDef,
-    PutEventsRequestRequestTypeDef,
+    PutEventsRequestEntryTypeDef,
+    PutPartnerEventsRequestEntryTypeDef,
     PutEventsResponseTypeDef,
-    PutPartnerEventsRequestRequestTypeDef,
     PutPartnerEventsResponseTypeDef,
     PutTargetsResponseTypeDef,
     RemoveTargetsResponseTypeDef,
+    ReplayDestinationUnionTypeDef,
     StartReplayRequestRequestTypeDef,
     RunCommandParametersOutputTypeDef,
     RunCommandParametersTypeDef,
     SageMakerPipelineParametersOutputTypeDef,
     SageMakerPipelineParametersTypeDef,
     EcsParametersOutputTypeDef,
     EcsParametersTypeDef,
     ConnectionOAuthResponseParametersTypeDef,
     CreateConnectionOAuthRequestParametersTypeDef,
     UpdateConnectionOAuthRequestParametersTypeDef,
     RoutingConfigTypeDef,
+    PutEventsRequestRequestTypeDef,
+    PutPartnerEventsRequestRequestTypeDef,
     TargetOutputTypeDef,
     TargetTypeDef,
     ConnectionAuthResponseParametersTypeDef,
     CreateConnectionAuthRequestParametersTypeDef,
     UpdateConnectionAuthRequestParametersTypeDef,
     CreateEndpointRequestRequestTypeDef,
     CreateEndpointResponseTypeDef,
     DescribeEndpointResponseTypeDef,
     EndpointTypeDef,
     UpdateEndpointRequestRequestTypeDef,
     UpdateEndpointResponseTypeDef,
     ListTargetsByRuleResponseTypeDef,
-    PutTargetsRequestRequestTypeDef,
+    TargetUnionTypeDef,
     DescribeConnectionResponseTypeDef,
     CreateConnectionRequestRequestTypeDef,
     UpdateConnectionRequestRequestTypeDef,
     ListEndpointsResponseTypeDef,
+    PutTargetsRequestRequestTypeDef,
 )
 
 
-def get_structure() -> ActivateEventSourceRequestRequestTypeDef:
+def get_value() -> ActivateEventSourceRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-events-1.28.15.post1/mypy_boto3_events.egg-info/SOURCES.txt` & `mypy-boto3-events-1.28.16/mypy_boto3_events.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-events-1.28.15.post1/setup.py` & `mypy-boto3-events-1.28.16/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-events",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_events"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.EventBridge 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.2"
+        "Type annotations for boto3.EventBridge 1.28.16 service generated with mypy-boto3-builder"
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
-    keywords="boto3 events type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 events type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_events": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_events/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

