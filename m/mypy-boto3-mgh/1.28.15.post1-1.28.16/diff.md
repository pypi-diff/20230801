# Comparing `tmp/mypy-boto3-mgh-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-mgh-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-mgh-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:42 2023, max compression
+gzip compressed data, was "mypy-boto3-mgh-1.28.16.tar", last modified: Tue Aug  1 11:37:23 2023, max compression
```

## Comparing `mypy-boto3-mgh-1.28.15.post1.tar` & `mypy-boto3-mgh-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:42.421292 mypy-boto3-mgh-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:51:30.000000 mypy-boto3-mgh-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15044 2023-07-29 10:03:42.421292 mypy-boto3-mgh-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13558 2023-07-29 09:51:30.000000 mypy-boto3-mgh-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:42.405292 mypy-boto3-mgh-1.28.15.post1/mypy_boto3_mgh/
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-07-29 09:51:30.000000 mypy-boto3-mgh-1.28.15.post1/mypy_boto3_mgh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-07-29 09:51:30.000000 mypy-boto3-mgh-1.28.15.post1/mypy_boto3_mgh/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-29 09:51:30.000000 mypy-boto3-mgh-1.28.15.post1/mypy_boto3_mgh/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17205 2023-07-29 09:51:30.000000 mypy-boto3-mgh-1.28.15.post1/mypy_boto3_mgh/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    17176 2023-07-29 09:51:30.000000 mypy-boto3-mgh-1.28.15.post1/mypy_boto3_mgh/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9027 2023-07-29 09:51:31.000000 mypy-boto3-mgh-1.28.15.post1/mypy_boto3_mgh/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9025 2023-07-29 09:51:31.000000 mypy-boto3-mgh-1.28.15.post1/mypy_boto3_mgh/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6519 2023-07-29 09:51:31.000000 mypy-boto3-mgh-1.28.15.post1/mypy_boto3_mgh/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6512 2023-07-29 09:51:30.000000 mypy-boto3-mgh-1.28.15.post1/mypy_boto3_mgh/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:51:30.000000 mypy-boto3-mgh-1.28.15.post1/mypy_boto3_mgh/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    17664 2023-07-29 09:51:31.000000 mypy-boto3-mgh-1.28.15.post1/mypy_boto3_mgh/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    17629 2023-07-29 09:51:31.000000 mypy-boto3-mgh-1.28.15.post1/mypy_boto3_mgh/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:51:30.000000 mypy-boto3-mgh-1.28.15.post1/mypy_boto3_mgh/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:42.421292 mypy-boto3-mgh-1.28.15.post1/mypy_boto3_mgh.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15044 2023-07-29 10:03:42.000000 mypy-boto3-mgh-1.28.15.post1/mypy_boto3_mgh.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-29 10:03:42.000000 mypy-boto3-mgh-1.28.15.post1/mypy_boto3_mgh.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:42.000000 mypy-boto3-mgh-1.28.15.post1/mypy_boto3_mgh.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:42.000000 mypy-boto3-mgh-1.28.15.post1/mypy_boto3_mgh.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:42.000000 mypy-boto3-mgh-1.28.15.post1/mypy_boto3_mgh.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-29 10:03:42.000000 mypy-boto3-mgh-1.28.15.post1/mypy_boto3_mgh.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:42.421292 mypy-boto3-mgh-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-29 09:51:30.000000 mypy-boto3-mgh-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:23.140815 mypy-boto3-mgh-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:24:29.000000 mypy-boto3-mgh-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15056 2023-08-01 11:37:23.132815 mypy-boto3-mgh-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13579 2023-08-01 11:24:29.000000 mypy-boto3-mgh-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:23.120815 mypy-boto3-mgh-1.28.16/mypy_boto3_mgh/
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-08-01 11:24:30.000000 mypy-boto3-mgh-1.28.16/mypy_boto3_mgh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-08-01 11:24:29.000000 mypy-boto3-mgh-1.28.16/mypy_boto3_mgh/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-08-01 11:24:30.000000 mypy-boto3-mgh-1.28.16/mypy_boto3_mgh/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17182 2023-08-01 11:24:30.000000 mypy-boto3-mgh-1.28.16/mypy_boto3_mgh/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17153 2023-08-01 11:24:30.000000 mypy-boto3-mgh-1.28.16/mypy_boto3_mgh/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9027 2023-08-01 11:24:30.000000 mypy-boto3-mgh-1.28.16/mypy_boto3_mgh/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9025 2023-08-01 11:24:30.000000 mypy-boto3-mgh-1.28.16/mypy_boto3_mgh/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6519 2023-08-01 11:24:30.000000 mypy-boto3-mgh-1.28.16/mypy_boto3_mgh/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6512 2023-08-01 11:24:30.000000 mypy-boto3-mgh-1.28.16/mypy_boto3_mgh/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:24:30.000000 mypy-boto3-mgh-1.28.16/mypy_boto3_mgh/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    17718 2023-08-01 11:24:30.000000 mypy-boto3-mgh-1.28.16/mypy_boto3_mgh/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17683 2023-08-01 11:24:30.000000 mypy-boto3-mgh-1.28.16/mypy_boto3_mgh/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:24:29.000000 mypy-boto3-mgh-1.28.16/mypy_boto3_mgh/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:23.132815 mypy-boto3-mgh-1.28.16/mypy_boto3_mgh.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15056 2023-08-01 11:37:22.000000 mypy-boto3-mgh-1.28.16/mypy_boto3_mgh.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-08-01 11:37:22.000000 mypy-boto3-mgh-1.28.16/mypy_boto3_mgh.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:22.000000 mypy-boto3-mgh-1.28.16/mypy_boto3_mgh.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:22.000000 mypy-boto3-mgh-1.28.16/mypy_boto3_mgh.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:22.000000 mypy-boto3-mgh-1.28.16/mypy_boto3_mgh.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-01 11:37:22.000000 mypy-boto3-mgh-1.28.16/mypy_boto3_mgh.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:23.140815 mypy-boto3-mgh-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-08-01 11:24:29.000000 mypy-boto3-mgh-1.28.16/setup.py
```

### Comparing `mypy-boto3-mgh-1.28.15.post1/LICENSE` & `mypy-boto3-mgh-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mgh-1.28.15.post1/PKG-INFO` & `mypy-boto3-mgh-1.28.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mgh
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.MigrationHub 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.MigrationHub 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgh/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 mgh type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 mgh type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mgh.svg?color=blue)](https://pypi.org/project/mypy-boto3-mgh)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgh/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mgh)](https://pepy.tech/project/mypy-boto3-mgh)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MigrationHub 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub)
+[boto3.MigrationHub 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub)
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
 [mypy-boto3-mgh docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgh/).
 
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
@@ -335,20 +335,20 @@
 )
 
 
 def check_value(value: ApplicationStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_mgh.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_mgh.type_defs import (
     ApplicationStateTypeDef,
     CreatedArtifactTypeDef,
     DiscoveredResourceTypeDef,
     CreateProgressUpdateStreamRequestRequestTypeDef,
@@ -365,15 +365,15 @@
     ListDiscoveredResourcesRequestRequestTypeDef,
     ListMigrationTasksRequestRequestTypeDef,
     MigrationTaskSummaryTypeDef,
     ListProgressUpdateStreamsRequestRequestTypeDef,
     ProgressUpdateStreamSummaryTypeDef,
     ResourceAttributeTypeDef,
     TaskTypeDef,
-    NotifyApplicationStateRequestRequestTypeDef,
+    TimestampTypeDef,
     AssociateCreatedArtifactRequestRequestTypeDef,
     AssociateDiscoveredResourceRequestRequestTypeDef,
     DescribeApplicationStateResultTypeDef,
     ListApplicationStatesResultTypeDef,
     ListCreatedArtifactsResultTypeDef,
     ListDiscoveredResourcesResultTypeDef,
     ListApplicationStatesRequestListApplicationStatesPaginateTypeDef,
@@ -381,20 +381,21 @@
     ListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef,
     ListMigrationTasksRequestListMigrationTasksPaginateTypeDef,
     ListProgressUpdateStreamsRequestListProgressUpdateStreamsPaginateTypeDef,
     ListMigrationTasksResultTypeDef,
     ListProgressUpdateStreamsResultTypeDef,
     PutResourceAttributesRequestRequestTypeDef,
     MigrationTaskTypeDef,
+    NotifyApplicationStateRequestRequestTypeDef,
     NotifyMigrationTaskStateRequestRequestTypeDef,
     DescribeMigrationTaskResultTypeDef,
 )
 
 
-def get_structure() -> ApplicationStateTypeDef:
+def get_value() -> ApplicationStateTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-mgh-1.28.15.post1/README.md` & `mypy-boto3-mgh-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mgh.svg?color=blue)](https://pypi.org/project/mypy-boto3-mgh)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgh/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mgh)](https://pepy.tech/project/mypy-boto3-mgh)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MigrationHub 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub)
+[boto3.MigrationHub 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub)
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
 [mypy-boto3-mgh docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgh/).
 
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
@@ -303,20 +303,20 @@
 )
 
 
 def check_value(value: ApplicationStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_mgh.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_mgh.type_defs import (
     ApplicationStateTypeDef,
     CreatedArtifactTypeDef,
     DiscoveredResourceTypeDef,
     CreateProgressUpdateStreamRequestRequestTypeDef,
@@ -333,15 +333,15 @@
     ListDiscoveredResourcesRequestRequestTypeDef,
     ListMigrationTasksRequestRequestTypeDef,
     MigrationTaskSummaryTypeDef,
     ListProgressUpdateStreamsRequestRequestTypeDef,
     ProgressUpdateStreamSummaryTypeDef,
     ResourceAttributeTypeDef,
     TaskTypeDef,
-    NotifyApplicationStateRequestRequestTypeDef,
+    TimestampTypeDef,
     AssociateCreatedArtifactRequestRequestTypeDef,
     AssociateDiscoveredResourceRequestRequestTypeDef,
     DescribeApplicationStateResultTypeDef,
     ListApplicationStatesResultTypeDef,
     ListCreatedArtifactsResultTypeDef,
     ListDiscoveredResourcesResultTypeDef,
     ListApplicationStatesRequestListApplicationStatesPaginateTypeDef,
@@ -349,20 +349,21 @@
     ListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef,
     ListMigrationTasksRequestListMigrationTasksPaginateTypeDef,
     ListProgressUpdateStreamsRequestListProgressUpdateStreamsPaginateTypeDef,
     ListMigrationTasksResultTypeDef,
     ListProgressUpdateStreamsResultTypeDef,
     PutResourceAttributesRequestRequestTypeDef,
     MigrationTaskTypeDef,
+    NotifyApplicationStateRequestRequestTypeDef,
     NotifyMigrationTaskStateRequestRequestTypeDef,
     DescribeMigrationTaskResultTypeDef,
 )
 
 
-def get_structure() -> ApplicationStateTypeDef:
+def get_value() -> ApplicationStateTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-mgh-1.28.15.post1/mypy_boto3_mgh/__init__.py` & `mypy-boto3-mgh-1.28.16/mypy_boto3_mgh/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mgh-1.28.15.post1/mypy_boto3_mgh/__init__.pyi` & `mypy-boto3-mgh-1.28.16/mypy_boto3_mgh/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mgh-1.28.15.post1/mypy_boto3_mgh/__main__.py` & `mypy-boto3-mgh-1.28.16/mypy_boto3_mgh/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.MigrationHub 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.MigrationHub 1.28.16\nVersion:         1.28.16\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgh//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub\nOther"
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

### Comparing `mypy-boto3-mgh-1.28.15.post1/mypy_boto3_mgh/client.py` & `mypy-boto3-mgh-1.28.16/mypy_boto3_mgh/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from mypy_boto3_mgh.client import MigrationHubClient
 
     session = Session()
     client: MigrationHubClient = session.client("mgh")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import ApplicationStatusType
 from .paginator import (
     ListApplicationStatesPaginator,
     ListCreatedArtifactsPaginator,
@@ -35,14 +34,15 @@
     ListApplicationStatesResultTypeDef,
     ListCreatedArtifactsResultTypeDef,
     ListDiscoveredResourcesResultTypeDef,
     ListMigrationTasksResultTypeDef,
     ListProgressUpdateStreamsResultTypeDef,
     ResourceAttributeTypeDef,
     TaskTypeDef,
+    TimestampTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -300,15 +300,15 @@
         """
 
     def notify_application_state(
         self,
         *,
         ApplicationId: str,
         Status: ApplicationStatusType,
-        UpdateDateTime: Union[datetime, str] = ...,
+        UpdateDateTime: TimestampTypeDef = ...,
         DryRun: bool = ...
     ) -> Dict[str, Any]:
         """
         Sets the migration state of an application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub.Client.notify_application_state)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgh/client/#notify_application_state)
@@ -316,15 +316,15 @@
 
     def notify_migration_task_state(
         self,
         *,
         ProgressUpdateStream: str,
         MigrationTaskName: str,
         Task: TaskTypeDef,
-        UpdateDateTime: Union[datetime, str],
+        UpdateDateTime: TimestampTypeDef,
         NextUpdateSeconds: int,
         DryRun: bool = ...
     ) -> Dict[str, Any]:
         """
         Notifies Migration Hub of the current status, progress, or other detail
         regarding a migration task.
```

### Comparing `mypy-boto3-mgh-1.28.15.post1/mypy_boto3_mgh/client.pyi` & `mypy-boto3-mgh-1.28.16/mypy_boto3_mgh/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from mypy_boto3_mgh.client import MigrationHubClient
 
     session = Session()
     client: MigrationHubClient = session.client("mgh")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import ApplicationStatusType
 from .paginator import (
     ListApplicationStatesPaginator,
     ListCreatedArtifactsPaginator,
@@ -35,14 +34,15 @@
     ListApplicationStatesResultTypeDef,
     ListCreatedArtifactsResultTypeDef,
     ListDiscoveredResourcesResultTypeDef,
     ListMigrationTasksResultTypeDef,
     ListProgressUpdateStreamsResultTypeDef,
     ResourceAttributeTypeDef,
     TaskTypeDef,
+    TimestampTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -278,30 +278,30 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgh/client/#list_progress_update_streams)
         """
     def notify_application_state(
         self,
         *,
         ApplicationId: str,
         Status: ApplicationStatusType,
-        UpdateDateTime: Union[datetime, str] = ...,
+        UpdateDateTime: TimestampTypeDef = ...,
         DryRun: bool = ...
     ) -> Dict[str, Any]:
         """
         Sets the migration state of an application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub.Client.notify_application_state)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgh/client/#notify_application_state)
         """
     def notify_migration_task_state(
         self,
         *,
         ProgressUpdateStream: str,
         MigrationTaskName: str,
         Task: TaskTypeDef,
-        UpdateDateTime: Union[datetime, str],
+        UpdateDateTime: TimestampTypeDef,
         NextUpdateSeconds: int,
         DryRun: bool = ...
     ) -> Dict[str, Any]:
         """
         Notifies Migration Hub of the current status, progress, or other detail
         regarding a migration task.
```

### Comparing `mypy-boto3-mgh-1.28.15.post1/mypy_boto3_mgh/literals.py` & `mypy-boto3-mgh-1.28.16/mypy_boto3_mgh/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mgh-1.28.15.post1/mypy_boto3_mgh/literals.pyi` & `mypy-boto3-mgh-1.28.16/mypy_boto3_mgh/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mgh-1.28.15.post1/mypy_boto3_mgh/paginator.py` & `mypy-boto3-mgh-1.28.16/mypy_boto3_mgh/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mgh-1.28.15.post1/mypy_boto3_mgh/paginator.pyi` & `mypy-boto3-mgh-1.28.16/mypy_boto3_mgh/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mgh-1.28.15.post1/mypy_boto3_mgh/type_defs.py` & `mypy-boto3-mgh-1.28.16/mypy_boto3_mgh/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgh/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_mgh.type_defs import ApplicationStateTypeDef
 
-    data: ApplicationStateTypeDef = {...}
+    data: ApplicationStateTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import ApplicationStatusType, ResourceAttributeTypeType, StatusType
@@ -41,15 +41,15 @@
     "ListDiscoveredResourcesRequestRequestTypeDef",
     "ListMigrationTasksRequestRequestTypeDef",
     "MigrationTaskSummaryTypeDef",
     "ListProgressUpdateStreamsRequestRequestTypeDef",
     "ProgressUpdateStreamSummaryTypeDef",
     "ResourceAttributeTypeDef",
     "TaskTypeDef",
-    "NotifyApplicationStateRequestRequestTypeDef",
+    "TimestampTypeDef",
     "AssociateCreatedArtifactRequestRequestTypeDef",
     "AssociateDiscoveredResourceRequestRequestTypeDef",
     "DescribeApplicationStateResultTypeDef",
     "ListApplicationStatesResultTypeDef",
     "ListCreatedArtifactsResultTypeDef",
     "ListDiscoveredResourcesResultTypeDef",
     "ListApplicationStatesRequestListApplicationStatesPaginateTypeDef",
@@ -57,14 +57,15 @@
     "ListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef",
     "ListMigrationTasksRequestListMigrationTasksPaginateTypeDef",
     "ListProgressUpdateStreamsRequestListProgressUpdateStreamsPaginateTypeDef",
     "ListMigrationTasksResultTypeDef",
     "ListProgressUpdateStreamsResultTypeDef",
     "PutResourceAttributesRequestRequestTypeDef",
     "MigrationTaskTypeDef",
+    "NotifyApplicationStateRequestRequestTypeDef",
     "NotifyMigrationTaskStateRequestRequestTypeDef",
     "DescribeMigrationTaskResultTypeDef",
 )
 
 ApplicationStateTypeDef = TypedDict(
     "ApplicationStateTypeDef",
     {
@@ -388,38 +389,15 @@
 )
 
 
 class TaskTypeDef(_RequiredTaskTypeDef, _OptionalTaskTypeDef):
     pass
 
 
-_RequiredNotifyApplicationStateRequestRequestTypeDef = TypedDict(
-    "_RequiredNotifyApplicationStateRequestRequestTypeDef",
-    {
-        "ApplicationId": str,
-        "Status": ApplicationStatusType,
-    },
-)
-_OptionalNotifyApplicationStateRequestRequestTypeDef = TypedDict(
-    "_OptionalNotifyApplicationStateRequestRequestTypeDef",
-    {
-        "UpdateDateTime": Union[datetime, str],
-        "DryRun": bool,
-    },
-    total=False,
-)
-
-
-class NotifyApplicationStateRequestRequestTypeDef(
-    _RequiredNotifyApplicationStateRequestRequestTypeDef,
-    _OptionalNotifyApplicationStateRequestRequestTypeDef,
-):
-    pass
-
-
+TimestampTypeDef = Union[datetime, str]
 _RequiredAssociateCreatedArtifactRequestRequestTypeDef = TypedDict(
     "_RequiredAssociateCreatedArtifactRequestRequestTypeDef",
     {
         "ProgressUpdateStream": str,
         "MigrationTaskName": str,
         "CreatedArtifact": CreatedArtifactTypeDef,
     },
@@ -622,21 +600,45 @@
         "Task": TaskTypeDef,
         "UpdateDateTime": datetime,
         "ResourceAttributeList": List[ResourceAttributeTypeDef],
     },
     total=False,
 )
 
+_RequiredNotifyApplicationStateRequestRequestTypeDef = TypedDict(
+    "_RequiredNotifyApplicationStateRequestRequestTypeDef",
+    {
+        "ApplicationId": str,
+        "Status": ApplicationStatusType,
+    },
+)
+_OptionalNotifyApplicationStateRequestRequestTypeDef = TypedDict(
+    "_OptionalNotifyApplicationStateRequestRequestTypeDef",
+    {
+        "UpdateDateTime": TimestampTypeDef,
+        "DryRun": bool,
+    },
+    total=False,
+)
+
+
+class NotifyApplicationStateRequestRequestTypeDef(
+    _RequiredNotifyApplicationStateRequestRequestTypeDef,
+    _OptionalNotifyApplicationStateRequestRequestTypeDef,
+):
+    pass
+
+
 _RequiredNotifyMigrationTaskStateRequestRequestTypeDef = TypedDict(
     "_RequiredNotifyMigrationTaskStateRequestRequestTypeDef",
     {
         "ProgressUpdateStream": str,
         "MigrationTaskName": str,
         "Task": TaskTypeDef,
-        "UpdateDateTime": Union[datetime, str],
+        "UpdateDateTime": TimestampTypeDef,
         "NextUpdateSeconds": int,
     },
 )
 _OptionalNotifyMigrationTaskStateRequestRequestTypeDef = TypedDict(
     "_OptionalNotifyMigrationTaskStateRequestRequestTypeDef",
     {
         "DryRun": bool,
```

### Comparing `mypy-boto3-mgh-1.28.15.post1/mypy_boto3_mgh/type_defs.pyi` & `mypy-boto3-mgh-1.28.16/mypy_boto3_mgh/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgh/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_mgh.type_defs import ApplicationStateTypeDef
 
-    data: ApplicationStateTypeDef = {...}
+    data: ApplicationStateTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import ApplicationStatusType, ResourceAttributeTypeType, StatusType
@@ -40,15 +40,15 @@
     "ListDiscoveredResourcesRequestRequestTypeDef",
     "ListMigrationTasksRequestRequestTypeDef",
     "MigrationTaskSummaryTypeDef",
     "ListProgressUpdateStreamsRequestRequestTypeDef",
     "ProgressUpdateStreamSummaryTypeDef",
     "ResourceAttributeTypeDef",
     "TaskTypeDef",
-    "NotifyApplicationStateRequestRequestTypeDef",
+    "TimestampTypeDef",
     "AssociateCreatedArtifactRequestRequestTypeDef",
     "AssociateDiscoveredResourceRequestRequestTypeDef",
     "DescribeApplicationStateResultTypeDef",
     "ListApplicationStatesResultTypeDef",
     "ListCreatedArtifactsResultTypeDef",
     "ListDiscoveredResourcesResultTypeDef",
     "ListApplicationStatesRequestListApplicationStatesPaginateTypeDef",
@@ -56,14 +56,15 @@
     "ListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef",
     "ListMigrationTasksRequestListMigrationTasksPaginateTypeDef",
     "ListProgressUpdateStreamsRequestListProgressUpdateStreamsPaginateTypeDef",
     "ListMigrationTasksResultTypeDef",
     "ListProgressUpdateStreamsResultTypeDef",
     "PutResourceAttributesRequestRequestTypeDef",
     "MigrationTaskTypeDef",
+    "NotifyApplicationStateRequestRequestTypeDef",
     "NotifyMigrationTaskStateRequestRequestTypeDef",
     "DescribeMigrationTaskResultTypeDef",
 )
 
 ApplicationStateTypeDef = TypedDict(
     "ApplicationStateTypeDef",
     {
@@ -367,36 +368,15 @@
     },
     total=False,
 )
 
 class TaskTypeDef(_RequiredTaskTypeDef, _OptionalTaskTypeDef):
     pass
 
-_RequiredNotifyApplicationStateRequestRequestTypeDef = TypedDict(
-    "_RequiredNotifyApplicationStateRequestRequestTypeDef",
-    {
-        "ApplicationId": str,
-        "Status": ApplicationStatusType,
-    },
-)
-_OptionalNotifyApplicationStateRequestRequestTypeDef = TypedDict(
-    "_OptionalNotifyApplicationStateRequestRequestTypeDef",
-    {
-        "UpdateDateTime": Union[datetime, str],
-        "DryRun": bool,
-    },
-    total=False,
-)
-
-class NotifyApplicationStateRequestRequestTypeDef(
-    _RequiredNotifyApplicationStateRequestRequestTypeDef,
-    _OptionalNotifyApplicationStateRequestRequestTypeDef,
-):
-    pass
-
+TimestampTypeDef = Union[datetime, str]
 _RequiredAssociateCreatedArtifactRequestRequestTypeDef = TypedDict(
     "_RequiredAssociateCreatedArtifactRequestRequestTypeDef",
     {
         "ProgressUpdateStream": str,
         "MigrationTaskName": str,
         "CreatedArtifact": CreatedArtifactTypeDef,
     },
@@ -589,21 +569,43 @@
         "Task": TaskTypeDef,
         "UpdateDateTime": datetime,
         "ResourceAttributeList": List[ResourceAttributeTypeDef],
     },
     total=False,
 )
 
+_RequiredNotifyApplicationStateRequestRequestTypeDef = TypedDict(
+    "_RequiredNotifyApplicationStateRequestRequestTypeDef",
+    {
+        "ApplicationId": str,
+        "Status": ApplicationStatusType,
+    },
+)
+_OptionalNotifyApplicationStateRequestRequestTypeDef = TypedDict(
+    "_OptionalNotifyApplicationStateRequestRequestTypeDef",
+    {
+        "UpdateDateTime": TimestampTypeDef,
+        "DryRun": bool,
+    },
+    total=False,
+)
+
+class NotifyApplicationStateRequestRequestTypeDef(
+    _RequiredNotifyApplicationStateRequestRequestTypeDef,
+    _OptionalNotifyApplicationStateRequestRequestTypeDef,
+):
+    pass
+
 _RequiredNotifyMigrationTaskStateRequestRequestTypeDef = TypedDict(
     "_RequiredNotifyMigrationTaskStateRequestRequestTypeDef",
     {
         "ProgressUpdateStream": str,
         "MigrationTaskName": str,
         "Task": TaskTypeDef,
-        "UpdateDateTime": Union[datetime, str],
+        "UpdateDateTime": TimestampTypeDef,
         "NextUpdateSeconds": int,
     },
 )
 _OptionalNotifyMigrationTaskStateRequestRequestTypeDef = TypedDict(
     "_OptionalNotifyMigrationTaskStateRequestRequestTypeDef",
     {
         "DryRun": bool,
```

### Comparing `mypy-boto3-mgh-1.28.15.post1/mypy_boto3_mgh.egg-info/PKG-INFO` & `mypy-boto3-mgh-1.28.16/mypy_boto3_mgh.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mgh
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.MigrationHub 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.MigrationHub 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgh/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 mgh type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 mgh type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mgh.svg?color=blue)](https://pypi.org/project/mypy-boto3-mgh)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgh/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mgh)](https://pepy.tech/project/mypy-boto3-mgh)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MigrationHub 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub)
+[boto3.MigrationHub 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub)
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
 [mypy-boto3-mgh docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgh/).
 
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
@@ -335,20 +335,20 @@
 )
 
 
 def check_value(value: ApplicationStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_mgh.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_mgh.type_defs import (
     ApplicationStateTypeDef,
     CreatedArtifactTypeDef,
     DiscoveredResourceTypeDef,
     CreateProgressUpdateStreamRequestRequestTypeDef,
@@ -365,15 +365,15 @@
     ListDiscoveredResourcesRequestRequestTypeDef,
     ListMigrationTasksRequestRequestTypeDef,
     MigrationTaskSummaryTypeDef,
     ListProgressUpdateStreamsRequestRequestTypeDef,
     ProgressUpdateStreamSummaryTypeDef,
     ResourceAttributeTypeDef,
     TaskTypeDef,
-    NotifyApplicationStateRequestRequestTypeDef,
+    TimestampTypeDef,
     AssociateCreatedArtifactRequestRequestTypeDef,
     AssociateDiscoveredResourceRequestRequestTypeDef,
     DescribeApplicationStateResultTypeDef,
     ListApplicationStatesResultTypeDef,
     ListCreatedArtifactsResultTypeDef,
     ListDiscoveredResourcesResultTypeDef,
     ListApplicationStatesRequestListApplicationStatesPaginateTypeDef,
@@ -381,20 +381,21 @@
     ListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef,
     ListMigrationTasksRequestListMigrationTasksPaginateTypeDef,
     ListProgressUpdateStreamsRequestListProgressUpdateStreamsPaginateTypeDef,
     ListMigrationTasksResultTypeDef,
     ListProgressUpdateStreamsResultTypeDef,
     PutResourceAttributesRequestRequestTypeDef,
     MigrationTaskTypeDef,
+    NotifyApplicationStateRequestRequestTypeDef,
     NotifyMigrationTaskStateRequestRequestTypeDef,
     DescribeMigrationTaskResultTypeDef,
 )
 
 
-def get_structure() -> ApplicationStateTypeDef:
+def get_value() -> ApplicationStateTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-mgh-1.28.15.post1/mypy_boto3_mgh.egg-info/SOURCES.txt` & `mypy-boto3-mgh-1.28.16/mypy_boto3_mgh.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mgh-1.28.15.post1/setup.py` & `mypy-boto3-mgh-1.28.16/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-mgh",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_mgh"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.MigrationHub 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.2"
+        "Type annotations for boto3.MigrationHub 1.28.16 service generated with mypy-boto3-builder"
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
-    keywords="boto3 mgh type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 mgh type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_mgh": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgh/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

