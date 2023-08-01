# Comparing `tmp/mypy-boto3-sms-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-sms-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-sms-1.28.15.post1.tar", last modified: Sat Jul 29 10:04:13 2023, max compression
+gzip compressed data, was "mypy-boto3-sms-1.28.16.tar", last modified: Tue Aug  1 11:37:53 2023, max compression
```

## Comparing `mypy-boto3-sms-1.28.15.post1.tar` & `mypy-boto3-sms-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:13.497409 mypy-boto3-sms-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:59:44.000000 mypy-boto3-sms-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17055 2023-07-29 10:04:13.493409 mypy-boto3-sms-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15578 2023-07-29 09:59:44.000000 mypy-boto3-sms-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:13.489409 mypy-boto3-sms-1.28.15.post1/mypy_boto3_sms/
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-29 09:59:44.000000 mypy-boto3-sms-1.28.15.post1/mypy_boto3_sms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-29 09:59:44.000000 mypy-boto3-sms-1.28.15.post1/mypy_boto3_sms/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-29 09:59:44.000000 mypy-boto3-sms-1.28.15.post1/mypy_boto3_sms/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26432 2023-07-29 09:59:45.000000 mypy-boto3-sms-1.28.15.post1/mypy_boto3_sms/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    26385 2023-07-29 09:59:45.000000 mypy-boto3-sms-1.28.15.post1/mypy_boto3_sms/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11056 2023-07-29 09:59:45.000000 mypy-boto3-sms-1.28.15.post1/mypy_boto3_sms/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11054 2023-07-29 09:59:45.000000 mypy-boto3-sms-1.28.15.post1/mypy_boto3_sms/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5909 2023-07-29 09:59:45.000000 mypy-boto3-sms-1.28.15.post1/mypy_boto3_sms/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5902 2023-07-29 09:59:45.000000 mypy-boto3-sms-1.28.15.post1/mypy_boto3_sms/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:59:44.000000 mypy-boto3-sms-1.28.15.post1/mypy_boto3_sms/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    30876 2023-07-29 09:59:46.000000 mypy-boto3-sms-1.28.15.post1/mypy_boto3_sms/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    30859 2023-07-29 09:59:45.000000 mypy-boto3-sms-1.28.15.post1/mypy_boto3_sms/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:59:44.000000 mypy-boto3-sms-1.28.15.post1/mypy_boto3_sms/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:13.493409 mypy-boto3-sms-1.28.15.post1/mypy_boto3_sms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17055 2023-07-29 10:04:13.000000 mypy-boto3-sms-1.28.15.post1/mypy_boto3_sms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-29 10:04:13.000000 mypy-boto3-sms-1.28.15.post1/mypy_boto3_sms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:13.000000 mypy-boto3-sms-1.28.15.post1/mypy_boto3_sms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:13.000000 mypy-boto3-sms-1.28.15.post1/mypy_boto3_sms.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:04:13.000000 mypy-boto3-sms-1.28.15.post1/mypy_boto3_sms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-29 10:04:13.000000 mypy-boto3-sms-1.28.15.post1/mypy_boto3_sms.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:04:13.497409 mypy-boto3-sms-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-29 09:59:44.000000 mypy-boto3-sms-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:53.640724 mypy-boto3-sms-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:33:18.000000 mypy-boto3-sms-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17249 2023-08-01 11:37:53.636724 mypy-boto3-sms-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15781 2023-08-01 11:33:18.000000 mypy-boto3-sms-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:53.632724 mypy-boto3-sms-1.28.16/mypy_boto3_sms/
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-08-01 11:33:18.000000 mypy-boto3-sms-1.28.16/mypy_boto3_sms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-08-01 11:33:18.000000 mypy-boto3-sms-1.28.16/mypy_boto3_sms/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-08-01 11:33:18.000000 mypy-boto3-sms-1.28.16/mypy_boto3_sms/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25891 2023-08-01 11:33:18.000000 mypy-boto3-sms-1.28.16/mypy_boto3_sms/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25844 2023-08-01 11:33:18.000000 mypy-boto3-sms-1.28.16/mypy_boto3_sms/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11056 2023-08-01 11:33:19.000000 mypy-boto3-sms-1.28.16/mypy_boto3_sms/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11054 2023-08-01 11:33:18.000000 mypy-boto3-sms-1.28.16/mypy_boto3_sms/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5909 2023-08-01 11:33:18.000000 mypy-boto3-sms-1.28.16/mypy_boto3_sms/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5902 2023-08-01 11:33:18.000000 mypy-boto3-sms-1.28.16/mypy_boto3_sms/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:33:18.000000 mypy-boto3-sms-1.28.16/mypy_boto3_sms/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    31291 2023-08-01 11:33:19.000000 mypy-boto3-sms-1.28.16/mypy_boto3_sms/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31275 2023-08-01 11:33:19.000000 mypy-boto3-sms-1.28.16/mypy_boto3_sms/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:33:18.000000 mypy-boto3-sms-1.28.16/mypy_boto3_sms/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:53.636724 mypy-boto3-sms-1.28.16/mypy_boto3_sms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17249 2023-08-01 11:37:53.000000 mypy-boto3-sms-1.28.16/mypy_boto3_sms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-08-01 11:37:53.000000 mypy-boto3-sms-1.28.16/mypy_boto3_sms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:53.000000 mypy-boto3-sms-1.28.16/mypy_boto3_sms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:53.000000 mypy-boto3-sms-1.28.16/mypy_boto3_sms.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:53.000000 mypy-boto3-sms-1.28.16/mypy_boto3_sms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-01 11:37:53.000000 mypy-boto3-sms-1.28.16/mypy_boto3_sms.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:53.640724 mypy-boto3-sms-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-08-01 11:33:18.000000 mypy-boto3-sms-1.28.16/setup.py
```

### Comparing `mypy-boto3-sms-1.28.15.post1/LICENSE` & `mypy-boto3-sms-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sms-1.28.15.post1/PKG-INFO` & `mypy-boto3-sms-1.28.16/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sms
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.SMS 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.SMS 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 sms type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 sms type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sms.svg?color=blue)](https://pypi.org/project/mypy-boto3-sms)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sms)](https://pepy.tech/project/mypy-boto3-sms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SMS 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS)
+[boto3.SMS 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS)
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
 [mypy-boto3-sms docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/).
 
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
@@ -345,28 +345,28 @@
 )
 
 
 def check_value(value: AppLaunchConfigurationStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_sms.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_sms.type_defs import (
     LaunchDetailsTypeDef,
     ConnectorTypeDef,
     TagTypeDef,
     ResponseMetadataTypeDef,
-    CreateReplicationJobRequestRequestTypeDef,
+    TimestampTypeDef,
     DeleteAppLaunchConfigurationRequestRequestTypeDef,
     DeleteAppReplicationConfigurationRequestRequestTypeDef,
     DeleteAppRequestRequestTypeDef,
     DeleteAppValidationConfigurationRequestRequestTypeDef,
     DeleteReplicationJobRequestRequestTypeDef,
     DisassociateConnectorRequestRequestTypeDef,
     GenerateChangeSetRequestRequestTypeDef,
@@ -384,25 +384,26 @@
     VmServerAddressTypeDef,
     ImportAppCatalogRequestRequestTypeDef,
     LaunchAppRequestRequestTypeDef,
     ListAppsRequestRequestTypeDef,
     NotificationContextTypeDef,
     ReplicationRunStageDetailsTypeDef,
     ServerReplicationParametersOutputTypeDef,
-    ServerReplicationParametersTypeDef,
     StartAppReplicationRequestRequestTypeDef,
     StartOnDemandAppReplicationRequestRequestTypeDef,
     StartOnDemandReplicationRunRequestRequestTypeDef,
     StopAppReplicationRequestRequestTypeDef,
     TerminateAppRequestRequestTypeDef,
-    UpdateReplicationJobRequestRequestTypeDef,
     AppSummaryTypeDef,
     CreateReplicationJobResponseTypeDef,
     GetConnectorsResponseTypeDef,
     StartOnDemandReplicationRunResponseTypeDef,
+    CreateReplicationJobRequestRequestTypeDef,
+    ServerReplicationParametersTypeDef,
+    UpdateReplicationJobRequestRequestTypeDef,
     GenerateChangeSetResponseTypeDef,
     GenerateTemplateResponseTypeDef,
     SSMOutputTypeDef,
     SourceTypeDef,
     UserDataTypeDef,
     GetConnectorsRequestGetConnectorsPaginateTypeDef,
     GetReplicationJobsRequestGetReplicationJobsPaginateTypeDef,
@@ -429,34 +430,38 @@
     ServerValidationConfigurationTypeDef,
     ServerValidationOutputTypeDef,
     GetReplicationJobsResponseTypeDef,
     GetReplicationRunsResponseTypeDef,
     CreateAppResponseTypeDef,
     GetAppResponseTypeDef,
     UpdateAppResponseTypeDef,
-    CreateAppRequestRequestTypeDef,
-    UpdateAppRequestRequestTypeDef,
+    ServerGroupUnionTypeDef,
     ServerGroupLaunchConfigurationOutputTypeDef,
     ServerGroupLaunchConfigurationTypeDef,
     ServerGroupReplicationConfigurationOutputTypeDef,
     ServerGroupReplicationConfigurationTypeDef,
     ServerGroupValidationConfigurationOutputTypeDef,
     ServerGroupValidationConfigurationTypeDef,
     ValidationOutputTypeDef,
+    CreateAppRequestRequestTypeDef,
+    UpdateAppRequestRequestTypeDef,
     GetAppLaunchConfigurationResponseTypeDef,
-    PutAppLaunchConfigurationRequestRequestTypeDef,
+    ServerGroupLaunchConfigurationUnionTypeDef,
     GetAppReplicationConfigurationResponseTypeDef,
-    PutAppReplicationConfigurationRequestRequestTypeDef,
+    ServerGroupReplicationConfigurationUnionTypeDef,
     GetAppValidationConfigurationResponseTypeDef,
-    PutAppValidationConfigurationRequestRequestTypeDef,
+    ServerGroupValidationConfigurationUnionTypeDef,
     GetAppValidationOutputResponseTypeDef,
+    PutAppLaunchConfigurationRequestRequestTypeDef,
+    PutAppReplicationConfigurationRequestRequestTypeDef,
+    PutAppValidationConfigurationRequestRequestTypeDef,
 )
 
 
-def get_structure() -> LaunchDetailsTypeDef:
+def get_value() -> LaunchDetailsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-sms-1.28.15.post1/README.md` & `mypy-boto3-sms-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sms.svg?color=blue)](https://pypi.org/project/mypy-boto3-sms)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sms)](https://pepy.tech/project/mypy-boto3-sms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SMS 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS)
+[boto3.SMS 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS)
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
 [mypy-boto3-sms docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/).
 
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
@@ -313,28 +313,28 @@
 )
 
 
 def check_value(value: AppLaunchConfigurationStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_sms.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_sms.type_defs import (
     LaunchDetailsTypeDef,
     ConnectorTypeDef,
     TagTypeDef,
     ResponseMetadataTypeDef,
-    CreateReplicationJobRequestRequestTypeDef,
+    TimestampTypeDef,
     DeleteAppLaunchConfigurationRequestRequestTypeDef,
     DeleteAppReplicationConfigurationRequestRequestTypeDef,
     DeleteAppRequestRequestTypeDef,
     DeleteAppValidationConfigurationRequestRequestTypeDef,
     DeleteReplicationJobRequestRequestTypeDef,
     DisassociateConnectorRequestRequestTypeDef,
     GenerateChangeSetRequestRequestTypeDef,
@@ -352,25 +352,26 @@
     VmServerAddressTypeDef,
     ImportAppCatalogRequestRequestTypeDef,
     LaunchAppRequestRequestTypeDef,
     ListAppsRequestRequestTypeDef,
     NotificationContextTypeDef,
     ReplicationRunStageDetailsTypeDef,
     ServerReplicationParametersOutputTypeDef,
-    ServerReplicationParametersTypeDef,
     StartAppReplicationRequestRequestTypeDef,
     StartOnDemandAppReplicationRequestRequestTypeDef,
     StartOnDemandReplicationRunRequestRequestTypeDef,
     StopAppReplicationRequestRequestTypeDef,
     TerminateAppRequestRequestTypeDef,
-    UpdateReplicationJobRequestRequestTypeDef,
     AppSummaryTypeDef,
     CreateReplicationJobResponseTypeDef,
     GetConnectorsResponseTypeDef,
     StartOnDemandReplicationRunResponseTypeDef,
+    CreateReplicationJobRequestRequestTypeDef,
+    ServerReplicationParametersTypeDef,
+    UpdateReplicationJobRequestRequestTypeDef,
     GenerateChangeSetResponseTypeDef,
     GenerateTemplateResponseTypeDef,
     SSMOutputTypeDef,
     SourceTypeDef,
     UserDataTypeDef,
     GetConnectorsRequestGetConnectorsPaginateTypeDef,
     GetReplicationJobsRequestGetReplicationJobsPaginateTypeDef,
@@ -397,34 +398,38 @@
     ServerValidationConfigurationTypeDef,
     ServerValidationOutputTypeDef,
     GetReplicationJobsResponseTypeDef,
     GetReplicationRunsResponseTypeDef,
     CreateAppResponseTypeDef,
     GetAppResponseTypeDef,
     UpdateAppResponseTypeDef,
-    CreateAppRequestRequestTypeDef,
-    UpdateAppRequestRequestTypeDef,
+    ServerGroupUnionTypeDef,
     ServerGroupLaunchConfigurationOutputTypeDef,
     ServerGroupLaunchConfigurationTypeDef,
     ServerGroupReplicationConfigurationOutputTypeDef,
     ServerGroupReplicationConfigurationTypeDef,
     ServerGroupValidationConfigurationOutputTypeDef,
     ServerGroupValidationConfigurationTypeDef,
     ValidationOutputTypeDef,
+    CreateAppRequestRequestTypeDef,
+    UpdateAppRequestRequestTypeDef,
     GetAppLaunchConfigurationResponseTypeDef,
-    PutAppLaunchConfigurationRequestRequestTypeDef,
+    ServerGroupLaunchConfigurationUnionTypeDef,
     GetAppReplicationConfigurationResponseTypeDef,
-    PutAppReplicationConfigurationRequestRequestTypeDef,
+    ServerGroupReplicationConfigurationUnionTypeDef,
     GetAppValidationConfigurationResponseTypeDef,
-    PutAppValidationConfigurationRequestRequestTypeDef,
+    ServerGroupValidationConfigurationUnionTypeDef,
     GetAppValidationOutputResponseTypeDef,
+    PutAppLaunchConfigurationRequestRequestTypeDef,
+    PutAppReplicationConfigurationRequestRequestTypeDef,
+    PutAppValidationConfigurationRequestRequestTypeDef,
 )
 
 
-def get_structure() -> LaunchDetailsTypeDef:
+def get_value() -> LaunchDetailsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-sms-1.28.15.post1/mypy_boto3_sms/__init__.py` & `mypy-boto3-sms-1.28.16/mypy_boto3_sms/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sms-1.28.15.post1/mypy_boto3_sms/__init__.pyi` & `mypy-boto3-sms-1.28.16/mypy_boto3_sms/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sms-1.28.15.post1/mypy_boto3_sms/__main__.py` & `mypy-boto3-sms-1.28.16/mypy_boto3_sms/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SMS 1.28.15\nVersion:         1.28.15.post1\nBuilder version:"
-        " 7.16.2\nDocs:           "
+        "Type annotations for boto3.SMS 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS\nOther"
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

### Comparing `mypy-boto3-sms-1.28.15.post1/mypy_boto3_sms/client.py` & `mypy-boto3-sms-1.28.16/mypy_boto3_sms/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from mypy_boto3_sms.client import SMSClient
 
     session = Session()
     client: SMSClient = session.client("sms")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import LicenseTypeType, OutputFormatType
 from .paginator import (
     GetConnectorsPaginator,
     GetReplicationJobsPaginator,
@@ -40,45 +39,39 @@
     GetAppValidationOutputResponseTypeDef,
     GetConnectorsResponseTypeDef,
     GetReplicationJobsResponseTypeDef,
     GetReplicationRunsResponseTypeDef,
     GetServersResponseTypeDef,
     ListAppsResponseTypeDef,
     NotificationContextTypeDef,
-    ServerGroupLaunchConfigurationOutputTypeDef,
-    ServerGroupLaunchConfigurationTypeDef,
-    ServerGroupOutputTypeDef,
-    ServerGroupReplicationConfigurationOutputTypeDef,
-    ServerGroupReplicationConfigurationTypeDef,
-    ServerGroupTypeDef,
-    ServerGroupValidationConfigurationOutputTypeDef,
-    ServerGroupValidationConfigurationTypeDef,
+    ServerGroupLaunchConfigurationUnionTypeDef,
+    ServerGroupReplicationConfigurationUnionTypeDef,
+    ServerGroupUnionTypeDef,
+    ServerGroupValidationConfigurationUnionTypeDef,
     StartOnDemandReplicationRunResponseTypeDef,
     TagTypeDef,
+    TimestampTypeDef,
     UpdateAppResponseTypeDef,
     VmServerAddressTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("SMSClient",)
 
-
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     ClientError: Type[BotocoreClientError]
     DryRunOperationException: Type[BotocoreClientError]
     InternalError: Type[BotocoreClientError]
     InvalidParameterException: Type[BotocoreClientError]
     MissingRequiredParameterException: Type[BotocoreClientError]
     NoConnectorsAvailableException: Type[BotocoreClientError]
@@ -86,15 +79,14 @@
     ReplicationJobAlreadyExistsException: Type[BotocoreClientError]
     ReplicationJobNotFoundException: Type[BotocoreClientError]
     ReplicationRunLimitExceededException: Type[BotocoreClientError]
     ServerCannotBeReplicatedException: Type[BotocoreClientError]
     TemporarilyUnavailableException: Type[BotocoreClientError]
     UnauthorizedOperationException: Type[BotocoreClientError]
 
-
 class SMSClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/client/)
     """
 
     meta: ClientMeta
@@ -103,53 +95,49 @@
     def exceptions(self) -> Exceptions:
         """
         SMSClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/client/#exceptions)
         """
-
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/client/#can_paginate)
         """
-
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/client/#close)
         """
-
     def create_app(
         self,
         *,
         name: str = ...,
         description: str = ...,
         roleName: str = ...,
         clientToken: str = ...,
-        serverGroups: Sequence[Union[ServerGroupTypeDef, ServerGroupOutputTypeDef]] = ...,
+        serverGroups: Sequence[ServerGroupUnionTypeDef] = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateAppResponseTypeDef:
         """
         Creates an application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.create_app)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/client/#create_app)
         """
-
     def create_replication_job(
         self,
         *,
         serverId: str,
-        seedReplicationTime: Union[datetime, str],
+        seedReplicationTime: TimestampTypeDef,
         frequency: int = ...,
         runOnce: bool = ...,
         licenseType: LicenseTypeType = ...,
         roleName: str = ...,
         description: str = ...,
         numberOfRecentAmisToKeep: int = ...,
         encrypted: bool = ...,
@@ -157,420 +145,371 @@
     ) -> CreateReplicationJobResponseTypeDef:
         """
         Creates a replication job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.create_replication_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/client/#create_replication_job)
         """
-
     def delete_app(
         self,
         *,
         appId: str = ...,
         forceStopAppReplication: bool = ...,
         forceTerminateApp: bool = ...
     ) -> Dict[str, Any]:
         """
         Deletes the specified application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.delete_app)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/client/#delete_app)
         """
-
     def delete_app_launch_configuration(self, *, appId: str = ...) -> Dict[str, Any]:
         """
         Deletes the launch configuration for the specified application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.delete_app_launch_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/client/#delete_app_launch_configuration)
         """
-
     def delete_app_replication_configuration(self, *, appId: str = ...) -> Dict[str, Any]:
         """
         Deletes the replication configuration for the specified application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.delete_app_replication_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/client/#delete_app_replication_configuration)
         """
-
     def delete_app_validation_configuration(self, *, appId: str) -> Dict[str, Any]:
         """
         Deletes the validation configuration for the specified application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.delete_app_validation_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/client/#delete_app_validation_configuration)
         """
-
     def delete_replication_job(self, *, replicationJobId: str) -> Dict[str, Any]:
         """
         Deletes the specified replication job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.delete_replication_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/client/#delete_replication_job)
         """
-
     def delete_server_catalog(self) -> Dict[str, Any]:
         """
         Deletes all servers from your server catalog.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.delete_server_catalog)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/client/#delete_server_catalog)
         """
-
     def disassociate_connector(self, *, connectorId: str) -> Dict[str, Any]:
         """
         Disassociates the specified connector from Server Migration Service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.disassociate_connector)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/client/#disassociate_connector)
         """
-
     def generate_change_set(
         self, *, appId: str = ..., changesetFormat: OutputFormatType = ...
     ) -> GenerateChangeSetResponseTypeDef:
         """
         Generates a target change set for a currently launched stack and writes it to an
         Amazon S3 object in the customer’s Amazon S3 bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.generate_change_set)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/client/#generate_change_set)
         """
-
     def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/client/#generate_presigned_url)
         """
-
     def generate_template(
         self, *, appId: str = ..., templateFormat: OutputFormatType = ...
     ) -> GenerateTemplateResponseTypeDef:
         """
         Generates an CloudFormation template based on the current launch configuration
         and writes it to an Amazon S3 object in the customer’s Amazon S3 bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.generate_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/client/#generate_template)
         """
-
     def get_app(self, *, appId: str = ...) -> GetAppResponseTypeDef:
         """
         Retrieve information about the specified application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.get_app)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/client/#get_app)
         """
-
     def get_app_launch_configuration(
         self, *, appId: str = ...
     ) -> GetAppLaunchConfigurationResponseTypeDef:
         """
         Retrieves the application launch configuration associated with the specified
         application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.get_app_launch_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/client/#get_app_launch_configuration)
         """
-
     def get_app_replication_configuration(
         self, *, appId: str = ...
     ) -> GetAppReplicationConfigurationResponseTypeDef:
         """
         Retrieves the application replication configuration associated with the
         specified application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.get_app_replication_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/client/#get_app_replication_configuration)
         """
-
     def get_app_validation_configuration(
         self, *, appId: str
     ) -> GetAppValidationConfigurationResponseTypeDef:
         """
         Retrieves information about a configuration for validating an application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.get_app_validation_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/client/#get_app_validation_configuration)
         """
-
     def get_app_validation_output(self, *, appId: str) -> GetAppValidationOutputResponseTypeDef:
         """
         Retrieves output from validating an application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.get_app_validation_output)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/client/#get_app_validation_output)
         """
-
     def get_connectors(
         self, *, nextToken: str = ..., maxResults: int = ...
     ) -> GetConnectorsResponseTypeDef:
         """
         Describes the connectors registered with the Server Migration Service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.get_connectors)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/client/#get_connectors)
         """
-
     def get_replication_jobs(
         self, *, replicationJobId: str = ..., nextToken: str = ..., maxResults: int = ...
     ) -> GetReplicationJobsResponseTypeDef:
         """
         Describes the specified replication job or all of your replication jobs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.get_replication_jobs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/client/#get_replication_jobs)
         """
-
     def get_replication_runs(
         self, *, replicationJobId: str, nextToken: str = ..., maxResults: int = ...
     ) -> GetReplicationRunsResponseTypeDef:
         """
         Describes the replication runs for the specified replication job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.get_replication_runs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/client/#get_replication_runs)
         """
-
     def get_servers(
         self,
         *,
         nextToken: str = ...,
         maxResults: int = ...,
         vmServerAddressList: Sequence[VmServerAddressTypeDef] = ...
     ) -> GetServersResponseTypeDef:
         """
         Describes the servers in your server catalog.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.get_servers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/client/#get_servers)
         """
-
     def import_app_catalog(self, *, roleName: str = ...) -> Dict[str, Any]:
         """
         Allows application import from Migration Hub.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.import_app_catalog)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/client/#import_app_catalog)
         """
-
     def import_server_catalog(self) -> Dict[str, Any]:
         """
         Gathers a complete list of on-premises servers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.import_server_catalog)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/client/#import_server_catalog)
         """
-
     def launch_app(self, *, appId: str = ...) -> Dict[str, Any]:
         """
         Launches the specified application as a stack in CloudFormation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.launch_app)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/client/#launch_app)
         """
-
     def list_apps(
         self, *, appIds: Sequence[str] = ..., nextToken: str = ..., maxResults: int = ...
     ) -> ListAppsResponseTypeDef:
         """
         Retrieves summaries for all applications.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.list_apps)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/client/#list_apps)
         """
-
     def notify_app_validation_output(
         self, *, appId: str, notificationContext: NotificationContextTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Provides information to Server Migration Service about whether application
         validation is successful.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.notify_app_validation_output)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/client/#notify_app_validation_output)
         """
-
     def put_app_launch_configuration(
         self,
         *,
         appId: str = ...,
         roleName: str = ...,
         autoLaunch: bool = ...,
-        serverGroupLaunchConfigurations: Sequence[
-            Union[
-                ServerGroupLaunchConfigurationTypeDef, ServerGroupLaunchConfigurationOutputTypeDef
-            ]
-        ] = ...
+        serverGroupLaunchConfigurations: Sequence[ServerGroupLaunchConfigurationUnionTypeDef] = ...
     ) -> Dict[str, Any]:
         """
         Creates or updates the launch configuration for the specified application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.put_app_launch_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/client/#put_app_launch_configuration)
         """
-
     def put_app_replication_configuration(
         self,
         *,
         appId: str = ...,
         serverGroupReplicationConfigurations: Sequence[
-            Union[
-                ServerGroupReplicationConfigurationTypeDef,
-                ServerGroupReplicationConfigurationOutputTypeDef,
-            ]
+            ServerGroupReplicationConfigurationUnionTypeDef
         ] = ...
     ) -> Dict[str, Any]:
         """
         Creates or updates the replication configuration for the specified application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.put_app_replication_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/client/#put_app_replication_configuration)
         """
-
     def put_app_validation_configuration(
         self,
         *,
         appId: str,
         appValidationConfigurations: Sequence[AppValidationConfigurationTypeDef] = ...,
         serverGroupValidationConfigurations: Sequence[
-            Union[
-                ServerGroupValidationConfigurationTypeDef,
-                ServerGroupValidationConfigurationOutputTypeDef,
-            ]
+            ServerGroupValidationConfigurationUnionTypeDef
         ] = ...
     ) -> Dict[str, Any]:
         """
         Creates or updates a validation configuration for the specified application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.put_app_validation_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/client/#put_app_validation_configuration)
         """
-
     def start_app_replication(self, *, appId: str = ...) -> Dict[str, Any]:
         """
         Starts replicating the specified application by creating replication jobs for
         each server in the application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.start_app_replication)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/client/#start_app_replication)
         """
-
     def start_on_demand_app_replication(
         self, *, appId: str, description: str = ...
     ) -> Dict[str, Any]:
         """
         Starts an on-demand replication run for the specified application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.start_on_demand_app_replication)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/client/#start_on_demand_app_replication)
         """
-
     def start_on_demand_replication_run(
         self, *, replicationJobId: str, description: str = ...
     ) -> StartOnDemandReplicationRunResponseTypeDef:
         """
         Starts an on-demand replication run for the specified replication job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.start_on_demand_replication_run)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/client/#start_on_demand_replication_run)
         """
-
     def stop_app_replication(self, *, appId: str = ...) -> Dict[str, Any]:
         """
         Stops replicating the specified application by deleting the replication job for
         each server in the application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.stop_app_replication)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/client/#stop_app_replication)
         """
-
     def terminate_app(self, *, appId: str = ...) -> Dict[str, Any]:
         """
         Terminates the stack for the specified application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.terminate_app)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/client/#terminate_app)
         """
-
     def update_app(
         self,
         *,
         appId: str = ...,
         name: str = ...,
         description: str = ...,
         roleName: str = ...,
-        serverGroups: Sequence[Union[ServerGroupTypeDef, ServerGroupOutputTypeDef]] = ...,
+        serverGroups: Sequence[ServerGroupUnionTypeDef] = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> UpdateAppResponseTypeDef:
         """
         Updates the specified application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.update_app)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/client/#update_app)
         """
-
     def update_replication_job(
         self,
         *,
         replicationJobId: str,
         frequency: int = ...,
-        nextReplicationRunStartTime: Union[datetime, str] = ...,
+        nextReplicationRunStartTime: TimestampTypeDef = ...,
         licenseType: LicenseTypeType = ...,
         roleName: str = ...,
         description: str = ...,
         numberOfRecentAmisToKeep: int = ...,
         encrypted: bool = ...,
         kmsKeyId: str = ...
     ) -> Dict[str, Any]:
         """
         Updates the specified settings for the specified replication job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.update_replication_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/client/#update_replication_job)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["get_connectors"]) -> GetConnectorsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["get_replication_jobs"]
     ) -> GetReplicationJobsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["get_replication_runs"]
     ) -> GetReplicationRunsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["get_servers"]) -> GetServersPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["list_apps"]) -> ListAppsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/client/#get_paginator)
         """
```

### Comparing `mypy-boto3-sms-1.28.15.post1/mypy_boto3_sms/client.pyi` & `mypy-boto3-sms-1.28.16/mypy_boto3_sms/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from mypy_boto3_sms.client import SMSClient
 
     session = Session()
     client: SMSClient = session.client("sms")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import LicenseTypeType, OutputFormatType
 from .paginator import (
     GetConnectorsPaginator,
     GetReplicationJobsPaginator,
@@ -40,42 +39,42 @@
     GetAppValidationOutputResponseTypeDef,
     GetConnectorsResponseTypeDef,
     GetReplicationJobsResponseTypeDef,
     GetReplicationRunsResponseTypeDef,
     GetServersResponseTypeDef,
     ListAppsResponseTypeDef,
     NotificationContextTypeDef,
-    ServerGroupLaunchConfigurationOutputTypeDef,
-    ServerGroupLaunchConfigurationTypeDef,
-    ServerGroupOutputTypeDef,
-    ServerGroupReplicationConfigurationOutputTypeDef,
-    ServerGroupReplicationConfigurationTypeDef,
-    ServerGroupTypeDef,
-    ServerGroupValidationConfigurationOutputTypeDef,
-    ServerGroupValidationConfigurationTypeDef,
+    ServerGroupLaunchConfigurationUnionTypeDef,
+    ServerGroupReplicationConfigurationUnionTypeDef,
+    ServerGroupUnionTypeDef,
+    ServerGroupValidationConfigurationUnionTypeDef,
     StartOnDemandReplicationRunResponseTypeDef,
     TagTypeDef,
+    TimestampTypeDef,
     UpdateAppResponseTypeDef,
     VmServerAddressTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = ("SMSClient",)
 
+
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     ClientError: Type[BotocoreClientError]
     DryRunOperationException: Type[BotocoreClientError]
     InternalError: Type[BotocoreClientError]
     InvalidParameterException: Type[BotocoreClientError]
     MissingRequiredParameterException: Type[BotocoreClientError]
     NoConnectorsAvailableException: Type[BotocoreClientError]
@@ -83,14 +82,15 @@
     ReplicationJobAlreadyExistsException: Type[BotocoreClientError]
     ReplicationJobNotFoundException: Type[BotocoreClientError]
     ReplicationRunLimitExceededException: Type[BotocoreClientError]
     ServerCannotBeReplicatedException: Type[BotocoreClientError]
     TemporarilyUnavailableException: Type[BotocoreClientError]
     UnauthorizedOperationException: Type[BotocoreClientError]
 
+
 class SMSClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/client/)
     """
 
     meta: ClientMeta
@@ -99,49 +99,53 @@
     def exceptions(self) -> Exceptions:
         """
         SMSClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/client/#exceptions)
         """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/client/#can_paginate)
         """
+
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/client/#close)
         """
+
     def create_app(
         self,
         *,
         name: str = ...,
         description: str = ...,
         roleName: str = ...,
         clientToken: str = ...,
-        serverGroups: Sequence[Union[ServerGroupTypeDef, ServerGroupOutputTypeDef]] = ...,
+        serverGroups: Sequence[ServerGroupUnionTypeDef] = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateAppResponseTypeDef:
         """
         Creates an application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.create_app)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/client/#create_app)
         """
+
     def create_replication_job(
         self,
         *,
         serverId: str,
-        seedReplicationTime: Union[datetime, str],
+        seedReplicationTime: TimestampTypeDef,
         frequency: int = ...,
         runOnce: bool = ...,
         licenseType: LicenseTypeType = ...,
         roleName: str = ...,
         description: str = ...,
         numberOfRecentAmisToKeep: int = ...,
         encrypted: bool = ...,
@@ -149,381 +153,410 @@
     ) -> CreateReplicationJobResponseTypeDef:
         """
         Creates a replication job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.create_replication_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/client/#create_replication_job)
         """
+
     def delete_app(
         self,
         *,
         appId: str = ...,
         forceStopAppReplication: bool = ...,
         forceTerminateApp: bool = ...
     ) -> Dict[str, Any]:
         """
         Deletes the specified application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.delete_app)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/client/#delete_app)
         """
+
     def delete_app_launch_configuration(self, *, appId: str = ...) -> Dict[str, Any]:
         """
         Deletes the launch configuration for the specified application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.delete_app_launch_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/client/#delete_app_launch_configuration)
         """
+
     def delete_app_replication_configuration(self, *, appId: str = ...) -> Dict[str, Any]:
         """
         Deletes the replication configuration for the specified application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.delete_app_replication_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/client/#delete_app_replication_configuration)
         """
+
     def delete_app_validation_configuration(self, *, appId: str) -> Dict[str, Any]:
         """
         Deletes the validation configuration for the specified application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.delete_app_validation_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/client/#delete_app_validation_configuration)
         """
+
     def delete_replication_job(self, *, replicationJobId: str) -> Dict[str, Any]:
         """
         Deletes the specified replication job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.delete_replication_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/client/#delete_replication_job)
         """
+
     def delete_server_catalog(self) -> Dict[str, Any]:
         """
         Deletes all servers from your server catalog.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.delete_server_catalog)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/client/#delete_server_catalog)
         """
+
     def disassociate_connector(self, *, connectorId: str) -> Dict[str, Any]:
         """
         Disassociates the specified connector from Server Migration Service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.disassociate_connector)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/client/#disassociate_connector)
         """
+
     def generate_change_set(
         self, *, appId: str = ..., changesetFormat: OutputFormatType = ...
     ) -> GenerateChangeSetResponseTypeDef:
         """
         Generates a target change set for a currently launched stack and writes it to an
         Amazon S3 object in the customer’s Amazon S3 bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.generate_change_set)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/client/#generate_change_set)
         """
+
     def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/client/#generate_presigned_url)
         """
+
     def generate_template(
         self, *, appId: str = ..., templateFormat: OutputFormatType = ...
     ) -> GenerateTemplateResponseTypeDef:
         """
         Generates an CloudFormation template based on the current launch configuration
         and writes it to an Amazon S3 object in the customer’s Amazon S3 bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.generate_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/client/#generate_template)
         """
+
     def get_app(self, *, appId: str = ...) -> GetAppResponseTypeDef:
         """
         Retrieve information about the specified application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.get_app)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/client/#get_app)
         """
+
     def get_app_launch_configuration(
         self, *, appId: str = ...
     ) -> GetAppLaunchConfigurationResponseTypeDef:
         """
         Retrieves the application launch configuration associated with the specified
         application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.get_app_launch_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/client/#get_app_launch_configuration)
         """
+
     def get_app_replication_configuration(
         self, *, appId: str = ...
     ) -> GetAppReplicationConfigurationResponseTypeDef:
         """
         Retrieves the application replication configuration associated with the
         specified application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.get_app_replication_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/client/#get_app_replication_configuration)
         """
+
     def get_app_validation_configuration(
         self, *, appId: str
     ) -> GetAppValidationConfigurationResponseTypeDef:
         """
         Retrieves information about a configuration for validating an application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.get_app_validation_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/client/#get_app_validation_configuration)
         """
+
     def get_app_validation_output(self, *, appId: str) -> GetAppValidationOutputResponseTypeDef:
         """
         Retrieves output from validating an application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.get_app_validation_output)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/client/#get_app_validation_output)
         """
+
     def get_connectors(
         self, *, nextToken: str = ..., maxResults: int = ...
     ) -> GetConnectorsResponseTypeDef:
         """
         Describes the connectors registered with the Server Migration Service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.get_connectors)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/client/#get_connectors)
         """
+
     def get_replication_jobs(
         self, *, replicationJobId: str = ..., nextToken: str = ..., maxResults: int = ...
     ) -> GetReplicationJobsResponseTypeDef:
         """
         Describes the specified replication job or all of your replication jobs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.get_replication_jobs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/client/#get_replication_jobs)
         """
+
     def get_replication_runs(
         self, *, replicationJobId: str, nextToken: str = ..., maxResults: int = ...
     ) -> GetReplicationRunsResponseTypeDef:
         """
         Describes the replication runs for the specified replication job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.get_replication_runs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/client/#get_replication_runs)
         """
+
     def get_servers(
         self,
         *,
         nextToken: str = ...,
         maxResults: int = ...,
         vmServerAddressList: Sequence[VmServerAddressTypeDef] = ...
     ) -> GetServersResponseTypeDef:
         """
         Describes the servers in your server catalog.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.get_servers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/client/#get_servers)
         """
+
     def import_app_catalog(self, *, roleName: str = ...) -> Dict[str, Any]:
         """
         Allows application import from Migration Hub.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.import_app_catalog)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/client/#import_app_catalog)
         """
+
     def import_server_catalog(self) -> Dict[str, Any]:
         """
         Gathers a complete list of on-premises servers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.import_server_catalog)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/client/#import_server_catalog)
         """
+
     def launch_app(self, *, appId: str = ...) -> Dict[str, Any]:
         """
         Launches the specified application as a stack in CloudFormation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.launch_app)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/client/#launch_app)
         """
+
     def list_apps(
         self, *, appIds: Sequence[str] = ..., nextToken: str = ..., maxResults: int = ...
     ) -> ListAppsResponseTypeDef:
         """
         Retrieves summaries for all applications.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.list_apps)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/client/#list_apps)
         """
+
     def notify_app_validation_output(
         self, *, appId: str, notificationContext: NotificationContextTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Provides information to Server Migration Service about whether application
         validation is successful.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.notify_app_validation_output)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/client/#notify_app_validation_output)
         """
+
     def put_app_launch_configuration(
         self,
         *,
         appId: str = ...,
         roleName: str = ...,
         autoLaunch: bool = ...,
-        serverGroupLaunchConfigurations: Sequence[
-            Union[
-                ServerGroupLaunchConfigurationTypeDef, ServerGroupLaunchConfigurationOutputTypeDef
-            ]
-        ] = ...
+        serverGroupLaunchConfigurations: Sequence[ServerGroupLaunchConfigurationUnionTypeDef] = ...
     ) -> Dict[str, Any]:
         """
         Creates or updates the launch configuration for the specified application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.put_app_launch_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/client/#put_app_launch_configuration)
         """
+
     def put_app_replication_configuration(
         self,
         *,
         appId: str = ...,
         serverGroupReplicationConfigurations: Sequence[
-            Union[
-                ServerGroupReplicationConfigurationTypeDef,
-                ServerGroupReplicationConfigurationOutputTypeDef,
-            ]
+            ServerGroupReplicationConfigurationUnionTypeDef
         ] = ...
     ) -> Dict[str, Any]:
         """
         Creates or updates the replication configuration for the specified application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.put_app_replication_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/client/#put_app_replication_configuration)
         """
+
     def put_app_validation_configuration(
         self,
         *,
         appId: str,
         appValidationConfigurations: Sequence[AppValidationConfigurationTypeDef] = ...,
         serverGroupValidationConfigurations: Sequence[
-            Union[
-                ServerGroupValidationConfigurationTypeDef,
-                ServerGroupValidationConfigurationOutputTypeDef,
-            ]
+            ServerGroupValidationConfigurationUnionTypeDef
         ] = ...
     ) -> Dict[str, Any]:
         """
         Creates or updates a validation configuration for the specified application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.put_app_validation_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/client/#put_app_validation_configuration)
         """
+
     def start_app_replication(self, *, appId: str = ...) -> Dict[str, Any]:
         """
         Starts replicating the specified application by creating replication jobs for
         each server in the application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.start_app_replication)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/client/#start_app_replication)
         """
+
     def start_on_demand_app_replication(
         self, *, appId: str, description: str = ...
     ) -> Dict[str, Any]:
         """
         Starts an on-demand replication run for the specified application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.start_on_demand_app_replication)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/client/#start_on_demand_app_replication)
         """
+
     def start_on_demand_replication_run(
         self, *, replicationJobId: str, description: str = ...
     ) -> StartOnDemandReplicationRunResponseTypeDef:
         """
         Starts an on-demand replication run for the specified replication job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.start_on_demand_replication_run)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/client/#start_on_demand_replication_run)
         """
+
     def stop_app_replication(self, *, appId: str = ...) -> Dict[str, Any]:
         """
         Stops replicating the specified application by deleting the replication job for
         each server in the application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.stop_app_replication)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/client/#stop_app_replication)
         """
+
     def terminate_app(self, *, appId: str = ...) -> Dict[str, Any]:
         """
         Terminates the stack for the specified application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.terminate_app)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/client/#terminate_app)
         """
+
     def update_app(
         self,
         *,
         appId: str = ...,
         name: str = ...,
         description: str = ...,
         roleName: str = ...,
-        serverGroups: Sequence[Union[ServerGroupTypeDef, ServerGroupOutputTypeDef]] = ...,
+        serverGroups: Sequence[ServerGroupUnionTypeDef] = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> UpdateAppResponseTypeDef:
         """
         Updates the specified application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.update_app)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/client/#update_app)
         """
+
     def update_replication_job(
         self,
         *,
         replicationJobId: str,
         frequency: int = ...,
-        nextReplicationRunStartTime: Union[datetime, str] = ...,
+        nextReplicationRunStartTime: TimestampTypeDef = ...,
         licenseType: LicenseTypeType = ...,
         roleName: str = ...,
         description: str = ...,
         numberOfRecentAmisToKeep: int = ...,
         encrypted: bool = ...,
         kmsKeyId: str = ...
     ) -> Dict[str, Any]:
         """
         Updates the specified settings for the specified replication job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.update_replication_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/client/#update_replication_job)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["get_connectors"]) -> GetConnectorsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["get_replication_jobs"]
     ) -> GetReplicationJobsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["get_replication_runs"]
     ) -> GetReplicationRunsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["get_servers"]) -> GetServersPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["list_apps"]) -> ListAppsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/client/#get_paginator)
         """
```

### Comparing `mypy-boto3-sms-1.28.15.post1/mypy_boto3_sms/literals.py` & `mypy-boto3-sms-1.28.16/mypy_boto3_sms/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sms-1.28.15.post1/mypy_boto3_sms/literals.pyi` & `mypy-boto3-sms-1.28.16/mypy_boto3_sms/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sms-1.28.15.post1/mypy_boto3_sms/paginator.py` & `mypy-boto3-sms-1.28.16/mypy_boto3_sms/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sms-1.28.15.post1/mypy_boto3_sms/paginator.pyi` & `mypy-boto3-sms-1.28.16/mypy_boto3_sms/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sms-1.28.15.post1/mypy_boto3_sms/type_defs.py` & `mypy-boto3-sms-1.28.16/mypy_boto3_sms/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_sms.type_defs import LaunchDetailsTypeDef
 
-    data: LaunchDetailsTypeDef = {...}
+    data: LaunchDetailsTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -39,21 +39,20 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "LaunchDetailsTypeDef",
     "ConnectorTypeDef",
     "TagTypeDef",
     "ResponseMetadataTypeDef",
-    "CreateReplicationJobRequestRequestTypeDef",
+    "TimestampTypeDef",
     "DeleteAppLaunchConfigurationRequestRequestTypeDef",
     "DeleteAppReplicationConfigurationRequestRequestTypeDef",
     "DeleteAppRequestRequestTypeDef",
     "DeleteAppValidationConfigurationRequestRequestTypeDef",
     "DeleteReplicationJobRequestRequestTypeDef",
     "DisassociateConnectorRequestRequestTypeDef",
     "GenerateChangeSetRequestRequestTypeDef",
@@ -71,25 +70,26 @@
     "VmServerAddressTypeDef",
     "ImportAppCatalogRequestRequestTypeDef",
     "LaunchAppRequestRequestTypeDef",
     "ListAppsRequestRequestTypeDef",
     "NotificationContextTypeDef",
     "ReplicationRunStageDetailsTypeDef",
     "ServerReplicationParametersOutputTypeDef",
-    "ServerReplicationParametersTypeDef",
     "StartAppReplicationRequestRequestTypeDef",
     "StartOnDemandAppReplicationRequestRequestTypeDef",
     "StartOnDemandReplicationRunRequestRequestTypeDef",
     "StopAppReplicationRequestRequestTypeDef",
     "TerminateAppRequestRequestTypeDef",
-    "UpdateReplicationJobRequestRequestTypeDef",
     "AppSummaryTypeDef",
     "CreateReplicationJobResponseTypeDef",
     "GetConnectorsResponseTypeDef",
     "StartOnDemandReplicationRunResponseTypeDef",
+    "CreateReplicationJobRequestRequestTypeDef",
+    "ServerReplicationParametersTypeDef",
+    "UpdateReplicationJobRequestRequestTypeDef",
     "GenerateChangeSetResponseTypeDef",
     "GenerateTemplateResponseTypeDef",
     "SSMOutputTypeDef",
     "SourceTypeDef",
     "UserDataTypeDef",
     "GetConnectorsRequestGetConnectorsPaginateTypeDef",
     "GetReplicationJobsRequestGetReplicationJobsPaginateTypeDef",
@@ -116,30 +116,34 @@
     "ServerValidationConfigurationTypeDef",
     "ServerValidationOutputTypeDef",
     "GetReplicationJobsResponseTypeDef",
     "GetReplicationRunsResponseTypeDef",
     "CreateAppResponseTypeDef",
     "GetAppResponseTypeDef",
     "UpdateAppResponseTypeDef",
-    "CreateAppRequestRequestTypeDef",
-    "UpdateAppRequestRequestTypeDef",
+    "ServerGroupUnionTypeDef",
     "ServerGroupLaunchConfigurationOutputTypeDef",
     "ServerGroupLaunchConfigurationTypeDef",
     "ServerGroupReplicationConfigurationOutputTypeDef",
     "ServerGroupReplicationConfigurationTypeDef",
     "ServerGroupValidationConfigurationOutputTypeDef",
     "ServerGroupValidationConfigurationTypeDef",
     "ValidationOutputTypeDef",
+    "CreateAppRequestRequestTypeDef",
+    "UpdateAppRequestRequestTypeDef",
     "GetAppLaunchConfigurationResponseTypeDef",
-    "PutAppLaunchConfigurationRequestRequestTypeDef",
+    "ServerGroupLaunchConfigurationUnionTypeDef",
     "GetAppReplicationConfigurationResponseTypeDef",
-    "PutAppReplicationConfigurationRequestRequestTypeDef",
+    "ServerGroupReplicationConfigurationUnionTypeDef",
     "GetAppValidationConfigurationResponseTypeDef",
-    "PutAppValidationConfigurationRequestRequestTypeDef",
+    "ServerGroupValidationConfigurationUnionTypeDef",
     "GetAppValidationOutputResponseTypeDef",
+    "PutAppLaunchConfigurationRequestRequestTypeDef",
+    "PutAppReplicationConfigurationRequestRequestTypeDef",
+    "PutAppValidationConfigurationRequestRequestTypeDef",
 )
 
 LaunchDetailsTypeDef = TypedDict(
     "LaunchDetailsTypeDef",
     {
         "latestLaunchTime": datetime,
         "stackName": str,
@@ -181,44 +185,15 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
-_RequiredCreateReplicationJobRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateReplicationJobRequestRequestTypeDef",
-    {
-        "serverId": str,
-        "seedReplicationTime": Union[datetime, str],
-    },
-)
-_OptionalCreateReplicationJobRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateReplicationJobRequestRequestTypeDef",
-    {
-        "frequency": int,
-        "runOnce": bool,
-        "licenseType": LicenseTypeType,
-        "roleName": str,
-        "description": str,
-        "numberOfRecentAmisToKeep": int,
-        "encrypted": bool,
-        "kmsKeyId": str,
-    },
-    total=False,
-)
-
-
-class CreateReplicationJobRequestRequestTypeDef(
-    _RequiredCreateReplicationJobRequestRequestTypeDef,
-    _OptionalCreateReplicationJobRequestRequestTypeDef,
-):
-    pass
-
-
+TimestampTypeDef = Union[datetime, str]
 DeleteAppLaunchConfigurationRequestRequestTypeDef = TypedDict(
     "DeleteAppLaunchConfigurationRequestRequestTypeDef",
     {
         "appId": str,
     },
     total=False,
 )
@@ -367,22 +342,20 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class GetReplicationRunsRequestRequestTypeDef(
     _RequiredGetReplicationRunsRequestRequestTypeDef,
     _OptionalGetReplicationRunsRequestRequestTypeDef,
 ):
     pass
 
-
 VmServerAddressTypeDef = TypedDict(
     "VmServerAddressTypeDef",
     {
         "vmManagerId": str,
         "vmId": str,
     },
     total=False,
@@ -443,28 +416,14 @@
         "numberOfRecentAmisToKeep": int,
         "encrypted": bool,
         "kmsKeyId": str,
     },
     total=False,
 )
 
-ServerReplicationParametersTypeDef = TypedDict(
-    "ServerReplicationParametersTypeDef",
-    {
-        "seedTime": Union[datetime, str],
-        "frequency": int,
-        "runOnce": bool,
-        "licenseType": LicenseTypeType,
-        "numberOfRecentAmisToKeep": int,
-        "encrypted": bool,
-        "kmsKeyId": str,
-    },
-    total=False,
-)
-
 StartAppReplicationRequestRequestTypeDef = TypedDict(
     "StartAppReplicationRequestRequestTypeDef",
     {
         "appId": str,
     },
     total=False,
 )
@@ -479,44 +438,40 @@
     "_OptionalStartOnDemandAppReplicationRequestRequestTypeDef",
     {
         "description": str,
     },
     total=False,
 )
 
-
 class StartOnDemandAppReplicationRequestRequestTypeDef(
     _RequiredStartOnDemandAppReplicationRequestRequestTypeDef,
     _OptionalStartOnDemandAppReplicationRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredStartOnDemandReplicationRunRequestRequestTypeDef = TypedDict(
     "_RequiredStartOnDemandReplicationRunRequestRequestTypeDef",
     {
         "replicationJobId": str,
     },
 )
 _OptionalStartOnDemandReplicationRunRequestRequestTypeDef = TypedDict(
     "_OptionalStartOnDemandReplicationRunRequestRequestTypeDef",
     {
         "description": str,
     },
     total=False,
 )
 
-
 class StartOnDemandReplicationRunRequestRequestTypeDef(
     _RequiredStartOnDemandReplicationRunRequestRequestTypeDef,
     _OptionalStartOnDemandReplicationRunRequestRequestTypeDef,
 ):
     pass
 
-
 StopAppReplicationRequestRequestTypeDef = TypedDict(
     "StopAppReplicationRequestRequestTypeDef",
     {
         "appId": str,
     },
     total=False,
 )
@@ -525,43 +480,14 @@
     "TerminateAppRequestRequestTypeDef",
     {
         "appId": str,
     },
     total=False,
 )
 
-_RequiredUpdateReplicationJobRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateReplicationJobRequestRequestTypeDef",
-    {
-        "replicationJobId": str,
-    },
-)
-_OptionalUpdateReplicationJobRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateReplicationJobRequestRequestTypeDef",
-    {
-        "frequency": int,
-        "nextReplicationRunStartTime": Union[datetime, str],
-        "licenseType": LicenseTypeType,
-        "roleName": str,
-        "description": str,
-        "numberOfRecentAmisToKeep": int,
-        "encrypted": bool,
-        "kmsKeyId": str,
-    },
-    total=False,
-)
-
-
-class UpdateReplicationJobRequestRequestTypeDef(
-    _RequiredUpdateReplicationJobRequestRequestTypeDef,
-    _OptionalUpdateReplicationJobRequestRequestTypeDef,
-):
-    pass
-
-
 AppSummaryTypeDef = TypedDict(
     "AppSummaryTypeDef",
     {
         "appId": str,
         "importedAppId": str,
         "name": str,
         "description": str,
@@ -605,14 +531,83 @@
     "StartOnDemandReplicationRunResponseTypeDef",
     {
         "replicationRunId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredCreateReplicationJobRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateReplicationJobRequestRequestTypeDef",
+    {
+        "serverId": str,
+        "seedReplicationTime": TimestampTypeDef,
+    },
+)
+_OptionalCreateReplicationJobRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateReplicationJobRequestRequestTypeDef",
+    {
+        "frequency": int,
+        "runOnce": bool,
+        "licenseType": LicenseTypeType,
+        "roleName": str,
+        "description": str,
+        "numberOfRecentAmisToKeep": int,
+        "encrypted": bool,
+        "kmsKeyId": str,
+    },
+    total=False,
+)
+
+class CreateReplicationJobRequestRequestTypeDef(
+    _RequiredCreateReplicationJobRequestRequestTypeDef,
+    _OptionalCreateReplicationJobRequestRequestTypeDef,
+):
+    pass
+
+ServerReplicationParametersTypeDef = TypedDict(
+    "ServerReplicationParametersTypeDef",
+    {
+        "seedTime": TimestampTypeDef,
+        "frequency": int,
+        "runOnce": bool,
+        "licenseType": LicenseTypeType,
+        "numberOfRecentAmisToKeep": int,
+        "encrypted": bool,
+        "kmsKeyId": str,
+    },
+    total=False,
+)
+
+_RequiredUpdateReplicationJobRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateReplicationJobRequestRequestTypeDef",
+    {
+        "replicationJobId": str,
+    },
+)
+_OptionalUpdateReplicationJobRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateReplicationJobRequestRequestTypeDef",
+    {
+        "frequency": int,
+        "nextReplicationRunStartTime": TimestampTypeDef,
+        "licenseType": LicenseTypeType,
+        "roleName": str,
+        "description": str,
+        "numberOfRecentAmisToKeep": int,
+        "encrypted": bool,
+        "kmsKeyId": str,
+    },
+    total=False,
+)
+
+class UpdateReplicationJobRequestRequestTypeDef(
+    _RequiredUpdateReplicationJobRequestRequestTypeDef,
+    _OptionalUpdateReplicationJobRequestRequestTypeDef,
+):
+    pass
+
 GenerateChangeSetResponseTypeDef = TypedDict(
     "GenerateChangeSetResponseTypeDef",
     {
         "s3Location": S3LocationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -676,22 +671,20 @@
     "_OptionalGetReplicationRunsRequestGetReplicationRunsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetReplicationRunsRequestGetReplicationRunsPaginateTypeDef(
     _RequiredGetReplicationRunsRequestGetReplicationRunsPaginateTypeDef,
     _OptionalGetReplicationRunsRequestGetReplicationRunsPaginateTypeDef,
 ):
     pass
 
-
 ListAppsRequestListAppsPaginateTypeDef = TypedDict(
     "ListAppsRequestListAppsPaginateTypeDef",
     {
         "appIds": Sequence[str],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -738,22 +731,20 @@
     "_OptionalNotifyAppValidationOutputRequestRequestTypeDef",
     {
         "notificationContext": NotificationContextTypeDef,
     },
     total=False,
 )
 
-
 class NotifyAppValidationOutputRequestRequestTypeDef(
     _RequiredNotifyAppValidationOutputRequestRequestTypeDef,
     _OptionalNotifyAppValidationOutputRequestRequestTypeDef,
 ):
     pass
 
-
 ReplicationRunTypeDef = TypedDict(
     "ReplicationRunTypeDef",
     {
         "replicationRunId": str,
         "state": ReplicationRunStateType,
         "type": ReplicationRunTypeType,
         "stageDetails": ReplicationRunStageDetailsTypeDef,
@@ -988,40 +979,15 @@
         "appSummary": AppSummaryTypeDef,
         "serverGroups": List[ServerGroupOutputTypeDef],
         "tags": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateAppRequestRequestTypeDef = TypedDict(
-    "CreateAppRequestRequestTypeDef",
-    {
-        "name": str,
-        "description": str,
-        "roleName": str,
-        "clientToken": str,
-        "serverGroups": Sequence[Union[ServerGroupTypeDef, ServerGroupOutputTypeDef]],
-        "tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-UpdateAppRequestRequestTypeDef = TypedDict(
-    "UpdateAppRequestRequestTypeDef",
-    {
-        "appId": str,
-        "name": str,
-        "description": str,
-        "roleName": str,
-        "serverGroups": Sequence[Union[ServerGroupTypeDef, ServerGroupOutputTypeDef]],
-        "tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
+ServerGroupUnionTypeDef = Union[ServerGroupTypeDef, ServerGroupOutputTypeDef]
 ServerGroupLaunchConfigurationOutputTypeDef = TypedDict(
     "ServerGroupLaunchConfigurationOutputTypeDef",
     {
         "serverGroupId": str,
         "launchOrder": int,
         "serverLaunchConfigurations": List[ServerLaunchConfigurationTypeDef],
     },
@@ -1084,103 +1050,126 @@
         "latestValidationTime": datetime,
         "appValidationOutput": AppValidationOutputTypeDef,
         "serverValidationOutput": ServerValidationOutputTypeDef,
     },
     total=False,
 )
 
-GetAppLaunchConfigurationResponseTypeDef = TypedDict(
-    "GetAppLaunchConfigurationResponseTypeDef",
+CreateAppRequestRequestTypeDef = TypedDict(
+    "CreateAppRequestRequestTypeDef",
+    {
+        "name": str,
+        "description": str,
+        "roleName": str,
+        "clientToken": str,
+        "serverGroups": Sequence[ServerGroupUnionTypeDef],
+        "tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+UpdateAppRequestRequestTypeDef = TypedDict(
+    "UpdateAppRequestRequestTypeDef",
     {
         "appId": str,
+        "name": str,
+        "description": str,
         "roleName": str,
-        "autoLaunch": bool,
-        "serverGroupLaunchConfigurations": List[ServerGroupLaunchConfigurationOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "serverGroups": Sequence[ServerGroupUnionTypeDef],
+        "tags": Sequence[TagTypeDef],
     },
+    total=False,
 )
 
-PutAppLaunchConfigurationRequestRequestTypeDef = TypedDict(
-    "PutAppLaunchConfigurationRequestRequestTypeDef",
+GetAppLaunchConfigurationResponseTypeDef = TypedDict(
+    "GetAppLaunchConfigurationResponseTypeDef",
     {
         "appId": str,
         "roleName": str,
         "autoLaunch": bool,
-        "serverGroupLaunchConfigurations": Sequence[
-            Union[
-                ServerGroupLaunchConfigurationTypeDef, ServerGroupLaunchConfigurationOutputTypeDef
-            ]
-        ],
+        "serverGroupLaunchConfigurations": List[ServerGroupLaunchConfigurationOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
+ServerGroupLaunchConfigurationUnionTypeDef = Union[
+    ServerGroupLaunchConfigurationTypeDef, ServerGroupLaunchConfigurationOutputTypeDef
+]
 GetAppReplicationConfigurationResponseTypeDef = TypedDict(
     "GetAppReplicationConfigurationResponseTypeDef",
     {
         "serverGroupReplicationConfigurations": List[
             ServerGroupReplicationConfigurationOutputTypeDef
         ],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutAppReplicationConfigurationRequestRequestTypeDef = TypedDict(
-    "PutAppReplicationConfigurationRequestRequestTypeDef",
-    {
-        "appId": str,
-        "serverGroupReplicationConfigurations": Sequence[
-            Union[
-                ServerGroupReplicationConfigurationTypeDef,
-                ServerGroupReplicationConfigurationOutputTypeDef,
-            ]
-        ],
-    },
-    total=False,
-)
-
+ServerGroupReplicationConfigurationUnionTypeDef = Union[
+    ServerGroupReplicationConfigurationTypeDef, ServerGroupReplicationConfigurationOutputTypeDef
+]
 GetAppValidationConfigurationResponseTypeDef = TypedDict(
     "GetAppValidationConfigurationResponseTypeDef",
     {
         "appValidationConfigurations": List[AppValidationConfigurationTypeDef],
         "serverGroupValidationConfigurations": List[
             ServerGroupValidationConfigurationOutputTypeDef
         ],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ServerGroupValidationConfigurationUnionTypeDef = Union[
+    ServerGroupValidationConfigurationTypeDef, ServerGroupValidationConfigurationOutputTypeDef
+]
+GetAppValidationOutputResponseTypeDef = TypedDict(
+    "GetAppValidationOutputResponseTypeDef",
+    {
+        "validationOutputList": List[ValidationOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutAppLaunchConfigurationRequestRequestTypeDef = TypedDict(
+    "PutAppLaunchConfigurationRequestRequestTypeDef",
+    {
+        "appId": str,
+        "roleName": str,
+        "autoLaunch": bool,
+        "serverGroupLaunchConfigurations": Sequence[ServerGroupLaunchConfigurationUnionTypeDef],
+    },
+    total=False,
+)
+
+PutAppReplicationConfigurationRequestRequestTypeDef = TypedDict(
+    "PutAppReplicationConfigurationRequestRequestTypeDef",
+    {
+        "appId": str,
+        "serverGroupReplicationConfigurations": Sequence[
+            ServerGroupReplicationConfigurationUnionTypeDef
+        ],
+    },
+    total=False,
+)
+
 _RequiredPutAppValidationConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredPutAppValidationConfigurationRequestRequestTypeDef",
     {
         "appId": str,
     },
 )
 _OptionalPutAppValidationConfigurationRequestRequestTypeDef = TypedDict(
     "_OptionalPutAppValidationConfigurationRequestRequestTypeDef",
     {
         "appValidationConfigurations": Sequence[AppValidationConfigurationTypeDef],
         "serverGroupValidationConfigurations": Sequence[
-            Union[
-                ServerGroupValidationConfigurationTypeDef,
-                ServerGroupValidationConfigurationOutputTypeDef,
-            ]
+            ServerGroupValidationConfigurationUnionTypeDef
         ],
     },
     total=False,
 )
 
-
 class PutAppValidationConfigurationRequestRequestTypeDef(
     _RequiredPutAppValidationConfigurationRequestRequestTypeDef,
     _OptionalPutAppValidationConfigurationRequestRequestTypeDef,
 ):
     pass
-
-
-GetAppValidationOutputResponseTypeDef = TypedDict(
-    "GetAppValidationOutputResponseTypeDef",
-    {
-        "validationOutputList": List[ValidationOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
```

### Comparing `mypy-boto3-sms-1.28.15.post1/mypy_boto3_sms/type_defs.pyi` & `mypy-boto3-sms-1.28.16/mypy_boto3_sms/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_sms.type_defs import LaunchDetailsTypeDef
 
-    data: LaunchDetailsTypeDef = {...}
+    data: LaunchDetailsTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -39,20 +39,21 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "LaunchDetailsTypeDef",
     "ConnectorTypeDef",
     "TagTypeDef",
     "ResponseMetadataTypeDef",
-    "CreateReplicationJobRequestRequestTypeDef",
+    "TimestampTypeDef",
     "DeleteAppLaunchConfigurationRequestRequestTypeDef",
     "DeleteAppReplicationConfigurationRequestRequestTypeDef",
     "DeleteAppRequestRequestTypeDef",
     "DeleteAppValidationConfigurationRequestRequestTypeDef",
     "DeleteReplicationJobRequestRequestTypeDef",
     "DisassociateConnectorRequestRequestTypeDef",
     "GenerateChangeSetRequestRequestTypeDef",
@@ -70,25 +71,26 @@
     "VmServerAddressTypeDef",
     "ImportAppCatalogRequestRequestTypeDef",
     "LaunchAppRequestRequestTypeDef",
     "ListAppsRequestRequestTypeDef",
     "NotificationContextTypeDef",
     "ReplicationRunStageDetailsTypeDef",
     "ServerReplicationParametersOutputTypeDef",
-    "ServerReplicationParametersTypeDef",
     "StartAppReplicationRequestRequestTypeDef",
     "StartOnDemandAppReplicationRequestRequestTypeDef",
     "StartOnDemandReplicationRunRequestRequestTypeDef",
     "StopAppReplicationRequestRequestTypeDef",
     "TerminateAppRequestRequestTypeDef",
-    "UpdateReplicationJobRequestRequestTypeDef",
     "AppSummaryTypeDef",
     "CreateReplicationJobResponseTypeDef",
     "GetConnectorsResponseTypeDef",
     "StartOnDemandReplicationRunResponseTypeDef",
+    "CreateReplicationJobRequestRequestTypeDef",
+    "ServerReplicationParametersTypeDef",
+    "UpdateReplicationJobRequestRequestTypeDef",
     "GenerateChangeSetResponseTypeDef",
     "GenerateTemplateResponseTypeDef",
     "SSMOutputTypeDef",
     "SourceTypeDef",
     "UserDataTypeDef",
     "GetConnectorsRequestGetConnectorsPaginateTypeDef",
     "GetReplicationJobsRequestGetReplicationJobsPaginateTypeDef",
@@ -115,30 +117,34 @@
     "ServerValidationConfigurationTypeDef",
     "ServerValidationOutputTypeDef",
     "GetReplicationJobsResponseTypeDef",
     "GetReplicationRunsResponseTypeDef",
     "CreateAppResponseTypeDef",
     "GetAppResponseTypeDef",
     "UpdateAppResponseTypeDef",
-    "CreateAppRequestRequestTypeDef",
-    "UpdateAppRequestRequestTypeDef",
+    "ServerGroupUnionTypeDef",
     "ServerGroupLaunchConfigurationOutputTypeDef",
     "ServerGroupLaunchConfigurationTypeDef",
     "ServerGroupReplicationConfigurationOutputTypeDef",
     "ServerGroupReplicationConfigurationTypeDef",
     "ServerGroupValidationConfigurationOutputTypeDef",
     "ServerGroupValidationConfigurationTypeDef",
     "ValidationOutputTypeDef",
+    "CreateAppRequestRequestTypeDef",
+    "UpdateAppRequestRequestTypeDef",
     "GetAppLaunchConfigurationResponseTypeDef",
-    "PutAppLaunchConfigurationRequestRequestTypeDef",
+    "ServerGroupLaunchConfigurationUnionTypeDef",
     "GetAppReplicationConfigurationResponseTypeDef",
-    "PutAppReplicationConfigurationRequestRequestTypeDef",
+    "ServerGroupReplicationConfigurationUnionTypeDef",
     "GetAppValidationConfigurationResponseTypeDef",
-    "PutAppValidationConfigurationRequestRequestTypeDef",
+    "ServerGroupValidationConfigurationUnionTypeDef",
     "GetAppValidationOutputResponseTypeDef",
+    "PutAppLaunchConfigurationRequestRequestTypeDef",
+    "PutAppReplicationConfigurationRequestRequestTypeDef",
+    "PutAppValidationConfigurationRequestRequestTypeDef",
 )
 
 LaunchDetailsTypeDef = TypedDict(
     "LaunchDetailsTypeDef",
     {
         "latestLaunchTime": datetime,
         "stackName": str,
@@ -180,42 +186,15 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
-_RequiredCreateReplicationJobRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateReplicationJobRequestRequestTypeDef",
-    {
-        "serverId": str,
-        "seedReplicationTime": Union[datetime, str],
-    },
-)
-_OptionalCreateReplicationJobRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateReplicationJobRequestRequestTypeDef",
-    {
-        "frequency": int,
-        "runOnce": bool,
-        "licenseType": LicenseTypeType,
-        "roleName": str,
-        "description": str,
-        "numberOfRecentAmisToKeep": int,
-        "encrypted": bool,
-        "kmsKeyId": str,
-    },
-    total=False,
-)
-
-class CreateReplicationJobRequestRequestTypeDef(
-    _RequiredCreateReplicationJobRequestRequestTypeDef,
-    _OptionalCreateReplicationJobRequestRequestTypeDef,
-):
-    pass
-
+TimestampTypeDef = Union[datetime, str]
 DeleteAppLaunchConfigurationRequestRequestTypeDef = TypedDict(
     "DeleteAppLaunchConfigurationRequestRequestTypeDef",
     {
         "appId": str,
     },
     total=False,
 )
@@ -364,20 +343,22 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class GetReplicationRunsRequestRequestTypeDef(
     _RequiredGetReplicationRunsRequestRequestTypeDef,
     _OptionalGetReplicationRunsRequestRequestTypeDef,
 ):
     pass
 
+
 VmServerAddressTypeDef = TypedDict(
     "VmServerAddressTypeDef",
     {
         "vmManagerId": str,
         "vmId": str,
     },
     total=False,
@@ -438,28 +419,14 @@
         "numberOfRecentAmisToKeep": int,
         "encrypted": bool,
         "kmsKeyId": str,
     },
     total=False,
 )
 
-ServerReplicationParametersTypeDef = TypedDict(
-    "ServerReplicationParametersTypeDef",
-    {
-        "seedTime": Union[datetime, str],
-        "frequency": int,
-        "runOnce": bool,
-        "licenseType": LicenseTypeType,
-        "numberOfRecentAmisToKeep": int,
-        "encrypted": bool,
-        "kmsKeyId": str,
-    },
-    total=False,
-)
-
 StartAppReplicationRequestRequestTypeDef = TypedDict(
     "StartAppReplicationRequestRequestTypeDef",
     {
         "appId": str,
     },
     total=False,
 )
@@ -474,40 +441,44 @@
     "_OptionalStartOnDemandAppReplicationRequestRequestTypeDef",
     {
         "description": str,
     },
     total=False,
 )
 
+
 class StartOnDemandAppReplicationRequestRequestTypeDef(
     _RequiredStartOnDemandAppReplicationRequestRequestTypeDef,
     _OptionalStartOnDemandAppReplicationRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredStartOnDemandReplicationRunRequestRequestTypeDef = TypedDict(
     "_RequiredStartOnDemandReplicationRunRequestRequestTypeDef",
     {
         "replicationJobId": str,
     },
 )
 _OptionalStartOnDemandReplicationRunRequestRequestTypeDef = TypedDict(
     "_OptionalStartOnDemandReplicationRunRequestRequestTypeDef",
     {
         "description": str,
     },
     total=False,
 )
 
+
 class StartOnDemandReplicationRunRequestRequestTypeDef(
     _RequiredStartOnDemandReplicationRunRequestRequestTypeDef,
     _OptionalStartOnDemandReplicationRunRequestRequestTypeDef,
 ):
     pass
 
+
 StopAppReplicationRequestRequestTypeDef = TypedDict(
     "StopAppReplicationRequestRequestTypeDef",
     {
         "appId": str,
     },
     total=False,
 )
@@ -516,41 +487,14 @@
     "TerminateAppRequestRequestTypeDef",
     {
         "appId": str,
     },
     total=False,
 )
 
-_RequiredUpdateReplicationJobRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateReplicationJobRequestRequestTypeDef",
-    {
-        "replicationJobId": str,
-    },
-)
-_OptionalUpdateReplicationJobRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateReplicationJobRequestRequestTypeDef",
-    {
-        "frequency": int,
-        "nextReplicationRunStartTime": Union[datetime, str],
-        "licenseType": LicenseTypeType,
-        "roleName": str,
-        "description": str,
-        "numberOfRecentAmisToKeep": int,
-        "encrypted": bool,
-        "kmsKeyId": str,
-    },
-    total=False,
-)
-
-class UpdateReplicationJobRequestRequestTypeDef(
-    _RequiredUpdateReplicationJobRequestRequestTypeDef,
-    _OptionalUpdateReplicationJobRequestRequestTypeDef,
-):
-    pass
-
 AppSummaryTypeDef = TypedDict(
     "AppSummaryTypeDef",
     {
         "appId": str,
         "importedAppId": str,
         "name": str,
         "description": str,
@@ -594,14 +538,87 @@
     "StartOnDemandReplicationRunResponseTypeDef",
     {
         "replicationRunId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredCreateReplicationJobRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateReplicationJobRequestRequestTypeDef",
+    {
+        "serverId": str,
+        "seedReplicationTime": TimestampTypeDef,
+    },
+)
+_OptionalCreateReplicationJobRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateReplicationJobRequestRequestTypeDef",
+    {
+        "frequency": int,
+        "runOnce": bool,
+        "licenseType": LicenseTypeType,
+        "roleName": str,
+        "description": str,
+        "numberOfRecentAmisToKeep": int,
+        "encrypted": bool,
+        "kmsKeyId": str,
+    },
+    total=False,
+)
+
+
+class CreateReplicationJobRequestRequestTypeDef(
+    _RequiredCreateReplicationJobRequestRequestTypeDef,
+    _OptionalCreateReplicationJobRequestRequestTypeDef,
+):
+    pass
+
+
+ServerReplicationParametersTypeDef = TypedDict(
+    "ServerReplicationParametersTypeDef",
+    {
+        "seedTime": TimestampTypeDef,
+        "frequency": int,
+        "runOnce": bool,
+        "licenseType": LicenseTypeType,
+        "numberOfRecentAmisToKeep": int,
+        "encrypted": bool,
+        "kmsKeyId": str,
+    },
+    total=False,
+)
+
+_RequiredUpdateReplicationJobRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateReplicationJobRequestRequestTypeDef",
+    {
+        "replicationJobId": str,
+    },
+)
+_OptionalUpdateReplicationJobRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateReplicationJobRequestRequestTypeDef",
+    {
+        "frequency": int,
+        "nextReplicationRunStartTime": TimestampTypeDef,
+        "licenseType": LicenseTypeType,
+        "roleName": str,
+        "description": str,
+        "numberOfRecentAmisToKeep": int,
+        "encrypted": bool,
+        "kmsKeyId": str,
+    },
+    total=False,
+)
+
+
+class UpdateReplicationJobRequestRequestTypeDef(
+    _RequiredUpdateReplicationJobRequestRequestTypeDef,
+    _OptionalUpdateReplicationJobRequestRequestTypeDef,
+):
+    pass
+
+
 GenerateChangeSetResponseTypeDef = TypedDict(
     "GenerateChangeSetResponseTypeDef",
     {
         "s3Location": S3LocationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -665,20 +682,22 @@
     "_OptionalGetReplicationRunsRequestGetReplicationRunsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetReplicationRunsRequestGetReplicationRunsPaginateTypeDef(
     _RequiredGetReplicationRunsRequestGetReplicationRunsPaginateTypeDef,
     _OptionalGetReplicationRunsRequestGetReplicationRunsPaginateTypeDef,
 ):
     pass
 
+
 ListAppsRequestListAppsPaginateTypeDef = TypedDict(
     "ListAppsRequestListAppsPaginateTypeDef",
     {
         "appIds": Sequence[str],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -725,20 +744,22 @@
     "_OptionalNotifyAppValidationOutputRequestRequestTypeDef",
     {
         "notificationContext": NotificationContextTypeDef,
     },
     total=False,
 )
 
+
 class NotifyAppValidationOutputRequestRequestTypeDef(
     _RequiredNotifyAppValidationOutputRequestRequestTypeDef,
     _OptionalNotifyAppValidationOutputRequestRequestTypeDef,
 ):
     pass
 
+
 ReplicationRunTypeDef = TypedDict(
     "ReplicationRunTypeDef",
     {
         "replicationRunId": str,
         "state": ReplicationRunStateType,
         "type": ReplicationRunTypeType,
         "stageDetails": ReplicationRunStageDetailsTypeDef,
@@ -973,40 +994,15 @@
         "appSummary": AppSummaryTypeDef,
         "serverGroups": List[ServerGroupOutputTypeDef],
         "tags": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateAppRequestRequestTypeDef = TypedDict(
-    "CreateAppRequestRequestTypeDef",
-    {
-        "name": str,
-        "description": str,
-        "roleName": str,
-        "clientToken": str,
-        "serverGroups": Sequence[Union[ServerGroupTypeDef, ServerGroupOutputTypeDef]],
-        "tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-UpdateAppRequestRequestTypeDef = TypedDict(
-    "UpdateAppRequestRequestTypeDef",
-    {
-        "appId": str,
-        "name": str,
-        "description": str,
-        "roleName": str,
-        "serverGroups": Sequence[Union[ServerGroupTypeDef, ServerGroupOutputTypeDef]],
-        "tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
+ServerGroupUnionTypeDef = Union[ServerGroupTypeDef, ServerGroupOutputTypeDef]
 ServerGroupLaunchConfigurationOutputTypeDef = TypedDict(
     "ServerGroupLaunchConfigurationOutputTypeDef",
     {
         "serverGroupId": str,
         "launchOrder": int,
         "serverLaunchConfigurations": List[ServerLaunchConfigurationTypeDef],
     },
@@ -1069,101 +1065,127 @@
         "latestValidationTime": datetime,
         "appValidationOutput": AppValidationOutputTypeDef,
         "serverValidationOutput": ServerValidationOutputTypeDef,
     },
     total=False,
 )
 
-GetAppLaunchConfigurationResponseTypeDef = TypedDict(
-    "GetAppLaunchConfigurationResponseTypeDef",
+CreateAppRequestRequestTypeDef = TypedDict(
+    "CreateAppRequestRequestTypeDef",
+    {
+        "name": str,
+        "description": str,
+        "roleName": str,
+        "clientToken": str,
+        "serverGroups": Sequence[ServerGroupUnionTypeDef],
+        "tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+UpdateAppRequestRequestTypeDef = TypedDict(
+    "UpdateAppRequestRequestTypeDef",
     {
         "appId": str,
+        "name": str,
+        "description": str,
         "roleName": str,
-        "autoLaunch": bool,
-        "serverGroupLaunchConfigurations": List[ServerGroupLaunchConfigurationOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "serverGroups": Sequence[ServerGroupUnionTypeDef],
+        "tags": Sequence[TagTypeDef],
     },
+    total=False,
 )
 
-PutAppLaunchConfigurationRequestRequestTypeDef = TypedDict(
-    "PutAppLaunchConfigurationRequestRequestTypeDef",
+GetAppLaunchConfigurationResponseTypeDef = TypedDict(
+    "GetAppLaunchConfigurationResponseTypeDef",
     {
         "appId": str,
         "roleName": str,
         "autoLaunch": bool,
-        "serverGroupLaunchConfigurations": Sequence[
-            Union[
-                ServerGroupLaunchConfigurationTypeDef, ServerGroupLaunchConfigurationOutputTypeDef
-            ]
-        ],
+        "serverGroupLaunchConfigurations": List[ServerGroupLaunchConfigurationOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
+ServerGroupLaunchConfigurationUnionTypeDef = Union[
+    ServerGroupLaunchConfigurationTypeDef, ServerGroupLaunchConfigurationOutputTypeDef
+]
 GetAppReplicationConfigurationResponseTypeDef = TypedDict(
     "GetAppReplicationConfigurationResponseTypeDef",
     {
         "serverGroupReplicationConfigurations": List[
             ServerGroupReplicationConfigurationOutputTypeDef
         ],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutAppReplicationConfigurationRequestRequestTypeDef = TypedDict(
-    "PutAppReplicationConfigurationRequestRequestTypeDef",
-    {
-        "appId": str,
-        "serverGroupReplicationConfigurations": Sequence[
-            Union[
-                ServerGroupReplicationConfigurationTypeDef,
-                ServerGroupReplicationConfigurationOutputTypeDef,
-            ]
-        ],
-    },
-    total=False,
-)
-
+ServerGroupReplicationConfigurationUnionTypeDef = Union[
+    ServerGroupReplicationConfigurationTypeDef, ServerGroupReplicationConfigurationOutputTypeDef
+]
 GetAppValidationConfigurationResponseTypeDef = TypedDict(
     "GetAppValidationConfigurationResponseTypeDef",
     {
         "appValidationConfigurations": List[AppValidationConfigurationTypeDef],
         "serverGroupValidationConfigurations": List[
             ServerGroupValidationConfigurationOutputTypeDef
         ],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ServerGroupValidationConfigurationUnionTypeDef = Union[
+    ServerGroupValidationConfigurationTypeDef, ServerGroupValidationConfigurationOutputTypeDef
+]
+GetAppValidationOutputResponseTypeDef = TypedDict(
+    "GetAppValidationOutputResponseTypeDef",
+    {
+        "validationOutputList": List[ValidationOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutAppLaunchConfigurationRequestRequestTypeDef = TypedDict(
+    "PutAppLaunchConfigurationRequestRequestTypeDef",
+    {
+        "appId": str,
+        "roleName": str,
+        "autoLaunch": bool,
+        "serverGroupLaunchConfigurations": Sequence[ServerGroupLaunchConfigurationUnionTypeDef],
+    },
+    total=False,
+)
+
+PutAppReplicationConfigurationRequestRequestTypeDef = TypedDict(
+    "PutAppReplicationConfigurationRequestRequestTypeDef",
+    {
+        "appId": str,
+        "serverGroupReplicationConfigurations": Sequence[
+            ServerGroupReplicationConfigurationUnionTypeDef
+        ],
+    },
+    total=False,
+)
+
 _RequiredPutAppValidationConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredPutAppValidationConfigurationRequestRequestTypeDef",
     {
         "appId": str,
     },
 )
 _OptionalPutAppValidationConfigurationRequestRequestTypeDef = TypedDict(
     "_OptionalPutAppValidationConfigurationRequestRequestTypeDef",
     {
         "appValidationConfigurations": Sequence[AppValidationConfigurationTypeDef],
         "serverGroupValidationConfigurations": Sequence[
-            Union[
-                ServerGroupValidationConfigurationTypeDef,
-                ServerGroupValidationConfigurationOutputTypeDef,
-            ]
+            ServerGroupValidationConfigurationUnionTypeDef
         ],
     },
     total=False,
 )
 
+
 class PutAppValidationConfigurationRequestRequestTypeDef(
     _RequiredPutAppValidationConfigurationRequestRequestTypeDef,
     _OptionalPutAppValidationConfigurationRequestRequestTypeDef,
 ):
     pass
-
-GetAppValidationOutputResponseTypeDef = TypedDict(
-    "GetAppValidationOutputResponseTypeDef",
-    {
-        "validationOutputList": List[ValidationOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
```

### Comparing `mypy-boto3-sms-1.28.15.post1/mypy_boto3_sms.egg-info/PKG-INFO` & `mypy-boto3-sms-1.28.16/mypy_boto3_sms.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sms
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.SMS 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.SMS 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 sms type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 sms type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sms.svg?color=blue)](https://pypi.org/project/mypy-boto3-sms)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sms)](https://pepy.tech/project/mypy-boto3-sms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SMS 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS)
+[boto3.SMS 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS)
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
 [mypy-boto3-sms docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/).
 
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
@@ -345,28 +345,28 @@
 )
 
 
 def check_value(value: AppLaunchConfigurationStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_sms.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_sms.type_defs import (
     LaunchDetailsTypeDef,
     ConnectorTypeDef,
     TagTypeDef,
     ResponseMetadataTypeDef,
-    CreateReplicationJobRequestRequestTypeDef,
+    TimestampTypeDef,
     DeleteAppLaunchConfigurationRequestRequestTypeDef,
     DeleteAppReplicationConfigurationRequestRequestTypeDef,
     DeleteAppRequestRequestTypeDef,
     DeleteAppValidationConfigurationRequestRequestTypeDef,
     DeleteReplicationJobRequestRequestTypeDef,
     DisassociateConnectorRequestRequestTypeDef,
     GenerateChangeSetRequestRequestTypeDef,
@@ -384,25 +384,26 @@
     VmServerAddressTypeDef,
     ImportAppCatalogRequestRequestTypeDef,
     LaunchAppRequestRequestTypeDef,
     ListAppsRequestRequestTypeDef,
     NotificationContextTypeDef,
     ReplicationRunStageDetailsTypeDef,
     ServerReplicationParametersOutputTypeDef,
-    ServerReplicationParametersTypeDef,
     StartAppReplicationRequestRequestTypeDef,
     StartOnDemandAppReplicationRequestRequestTypeDef,
     StartOnDemandReplicationRunRequestRequestTypeDef,
     StopAppReplicationRequestRequestTypeDef,
     TerminateAppRequestRequestTypeDef,
-    UpdateReplicationJobRequestRequestTypeDef,
     AppSummaryTypeDef,
     CreateReplicationJobResponseTypeDef,
     GetConnectorsResponseTypeDef,
     StartOnDemandReplicationRunResponseTypeDef,
+    CreateReplicationJobRequestRequestTypeDef,
+    ServerReplicationParametersTypeDef,
+    UpdateReplicationJobRequestRequestTypeDef,
     GenerateChangeSetResponseTypeDef,
     GenerateTemplateResponseTypeDef,
     SSMOutputTypeDef,
     SourceTypeDef,
     UserDataTypeDef,
     GetConnectorsRequestGetConnectorsPaginateTypeDef,
     GetReplicationJobsRequestGetReplicationJobsPaginateTypeDef,
@@ -429,34 +430,38 @@
     ServerValidationConfigurationTypeDef,
     ServerValidationOutputTypeDef,
     GetReplicationJobsResponseTypeDef,
     GetReplicationRunsResponseTypeDef,
     CreateAppResponseTypeDef,
     GetAppResponseTypeDef,
     UpdateAppResponseTypeDef,
-    CreateAppRequestRequestTypeDef,
-    UpdateAppRequestRequestTypeDef,
+    ServerGroupUnionTypeDef,
     ServerGroupLaunchConfigurationOutputTypeDef,
     ServerGroupLaunchConfigurationTypeDef,
     ServerGroupReplicationConfigurationOutputTypeDef,
     ServerGroupReplicationConfigurationTypeDef,
     ServerGroupValidationConfigurationOutputTypeDef,
     ServerGroupValidationConfigurationTypeDef,
     ValidationOutputTypeDef,
+    CreateAppRequestRequestTypeDef,
+    UpdateAppRequestRequestTypeDef,
     GetAppLaunchConfigurationResponseTypeDef,
-    PutAppLaunchConfigurationRequestRequestTypeDef,
+    ServerGroupLaunchConfigurationUnionTypeDef,
     GetAppReplicationConfigurationResponseTypeDef,
-    PutAppReplicationConfigurationRequestRequestTypeDef,
+    ServerGroupReplicationConfigurationUnionTypeDef,
     GetAppValidationConfigurationResponseTypeDef,
-    PutAppValidationConfigurationRequestRequestTypeDef,
+    ServerGroupValidationConfigurationUnionTypeDef,
     GetAppValidationOutputResponseTypeDef,
+    PutAppLaunchConfigurationRequestRequestTypeDef,
+    PutAppReplicationConfigurationRequestRequestTypeDef,
+    PutAppValidationConfigurationRequestRequestTypeDef,
 )
 
 
-def get_structure() -> LaunchDetailsTypeDef:
+def get_value() -> LaunchDetailsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-sms-1.28.15.post1/mypy_boto3_sms.egg-info/SOURCES.txt` & `mypy-boto3-sms-1.28.16/mypy_boto3_sms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sms-1.28.15.post1/setup.py` & `mypy-boto3-sms-1.28.16/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-sms",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_sms"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.SMS 1.28.15 service generated with mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.SMS 1.28.16 service generated with mypy-boto3-builder 7.17.1"
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
-    keywords="boto3 sms type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 sms type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_sms": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

