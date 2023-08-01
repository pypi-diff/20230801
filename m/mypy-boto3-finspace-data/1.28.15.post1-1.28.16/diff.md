# Comparing `tmp/mypy-boto3-finspace-data-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-finspace-data-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-finspace-data-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:08 2023, max compression
+gzip compressed data, was "mypy-boto3-finspace-data-1.28.16.tar", last modified: Tue Aug  1 11:36:48 2023, max compression
```

## Comparing `mypy-boto3-finspace-data-1.28.15.post1.tar` & `mypy-boto3-finspace-data-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:08.061150 mypy-boto3-finspace-data-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:45:22.000000 mypy-boto3-finspace-data-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17310 2023-07-29 10:03:08.057150 mypy-boto3-finspace-data-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15794 2023-07-29 09:45:22.000000 mypy-boto3-finspace-data-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:08.045150 mypy-boto3-finspace-data-1.28.15.post1/mypy_boto3_finspace_data/
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-07-29 09:45:22.000000 mypy-boto3-finspace-data-1.28.15.post1/mypy_boto3_finspace_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-07-29 09:45:22.000000 mypy-boto3-finspace-data-1.28.15.post1/mypy_boto3_finspace_data/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-29 09:45:22.000000 mypy-boto3-finspace-data-1.28.15.post1/mypy_boto3_finspace_data/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25464 2023-07-29 09:45:22.000000 mypy-boto3-finspace-data-1.28.15.post1/mypy_boto3_finspace_data/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    25421 2023-07-29 09:45:22.000000 mypy-boto3-finspace-data-1.28.15.post1/mypy_boto3_finspace_data/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10153 2023-07-29 09:45:22.000000 mypy-boto3-finspace-data-1.28.15.post1/mypy_boto3_finspace_data/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10151 2023-07-29 09:45:22.000000 mypy-boto3-finspace-data-1.28.15.post1/mypy_boto3_finspace_data/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-07-29 09:45:22.000000 mypy-boto3-finspace-data-1.28.15.post1/mypy_boto3_finspace_data/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6100 2023-07-29 09:45:22.000000 mypy-boto3-finspace-data-1.28.15.post1/mypy_boto3_finspace_data/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:45:22.000000 mypy-boto3-finspace-data-1.28.15.post1/mypy_boto3_finspace_data/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    35600 2023-07-29 09:45:23.000000 mypy-boto3-finspace-data-1.28.15.post1/mypy_boto3_finspace_data/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    35545 2023-07-29 09:45:23.000000 mypy-boto3-finspace-data-1.28.15.post1/mypy_boto3_finspace_data/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:45:22.000000 mypy-boto3-finspace-data-1.28.15.post1/mypy_boto3_finspace_data/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:08.057150 mypy-boto3-finspace-data-1.28.15.post1/mypy_boto3_finspace_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17310 2023-07-29 10:03:07.000000 mypy-boto3-finspace-data-1.28.15.post1/mypy_boto3_finspace_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-29 10:03:07.000000 mypy-boto3-finspace-data-1.28.15.post1/mypy_boto3_finspace_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:07.000000 mypy-boto3-finspace-data-1.28.15.post1/mypy_boto3_finspace_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:07.000000 mypy-boto3-finspace-data-1.28.15.post1/mypy_boto3_finspace_data.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:07.000000 mypy-boto3-finspace-data-1.28.15.post1/mypy_boto3_finspace_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-29 10:03:07.000000 mypy-boto3-finspace-data-1.28.15.post1/mypy_boto3_finspace_data.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:08.061150 mypy-boto3-finspace-data-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-07-29 09:45:22.000000 mypy-boto3-finspace-data-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:48.412889 mypy-boto3-finspace-data-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:17:58.000000 mypy-boto3-finspace-data-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17376 2023-08-01 11:36:48.412889 mypy-boto3-finspace-data-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15869 2023-08-01 11:17:58.000000 mypy-boto3-finspace-data-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:48.392889 mypy-boto3-finspace-data-1.28.16/mypy_boto3_finspace_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-08-01 11:17:58.000000 mypy-boto3-finspace-data-1.28.16/mypy_boto3_finspace_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-08-01 11:17:58.000000 mypy-boto3-finspace-data-1.28.16/mypy_boto3_finspace_data/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-08-01 11:17:58.000000 mypy-boto3-finspace-data-1.28.16/mypy_boto3_finspace_data/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25265 2023-08-01 11:17:58.000000 mypy-boto3-finspace-data-1.28.16/mypy_boto3_finspace_data/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25222 2023-08-01 11:17:58.000000 mypy-boto3-finspace-data-1.28.16/mypy_boto3_finspace_data/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10153 2023-08-01 11:17:59.000000 mypy-boto3-finspace-data-1.28.16/mypy_boto3_finspace_data/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10151 2023-08-01 11:17:58.000000 mypy-boto3-finspace-data-1.28.16/mypy_boto3_finspace_data/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-08-01 11:17:58.000000 mypy-boto3-finspace-data-1.28.16/mypy_boto3_finspace_data/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6100 2023-08-01 11:17:58.000000 mypy-boto3-finspace-data-1.28.16/mypy_boto3_finspace_data/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:17:58.000000 mypy-boto3-finspace-data-1.28.16/mypy_boto3_finspace_data/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    35901 2023-08-01 11:18:00.000000 mypy-boto3-finspace-data-1.28.16/mypy_boto3_finspace_data/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35846 2023-08-01 11:17:59.000000 mypy-boto3-finspace-data-1.28.16/mypy_boto3_finspace_data/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:17:58.000000 mypy-boto3-finspace-data-1.28.16/mypy_boto3_finspace_data/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:48.412889 mypy-boto3-finspace-data-1.28.16/mypy_boto3_finspace_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17376 2023-08-01 11:36:48.000000 mypy-boto3-finspace-data-1.28.16/mypy_boto3_finspace_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-08-01 11:36:48.000000 mypy-boto3-finspace-data-1.28.16/mypy_boto3_finspace_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:48.000000 mypy-boto3-finspace-data-1.28.16/mypy_boto3_finspace_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:48.000000 mypy-boto3-finspace-data-1.28.16/mypy_boto3_finspace_data.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:48.000000 mypy-boto3-finspace-data-1.28.16/mypy_boto3_finspace_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-01 11:36:48.000000 mypy-boto3-finspace-data-1.28.16/mypy_boto3_finspace_data.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:48.412889 mypy-boto3-finspace-data-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-08-01 11:17:58.000000 mypy-boto3-finspace-data-1.28.16/setup.py
```

### Comparing `mypy-boto3-finspace-data-1.28.15.post1/LICENSE` & `mypy-boto3-finspace-data-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-finspace-data-1.28.15.post1/PKG-INFO` & `mypy-boto3-finspace-data-1.28.16/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-finspace-data
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.FinSpaceData 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.FinSpaceData 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace_data/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 finspace-data type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 finspace-data type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-finspace-data.svg?color=blue)](https://pypi.org/project/mypy-boto3-finspace-data)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace_data/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-finspace-data)](https://pepy.tech/project/mypy-boto3-finspace-data)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.FinSpaceData 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData)
+[boto3.FinSpaceData 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData)
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
 [mypy-boto3-finspace-data docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace_data/).
 
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
@@ -340,20 +340,20 @@
 )
 
 
 def check_value(value: ApiAccessType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_finspace_data.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_finspace_data.type_defs import (
     AssociateUserToPermissionGroupRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     AwsCredentialsTypeDef,
     ChangesetErrorInfoTypeDef,
@@ -417,14 +417,15 @@
     UpdateUserResponseTypeDef,
     ChangesetSummaryTypeDef,
     GetChangesetResponseTypeDef,
     SchemaDefinitionOutputTypeDef,
     SchemaDefinitionTypeDef,
     CreateDataViewRequestRequestTypeDef,
     GetProgrammaticAccessCredentialsResponseTypeDef,
+    DataViewDestinationTypeParamsUnionTypeDef,
     DataViewSummaryTypeDef,
     GetDataViewResponseTypeDef,
     GetExternalDataViewAccessDetailsResponseTypeDef,
     GetPermissionGroupResponseTypeDef,
     ListPermissionGroupsResponseTypeDef,
     ListChangesetsRequestListChangesetsPaginateTypeDef,
     ListDataViewsRequestListDataViewsPaginateTypeDef,
@@ -438,20 +439,21 @@
     ListChangesetsResponseTypeDef,
     SchemaUnionOutputTypeDef,
     SchemaUnionTypeDef,
     ListDataViewsResponseTypeDef,
     DatasetTypeDef,
     GetDatasetResponseTypeDef,
     CreateDatasetRequestRequestTypeDef,
+    SchemaUnionUnionTypeDef,
     UpdateDatasetRequestRequestTypeDef,
     ListDatasetsResponseTypeDef,
 )
 
 
-def get_structure() -> AssociateUserToPermissionGroupRequestRequestTypeDef:
+def get_value() -> AssociateUserToPermissionGroupRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-finspace-data-1.28.15.post1/README.md` & `mypy-boto3-finspace-data-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-finspace-data.svg?color=blue)](https://pypi.org/project/mypy-boto3-finspace-data)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace_data/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-finspace-data)](https://pepy.tech/project/mypy-boto3-finspace-data)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.FinSpaceData 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData)
+[boto3.FinSpaceData 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData)
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
 [mypy-boto3-finspace-data docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace_data/).
 
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
@@ -308,20 +308,20 @@
 )
 
 
 def check_value(value: ApiAccessType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_finspace_data.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_finspace_data.type_defs import (
     AssociateUserToPermissionGroupRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     AwsCredentialsTypeDef,
     ChangesetErrorInfoTypeDef,
@@ -385,14 +385,15 @@
     UpdateUserResponseTypeDef,
     ChangesetSummaryTypeDef,
     GetChangesetResponseTypeDef,
     SchemaDefinitionOutputTypeDef,
     SchemaDefinitionTypeDef,
     CreateDataViewRequestRequestTypeDef,
     GetProgrammaticAccessCredentialsResponseTypeDef,
+    DataViewDestinationTypeParamsUnionTypeDef,
     DataViewSummaryTypeDef,
     GetDataViewResponseTypeDef,
     GetExternalDataViewAccessDetailsResponseTypeDef,
     GetPermissionGroupResponseTypeDef,
     ListPermissionGroupsResponseTypeDef,
     ListChangesetsRequestListChangesetsPaginateTypeDef,
     ListDataViewsRequestListDataViewsPaginateTypeDef,
@@ -406,20 +407,21 @@
     ListChangesetsResponseTypeDef,
     SchemaUnionOutputTypeDef,
     SchemaUnionTypeDef,
     ListDataViewsResponseTypeDef,
     DatasetTypeDef,
     GetDatasetResponseTypeDef,
     CreateDatasetRequestRequestTypeDef,
+    SchemaUnionUnionTypeDef,
     UpdateDatasetRequestRequestTypeDef,
     ListDatasetsResponseTypeDef,
 )
 
 
-def get_structure() -> AssociateUserToPermissionGroupRequestRequestTypeDef:
+def get_value() -> AssociateUserToPermissionGroupRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-finspace-data-1.28.15.post1/mypy_boto3_finspace_data/__init__.py` & `mypy-boto3-finspace-data-1.28.16/mypy_boto3_finspace_data/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-finspace-data-1.28.15.post1/mypy_boto3_finspace_data/__init__.pyi` & `mypy-boto3-finspace-data-1.28.16/mypy_boto3_finspace_data/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-finspace-data-1.28.15.post1/mypy_boto3_finspace_data/__main__.py` & `mypy-boto3-finspace-data-1.28.16/mypy_boto3_finspace_data/__main__.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.FinSpaceData 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.FinSpaceData 1.28.16\nVersion:         1.28.16\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace_data//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData\nOther"
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

### Comparing `mypy-boto3-finspace-data-1.28.15.post1/mypy_boto3_finspace_data/client.py` & `mypy-boto3-finspace-data-1.28.16/mypy_boto3_finspace_data/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_finspace_data.client import FinSpaceDataClient
 
     session = Session()
     client: FinSpaceDataClient = session.client("finspace-data")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     ApiAccessType,
     ApplicationPermissionType,
     ChangeTypeType,
@@ -37,16 +37,15 @@
     AssociateUserToPermissionGroupResponseTypeDef,
     CreateChangesetResponseTypeDef,
     CreateDatasetResponseTypeDef,
     CreateDataViewResponseTypeDef,
     CreatePermissionGroupResponseTypeDef,
     CreateUserResponseTypeDef,
     DatasetOwnerInfoTypeDef,
-    DataViewDestinationTypeParamsOutputTypeDef,
-    DataViewDestinationTypeParamsTypeDef,
+    DataViewDestinationTypeParamsUnionTypeDef,
     DeleteDatasetResponseTypeDef,
     DeletePermissionGroupResponseTypeDef,
     DisableUserResponseTypeDef,
     DisassociateUserFromPermissionGroupResponseTypeDef,
     EnableUserResponseTypeDef,
     GetChangesetResponseTypeDef,
     GetDatasetResponseTypeDef,
@@ -61,16 +60,15 @@
     ListDataViewsResponseTypeDef,
     ListPermissionGroupsByUserResponseTypeDef,
     ListPermissionGroupsResponseTypeDef,
     ListUsersByPermissionGroupResponseTypeDef,
     ListUsersResponseTypeDef,
     PermissionGroupParamsTypeDef,
     ResetUserPasswordResponseTypeDef,
-    SchemaUnionOutputTypeDef,
-    SchemaUnionTypeDef,
+    SchemaUnionUnionTypeDef,
     UpdateChangesetResponseTypeDef,
     UpdateDatasetResponseTypeDef,
     UpdatePermissionGroupResponseTypeDef,
     UpdateUserResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
@@ -161,17 +159,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace_data/client/#create_changeset)
         """
 
     def create_data_view(
         self,
         *,
         datasetId: str,
-        destinationTypeParams: Union[
-            DataViewDestinationTypeParamsTypeDef, DataViewDestinationTypeParamsOutputTypeDef
-        ],
+        destinationTypeParams: DataViewDestinationTypeParamsUnionTypeDef,
         clientToken: str = ...,
         autoUpdate: bool = ...,
         sortColumns: Sequence[str] = ...,
         partitionColumns: Sequence[str] = ...,
         asOfTimestamp: int = ...
     ) -> CreateDataViewResponseTypeDef:
         """
@@ -187,15 +183,15 @@
         datasetTitle: str,
         kind: DatasetKindType,
         permissionGroupParams: PermissionGroupParamsTypeDef,
         clientToken: str = ...,
         datasetDescription: str = ...,
         ownerInfo: DatasetOwnerInfoTypeDef = ...,
         alias: str = ...,
-        schemaDefinition: Union[SchemaUnionTypeDef, SchemaUnionOutputTypeDef] = ...
+        schemaDefinition: SchemaUnionUnionTypeDef = ...
     ) -> CreateDatasetResponseTypeDef:
         """
         Creates a new FinSpace Dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData.Client.create_dataset)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace_data/client/#create_dataset)
         """
@@ -465,15 +461,15 @@
         *,
         datasetId: str,
         datasetTitle: str,
         kind: DatasetKindType,
         clientToken: str = ...,
         datasetDescription: str = ...,
         alias: str = ...,
-        schemaDefinition: Union[SchemaUnionTypeDef, SchemaUnionOutputTypeDef] = ...
+        schemaDefinition: SchemaUnionUnionTypeDef = ...
     ) -> UpdateDatasetResponseTypeDef:
         """
         Updates a FinSpace Dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData.Client.update_dataset)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace_data/client/#update_dataset)
         """
```

### Comparing `mypy-boto3-finspace-data-1.28.15.post1/mypy_boto3_finspace_data/client.pyi` & `mypy-boto3-finspace-data-1.28.16/mypy_boto3_finspace_data/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_finspace_data.client import FinSpaceDataClient
 
     session = Session()
     client: FinSpaceDataClient = session.client("finspace-data")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     ApiAccessType,
     ApplicationPermissionType,
     ChangeTypeType,
@@ -37,16 +37,15 @@
     AssociateUserToPermissionGroupResponseTypeDef,
     CreateChangesetResponseTypeDef,
     CreateDatasetResponseTypeDef,
     CreateDataViewResponseTypeDef,
     CreatePermissionGroupResponseTypeDef,
     CreateUserResponseTypeDef,
     DatasetOwnerInfoTypeDef,
-    DataViewDestinationTypeParamsOutputTypeDef,
-    DataViewDestinationTypeParamsTypeDef,
+    DataViewDestinationTypeParamsUnionTypeDef,
     DeleteDatasetResponseTypeDef,
     DeletePermissionGroupResponseTypeDef,
     DisableUserResponseTypeDef,
     DisassociateUserFromPermissionGroupResponseTypeDef,
     EnableUserResponseTypeDef,
     GetChangesetResponseTypeDef,
     GetDatasetResponseTypeDef,
@@ -61,16 +60,15 @@
     ListDataViewsResponseTypeDef,
     ListPermissionGroupsByUserResponseTypeDef,
     ListPermissionGroupsResponseTypeDef,
     ListUsersByPermissionGroupResponseTypeDef,
     ListUsersResponseTypeDef,
     PermissionGroupParamsTypeDef,
     ResetUserPasswordResponseTypeDef,
-    SchemaUnionOutputTypeDef,
-    SchemaUnionTypeDef,
+    SchemaUnionUnionTypeDef,
     UpdateChangesetResponseTypeDef,
     UpdateDatasetResponseTypeDef,
     UpdatePermissionGroupResponseTypeDef,
     UpdateUserResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
@@ -152,17 +150,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData.Client.create_changeset)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace_data/client/#create_changeset)
         """
     def create_data_view(
         self,
         *,
         datasetId: str,
-        destinationTypeParams: Union[
-            DataViewDestinationTypeParamsTypeDef, DataViewDestinationTypeParamsOutputTypeDef
-        ],
+        destinationTypeParams: DataViewDestinationTypeParamsUnionTypeDef,
         clientToken: str = ...,
         autoUpdate: bool = ...,
         sortColumns: Sequence[str] = ...,
         partitionColumns: Sequence[str] = ...,
         asOfTimestamp: int = ...
     ) -> CreateDataViewResponseTypeDef:
         """
@@ -177,15 +173,15 @@
         datasetTitle: str,
         kind: DatasetKindType,
         permissionGroupParams: PermissionGroupParamsTypeDef,
         clientToken: str = ...,
         datasetDescription: str = ...,
         ownerInfo: DatasetOwnerInfoTypeDef = ...,
         alias: str = ...,
-        schemaDefinition: Union[SchemaUnionTypeDef, SchemaUnionOutputTypeDef] = ...
+        schemaDefinition: SchemaUnionUnionTypeDef = ...
     ) -> CreateDatasetResponseTypeDef:
         """
         Creates a new FinSpace Dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData.Client.create_dataset)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace_data/client/#create_dataset)
         """
@@ -429,15 +425,15 @@
         *,
         datasetId: str,
         datasetTitle: str,
         kind: DatasetKindType,
         clientToken: str = ...,
         datasetDescription: str = ...,
         alias: str = ...,
-        schemaDefinition: Union[SchemaUnionTypeDef, SchemaUnionOutputTypeDef] = ...
+        schemaDefinition: SchemaUnionUnionTypeDef = ...
     ) -> UpdateDatasetResponseTypeDef:
         """
         Updates a FinSpace Dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData.Client.update_dataset)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace_data/client/#update_dataset)
         """
```

### Comparing `mypy-boto3-finspace-data-1.28.15.post1/mypy_boto3_finspace_data/literals.py` & `mypy-boto3-finspace-data-1.28.16/mypy_boto3_finspace_data/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-finspace-data-1.28.15.post1/mypy_boto3_finspace_data/literals.pyi` & `mypy-boto3-finspace-data-1.28.16/mypy_boto3_finspace_data/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-finspace-data-1.28.15.post1/mypy_boto3_finspace_data/paginator.py` & `mypy-boto3-finspace-data-1.28.16/mypy_boto3_finspace_data/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-finspace-data-1.28.15.post1/mypy_boto3_finspace_data/paginator.pyi` & `mypy-boto3-finspace-data-1.28.16/mypy_boto3_finspace_data/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-finspace-data-1.28.15.post1/mypy_boto3_finspace_data/type_defs.py` & `mypy-boto3-finspace-data-1.28.16/mypy_boto3_finspace_data/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace_data/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_finspace_data.type_defs import AssociateUserToPermissionGroupRequestRequestTypeDef
 
-    data: AssociateUserToPermissionGroupRequestRequestTypeDef = {...}
+    data: AssociateUserToPermissionGroupRequestRequestTypeDef = ...
     ```
 """
 import sys
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     ApiAccessType,
     ApplicationPermissionType,
     ChangeTypeType,
     ColumnDataTypeType,
     DatasetKindType,
@@ -102,14 +102,15 @@
     "UpdateUserResponseTypeDef",
     "ChangesetSummaryTypeDef",
     "GetChangesetResponseTypeDef",
     "SchemaDefinitionOutputTypeDef",
     "SchemaDefinitionTypeDef",
     "CreateDataViewRequestRequestTypeDef",
     "GetProgrammaticAccessCredentialsResponseTypeDef",
+    "DataViewDestinationTypeParamsUnionTypeDef",
     "DataViewSummaryTypeDef",
     "GetDataViewResponseTypeDef",
     "GetExternalDataViewAccessDetailsResponseTypeDef",
     "GetPermissionGroupResponseTypeDef",
     "ListPermissionGroupsResponseTypeDef",
     "ListChangesetsRequestListChangesetsPaginateTypeDef",
     "ListDataViewsRequestListDataViewsPaginateTypeDef",
@@ -123,14 +124,15 @@
     "ListChangesetsResponseTypeDef",
     "SchemaUnionOutputTypeDef",
     "SchemaUnionTypeDef",
     "ListDataViewsResponseTypeDef",
     "DatasetTypeDef",
     "GetDatasetResponseTypeDef",
     "CreateDatasetRequestRequestTypeDef",
+    "SchemaUnionUnionTypeDef",
     "UpdateDatasetRequestRequestTypeDef",
     "ListDatasetsResponseTypeDef",
 )
 
 _RequiredAssociateUserToPermissionGroupRequestRequestTypeDef = TypedDict(
     "_RequiredAssociateUserToPermissionGroupRequestRequestTypeDef",
     {
@@ -1101,14 +1103,17 @@
     {
         "credentials": CredentialsTypeDef,
         "durationInMinutes": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DataViewDestinationTypeParamsUnionTypeDef = Union[
+    DataViewDestinationTypeParamsTypeDef, DataViewDestinationTypeParamsOutputTypeDef
+]
 DataViewSummaryTypeDef = TypedDict(
     "DataViewSummaryTypeDef",
     {
         "dataViewId": str,
         "dataViewArn": str,
         "datasetId": str,
         "asOfTimestamp": int,
@@ -1364,14 +1369,15 @@
 
 class CreateDatasetRequestRequestTypeDef(
     _RequiredCreateDatasetRequestRequestTypeDef, _OptionalCreateDatasetRequestRequestTypeDef
 ):
     pass
 
 
+SchemaUnionUnionTypeDef = Union[SchemaUnionTypeDef, SchemaUnionOutputTypeDef]
 _RequiredUpdateDatasetRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDatasetRequestRequestTypeDef",
     {
         "datasetId": str,
         "datasetTitle": str,
         "kind": DatasetKindType,
     },
```

### Comparing `mypy-boto3-finspace-data-1.28.15.post1/mypy_boto3_finspace_data/type_defs.pyi` & `mypy-boto3-finspace-data-1.28.16/mypy_boto3_finspace_data/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace_data/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_finspace_data.type_defs import AssociateUserToPermissionGroupRequestRequestTypeDef
 
-    data: AssociateUserToPermissionGroupRequestRequestTypeDef = {...}
+    data: AssociateUserToPermissionGroupRequestRequestTypeDef = ...
     ```
 """
 import sys
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     ApiAccessType,
     ApplicationPermissionType,
     ChangeTypeType,
     ColumnDataTypeType,
     DatasetKindType,
@@ -101,14 +101,15 @@
     "UpdateUserResponseTypeDef",
     "ChangesetSummaryTypeDef",
     "GetChangesetResponseTypeDef",
     "SchemaDefinitionOutputTypeDef",
     "SchemaDefinitionTypeDef",
     "CreateDataViewRequestRequestTypeDef",
     "GetProgrammaticAccessCredentialsResponseTypeDef",
+    "DataViewDestinationTypeParamsUnionTypeDef",
     "DataViewSummaryTypeDef",
     "GetDataViewResponseTypeDef",
     "GetExternalDataViewAccessDetailsResponseTypeDef",
     "GetPermissionGroupResponseTypeDef",
     "ListPermissionGroupsResponseTypeDef",
     "ListChangesetsRequestListChangesetsPaginateTypeDef",
     "ListDataViewsRequestListDataViewsPaginateTypeDef",
@@ -122,14 +123,15 @@
     "ListChangesetsResponseTypeDef",
     "SchemaUnionOutputTypeDef",
     "SchemaUnionTypeDef",
     "ListDataViewsResponseTypeDef",
     "DatasetTypeDef",
     "GetDatasetResponseTypeDef",
     "CreateDatasetRequestRequestTypeDef",
+    "SchemaUnionUnionTypeDef",
     "UpdateDatasetRequestRequestTypeDef",
     "ListDatasetsResponseTypeDef",
 )
 
 _RequiredAssociateUserToPermissionGroupRequestRequestTypeDef = TypedDict(
     "_RequiredAssociateUserToPermissionGroupRequestRequestTypeDef",
     {
@@ -1054,14 +1056,17 @@
     {
         "credentials": CredentialsTypeDef,
         "durationInMinutes": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DataViewDestinationTypeParamsUnionTypeDef = Union[
+    DataViewDestinationTypeParamsTypeDef, DataViewDestinationTypeParamsOutputTypeDef
+]
 DataViewSummaryTypeDef = TypedDict(
     "DataViewSummaryTypeDef",
     {
         "dataViewId": str,
         "dataViewArn": str,
         "datasetId": str,
         "asOfTimestamp": int,
@@ -1311,14 +1316,15 @@
 )
 
 class CreateDatasetRequestRequestTypeDef(
     _RequiredCreateDatasetRequestRequestTypeDef, _OptionalCreateDatasetRequestRequestTypeDef
 ):
     pass
 
+SchemaUnionUnionTypeDef = Union[SchemaUnionTypeDef, SchemaUnionOutputTypeDef]
 _RequiredUpdateDatasetRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDatasetRequestRequestTypeDef",
     {
         "datasetId": str,
         "datasetTitle": str,
         "kind": DatasetKindType,
     },
```

### Comparing `mypy-boto3-finspace-data-1.28.15.post1/mypy_boto3_finspace_data.egg-info/PKG-INFO` & `mypy-boto3-finspace-data-1.28.16/mypy_boto3_finspace_data.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-finspace-data
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.FinSpaceData 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.FinSpaceData 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace_data/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 finspace-data type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 finspace-data type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-finspace-data.svg?color=blue)](https://pypi.org/project/mypy-boto3-finspace-data)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace_data/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-finspace-data)](https://pepy.tech/project/mypy-boto3-finspace-data)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.FinSpaceData 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData)
+[boto3.FinSpaceData 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData)
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
 [mypy-boto3-finspace-data docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace_data/).
 
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
@@ -340,20 +340,20 @@
 )
 
 
 def check_value(value: ApiAccessType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_finspace_data.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_finspace_data.type_defs import (
     AssociateUserToPermissionGroupRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     AwsCredentialsTypeDef,
     ChangesetErrorInfoTypeDef,
@@ -417,14 +417,15 @@
     UpdateUserResponseTypeDef,
     ChangesetSummaryTypeDef,
     GetChangesetResponseTypeDef,
     SchemaDefinitionOutputTypeDef,
     SchemaDefinitionTypeDef,
     CreateDataViewRequestRequestTypeDef,
     GetProgrammaticAccessCredentialsResponseTypeDef,
+    DataViewDestinationTypeParamsUnionTypeDef,
     DataViewSummaryTypeDef,
     GetDataViewResponseTypeDef,
     GetExternalDataViewAccessDetailsResponseTypeDef,
     GetPermissionGroupResponseTypeDef,
     ListPermissionGroupsResponseTypeDef,
     ListChangesetsRequestListChangesetsPaginateTypeDef,
     ListDataViewsRequestListDataViewsPaginateTypeDef,
@@ -438,20 +439,21 @@
     ListChangesetsResponseTypeDef,
     SchemaUnionOutputTypeDef,
     SchemaUnionTypeDef,
     ListDataViewsResponseTypeDef,
     DatasetTypeDef,
     GetDatasetResponseTypeDef,
     CreateDatasetRequestRequestTypeDef,
+    SchemaUnionUnionTypeDef,
     UpdateDatasetRequestRequestTypeDef,
     ListDatasetsResponseTypeDef,
 )
 
 
-def get_structure() -> AssociateUserToPermissionGroupRequestRequestTypeDef:
+def get_value() -> AssociateUserToPermissionGroupRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-finspace-data-1.28.15.post1/mypy_boto3_finspace_data.egg-info/SOURCES.txt` & `mypy-boto3-finspace-data-1.28.16/mypy_boto3_finspace_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-finspace-data-1.28.15.post1/setup.py` & `mypy-boto3-finspace-data-1.28.16/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-finspace-data",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_finspace_data"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.FinSpaceData 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.2"
+        "Type annotations for boto3.FinSpaceData 1.28.16 service generated with mypy-boto3-builder"
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
-    keywords="boto3 finspace-data type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 finspace-data type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_finspace_data": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace_data/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

