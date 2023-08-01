# Comparing `tmp/mypy-boto3-scheduler-1.28.16.tar.gz` & `tmp/mypy-boto3-scheduler-1.28.16.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-scheduler-1.28.16.tar", last modified: Mon Jul 31 19:32:48 2023, max compression
+gzip compressed data, was "mypy-boto3-scheduler-1.28.16.post1.tar", last modified: Tue Aug  1 11:37:48 2023, max compression
```

## Comparing `mypy-boto3-scheduler-1.28.16.tar` & `mypy-boto3-scheduler-1.28.16.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:32:48.078182 mypy-boto3-scheduler-1.28.16/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-31 19:32:36.000000 mypy-boto3-scheduler-1.28.16/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14794 2023-07-31 19:32:48.078182 mypy-boto3-scheduler-1.28.16/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13288 2023-07-31 19:32:36.000000 mypy-boto3-scheduler-1.28.16/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:32:48.078182 mypy-boto3-scheduler-1.28.16/mypy_boto3_scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-31 19:32:36.000000 mypy-boto3-scheduler-1.28.16/mypy_boto3_scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-31 19:32:36.000000 mypy-boto3-scheduler-1.28.16/mypy_boto3_scheduler/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-31 19:32:36.000000 mypy-boto3-scheduler-1.28.16/mypy_boto3_scheduler/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12049 2023-07-31 19:32:36.000000 mypy-boto3-scheduler-1.28.16/mypy_boto3_scheduler/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12028 2023-07-31 19:32:36.000000 mypy-boto3-scheduler-1.28.16/mypy_boto3_scheduler/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9248 2023-07-31 19:32:37.000000 mypy-boto3-scheduler-1.28.16/mypy_boto3_scheduler/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9246 2023-07-31 19:32:36.000000 mypy-boto3-scheduler-1.28.16/mypy_boto3_scheduler/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-07-31 19:32:36.000000 mypy-boto3-scheduler-1.28.16/mypy_boto3_scheduler/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-07-31 19:32:36.000000 mypy-boto3-scheduler-1.28.16/mypy_boto3_scheduler/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 19:32:36.000000 mypy-boto3-scheduler-1.28.16/mypy_boto3_scheduler/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    18595 2023-07-31 19:32:37.000000 mypy-boto3-scheduler-1.28.16/mypy_boto3_scheduler/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    18567 2023-07-31 19:32:37.000000 mypy-boto3-scheduler-1.28.16/mypy_boto3_scheduler/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-31 19:32:36.000000 mypy-boto3-scheduler-1.28.16/mypy_boto3_scheduler/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:32:48.078182 mypy-boto3-scheduler-1.28.16/mypy_boto3_scheduler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14794 2023-07-31 19:32:47.000000 mypy-boto3-scheduler-1.28.16/mypy_boto3_scheduler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-31 19:32:48.000000 mypy-boto3-scheduler-1.28.16/mypy_boto3_scheduler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 19:32:47.000000 mypy-boto3-scheduler-1.28.16/mypy_boto3_scheduler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 19:32:47.000000 mypy-boto3-scheduler-1.28.16/mypy_boto3_scheduler.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-31 19:32:47.000000 mypy-boto3-scheduler-1.28.16/mypy_boto3_scheduler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-31 19:32:47.000000 mypy-boto3-scheduler-1.28.16/mypy_boto3_scheduler.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 19:32:48.078182 mypy-boto3-scheduler-1.28.16/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-07-31 19:32:36.000000 mypy-boto3-scheduler-1.28.16/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:48.108742 mypy-boto3-scheduler-1.28.16.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:32:10.000000 mypy-boto3-scheduler-1.28.16.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14842 2023-08-01 11:37:48.108742 mypy-boto3-scheduler-1.28.16.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13333 2023-08-01 11:32:10.000000 mypy-boto3-scheduler-1.28.16.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:48.108742 mypy-boto3-scheduler-1.28.16.post1/mypy_boto3_scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-08-01 11:32:10.000000 mypy-boto3-scheduler-1.28.16.post1/mypy_boto3_scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-08-01 11:32:10.000000 mypy-boto3-scheduler-1.28.16.post1/mypy_boto3_scheduler/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-08-01 11:32:10.000000 mypy-boto3-scheduler-1.28.16.post1/mypy_boto3_scheduler/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11952 2023-08-01 11:32:10.000000 mypy-boto3-scheduler-1.28.16.post1/mypy_boto3_scheduler/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11931 2023-08-01 11:32:10.000000 mypy-boto3-scheduler-1.28.16.post1/mypy_boto3_scheduler/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9248 2023-08-01 11:32:10.000000 mypy-boto3-scheduler-1.28.16.post1/mypy_boto3_scheduler/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9246 2023-08-01 11:32:10.000000 mypy-boto3-scheduler-1.28.16.post1/mypy_boto3_scheduler/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-08-01 11:32:10.000000 mypy-boto3-scheduler-1.28.16.post1/mypy_boto3_scheduler/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-08-01 11:32:10.000000 mypy-boto3-scheduler-1.28.16.post1/mypy_boto3_scheduler/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:32:10.000000 mypy-boto3-scheduler-1.28.16.post1/mypy_boto3_scheduler/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    18730 2023-08-01 11:32:11.000000 mypy-boto3-scheduler-1.28.16.post1/mypy_boto3_scheduler/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18702 2023-08-01 11:32:11.000000 mypy-boto3-scheduler-1.28.16.post1/mypy_boto3_scheduler/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-01 11:32:10.000000 mypy-boto3-scheduler-1.28.16.post1/mypy_boto3_scheduler/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:48.108742 mypy-boto3-scheduler-1.28.16.post1/mypy_boto3_scheduler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14842 2023-08-01 11:37:47.000000 mypy-boto3-scheduler-1.28.16.post1/mypy_boto3_scheduler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-08-01 11:37:47.000000 mypy-boto3-scheduler-1.28.16.post1/mypy_boto3_scheduler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:47.000000 mypy-boto3-scheduler-1.28.16.post1/mypy_boto3_scheduler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:47.000000 mypy-boto3-scheduler-1.28.16.post1/mypy_boto3_scheduler.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:47.000000 mypy-boto3-scheduler-1.28.16.post1/mypy_boto3_scheduler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-01 11:37:47.000000 mypy-boto3-scheduler-1.28.16.post1/mypy_boto3_scheduler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:48.108742 mypy-boto3-scheduler-1.28.16.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-08-01 11:32:10.000000 mypy-boto3-scheduler-1.28.16.post1/setup.py
```

### Comparing `mypy-boto3-scheduler-1.28.16/LICENSE` & `mypy-boto3-scheduler-1.28.16.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-scheduler-1.28.16/PKG-INFO` & `mypy-boto3-scheduler-1.28.16.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-scheduler
-Version: 1.28.16
-Summary: Type annotations for boto3.EventBridgeScheduler 1.28.16 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16.post1
+Summary: Type annotations for boto3.EventBridgeScheduler 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 scheduler type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 scheduler type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -47,15 +47,15 @@
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
 [mypy-boto3-scheduler docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/).
 
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
@@ -323,29 +323,30 @@
 )
 
 
 def check_value(value: ActionAfterCompletionType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_scheduler.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_scheduler.type_defs import (
     AwsVpcConfigurationOutputTypeDef,
     AwsVpcConfigurationTypeDef,
     CapacityProviderStrategyItemTypeDef,
     TagTypeDef,
     ResponseMetadataTypeDef,
     FlexibleTimeWindowTypeDef,
+    TimestampTypeDef,
     DeadLetterConfigTypeDef,
     DeleteScheduleGroupInputRequestTypeDef,
     DeleteScheduleInputRequestTypeDef,
     PlacementConstraintTypeDef,
     PlacementStrategyTypeDef,
     EventBridgeParametersTypeDef,
     GetScheduleGroupInputRequestTypeDef,
@@ -379,19 +380,20 @@
     EcsParametersOutputTypeDef,
     EcsParametersTypeDef,
     ListSchedulesOutputTypeDef,
     TargetOutputTypeDef,
     TargetTypeDef,
     GetScheduleOutputTypeDef,
     CreateScheduleInputRequestTypeDef,
+    TargetUnionTypeDef,
     UpdateScheduleInputRequestTypeDef,
 )
 
 
-def get_structure() -> AwsVpcConfigurationOutputTypeDef:
+def get_value() -> AwsVpcConfigurationOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-scheduler-1.28.16/README.md` & `mypy-boto3-scheduler-1.28.16.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
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
 [mypy-boto3-scheduler docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/).
 
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
@@ -291,29 +291,30 @@
 )
 
 
 def check_value(value: ActionAfterCompletionType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_scheduler.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_scheduler.type_defs import (
     AwsVpcConfigurationOutputTypeDef,
     AwsVpcConfigurationTypeDef,
     CapacityProviderStrategyItemTypeDef,
     TagTypeDef,
     ResponseMetadataTypeDef,
     FlexibleTimeWindowTypeDef,
+    TimestampTypeDef,
     DeadLetterConfigTypeDef,
     DeleteScheduleGroupInputRequestTypeDef,
     DeleteScheduleInputRequestTypeDef,
     PlacementConstraintTypeDef,
     PlacementStrategyTypeDef,
     EventBridgeParametersTypeDef,
     GetScheduleGroupInputRequestTypeDef,
@@ -347,19 +348,20 @@
     EcsParametersOutputTypeDef,
     EcsParametersTypeDef,
     ListSchedulesOutputTypeDef,
     TargetOutputTypeDef,
     TargetTypeDef,
     GetScheduleOutputTypeDef,
     CreateScheduleInputRequestTypeDef,
+    TargetUnionTypeDef,
     UpdateScheduleInputRequestTypeDef,
 )
 
 
-def get_structure() -> AwsVpcConfigurationOutputTypeDef:
+def get_value() -> AwsVpcConfigurationOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-scheduler-1.28.16/mypy_boto3_scheduler/__init__.py` & `mypy-boto3-scheduler-1.28.16.post1/mypy_boto3_scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-scheduler-1.28.16/mypy_boto3_scheduler/__init__.pyi` & `mypy-boto3-scheduler-1.28.16.post1/mypy_boto3_scheduler/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-scheduler-1.28.16/mypy_boto3_scheduler/__main__.py` & `mypy-boto3-scheduler-1.28.16.post1/mypy_boto3_scheduler/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.EventBridgeScheduler 1.28.16\nVersion:         1.28.16\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.EventBridgeScheduler 1.28.16\nVersion:        "
+        " 1.28.16.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.16")
+    print("1.28.16.post1")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-scheduler-1.28.16/mypy_boto3_scheduler/client.py` & `mypy-boto3-scheduler-1.28.16.post1/mypy_boto3_scheduler/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from mypy_boto3_scheduler.client import EventBridgeSchedulerClient
 
     session = Session()
     client: EventBridgeSchedulerClient = session.client("scheduler")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import ActionAfterCompletionType, ScheduleStateType
 from .paginator import ListScheduleGroupsPaginator, ListSchedulesPaginator
 from .type_defs import (
     CreateScheduleGroupOutputTypeDef,
@@ -27,16 +26,16 @@
     FlexibleTimeWindowTypeDef,
     GetScheduleGroupOutputTypeDef,
     GetScheduleOutputTypeDef,
     ListScheduleGroupsOutputTypeDef,
     ListSchedulesOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     TagTypeDef,
-    TargetOutputTypeDef,
-    TargetTypeDef,
+    TargetUnionTypeDef,
+    TimestampTypeDef,
     UpdateScheduleOutputTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -98,23 +97,23 @@
 
     def create_schedule(
         self,
         *,
         FlexibleTimeWindow: FlexibleTimeWindowTypeDef,
         Name: str,
         ScheduleExpression: str,
-        Target: Union[TargetTypeDef, TargetOutputTypeDef],
+        Target: TargetUnionTypeDef,
         ActionAfterCompletion: ActionAfterCompletionType = ...,
         ClientToken: str = ...,
         Description: str = ...,
-        EndDate: Union[datetime, str] = ...,
+        EndDate: TimestampTypeDef = ...,
         GroupName: str = ...,
         KmsKeyArn: str = ...,
         ScheduleExpressionTimezone: str = ...,
-        StartDate: Union[datetime, str] = ...,
+        StartDate: TimestampTypeDef = ...,
         State: ScheduleStateType = ...
     ) -> CreateScheduleOutputTypeDef:
         """
         Creates the specified schedule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler.Client.create_schedule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/client/#create_schedule)
@@ -232,23 +231,23 @@
 
     def update_schedule(
         self,
         *,
         FlexibleTimeWindow: FlexibleTimeWindowTypeDef,
         Name: str,
         ScheduleExpression: str,
-        Target: Union[TargetTypeDef, TargetOutputTypeDef],
+        Target: TargetUnionTypeDef,
         ActionAfterCompletion: ActionAfterCompletionType = ...,
         ClientToken: str = ...,
         Description: str = ...,
-        EndDate: Union[datetime, str] = ...,
+        EndDate: TimestampTypeDef = ...,
         GroupName: str = ...,
         KmsKeyArn: str = ...,
         ScheduleExpressionTimezone: str = ...,
-        StartDate: Union[datetime, str] = ...,
+        StartDate: TimestampTypeDef = ...,
         State: ScheduleStateType = ...
     ) -> UpdateScheduleOutputTypeDef:
         """
         Updates the specified schedule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler.Client.update_schedule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/client/#update_schedule)
```

### Comparing `mypy-boto3-scheduler-1.28.16/mypy_boto3_scheduler/client.pyi` & `mypy-boto3-scheduler-1.28.16.post1/mypy_boto3_scheduler/client.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from mypy_boto3_scheduler.client import EventBridgeSchedulerClient
 
     session = Session()
     client: EventBridgeSchedulerClient = session.client("scheduler")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import ActionAfterCompletionType, ScheduleStateType
 from .paginator import ListScheduleGroupsPaginator, ListSchedulesPaginator
 from .type_defs import (
     CreateScheduleGroupOutputTypeDef,
@@ -27,16 +26,16 @@
     FlexibleTimeWindowTypeDef,
     GetScheduleGroupOutputTypeDef,
     GetScheduleOutputTypeDef,
     ListScheduleGroupsOutputTypeDef,
     ListSchedulesOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     TagTypeDef,
-    TargetOutputTypeDef,
-    TargetTypeDef,
+    TargetUnionTypeDef,
+    TimestampTypeDef,
     UpdateScheduleOutputTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -91,23 +90,23 @@
         """
     def create_schedule(
         self,
         *,
         FlexibleTimeWindow: FlexibleTimeWindowTypeDef,
         Name: str,
         ScheduleExpression: str,
-        Target: Union[TargetTypeDef, TargetOutputTypeDef],
+        Target: TargetUnionTypeDef,
         ActionAfterCompletion: ActionAfterCompletionType = ...,
         ClientToken: str = ...,
         Description: str = ...,
-        EndDate: Union[datetime, str] = ...,
+        EndDate: TimestampTypeDef = ...,
         GroupName: str = ...,
         KmsKeyArn: str = ...,
         ScheduleExpressionTimezone: str = ...,
-        StartDate: Union[datetime, str] = ...,
+        StartDate: TimestampTypeDef = ...,
         State: ScheduleStateType = ...
     ) -> CreateScheduleOutputTypeDef:
         """
         Creates the specified schedule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler.Client.create_schedule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/client/#create_schedule)
@@ -213,23 +212,23 @@
         """
     def update_schedule(
         self,
         *,
         FlexibleTimeWindow: FlexibleTimeWindowTypeDef,
         Name: str,
         ScheduleExpression: str,
-        Target: Union[TargetTypeDef, TargetOutputTypeDef],
+        Target: TargetUnionTypeDef,
         ActionAfterCompletion: ActionAfterCompletionType = ...,
         ClientToken: str = ...,
         Description: str = ...,
-        EndDate: Union[datetime, str] = ...,
+        EndDate: TimestampTypeDef = ...,
         GroupName: str = ...,
         KmsKeyArn: str = ...,
         ScheduleExpressionTimezone: str = ...,
-        StartDate: Union[datetime, str] = ...,
+        StartDate: TimestampTypeDef = ...,
         State: ScheduleStateType = ...
     ) -> UpdateScheduleOutputTypeDef:
         """
         Updates the specified schedule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler.Client.update_schedule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/client/#update_schedule)
```

### Comparing `mypy-boto3-scheduler-1.28.16/mypy_boto3_scheduler/literals.py` & `mypy-boto3-scheduler-1.28.16.post1/mypy_boto3_scheduler/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-scheduler-1.28.16/mypy_boto3_scheduler/literals.pyi` & `mypy-boto3-scheduler-1.28.16.post1/mypy_boto3_scheduler/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-scheduler-1.28.16/mypy_boto3_scheduler/paginator.py` & `mypy-boto3-scheduler-1.28.16.post1/mypy_boto3_scheduler/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-scheduler-1.28.16/mypy_boto3_scheduler/paginator.pyi` & `mypy-boto3-scheduler-1.28.16.post1/mypy_boto3_scheduler/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-scheduler-1.28.16/mypy_boto3_scheduler/type_defs.py` & `mypy-boto3-scheduler-1.28.16.post1/mypy_boto3_scheduler/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_scheduler.type_defs import AwsVpcConfigurationOutputTypeDef
 
-    data: AwsVpcConfigurationOutputTypeDef = {...}
+    data: AwsVpcConfigurationOutputTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -39,14 +39,15 @@
 __all__ = (
     "AwsVpcConfigurationOutputTypeDef",
     "AwsVpcConfigurationTypeDef",
     "CapacityProviderStrategyItemTypeDef",
     "TagTypeDef",
     "ResponseMetadataTypeDef",
     "FlexibleTimeWindowTypeDef",
+    "TimestampTypeDef",
     "DeadLetterConfigTypeDef",
     "DeleteScheduleGroupInputRequestTypeDef",
     "DeleteScheduleInputRequestTypeDef",
     "PlacementConstraintTypeDef",
     "PlacementStrategyTypeDef",
     "EventBridgeParametersTypeDef",
     "GetScheduleGroupInputRequestTypeDef",
@@ -80,14 +81,15 @@
     "EcsParametersOutputTypeDef",
     "EcsParametersTypeDef",
     "ListSchedulesOutputTypeDef",
     "TargetOutputTypeDef",
     "TargetTypeDef",
     "GetScheduleOutputTypeDef",
     "CreateScheduleInputRequestTypeDef",
+    "TargetUnionTypeDef",
     "UpdateScheduleInputRequestTypeDef",
 )
 
 _RequiredAwsVpcConfigurationOutputTypeDef = TypedDict(
     "_RequiredAwsVpcConfigurationOutputTypeDef",
     {
         "Subnets": List[str],
@@ -189,14 +191,15 @@
 
 class FlexibleTimeWindowTypeDef(
     _RequiredFlexibleTimeWindowTypeDef, _OptionalFlexibleTimeWindowTypeDef
 ):
     pass
 
 
+TimestampTypeDef = Union[datetime, str]
 DeadLetterConfigTypeDef = TypedDict(
     "DeadLetterConfigTypeDef",
     {
         "Arn": str,
     },
     total=False,
 )
@@ -705,31 +708,32 @@
 )
 _OptionalCreateScheduleInputRequestTypeDef = TypedDict(
     "_OptionalCreateScheduleInputRequestTypeDef",
     {
         "ActionAfterCompletion": ActionAfterCompletionType,
         "ClientToken": str,
         "Description": str,
-        "EndDate": Union[datetime, str],
+        "EndDate": TimestampTypeDef,
         "GroupName": str,
         "KmsKeyArn": str,
         "ScheduleExpressionTimezone": str,
-        "StartDate": Union[datetime, str],
+        "StartDate": TimestampTypeDef,
         "State": ScheduleStateType,
     },
     total=False,
 )
 
 
 class CreateScheduleInputRequestTypeDef(
     _RequiredCreateScheduleInputRequestTypeDef, _OptionalCreateScheduleInputRequestTypeDef
 ):
     pass
 
 
+TargetUnionTypeDef = Union[TargetTypeDef, TargetOutputTypeDef]
 _RequiredUpdateScheduleInputRequestTypeDef = TypedDict(
     "_RequiredUpdateScheduleInputRequestTypeDef",
     {
         "FlexibleTimeWindow": FlexibleTimeWindowTypeDef,
         "Name": str,
         "ScheduleExpression": str,
         "Target": TargetTypeDef,
@@ -737,19 +741,19 @@
 )
 _OptionalUpdateScheduleInputRequestTypeDef = TypedDict(
     "_OptionalUpdateScheduleInputRequestTypeDef",
     {
         "ActionAfterCompletion": ActionAfterCompletionType,
         "ClientToken": str,
         "Description": str,
-        "EndDate": Union[datetime, str],
+        "EndDate": TimestampTypeDef,
         "GroupName": str,
         "KmsKeyArn": str,
         "ScheduleExpressionTimezone": str,
-        "StartDate": Union[datetime, str],
+        "StartDate": TimestampTypeDef,
         "State": ScheduleStateType,
     },
     total=False,
 )
 
 
 class UpdateScheduleInputRequestTypeDef(
```

### Comparing `mypy-boto3-scheduler-1.28.16/mypy_boto3_scheduler/type_defs.pyi` & `mypy-boto3-scheduler-1.28.16.post1/mypy_boto3_scheduler/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_scheduler.type_defs import AwsVpcConfigurationOutputTypeDef
 
-    data: AwsVpcConfigurationOutputTypeDef = {...}
+    data: AwsVpcConfigurationOutputTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -38,14 +38,15 @@
 __all__ = (
     "AwsVpcConfigurationOutputTypeDef",
     "AwsVpcConfigurationTypeDef",
     "CapacityProviderStrategyItemTypeDef",
     "TagTypeDef",
     "ResponseMetadataTypeDef",
     "FlexibleTimeWindowTypeDef",
+    "TimestampTypeDef",
     "DeadLetterConfigTypeDef",
     "DeleteScheduleGroupInputRequestTypeDef",
     "DeleteScheduleInputRequestTypeDef",
     "PlacementConstraintTypeDef",
     "PlacementStrategyTypeDef",
     "EventBridgeParametersTypeDef",
     "GetScheduleGroupInputRequestTypeDef",
@@ -79,14 +80,15 @@
     "EcsParametersOutputTypeDef",
     "EcsParametersTypeDef",
     "ListSchedulesOutputTypeDef",
     "TargetOutputTypeDef",
     "TargetTypeDef",
     "GetScheduleOutputTypeDef",
     "CreateScheduleInputRequestTypeDef",
+    "TargetUnionTypeDef",
     "UpdateScheduleInputRequestTypeDef",
 )
 
 _RequiredAwsVpcConfigurationOutputTypeDef = TypedDict(
     "_RequiredAwsVpcConfigurationOutputTypeDef",
     {
         "Subnets": List[str],
@@ -180,14 +182,15 @@
 )
 
 class FlexibleTimeWindowTypeDef(
     _RequiredFlexibleTimeWindowTypeDef, _OptionalFlexibleTimeWindowTypeDef
 ):
     pass
 
+TimestampTypeDef = Union[datetime, str]
 DeadLetterConfigTypeDef = TypedDict(
     "DeadLetterConfigTypeDef",
     {
         "Arn": str,
     },
     total=False,
 )
@@ -680,29 +683,30 @@
 )
 _OptionalCreateScheduleInputRequestTypeDef = TypedDict(
     "_OptionalCreateScheduleInputRequestTypeDef",
     {
         "ActionAfterCompletion": ActionAfterCompletionType,
         "ClientToken": str,
         "Description": str,
-        "EndDate": Union[datetime, str],
+        "EndDate": TimestampTypeDef,
         "GroupName": str,
         "KmsKeyArn": str,
         "ScheduleExpressionTimezone": str,
-        "StartDate": Union[datetime, str],
+        "StartDate": TimestampTypeDef,
         "State": ScheduleStateType,
     },
     total=False,
 )
 
 class CreateScheduleInputRequestTypeDef(
     _RequiredCreateScheduleInputRequestTypeDef, _OptionalCreateScheduleInputRequestTypeDef
 ):
     pass
 
+TargetUnionTypeDef = Union[TargetTypeDef, TargetOutputTypeDef]
 _RequiredUpdateScheduleInputRequestTypeDef = TypedDict(
     "_RequiredUpdateScheduleInputRequestTypeDef",
     {
         "FlexibleTimeWindow": FlexibleTimeWindowTypeDef,
         "Name": str,
         "ScheduleExpression": str,
         "Target": TargetTypeDef,
@@ -710,19 +714,19 @@
 )
 _OptionalUpdateScheduleInputRequestTypeDef = TypedDict(
     "_OptionalUpdateScheduleInputRequestTypeDef",
     {
         "ActionAfterCompletion": ActionAfterCompletionType,
         "ClientToken": str,
         "Description": str,
-        "EndDate": Union[datetime, str],
+        "EndDate": TimestampTypeDef,
         "GroupName": str,
         "KmsKeyArn": str,
         "ScheduleExpressionTimezone": str,
-        "StartDate": Union[datetime, str],
+        "StartDate": TimestampTypeDef,
         "State": ScheduleStateType,
     },
     total=False,
 )
 
 class UpdateScheduleInputRequestTypeDef(
     _RequiredUpdateScheduleInputRequestTypeDef, _OptionalUpdateScheduleInputRequestTypeDef
```

### Comparing `mypy-boto3-scheduler-1.28.16/mypy_boto3_scheduler.egg-info/PKG-INFO` & `mypy-boto3-scheduler-1.28.16.post1/mypy_boto3_scheduler.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-scheduler
-Version: 1.28.16
-Summary: Type annotations for boto3.EventBridgeScheduler 1.28.16 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16.post1
+Summary: Type annotations for boto3.EventBridgeScheduler 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 scheduler type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 scheduler type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -47,15 +47,15 @@
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
 [mypy-boto3-scheduler docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/).
 
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
@@ -323,29 +323,30 @@
 )
 
 
 def check_value(value: ActionAfterCompletionType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_scheduler.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_scheduler.type_defs import (
     AwsVpcConfigurationOutputTypeDef,
     AwsVpcConfigurationTypeDef,
     CapacityProviderStrategyItemTypeDef,
     TagTypeDef,
     ResponseMetadataTypeDef,
     FlexibleTimeWindowTypeDef,
+    TimestampTypeDef,
     DeadLetterConfigTypeDef,
     DeleteScheduleGroupInputRequestTypeDef,
     DeleteScheduleInputRequestTypeDef,
     PlacementConstraintTypeDef,
     PlacementStrategyTypeDef,
     EventBridgeParametersTypeDef,
     GetScheduleGroupInputRequestTypeDef,
@@ -379,19 +380,20 @@
     EcsParametersOutputTypeDef,
     EcsParametersTypeDef,
     ListSchedulesOutputTypeDef,
     TargetOutputTypeDef,
     TargetTypeDef,
     GetScheduleOutputTypeDef,
     CreateScheduleInputRequestTypeDef,
+    TargetUnionTypeDef,
     UpdateScheduleInputRequestTypeDef,
 )
 
 
-def get_structure() -> AwsVpcConfigurationOutputTypeDef:
+def get_value() -> AwsVpcConfigurationOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-scheduler-1.28.16/mypy_boto3_scheduler.egg-info/SOURCES.txt` & `mypy-boto3-scheduler-1.28.16.post1/mypy_boto3_scheduler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-scheduler-1.28.16/setup.py` & `mypy-boto3-scheduler-1.28.16.post1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-scheduler",
-    version="1.28.16",
+    version="1.28.16.post1",
     packages=["mypy_boto3_scheduler"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.EventBridgeScheduler 1.28.16 service generated with"
-        " mypy-boto3-builder 7.16.2"
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
-    keywords="boto3 scheduler type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 scheduler type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_scheduler": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_scheduler/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

