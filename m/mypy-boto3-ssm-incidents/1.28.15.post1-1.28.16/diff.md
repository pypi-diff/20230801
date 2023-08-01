# Comparing `tmp/mypy-boto3-ssm-incidents-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-ssm-incidents-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-ssm-incidents-1.28.15.post1.tar", last modified: Sat Jul 29 10:04:16 2023, max compression
+gzip compressed data, was "mypy-boto3-ssm-incidents-1.28.16.tar", last modified: Tue Aug  1 11:37:55 2023, max compression
```

## Comparing `mypy-boto3-ssm-incidents-1.28.15.post1.tar` & `mypy-boto3-ssm-incidents-1.28.16.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:16.089419 mypy-boto3-ssm-incidents-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 10:00:16.000000 mypy-boto3-ssm-incidents-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18407 2023-07-29 10:04:16.089419 mypy-boto3-ssm-incidents-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16891 2023-07-29 10:00:16.000000 mypy-boto3-ssm-incidents-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:16.085419 mypy-boto3-ssm-incidents-1.28.15.post1/mypy_boto3_ssm_incidents/
--rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-07-29 10:00:16.000000 mypy-boto3-ssm-incidents-1.28.15.post1/mypy_boto3_ssm_incidents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-07-29 10:00:16.000000 mypy-boto3-ssm-incidents-1.28.15.post1/mypy_boto3_ssm_incidents/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-29 10:00:16.000000 mypy-boto3-ssm-incidents-1.28.15.post1/mypy_boto3_ssm_incidents/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25970 2023-07-29 10:00:17.000000 mypy-boto3-ssm-incidents-1.28.15.post1/mypy_boto3_ssm_incidents/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    25926 2023-07-29 10:00:16.000000 mypy-boto3-ssm-incidents-1.28.15.post1/mypy_boto3_ssm_incidents/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10078 2023-07-29 10:00:17.000000 mypy-boto3-ssm-incidents-1.28.15.post1/mypy_boto3_ssm_incidents/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10076 2023-07-29 10:00:17.000000 mypy-boto3-ssm-incidents-1.28.15.post1/mypy_boto3_ssm_incidents/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7893 2023-07-29 10:00:17.000000 mypy-boto3-ssm-incidents-1.28.15.post1/mypy_boto3_ssm_incidents/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-07-29 10:00:17.000000 mypy-boto3-ssm-incidents-1.28.15.post1/mypy_boto3_ssm_incidents/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 10:00:16.000000 mypy-boto3-ssm-incidents-1.28.15.post1/mypy_boto3_ssm_incidents/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    35608 2023-07-29 10:00:18.000000 mypy-boto3-ssm-incidents-1.28.15.post1/mypy_boto3_ssm_incidents/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    35540 2023-07-29 10:00:17.000000 mypy-boto3-ssm-incidents-1.28.15.post1/mypy_boto3_ssm_incidents/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 10:00:16.000000 mypy-boto3-ssm-incidents-1.28.15.post1/mypy_boto3_ssm_incidents/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-07-29 10:00:17.000000 mypy-boto3-ssm-incidents-1.28.15.post1/mypy_boto3_ssm_incidents/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-07-29 10:00:17.000000 mypy-boto3-ssm-incidents-1.28.15.post1/mypy_boto3_ssm_incidents/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:16.089419 mypy-boto3-ssm-incidents-1.28.15.post1/mypy_boto3_ssm_incidents.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18407 2023-07-29 10:04:15.000000 mypy-boto3-ssm-incidents-1.28.15.post1/mypy_boto3_ssm_incidents.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-29 10:04:15.000000 mypy-boto3-ssm-incidents-1.28.15.post1/mypy_boto3_ssm_incidents.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:15.000000 mypy-boto3-ssm-incidents-1.28.15.post1/mypy_boto3_ssm_incidents.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:15.000000 mypy-boto3-ssm-incidents-1.28.15.post1/mypy_boto3_ssm_incidents.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:04:15.000000 mypy-boto3-ssm-incidents-1.28.15.post1/mypy_boto3_ssm_incidents.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-29 10:04:15.000000 mypy-boto3-ssm-incidents-1.28.15.post1/mypy_boto3_ssm_incidents.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:04:16.089419 mypy-boto3-ssm-incidents-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-07-29 10:00:16.000000 mypy-boto3-ssm-incidents-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:55.332720 mypy-boto3-ssm-incidents-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:33:51.000000 mypy-boto3-ssm-incidents-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18506 2023-08-01 11:37:55.328720 mypy-boto3-ssm-incidents-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16999 2023-08-01 11:33:51.000000 mypy-boto3-ssm-incidents-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:55.316720 mypy-boto3-ssm-incidents-1.28.16/mypy_boto3_ssm_incidents/
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-08-01 11:33:51.000000 mypy-boto3-ssm-incidents-1.28.16/mypy_boto3_ssm_incidents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-08-01 11:33:51.000000 mypy-boto3-ssm-incidents-1.28.16/mypy_boto3_ssm_incidents/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-08-01 11:33:51.000000 mypy-boto3-ssm-incidents-1.28.16/mypy_boto3_ssm_incidents/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25709 2023-08-01 11:33:51.000000 mypy-boto3-ssm-incidents-1.28.16/mypy_boto3_ssm_incidents/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25665 2023-08-01 11:33:51.000000 mypy-boto3-ssm-incidents-1.28.16/mypy_boto3_ssm_incidents/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10078 2023-08-01 11:33:52.000000 mypy-boto3-ssm-incidents-1.28.16/mypy_boto3_ssm_incidents/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10076 2023-08-01 11:33:52.000000 mypy-boto3-ssm-incidents-1.28.16/mypy_boto3_ssm_incidents/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7893 2023-08-01 11:33:52.000000 mypy-boto3-ssm-incidents-1.28.16/mypy_boto3_ssm_incidents/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-08-01 11:33:52.000000 mypy-boto3-ssm-incidents-1.28.16/mypy_boto3_ssm_incidents/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:33:51.000000 mypy-boto3-ssm-incidents-1.28.16/mypy_boto3_ssm_incidents/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    35931 2023-08-01 11:33:53.000000 mypy-boto3-ssm-incidents-1.28.16/mypy_boto3_ssm_incidents/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35863 2023-08-01 11:33:52.000000 mypy-boto3-ssm-incidents-1.28.16/mypy_boto3_ssm_incidents/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:33:51.000000 mypy-boto3-ssm-incidents-1.28.16/mypy_boto3_ssm_incidents/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-08-01 11:33:52.000000 mypy-boto3-ssm-incidents-1.28.16/mypy_boto3_ssm_incidents/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-08-01 11:33:52.000000 mypy-boto3-ssm-incidents-1.28.16/mypy_boto3_ssm_incidents/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:55.328720 mypy-boto3-ssm-incidents-1.28.16/mypy_boto3_ssm_incidents.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18506 2023-08-01 11:37:55.000000 mypy-boto3-ssm-incidents-1.28.16/mypy_boto3_ssm_incidents.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-08-01 11:37:55.000000 mypy-boto3-ssm-incidents-1.28.16/mypy_boto3_ssm_incidents.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:55.000000 mypy-boto3-ssm-incidents-1.28.16/mypy_boto3_ssm_incidents.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:55.000000 mypy-boto3-ssm-incidents-1.28.16/mypy_boto3_ssm_incidents.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:55.000000 mypy-boto3-ssm-incidents-1.28.16/mypy_boto3_ssm_incidents.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-01 11:37:55.000000 mypy-boto3-ssm-incidents-1.28.16/mypy_boto3_ssm_incidents.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:55.332720 mypy-boto3-ssm-incidents-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-08-01 11:33:51.000000 mypy-boto3-ssm-incidents-1.28.16/setup.py
```

### Comparing `mypy-boto3-ssm-incidents-1.28.15.post1/LICENSE` & `mypy-boto3-ssm-incidents-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-incidents-1.28.15.post1/PKG-INFO` & `mypy-boto3-ssm-incidents-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ssm-incidents
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.SSMIncidents 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.SSMIncidents 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 ssm-incidents type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 ssm-incidents type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ssm-incidents.svg?color=blue)](https://pypi.org/project/mypy-boto3-ssm-incidents)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ssm-incidents)](https://pepy.tech/project/mypy-boto3-ssm-incidents)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SSMIncidents 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents)
+[boto3.SSMIncidents 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents)
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
 [mypy-boto3-ssm-incidents docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/).
 
 See how it helps to find and fix potential bugs:
 
@@ -75,15 +75,15 @@
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Waiters annotations](#waiters-annotations)
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
@@ -377,28 +377,29 @@
 )
 
 
 def check_value(value: GetResourcePoliciesPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_ssm_incidents.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_ssm_incidents.type_defs import (
     AddRegionActionTypeDef,
     AttributeValueListTypeDef,
     AutomationExecutionTypeDef,
     ChatChannelOutputTypeDef,
     ChatChannelTypeDef,
+    TimestampTypeDef,
     RegionMapInputValueTypeDef,
     ResponseMetadataTypeDef,
     EventReferenceTypeDef,
     DeleteIncidentRecordInputRequestTypeDef,
     DeleteRegionActionTypeDef,
     DeleteReplicationSetInputRequestTypeDef,
     DeleteResourcePolicyInputRequestTypeDef,
@@ -420,19 +421,20 @@
     ListReplicationSetsInputRequestTypeDef,
     ListResponsePlansInputRequestTypeDef,
     ResponsePlanSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     PagerDutyIncidentConfigurationTypeDef,
     PutResourcePolicyInputRequestTypeDef,
     RegionInfoTypeDef,
-    TriggerDetailsTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDeletionProtectionInputRequestTypeDef,
+    ChatChannelUnionTypeDef,
     ConditionTypeDef,
+    TriggerDetailsTypeDef,
     CreateReplicationSetInputRequestTypeDef,
     CreateReplicationSetOutputTypeDef,
     CreateResponsePlanOutputTypeDef,
     CreateTimelineEventOutputTypeDef,
     ListReplicationSetsOutputTypeDef,
     ListTagsForResourceResponseTypeDef,
     PutResourcePolicyOutputTypeDef,
@@ -464,33 +466,35 @@
     ListTimelineEventsOutputTypeDef,
     GetTimelineEventOutputTypeDef,
     UpdateReplicationSetInputRequestTypeDef,
     ActionOutputTypeDef,
     ActionTypeDef,
     ListIncidentRecordsOutputTypeDef,
     GetIncidentRecordOutputTypeDef,
+    IncidentTemplateUnionTypeDef,
     ItemIdentifierTypeDef,
     IntegrationTypeDef,
     GetReplicationSetOutputTypeDef,
     ListIncidentRecordsInputListIncidentRecordsPaginateTypeDef,
     ListIncidentRecordsInputRequestTypeDef,
     ListTimelineEventsInputListTimelineEventsPaginateTypeDef,
     ListTimelineEventsInputRequestTypeDef,
+    ActionUnionTypeDef,
     RelatedItemTypeDef,
-    CreateResponsePlanInputRequestTypeDef,
     GetResponsePlanOutputTypeDef,
+    CreateResponsePlanInputRequestTypeDef,
     UpdateResponsePlanInputRequestTypeDef,
     ListRelatedItemsOutputTypeDef,
     RelatedItemsUpdateTypeDef,
     StartIncidentInputRequestTypeDef,
     UpdateRelatedItemsInputRequestTypeDef,
 )
 
 
-def get_structure() -> AddRegionActionTypeDef:
+def get_value() -> AddRegionActionTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-ssm-incidents-1.28.15.post1/README.md` & `mypy-boto3-ssm-incidents-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ssm-incidents.svg?color=blue)](https://pypi.org/project/mypy-boto3-ssm-incidents)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ssm-incidents)](https://pepy.tech/project/mypy-boto3-ssm-incidents)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SSMIncidents 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents)
+[boto3.SSMIncidents 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents)
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
 [mypy-boto3-ssm-incidents docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/).
 
 See how it helps to find and fix potential bugs:
 
@@ -43,15 +43,15 @@
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Waiters annotations](#waiters-annotations)
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
@@ -345,28 +345,29 @@
 )
 
 
 def check_value(value: GetResourcePoliciesPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_ssm_incidents.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_ssm_incidents.type_defs import (
     AddRegionActionTypeDef,
     AttributeValueListTypeDef,
     AutomationExecutionTypeDef,
     ChatChannelOutputTypeDef,
     ChatChannelTypeDef,
+    TimestampTypeDef,
     RegionMapInputValueTypeDef,
     ResponseMetadataTypeDef,
     EventReferenceTypeDef,
     DeleteIncidentRecordInputRequestTypeDef,
     DeleteRegionActionTypeDef,
     DeleteReplicationSetInputRequestTypeDef,
     DeleteResourcePolicyInputRequestTypeDef,
@@ -388,19 +389,20 @@
     ListReplicationSetsInputRequestTypeDef,
     ListResponsePlansInputRequestTypeDef,
     ResponsePlanSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     PagerDutyIncidentConfigurationTypeDef,
     PutResourcePolicyInputRequestTypeDef,
     RegionInfoTypeDef,
-    TriggerDetailsTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDeletionProtectionInputRequestTypeDef,
+    ChatChannelUnionTypeDef,
     ConditionTypeDef,
+    TriggerDetailsTypeDef,
     CreateReplicationSetInputRequestTypeDef,
     CreateReplicationSetOutputTypeDef,
     CreateResponsePlanOutputTypeDef,
     CreateTimelineEventOutputTypeDef,
     ListReplicationSetsOutputTypeDef,
     ListTagsForResourceResponseTypeDef,
     PutResourcePolicyOutputTypeDef,
@@ -432,33 +434,35 @@
     ListTimelineEventsOutputTypeDef,
     GetTimelineEventOutputTypeDef,
     UpdateReplicationSetInputRequestTypeDef,
     ActionOutputTypeDef,
     ActionTypeDef,
     ListIncidentRecordsOutputTypeDef,
     GetIncidentRecordOutputTypeDef,
+    IncidentTemplateUnionTypeDef,
     ItemIdentifierTypeDef,
     IntegrationTypeDef,
     GetReplicationSetOutputTypeDef,
     ListIncidentRecordsInputListIncidentRecordsPaginateTypeDef,
     ListIncidentRecordsInputRequestTypeDef,
     ListTimelineEventsInputListTimelineEventsPaginateTypeDef,
     ListTimelineEventsInputRequestTypeDef,
+    ActionUnionTypeDef,
     RelatedItemTypeDef,
-    CreateResponsePlanInputRequestTypeDef,
     GetResponsePlanOutputTypeDef,
+    CreateResponsePlanInputRequestTypeDef,
     UpdateResponsePlanInputRequestTypeDef,
     ListRelatedItemsOutputTypeDef,
     RelatedItemsUpdateTypeDef,
     StartIncidentInputRequestTypeDef,
     UpdateRelatedItemsInputRequestTypeDef,
 )
 
 
-def get_structure() -> AddRegionActionTypeDef:
+def get_value() -> AddRegionActionTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-ssm-incidents-1.28.15.post1/mypy_boto3_ssm_incidents/__init__.py` & `mypy-boto3-ssm-incidents-1.28.16/mypy_boto3_ssm_incidents/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-incidents-1.28.15.post1/mypy_boto3_ssm_incidents/__init__.pyi` & `mypy-boto3-ssm-incidents-1.28.16/mypy_boto3_ssm_incidents/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-incidents-1.28.15.post1/mypy_boto3_ssm_incidents/__main__.py` & `mypy-boto3-ssm-incidents-1.28.16/mypy_boto3_ssm_incidents/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SSMIncidents 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.SSMIncidents 1.28.16\nVersion:         1.28.16\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents\nOther"
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

### Comparing `mypy-boto3-ssm-incidents-1.28.15.post1/mypy_boto3_ssm_incidents/client.py` & `mypy-boto3-ssm-incidents-1.28.16/mypy_boto3_ssm_incidents/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,58 +10,55 @@
     from mypy_boto3_ssm_incidents.client import SSMIncidentsClient
 
     session = Session()
     client: SSMIncidentsClient = session.client("ssm-incidents")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import IncidentRecordStatusType, SortOrderType
 from .paginator import (
     GetResourcePoliciesPaginator,
     ListIncidentRecordsPaginator,
     ListRelatedItemsPaginator,
     ListReplicationSetsPaginator,
     ListResponsePlansPaginator,
     ListTimelineEventsPaginator,
 )
 from .type_defs import (
-    ActionOutputTypeDef,
-    ActionTypeDef,
-    ChatChannelOutputTypeDef,
-    ChatChannelTypeDef,
+    ActionUnionTypeDef,
+    ChatChannelUnionTypeDef,
     CreateReplicationSetOutputTypeDef,
     CreateResponsePlanOutputTypeDef,
     CreateTimelineEventOutputTypeDef,
     EventReferenceTypeDef,
     FilterTypeDef,
     GetIncidentRecordOutputTypeDef,
     GetReplicationSetOutputTypeDef,
     GetResourcePoliciesOutputTypeDef,
     GetResponsePlanOutputTypeDef,
     GetTimelineEventOutputTypeDef,
-    IncidentTemplateOutputTypeDef,
-    IncidentTemplateTypeDef,
+    IncidentTemplateUnionTypeDef,
     IntegrationTypeDef,
     ListIncidentRecordsOutputTypeDef,
     ListRelatedItemsOutputTypeDef,
     ListReplicationSetsOutputTypeDef,
     ListResponsePlansOutputTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTimelineEventsOutputTypeDef,
     NotificationTargetItemTypeDef,
     PutResourcePolicyOutputTypeDef,
     RegionMapInputValueTypeDef,
     RelatedItemsUpdateTypeDef,
     RelatedItemTypeDef,
     StartIncidentOutputTypeDef,
+    TimestampTypeDef,
     TriggerDetailsTypeDef,
     UpdateReplicationSetActionTypeDef,
 )
 from .waiter import WaitForReplicationSetActiveWaiter, WaitForReplicationSetDeletedWaiter
 
 if sys.version_info >= (3, 9):
     from typing import Literal
@@ -138,18 +135,18 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.create_replication_set)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/client/#create_replication_set)
         """
 
     def create_response_plan(
         self,
         *,
-        incidentTemplate: Union[IncidentTemplateTypeDef, IncidentTemplateOutputTypeDef],
+        incidentTemplate: IncidentTemplateUnionTypeDef,
         name: str,
-        actions: Sequence[Union[ActionTypeDef, ActionOutputTypeDef]] = ...,
-        chatChannel: Union[ChatChannelTypeDef, ChatChannelOutputTypeDef] = ...,
+        actions: Sequence[ActionUnionTypeDef] = ...,
+        chatChannel: ChatChannelUnionTypeDef = ...,
         clientToken: str = ...,
         displayName: str = ...,
         engagements: Sequence[str] = ...,
         integrations: Sequence[IntegrationTypeDef] = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateResponsePlanOutputTypeDef:
         """
@@ -159,15 +156,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/client/#create_response_plan)
         """
 
     def create_timeline_event(
         self,
         *,
         eventData: str,
-        eventTime: Union[datetime, str],
+        eventTime: TimestampTypeDef,
         eventType: str,
         incidentRecordArn: str,
         clientToken: str = ...,
         eventReferences: Sequence[EventReferenceTypeDef] = ...
     ) -> CreateTimelineEventOutputTypeDef:
         """
         Creates a custom timeline event on the incident details page of an incident
@@ -396,15 +393,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/client/#update_deletion_protection)
         """
 
     def update_incident_record(
         self,
         *,
         arn: str,
-        chatChannel: Union[ChatChannelTypeDef, ChatChannelOutputTypeDef] = ...,
+        chatChannel: ChatChannelUnionTypeDef = ...,
         clientToken: str = ...,
         impact: int = ...,
         notificationTargets: Sequence[NotificationTargetItemTypeDef] = ...,
         status: IncidentRecordStatusType = ...,
         summary: str = ...,
         title: str = ...
     ) -> Dict[str, Any]:
@@ -443,16 +440,16 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/client/#update_replication_set)
         """
 
     def update_response_plan(
         self,
         *,
         arn: str,
-        actions: Sequence[Union[ActionTypeDef, ActionOutputTypeDef]] = ...,
-        chatChannel: Union[ChatChannelTypeDef, ChatChannelOutputTypeDef] = ...,
+        actions: Sequence[ActionUnionTypeDef] = ...,
+        chatChannel: ChatChannelUnionTypeDef = ...,
         clientToken: str = ...,
         displayName: str = ...,
         engagements: Sequence[str] = ...,
         incidentTemplateDedupeString: str = ...,
         incidentTemplateImpact: int = ...,
         incidentTemplateNotificationTargets: Sequence[NotificationTargetItemTypeDef] = ...,
         incidentTemplateSummary: str = ...,
@@ -471,15 +468,15 @@
         self,
         *,
         eventId: str,
         incidentRecordArn: str,
         clientToken: str = ...,
         eventData: str = ...,
         eventReferences: Sequence[EventReferenceTypeDef] = ...,
-        eventTime: Union[datetime, str] = ...,
+        eventTime: TimestampTypeDef = ...,
         eventType: str = ...
     ) -> Dict[str, Any]:
         """
         Updates a timeline event.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.update_timeline_event)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/client/#update_timeline_event)
```

### Comparing `mypy-boto3-ssm-incidents-1.28.15.post1/mypy_boto3_ssm_incidents/client.pyi` & `mypy-boto3-ssm-incidents-1.28.16/mypy_boto3_ssm_incidents/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -10,58 +10,55 @@
     from mypy_boto3_ssm_incidents.client import SSMIncidentsClient
 
     session = Session()
     client: SSMIncidentsClient = session.client("ssm-incidents")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import IncidentRecordStatusType, SortOrderType
 from .paginator import (
     GetResourcePoliciesPaginator,
     ListIncidentRecordsPaginator,
     ListRelatedItemsPaginator,
     ListReplicationSetsPaginator,
     ListResponsePlansPaginator,
     ListTimelineEventsPaginator,
 )
 from .type_defs import (
-    ActionOutputTypeDef,
-    ActionTypeDef,
-    ChatChannelOutputTypeDef,
-    ChatChannelTypeDef,
+    ActionUnionTypeDef,
+    ChatChannelUnionTypeDef,
     CreateReplicationSetOutputTypeDef,
     CreateResponsePlanOutputTypeDef,
     CreateTimelineEventOutputTypeDef,
     EventReferenceTypeDef,
     FilterTypeDef,
     GetIncidentRecordOutputTypeDef,
     GetReplicationSetOutputTypeDef,
     GetResourcePoliciesOutputTypeDef,
     GetResponsePlanOutputTypeDef,
     GetTimelineEventOutputTypeDef,
-    IncidentTemplateOutputTypeDef,
-    IncidentTemplateTypeDef,
+    IncidentTemplateUnionTypeDef,
     IntegrationTypeDef,
     ListIncidentRecordsOutputTypeDef,
     ListRelatedItemsOutputTypeDef,
     ListReplicationSetsOutputTypeDef,
     ListResponsePlansOutputTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTimelineEventsOutputTypeDef,
     NotificationTargetItemTypeDef,
     PutResourcePolicyOutputTypeDef,
     RegionMapInputValueTypeDef,
     RelatedItemsUpdateTypeDef,
     RelatedItemTypeDef,
     StartIncidentOutputTypeDef,
+    TimestampTypeDef,
     TriggerDetailsTypeDef,
     UpdateReplicationSetActionTypeDef,
 )
 from .waiter import WaitForReplicationSetActiveWaiter, WaitForReplicationSetDeletedWaiter
 
 if sys.version_info >= (3, 9):
     from typing import Literal
@@ -130,18 +127,18 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.create_replication_set)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/client/#create_replication_set)
         """
     def create_response_plan(
         self,
         *,
-        incidentTemplate: Union[IncidentTemplateTypeDef, IncidentTemplateOutputTypeDef],
+        incidentTemplate: IncidentTemplateUnionTypeDef,
         name: str,
-        actions: Sequence[Union[ActionTypeDef, ActionOutputTypeDef]] = ...,
-        chatChannel: Union[ChatChannelTypeDef, ChatChannelOutputTypeDef] = ...,
+        actions: Sequence[ActionUnionTypeDef] = ...,
+        chatChannel: ChatChannelUnionTypeDef = ...,
         clientToken: str = ...,
         displayName: str = ...,
         engagements: Sequence[str] = ...,
         integrations: Sequence[IntegrationTypeDef] = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateResponsePlanOutputTypeDef:
         """
@@ -150,15 +147,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.create_response_plan)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/client/#create_response_plan)
         """
     def create_timeline_event(
         self,
         *,
         eventData: str,
-        eventTime: Union[datetime, str],
+        eventTime: TimestampTypeDef,
         eventType: str,
         incidentRecordArn: str,
         clientToken: str = ...,
         eventReferences: Sequence[EventReferenceTypeDef] = ...
     ) -> CreateTimelineEventOutputTypeDef:
         """
         Creates a custom timeline event on the incident details page of an incident
@@ -364,15 +361,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.update_deletion_protection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/client/#update_deletion_protection)
         """
     def update_incident_record(
         self,
         *,
         arn: str,
-        chatChannel: Union[ChatChannelTypeDef, ChatChannelOutputTypeDef] = ...,
+        chatChannel: ChatChannelUnionTypeDef = ...,
         clientToken: str = ...,
         impact: int = ...,
         notificationTargets: Sequence[NotificationTargetItemTypeDef] = ...,
         status: IncidentRecordStatusType = ...,
         summary: str = ...,
         title: str = ...
     ) -> Dict[str, Any]:
@@ -408,16 +405,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.update_replication_set)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/client/#update_replication_set)
         """
     def update_response_plan(
         self,
         *,
         arn: str,
-        actions: Sequence[Union[ActionTypeDef, ActionOutputTypeDef]] = ...,
-        chatChannel: Union[ChatChannelTypeDef, ChatChannelOutputTypeDef] = ...,
+        actions: Sequence[ActionUnionTypeDef] = ...,
+        chatChannel: ChatChannelUnionTypeDef = ...,
         clientToken: str = ...,
         displayName: str = ...,
         engagements: Sequence[str] = ...,
         incidentTemplateDedupeString: str = ...,
         incidentTemplateImpact: int = ...,
         incidentTemplateNotificationTargets: Sequence[NotificationTargetItemTypeDef] = ...,
         incidentTemplateSummary: str = ...,
@@ -435,15 +432,15 @@
         self,
         *,
         eventId: str,
         incidentRecordArn: str,
         clientToken: str = ...,
         eventData: str = ...,
         eventReferences: Sequence[EventReferenceTypeDef] = ...,
-        eventTime: Union[datetime, str] = ...,
+        eventTime: TimestampTypeDef = ...,
         eventType: str = ...
     ) -> Dict[str, Any]:
         """
         Updates a timeline event.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client.update_timeline_event)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/client/#update_timeline_event)
```

### Comparing `mypy-boto3-ssm-incidents-1.28.15.post1/mypy_boto3_ssm_incidents/literals.py` & `mypy-boto3-ssm-incidents-1.28.16/mypy_boto3_ssm_incidents/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-incidents-1.28.15.post1/mypy_boto3_ssm_incidents/literals.pyi` & `mypy-boto3-ssm-incidents-1.28.16/mypy_boto3_ssm_incidents/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-incidents-1.28.15.post1/mypy_boto3_ssm_incidents/paginator.py` & `mypy-boto3-ssm-incidents-1.28.16/mypy_boto3_ssm_incidents/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-incidents-1.28.15.post1/mypy_boto3_ssm_incidents/paginator.pyi` & `mypy-boto3-ssm-incidents-1.28.16/mypy_boto3_ssm_incidents/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-incidents-1.28.15.post1/mypy_boto3_ssm_incidents/type_defs.py` & `mypy-boto3-ssm-incidents-1.28.16/mypy_boto3_ssm_incidents/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_ssm_incidents.type_defs import AddRegionActionTypeDef
 
-    data: AddRegionActionTypeDef = {...}
+    data: AddRegionActionTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -30,21 +30,21 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AddRegionActionTypeDef",
     "AttributeValueListTypeDef",
     "AutomationExecutionTypeDef",
     "ChatChannelOutputTypeDef",
     "ChatChannelTypeDef",
+    "TimestampTypeDef",
     "RegionMapInputValueTypeDef",
     "ResponseMetadataTypeDef",
     "EventReferenceTypeDef",
     "DeleteIncidentRecordInputRequestTypeDef",
     "DeleteRegionActionTypeDef",
     "DeleteReplicationSetInputRequestTypeDef",
     "DeleteResourcePolicyInputRequestTypeDef",
@@ -66,19 +66,20 @@
     "ListReplicationSetsInputRequestTypeDef",
     "ListResponsePlansInputRequestTypeDef",
     "ResponsePlanSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "PagerDutyIncidentConfigurationTypeDef",
     "PutResourcePolicyInputRequestTypeDef",
     "RegionInfoTypeDef",
-    "TriggerDetailsTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDeletionProtectionInputRequestTypeDef",
+    "ChatChannelUnionTypeDef",
     "ConditionTypeDef",
+    "TriggerDetailsTypeDef",
     "CreateReplicationSetInputRequestTypeDef",
     "CreateReplicationSetOutputTypeDef",
     "CreateResponsePlanOutputTypeDef",
     "CreateTimelineEventOutputTypeDef",
     "ListReplicationSetsOutputTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "PutResourcePolicyOutputTypeDef",
@@ -110,24 +111,26 @@
     "ListTimelineEventsOutputTypeDef",
     "GetTimelineEventOutputTypeDef",
     "UpdateReplicationSetInputRequestTypeDef",
     "ActionOutputTypeDef",
     "ActionTypeDef",
     "ListIncidentRecordsOutputTypeDef",
     "GetIncidentRecordOutputTypeDef",
+    "IncidentTemplateUnionTypeDef",
     "ItemIdentifierTypeDef",
     "IntegrationTypeDef",
     "GetReplicationSetOutputTypeDef",
     "ListIncidentRecordsInputListIncidentRecordsPaginateTypeDef",
     "ListIncidentRecordsInputRequestTypeDef",
     "ListTimelineEventsInputListTimelineEventsPaginateTypeDef",
     "ListTimelineEventsInputRequestTypeDef",
+    "ActionUnionTypeDef",
     "RelatedItemTypeDef",
-    "CreateResponsePlanInputRequestTypeDef",
     "GetResponsePlanOutputTypeDef",
+    "CreateResponsePlanInputRequestTypeDef",
     "UpdateResponsePlanInputRequestTypeDef",
     "ListRelatedItemsOutputTypeDef",
     "RelatedItemsUpdateTypeDef",
     "StartIncidentInputRequestTypeDef",
     "UpdateRelatedItemsInputRequestTypeDef",
 )
 
@@ -141,19 +144,17 @@
     "_OptionalAddRegionActionTypeDef",
     {
         "sseKmsKeyId": str,
     },
     total=False,
 )
 
-
 class AddRegionActionTypeDef(_RequiredAddRegionActionTypeDef, _OptionalAddRegionActionTypeDef):
     pass
 
-
 AttributeValueListTypeDef = TypedDict(
     "AttributeValueListTypeDef",
     {
         "integerValues": Sequence[int],
         "stringValues": Sequence[str],
     },
     total=False,
@@ -181,14 +182,15 @@
     {
         "chatbotSns": Sequence[str],
         "empty": Mapping[str, Any],
     },
     total=False,
 )
 
+TimestampTypeDef = Union[datetime, str]
 RegionMapInputValueTypeDef = TypedDict(
     "RegionMapInputValueTypeDef",
     {
         "sseKmsKeyId": str,
     },
     total=False,
 )
@@ -309,21 +311,19 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class GetResourcePoliciesInputRequestTypeDef(
     _RequiredGetResourcePoliciesInputRequestTypeDef, _OptionalGetResourcePoliciesInputRequestTypeDef
 ):
     pass
 
-
 ResourcePolicyTypeDef = TypedDict(
     "ResourcePolicyTypeDef",
     {
         "policyDocument": str,
         "policyId": str,
         "ramResourceShareRegion": str,
     },
@@ -356,21 +356,19 @@
     {
         "invokedBy": str,
         "resourceArn": str,
     },
     total=False,
 )
 
-
 class IncidentRecordSourceTypeDef(
     _RequiredIncidentRecordSourceTypeDef, _OptionalIncidentRecordSourceTypeDef
 ):
     pass
 
-
 NotificationTargetItemTypeDef = TypedDict(
     "NotificationTargetItemTypeDef",
     {
         "snsTopicArn": str,
     },
     total=False,
 )
@@ -386,21 +384,19 @@
     {
         "autoResolve": bool,
         "secretId": str,
     },
     total=False,
 )
 
-
 class PagerDutyIncidentDetailTypeDef(
     _RequiredPagerDutyIncidentDetailTypeDef, _OptionalPagerDutyIncidentDetailTypeDef
 ):
     pass
 
-
 _RequiredListRelatedItemsInputRequestTypeDef = TypedDict(
     "_RequiredListRelatedItemsInputRequestTypeDef",
     {
         "incidentRecordArn": str,
     },
 )
 _OptionalListRelatedItemsInputRequestTypeDef = TypedDict(
@@ -408,21 +404,19 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListRelatedItemsInputRequestTypeDef(
     _RequiredListRelatedItemsInputRequestTypeDef, _OptionalListRelatedItemsInputRequestTypeDef
 ):
     pass
 
-
 ListReplicationSetsInputRequestTypeDef = TypedDict(
     "ListReplicationSetsInputRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -448,21 +442,19 @@
     "_OptionalResponsePlanSummaryTypeDef",
     {
         "displayName": str,
     },
     total=False,
 )
 
-
 class ResponsePlanSummaryTypeDef(
     _RequiredResponsePlanSummaryTypeDef, _OptionalResponsePlanSummaryTypeDef
 ):
     pass
 
-
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
@@ -493,40 +485,17 @@
     {
         "sseKmsKeyId": str,
         "statusMessage": str,
     },
     total=False,
 )
 
-
 class RegionInfoTypeDef(_RequiredRegionInfoTypeDef, _OptionalRegionInfoTypeDef):
     pass
 
-
-_RequiredTriggerDetailsTypeDef = TypedDict(
-    "_RequiredTriggerDetailsTypeDef",
-    {
-        "source": str,
-        "timestamp": Union[datetime, str],
-    },
-)
-_OptionalTriggerDetailsTypeDef = TypedDict(
-    "_OptionalTriggerDetailsTypeDef",
-    {
-        "rawData": str,
-        "triggerArn": str,
-    },
-    total=False,
-)
-
-
-class TriggerDetailsTypeDef(_RequiredTriggerDetailsTypeDef, _OptionalTriggerDetailsTypeDef):
-    pass
-
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -550,32 +519,50 @@
     "_OptionalUpdateDeletionProtectionInputRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
-
 class UpdateDeletionProtectionInputRequestTypeDef(
     _RequiredUpdateDeletionProtectionInputRequestTypeDef,
     _OptionalUpdateDeletionProtectionInputRequestTypeDef,
 ):
     pass
 
-
+ChatChannelUnionTypeDef = Union[ChatChannelTypeDef, ChatChannelOutputTypeDef]
 ConditionTypeDef = TypedDict(
     "ConditionTypeDef",
     {
-        "after": Union[datetime, str],
-        "before": Union[datetime, str],
+        "after": TimestampTypeDef,
+        "before": TimestampTypeDef,
         "equals": AttributeValueListTypeDef,
     },
     total=False,
 )
 
+_RequiredTriggerDetailsTypeDef = TypedDict(
+    "_RequiredTriggerDetailsTypeDef",
+    {
+        "source": str,
+        "timestamp": TimestampTypeDef,
+    },
+)
+_OptionalTriggerDetailsTypeDef = TypedDict(
+    "_OptionalTriggerDetailsTypeDef",
+    {
+        "rawData": str,
+        "triggerArn": str,
+    },
+    total=False,
+)
+
+class TriggerDetailsTypeDef(_RequiredTriggerDetailsTypeDef, _OptionalTriggerDetailsTypeDef):
+    pass
+
 _RequiredCreateReplicationSetInputRequestTypeDef = TypedDict(
     "_RequiredCreateReplicationSetInputRequestTypeDef",
     {
         "regions": Mapping[str, RegionMapInputValueTypeDef],
     },
 )
 _OptionalCreateReplicationSetInputRequestTypeDef = TypedDict(
@@ -583,22 +570,20 @@
     {
         "clientToken": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateReplicationSetInputRequestTypeDef(
     _RequiredCreateReplicationSetInputRequestTypeDef,
     _OptionalCreateReplicationSetInputRequestTypeDef,
 ):
     pass
 
-
 CreateReplicationSetOutputTypeDef = TypedDict(
     "CreateReplicationSetOutputTypeDef",
     {
         "arn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -653,35 +638,33 @@
     },
 )
 
 _RequiredCreateTimelineEventInputRequestTypeDef = TypedDict(
     "_RequiredCreateTimelineEventInputRequestTypeDef",
     {
         "eventData": str,
-        "eventTime": Union[datetime, str],
+        "eventTime": TimestampTypeDef,
         "eventType": str,
         "incidentRecordArn": str,
     },
 )
 _OptionalCreateTimelineEventInputRequestTypeDef = TypedDict(
     "_OptionalCreateTimelineEventInputRequestTypeDef",
     {
         "clientToken": str,
         "eventReferences": Sequence[EventReferenceTypeDef],
     },
     total=False,
 )
 
-
 class CreateTimelineEventInputRequestTypeDef(
     _RequiredCreateTimelineEventInputRequestTypeDef, _OptionalCreateTimelineEventInputRequestTypeDef
 ):
     pass
 
-
 _RequiredEventSummaryTypeDef = TypedDict(
     "_RequiredEventSummaryTypeDef",
     {
         "eventId": str,
         "eventTime": datetime,
         "eventType": str,
         "eventUpdatedTime": datetime,
@@ -692,19 +675,17 @@
     "_OptionalEventSummaryTypeDef",
     {
         "eventReferences": List[EventReferenceTypeDef],
     },
     total=False,
 )
 
-
 class EventSummaryTypeDef(_RequiredEventSummaryTypeDef, _OptionalEventSummaryTypeDef):
     pass
 
-
 _RequiredTimelineEventTypeDef = TypedDict(
     "_RequiredTimelineEventTypeDef",
     {
         "eventData": str,
         "eventId": str,
         "eventTime": datetime,
         "eventType": str,
@@ -716,45 +697,41 @@
     "_OptionalTimelineEventTypeDef",
     {
         "eventReferences": List[EventReferenceTypeDef],
     },
     total=False,
 )
 
-
 class TimelineEventTypeDef(_RequiredTimelineEventTypeDef, _OptionalTimelineEventTypeDef):
     pass
 
-
 _RequiredUpdateTimelineEventInputRequestTypeDef = TypedDict(
     "_RequiredUpdateTimelineEventInputRequestTypeDef",
     {
         "eventId": str,
         "incidentRecordArn": str,
     },
 )
 _OptionalUpdateTimelineEventInputRequestTypeDef = TypedDict(
     "_OptionalUpdateTimelineEventInputRequestTypeDef",
     {
         "clientToken": str,
         "eventData": str,
         "eventReferences": Sequence[EventReferenceTypeDef],
-        "eventTime": Union[datetime, str],
+        "eventTime": TimestampTypeDef,
         "eventType": str,
     },
     total=False,
 )
 
-
 class UpdateTimelineEventInputRequestTypeDef(
     _RequiredUpdateTimelineEventInputRequestTypeDef, _OptionalUpdateTimelineEventInputRequestTypeDef
 ):
     pass
 
-
 UpdateReplicationSetActionTypeDef = TypedDict(
     "UpdateReplicationSetActionTypeDef",
     {
         "addRegionAction": AddRegionActionTypeDef,
         "deleteRegionAction": DeleteRegionActionTypeDef,
     },
     total=False,
@@ -774,21 +751,19 @@
         "dynamicParameters": Dict[str, DynamicSsmParameterValueTypeDef],
         "parameters": Dict[str, List[str]],
         "targetAccount": SsmTargetAccountType,
     },
     total=False,
 )
 
-
 class SsmAutomationOutputTypeDef(
     _RequiredSsmAutomationOutputTypeDef, _OptionalSsmAutomationOutputTypeDef
 ):
     pass
 
-
 _RequiredSsmAutomationTypeDef = TypedDict(
     "_RequiredSsmAutomationTypeDef",
     {
         "documentName": str,
         "roleArn": str,
     },
 )
@@ -799,107 +774,97 @@
         "dynamicParameters": Mapping[str, DynamicSsmParameterValueTypeDef],
         "parameters": Mapping[str, Sequence[str]],
         "targetAccount": SsmTargetAccountType,
     },
     total=False,
 )
 
-
 class SsmAutomationTypeDef(_RequiredSsmAutomationTypeDef, _OptionalSsmAutomationTypeDef):
     pass
 
-
 _RequiredGetReplicationSetInputWaitForReplicationSetActiveWaitTypeDef = TypedDict(
     "_RequiredGetReplicationSetInputWaitForReplicationSetActiveWaitTypeDef",
     {
         "arn": str,
     },
 )
 _OptionalGetReplicationSetInputWaitForReplicationSetActiveWaitTypeDef = TypedDict(
     "_OptionalGetReplicationSetInputWaitForReplicationSetActiveWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetReplicationSetInputWaitForReplicationSetActiveWaitTypeDef(
     _RequiredGetReplicationSetInputWaitForReplicationSetActiveWaitTypeDef,
     _OptionalGetReplicationSetInputWaitForReplicationSetActiveWaitTypeDef,
 ):
     pass
 
-
 _RequiredGetReplicationSetInputWaitForReplicationSetDeletedWaitTypeDef = TypedDict(
     "_RequiredGetReplicationSetInputWaitForReplicationSetDeletedWaitTypeDef",
     {
         "arn": str,
     },
 )
 _OptionalGetReplicationSetInputWaitForReplicationSetDeletedWaitTypeDef = TypedDict(
     "_OptionalGetReplicationSetInputWaitForReplicationSetDeletedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetReplicationSetInputWaitForReplicationSetDeletedWaitTypeDef(
     _RequiredGetReplicationSetInputWaitForReplicationSetDeletedWaitTypeDef,
     _OptionalGetReplicationSetInputWaitForReplicationSetDeletedWaitTypeDef,
 ):
     pass
 
-
 _RequiredGetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef = TypedDict(
     "_RequiredGetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef",
     {
         "resourceArn": str,
     },
 )
 _OptionalGetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef = TypedDict(
     "_OptionalGetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef(
     _RequiredGetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef,
     _OptionalGetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListRelatedItemsInputListRelatedItemsPaginateTypeDef = TypedDict(
     "_RequiredListRelatedItemsInputListRelatedItemsPaginateTypeDef",
     {
         "incidentRecordArn": str,
     },
 )
 _OptionalListRelatedItemsInputListRelatedItemsPaginateTypeDef = TypedDict(
     "_OptionalListRelatedItemsInputListRelatedItemsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListRelatedItemsInputListRelatedItemsPaginateTypeDef(
     _RequiredListRelatedItemsInputListRelatedItemsPaginateTypeDef,
     _OptionalListRelatedItemsInputListRelatedItemsPaginateTypeDef,
 ):
     pass
 
-
 ListReplicationSetsInputListReplicationSetsPaginateTypeDef = TypedDict(
     "ListReplicationSetsInputListReplicationSetsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -936,21 +901,19 @@
     "_OptionalIncidentRecordSummaryTypeDef",
     {
         "resolvedTime": datetime,
     },
     total=False,
 )
 
-
 class IncidentRecordSummaryTypeDef(
     _RequiredIncidentRecordSummaryTypeDef, _OptionalIncidentRecordSummaryTypeDef
 ):
     pass
 
-
 _RequiredIncidentRecordTypeDef = TypedDict(
     "_RequiredIncidentRecordTypeDef",
     {
         "arn": str,
         "creationTime": datetime,
         "dedupeString": str,
         "impact": int,
@@ -969,19 +932,17 @@
         "notificationTargets": List[NotificationTargetItemTypeDef],
         "resolvedTime": datetime,
         "summary": str,
     },
     total=False,
 )
 
-
 class IncidentRecordTypeDef(_RequiredIncidentRecordTypeDef, _OptionalIncidentRecordTypeDef):
     pass
 
-
 _RequiredIncidentTemplateOutputTypeDef = TypedDict(
     "_RequiredIncidentTemplateOutputTypeDef",
     {
         "impact": int,
         "title": str,
     },
 )
@@ -992,21 +953,19 @@
         "incidentTags": Dict[str, str],
         "notificationTargets": List[NotificationTargetItemTypeDef],
         "summary": str,
     },
     total=False,
 )
 
-
 class IncidentTemplateOutputTypeDef(
     _RequiredIncidentTemplateOutputTypeDef, _OptionalIncidentTemplateOutputTypeDef
 ):
     pass
 
-
 _RequiredIncidentTemplateTypeDef = TypedDict(
     "_RequiredIncidentTemplateTypeDef",
     {
         "impact": int,
         "title": str,
     },
 )
@@ -1017,19 +976,17 @@
         "incidentTags": Mapping[str, str],
         "notificationTargets": Sequence[NotificationTargetItemTypeDef],
         "summary": str,
     },
     total=False,
 )
 
-
 class IncidentTemplateTypeDef(_RequiredIncidentTemplateTypeDef, _OptionalIncidentTemplateTypeDef):
     pass
 
-
 _RequiredUpdateIncidentRecordInputRequestTypeDef = TypedDict(
     "_RequiredUpdateIncidentRecordInputRequestTypeDef",
     {
         "arn": str,
     },
 )
 _OptionalUpdateIncidentRecordInputRequestTypeDef = TypedDict(
@@ -1042,22 +999,20 @@
         "status": IncidentRecordStatusType,
         "summary": str,
         "title": str,
     },
     total=False,
 )
 
-
 class UpdateIncidentRecordInputRequestTypeDef(
     _RequiredUpdateIncidentRecordInputRequestTypeDef,
     _OptionalUpdateIncidentRecordInputRequestTypeDef,
 ):
     pass
 
-
 ItemValueTypeDef = TypedDict(
     "ItemValueTypeDef",
     {
         "arn": str,
         "metricDefinition": str,
         "pagerDutyIncidentDetail": PagerDutyIncidentDetailTypeDef,
         "url": str,
@@ -1099,19 +1054,17 @@
     "_OptionalReplicationSetTypeDef",
     {
         "arn": str,
     },
     total=False,
 )
 
-
 class ReplicationSetTypeDef(_RequiredReplicationSetTypeDef, _OptionalReplicationSetTypeDef):
     pass
 
-
 FilterTypeDef = TypedDict(
     "FilterTypeDef",
     {
         "condition": ConditionTypeDef,
         "key": str,
     },
 )
@@ -1144,22 +1097,20 @@
     "_OptionalUpdateReplicationSetInputRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
-
 class UpdateReplicationSetInputRequestTypeDef(
     _RequiredUpdateReplicationSetInputRequestTypeDef,
     _OptionalUpdateReplicationSetInputRequestTypeDef,
 ):
     pass
 
-
 ActionOutputTypeDef = TypedDict(
     "ActionOutputTypeDef",
     {
         "ssmAutomation": SsmAutomationOutputTypeDef,
     },
     total=False,
 )
@@ -1185,14 +1136,15 @@
     "GetIncidentRecordOutputTypeDef",
     {
         "incidentRecord": IncidentRecordTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+IncidentTemplateUnionTypeDef = Union[IncidentTemplateTypeDef, IncidentTemplateOutputTypeDef]
 ItemIdentifierTypeDef = TypedDict(
     "ItemIdentifierTypeDef",
     {
         "type": ItemTypeType,
         "value": ItemValueTypeDef,
     },
 )
@@ -1245,22 +1197,20 @@
         "sortBy": Literal["EVENT_TIME"],
         "sortOrder": SortOrderType,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListTimelineEventsInputListTimelineEventsPaginateTypeDef(
     _RequiredListTimelineEventsInputListTimelineEventsPaginateTypeDef,
     _OptionalListTimelineEventsInputListTimelineEventsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListTimelineEventsInputRequestTypeDef = TypedDict(
     "_RequiredListTimelineEventsInputRequestTypeDef",
     {
         "incidentRecordArn": str,
     },
 )
 _OptionalListTimelineEventsInputRequestTypeDef = TypedDict(
@@ -1271,21 +1221,20 @@
         "nextToken": str,
         "sortBy": Literal["EVENT_TIME"],
         "sortOrder": SortOrderType,
     },
     total=False,
 )
 
-
 class ListTimelineEventsInputRequestTypeDef(
     _RequiredListTimelineEventsInputRequestTypeDef, _OptionalListTimelineEventsInputRequestTypeDef
 ):
     pass
 
-
+ActionUnionTypeDef = Union[ActionTypeDef, ActionOutputTypeDef]
 _RequiredRelatedItemTypeDef = TypedDict(
     "_RequiredRelatedItemTypeDef",
     {
         "identifier": ItemIdentifierTypeDef,
     },
 )
 _OptionalRelatedItemTypeDef = TypedDict(
@@ -1293,72 +1242,68 @@
     {
         "generatedId": str,
         "title": str,
     },
     total=False,
 )
 
-
 class RelatedItemTypeDef(_RequiredRelatedItemTypeDef, _OptionalRelatedItemTypeDef):
     pass
 
+GetResponsePlanOutputTypeDef = TypedDict(
+    "GetResponsePlanOutputTypeDef",
+    {
+        "actions": List[ActionOutputTypeDef],
+        "arn": str,
+        "chatChannel": ChatChannelOutputTypeDef,
+        "displayName": str,
+        "engagements": List[str],
+        "incidentTemplate": IncidentTemplateOutputTypeDef,
+        "integrations": List[IntegrationTypeDef],
+        "name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 _RequiredCreateResponsePlanInputRequestTypeDef = TypedDict(
     "_RequiredCreateResponsePlanInputRequestTypeDef",
     {
         "incidentTemplate": IncidentTemplateTypeDef,
         "name": str,
     },
 )
 _OptionalCreateResponsePlanInputRequestTypeDef = TypedDict(
     "_OptionalCreateResponsePlanInputRequestTypeDef",
     {
-        "actions": Sequence[Union[ActionTypeDef, ActionOutputTypeDef]],
+        "actions": Sequence[ActionUnionTypeDef],
         "chatChannel": ChatChannelTypeDef,
         "clientToken": str,
         "displayName": str,
         "engagements": Sequence[str],
         "integrations": Sequence[IntegrationTypeDef],
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateResponsePlanInputRequestTypeDef(
     _RequiredCreateResponsePlanInputRequestTypeDef, _OptionalCreateResponsePlanInputRequestTypeDef
 ):
     pass
 
-
-GetResponsePlanOutputTypeDef = TypedDict(
-    "GetResponsePlanOutputTypeDef",
-    {
-        "actions": List[ActionOutputTypeDef],
-        "arn": str,
-        "chatChannel": ChatChannelOutputTypeDef,
-        "displayName": str,
-        "engagements": List[str],
-        "incidentTemplate": IncidentTemplateOutputTypeDef,
-        "integrations": List[IntegrationTypeDef],
-        "name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredUpdateResponsePlanInputRequestTypeDef = TypedDict(
     "_RequiredUpdateResponsePlanInputRequestTypeDef",
     {
         "arn": str,
     },
 )
 _OptionalUpdateResponsePlanInputRequestTypeDef = TypedDict(
     "_OptionalUpdateResponsePlanInputRequestTypeDef",
     {
-        "actions": Sequence[Union[ActionTypeDef, ActionOutputTypeDef]],
+        "actions": Sequence[ActionUnionTypeDef],
         "chatChannel": ChatChannelTypeDef,
         "clientToken": str,
         "displayName": str,
         "engagements": Sequence[str],
         "incidentTemplateDedupeString": str,
         "incidentTemplateImpact": int,
         "incidentTemplateNotificationTargets": Sequence[NotificationTargetItemTypeDef],
@@ -1366,21 +1311,19 @@
         "incidentTemplateTags": Mapping[str, str],
         "incidentTemplateTitle": str,
         "integrations": Sequence[IntegrationTypeDef],
     },
     total=False,
 )
 
-
 class UpdateResponsePlanInputRequestTypeDef(
     _RequiredUpdateResponsePlanInputRequestTypeDef, _OptionalUpdateResponsePlanInputRequestTypeDef
 ):
     pass
 
-
 ListRelatedItemsOutputTypeDef = TypedDict(
     "ListRelatedItemsOutputTypeDef",
     {
         "nextToken": str,
         "relatedItems": List[RelatedItemTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1409,21 +1352,19 @@
         "relatedItems": Sequence[RelatedItemTypeDef],
         "title": str,
         "triggerDetails": TriggerDetailsTypeDef,
     },
     total=False,
 )
 
-
 class StartIncidentInputRequestTypeDef(
     _RequiredStartIncidentInputRequestTypeDef, _OptionalStartIncidentInputRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateRelatedItemsInputRequestTypeDef = TypedDict(
     "_RequiredUpdateRelatedItemsInputRequestTypeDef",
     {
         "incidentRecordArn": str,
         "relatedItemsUpdate": RelatedItemsUpdateTypeDef,
     },
 )
@@ -1431,12 +1372,11 @@
     "_OptionalUpdateRelatedItemsInputRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
-
 class UpdateRelatedItemsInputRequestTypeDef(
     _RequiredUpdateRelatedItemsInputRequestTypeDef, _OptionalUpdateRelatedItemsInputRequestTypeDef
 ):
     pass
```

### Comparing `mypy-boto3-ssm-incidents-1.28.15.post1/mypy_boto3_ssm_incidents/type_defs.pyi` & `mypy-boto3-ssm-incidents-1.28.16/mypy_boto3_ssm_incidents/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_ssm_incidents.type_defs import AddRegionActionTypeDef
 
-    data: AddRegionActionTypeDef = {...}
+    data: AddRegionActionTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -30,20 +30,22 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AddRegionActionTypeDef",
     "AttributeValueListTypeDef",
     "AutomationExecutionTypeDef",
     "ChatChannelOutputTypeDef",
     "ChatChannelTypeDef",
+    "TimestampTypeDef",
     "RegionMapInputValueTypeDef",
     "ResponseMetadataTypeDef",
     "EventReferenceTypeDef",
     "DeleteIncidentRecordInputRequestTypeDef",
     "DeleteRegionActionTypeDef",
     "DeleteReplicationSetInputRequestTypeDef",
     "DeleteResourcePolicyInputRequestTypeDef",
@@ -65,19 +67,20 @@
     "ListReplicationSetsInputRequestTypeDef",
     "ListResponsePlansInputRequestTypeDef",
     "ResponsePlanSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "PagerDutyIncidentConfigurationTypeDef",
     "PutResourcePolicyInputRequestTypeDef",
     "RegionInfoTypeDef",
-    "TriggerDetailsTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDeletionProtectionInputRequestTypeDef",
+    "ChatChannelUnionTypeDef",
     "ConditionTypeDef",
+    "TriggerDetailsTypeDef",
     "CreateReplicationSetInputRequestTypeDef",
     "CreateReplicationSetOutputTypeDef",
     "CreateResponsePlanOutputTypeDef",
     "CreateTimelineEventOutputTypeDef",
     "ListReplicationSetsOutputTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "PutResourcePolicyOutputTypeDef",
@@ -109,24 +112,26 @@
     "ListTimelineEventsOutputTypeDef",
     "GetTimelineEventOutputTypeDef",
     "UpdateReplicationSetInputRequestTypeDef",
     "ActionOutputTypeDef",
     "ActionTypeDef",
     "ListIncidentRecordsOutputTypeDef",
     "GetIncidentRecordOutputTypeDef",
+    "IncidentTemplateUnionTypeDef",
     "ItemIdentifierTypeDef",
     "IntegrationTypeDef",
     "GetReplicationSetOutputTypeDef",
     "ListIncidentRecordsInputListIncidentRecordsPaginateTypeDef",
     "ListIncidentRecordsInputRequestTypeDef",
     "ListTimelineEventsInputListTimelineEventsPaginateTypeDef",
     "ListTimelineEventsInputRequestTypeDef",
+    "ActionUnionTypeDef",
     "RelatedItemTypeDef",
-    "CreateResponsePlanInputRequestTypeDef",
     "GetResponsePlanOutputTypeDef",
+    "CreateResponsePlanInputRequestTypeDef",
     "UpdateResponsePlanInputRequestTypeDef",
     "ListRelatedItemsOutputTypeDef",
     "RelatedItemsUpdateTypeDef",
     "StartIncidentInputRequestTypeDef",
     "UpdateRelatedItemsInputRequestTypeDef",
 )
 
@@ -140,17 +145,19 @@
     "_OptionalAddRegionActionTypeDef",
     {
         "sseKmsKeyId": str,
     },
     total=False,
 )
 
+
 class AddRegionActionTypeDef(_RequiredAddRegionActionTypeDef, _OptionalAddRegionActionTypeDef):
     pass
 
+
 AttributeValueListTypeDef = TypedDict(
     "AttributeValueListTypeDef",
     {
         "integerValues": Sequence[int],
         "stringValues": Sequence[str],
     },
     total=False,
@@ -178,14 +185,15 @@
     {
         "chatbotSns": Sequence[str],
         "empty": Mapping[str, Any],
     },
     total=False,
 )
 
+TimestampTypeDef = Union[datetime, str]
 RegionMapInputValueTypeDef = TypedDict(
     "RegionMapInputValueTypeDef",
     {
         "sseKmsKeyId": str,
     },
     total=False,
 )
@@ -306,19 +314,21 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class GetResourcePoliciesInputRequestTypeDef(
     _RequiredGetResourcePoliciesInputRequestTypeDef, _OptionalGetResourcePoliciesInputRequestTypeDef
 ):
     pass
 
+
 ResourcePolicyTypeDef = TypedDict(
     "ResourcePolicyTypeDef",
     {
         "policyDocument": str,
         "policyId": str,
         "ramResourceShareRegion": str,
     },
@@ -351,19 +361,21 @@
     {
         "invokedBy": str,
         "resourceArn": str,
     },
     total=False,
 )
 
+
 class IncidentRecordSourceTypeDef(
     _RequiredIncidentRecordSourceTypeDef, _OptionalIncidentRecordSourceTypeDef
 ):
     pass
 
+
 NotificationTargetItemTypeDef = TypedDict(
     "NotificationTargetItemTypeDef",
     {
         "snsTopicArn": str,
     },
     total=False,
 )
@@ -379,19 +391,21 @@
     {
         "autoResolve": bool,
         "secretId": str,
     },
     total=False,
 )
 
+
 class PagerDutyIncidentDetailTypeDef(
     _RequiredPagerDutyIncidentDetailTypeDef, _OptionalPagerDutyIncidentDetailTypeDef
 ):
     pass
 
+
 _RequiredListRelatedItemsInputRequestTypeDef = TypedDict(
     "_RequiredListRelatedItemsInputRequestTypeDef",
     {
         "incidentRecordArn": str,
     },
 )
 _OptionalListRelatedItemsInputRequestTypeDef = TypedDict(
@@ -399,19 +413,21 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListRelatedItemsInputRequestTypeDef(
     _RequiredListRelatedItemsInputRequestTypeDef, _OptionalListRelatedItemsInputRequestTypeDef
 ):
     pass
 
+
 ListReplicationSetsInputRequestTypeDef = TypedDict(
     "ListReplicationSetsInputRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -437,19 +453,21 @@
     "_OptionalResponsePlanSummaryTypeDef",
     {
         "displayName": str,
     },
     total=False,
 )
 
+
 class ResponsePlanSummaryTypeDef(
     _RequiredResponsePlanSummaryTypeDef, _OptionalResponsePlanSummaryTypeDef
 ):
     pass
 
+
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
@@ -480,35 +498,18 @@
     {
         "sseKmsKeyId": str,
         "statusMessage": str,
     },
     total=False,
 )
 
+
 class RegionInfoTypeDef(_RequiredRegionInfoTypeDef, _OptionalRegionInfoTypeDef):
     pass
 
-_RequiredTriggerDetailsTypeDef = TypedDict(
-    "_RequiredTriggerDetailsTypeDef",
-    {
-        "source": str,
-        "timestamp": Union[datetime, str],
-    },
-)
-_OptionalTriggerDetailsTypeDef = TypedDict(
-    "_OptionalTriggerDetailsTypeDef",
-    {
-        "rawData": str,
-        "triggerArn": str,
-    },
-    total=False,
-)
-
-class TriggerDetailsTypeDef(_RequiredTriggerDetailsTypeDef, _OptionalTriggerDetailsTypeDef):
-    pass
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
@@ -533,30 +534,54 @@
     "_OptionalUpdateDeletionProtectionInputRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
+
 class UpdateDeletionProtectionInputRequestTypeDef(
     _RequiredUpdateDeletionProtectionInputRequestTypeDef,
     _OptionalUpdateDeletionProtectionInputRequestTypeDef,
 ):
     pass
 
+
+ChatChannelUnionTypeDef = Union[ChatChannelTypeDef, ChatChannelOutputTypeDef]
 ConditionTypeDef = TypedDict(
     "ConditionTypeDef",
     {
-        "after": Union[datetime, str],
-        "before": Union[datetime, str],
+        "after": TimestampTypeDef,
+        "before": TimestampTypeDef,
         "equals": AttributeValueListTypeDef,
     },
     total=False,
 )
 
+_RequiredTriggerDetailsTypeDef = TypedDict(
+    "_RequiredTriggerDetailsTypeDef",
+    {
+        "source": str,
+        "timestamp": TimestampTypeDef,
+    },
+)
+_OptionalTriggerDetailsTypeDef = TypedDict(
+    "_OptionalTriggerDetailsTypeDef",
+    {
+        "rawData": str,
+        "triggerArn": str,
+    },
+    total=False,
+)
+
+
+class TriggerDetailsTypeDef(_RequiredTriggerDetailsTypeDef, _OptionalTriggerDetailsTypeDef):
+    pass
+
+
 _RequiredCreateReplicationSetInputRequestTypeDef = TypedDict(
     "_RequiredCreateReplicationSetInputRequestTypeDef",
     {
         "regions": Mapping[str, RegionMapInputValueTypeDef],
     },
 )
 _OptionalCreateReplicationSetInputRequestTypeDef = TypedDict(
@@ -564,20 +589,22 @@
     {
         "clientToken": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateReplicationSetInputRequestTypeDef(
     _RequiredCreateReplicationSetInputRequestTypeDef,
     _OptionalCreateReplicationSetInputRequestTypeDef,
 ):
     pass
 
+
 CreateReplicationSetOutputTypeDef = TypedDict(
     "CreateReplicationSetOutputTypeDef",
     {
         "arn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -632,33 +659,35 @@
     },
 )
 
 _RequiredCreateTimelineEventInputRequestTypeDef = TypedDict(
     "_RequiredCreateTimelineEventInputRequestTypeDef",
     {
         "eventData": str,
-        "eventTime": Union[datetime, str],
+        "eventTime": TimestampTypeDef,
         "eventType": str,
         "incidentRecordArn": str,
     },
 )
 _OptionalCreateTimelineEventInputRequestTypeDef = TypedDict(
     "_OptionalCreateTimelineEventInputRequestTypeDef",
     {
         "clientToken": str,
         "eventReferences": Sequence[EventReferenceTypeDef],
     },
     total=False,
 )
 
+
 class CreateTimelineEventInputRequestTypeDef(
     _RequiredCreateTimelineEventInputRequestTypeDef, _OptionalCreateTimelineEventInputRequestTypeDef
 ):
     pass
 
+
 _RequiredEventSummaryTypeDef = TypedDict(
     "_RequiredEventSummaryTypeDef",
     {
         "eventId": str,
         "eventTime": datetime,
         "eventType": str,
         "eventUpdatedTime": datetime,
@@ -669,17 +698,19 @@
     "_OptionalEventSummaryTypeDef",
     {
         "eventReferences": List[EventReferenceTypeDef],
     },
     total=False,
 )
 
+
 class EventSummaryTypeDef(_RequiredEventSummaryTypeDef, _OptionalEventSummaryTypeDef):
     pass
 
+
 _RequiredTimelineEventTypeDef = TypedDict(
     "_RequiredTimelineEventTypeDef",
     {
         "eventData": str,
         "eventId": str,
         "eventTime": datetime,
         "eventType": str,
@@ -691,41 +722,45 @@
     "_OptionalTimelineEventTypeDef",
     {
         "eventReferences": List[EventReferenceTypeDef],
     },
     total=False,
 )
 
+
 class TimelineEventTypeDef(_RequiredTimelineEventTypeDef, _OptionalTimelineEventTypeDef):
     pass
 
+
 _RequiredUpdateTimelineEventInputRequestTypeDef = TypedDict(
     "_RequiredUpdateTimelineEventInputRequestTypeDef",
     {
         "eventId": str,
         "incidentRecordArn": str,
     },
 )
 _OptionalUpdateTimelineEventInputRequestTypeDef = TypedDict(
     "_OptionalUpdateTimelineEventInputRequestTypeDef",
     {
         "clientToken": str,
         "eventData": str,
         "eventReferences": Sequence[EventReferenceTypeDef],
-        "eventTime": Union[datetime, str],
+        "eventTime": TimestampTypeDef,
         "eventType": str,
     },
     total=False,
 )
 
+
 class UpdateTimelineEventInputRequestTypeDef(
     _RequiredUpdateTimelineEventInputRequestTypeDef, _OptionalUpdateTimelineEventInputRequestTypeDef
 ):
     pass
 
+
 UpdateReplicationSetActionTypeDef = TypedDict(
     "UpdateReplicationSetActionTypeDef",
     {
         "addRegionAction": AddRegionActionTypeDef,
         "deleteRegionAction": DeleteRegionActionTypeDef,
     },
     total=False,
@@ -745,19 +780,21 @@
         "dynamicParameters": Dict[str, DynamicSsmParameterValueTypeDef],
         "parameters": Dict[str, List[str]],
         "targetAccount": SsmTargetAccountType,
     },
     total=False,
 )
 
+
 class SsmAutomationOutputTypeDef(
     _RequiredSsmAutomationOutputTypeDef, _OptionalSsmAutomationOutputTypeDef
 ):
     pass
 
+
 _RequiredSsmAutomationTypeDef = TypedDict(
     "_RequiredSsmAutomationTypeDef",
     {
         "documentName": str,
         "roleArn": str,
     },
 )
@@ -768,97 +805,107 @@
         "dynamicParameters": Mapping[str, DynamicSsmParameterValueTypeDef],
         "parameters": Mapping[str, Sequence[str]],
         "targetAccount": SsmTargetAccountType,
     },
     total=False,
 )
 
+
 class SsmAutomationTypeDef(_RequiredSsmAutomationTypeDef, _OptionalSsmAutomationTypeDef):
     pass
 
+
 _RequiredGetReplicationSetInputWaitForReplicationSetActiveWaitTypeDef = TypedDict(
     "_RequiredGetReplicationSetInputWaitForReplicationSetActiveWaitTypeDef",
     {
         "arn": str,
     },
 )
 _OptionalGetReplicationSetInputWaitForReplicationSetActiveWaitTypeDef = TypedDict(
     "_OptionalGetReplicationSetInputWaitForReplicationSetActiveWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetReplicationSetInputWaitForReplicationSetActiveWaitTypeDef(
     _RequiredGetReplicationSetInputWaitForReplicationSetActiveWaitTypeDef,
     _OptionalGetReplicationSetInputWaitForReplicationSetActiveWaitTypeDef,
 ):
     pass
 
+
 _RequiredGetReplicationSetInputWaitForReplicationSetDeletedWaitTypeDef = TypedDict(
     "_RequiredGetReplicationSetInputWaitForReplicationSetDeletedWaitTypeDef",
     {
         "arn": str,
     },
 )
 _OptionalGetReplicationSetInputWaitForReplicationSetDeletedWaitTypeDef = TypedDict(
     "_OptionalGetReplicationSetInputWaitForReplicationSetDeletedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetReplicationSetInputWaitForReplicationSetDeletedWaitTypeDef(
     _RequiredGetReplicationSetInputWaitForReplicationSetDeletedWaitTypeDef,
     _OptionalGetReplicationSetInputWaitForReplicationSetDeletedWaitTypeDef,
 ):
     pass
 
+
 _RequiredGetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef = TypedDict(
     "_RequiredGetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef",
     {
         "resourceArn": str,
     },
 )
 _OptionalGetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef = TypedDict(
     "_OptionalGetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef(
     _RequiredGetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef,
     _OptionalGetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListRelatedItemsInputListRelatedItemsPaginateTypeDef = TypedDict(
     "_RequiredListRelatedItemsInputListRelatedItemsPaginateTypeDef",
     {
         "incidentRecordArn": str,
     },
 )
 _OptionalListRelatedItemsInputListRelatedItemsPaginateTypeDef = TypedDict(
     "_OptionalListRelatedItemsInputListRelatedItemsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListRelatedItemsInputListRelatedItemsPaginateTypeDef(
     _RequiredListRelatedItemsInputListRelatedItemsPaginateTypeDef,
     _OptionalListRelatedItemsInputListRelatedItemsPaginateTypeDef,
 ):
     pass
 
+
 ListReplicationSetsInputListReplicationSetsPaginateTypeDef = TypedDict(
     "ListReplicationSetsInputListReplicationSetsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -895,19 +942,21 @@
     "_OptionalIncidentRecordSummaryTypeDef",
     {
         "resolvedTime": datetime,
     },
     total=False,
 )
 
+
 class IncidentRecordSummaryTypeDef(
     _RequiredIncidentRecordSummaryTypeDef, _OptionalIncidentRecordSummaryTypeDef
 ):
     pass
 
+
 _RequiredIncidentRecordTypeDef = TypedDict(
     "_RequiredIncidentRecordTypeDef",
     {
         "arn": str,
         "creationTime": datetime,
         "dedupeString": str,
         "impact": int,
@@ -926,17 +975,19 @@
         "notificationTargets": List[NotificationTargetItemTypeDef],
         "resolvedTime": datetime,
         "summary": str,
     },
     total=False,
 )
 
+
 class IncidentRecordTypeDef(_RequiredIncidentRecordTypeDef, _OptionalIncidentRecordTypeDef):
     pass
 
+
 _RequiredIncidentTemplateOutputTypeDef = TypedDict(
     "_RequiredIncidentTemplateOutputTypeDef",
     {
         "impact": int,
         "title": str,
     },
 )
@@ -947,19 +998,21 @@
         "incidentTags": Dict[str, str],
         "notificationTargets": List[NotificationTargetItemTypeDef],
         "summary": str,
     },
     total=False,
 )
 
+
 class IncidentTemplateOutputTypeDef(
     _RequiredIncidentTemplateOutputTypeDef, _OptionalIncidentTemplateOutputTypeDef
 ):
     pass
 
+
 _RequiredIncidentTemplateTypeDef = TypedDict(
     "_RequiredIncidentTemplateTypeDef",
     {
         "impact": int,
         "title": str,
     },
 )
@@ -970,17 +1023,19 @@
         "incidentTags": Mapping[str, str],
         "notificationTargets": Sequence[NotificationTargetItemTypeDef],
         "summary": str,
     },
     total=False,
 )
 
+
 class IncidentTemplateTypeDef(_RequiredIncidentTemplateTypeDef, _OptionalIncidentTemplateTypeDef):
     pass
 
+
 _RequiredUpdateIncidentRecordInputRequestTypeDef = TypedDict(
     "_RequiredUpdateIncidentRecordInputRequestTypeDef",
     {
         "arn": str,
     },
 )
 _OptionalUpdateIncidentRecordInputRequestTypeDef = TypedDict(
@@ -993,20 +1048,22 @@
         "status": IncidentRecordStatusType,
         "summary": str,
         "title": str,
     },
     total=False,
 )
 
+
 class UpdateIncidentRecordInputRequestTypeDef(
     _RequiredUpdateIncidentRecordInputRequestTypeDef,
     _OptionalUpdateIncidentRecordInputRequestTypeDef,
 ):
     pass
 
+
 ItemValueTypeDef = TypedDict(
     "ItemValueTypeDef",
     {
         "arn": str,
         "metricDefinition": str,
         "pagerDutyIncidentDetail": PagerDutyIncidentDetailTypeDef,
         "url": str,
@@ -1048,17 +1105,19 @@
     "_OptionalReplicationSetTypeDef",
     {
         "arn": str,
     },
     total=False,
 )
 
+
 class ReplicationSetTypeDef(_RequiredReplicationSetTypeDef, _OptionalReplicationSetTypeDef):
     pass
 
+
 FilterTypeDef = TypedDict(
     "FilterTypeDef",
     {
         "condition": ConditionTypeDef,
         "key": str,
     },
 )
@@ -1091,20 +1150,22 @@
     "_OptionalUpdateReplicationSetInputRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
+
 class UpdateReplicationSetInputRequestTypeDef(
     _RequiredUpdateReplicationSetInputRequestTypeDef,
     _OptionalUpdateReplicationSetInputRequestTypeDef,
 ):
     pass
 
+
 ActionOutputTypeDef = TypedDict(
     "ActionOutputTypeDef",
     {
         "ssmAutomation": SsmAutomationOutputTypeDef,
     },
     total=False,
 )
@@ -1130,14 +1191,15 @@
     "GetIncidentRecordOutputTypeDef",
     {
         "incidentRecord": IncidentRecordTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+IncidentTemplateUnionTypeDef = Union[IncidentTemplateTypeDef, IncidentTemplateOutputTypeDef]
 ItemIdentifierTypeDef = TypedDict(
     "ItemIdentifierTypeDef",
     {
         "type": ItemTypeType,
         "value": ItemValueTypeDef,
     },
 )
@@ -1190,20 +1252,22 @@
         "sortBy": Literal["EVENT_TIME"],
         "sortOrder": SortOrderType,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListTimelineEventsInputListTimelineEventsPaginateTypeDef(
     _RequiredListTimelineEventsInputListTimelineEventsPaginateTypeDef,
     _OptionalListTimelineEventsInputListTimelineEventsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListTimelineEventsInputRequestTypeDef = TypedDict(
     "_RequiredListTimelineEventsInputRequestTypeDef",
     {
         "incidentRecordArn": str,
     },
 )
 _OptionalListTimelineEventsInputRequestTypeDef = TypedDict(
@@ -1214,19 +1278,22 @@
         "nextToken": str,
         "sortBy": Literal["EVENT_TIME"],
         "sortOrder": SortOrderType,
     },
     total=False,
 )
 
+
 class ListTimelineEventsInputRequestTypeDef(
     _RequiredListTimelineEventsInputRequestTypeDef, _OptionalListTimelineEventsInputRequestTypeDef
 ):
     pass
 
+
+ActionUnionTypeDef = Union[ActionTypeDef, ActionOutputTypeDef]
 _RequiredRelatedItemTypeDef = TypedDict(
     "_RequiredRelatedItemTypeDef",
     {
         "identifier": ItemIdentifierTypeDef,
     },
 )
 _OptionalRelatedItemTypeDef = TypedDict(
@@ -1234,68 +1301,72 @@
     {
         "generatedId": str,
         "title": str,
     },
     total=False,
 )
 
+
 class RelatedItemTypeDef(_RequiredRelatedItemTypeDef, _OptionalRelatedItemTypeDef):
     pass
 
+
+GetResponsePlanOutputTypeDef = TypedDict(
+    "GetResponsePlanOutputTypeDef",
+    {
+        "actions": List[ActionOutputTypeDef],
+        "arn": str,
+        "chatChannel": ChatChannelOutputTypeDef,
+        "displayName": str,
+        "engagements": List[str],
+        "incidentTemplate": IncidentTemplateOutputTypeDef,
+        "integrations": List[IntegrationTypeDef],
+        "name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateResponsePlanInputRequestTypeDef = TypedDict(
     "_RequiredCreateResponsePlanInputRequestTypeDef",
     {
         "incidentTemplate": IncidentTemplateTypeDef,
         "name": str,
     },
 )
 _OptionalCreateResponsePlanInputRequestTypeDef = TypedDict(
     "_OptionalCreateResponsePlanInputRequestTypeDef",
     {
-        "actions": Sequence[Union[ActionTypeDef, ActionOutputTypeDef]],
+        "actions": Sequence[ActionUnionTypeDef],
         "chatChannel": ChatChannelTypeDef,
         "clientToken": str,
         "displayName": str,
         "engagements": Sequence[str],
         "integrations": Sequence[IntegrationTypeDef],
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateResponsePlanInputRequestTypeDef(
     _RequiredCreateResponsePlanInputRequestTypeDef, _OptionalCreateResponsePlanInputRequestTypeDef
 ):
     pass
 
-GetResponsePlanOutputTypeDef = TypedDict(
-    "GetResponsePlanOutputTypeDef",
-    {
-        "actions": List[ActionOutputTypeDef],
-        "arn": str,
-        "chatChannel": ChatChannelOutputTypeDef,
-        "displayName": str,
-        "engagements": List[str],
-        "incidentTemplate": IncidentTemplateOutputTypeDef,
-        "integrations": List[IntegrationTypeDef],
-        "name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 
 _RequiredUpdateResponsePlanInputRequestTypeDef = TypedDict(
     "_RequiredUpdateResponsePlanInputRequestTypeDef",
     {
         "arn": str,
     },
 )
 _OptionalUpdateResponsePlanInputRequestTypeDef = TypedDict(
     "_OptionalUpdateResponsePlanInputRequestTypeDef",
     {
-        "actions": Sequence[Union[ActionTypeDef, ActionOutputTypeDef]],
+        "actions": Sequence[ActionUnionTypeDef],
         "chatChannel": ChatChannelTypeDef,
         "clientToken": str,
         "displayName": str,
         "engagements": Sequence[str],
         "incidentTemplateDedupeString": str,
         "incidentTemplateImpact": int,
         "incidentTemplateNotificationTargets": Sequence[NotificationTargetItemTypeDef],
@@ -1303,19 +1374,21 @@
         "incidentTemplateTags": Mapping[str, str],
         "incidentTemplateTitle": str,
         "integrations": Sequence[IntegrationTypeDef],
     },
     total=False,
 )
 
+
 class UpdateResponsePlanInputRequestTypeDef(
     _RequiredUpdateResponsePlanInputRequestTypeDef, _OptionalUpdateResponsePlanInputRequestTypeDef
 ):
     pass
 
+
 ListRelatedItemsOutputTypeDef = TypedDict(
     "ListRelatedItemsOutputTypeDef",
     {
         "nextToken": str,
         "relatedItems": List[RelatedItemTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1344,19 +1417,21 @@
         "relatedItems": Sequence[RelatedItemTypeDef],
         "title": str,
         "triggerDetails": TriggerDetailsTypeDef,
     },
     total=False,
 )
 
+
 class StartIncidentInputRequestTypeDef(
     _RequiredStartIncidentInputRequestTypeDef, _OptionalStartIncidentInputRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateRelatedItemsInputRequestTypeDef = TypedDict(
     "_RequiredUpdateRelatedItemsInputRequestTypeDef",
     {
         "incidentRecordArn": str,
         "relatedItemsUpdate": RelatedItemsUpdateTypeDef,
     },
 )
@@ -1364,11 +1439,12 @@
     "_OptionalUpdateRelatedItemsInputRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
+
 class UpdateRelatedItemsInputRequestTypeDef(
     _RequiredUpdateRelatedItemsInputRequestTypeDef, _OptionalUpdateRelatedItemsInputRequestTypeDef
 ):
     pass
```

### Comparing `mypy-boto3-ssm-incidents-1.28.15.post1/mypy_boto3_ssm_incidents/waiter.py` & `mypy-boto3-ssm-incidents-1.28.16/mypy_boto3_ssm_incidents/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-incidents-1.28.15.post1/mypy_boto3_ssm_incidents/waiter.pyi` & `mypy-boto3-ssm-incidents-1.28.16/mypy_boto3_ssm_incidents/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-incidents-1.28.15.post1/mypy_boto3_ssm_incidents.egg-info/PKG-INFO` & `mypy-boto3-ssm-incidents-1.28.16/mypy_boto3_ssm_incidents.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ssm-incidents
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.SSMIncidents 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.SSMIncidents 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 ssm-incidents type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 ssm-incidents type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ssm-incidents.svg?color=blue)](https://pypi.org/project/mypy-boto3-ssm-incidents)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ssm-incidents)](https://pepy.tech/project/mypy-boto3-ssm-incidents)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SSMIncidents 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents)
+[boto3.SSMIncidents 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents)
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
 [mypy-boto3-ssm-incidents docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/).
 
 See how it helps to find and fix potential bugs:
 
@@ -75,15 +75,15 @@
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Waiters annotations](#waiters-annotations)
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
@@ -377,28 +377,29 @@
 )
 
 
 def check_value(value: GetResourcePoliciesPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_ssm_incidents.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_ssm_incidents.type_defs import (
     AddRegionActionTypeDef,
     AttributeValueListTypeDef,
     AutomationExecutionTypeDef,
     ChatChannelOutputTypeDef,
     ChatChannelTypeDef,
+    TimestampTypeDef,
     RegionMapInputValueTypeDef,
     ResponseMetadataTypeDef,
     EventReferenceTypeDef,
     DeleteIncidentRecordInputRequestTypeDef,
     DeleteRegionActionTypeDef,
     DeleteReplicationSetInputRequestTypeDef,
     DeleteResourcePolicyInputRequestTypeDef,
@@ -420,19 +421,20 @@
     ListReplicationSetsInputRequestTypeDef,
     ListResponsePlansInputRequestTypeDef,
     ResponsePlanSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     PagerDutyIncidentConfigurationTypeDef,
     PutResourcePolicyInputRequestTypeDef,
     RegionInfoTypeDef,
-    TriggerDetailsTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDeletionProtectionInputRequestTypeDef,
+    ChatChannelUnionTypeDef,
     ConditionTypeDef,
+    TriggerDetailsTypeDef,
     CreateReplicationSetInputRequestTypeDef,
     CreateReplicationSetOutputTypeDef,
     CreateResponsePlanOutputTypeDef,
     CreateTimelineEventOutputTypeDef,
     ListReplicationSetsOutputTypeDef,
     ListTagsForResourceResponseTypeDef,
     PutResourcePolicyOutputTypeDef,
@@ -464,33 +466,35 @@
     ListTimelineEventsOutputTypeDef,
     GetTimelineEventOutputTypeDef,
     UpdateReplicationSetInputRequestTypeDef,
     ActionOutputTypeDef,
     ActionTypeDef,
     ListIncidentRecordsOutputTypeDef,
     GetIncidentRecordOutputTypeDef,
+    IncidentTemplateUnionTypeDef,
     ItemIdentifierTypeDef,
     IntegrationTypeDef,
     GetReplicationSetOutputTypeDef,
     ListIncidentRecordsInputListIncidentRecordsPaginateTypeDef,
     ListIncidentRecordsInputRequestTypeDef,
     ListTimelineEventsInputListTimelineEventsPaginateTypeDef,
     ListTimelineEventsInputRequestTypeDef,
+    ActionUnionTypeDef,
     RelatedItemTypeDef,
-    CreateResponsePlanInputRequestTypeDef,
     GetResponsePlanOutputTypeDef,
+    CreateResponsePlanInputRequestTypeDef,
     UpdateResponsePlanInputRequestTypeDef,
     ListRelatedItemsOutputTypeDef,
     RelatedItemsUpdateTypeDef,
     StartIncidentInputRequestTypeDef,
     UpdateRelatedItemsInputRequestTypeDef,
 )
 
 
-def get_structure() -> AddRegionActionTypeDef:
+def get_value() -> AddRegionActionTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-ssm-incidents-1.28.15.post1/mypy_boto3_ssm_incidents.egg-info/SOURCES.txt` & `mypy-boto3-ssm-incidents-1.28.16/mypy_boto3_ssm_incidents.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-incidents-1.28.15.post1/setup.py` & `mypy-boto3-ssm-incidents-1.28.16/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-ssm-incidents",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_ssm_incidents"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.SSMIncidents 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.2"
+        "Type annotations for boto3.SSMIncidents 1.28.16 service generated with mypy-boto3-builder"
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
-    keywords="boto3 ssm-incidents type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 ssm-incidents type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_ssm_incidents": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

