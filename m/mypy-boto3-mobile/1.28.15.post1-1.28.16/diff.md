# Comparing `tmp/mypy-boto3-mobile-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-mobile-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-mobile-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:44 2023, max compression
+gzip compressed data, was "mypy-boto3-mobile-1.28.16.tar", last modified: Tue Aug  1 11:37:24 2023, max compression
```

## Comparing `mypy-boto3-mobile-1.28.15.post1.tar` & `mypy-boto3-mobile-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:44.385301 mypy-boto3-mobile-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:51:48.000000 mypy-boto3-mobile-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13455 2023-07-29 10:03:44.377301 mypy-boto3-mobile-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11966 2023-07-29 09:51:48.000000 mypy-boto3-mobile-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:44.369300 mypy-boto3-mobile-1.28.15.post1/mypy_boto3_mobile/
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-29 09:51:48.000000 mypy-boto3-mobile-1.28.15.post1/mypy_boto3_mobile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-29 09:51:48.000000 mypy-boto3-mobile-1.28.15.post1/mypy_boto3_mobile/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-29 09:51:48.000000 mypy-boto3-mobile-1.28.15.post1/mypy_boto3_mobile/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9113 2023-07-29 09:51:48.000000 mypy-boto3-mobile-1.28.15.post1/mypy_boto3_mobile/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9095 2023-07-29 09:51:48.000000 mypy-boto3-mobile-1.28.15.post1/mypy_boto3_mobile/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8050 2023-07-29 09:51:48.000000 mypy-boto3-mobile-1.28.15.post1/mypy_boto3_mobile/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8048 2023-07-29 09:51:48.000000 mypy-boto3-mobile-1.28.15.post1/mypy_boto3_mobile/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-07-29 09:51:48.000000 mypy-boto3-mobile-1.28.15.post1/mypy_boto3_mobile/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-07-29 09:51:48.000000 mypy-boto3-mobile-1.28.15.post1/mypy_boto3_mobile/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:51:48.000000 mypy-boto3-mobile-1.28.15.post1/mypy_boto3_mobile/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     7637 2023-07-29 09:51:48.000000 mypy-boto3-mobile-1.28.15.post1/mypy_boto3_mobile/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7630 2023-07-29 09:51:48.000000 mypy-boto3-mobile-1.28.15.post1/mypy_boto3_mobile/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:51:48.000000 mypy-boto3-mobile-1.28.15.post1/mypy_boto3_mobile/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:44.377301 mypy-boto3-mobile-1.28.15.post1/mypy_boto3_mobile.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13455 2023-07-29 10:03:44.000000 mypy-boto3-mobile-1.28.15.post1/mypy_boto3_mobile.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-29 10:03:44.000000 mypy-boto3-mobile-1.28.15.post1/mypy_boto3_mobile.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:44.000000 mypy-boto3-mobile-1.28.15.post1/mypy_boto3_mobile.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:44.000000 mypy-boto3-mobile-1.28.15.post1/mypy_boto3_mobile.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:44.000000 mypy-boto3-mobile-1.28.15.post1/mypy_boto3_mobile.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-29 10:03:44.000000 mypy-boto3-mobile-1.28.15.post1/mypy_boto3_mobile.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:44.385301 mypy-boto3-mobile-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-29 09:51:48.000000 mypy-boto3-mobile-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:24.136812 mypy-boto3-mobile-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:24:45.000000 mypy-boto3-mobile-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13453 2023-08-01 11:37:24.132812 mypy-boto3-mobile-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11973 2023-08-01 11:24:45.000000 mypy-boto3-mobile-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:24.128812 mypy-boto3-mobile-1.28.16/mypy_boto3_mobile/
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-08-01 11:24:45.000000 mypy-boto3-mobile-1.28.16/mypy_boto3_mobile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-08-01 11:24:45.000000 mypy-boto3-mobile-1.28.16/mypy_boto3_mobile/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-08-01 11:24:45.000000 mypy-boto3-mobile-1.28.16/mypy_boto3_mobile/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9015 2023-08-01 11:24:45.000000 mypy-boto3-mobile-1.28.16/mypy_boto3_mobile/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8997 2023-08-01 11:24:45.000000 mypy-boto3-mobile-1.28.16/mypy_boto3_mobile/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8050 2023-08-01 11:24:45.000000 mypy-boto3-mobile-1.28.16/mypy_boto3_mobile/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8048 2023-08-01 11:24:45.000000 mypy-boto3-mobile-1.28.16/mypy_boto3_mobile/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-08-01 11:24:45.000000 mypy-boto3-mobile-1.28.16/mypy_boto3_mobile/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-08-01 11:24:45.000000 mypy-boto3-mobile-1.28.16/mypy_boto3_mobile/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:24:45.000000 mypy-boto3-mobile-1.28.16/mypy_boto3_mobile/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     7632 2023-08-01 11:24:46.000000 mypy-boto3-mobile-1.28.16/mypy_boto3_mobile/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7625 2023-08-01 11:24:46.000000 mypy-boto3-mobile-1.28.16/mypy_boto3_mobile/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:24:45.000000 mypy-boto3-mobile-1.28.16/mypy_boto3_mobile/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:24.132812 mypy-boto3-mobile-1.28.16/mypy_boto3_mobile.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13453 2023-08-01 11:37:23.000000 mypy-boto3-mobile-1.28.16/mypy_boto3_mobile.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-08-01 11:37:23.000000 mypy-boto3-mobile-1.28.16/mypy_boto3_mobile.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:23.000000 mypy-boto3-mobile-1.28.16/mypy_boto3_mobile.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:23.000000 mypy-boto3-mobile-1.28.16/mypy_boto3_mobile.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:23.000000 mypy-boto3-mobile-1.28.16/mypy_boto3_mobile.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-01 11:37:23.000000 mypy-boto3-mobile-1.28.16/mypy_boto3_mobile.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:24.136812 mypy-boto3-mobile-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-08-01 11:24:45.000000 mypy-boto3-mobile-1.28.16/setup.py
```

### Comparing `mypy-boto3-mobile-1.28.15.post1/LICENSE` & `mypy-boto3-mobile-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mobile-1.28.15.post1/PKG-INFO` & `mypy-boto3-mobile-1.28.16/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mobile
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.Mobile 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.Mobile 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mobile/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 mobile type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 mobile type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mobile.svg?color=blue)](https://pypi.org/project/mypy-boto3-mobile)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mobile/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mobile)](https://pepy.tech/project/mypy-boto3-mobile)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Mobile 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mobile.html#Mobile)
+[boto3.Mobile 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mobile.html#Mobile)
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
 [mypy-boto3-mobile docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mobile/).
 
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
@@ -312,36 +312,37 @@
 )
 
 
 def check_value(value: ListBundlesPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_mobile.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_mobile.type_defs import (
+    BlobTypeDef,
     BundleDetailsTypeDef,
-    CreateProjectRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     DeleteProjectRequestRequestTypeDef,
     ResourceTypeDef,
     DescribeBundleRequestRequestTypeDef,
     DescribeProjectRequestRequestTypeDef,
     ExportBundleRequestRequestTypeDef,
     ExportProjectRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     ListBundlesRequestRequestTypeDef,
     ListProjectsRequestRequestTypeDef,
     ProjectSummaryTypeDef,
+    CreateProjectRequestRequestTypeDef,
     UpdateProjectRequestRequestTypeDef,
     DescribeBundleResultTypeDef,
     ExportBundleResultTypeDef,
     ExportProjectResultTypeDef,
     ListBundlesResultTypeDef,
     DeleteProjectResultTypeDef,
     ProjectDetailsTypeDef,
@@ -350,15 +351,15 @@
     ListProjectsResultTypeDef,
     CreateProjectResultTypeDef,
     DescribeProjectResultTypeDef,
     UpdateProjectResultTypeDef,
 )
 
 
-def get_structure() -> BundleDetailsTypeDef:
+def get_value() -> BlobTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-mobile-1.28.15.post1/README.md` & `mypy-boto3-mobile-1.28.16/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mobile.svg?color=blue)](https://pypi.org/project/mypy-boto3-mobile)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mobile/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mobile)](https://pepy.tech/project/mypy-boto3-mobile)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Mobile 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mobile.html#Mobile)
+[boto3.Mobile 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mobile.html#Mobile)
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
 [mypy-boto3-mobile docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mobile/).
 
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
@@ -280,36 +280,37 @@
 )
 
 
 def check_value(value: ListBundlesPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_mobile.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_mobile.type_defs import (
+    BlobTypeDef,
     BundleDetailsTypeDef,
-    CreateProjectRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     DeleteProjectRequestRequestTypeDef,
     ResourceTypeDef,
     DescribeBundleRequestRequestTypeDef,
     DescribeProjectRequestRequestTypeDef,
     ExportBundleRequestRequestTypeDef,
     ExportProjectRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     ListBundlesRequestRequestTypeDef,
     ListProjectsRequestRequestTypeDef,
     ProjectSummaryTypeDef,
+    CreateProjectRequestRequestTypeDef,
     UpdateProjectRequestRequestTypeDef,
     DescribeBundleResultTypeDef,
     ExportBundleResultTypeDef,
     ExportProjectResultTypeDef,
     ListBundlesResultTypeDef,
     DeleteProjectResultTypeDef,
     ProjectDetailsTypeDef,
@@ -318,15 +319,15 @@
     ListProjectsResultTypeDef,
     CreateProjectResultTypeDef,
     DescribeProjectResultTypeDef,
     UpdateProjectResultTypeDef,
 )
 
 
-def get_structure() -> BundleDetailsTypeDef:
+def get_value() -> BlobTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-mobile-1.28.15.post1/mypy_boto3_mobile/__init__.py` & `mypy-boto3-mobile-1.28.16/mypy_boto3_mobile/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mobile-1.28.15.post1/mypy_boto3_mobile/__init__.pyi` & `mypy-boto3-mobile-1.28.16/mypy_boto3_mobile/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mobile-1.28.15.post1/mypy_boto3_mobile/__main__.py` & `mypy-boto3-mobile-1.28.16/mypy_boto3_mobile/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Mobile 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.Mobile 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mobile//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mobile.html#Mobile\nOther"
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

### Comparing `mypy-boto3-mobile-1.28.15.post1/mypy_boto3_mobile/client.py` & `mypy-boto3-mobile-1.28.16/mypy_boto3_mobile/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,22 +10,22 @@
     from mypy_boto3_mobile.client import MobileClient
 
     session = Session()
     client: MobileClient = session.client("mobile")
     ```
 """
 import sys
-from typing import IO, Any, Dict, Mapping, Type, Union, overload
+from typing import Any, Dict, Mapping, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
-from botocore.response import StreamingBody
 
 from .literals import PlatformType
 from .paginator import ListBundlesPaginator, ListProjectsPaginator
 from .type_defs import (
+    BlobTypeDef,
     CreateProjectResultTypeDef,
     DeleteProjectResultTypeDef,
     DescribeBundleResultTypeDef,
     DescribeProjectResultTypeDef,
     ExportBundleResultTypeDef,
     ExportProjectResultTypeDef,
     ListBundlesResultTypeDef,
@@ -96,15 +96,15 @@
         """
 
     def create_project(
         self,
         *,
         name: str = ...,
         region: str = ...,
-        contents: Union[str, bytes, IO[Any], StreamingBody] = ...,
+        contents: BlobTypeDef = ...,
         snapshotId: str = ...
     ) -> CreateProjectResultTypeDef:
         """
         Creates an AWS Mobile Hub project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mobile.html#Mobile.Client.create_project)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mobile/client/#create_project)
@@ -186,15 +186,15 @@
         Lists projects in AWS Mobile Hub.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mobile.html#Mobile.Client.list_projects)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mobile/client/#list_projects)
         """
 
     def update_project(
-        self, *, projectId: str, contents: Union[str, bytes, IO[Any], StreamingBody] = ...
+        self, *, projectId: str, contents: BlobTypeDef = ...
     ) -> UpdateProjectResultTypeDef:
         """
         Update an existing project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mobile.html#Mobile.Client.update_project)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mobile/client/#update_project)
         """
```

### Comparing `mypy-boto3-mobile-1.28.15.post1/mypy_boto3_mobile/client.pyi` & `mypy-boto3-mobile-1.28.16/mypy_boto3_mobile/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -10,22 +10,22 @@
     from mypy_boto3_mobile.client import MobileClient
 
     session = Session()
     client: MobileClient = session.client("mobile")
     ```
 """
 import sys
-from typing import IO, Any, Dict, Mapping, Type, Union, overload
+from typing import Any, Dict, Mapping, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
-from botocore.response import StreamingBody
 
 from .literals import PlatformType
 from .paginator import ListBundlesPaginator, ListProjectsPaginator
 from .type_defs import (
+    BlobTypeDef,
     CreateProjectResultTypeDef,
     DeleteProjectResultTypeDef,
     DescribeBundleResultTypeDef,
     DescribeProjectResultTypeDef,
     ExportBundleResultTypeDef,
     ExportProjectResultTypeDef,
     ListBundlesResultTypeDef,
@@ -89,15 +89,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mobile/client/#close)
         """
     def create_project(
         self,
         *,
         name: str = ...,
         region: str = ...,
-        contents: Union[str, bytes, IO[Any], StreamingBody] = ...,
+        contents: BlobTypeDef = ...,
         snapshotId: str = ...
     ) -> CreateProjectResultTypeDef:
         """
         Creates an AWS Mobile Hub project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mobile.html#Mobile.Client.create_project)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mobile/client/#create_project)
@@ -170,15 +170,15 @@
         """
         Lists projects in AWS Mobile Hub.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mobile.html#Mobile.Client.list_projects)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mobile/client/#list_projects)
         """
     def update_project(
-        self, *, projectId: str, contents: Union[str, bytes, IO[Any], StreamingBody] = ...
+        self, *, projectId: str, contents: BlobTypeDef = ...
     ) -> UpdateProjectResultTypeDef:
         """
         Update an existing project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mobile.html#Mobile.Client.update_project)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mobile/client/#update_project)
         """
```

### Comparing `mypy-boto3-mobile-1.28.15.post1/mypy_boto3_mobile/literals.py` & `mypy-boto3-mobile-1.28.16/mypy_boto3_mobile/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mobile-1.28.15.post1/mypy_boto3_mobile/literals.pyi` & `mypy-boto3-mobile-1.28.16/mypy_boto3_mobile/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mobile-1.28.15.post1/mypy_boto3_mobile/paginator.py` & `mypy-boto3-mobile-1.28.16/mypy_boto3_mobile/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mobile-1.28.15.post1/mypy_boto3_mobile/paginator.pyi` & `mypy-boto3-mobile-1.28.16/mypy_boto3_mobile/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mobile-1.28.15.post1/mypy_boto3_mobile/type_defs.py` & `mypy-boto3-mobile-1.28.16/mypy_boto3_mobile/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for mobile service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mobile/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_mobile.type_defs import BundleDetailsTypeDef
+    from mypy_boto3_mobile.type_defs import BlobTypeDef
 
-    data: BundleDetailsTypeDef = {...}
+    data: BlobTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Union
 
 from botocore.response import StreamingBody
@@ -22,27 +22,28 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
+    "BlobTypeDef",
     "BundleDetailsTypeDef",
-    "CreateProjectRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "DeleteProjectRequestRequestTypeDef",
     "ResourceTypeDef",
     "DescribeBundleRequestRequestTypeDef",
     "DescribeProjectRequestRequestTypeDef",
     "ExportBundleRequestRequestTypeDef",
     "ExportProjectRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "ListBundlesRequestRequestTypeDef",
     "ListProjectsRequestRequestTypeDef",
     "ProjectSummaryTypeDef",
+    "CreateProjectRequestRequestTypeDef",
     "UpdateProjectRequestRequestTypeDef",
     "DescribeBundleResultTypeDef",
     "ExportBundleResultTypeDef",
     "ExportProjectResultTypeDef",
     "ListBundlesResultTypeDef",
     "DeleteProjectResultTypeDef",
     "ProjectDetailsTypeDef",
@@ -50,38 +51,28 @@
     "ListProjectsRequestListProjectsPaginateTypeDef",
     "ListProjectsResultTypeDef",
     "CreateProjectResultTypeDef",
     "DescribeProjectResultTypeDef",
     "UpdateProjectResultTypeDef",
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 BundleDetailsTypeDef = TypedDict(
     "BundleDetailsTypeDef",
     {
         "bundleId": str,
         "title": str,
         "version": str,
         "description": str,
         "iconUrl": str,
         "availablePlatforms": List[PlatformType],
     },
     total=False,
 )
 
-CreateProjectRequestRequestTypeDef = TypedDict(
-    "CreateProjectRequestRequestTypeDef",
-    {
-        "name": str,
-        "region": str,
-        "contents": Union[str, bytes, IO[Any], StreamingBody],
-        "snapshotId": str,
-    },
-    total=False,
-)
-
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -198,24 +189,35 @@
     {
         "name": str,
         "projectId": str,
     },
     total=False,
 )
 
+CreateProjectRequestRequestTypeDef = TypedDict(
+    "CreateProjectRequestRequestTypeDef",
+    {
+        "name": str,
+        "region": str,
+        "contents": BlobTypeDef,
+        "snapshotId": str,
+    },
+    total=False,
+)
+
 _RequiredUpdateProjectRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateProjectRequestRequestTypeDef",
     {
         "projectId": str,
     },
 )
 _OptionalUpdateProjectRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateProjectRequestRequestTypeDef",
     {
-        "contents": Union[str, bytes, IO[Any], StreamingBody],
+        "contents": BlobTypeDef,
     },
     total=False,
 )
 
 
 class UpdateProjectRequestRequestTypeDef(
     _RequiredUpdateProjectRequestRequestTypeDef, _OptionalUpdateProjectRequestRequestTypeDef
```

### Comparing `mypy-boto3-mobile-1.28.15.post1/mypy_boto3_mobile/type_defs.pyi` & `mypy-boto3-mobile-1.28.16/mypy_boto3_mobile/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for mobile service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mobile/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_mobile.type_defs import BundleDetailsTypeDef
+    from mypy_boto3_mobile.type_defs import BlobTypeDef
 
-    data: BundleDetailsTypeDef = {...}
+    data: BlobTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Union
 
 from botocore.response import StreamingBody
@@ -21,27 +21,28 @@
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
+    "BlobTypeDef",
     "BundleDetailsTypeDef",
-    "CreateProjectRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "DeleteProjectRequestRequestTypeDef",
     "ResourceTypeDef",
     "DescribeBundleRequestRequestTypeDef",
     "DescribeProjectRequestRequestTypeDef",
     "ExportBundleRequestRequestTypeDef",
     "ExportProjectRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "ListBundlesRequestRequestTypeDef",
     "ListProjectsRequestRequestTypeDef",
     "ProjectSummaryTypeDef",
+    "CreateProjectRequestRequestTypeDef",
     "UpdateProjectRequestRequestTypeDef",
     "DescribeBundleResultTypeDef",
     "ExportBundleResultTypeDef",
     "ExportProjectResultTypeDef",
     "ListBundlesResultTypeDef",
     "DeleteProjectResultTypeDef",
     "ProjectDetailsTypeDef",
@@ -49,38 +50,28 @@
     "ListProjectsRequestListProjectsPaginateTypeDef",
     "ListProjectsResultTypeDef",
     "CreateProjectResultTypeDef",
     "DescribeProjectResultTypeDef",
     "UpdateProjectResultTypeDef",
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 BundleDetailsTypeDef = TypedDict(
     "BundleDetailsTypeDef",
     {
         "bundleId": str,
         "title": str,
         "version": str,
         "description": str,
         "iconUrl": str,
         "availablePlatforms": List[PlatformType],
     },
     total=False,
 )
 
-CreateProjectRequestRequestTypeDef = TypedDict(
-    "CreateProjectRequestRequestTypeDef",
-    {
-        "name": str,
-        "region": str,
-        "contents": Union[str, bytes, IO[Any], StreamingBody],
-        "snapshotId": str,
-    },
-    total=False,
-)
-
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -193,24 +184,35 @@
     {
         "name": str,
         "projectId": str,
     },
     total=False,
 )
 
+CreateProjectRequestRequestTypeDef = TypedDict(
+    "CreateProjectRequestRequestTypeDef",
+    {
+        "name": str,
+        "region": str,
+        "contents": BlobTypeDef,
+        "snapshotId": str,
+    },
+    total=False,
+)
+
 _RequiredUpdateProjectRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateProjectRequestRequestTypeDef",
     {
         "projectId": str,
     },
 )
 _OptionalUpdateProjectRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateProjectRequestRequestTypeDef",
     {
-        "contents": Union[str, bytes, IO[Any], StreamingBody],
+        "contents": BlobTypeDef,
     },
     total=False,
 )
 
 class UpdateProjectRequestRequestTypeDef(
     _RequiredUpdateProjectRequestRequestTypeDef, _OptionalUpdateProjectRequestRequestTypeDef
 ):
```

### Comparing `mypy-boto3-mobile-1.28.15.post1/mypy_boto3_mobile.egg-info/PKG-INFO` & `mypy-boto3-mobile-1.28.16/mypy_boto3_mobile.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mobile
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.Mobile 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.Mobile 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mobile/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 mobile type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 mobile type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mobile.svg?color=blue)](https://pypi.org/project/mypy-boto3-mobile)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mobile/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mobile)](https://pepy.tech/project/mypy-boto3-mobile)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Mobile 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mobile.html#Mobile)
+[boto3.Mobile 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mobile.html#Mobile)
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
 [mypy-boto3-mobile docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mobile/).
 
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
@@ -312,36 +312,37 @@
 )
 
 
 def check_value(value: ListBundlesPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_mobile.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_mobile.type_defs import (
+    BlobTypeDef,
     BundleDetailsTypeDef,
-    CreateProjectRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     DeleteProjectRequestRequestTypeDef,
     ResourceTypeDef,
     DescribeBundleRequestRequestTypeDef,
     DescribeProjectRequestRequestTypeDef,
     ExportBundleRequestRequestTypeDef,
     ExportProjectRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     ListBundlesRequestRequestTypeDef,
     ListProjectsRequestRequestTypeDef,
     ProjectSummaryTypeDef,
+    CreateProjectRequestRequestTypeDef,
     UpdateProjectRequestRequestTypeDef,
     DescribeBundleResultTypeDef,
     ExportBundleResultTypeDef,
     ExportProjectResultTypeDef,
     ListBundlesResultTypeDef,
     DeleteProjectResultTypeDef,
     ProjectDetailsTypeDef,
@@ -350,15 +351,15 @@
     ListProjectsResultTypeDef,
     CreateProjectResultTypeDef,
     DescribeProjectResultTypeDef,
     UpdateProjectResultTypeDef,
 )
 
 
-def get_structure() -> BundleDetailsTypeDef:
+def get_value() -> BlobTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-mobile-1.28.15.post1/mypy_boto3_mobile.egg-info/SOURCES.txt` & `mypy-boto3-mobile-1.28.16/mypy_boto3_mobile.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mobile-1.28.15.post1/setup.py` & `mypy-boto3-mobile-1.28.16/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-mobile",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_mobile"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Mobile 1.28.15 service generated with mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.Mobile 1.28.16 service generated with mypy-boto3-builder 7.17.1"
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
-    keywords="boto3 mobile type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 mobile type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_mobile": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mobile/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

