# Comparing `tmp/mypy-boto3-serverlessrepo-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-serverlessrepo-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-serverlessrepo-1.28.15.post1.tar", last modified: Sat Jul 29 10:04:10 2023, max compression
+gzip compressed data, was "mypy-boto3-serverlessrepo-1.28.16.tar", last modified: Tue Aug  1 11:37:50 2023, max compression
```

## Comparing `mypy-boto3-serverlessrepo-1.28.15.post1.tar` & `mypy-boto3-serverlessrepo-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:10.033395 mypy-boto3-serverlessrepo-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:59:15.000000 mypy-boto3-serverlessrepo-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15374 2023-07-29 10:04:10.033395 mypy-boto3-serverlessrepo-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13836 2023-07-29 09:59:15.000000 mypy-boto3-serverlessrepo-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:10.033395 mypy-boto3-serverlessrepo-1.28.15.post1/mypy_boto3_serverlessrepo/
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-07-29 09:59:15.000000 mypy-boto3-serverlessrepo-1.28.15.post1/mypy_boto3_serverlessrepo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-07-29 09:59:15.000000 mypy-boto3-serverlessrepo-1.28.15.post1/mypy_boto3_serverlessrepo/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-07-29 09:59:15.000000 mypy-boto3-serverlessrepo-1.28.15.post1/mypy_boto3_serverlessrepo/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15250 2023-07-29 09:59:15.000000 mypy-boto3-serverlessrepo-1.28.15.post1/mypy_boto3_serverlessrepo/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15226 2023-07-29 09:59:15.000000 mypy-boto3-serverlessrepo-1.28.15.post1/mypy_boto3_serverlessrepo/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8763 2023-07-29 09:59:15.000000 mypy-boto3-serverlessrepo-1.28.15.post1/mypy_boto3_serverlessrepo/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8761 2023-07-29 09:59:15.000000 mypy-boto3-serverlessrepo-1.28.15.post1/mypy_boto3_serverlessrepo/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4562 2023-07-29 09:59:15.000000 mypy-boto3-serverlessrepo-1.28.15.post1/mypy_boto3_serverlessrepo/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4557 2023-07-29 09:59:15.000000 mypy-boto3-serverlessrepo-1.28.15.post1/mypy_boto3_serverlessrepo/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:59:15.000000 mypy-boto3-serverlessrepo-1.28.15.post1/mypy_boto3_serverlessrepo/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    20006 2023-07-29 09:59:16.000000 mypy-boto3-serverlessrepo-1.28.15.post1/mypy_boto3_serverlessrepo/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    19974 2023-07-29 09:59:15.000000 mypy-boto3-serverlessrepo-1.28.15.post1/mypy_boto3_serverlessrepo/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:59:15.000000 mypy-boto3-serverlessrepo-1.28.15.post1/mypy_boto3_serverlessrepo/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:10.033395 mypy-boto3-serverlessrepo-1.28.15.post1/mypy_boto3_serverlessrepo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15374 2023-07-29 10:04:09.000000 mypy-boto3-serverlessrepo-1.28.15.post1/mypy_boto3_serverlessrepo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-29 10:04:09.000000 mypy-boto3-serverlessrepo-1.28.15.post1/mypy_boto3_serverlessrepo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:09.000000 mypy-boto3-serverlessrepo-1.28.15.post1/mypy_boto3_serverlessrepo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:09.000000 mypy-boto3-serverlessrepo-1.28.15.post1/mypy_boto3_serverlessrepo.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:04:09.000000 mypy-boto3-serverlessrepo-1.28.15.post1/mypy_boto3_serverlessrepo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-29 10:04:09.000000 mypy-boto3-serverlessrepo-1.28.15.post1/mypy_boto3_serverlessrepo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:04:10.033395 mypy-boto3-serverlessrepo-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-07-29 09:59:15.000000 mypy-boto3-serverlessrepo-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:50.324732 mypy-boto3-serverlessrepo-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:32:45.000000 mypy-boto3-serverlessrepo-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15408 2023-08-01 11:37:50.316732 mypy-boto3-serverlessrepo-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13879 2023-08-01 11:32:45.000000 mypy-boto3-serverlessrepo-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:50.308732 mypy-boto3-serverlessrepo-1.28.16/mypy_boto3_serverlessrepo/
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-08-01 11:32:45.000000 mypy-boto3-serverlessrepo-1.28.16/mypy_boto3_serverlessrepo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-08-01 11:32:45.000000 mypy-boto3-serverlessrepo-1.28.16/mypy_boto3_serverlessrepo/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-08-01 11:32:45.000000 mypy-boto3-serverlessrepo-1.28.16/mypy_boto3_serverlessrepo/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15114 2023-08-01 11:32:45.000000 mypy-boto3-serverlessrepo-1.28.16/mypy_boto3_serverlessrepo/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15090 2023-08-01 11:32:45.000000 mypy-boto3-serverlessrepo-1.28.16/mypy_boto3_serverlessrepo/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8763 2023-08-01 11:32:46.000000 mypy-boto3-serverlessrepo-1.28.16/mypy_boto3_serverlessrepo/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8761 2023-08-01 11:32:45.000000 mypy-boto3-serverlessrepo-1.28.16/mypy_boto3_serverlessrepo/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4562 2023-08-01 11:32:45.000000 mypy-boto3-serverlessrepo-1.28.16/mypy_boto3_serverlessrepo/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4557 2023-08-01 11:32:45.000000 mypy-boto3-serverlessrepo-1.28.16/mypy_boto3_serverlessrepo/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:32:45.000000 mypy-boto3-serverlessrepo-1.28.16/mypy_boto3_serverlessrepo/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    20114 2023-08-01 11:32:46.000000 mypy-boto3-serverlessrepo-1.28.16/mypy_boto3_serverlessrepo/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20082 2023-08-01 11:32:46.000000 mypy-boto3-serverlessrepo-1.28.16/mypy_boto3_serverlessrepo/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:32:45.000000 mypy-boto3-serverlessrepo-1.28.16/mypy_boto3_serverlessrepo/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:50.316732 mypy-boto3-serverlessrepo-1.28.16/mypy_boto3_serverlessrepo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15408 2023-08-01 11:37:50.000000 mypy-boto3-serverlessrepo-1.28.16/mypy_boto3_serverlessrepo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-08-01 11:37:50.000000 mypy-boto3-serverlessrepo-1.28.16/mypy_boto3_serverlessrepo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:50.000000 mypy-boto3-serverlessrepo-1.28.16/mypy_boto3_serverlessrepo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:50.000000 mypy-boto3-serverlessrepo-1.28.16/mypy_boto3_serverlessrepo.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:50.000000 mypy-boto3-serverlessrepo-1.28.16/mypy_boto3_serverlessrepo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-01 11:37:50.000000 mypy-boto3-serverlessrepo-1.28.16/mypy_boto3_serverlessrepo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:50.324732 mypy-boto3-serverlessrepo-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-08-01 11:32:45.000000 mypy-boto3-serverlessrepo-1.28.16/setup.py
```

### Comparing `mypy-boto3-serverlessrepo-1.28.15.post1/LICENSE` & `mypy-boto3-serverlessrepo-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-serverlessrepo-1.28.15.post1/PKG-INFO` & `mypy-boto3-serverlessrepo-1.28.16/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,61 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-serverlessrepo
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.ServerlessApplicationRepository 1.28.15 service generated with mypy-boto3-builder 7.16.2
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_serverlessrepo/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 serverlessrepo type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-serverlessrepo"></a>
 
 # mypy-boto3-serverlessrepo
 
 [![PyPI - mypy-boto3-serverlessrepo](https://img.shields.io/pypi/v/mypy-boto3-serverlessrepo.svg?color=blue)](https://pypi.org/project/mypy-boto3-serverlessrepo)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-serverlessrepo.svg?color=blue)](https://pypi.org/project/mypy-boto3-serverlessrepo)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_serverlessrepo/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-serverlessrepo)](https://pepy.tech/project/mypy-boto3-serverlessrepo)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ServerlessApplicationRepository 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository)
+[boto3.ServerlessApplicationRepository 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository)
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
 [mypy-boto3-serverlessrepo docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_serverlessrepo/).
 
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
@@ -325,20 +293,20 @@
 )
 
 
 def check_value(value: CapabilityType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_serverlessrepo.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_serverlessrepo.type_defs import (
     ApplicationDependencySummaryTypeDef,
     ApplicationPolicyStatementOutputTypeDef,
     ApplicationPolicyStatementTypeDef,
     ApplicationSummaryTypeDef,
@@ -357,15 +325,15 @@
     ListApplicationDependenciesRequestRequestTypeDef,
     ListApplicationVersionsRequestRequestTypeDef,
     VersionSummaryTypeDef,
     ListApplicationsRequestRequestTypeDef,
     RollbackTriggerTypeDef,
     UnshareApplicationRequestRequestTypeDef,
     UpdateApplicationRequestRequestTypeDef,
-    PutApplicationPolicyRequestRequestTypeDef,
+    ApplicationPolicyStatementUnionTypeDef,
     CreateCloudFormationChangeSetResponseTypeDef,
     CreateCloudFormationTemplateResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetApplicationPolicyResponseTypeDef,
     GetCloudFormationTemplateResponseTypeDef,
     ListApplicationDependenciesResponseTypeDef,
     ListApplicationsResponseTypeDef,
@@ -373,22 +341,23 @@
     CreateApplicationVersionResponseTypeDef,
     VersionTypeDef,
     ListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef,
     ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef,
     ListApplicationsRequestListApplicationsPaginateTypeDef,
     ListApplicationVersionsResponseTypeDef,
     RollbackConfigurationTypeDef,
+    PutApplicationPolicyRequestRequestTypeDef,
     CreateApplicationResponseTypeDef,
     GetApplicationResponseTypeDef,
     UpdateApplicationResponseTypeDef,
     CreateCloudFormationChangeSetRequestRequestTypeDef,
 )
 
 
-def get_structure() -> ApplicationDependencySummaryTypeDef:
+def get_value() -> ApplicationDependencySummaryTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-serverlessrepo-1.28.15.post1/README.md` & `mypy-boto3-serverlessrepo-1.28.16/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-serverlessrepo
+Version: 1.28.16
+Summary: Type annotations for boto3.ServerlessApplicationRepository 1.28.16 service generated with mypy-boto3-builder 7.17.1
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_serverlessrepo/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 serverlessrepo type-annotations botocore mypy typeshed autocomplete
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
 <a id="mypy-boto3-serverlessrepo"></a>
 
 # mypy-boto3-serverlessrepo
 
 [![PyPI - mypy-boto3-serverlessrepo](https://img.shields.io/pypi/v/mypy-boto3-serverlessrepo.svg?color=blue)](https://pypi.org/project/mypy-boto3-serverlessrepo)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-serverlessrepo.svg?color=blue)](https://pypi.org/project/mypy-boto3-serverlessrepo)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_serverlessrepo/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-serverlessrepo)](https://pepy.tech/project/mypy-boto3-serverlessrepo)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ServerlessApplicationRepository 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository)
+[boto3.ServerlessApplicationRepository 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository)
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
 [mypy-boto3-serverlessrepo docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_serverlessrepo/).
 
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
@@ -293,20 +325,20 @@
 )
 
 
 def check_value(value: CapabilityType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_serverlessrepo.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_serverlessrepo.type_defs import (
     ApplicationDependencySummaryTypeDef,
     ApplicationPolicyStatementOutputTypeDef,
     ApplicationPolicyStatementTypeDef,
     ApplicationSummaryTypeDef,
@@ -325,15 +357,15 @@
     ListApplicationDependenciesRequestRequestTypeDef,
     ListApplicationVersionsRequestRequestTypeDef,
     VersionSummaryTypeDef,
     ListApplicationsRequestRequestTypeDef,
     RollbackTriggerTypeDef,
     UnshareApplicationRequestRequestTypeDef,
     UpdateApplicationRequestRequestTypeDef,
-    PutApplicationPolicyRequestRequestTypeDef,
+    ApplicationPolicyStatementUnionTypeDef,
     CreateCloudFormationChangeSetResponseTypeDef,
     CreateCloudFormationTemplateResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetApplicationPolicyResponseTypeDef,
     GetCloudFormationTemplateResponseTypeDef,
     ListApplicationDependenciesResponseTypeDef,
     ListApplicationsResponseTypeDef,
@@ -341,22 +373,23 @@
     CreateApplicationVersionResponseTypeDef,
     VersionTypeDef,
     ListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef,
     ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef,
     ListApplicationsRequestListApplicationsPaginateTypeDef,
     ListApplicationVersionsResponseTypeDef,
     RollbackConfigurationTypeDef,
+    PutApplicationPolicyRequestRequestTypeDef,
     CreateApplicationResponseTypeDef,
     GetApplicationResponseTypeDef,
     UpdateApplicationResponseTypeDef,
     CreateCloudFormationChangeSetRequestRequestTypeDef,
 )
 
 
-def get_structure() -> ApplicationDependencySummaryTypeDef:
+def get_value() -> ApplicationDependencySummaryTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-serverlessrepo-1.28.15.post1/mypy_boto3_serverlessrepo/__init__.py` & `mypy-boto3-serverlessrepo-1.28.16/mypy_boto3_serverlessrepo/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-serverlessrepo-1.28.15.post1/mypy_boto3_serverlessrepo/__init__.pyi` & `mypy-boto3-serverlessrepo-1.28.16/mypy_boto3_serverlessrepo/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-serverlessrepo-1.28.15.post1/mypy_boto3_serverlessrepo/__main__.py` & `mypy-boto3-serverlessrepo-1.28.16/mypy_boto3_serverlessrepo/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ServerlessApplicationRepository 1.28.15\nVersion:        "
-        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.ServerlessApplicationRepository 1.28.16\nVersion:        "
+        " 1.28.16\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_serverlessrepo//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository\nOther"
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

### Comparing `mypy-boto3-serverlessrepo-1.28.15.post1/mypy_boto3_serverlessrepo/client.py` & `mypy-boto3-serverlessrepo-1.28.16/mypy_boto3_serverlessrepo/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,26 +10,25 @@
     from mypy_boto3_serverlessrepo.client import ServerlessApplicationRepositoryClient
 
     session = Session()
     client: ServerlessApplicationRepositoryClient = session.client("serverlessrepo")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .paginator import (
     ListApplicationDependenciesPaginator,
     ListApplicationsPaginator,
     ListApplicationVersionsPaginator,
 )
 from .type_defs import (
-    ApplicationPolicyStatementOutputTypeDef,
-    ApplicationPolicyStatementTypeDef,
+    ApplicationPolicyStatementUnionTypeDef,
     CreateApplicationResponseTypeDef,
     CreateApplicationVersionResponseTypeDef,
     CreateCloudFormationChangeSetResponseTypeDef,
     CreateCloudFormationTemplateResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetApplicationPolicyResponseTypeDef,
     GetApplicationResponseTypeDef,
@@ -264,20 +263,15 @@
         Lists applications owned by the requester.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository.Client.list_applications)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_serverlessrepo/client/#list_applications)
         """
 
     def put_application_policy(
-        self,
-        *,
-        ApplicationId: str,
-        Statements: Sequence[
-            Union[ApplicationPolicyStatementTypeDef, ApplicationPolicyStatementOutputTypeDef]
-        ]
+        self, *, ApplicationId: str, Statements: Sequence[ApplicationPolicyStatementUnionTypeDef]
     ) -> PutApplicationPolicyResponseTypeDef:
         """
         Sets the permission policy for an application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository.Client.put_application_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_serverlessrepo/client/#put_application_policy)
         """
```

### Comparing `mypy-boto3-serverlessrepo-1.28.15.post1/mypy_boto3_serverlessrepo/client.pyi` & `mypy-boto3-serverlessrepo-1.28.16/mypy_boto3_serverlessrepo/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,26 +10,25 @@
     from mypy_boto3_serverlessrepo.client import ServerlessApplicationRepositoryClient
 
     session = Session()
     client: ServerlessApplicationRepositoryClient = session.client("serverlessrepo")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .paginator import (
     ListApplicationDependenciesPaginator,
     ListApplicationsPaginator,
     ListApplicationVersionsPaginator,
 )
 from .type_defs import (
-    ApplicationPolicyStatementOutputTypeDef,
-    ApplicationPolicyStatementTypeDef,
+    ApplicationPolicyStatementUnionTypeDef,
     CreateApplicationResponseTypeDef,
     CreateApplicationVersionResponseTypeDef,
     CreateCloudFormationChangeSetResponseTypeDef,
     CreateCloudFormationTemplateResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetApplicationPolicyResponseTypeDef,
     GetApplicationResponseTypeDef,
@@ -245,20 +244,15 @@
         """
         Lists applications owned by the requester.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository.Client.list_applications)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_serverlessrepo/client/#list_applications)
         """
     def put_application_policy(
-        self,
-        *,
-        ApplicationId: str,
-        Statements: Sequence[
-            Union[ApplicationPolicyStatementTypeDef, ApplicationPolicyStatementOutputTypeDef]
-        ]
+        self, *, ApplicationId: str, Statements: Sequence[ApplicationPolicyStatementUnionTypeDef]
     ) -> PutApplicationPolicyResponseTypeDef:
         """
         Sets the permission policy for an application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository.Client.put_application_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_serverlessrepo/client/#put_application_policy)
         """
```

### Comparing `mypy-boto3-serverlessrepo-1.28.15.post1/mypy_boto3_serverlessrepo/literals.py` & `mypy-boto3-serverlessrepo-1.28.16/mypy_boto3_serverlessrepo/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-serverlessrepo-1.28.15.post1/mypy_boto3_serverlessrepo/literals.pyi` & `mypy-boto3-serverlessrepo-1.28.16/mypy_boto3_serverlessrepo/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-serverlessrepo-1.28.15.post1/mypy_boto3_serverlessrepo/paginator.py` & `mypy-boto3-serverlessrepo-1.28.16/mypy_boto3_serverlessrepo/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-serverlessrepo-1.28.15.post1/mypy_boto3_serverlessrepo/paginator.pyi` & `mypy-boto3-serverlessrepo-1.28.16/mypy_boto3_serverlessrepo/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-serverlessrepo-1.28.15.post1/mypy_boto3_serverlessrepo/type_defs.py` & `mypy-boto3-serverlessrepo-1.28.16/mypy_boto3_serverlessrepo/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_serverlessrepo/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_serverlessrepo.type_defs import ApplicationDependencySummaryTypeDef
 
-    data: ApplicationDependencySummaryTypeDef = {...}
+    data: ApplicationDependencySummaryTypeDef = ...
     ```
 """
 import sys
 from typing import Dict, List, Sequence, Union
 
 from .literals import CapabilityType, StatusType
 
@@ -42,15 +42,15 @@
     "ListApplicationDependenciesRequestRequestTypeDef",
     "ListApplicationVersionsRequestRequestTypeDef",
     "VersionSummaryTypeDef",
     "ListApplicationsRequestRequestTypeDef",
     "RollbackTriggerTypeDef",
     "UnshareApplicationRequestRequestTypeDef",
     "UpdateApplicationRequestRequestTypeDef",
-    "PutApplicationPolicyRequestRequestTypeDef",
+    "ApplicationPolicyStatementUnionTypeDef",
     "CreateCloudFormationChangeSetResponseTypeDef",
     "CreateCloudFormationTemplateResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetApplicationPolicyResponseTypeDef",
     "GetCloudFormationTemplateResponseTypeDef",
     "ListApplicationDependenciesResponseTypeDef",
     "ListApplicationsResponseTypeDef",
@@ -58,14 +58,15 @@
     "CreateApplicationVersionResponseTypeDef",
     "VersionTypeDef",
     "ListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef",
     "ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef",
     "ListApplicationsRequestListApplicationsPaginateTypeDef",
     "ListApplicationVersionsResponseTypeDef",
     "RollbackConfigurationTypeDef",
+    "PutApplicationPolicyRequestRequestTypeDef",
     "CreateApplicationResponseTypeDef",
     "GetApplicationResponseTypeDef",
     "UpdateApplicationResponseTypeDef",
     "CreateCloudFormationChangeSetRequestRequestTypeDef",
 )
 
 ApplicationDependencySummaryTypeDef = TypedDict(
@@ -459,24 +460,17 @@
 
 class UpdateApplicationRequestRequestTypeDef(
     _RequiredUpdateApplicationRequestRequestTypeDef, _OptionalUpdateApplicationRequestRequestTypeDef
 ):
     pass
 
 
-PutApplicationPolicyRequestRequestTypeDef = TypedDict(
-    "PutApplicationPolicyRequestRequestTypeDef",
-    {
-        "ApplicationId": str,
-        "Statements": Sequence[
-            Union[ApplicationPolicyStatementTypeDef, ApplicationPolicyStatementOutputTypeDef]
-        ],
-    },
-)
-
+ApplicationPolicyStatementUnionTypeDef = Union[
+    ApplicationPolicyStatementTypeDef, ApplicationPolicyStatementOutputTypeDef
+]
 CreateCloudFormationChangeSetResponseTypeDef = TypedDict(
     "CreateCloudFormationChangeSetResponseTypeDef",
     {
         "ApplicationId": str,
         "ChangeSetId": str,
         "SemanticVersion": str,
         "StackId": str,
@@ -662,14 +656,22 @@
     {
         "MonitoringTimeInMinutes": int,
         "RollbackTriggers": Sequence[RollbackTriggerTypeDef],
     },
     total=False,
 )
 
+PutApplicationPolicyRequestRequestTypeDef = TypedDict(
+    "PutApplicationPolicyRequestRequestTypeDef",
+    {
+        "ApplicationId": str,
+        "Statements": Sequence[ApplicationPolicyStatementUnionTypeDef],
+    },
+)
+
 CreateApplicationResponseTypeDef = TypedDict(
     "CreateApplicationResponseTypeDef",
     {
         "ApplicationId": str,
         "Author": str,
         "CreationTime": str,
         "Description": str,
```

### Comparing `mypy-boto3-serverlessrepo-1.28.15.post1/mypy_boto3_serverlessrepo/type_defs.pyi` & `mypy-boto3-serverlessrepo-1.28.16/mypy_boto3_serverlessrepo/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_serverlessrepo/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_serverlessrepo.type_defs import ApplicationDependencySummaryTypeDef
 
-    data: ApplicationDependencySummaryTypeDef = {...}
+    data: ApplicationDependencySummaryTypeDef = ...
     ```
 """
 import sys
 from typing import Dict, List, Sequence, Union
 
 from .literals import CapabilityType, StatusType
 
@@ -41,15 +41,15 @@
     "ListApplicationDependenciesRequestRequestTypeDef",
     "ListApplicationVersionsRequestRequestTypeDef",
     "VersionSummaryTypeDef",
     "ListApplicationsRequestRequestTypeDef",
     "RollbackTriggerTypeDef",
     "UnshareApplicationRequestRequestTypeDef",
     "UpdateApplicationRequestRequestTypeDef",
-    "PutApplicationPolicyRequestRequestTypeDef",
+    "ApplicationPolicyStatementUnionTypeDef",
     "CreateCloudFormationChangeSetResponseTypeDef",
     "CreateCloudFormationTemplateResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetApplicationPolicyResponseTypeDef",
     "GetCloudFormationTemplateResponseTypeDef",
     "ListApplicationDependenciesResponseTypeDef",
     "ListApplicationsResponseTypeDef",
@@ -57,14 +57,15 @@
     "CreateApplicationVersionResponseTypeDef",
     "VersionTypeDef",
     "ListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef",
     "ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef",
     "ListApplicationsRequestListApplicationsPaginateTypeDef",
     "ListApplicationVersionsResponseTypeDef",
     "RollbackConfigurationTypeDef",
+    "PutApplicationPolicyRequestRequestTypeDef",
     "CreateApplicationResponseTypeDef",
     "GetApplicationResponseTypeDef",
     "UpdateApplicationResponseTypeDef",
     "CreateCloudFormationChangeSetRequestRequestTypeDef",
 )
 
 ApplicationDependencySummaryTypeDef = TypedDict(
@@ -434,24 +435,17 @@
 )
 
 class UpdateApplicationRequestRequestTypeDef(
     _RequiredUpdateApplicationRequestRequestTypeDef, _OptionalUpdateApplicationRequestRequestTypeDef
 ):
     pass
 
-PutApplicationPolicyRequestRequestTypeDef = TypedDict(
-    "PutApplicationPolicyRequestRequestTypeDef",
-    {
-        "ApplicationId": str,
-        "Statements": Sequence[
-            Union[ApplicationPolicyStatementTypeDef, ApplicationPolicyStatementOutputTypeDef]
-        ],
-    },
-)
-
+ApplicationPolicyStatementUnionTypeDef = Union[
+    ApplicationPolicyStatementTypeDef, ApplicationPolicyStatementOutputTypeDef
+]
 CreateCloudFormationChangeSetResponseTypeDef = TypedDict(
     "CreateCloudFormationChangeSetResponseTypeDef",
     {
         "ApplicationId": str,
         "ChangeSetId": str,
         "SemanticVersion": str,
         "StackId": str,
@@ -631,14 +625,22 @@
     {
         "MonitoringTimeInMinutes": int,
         "RollbackTriggers": Sequence[RollbackTriggerTypeDef],
     },
     total=False,
 )
 
+PutApplicationPolicyRequestRequestTypeDef = TypedDict(
+    "PutApplicationPolicyRequestRequestTypeDef",
+    {
+        "ApplicationId": str,
+        "Statements": Sequence[ApplicationPolicyStatementUnionTypeDef],
+    },
+)
+
 CreateApplicationResponseTypeDef = TypedDict(
     "CreateApplicationResponseTypeDef",
     {
         "ApplicationId": str,
         "Author": str,
         "CreationTime": str,
         "Description": str,
```

### Comparing `mypy-boto3-serverlessrepo-1.28.15.post1/mypy_boto3_serverlessrepo.egg-info/PKG-INFO` & `mypy-boto3-serverlessrepo-1.28.16/mypy_boto3_serverlessrepo.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-serverlessrepo
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.ServerlessApplicationRepository 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.ServerlessApplicationRepository 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_serverlessrepo/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 serverlessrepo type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 serverlessrepo type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-serverlessrepo.svg?color=blue)](https://pypi.org/project/mypy-boto3-serverlessrepo)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_serverlessrepo/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-serverlessrepo)](https://pepy.tech/project/mypy-boto3-serverlessrepo)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ServerlessApplicationRepository 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository)
+[boto3.ServerlessApplicationRepository 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository)
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
 [mypy-boto3-serverlessrepo docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_serverlessrepo/).
 
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
@@ -325,20 +325,20 @@
 )
 
 
 def check_value(value: CapabilityType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_serverlessrepo.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_serverlessrepo.type_defs import (
     ApplicationDependencySummaryTypeDef,
     ApplicationPolicyStatementOutputTypeDef,
     ApplicationPolicyStatementTypeDef,
     ApplicationSummaryTypeDef,
@@ -357,15 +357,15 @@
     ListApplicationDependenciesRequestRequestTypeDef,
     ListApplicationVersionsRequestRequestTypeDef,
     VersionSummaryTypeDef,
     ListApplicationsRequestRequestTypeDef,
     RollbackTriggerTypeDef,
     UnshareApplicationRequestRequestTypeDef,
     UpdateApplicationRequestRequestTypeDef,
-    PutApplicationPolicyRequestRequestTypeDef,
+    ApplicationPolicyStatementUnionTypeDef,
     CreateCloudFormationChangeSetResponseTypeDef,
     CreateCloudFormationTemplateResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetApplicationPolicyResponseTypeDef,
     GetCloudFormationTemplateResponseTypeDef,
     ListApplicationDependenciesResponseTypeDef,
     ListApplicationsResponseTypeDef,
@@ -373,22 +373,23 @@
     CreateApplicationVersionResponseTypeDef,
     VersionTypeDef,
     ListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef,
     ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef,
     ListApplicationsRequestListApplicationsPaginateTypeDef,
     ListApplicationVersionsResponseTypeDef,
     RollbackConfigurationTypeDef,
+    PutApplicationPolicyRequestRequestTypeDef,
     CreateApplicationResponseTypeDef,
     GetApplicationResponseTypeDef,
     UpdateApplicationResponseTypeDef,
     CreateCloudFormationChangeSetRequestRequestTypeDef,
 )
 
 
-def get_structure() -> ApplicationDependencySummaryTypeDef:
+def get_value() -> ApplicationDependencySummaryTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-serverlessrepo-1.28.15.post1/mypy_boto3_serverlessrepo.egg-info/SOURCES.txt` & `mypy-boto3-serverlessrepo-1.28.16/mypy_boto3_serverlessrepo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-serverlessrepo-1.28.15.post1/setup.py` & `mypy-boto3-serverlessrepo-1.28.16/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-serverlessrepo",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_serverlessrepo"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ServerlessApplicationRepository 1.28.15 service generated with"
-        " mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.ServerlessApplicationRepository 1.28.16 service generated with"
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
-    keywords="boto3 serverlessrepo type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 serverlessrepo type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_serverlessrepo": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_serverlessrepo/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

