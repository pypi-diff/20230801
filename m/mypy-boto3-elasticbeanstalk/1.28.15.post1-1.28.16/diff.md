# Comparing `tmp/mypy-boto3-elasticbeanstalk-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-elasticbeanstalk-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-elasticbeanstalk-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:04 2023, max compression
+gzip compressed data, was "mypy-boto3-elasticbeanstalk-1.28.16.tar", last modified: Tue Aug  1 11:36:44 2023, max compression
```

## Comparing `mypy-boto3-elasticbeanstalk-1.28.15.post1.tar` & `mypy-boto3-elasticbeanstalk-1.28.16.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:04.389136 mypy-boto3-elasticbeanstalk-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:44:41.000000 mypy-boto3-elasticbeanstalk-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21421 2023-07-29 10:03:04.389136 mypy-boto3-elasticbeanstalk-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19892 2023-07-29 09:44:41.000000 mypy-boto3-elasticbeanstalk-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:04.385136 mypy-boto3-elasticbeanstalk-1.28.15.post1/mypy_boto3_elasticbeanstalk/
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-07-29 09:44:41.000000 mypy-boto3-elasticbeanstalk-1.28.15.post1/mypy_boto3_elasticbeanstalk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-07-29 09:44:41.000000 mypy-boto3-elasticbeanstalk-1.28.15.post1/mypy_boto3_elasticbeanstalk/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-29 09:44:41.000000 mypy-boto3-elasticbeanstalk-1.28.15.post1/mypy_boto3_elasticbeanstalk/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42686 2023-07-29 09:44:41.000000 mypy-boto3-elasticbeanstalk-1.28.15.post1/mypy_boto3_elasticbeanstalk/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    42624 2023-07-29 09:44:41.000000 mypy-boto3-elasticbeanstalk-1.28.15.post1/mypy_boto3_elasticbeanstalk/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11853 2023-07-29 09:44:41.000000 mypy-boto3-elasticbeanstalk-1.28.15.post1/mypy_boto3_elasticbeanstalk/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11851 2023-07-29 09:44:41.000000 mypy-boto3-elasticbeanstalk-1.28.15.post1/mypy_boto3_elasticbeanstalk/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7857 2023-07-29 09:44:41.000000 mypy-boto3-elasticbeanstalk-1.28.15.post1/mypy_boto3_elasticbeanstalk/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7850 2023-07-29 09:44:41.000000 mypy-boto3-elasticbeanstalk-1.28.15.post1/mypy_boto3_elasticbeanstalk/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:44:41.000000 mypy-boto3-elasticbeanstalk-1.28.15.post1/mypy_boto3_elasticbeanstalk/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    52740 2023-07-29 09:44:44.000000 mypy-boto3-elasticbeanstalk-1.28.15.post1/mypy_boto3_elasticbeanstalk/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    52701 2023-07-29 09:44:44.000000 mypy-boto3-elasticbeanstalk-1.28.15.post1/mypy_boto3_elasticbeanstalk/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:44:41.000000 mypy-boto3-elasticbeanstalk-1.28.15.post1/mypy_boto3_elasticbeanstalk/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4573 2023-07-29 09:44:41.000000 mypy-boto3-elasticbeanstalk-1.28.15.post1/mypy_boto3_elasticbeanstalk/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-07-29 09:44:41.000000 mypy-boto3-elasticbeanstalk-1.28.15.post1/mypy_boto3_elasticbeanstalk/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:04.389136 mypy-boto3-elasticbeanstalk-1.28.15.post1/mypy_boto3_elasticbeanstalk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21421 2023-07-29 10:03:04.000000 mypy-boto3-elasticbeanstalk-1.28.15.post1/mypy_boto3_elasticbeanstalk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-29 10:03:04.000000 mypy-boto3-elasticbeanstalk-1.28.15.post1/mypy_boto3_elasticbeanstalk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:04.000000 mypy-boto3-elasticbeanstalk-1.28.15.post1/mypy_boto3_elasticbeanstalk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:04.000000 mypy-boto3-elasticbeanstalk-1.28.15.post1/mypy_boto3_elasticbeanstalk.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:04.000000 mypy-boto3-elasticbeanstalk-1.28.15.post1/mypy_boto3_elasticbeanstalk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-29 10:03:04.000000 mypy-boto3-elasticbeanstalk-1.28.15.post1/mypy_boto3_elasticbeanstalk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:04.389136 mypy-boto3-elasticbeanstalk-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-07-29 09:44:40.000000 mypy-boto3-elasticbeanstalk-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:44.964896 mypy-boto3-elasticbeanstalk-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:17:17.000000 mypy-boto3-elasticbeanstalk-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21433 2023-08-01 11:36:44.964896 mypy-boto3-elasticbeanstalk-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19913 2023-08-01 11:17:17.000000 mypy-boto3-elasticbeanstalk-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:44.964896 mypy-boto3-elasticbeanstalk-1.28.16/mypy_boto3_elasticbeanstalk/
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-08-01 11:17:17.000000 mypy-boto3-elasticbeanstalk-1.28.16/mypy_boto3_elasticbeanstalk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-08-01 11:17:17.000000 mypy-boto3-elasticbeanstalk-1.28.16/mypy_boto3_elasticbeanstalk/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-08-01 11:17:17.000000 mypy-boto3-elasticbeanstalk-1.28.16/mypy_boto3_elasticbeanstalk/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42659 2023-08-01 11:17:18.000000 mypy-boto3-elasticbeanstalk-1.28.16/mypy_boto3_elasticbeanstalk/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42597 2023-08-01 11:17:18.000000 mypy-boto3-elasticbeanstalk-1.28.16/mypy_boto3_elasticbeanstalk/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11853 2023-08-01 11:17:18.000000 mypy-boto3-elasticbeanstalk-1.28.16/mypy_boto3_elasticbeanstalk/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11851 2023-08-01 11:17:18.000000 mypy-boto3-elasticbeanstalk-1.28.16/mypy_boto3_elasticbeanstalk/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7830 2023-08-01 11:17:18.000000 mypy-boto3-elasticbeanstalk-1.28.16/mypy_boto3_elasticbeanstalk/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7823 2023-08-01 11:17:18.000000 mypy-boto3-elasticbeanstalk-1.28.16/mypy_boto3_elasticbeanstalk/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:17:17.000000 mypy-boto3-elasticbeanstalk-1.28.16/mypy_boto3_elasticbeanstalk/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    52766 2023-08-01 11:17:20.000000 mypy-boto3-elasticbeanstalk-1.28.16/mypy_boto3_elasticbeanstalk/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52727 2023-08-01 11:17:19.000000 mypy-boto3-elasticbeanstalk-1.28.16/mypy_boto3_elasticbeanstalk/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:17:17.000000 mypy-boto3-elasticbeanstalk-1.28.16/mypy_boto3_elasticbeanstalk/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4542 2023-08-01 11:17:18.000000 mypy-boto3-elasticbeanstalk-1.28.16/mypy_boto3_elasticbeanstalk/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4539 2023-08-01 11:17:18.000000 mypy-boto3-elasticbeanstalk-1.28.16/mypy_boto3_elasticbeanstalk/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:44.964896 mypy-boto3-elasticbeanstalk-1.28.16/mypy_boto3_elasticbeanstalk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21433 2023-08-01 11:36:44.000000 mypy-boto3-elasticbeanstalk-1.28.16/mypy_boto3_elasticbeanstalk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-08-01 11:36:44.000000 mypy-boto3-elasticbeanstalk-1.28.16/mypy_boto3_elasticbeanstalk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:44.000000 mypy-boto3-elasticbeanstalk-1.28.16/mypy_boto3_elasticbeanstalk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:44.000000 mypy-boto3-elasticbeanstalk-1.28.16/mypy_boto3_elasticbeanstalk.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:44.000000 mypy-boto3-elasticbeanstalk-1.28.16/mypy_boto3_elasticbeanstalk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-01 11:36:44.000000 mypy-boto3-elasticbeanstalk-1.28.16/mypy_boto3_elasticbeanstalk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:44.964896 mypy-boto3-elasticbeanstalk-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-08-01 11:17:17.000000 mypy-boto3-elasticbeanstalk-1.28.16/setup.py
```

### Comparing `mypy-boto3-elasticbeanstalk-1.28.15.post1/LICENSE` & `mypy-boto3-elasticbeanstalk-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elasticbeanstalk-1.28.15.post1/PKG-INFO` & `mypy-boto3-elasticbeanstalk-1.28.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-elasticbeanstalk
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.ElasticBeanstalk 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.ElasticBeanstalk 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticbeanstalk/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 elasticbeanstalk type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 elasticbeanstalk type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-elasticbeanstalk.svg?color=blue)](https://pypi.org/project/mypy-boto3-elasticbeanstalk)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticbeanstalk/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-elasticbeanstalk)](https://pepy.tech/project/mypy-boto3-elasticbeanstalk)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ElasticBeanstalk 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk)
+[boto3.ElasticBeanstalk 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk)
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
 [mypy-boto3-elasticbeanstalk docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticbeanstalk/).
 
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
@@ -385,20 +385,20 @@
 )
 
 
 def check_value(value: ActionHistoryStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_elasticbeanstalk.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_elasticbeanstalk.type_defs import (
     AbortEnvironmentUpdateMessageRequestTypeDef,
     ResponseMetadataTypeDef,
     LatencyTypeDef,
     StatusCodesTypeDef,
@@ -436,17 +436,16 @@
     DescribeEnvironmentHealthRequestRequestTypeDef,
     InstanceHealthSummaryTypeDef,
     DescribeEnvironmentManagedActionHistoryRequestRequestTypeDef,
     ManagedActionHistoryItemTypeDef,
     DescribeEnvironmentManagedActionsRequestRequestTypeDef,
     ManagedActionTypeDef,
     DescribeEnvironmentResourcesMessageRequestTypeDef,
+    TimestampTypeDef,
     WaiterConfigTypeDef,
-    DescribeEnvironmentsMessageRequestTypeDef,
-    DescribeEventsMessageRequestTypeDef,
     DescribeInstancesHealthRequestRequestTypeDef,
     DescribePlatformVersionRequestRequestTypeDef,
     DisassociateEnvironmentOperationsRoleMessageRequestTypeDef,
     EnvironmentLinkTypeDef,
     EnvironmentInfoDescriptionTypeDef,
     InstanceTypeDef,
     LaunchConfigurationTypeDef,
@@ -495,18 +494,20 @@
     UpdateConfigurationTemplateMessageRequestTypeDef,
     UpdateEnvironmentMessageRequestTypeDef,
     CreatePlatformVersionResultTypeDef,
     DeletePlatformVersionResultTypeDef,
     ListPlatformVersionsResultTypeDef,
     DescribeApplicationVersionsMessageDescribeApplicationVersionsPaginateTypeDef,
     DescribeEnvironmentManagedActionHistoryRequestDescribeEnvironmentManagedActionHistoryPaginateTypeDef,
-    DescribeEnvironmentsMessageDescribeEnvironmentsPaginateTypeDef,
-    DescribeEventsMessageDescribeEventsPaginateTypeDef,
     DescribeEnvironmentManagedActionHistoryResultTypeDef,
     DescribeEnvironmentManagedActionsResultTypeDef,
+    DescribeEnvironmentsMessageDescribeEnvironmentsPaginateTypeDef,
+    DescribeEnvironmentsMessageRequestTypeDef,
+    DescribeEventsMessageDescribeEventsPaginateTypeDef,
+    DescribeEventsMessageRequestTypeDef,
     DescribeEnvironmentsMessageEnvironmentExistsWaitTypeDef,
     DescribeEnvironmentsMessageEnvironmentTerminatedWaitTypeDef,
     DescribeEnvironmentsMessageEnvironmentUpdatedWaitTypeDef,
     RetrieveEnvironmentInfoResultMessageTypeDef,
     EnvironmentResourceDescriptionTypeDef,
     EventDescriptionsMessageTypeDef,
     ListAvailableSolutionStacksResultMessageTypeDef,
@@ -537,15 +538,15 @@
     EnvironmentDescriptionTypeDef,
     ApplicationDescriptionMessageTypeDef,
     ApplicationDescriptionsMessageTypeDef,
     EnvironmentDescriptionsMessageTypeDef,
 )
 
 
-def get_structure() -> AbortEnvironmentUpdateMessageRequestTypeDef:
+def get_value() -> AbortEnvironmentUpdateMessageRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-elasticbeanstalk-1.28.15.post1/README.md` & `mypy-boto3-elasticbeanstalk-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-elasticbeanstalk.svg?color=blue)](https://pypi.org/project/mypy-boto3-elasticbeanstalk)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticbeanstalk/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-elasticbeanstalk)](https://pepy.tech/project/mypy-boto3-elasticbeanstalk)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ElasticBeanstalk 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk)
+[boto3.ElasticBeanstalk 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk)
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
 [mypy-boto3-elasticbeanstalk docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticbeanstalk/).
 
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
@@ -353,20 +353,20 @@
 )
 
 
 def check_value(value: ActionHistoryStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_elasticbeanstalk.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_elasticbeanstalk.type_defs import (
     AbortEnvironmentUpdateMessageRequestTypeDef,
     ResponseMetadataTypeDef,
     LatencyTypeDef,
     StatusCodesTypeDef,
@@ -404,17 +404,16 @@
     DescribeEnvironmentHealthRequestRequestTypeDef,
     InstanceHealthSummaryTypeDef,
     DescribeEnvironmentManagedActionHistoryRequestRequestTypeDef,
     ManagedActionHistoryItemTypeDef,
     DescribeEnvironmentManagedActionsRequestRequestTypeDef,
     ManagedActionTypeDef,
     DescribeEnvironmentResourcesMessageRequestTypeDef,
+    TimestampTypeDef,
     WaiterConfigTypeDef,
-    DescribeEnvironmentsMessageRequestTypeDef,
-    DescribeEventsMessageRequestTypeDef,
     DescribeInstancesHealthRequestRequestTypeDef,
     DescribePlatformVersionRequestRequestTypeDef,
     DisassociateEnvironmentOperationsRoleMessageRequestTypeDef,
     EnvironmentLinkTypeDef,
     EnvironmentInfoDescriptionTypeDef,
     InstanceTypeDef,
     LaunchConfigurationTypeDef,
@@ -463,18 +462,20 @@
     UpdateConfigurationTemplateMessageRequestTypeDef,
     UpdateEnvironmentMessageRequestTypeDef,
     CreatePlatformVersionResultTypeDef,
     DeletePlatformVersionResultTypeDef,
     ListPlatformVersionsResultTypeDef,
     DescribeApplicationVersionsMessageDescribeApplicationVersionsPaginateTypeDef,
     DescribeEnvironmentManagedActionHistoryRequestDescribeEnvironmentManagedActionHistoryPaginateTypeDef,
-    DescribeEnvironmentsMessageDescribeEnvironmentsPaginateTypeDef,
-    DescribeEventsMessageDescribeEventsPaginateTypeDef,
     DescribeEnvironmentManagedActionHistoryResultTypeDef,
     DescribeEnvironmentManagedActionsResultTypeDef,
+    DescribeEnvironmentsMessageDescribeEnvironmentsPaginateTypeDef,
+    DescribeEnvironmentsMessageRequestTypeDef,
+    DescribeEventsMessageDescribeEventsPaginateTypeDef,
+    DescribeEventsMessageRequestTypeDef,
     DescribeEnvironmentsMessageEnvironmentExistsWaitTypeDef,
     DescribeEnvironmentsMessageEnvironmentTerminatedWaitTypeDef,
     DescribeEnvironmentsMessageEnvironmentUpdatedWaitTypeDef,
     RetrieveEnvironmentInfoResultMessageTypeDef,
     EnvironmentResourceDescriptionTypeDef,
     EventDescriptionsMessageTypeDef,
     ListAvailableSolutionStacksResultMessageTypeDef,
@@ -505,15 +506,15 @@
     EnvironmentDescriptionTypeDef,
     ApplicationDescriptionMessageTypeDef,
     ApplicationDescriptionsMessageTypeDef,
     EnvironmentDescriptionsMessageTypeDef,
 )
 
 
-def get_structure() -> AbortEnvironmentUpdateMessageRequestTypeDef:
+def get_value() -> AbortEnvironmentUpdateMessageRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-elasticbeanstalk-1.28.15.post1/mypy_boto3_elasticbeanstalk/__init__.py` & `mypy-boto3-elasticbeanstalk-1.28.16/mypy_boto3_elasticbeanstalk/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elasticbeanstalk-1.28.15.post1/mypy_boto3_elasticbeanstalk/__init__.pyi` & `mypy-boto3-elasticbeanstalk-1.28.16/mypy_boto3_elasticbeanstalk/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elasticbeanstalk-1.28.15.post1/mypy_boto3_elasticbeanstalk/__main__.py` & `mypy-boto3-elasticbeanstalk-1.28.16/mypy_boto3_elasticbeanstalk/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ElasticBeanstalk 1.28.15\nVersion:        "
-        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.ElasticBeanstalk 1.28.16\nVersion:         1.28.16\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticbeanstalk//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk\nOther"
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

### Comparing `mypy-boto3-elasticbeanstalk-1.28.15.post1/mypy_boto3_elasticbeanstalk/client.py` & `mypy-boto3-elasticbeanstalk-1.28.16/mypy_boto3_elasticbeanstalk/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from mypy_boto3_elasticbeanstalk.client import ElasticBeanstalkClient
 
     session = Session()
     client: ElasticBeanstalkClient = session.client("elasticbeanstalk")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     ActionStatusType,
     EnvironmentHealthAttributeType,
     EnvironmentInfoTypeType,
@@ -71,14 +70,15 @@
     ResourceTagsDescriptionMessageTypeDef,
     RetrieveEnvironmentInfoResultMessageTypeDef,
     S3LocationTypeDef,
     SearchFilterTypeDef,
     SourceBuildInformationTypeDef,
     SourceConfigurationTypeDef,
     TagTypeDef,
+    TimestampTypeDef,
 )
 from .waiter import EnvironmentExistsWaiter, EnvironmentTerminatedWaiter, EnvironmentUpdatedWaiter
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -488,15 +488,15 @@
         self,
         *,
         ApplicationName: str = ...,
         VersionLabel: str = ...,
         EnvironmentIds: Sequence[str] = ...,
         EnvironmentNames: Sequence[str] = ...,
         IncludeDeleted: bool = ...,
-        IncludedDeletedBackTo: Union[datetime, str] = ...,
+        IncludedDeletedBackTo: TimestampTypeDef = ...,
         MaxRecords: int = ...,
         NextToken: str = ...
     ) -> EnvironmentDescriptionsMessageTypeDef:
         """
         Returns descriptions for existing environments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Client.describe_environments)
@@ -510,16 +510,16 @@
         VersionLabel: str = ...,
         TemplateName: str = ...,
         EnvironmentId: str = ...,
         EnvironmentName: str = ...,
         PlatformArn: str = ...,
         RequestId: str = ...,
         Severity: EventSeverityType = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         MaxRecords: int = ...,
         NextToken: str = ...
     ) -> EventDescriptionsMessageTypeDef:
         """
         Returns list of event descriptions matching criteria up to the last 6 weeks.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Client.describe_events)
```

### Comparing `mypy-boto3-elasticbeanstalk-1.28.15.post1/mypy_boto3_elasticbeanstalk/client.pyi` & `mypy-boto3-elasticbeanstalk-1.28.16/mypy_boto3_elasticbeanstalk/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from mypy_boto3_elasticbeanstalk.client import ElasticBeanstalkClient
 
     session = Session()
     client: ElasticBeanstalkClient = session.client("elasticbeanstalk")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     ActionStatusType,
     EnvironmentHealthAttributeType,
     EnvironmentInfoTypeType,
@@ -71,14 +70,15 @@
     ResourceTagsDescriptionMessageTypeDef,
     RetrieveEnvironmentInfoResultMessageTypeDef,
     S3LocationTypeDef,
     SearchFilterTypeDef,
     SourceBuildInformationTypeDef,
     SourceConfigurationTypeDef,
     TagTypeDef,
+    TimestampTypeDef,
 )
 from .waiter import EnvironmentExistsWaiter, EnvironmentTerminatedWaiter, EnvironmentUpdatedWaiter
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -456,15 +456,15 @@
         self,
         *,
         ApplicationName: str = ...,
         VersionLabel: str = ...,
         EnvironmentIds: Sequence[str] = ...,
         EnvironmentNames: Sequence[str] = ...,
         IncludeDeleted: bool = ...,
-        IncludedDeletedBackTo: Union[datetime, str] = ...,
+        IncludedDeletedBackTo: TimestampTypeDef = ...,
         MaxRecords: int = ...,
         NextToken: str = ...
     ) -> EnvironmentDescriptionsMessageTypeDef:
         """
         Returns descriptions for existing environments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Client.describe_environments)
@@ -477,16 +477,16 @@
         VersionLabel: str = ...,
         TemplateName: str = ...,
         EnvironmentId: str = ...,
         EnvironmentName: str = ...,
         PlatformArn: str = ...,
         RequestId: str = ...,
         Severity: EventSeverityType = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         MaxRecords: int = ...,
         NextToken: str = ...
     ) -> EventDescriptionsMessageTypeDef:
         """
         Returns list of event descriptions matching criteria up to the last 6 weeks.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Client.describe_events)
```

### Comparing `mypy-boto3-elasticbeanstalk-1.28.15.post1/mypy_boto3_elasticbeanstalk/literals.py` & `mypy-boto3-elasticbeanstalk-1.28.16/mypy_boto3_elasticbeanstalk/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elasticbeanstalk-1.28.15.post1/mypy_boto3_elasticbeanstalk/literals.pyi` & `mypy-boto3-elasticbeanstalk-1.28.16/mypy_boto3_elasticbeanstalk/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elasticbeanstalk-1.28.15.post1/mypy_boto3_elasticbeanstalk/paginator.py` & `mypy-boto3-elasticbeanstalk-1.28.16/mypy_boto3_elasticbeanstalk/paginator.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,28 +23,28 @@
     describe_application_versions_paginator: DescribeApplicationVersionsPaginator = client.get_paginator("describe_application_versions")
     describe_environment_managed_action_history_paginator: DescribeEnvironmentManagedActionHistoryPaginator = client.get_paginator("describe_environment_managed_action_history")
     describe_environments_paginator: DescribeEnvironmentsPaginator = client.get_paginator("describe_environments")
     describe_events_paginator: DescribeEventsPaginator = client.get_paginator("describe_events")
     list_platform_versions_paginator: ListPlatformVersionsPaginator = client.get_paginator("list_platform_versions")
     ```
 """
-from datetime import datetime
-from typing import Generic, Iterator, Sequence, TypeVar, Union
+from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import EventSeverityType
 from .type_defs import (
     ApplicationVersionDescriptionsMessageTypeDef,
     DescribeEnvironmentManagedActionHistoryResultTypeDef,
     EnvironmentDescriptionsMessageTypeDef,
     EventDescriptionsMessageTypeDef,
     ListPlatformVersionsResultTypeDef,
     PaginatorConfigTypeDef,
     PlatformFilterTypeDef,
+    TimestampTypeDef,
 )
 
 __all__ = (
     "DescribeApplicationVersionsPaginator",
     "DescribeEnvironmentManagedActionHistoryPaginator",
     "DescribeEnvironmentsPaginator",
     "DescribeEventsPaginator",
@@ -110,15 +110,15 @@
         self,
         *,
         ApplicationName: str = ...,
         VersionLabel: str = ...,
         EnvironmentIds: Sequence[str] = ...,
         EnvironmentNames: Sequence[str] = ...,
         IncludeDeleted: bool = ...,
-        IncludedDeletedBackTo: Union[datetime, str] = ...,
+        IncludedDeletedBackTo: TimestampTypeDef = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[EnvironmentDescriptionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Paginator.DescribeEnvironments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticbeanstalk/paginators/#describeenvironmentspaginator)
         """
 
@@ -136,16 +136,16 @@
         VersionLabel: str = ...,
         TemplateName: str = ...,
         EnvironmentId: str = ...,
         EnvironmentName: str = ...,
         PlatformArn: str = ...,
         RequestId: str = ...,
         Severity: EventSeverityType = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[EventDescriptionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Paginator.DescribeEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticbeanstalk/paginators/#describeeventspaginator)
         """
```

### Comparing `mypy-boto3-elasticbeanstalk-1.28.15.post1/mypy_boto3_elasticbeanstalk/paginator.pyi` & `mypy-boto3-elasticbeanstalk-1.28.16/mypy_boto3_elasticbeanstalk/paginator.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -23,28 +23,28 @@
     describe_application_versions_paginator: DescribeApplicationVersionsPaginator = client.get_paginator("describe_application_versions")
     describe_environment_managed_action_history_paginator: DescribeEnvironmentManagedActionHistoryPaginator = client.get_paginator("describe_environment_managed_action_history")
     describe_environments_paginator: DescribeEnvironmentsPaginator = client.get_paginator("describe_environments")
     describe_events_paginator: DescribeEventsPaginator = client.get_paginator("describe_events")
     list_platform_versions_paginator: ListPlatformVersionsPaginator = client.get_paginator("list_platform_versions")
     ```
 """
-from datetime import datetime
-from typing import Generic, Iterator, Sequence, TypeVar, Union
+from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import EventSeverityType
 from .type_defs import (
     ApplicationVersionDescriptionsMessageTypeDef,
     DescribeEnvironmentManagedActionHistoryResultTypeDef,
     EnvironmentDescriptionsMessageTypeDef,
     EventDescriptionsMessageTypeDef,
     ListPlatformVersionsResultTypeDef,
     PaginatorConfigTypeDef,
     PlatformFilterTypeDef,
+    TimestampTypeDef,
 )
 
 __all__ = (
     "DescribeApplicationVersionsPaginator",
     "DescribeEnvironmentManagedActionHistoryPaginator",
     "DescribeEnvironmentsPaginator",
     "DescribeEventsPaginator",
@@ -105,15 +105,15 @@
         self,
         *,
         ApplicationName: str = ...,
         VersionLabel: str = ...,
         EnvironmentIds: Sequence[str] = ...,
         EnvironmentNames: Sequence[str] = ...,
         IncludeDeleted: bool = ...,
-        IncludedDeletedBackTo: Union[datetime, str] = ...,
+        IncludedDeletedBackTo: TimestampTypeDef = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[EnvironmentDescriptionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Paginator.DescribeEnvironments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticbeanstalk/paginators/#describeenvironmentspaginator)
         """
 
@@ -130,16 +130,16 @@
         VersionLabel: str = ...,
         TemplateName: str = ...,
         EnvironmentId: str = ...,
         EnvironmentName: str = ...,
         PlatformArn: str = ...,
         RequestId: str = ...,
         Severity: EventSeverityType = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[EventDescriptionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Paginator.DescribeEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticbeanstalk/paginators/#describeeventspaginator)
         """
```

### Comparing `mypy-boto3-elasticbeanstalk-1.28.15.post1/mypy_boto3_elasticbeanstalk/type_defs.py` & `mypy-boto3-elasticbeanstalk-1.28.16/mypy_boto3_elasticbeanstalk/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticbeanstalk/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_elasticbeanstalk.type_defs import AbortEnvironmentUpdateMessageRequestTypeDef
 
-    data: AbortEnvironmentUpdateMessageRequestTypeDef = {...}
+    data: AbortEnvironmentUpdateMessageRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -82,17 +82,16 @@
     "DescribeEnvironmentHealthRequestRequestTypeDef",
     "InstanceHealthSummaryTypeDef",
     "DescribeEnvironmentManagedActionHistoryRequestRequestTypeDef",
     "ManagedActionHistoryItemTypeDef",
     "DescribeEnvironmentManagedActionsRequestRequestTypeDef",
     "ManagedActionTypeDef",
     "DescribeEnvironmentResourcesMessageRequestTypeDef",
+    "TimestampTypeDef",
     "WaiterConfigTypeDef",
-    "DescribeEnvironmentsMessageRequestTypeDef",
-    "DescribeEventsMessageRequestTypeDef",
     "DescribeInstancesHealthRequestRequestTypeDef",
     "DescribePlatformVersionRequestRequestTypeDef",
     "DisassociateEnvironmentOperationsRoleMessageRequestTypeDef",
     "EnvironmentLinkTypeDef",
     "EnvironmentInfoDescriptionTypeDef",
     "InstanceTypeDef",
     "LaunchConfigurationTypeDef",
@@ -141,18 +140,20 @@
     "UpdateConfigurationTemplateMessageRequestTypeDef",
     "UpdateEnvironmentMessageRequestTypeDef",
     "CreatePlatformVersionResultTypeDef",
     "DeletePlatformVersionResultTypeDef",
     "ListPlatformVersionsResultTypeDef",
     "DescribeApplicationVersionsMessageDescribeApplicationVersionsPaginateTypeDef",
     "DescribeEnvironmentManagedActionHistoryRequestDescribeEnvironmentManagedActionHistoryPaginateTypeDef",
-    "DescribeEnvironmentsMessageDescribeEnvironmentsPaginateTypeDef",
-    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
     "DescribeEnvironmentManagedActionHistoryResultTypeDef",
     "DescribeEnvironmentManagedActionsResultTypeDef",
+    "DescribeEnvironmentsMessageDescribeEnvironmentsPaginateTypeDef",
+    "DescribeEnvironmentsMessageRequestTypeDef",
+    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
+    "DescribeEventsMessageRequestTypeDef",
     "DescribeEnvironmentsMessageEnvironmentExistsWaitTypeDef",
     "DescribeEnvironmentsMessageEnvironmentTerminatedWaitTypeDef",
     "DescribeEnvironmentsMessageEnvironmentUpdatedWaitTypeDef",
     "RetrieveEnvironmentInfoResultMessageTypeDef",
     "EnvironmentResourceDescriptionTypeDef",
     "EventDescriptionsMessageTypeDef",
     "ListAvailableSolutionStacksResultMessageTypeDef",
@@ -699,57 +700,24 @@
     {
         "EnvironmentId": str,
         "EnvironmentName": str,
     },
     total=False,
 )
 
+TimestampTypeDef = Union[datetime, str]
 WaiterConfigTypeDef = TypedDict(
     "WaiterConfigTypeDef",
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
 )
 
-DescribeEnvironmentsMessageRequestTypeDef = TypedDict(
-    "DescribeEnvironmentsMessageRequestTypeDef",
-    {
-        "ApplicationName": str,
-        "VersionLabel": str,
-        "EnvironmentIds": Sequence[str],
-        "EnvironmentNames": Sequence[str],
-        "IncludeDeleted": bool,
-        "IncludedDeletedBackTo": Union[datetime, str],
-        "MaxRecords": int,
-        "NextToken": str,
-    },
-    total=False,
-)
-
-DescribeEventsMessageRequestTypeDef = TypedDict(
-    "DescribeEventsMessageRequestTypeDef",
-    {
-        "ApplicationName": str,
-        "VersionLabel": str,
-        "TemplateName": str,
-        "EnvironmentId": str,
-        "EnvironmentName": str,
-        "PlatformArn": str,
-        "RequestId": str,
-        "Severity": EventSeverityType,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "MaxRecords": int,
-        "NextToken": str,
-    },
-    total=False,
-)
-
 DescribeInstancesHealthRequestRequestTypeDef = TypedDict(
     "DescribeInstancesHealthRequestRequestTypeDef",
     {
         "EnvironmentName": str,
         "EnvironmentId": str,
         "AttributeNames": Sequence[InstancesHealthAttributeType],
         "NextToken": str,
@@ -1483,72 +1451,106 @@
         "EnvironmentId": str,
         "EnvironmentName": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+DescribeEnvironmentManagedActionHistoryResultTypeDef = TypedDict(
+    "DescribeEnvironmentManagedActionHistoryResultTypeDef",
+    {
+        "ManagedActionHistoryItems": List[ManagedActionHistoryItemTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeEnvironmentManagedActionsResultTypeDef = TypedDict(
+    "DescribeEnvironmentManagedActionsResultTypeDef",
+    {
+        "ManagedActions": List[ManagedActionTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DescribeEnvironmentsMessageDescribeEnvironmentsPaginateTypeDef = TypedDict(
     "DescribeEnvironmentsMessageDescribeEnvironmentsPaginateTypeDef",
     {
         "ApplicationName": str,
         "VersionLabel": str,
         "EnvironmentIds": Sequence[str],
         "EnvironmentNames": Sequence[str],
         "IncludeDeleted": bool,
-        "IncludedDeletedBackTo": Union[datetime, str],
+        "IncludedDeletedBackTo": TimestampTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+DescribeEnvironmentsMessageRequestTypeDef = TypedDict(
+    "DescribeEnvironmentsMessageRequestTypeDef",
+    {
+        "ApplicationName": str,
+        "VersionLabel": str,
+        "EnvironmentIds": Sequence[str],
+        "EnvironmentNames": Sequence[str],
+        "IncludeDeleted": bool,
+        "IncludedDeletedBackTo": TimestampTypeDef,
+        "MaxRecords": int,
+        "NextToken": str,
+    },
+    total=False,
+)
+
 DescribeEventsMessageDescribeEventsPaginateTypeDef = TypedDict(
     "DescribeEventsMessageDescribeEventsPaginateTypeDef",
     {
         "ApplicationName": str,
         "VersionLabel": str,
         "TemplateName": str,
         "EnvironmentId": str,
         "EnvironmentName": str,
         "PlatformArn": str,
         "RequestId": str,
         "Severity": EventSeverityType,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-DescribeEnvironmentManagedActionHistoryResultTypeDef = TypedDict(
-    "DescribeEnvironmentManagedActionHistoryResultTypeDef",
+DescribeEventsMessageRequestTypeDef = TypedDict(
+    "DescribeEventsMessageRequestTypeDef",
     {
-        "ManagedActionHistoryItems": List[ManagedActionHistoryItemTypeDef],
+        "ApplicationName": str,
+        "VersionLabel": str,
+        "TemplateName": str,
+        "EnvironmentId": str,
+        "EnvironmentName": str,
+        "PlatformArn": str,
+        "RequestId": str,
+        "Severity": EventSeverityType,
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "MaxRecords": int,
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeEnvironmentManagedActionsResultTypeDef = TypedDict(
-    "DescribeEnvironmentManagedActionsResultTypeDef",
-    {
-        "ManagedActions": List[ManagedActionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
     },
+    total=False,
 )
 
 DescribeEnvironmentsMessageEnvironmentExistsWaitTypeDef = TypedDict(
     "DescribeEnvironmentsMessageEnvironmentExistsWaitTypeDef",
     {
         "ApplicationName": str,
         "VersionLabel": str,
         "EnvironmentIds": Sequence[str],
         "EnvironmentNames": Sequence[str],
         "IncludeDeleted": bool,
-        "IncludedDeletedBackTo": Union[datetime, str],
+        "IncludedDeletedBackTo": TimestampTypeDef,
         "MaxRecords": int,
         "NextToken": str,
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
@@ -1556,15 +1558,15 @@
     "DescribeEnvironmentsMessageEnvironmentTerminatedWaitTypeDef",
     {
         "ApplicationName": str,
         "VersionLabel": str,
         "EnvironmentIds": Sequence[str],
         "EnvironmentNames": Sequence[str],
         "IncludeDeleted": bool,
-        "IncludedDeletedBackTo": Union[datetime, str],
+        "IncludedDeletedBackTo": TimestampTypeDef,
         "MaxRecords": int,
         "NextToken": str,
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
@@ -1572,15 +1574,15 @@
     "DescribeEnvironmentsMessageEnvironmentUpdatedWaitTypeDef",
     {
         "ApplicationName": str,
         "VersionLabel": str,
         "EnvironmentIds": Sequence[str],
         "EnvironmentNames": Sequence[str],
         "IncludeDeleted": bool,
-        "IncludedDeletedBackTo": Union[datetime, str],
+        "IncludedDeletedBackTo": TimestampTypeDef,
         "MaxRecords": int,
         "NextToken": str,
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
```

### Comparing `mypy-boto3-elasticbeanstalk-1.28.15.post1/mypy_boto3_elasticbeanstalk/type_defs.pyi` & `mypy-boto3-elasticbeanstalk-1.28.16/mypy_boto3_elasticbeanstalk/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticbeanstalk/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_elasticbeanstalk.type_defs import AbortEnvironmentUpdateMessageRequestTypeDef
 
-    data: AbortEnvironmentUpdateMessageRequestTypeDef = {...}
+    data: AbortEnvironmentUpdateMessageRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -81,17 +81,16 @@
     "DescribeEnvironmentHealthRequestRequestTypeDef",
     "InstanceHealthSummaryTypeDef",
     "DescribeEnvironmentManagedActionHistoryRequestRequestTypeDef",
     "ManagedActionHistoryItemTypeDef",
     "DescribeEnvironmentManagedActionsRequestRequestTypeDef",
     "ManagedActionTypeDef",
     "DescribeEnvironmentResourcesMessageRequestTypeDef",
+    "TimestampTypeDef",
     "WaiterConfigTypeDef",
-    "DescribeEnvironmentsMessageRequestTypeDef",
-    "DescribeEventsMessageRequestTypeDef",
     "DescribeInstancesHealthRequestRequestTypeDef",
     "DescribePlatformVersionRequestRequestTypeDef",
     "DisassociateEnvironmentOperationsRoleMessageRequestTypeDef",
     "EnvironmentLinkTypeDef",
     "EnvironmentInfoDescriptionTypeDef",
     "InstanceTypeDef",
     "LaunchConfigurationTypeDef",
@@ -140,18 +139,20 @@
     "UpdateConfigurationTemplateMessageRequestTypeDef",
     "UpdateEnvironmentMessageRequestTypeDef",
     "CreatePlatformVersionResultTypeDef",
     "DeletePlatformVersionResultTypeDef",
     "ListPlatformVersionsResultTypeDef",
     "DescribeApplicationVersionsMessageDescribeApplicationVersionsPaginateTypeDef",
     "DescribeEnvironmentManagedActionHistoryRequestDescribeEnvironmentManagedActionHistoryPaginateTypeDef",
-    "DescribeEnvironmentsMessageDescribeEnvironmentsPaginateTypeDef",
-    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
     "DescribeEnvironmentManagedActionHistoryResultTypeDef",
     "DescribeEnvironmentManagedActionsResultTypeDef",
+    "DescribeEnvironmentsMessageDescribeEnvironmentsPaginateTypeDef",
+    "DescribeEnvironmentsMessageRequestTypeDef",
+    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
+    "DescribeEventsMessageRequestTypeDef",
     "DescribeEnvironmentsMessageEnvironmentExistsWaitTypeDef",
     "DescribeEnvironmentsMessageEnvironmentTerminatedWaitTypeDef",
     "DescribeEnvironmentsMessageEnvironmentUpdatedWaitTypeDef",
     "RetrieveEnvironmentInfoResultMessageTypeDef",
     "EnvironmentResourceDescriptionTypeDef",
     "EventDescriptionsMessageTypeDef",
     "ListAvailableSolutionStacksResultMessageTypeDef",
@@ -684,57 +685,24 @@
     {
         "EnvironmentId": str,
         "EnvironmentName": str,
     },
     total=False,
 )
 
+TimestampTypeDef = Union[datetime, str]
 WaiterConfigTypeDef = TypedDict(
     "WaiterConfigTypeDef",
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
 )
 
-DescribeEnvironmentsMessageRequestTypeDef = TypedDict(
-    "DescribeEnvironmentsMessageRequestTypeDef",
-    {
-        "ApplicationName": str,
-        "VersionLabel": str,
-        "EnvironmentIds": Sequence[str],
-        "EnvironmentNames": Sequence[str],
-        "IncludeDeleted": bool,
-        "IncludedDeletedBackTo": Union[datetime, str],
-        "MaxRecords": int,
-        "NextToken": str,
-    },
-    total=False,
-)
-
-DescribeEventsMessageRequestTypeDef = TypedDict(
-    "DescribeEventsMessageRequestTypeDef",
-    {
-        "ApplicationName": str,
-        "VersionLabel": str,
-        "TemplateName": str,
-        "EnvironmentId": str,
-        "EnvironmentName": str,
-        "PlatformArn": str,
-        "RequestId": str,
-        "Severity": EventSeverityType,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "MaxRecords": int,
-        "NextToken": str,
-    },
-    total=False,
-)
-
 DescribeInstancesHealthRequestRequestTypeDef = TypedDict(
     "DescribeInstancesHealthRequestRequestTypeDef",
     {
         "EnvironmentName": str,
         "EnvironmentId": str,
         "AttributeNames": Sequence[InstancesHealthAttributeType],
         "NextToken": str,
@@ -1446,72 +1414,106 @@
         "EnvironmentId": str,
         "EnvironmentName": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+DescribeEnvironmentManagedActionHistoryResultTypeDef = TypedDict(
+    "DescribeEnvironmentManagedActionHistoryResultTypeDef",
+    {
+        "ManagedActionHistoryItems": List[ManagedActionHistoryItemTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeEnvironmentManagedActionsResultTypeDef = TypedDict(
+    "DescribeEnvironmentManagedActionsResultTypeDef",
+    {
+        "ManagedActions": List[ManagedActionTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DescribeEnvironmentsMessageDescribeEnvironmentsPaginateTypeDef = TypedDict(
     "DescribeEnvironmentsMessageDescribeEnvironmentsPaginateTypeDef",
     {
         "ApplicationName": str,
         "VersionLabel": str,
         "EnvironmentIds": Sequence[str],
         "EnvironmentNames": Sequence[str],
         "IncludeDeleted": bool,
-        "IncludedDeletedBackTo": Union[datetime, str],
+        "IncludedDeletedBackTo": TimestampTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+DescribeEnvironmentsMessageRequestTypeDef = TypedDict(
+    "DescribeEnvironmentsMessageRequestTypeDef",
+    {
+        "ApplicationName": str,
+        "VersionLabel": str,
+        "EnvironmentIds": Sequence[str],
+        "EnvironmentNames": Sequence[str],
+        "IncludeDeleted": bool,
+        "IncludedDeletedBackTo": TimestampTypeDef,
+        "MaxRecords": int,
+        "NextToken": str,
+    },
+    total=False,
+)
+
 DescribeEventsMessageDescribeEventsPaginateTypeDef = TypedDict(
     "DescribeEventsMessageDescribeEventsPaginateTypeDef",
     {
         "ApplicationName": str,
         "VersionLabel": str,
         "TemplateName": str,
         "EnvironmentId": str,
         "EnvironmentName": str,
         "PlatformArn": str,
         "RequestId": str,
         "Severity": EventSeverityType,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-DescribeEnvironmentManagedActionHistoryResultTypeDef = TypedDict(
-    "DescribeEnvironmentManagedActionHistoryResultTypeDef",
+DescribeEventsMessageRequestTypeDef = TypedDict(
+    "DescribeEventsMessageRequestTypeDef",
     {
-        "ManagedActionHistoryItems": List[ManagedActionHistoryItemTypeDef],
+        "ApplicationName": str,
+        "VersionLabel": str,
+        "TemplateName": str,
+        "EnvironmentId": str,
+        "EnvironmentName": str,
+        "PlatformArn": str,
+        "RequestId": str,
+        "Severity": EventSeverityType,
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "MaxRecords": int,
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeEnvironmentManagedActionsResultTypeDef = TypedDict(
-    "DescribeEnvironmentManagedActionsResultTypeDef",
-    {
-        "ManagedActions": List[ManagedActionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
     },
+    total=False,
 )
 
 DescribeEnvironmentsMessageEnvironmentExistsWaitTypeDef = TypedDict(
     "DescribeEnvironmentsMessageEnvironmentExistsWaitTypeDef",
     {
         "ApplicationName": str,
         "VersionLabel": str,
         "EnvironmentIds": Sequence[str],
         "EnvironmentNames": Sequence[str],
         "IncludeDeleted": bool,
-        "IncludedDeletedBackTo": Union[datetime, str],
+        "IncludedDeletedBackTo": TimestampTypeDef,
         "MaxRecords": int,
         "NextToken": str,
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
@@ -1519,15 +1521,15 @@
     "DescribeEnvironmentsMessageEnvironmentTerminatedWaitTypeDef",
     {
         "ApplicationName": str,
         "VersionLabel": str,
         "EnvironmentIds": Sequence[str],
         "EnvironmentNames": Sequence[str],
         "IncludeDeleted": bool,
-        "IncludedDeletedBackTo": Union[datetime, str],
+        "IncludedDeletedBackTo": TimestampTypeDef,
         "MaxRecords": int,
         "NextToken": str,
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
@@ -1535,15 +1537,15 @@
     "DescribeEnvironmentsMessageEnvironmentUpdatedWaitTypeDef",
     {
         "ApplicationName": str,
         "VersionLabel": str,
         "EnvironmentIds": Sequence[str],
         "EnvironmentNames": Sequence[str],
         "IncludeDeleted": bool,
-        "IncludedDeletedBackTo": Union[datetime, str],
+        "IncludedDeletedBackTo": TimestampTypeDef,
         "MaxRecords": int,
         "NextToken": str,
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
```

### Comparing `mypy-boto3-elasticbeanstalk-1.28.15.post1/mypy_boto3_elasticbeanstalk/waiter.py` & `mypy-boto3-elasticbeanstalk-1.28.16/mypy_boto3_elasticbeanstalk/waiter.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,20 +19,19 @@
     client: ElasticBeanstalkClient = session.client("elasticbeanstalk")
 
     environment_exists_waiter: EnvironmentExistsWaiter = client.get_waiter("environment_exists")
     environment_terminated_waiter: EnvironmentTerminatedWaiter = client.get_waiter("environment_terminated")
     environment_updated_waiter: EnvironmentUpdatedWaiter = client.get_waiter("environment_updated")
     ```
 """
-from datetime import datetime
-from typing import Sequence, Union
+from typing import Sequence
 
 from botocore.waiter import Waiter
 
-from .type_defs import WaiterConfigTypeDef
+from .type_defs import TimestampTypeDef, WaiterConfigTypeDef
 
 __all__ = ("EnvironmentExistsWaiter", "EnvironmentTerminatedWaiter", "EnvironmentUpdatedWaiter")
 
 
 class EnvironmentExistsWaiter(Waiter):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Waiter.EnvironmentExists)
@@ -43,15 +42,15 @@
         self,
         *,
         ApplicationName: str = ...,
         VersionLabel: str = ...,
         EnvironmentIds: Sequence[str] = ...,
         EnvironmentNames: Sequence[str] = ...,
         IncludeDeleted: bool = ...,
-        IncludedDeletedBackTo: Union[datetime, str] = ...,
+        IncludedDeletedBackTo: TimestampTypeDef = ...,
         MaxRecords: int = ...,
         NextToken: str = ...,
         WaiterConfig: WaiterConfigTypeDef = ...
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Waiter.EnvironmentExists.wait)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticbeanstalk/waiters/#environmentexistswaiter)
@@ -68,15 +67,15 @@
         self,
         *,
         ApplicationName: str = ...,
         VersionLabel: str = ...,
         EnvironmentIds: Sequence[str] = ...,
         EnvironmentNames: Sequence[str] = ...,
         IncludeDeleted: bool = ...,
-        IncludedDeletedBackTo: Union[datetime, str] = ...,
+        IncludedDeletedBackTo: TimestampTypeDef = ...,
         MaxRecords: int = ...,
         NextToken: str = ...,
         WaiterConfig: WaiterConfigTypeDef = ...
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Waiter.EnvironmentTerminated.wait)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticbeanstalk/waiters/#environmentterminatedwaiter)
@@ -93,15 +92,15 @@
         self,
         *,
         ApplicationName: str = ...,
         VersionLabel: str = ...,
         EnvironmentIds: Sequence[str] = ...,
         EnvironmentNames: Sequence[str] = ...,
         IncludeDeleted: bool = ...,
-        IncludedDeletedBackTo: Union[datetime, str] = ...,
+        IncludedDeletedBackTo: TimestampTypeDef = ...,
         MaxRecords: int = ...,
         NextToken: str = ...,
         WaiterConfig: WaiterConfigTypeDef = ...
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Waiter.EnvironmentUpdated.wait)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticbeanstalk/waiters/#environmentupdatedwaiter)
```

### Comparing `mypy-boto3-elasticbeanstalk-1.28.15.post1/mypy_boto3_elasticbeanstalk/waiter.pyi` & `mypy-boto3-elasticbeanstalk-1.28.16/mypy_boto3_elasticbeanstalk/waiter.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -19,20 +19,19 @@
     client: ElasticBeanstalkClient = session.client("elasticbeanstalk")
 
     environment_exists_waiter: EnvironmentExistsWaiter = client.get_waiter("environment_exists")
     environment_terminated_waiter: EnvironmentTerminatedWaiter = client.get_waiter("environment_terminated")
     environment_updated_waiter: EnvironmentUpdatedWaiter = client.get_waiter("environment_updated")
     ```
 """
-from datetime import datetime
-from typing import Sequence, Union
+from typing import Sequence
 
 from botocore.waiter import Waiter
 
-from .type_defs import WaiterConfigTypeDef
+from .type_defs import TimestampTypeDef, WaiterConfigTypeDef
 
 __all__ = ("EnvironmentExistsWaiter", "EnvironmentTerminatedWaiter", "EnvironmentUpdatedWaiter")
 
 class EnvironmentExistsWaiter(Waiter):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Waiter.EnvironmentExists)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticbeanstalk/waiters/#environmentexistswaiter)
@@ -42,15 +41,15 @@
         self,
         *,
         ApplicationName: str = ...,
         VersionLabel: str = ...,
         EnvironmentIds: Sequence[str] = ...,
         EnvironmentNames: Sequence[str] = ...,
         IncludeDeleted: bool = ...,
-        IncludedDeletedBackTo: Union[datetime, str] = ...,
+        IncludedDeletedBackTo: TimestampTypeDef = ...,
         MaxRecords: int = ...,
         NextToken: str = ...,
         WaiterConfig: WaiterConfigTypeDef = ...
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Waiter.EnvironmentExists.wait)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticbeanstalk/waiters/#environmentexistswaiter)
@@ -66,15 +65,15 @@
         self,
         *,
         ApplicationName: str = ...,
         VersionLabel: str = ...,
         EnvironmentIds: Sequence[str] = ...,
         EnvironmentNames: Sequence[str] = ...,
         IncludeDeleted: bool = ...,
-        IncludedDeletedBackTo: Union[datetime, str] = ...,
+        IncludedDeletedBackTo: TimestampTypeDef = ...,
         MaxRecords: int = ...,
         NextToken: str = ...,
         WaiterConfig: WaiterConfigTypeDef = ...
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Waiter.EnvironmentTerminated.wait)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticbeanstalk/waiters/#environmentterminatedwaiter)
@@ -90,15 +89,15 @@
         self,
         *,
         ApplicationName: str = ...,
         VersionLabel: str = ...,
         EnvironmentIds: Sequence[str] = ...,
         EnvironmentNames: Sequence[str] = ...,
         IncludeDeleted: bool = ...,
-        IncludedDeletedBackTo: Union[datetime, str] = ...,
+        IncludedDeletedBackTo: TimestampTypeDef = ...,
         MaxRecords: int = ...,
         NextToken: str = ...,
         WaiterConfig: WaiterConfigTypeDef = ...
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Waiter.EnvironmentUpdated.wait)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticbeanstalk/waiters/#environmentupdatedwaiter)
```

### Comparing `mypy-boto3-elasticbeanstalk-1.28.15.post1/mypy_boto3_elasticbeanstalk.egg-info/PKG-INFO` & `mypy-boto3-elasticbeanstalk-1.28.16/mypy_boto3_elasticbeanstalk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-elasticbeanstalk
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.ElasticBeanstalk 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.ElasticBeanstalk 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticbeanstalk/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 elasticbeanstalk type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 elasticbeanstalk type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-elasticbeanstalk.svg?color=blue)](https://pypi.org/project/mypy-boto3-elasticbeanstalk)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticbeanstalk/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-elasticbeanstalk)](https://pepy.tech/project/mypy-boto3-elasticbeanstalk)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ElasticBeanstalk 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk)
+[boto3.ElasticBeanstalk 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk)
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
 [mypy-boto3-elasticbeanstalk docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticbeanstalk/).
 
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
@@ -385,20 +385,20 @@
 )
 
 
 def check_value(value: ActionHistoryStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_elasticbeanstalk.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_elasticbeanstalk.type_defs import (
     AbortEnvironmentUpdateMessageRequestTypeDef,
     ResponseMetadataTypeDef,
     LatencyTypeDef,
     StatusCodesTypeDef,
@@ -436,17 +436,16 @@
     DescribeEnvironmentHealthRequestRequestTypeDef,
     InstanceHealthSummaryTypeDef,
     DescribeEnvironmentManagedActionHistoryRequestRequestTypeDef,
     ManagedActionHistoryItemTypeDef,
     DescribeEnvironmentManagedActionsRequestRequestTypeDef,
     ManagedActionTypeDef,
     DescribeEnvironmentResourcesMessageRequestTypeDef,
+    TimestampTypeDef,
     WaiterConfigTypeDef,
-    DescribeEnvironmentsMessageRequestTypeDef,
-    DescribeEventsMessageRequestTypeDef,
     DescribeInstancesHealthRequestRequestTypeDef,
     DescribePlatformVersionRequestRequestTypeDef,
     DisassociateEnvironmentOperationsRoleMessageRequestTypeDef,
     EnvironmentLinkTypeDef,
     EnvironmentInfoDescriptionTypeDef,
     InstanceTypeDef,
     LaunchConfigurationTypeDef,
@@ -495,18 +494,20 @@
     UpdateConfigurationTemplateMessageRequestTypeDef,
     UpdateEnvironmentMessageRequestTypeDef,
     CreatePlatformVersionResultTypeDef,
     DeletePlatformVersionResultTypeDef,
     ListPlatformVersionsResultTypeDef,
     DescribeApplicationVersionsMessageDescribeApplicationVersionsPaginateTypeDef,
     DescribeEnvironmentManagedActionHistoryRequestDescribeEnvironmentManagedActionHistoryPaginateTypeDef,
-    DescribeEnvironmentsMessageDescribeEnvironmentsPaginateTypeDef,
-    DescribeEventsMessageDescribeEventsPaginateTypeDef,
     DescribeEnvironmentManagedActionHistoryResultTypeDef,
     DescribeEnvironmentManagedActionsResultTypeDef,
+    DescribeEnvironmentsMessageDescribeEnvironmentsPaginateTypeDef,
+    DescribeEnvironmentsMessageRequestTypeDef,
+    DescribeEventsMessageDescribeEventsPaginateTypeDef,
+    DescribeEventsMessageRequestTypeDef,
     DescribeEnvironmentsMessageEnvironmentExistsWaitTypeDef,
     DescribeEnvironmentsMessageEnvironmentTerminatedWaitTypeDef,
     DescribeEnvironmentsMessageEnvironmentUpdatedWaitTypeDef,
     RetrieveEnvironmentInfoResultMessageTypeDef,
     EnvironmentResourceDescriptionTypeDef,
     EventDescriptionsMessageTypeDef,
     ListAvailableSolutionStacksResultMessageTypeDef,
@@ -537,15 +538,15 @@
     EnvironmentDescriptionTypeDef,
     ApplicationDescriptionMessageTypeDef,
     ApplicationDescriptionsMessageTypeDef,
     EnvironmentDescriptionsMessageTypeDef,
 )
 
 
-def get_structure() -> AbortEnvironmentUpdateMessageRequestTypeDef:
+def get_value() -> AbortEnvironmentUpdateMessageRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-elasticbeanstalk-1.28.15.post1/mypy_boto3_elasticbeanstalk.egg-info/SOURCES.txt` & `mypy-boto3-elasticbeanstalk-1.28.16/mypy_boto3_elasticbeanstalk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elasticbeanstalk-1.28.15.post1/setup.py` & `mypy-boto3-elasticbeanstalk-1.28.16/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-elasticbeanstalk",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_elasticbeanstalk"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ElasticBeanstalk 1.28.15 service generated with"
-        " mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.ElasticBeanstalk 1.28.16 service generated with"
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
-    keywords="boto3 elasticbeanstalk type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 elasticbeanstalk type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_elasticbeanstalk": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticbeanstalk/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

