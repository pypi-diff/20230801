# Comparing `tmp/mypy-boto3-iot1click-projects-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-iot1click-projects-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-iot1click-projects-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:18 2023, max compression
+gzip compressed data, was "mypy-boto3-iot1click-projects-1.28.16.tar", last modified: Tue Aug  1 11:36:58 2023, max compression
```

## Comparing `mypy-boto3-iot1click-projects-1.28.15.post1.tar` & `mypy-boto3-iot1click-projects-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:18.397176 mypy-boto3-iot1click-projects-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:47:46.000000 mypy-boto3-iot1click-projects-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14579 2023-07-29 10:03:18.397176 mypy-boto3-iot1click-projects-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13043 2023-07-29 09:47:46.000000 mypy-boto3-iot1click-projects-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:18.397176 mypy-boto3-iot1click-projects-1.28.15.post1/mypy_boto3_iot1click_projects/
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-29 09:47:46.000000 mypy-boto3-iot1click-projects-1.28.15.post1/mypy_boto3_iot1click_projects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-07-29 09:47:46.000000 mypy-boto3-iot1click-projects-1.28.15.post1/mypy_boto3_iot1click_projects/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-07-29 09:47:46.000000 mypy-boto3-iot1click-projects-1.28.15.post1/mypy_boto3_iot1click_projects/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13410 2023-07-29 09:47:47.000000 mypy-boto3-iot1click-projects-1.28.15.post1/mypy_boto3_iot1click_projects/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    13385 2023-07-29 09:47:46.000000 mypy-boto3-iot1click-projects-1.28.15.post1/mypy_boto3_iot1click_projects/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8113 2023-07-29 09:47:47.000000 mypy-boto3-iot1click-projects-1.28.15.post1/mypy_boto3_iot1click_projects/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8111 2023-07-29 09:47:47.000000 mypy-boto3-iot1click-projects-1.28.15.post1/mypy_boto3_iot1click_projects/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-07-29 09:47:47.000000 mypy-boto3-iot1click-projects-1.28.15.post1/mypy_boto3_iot1click_projects/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-07-29 09:47:47.000000 mypy-boto3-iot1click-projects-1.28.15.post1/mypy_boto3_iot1click_projects/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:47:46.000000 mypy-boto3-iot1click-projects-1.28.15.post1/mypy_boto3_iot1click_projects/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    11351 2023-07-29 09:47:47.000000 mypy-boto3-iot1click-projects-1.28.15.post1/mypy_boto3_iot1click_projects/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    11334 2023-07-29 09:47:47.000000 mypy-boto3-iot1click-projects-1.28.15.post1/mypy_boto3_iot1click_projects/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:47:46.000000 mypy-boto3-iot1click-projects-1.28.15.post1/mypy_boto3_iot1click_projects/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:18.397176 mypy-boto3-iot1click-projects-1.28.15.post1/mypy_boto3_iot1click_projects.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14579 2023-07-29 10:03:18.000000 mypy-boto3-iot1click-projects-1.28.15.post1/mypy_boto3_iot1click_projects.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-07-29 10:03:18.000000 mypy-boto3-iot1click-projects-1.28.15.post1/mypy_boto3_iot1click_projects.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:18.000000 mypy-boto3-iot1click-projects-1.28.15.post1/mypy_boto3_iot1click_projects.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:18.000000 mypy-boto3-iot1click-projects-1.28.15.post1/mypy_boto3_iot1click_projects.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:18.000000 mypy-boto3-iot1click-projects-1.28.15.post1/mypy_boto3_iot1click_projects.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-29 10:03:18.000000 mypy-boto3-iot1click-projects-1.28.15.post1/mypy_boto3_iot1click_projects.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:18.397176 mypy-boto3-iot1click-projects-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-07-29 09:47:46.000000 mypy-boto3-iot1click-projects-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:58.856868 mypy-boto3-iot1click-projects-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:20:28.000000 mypy-boto3-iot1click-projects-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14604 2023-08-01 11:36:58.832868 mypy-boto3-iot1click-projects-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13077 2023-08-01 11:20:28.000000 mypy-boto3-iot1click-projects-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:58.832868 mypy-boto3-iot1click-projects-1.28.16/mypy_boto3_iot1click_projects/
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-08-01 11:20:28.000000 mypy-boto3-iot1click-projects-1.28.16/mypy_boto3_iot1click_projects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-08-01 11:20:28.000000 mypy-boto3-iot1click-projects-1.28.16/mypy_boto3_iot1click_projects/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-08-01 11:20:28.000000 mypy-boto3-iot1click-projects-1.28.16/mypy_boto3_iot1click_projects/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13304 2023-08-01 11:20:28.000000 mypy-boto3-iot1click-projects-1.28.16/mypy_boto3_iot1click_projects/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13279 2023-08-01 11:20:28.000000 mypy-boto3-iot1click-projects-1.28.16/mypy_boto3_iot1click_projects/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8113 2023-08-01 11:20:29.000000 mypy-boto3-iot1click-projects-1.28.16/mypy_boto3_iot1click_projects/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8111 2023-08-01 11:20:29.000000 mypy-boto3-iot1click-projects-1.28.16/mypy_boto3_iot1click_projects/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-08-01 11:20:28.000000 mypy-boto3-iot1click-projects-1.28.16/mypy_boto3_iot1click_projects/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-08-01 11:20:28.000000 mypy-boto3-iot1click-projects-1.28.16/mypy_boto3_iot1click_projects/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:20:28.000000 mypy-boto3-iot1click-projects-1.28.16/mypy_boto3_iot1click_projects/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    11489 2023-08-01 11:20:31.000000 mypy-boto3-iot1click-projects-1.28.16/mypy_boto3_iot1click_projects/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11472 2023-08-01 11:20:29.000000 mypy-boto3-iot1click-projects-1.28.16/mypy_boto3_iot1click_projects/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:20:28.000000 mypy-boto3-iot1click-projects-1.28.16/mypy_boto3_iot1click_projects/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:58.832868 mypy-boto3-iot1click-projects-1.28.16/mypy_boto3_iot1click_projects.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14604 2023-08-01 11:36:58.000000 mypy-boto3-iot1click-projects-1.28.16/mypy_boto3_iot1click_projects.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-08-01 11:36:58.000000 mypy-boto3-iot1click-projects-1.28.16/mypy_boto3_iot1click_projects.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:58.000000 mypy-boto3-iot1click-projects-1.28.16/mypy_boto3_iot1click_projects.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:58.000000 mypy-boto3-iot1click-projects-1.28.16/mypy_boto3_iot1click_projects.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:58.000000 mypy-boto3-iot1click-projects-1.28.16/mypy_boto3_iot1click_projects.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-01 11:36:58.000000 mypy-boto3-iot1click-projects-1.28.16/mypy_boto3_iot1click_projects.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:58.856868 mypy-boto3-iot1click-projects-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-08-01 11:20:28.000000 mypy-boto3-iot1click-projects-1.28.16/setup.py
```

### Comparing `mypy-boto3-iot1click-projects-1.28.15.post1/LICENSE` & `mypy-boto3-iot1click-projects-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot1click-projects-1.28.15.post1/PKG-INFO` & `mypy-boto3-iot1click-projects-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iot1click-projects
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.IoT1ClickProjects 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.IoT1ClickProjects 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_projects/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 iot1click-projects type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 iot1click-projects type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iot1click-projects.svg?color=blue)](https://pypi.org/project/mypy-boto3-iot1click-projects)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_projects/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iot1click-projects)](https://pepy.tech/project/mypy-boto3-iot1click-projects)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoT1ClickProjects 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects)
+[boto3.IoT1ClickProjects 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects)
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
 [mypy-boto3-iot1click-projects docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_projects/).
 
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
@@ -313,20 +313,20 @@
 )
 
 
 def check_value(value: ListPlacementsPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_iot1click_projects.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_iot1click_projects.type_defs import (
     AssociateDeviceWithPlacementRequestRequestTypeDef,
     CreatePlacementRequestRequestTypeDef,
     DeletePlacementRequestRequestTypeDef,
     DeleteProjectRequestRequestTypeDef,
@@ -354,20 +354,21 @@
     PlacementTemplateTypeDef,
     ListPlacementsRequestListPlacementsPaginateTypeDef,
     ListProjectsRequestListProjectsPaginateTypeDef,
     ListPlacementsResponseTypeDef,
     ListProjectsResponseTypeDef,
     ProjectDescriptionTypeDef,
     CreateProjectRequestRequestTypeDef,
+    PlacementTemplateUnionTypeDef,
     UpdateProjectRequestRequestTypeDef,
     DescribeProjectResponseTypeDef,
 )
 
 
-def get_structure() -> AssociateDeviceWithPlacementRequestRequestTypeDef:
+def get_value() -> AssociateDeviceWithPlacementRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-iot1click-projects-1.28.15.post1/README.md` & `mypy-boto3-iot1click-projects-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iot1click-projects.svg?color=blue)](https://pypi.org/project/mypy-boto3-iot1click-projects)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_projects/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iot1click-projects)](https://pepy.tech/project/mypy-boto3-iot1click-projects)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoT1ClickProjects 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects)
+[boto3.IoT1ClickProjects 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects)
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
 [mypy-boto3-iot1click-projects docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_projects/).
 
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
@@ -281,20 +281,20 @@
 )
 
 
 def check_value(value: ListPlacementsPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_iot1click_projects.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_iot1click_projects.type_defs import (
     AssociateDeviceWithPlacementRequestRequestTypeDef,
     CreatePlacementRequestRequestTypeDef,
     DeletePlacementRequestRequestTypeDef,
     DeleteProjectRequestRequestTypeDef,
@@ -322,20 +322,21 @@
     PlacementTemplateTypeDef,
     ListPlacementsRequestListPlacementsPaginateTypeDef,
     ListProjectsRequestListProjectsPaginateTypeDef,
     ListPlacementsResponseTypeDef,
     ListProjectsResponseTypeDef,
     ProjectDescriptionTypeDef,
     CreateProjectRequestRequestTypeDef,
+    PlacementTemplateUnionTypeDef,
     UpdateProjectRequestRequestTypeDef,
     DescribeProjectResponseTypeDef,
 )
 
 
-def get_structure() -> AssociateDeviceWithPlacementRequestRequestTypeDef:
+def get_value() -> AssociateDeviceWithPlacementRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-iot1click-projects-1.28.15.post1/mypy_boto3_iot1click_projects/__init__.py` & `mypy-boto3-iot1click-projects-1.28.16/mypy_boto3_iot1click_projects/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot1click-projects-1.28.15.post1/mypy_boto3_iot1click_projects/__init__.pyi` & `mypy-boto3-iot1click-projects-1.28.16/mypy_boto3_iot1click_projects/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot1click-projects-1.28.15.post1/mypy_boto3_iot1click_projects/__main__.py` & `mypy-boto3-iot1click-projects-1.28.16/mypy_boto3_iot1click_projects/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.IoT1ClickProjects 1.28.15\nVersion:        "
-        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.IoT1ClickProjects 1.28.16\nVersion:         1.28.16\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_projects//\nBoto3 docs:  "
         "    https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects\nOther"
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

### Comparing `mypy-boto3-iot1click-projects-1.28.15.post1/mypy_boto3_iot1click_projects/client.py` & `mypy-boto3-iot1click-projects-1.28.16/mypy_boto3_iot1click_projects/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,28 +10,27 @@
     from mypy_boto3_iot1click_projects.client import IoT1ClickProjectsClient
 
     session = Session()
     client: IoT1ClickProjectsClient = session.client("iot1click-projects")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .paginator import ListPlacementsPaginator, ListProjectsPaginator
 from .type_defs import (
     DescribePlacementResponseTypeDef,
     DescribeProjectResponseTypeDef,
     GetDevicesInPlacementResponseTypeDef,
     ListPlacementsResponseTypeDef,
     ListProjectsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    PlacementTemplateOutputTypeDef,
-    PlacementTemplateTypeDef,
+    PlacementTemplateUnionTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -110,15 +109,15 @@
         """
 
     def create_project(
         self,
         *,
         projectName: str,
         description: str = ...,
-        placementTemplate: Union[PlacementTemplateTypeDef, PlacementTemplateOutputTypeDef] = ...,
+        placementTemplate: PlacementTemplateUnionTypeDef = ...,
         tags: Mapping[str, str] = ...
     ) -> Dict[str, Any]:
         """
         Creates an empty project with a placement template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects.Client.create_project)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_projects/client/#create_project)
@@ -249,15 +248,15 @@
         """
 
     def update_project(
         self,
         *,
         projectName: str,
         description: str = ...,
-        placementTemplate: Union[PlacementTemplateTypeDef, PlacementTemplateOutputTypeDef] = ...
+        placementTemplate: PlacementTemplateUnionTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Updates a project associated with your AWS account and region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects.Client.update_project)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_projects/client/#update_project)
         """
```

### Comparing `mypy-boto3-iot1click-projects-1.28.15.post1/mypy_boto3_iot1click_projects/client.pyi` & `mypy-boto3-iot1click-projects-1.28.16/mypy_boto3_iot1click_projects/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -10,28 +10,27 @@
     from mypy_boto3_iot1click_projects.client import IoT1ClickProjectsClient
 
     session = Session()
     client: IoT1ClickProjectsClient = session.client("iot1click-projects")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .paginator import ListPlacementsPaginator, ListProjectsPaginator
 from .type_defs import (
     DescribePlacementResponseTypeDef,
     DescribeProjectResponseTypeDef,
     GetDevicesInPlacementResponseTypeDef,
     ListPlacementsResponseTypeDef,
     ListProjectsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    PlacementTemplateOutputTypeDef,
-    PlacementTemplateTypeDef,
+    PlacementTemplateUnionTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -101,15 +100,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_projects/client/#create_placement)
         """
     def create_project(
         self,
         *,
         projectName: str,
         description: str = ...,
-        placementTemplate: Union[PlacementTemplateTypeDef, PlacementTemplateOutputTypeDef] = ...,
+        placementTemplate: PlacementTemplateUnionTypeDef = ...,
         tags: Mapping[str, str] = ...
     ) -> Dict[str, Any]:
         """
         Creates an empty project with a placement template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects.Client.create_project)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_projects/client/#create_project)
@@ -226,15 +225,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_projects/client/#update_placement)
         """
     def update_project(
         self,
         *,
         projectName: str,
         description: str = ...,
-        placementTemplate: Union[PlacementTemplateTypeDef, PlacementTemplateOutputTypeDef] = ...
+        placementTemplate: PlacementTemplateUnionTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Updates a project associated with your AWS account and region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects.Client.update_project)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_projects/client/#update_project)
         """
```

### Comparing `mypy-boto3-iot1click-projects-1.28.15.post1/mypy_boto3_iot1click_projects/literals.py` & `mypy-boto3-iot1click-projects-1.28.16/mypy_boto3_iot1click_projects/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot1click-projects-1.28.15.post1/mypy_boto3_iot1click_projects/literals.pyi` & `mypy-boto3-iot1click-projects-1.28.16/mypy_boto3_iot1click_projects/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot1click-projects-1.28.15.post1/mypy_boto3_iot1click_projects/paginator.py` & `mypy-boto3-iot1click-projects-1.28.16/mypy_boto3_iot1click_projects/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot1click-projects-1.28.15.post1/mypy_boto3_iot1click_projects/paginator.pyi` & `mypy-boto3-iot1click-projects-1.28.16/mypy_boto3_iot1click_projects/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot1click-projects-1.28.15.post1/mypy_boto3_iot1click_projects/type_defs.py` & `mypy-boto3-iot1click-projects-1.28.16/mypy_boto3_iot1click_projects/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_projects/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_iot1click_projects.type_defs import AssociateDeviceWithPlacementRequestRequestTypeDef
 
-    data: AssociateDeviceWithPlacementRequestRequestTypeDef = {...}
+    data: AssociateDeviceWithPlacementRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
@@ -50,14 +50,15 @@
     "PlacementTemplateTypeDef",
     "ListPlacementsRequestListPlacementsPaginateTypeDef",
     "ListProjectsRequestListProjectsPaginateTypeDef",
     "ListPlacementsResponseTypeDef",
     "ListProjectsResponseTypeDef",
     "ProjectDescriptionTypeDef",
     "CreateProjectRequestRequestTypeDef",
+    "PlacementTemplateUnionTypeDef",
     "UpdateProjectRequestRequestTypeDef",
     "DescribeProjectResponseTypeDef",
 )
 
 AssociateDeviceWithPlacementRequestRequestTypeDef = TypedDict(
     "AssociateDeviceWithPlacementRequestRequestTypeDef",
     {
@@ -430,14 +431,15 @@
 
 class CreateProjectRequestRequestTypeDef(
     _RequiredCreateProjectRequestRequestTypeDef, _OptionalCreateProjectRequestRequestTypeDef
 ):
     pass
 
 
+PlacementTemplateUnionTypeDef = Union[PlacementTemplateTypeDef, PlacementTemplateOutputTypeDef]
 _RequiredUpdateProjectRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateProjectRequestRequestTypeDef",
     {
         "projectName": str,
     },
 )
 _OptionalUpdateProjectRequestRequestTypeDef = TypedDict(
```

### Comparing `mypy-boto3-iot1click-projects-1.28.15.post1/mypy_boto3_iot1click_projects/type_defs.pyi` & `mypy-boto3-iot1click-projects-1.28.16/mypy_boto3_iot1click_projects/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_projects/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_iot1click_projects.type_defs import AssociateDeviceWithPlacementRequestRequestTypeDef
 
-    data: AssociateDeviceWithPlacementRequestRequestTypeDef = {...}
+    data: AssociateDeviceWithPlacementRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
@@ -49,14 +49,15 @@
     "PlacementTemplateTypeDef",
     "ListPlacementsRequestListPlacementsPaginateTypeDef",
     "ListProjectsRequestListProjectsPaginateTypeDef",
     "ListPlacementsResponseTypeDef",
     "ListProjectsResponseTypeDef",
     "ProjectDescriptionTypeDef",
     "CreateProjectRequestRequestTypeDef",
+    "PlacementTemplateUnionTypeDef",
     "UpdateProjectRequestRequestTypeDef",
     "DescribeProjectResponseTypeDef",
 )
 
 AssociateDeviceWithPlacementRequestRequestTypeDef = TypedDict(
     "AssociateDeviceWithPlacementRequestRequestTypeDef",
     {
@@ -415,14 +416,15 @@
 )
 
 class CreateProjectRequestRequestTypeDef(
     _RequiredCreateProjectRequestRequestTypeDef, _OptionalCreateProjectRequestRequestTypeDef
 ):
     pass
 
+PlacementTemplateUnionTypeDef = Union[PlacementTemplateTypeDef, PlacementTemplateOutputTypeDef]
 _RequiredUpdateProjectRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateProjectRequestRequestTypeDef",
     {
         "projectName": str,
     },
 )
 _OptionalUpdateProjectRequestRequestTypeDef = TypedDict(
```

### Comparing `mypy-boto3-iot1click-projects-1.28.15.post1/mypy_boto3_iot1click_projects.egg-info/PKG-INFO` & `mypy-boto3-iot1click-projects-1.28.16/mypy_boto3_iot1click_projects.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iot1click-projects
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.IoT1ClickProjects 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.IoT1ClickProjects 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_projects/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 iot1click-projects type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 iot1click-projects type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iot1click-projects.svg?color=blue)](https://pypi.org/project/mypy-boto3-iot1click-projects)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_projects/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iot1click-projects)](https://pepy.tech/project/mypy-boto3-iot1click-projects)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoT1ClickProjects 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects)
+[boto3.IoT1ClickProjects 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects)
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
 [mypy-boto3-iot1click-projects docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_projects/).
 
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
@@ -313,20 +313,20 @@
 )
 
 
 def check_value(value: ListPlacementsPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_iot1click_projects.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_iot1click_projects.type_defs import (
     AssociateDeviceWithPlacementRequestRequestTypeDef,
     CreatePlacementRequestRequestTypeDef,
     DeletePlacementRequestRequestTypeDef,
     DeleteProjectRequestRequestTypeDef,
@@ -354,20 +354,21 @@
     PlacementTemplateTypeDef,
     ListPlacementsRequestListPlacementsPaginateTypeDef,
     ListProjectsRequestListProjectsPaginateTypeDef,
     ListPlacementsResponseTypeDef,
     ListProjectsResponseTypeDef,
     ProjectDescriptionTypeDef,
     CreateProjectRequestRequestTypeDef,
+    PlacementTemplateUnionTypeDef,
     UpdateProjectRequestRequestTypeDef,
     DescribeProjectResponseTypeDef,
 )
 
 
-def get_structure() -> AssociateDeviceWithPlacementRequestRequestTypeDef:
+def get_value() -> AssociateDeviceWithPlacementRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-iot1click-projects-1.28.15.post1/mypy_boto3_iot1click_projects.egg-info/SOURCES.txt` & `mypy-boto3-iot1click-projects-1.28.16/mypy_boto3_iot1click_projects.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot1click-projects-1.28.15.post1/setup.py` & `mypy-boto3-iot1click-projects-1.28.16/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-iot1click-projects",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_iot1click_projects"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.IoT1ClickProjects 1.28.15 service generated with"
-        " mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.IoT1ClickProjects 1.28.16 service generated with"
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
-    keywords="boto3 iot1click-projects type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 iot1click-projects type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_iot1click_projects": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_projects/"
```

