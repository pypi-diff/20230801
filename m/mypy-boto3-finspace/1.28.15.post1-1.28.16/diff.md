# Comparing `tmp/mypy-boto3-finspace-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-finspace-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-finspace-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:09 2023, max compression
+gzip compressed data, was "mypy-boto3-finspace-1.28.16.tar", last modified: Tue Aug  1 11:36:49 2023, max compression
```

## Comparing `mypy-boto3-finspace-1.28.15.post1.tar` & `mypy-boto3-finspace-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:09.085153 mypy-boto3-finspace-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:45:18.000000 mypy-boto3-finspace-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16231 2023-07-29 10:03:09.077153 mypy-boto3-finspace-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14734 2023-07-29 09:45:18.000000 mypy-boto3-finspace-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:09.073153 mypy-boto3-finspace-1.28.15.post1/mypy_boto3_finspace/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-29 09:45:18.000000 mypy-boto3-finspace-1.28.15.post1/mypy_boto3_finspace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-29 09:45:18.000000 mypy-boto3-finspace-1.28.15.post1/mypy_boto3_finspace/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-29 09:45:18.000000 mypy-boto3-finspace-1.28.15.post1/mypy_boto3_finspace/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25141 2023-07-29 09:45:18.000000 mypy-boto3-finspace-1.28.15.post1/mypy_boto3_finspace/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    25099 2023-07-29 09:45:18.000000 mypy-boto3-finspace-1.28.15.post1/mypy_boto3_finspace/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9772 2023-07-29 09:45:18.000000 mypy-boto3-finspace-1.28.15.post1/mypy_boto3_finspace/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9770 2023-07-29 09:45:18.000000 mypy-boto3-finspace-1.28.15.post1/mypy_boto3_finspace/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-07-29 09:45:18.000000 mypy-boto3-finspace-1.28.15.post1/mypy_boto3_finspace/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-07-29 09:45:18.000000 mypy-boto3-finspace-1.28.15.post1/mypy_boto3_finspace/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:45:18.000000 mypy-boto3-finspace-1.28.15.post1/mypy_boto3_finspace/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    36543 2023-07-29 09:45:21.000000 mypy-boto3-finspace-1.28.15.post1/mypy_boto3_finspace/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    36503 2023-07-29 09:45:19.000000 mypy-boto3-finspace-1.28.15.post1/mypy_boto3_finspace/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:45:18.000000 mypy-boto3-finspace-1.28.15.post1/mypy_boto3_finspace/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:09.077153 mypy-boto3-finspace-1.28.15.post1/mypy_boto3_finspace.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16231 2023-07-29 10:03:08.000000 mypy-boto3-finspace-1.28.15.post1/mypy_boto3_finspace.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-29 10:03:08.000000 mypy-boto3-finspace-1.28.15.post1/mypy_boto3_finspace.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:08.000000 mypy-boto3-finspace-1.28.15.post1/mypy_boto3_finspace.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:08.000000 mypy-boto3-finspace-1.28.15.post1/mypy_boto3_finspace.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:08.000000 mypy-boto3-finspace-1.28.15.post1/mypy_boto3_finspace.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-29 10:03:08.000000 mypy-boto3-finspace-1.28.15.post1/mypy_boto3_finspace.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:09.085153 mypy-boto3-finspace-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-07-29 09:45:18.000000 mypy-boto3-finspace-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:48.992888 mypy-boto3-finspace-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:17:54.000000 mypy-boto3-finspace-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16334 2023-08-01 11:36:48.992888 mypy-boto3-finspace-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14846 2023-08-01 11:17:54.000000 mypy-boto3-finspace-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:48.984888 mypy-boto3-finspace-1.28.16/mypy_boto3_finspace/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-08-01 11:17:54.000000 mypy-boto3-finspace-1.28.16/mypy_boto3_finspace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-08-01 11:17:54.000000 mypy-boto3-finspace-1.28.16/mypy_boto3_finspace/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-08-01 11:17:54.000000 mypy-boto3-finspace-1.28.16/mypy_boto3_finspace/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24758 2023-08-01 11:17:56.000000 mypy-boto3-finspace-1.28.16/mypy_boto3_finspace/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24716 2023-08-01 11:17:56.000000 mypy-boto3-finspace-1.28.16/mypy_boto3_finspace/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9772 2023-08-01 11:17:56.000000 mypy-boto3-finspace-1.28.16/mypy_boto3_finspace/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9770 2023-08-01 11:17:56.000000 mypy-boto3-finspace-1.28.16/mypy_boto3_finspace/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-08-01 11:17:56.000000 mypy-boto3-finspace-1.28.16/mypy_boto3_finspace/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-08-01 11:17:56.000000 mypy-boto3-finspace-1.28.16/mypy_boto3_finspace/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:17:54.000000 mypy-boto3-finspace-1.28.16/mypy_boto3_finspace/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    36860 2023-08-01 11:17:57.000000 mypy-boto3-finspace-1.28.16/mypy_boto3_finspace/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36820 2023-08-01 11:17:57.000000 mypy-boto3-finspace-1.28.16/mypy_boto3_finspace/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:17:54.000000 mypy-boto3-finspace-1.28.16/mypy_boto3_finspace/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:48.992888 mypy-boto3-finspace-1.28.16/mypy_boto3_finspace.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16334 2023-08-01 11:36:48.000000 mypy-boto3-finspace-1.28.16/mypy_boto3_finspace.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-08-01 11:36:48.000000 mypy-boto3-finspace-1.28.16/mypy_boto3_finspace.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:48.000000 mypy-boto3-finspace-1.28.16/mypy_boto3_finspace.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:48.000000 mypy-boto3-finspace-1.28.16/mypy_boto3_finspace.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:48.000000 mypy-boto3-finspace-1.28.16/mypy_boto3_finspace.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-01 11:36:48.000000 mypy-boto3-finspace-1.28.16/mypy_boto3_finspace.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:48.992888 mypy-boto3-finspace-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-08-01 11:17:54.000000 mypy-boto3-finspace-1.28.16/setup.py
```

### Comparing `mypy-boto3-finspace-1.28.15.post1/LICENSE` & `mypy-boto3-finspace-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-finspace-1.28.15.post1/PKG-INFO` & `mypy-boto3-finspace-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-finspace
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.finspace 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.finspace 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 finspace type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 finspace type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-finspace.svg?color=blue)](https://pypi.org/project/mypy-boto3-finspace)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-finspace)](https://pepy.tech/project/mypy-boto3-finspace)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.finspace 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace)
+[boto3.finspace 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace)
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
 [mypy-boto3-finspace docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/).
 
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
@@ -324,20 +324,20 @@
 )
 
 
 def check_value(value: AutoScalingMetricType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_finspace.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_finspace.type_defs import (
     AutoScalingConfigurationTypeDef,
     CapacityConfigurationTypeDef,
     ChangeRequestTypeDef,
     CodeConfigurationTypeDef,
@@ -400,15 +400,17 @@
     GetKxDatabaseResponseTypeDef,
     GetKxUserResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     UpdateKxDatabaseResponseTypeDef,
     UpdateKxUserResponseTypeDef,
     CreateKxChangesetResponseTypeDef,
     GetKxChangesetResponseTypeDef,
+    VpcConfigurationUnionTypeDef,
     EnvironmentTypeDef,
+    FederationParametersUnionTypeDef,
     GetKxEnvironmentResponseTypeDef,
     KxEnvironmentTypeDef,
     UpdateKxEnvironmentNetworkRequestRequestTypeDef,
     UpdateKxEnvironmentNetworkResponseTypeDef,
     UpdateKxEnvironmentResponseTypeDef,
     ListKxChangesetsResponseTypeDef,
     ListKxClustersResponseTypeDef,
@@ -420,20 +422,21 @@
     ListKxEnvironmentsRequestListKxEnvironmentsPaginateTypeDef,
     GetEnvironmentResponseTypeDef,
     ListEnvironmentsResponseTypeDef,
     UpdateEnvironmentResponseTypeDef,
     ListKxEnvironmentsResponseTypeDef,
     CreateKxClusterResponseTypeDef,
     GetKxClusterResponseTypeDef,
+    KxDatabaseConfigurationUnionTypeDef,
     CreateKxClusterRequestRequestTypeDef,
     UpdateKxClusterDatabasesRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AutoScalingConfigurationTypeDef:
+def get_value() -> AutoScalingConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-finspace-1.28.15.post1/README.md` & `mypy-boto3-finspace-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-finspace.svg?color=blue)](https://pypi.org/project/mypy-boto3-finspace)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-finspace)](https://pepy.tech/project/mypy-boto3-finspace)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.finspace 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace)
+[boto3.finspace 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace)
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
 [mypy-boto3-finspace docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/).
 
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
@@ -292,20 +292,20 @@
 )
 
 
 def check_value(value: AutoScalingMetricType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_finspace.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_finspace.type_defs import (
     AutoScalingConfigurationTypeDef,
     CapacityConfigurationTypeDef,
     ChangeRequestTypeDef,
     CodeConfigurationTypeDef,
@@ -368,15 +368,17 @@
     GetKxDatabaseResponseTypeDef,
     GetKxUserResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     UpdateKxDatabaseResponseTypeDef,
     UpdateKxUserResponseTypeDef,
     CreateKxChangesetResponseTypeDef,
     GetKxChangesetResponseTypeDef,
+    VpcConfigurationUnionTypeDef,
     EnvironmentTypeDef,
+    FederationParametersUnionTypeDef,
     GetKxEnvironmentResponseTypeDef,
     KxEnvironmentTypeDef,
     UpdateKxEnvironmentNetworkRequestRequestTypeDef,
     UpdateKxEnvironmentNetworkResponseTypeDef,
     UpdateKxEnvironmentResponseTypeDef,
     ListKxChangesetsResponseTypeDef,
     ListKxClustersResponseTypeDef,
@@ -388,20 +390,21 @@
     ListKxEnvironmentsRequestListKxEnvironmentsPaginateTypeDef,
     GetEnvironmentResponseTypeDef,
     ListEnvironmentsResponseTypeDef,
     UpdateEnvironmentResponseTypeDef,
     ListKxEnvironmentsResponseTypeDef,
     CreateKxClusterResponseTypeDef,
     GetKxClusterResponseTypeDef,
+    KxDatabaseConfigurationUnionTypeDef,
     CreateKxClusterRequestRequestTypeDef,
     UpdateKxClusterDatabasesRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AutoScalingConfigurationTypeDef:
+def get_value() -> AutoScalingConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-finspace-1.28.15.post1/mypy_boto3_finspace/__init__.py` & `mypy-boto3-finspace-1.28.16/mypy_boto3_finspace/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-finspace-1.28.15.post1/mypy_boto3_finspace/__init__.pyi` & `mypy-boto3-finspace-1.28.16/mypy_boto3_finspace/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-finspace-1.28.15.post1/mypy_boto3_finspace/__main__.py` & `mypy-boto3-finspace-1.28.16/mypy_boto3_finspace/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.finspace 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.finspace 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace\nOther"
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

### Comparing `mypy-boto3-finspace-1.28.15.post1/mypy_boto3_finspace/client.py` & `mypy-boto3-finspace-1.28.16/mypy_boto3_finspace/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_finspace.client import finspaceClient
 
     session = Session()
     client: finspaceClient = session.client("finspace")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import FederationModeType, KxAzModeType, KxClusterTypeType
 from .paginator import ListKxEnvironmentsPaginator
 from .type_defs import (
     AutoScalingConfigurationTypeDef,
@@ -28,27 +28,25 @@
     CreateEnvironmentResponseTypeDef,
     CreateKxChangesetResponseTypeDef,
     CreateKxClusterResponseTypeDef,
     CreateKxDatabaseResponseTypeDef,
     CreateKxEnvironmentResponseTypeDef,
     CreateKxUserResponseTypeDef,
     CustomDNSServerTypeDef,
-    FederationParametersOutputTypeDef,
-    FederationParametersTypeDef,
+    FederationParametersUnionTypeDef,
     GetEnvironmentResponseTypeDef,
     GetKxChangesetResponseTypeDef,
     GetKxClusterResponseTypeDef,
     GetKxConnectionStringResponseTypeDef,
     GetKxDatabaseResponseTypeDef,
     GetKxEnvironmentResponseTypeDef,
     GetKxUserResponseTypeDef,
     KxCacheStorageConfigurationTypeDef,
     KxCommandLineArgumentTypeDef,
-    KxDatabaseConfigurationOutputTypeDef,
-    KxDatabaseConfigurationTypeDef,
+    KxDatabaseConfigurationUnionTypeDef,
     KxSavedownStorageConfigurationTypeDef,
     ListEnvironmentsResponseTypeDef,
     ListKxChangesetsResponseTypeDef,
     ListKxClusterNodesResponseTypeDef,
     ListKxClustersResponseTypeDef,
     ListKxDatabasesResponseTypeDef,
     ListKxEnvironmentsResponseTypeDef,
@@ -57,16 +55,15 @@
     SuperuserParametersTypeDef,
     TransitGatewayConfigurationTypeDef,
     UpdateEnvironmentResponseTypeDef,
     UpdateKxDatabaseResponseTypeDef,
     UpdateKxEnvironmentNetworkResponseTypeDef,
     UpdateKxEnvironmentResponseTypeDef,
     UpdateKxUserResponseTypeDef,
-    VpcConfigurationOutputTypeDef,
-    VpcConfigurationTypeDef,
+    VpcConfigurationUnionTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -133,17 +130,15 @@
         self,
         *,
         name: str,
         description: str = ...,
         kmsKeyId: str = ...,
         tags: Mapping[str, str] = ...,
         federationMode: FederationModeType = ...,
-        federationParameters: Union[
-            FederationParametersTypeDef, FederationParametersOutputTypeDef
-        ] = ...,
+        federationParameters: FederationParametersUnionTypeDef = ...,
         superuserParameters: SuperuserParametersTypeDef = ...,
         dataBundles: Sequence[str] = ...
     ) -> CreateEnvironmentResponseTypeDef:
         """
         Create a new FinSpace environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.create_environment)
@@ -171,21 +166,19 @@
         environmentId: str,
         clusterName: str,
         clusterType: KxClusterTypeType,
         capacityConfiguration: CapacityConfigurationTypeDef,
         releaseLabel: str,
         azMode: KxAzModeType,
         clientToken: str = ...,
-        databases: Sequence[
-            Union[KxDatabaseConfigurationTypeDef, KxDatabaseConfigurationOutputTypeDef]
-        ] = ...,
+        databases: Sequence[KxDatabaseConfigurationUnionTypeDef] = ...,
         cacheStorageConfigurations: Sequence[KxCacheStorageConfigurationTypeDef] = ...,
         autoScalingConfiguration: AutoScalingConfigurationTypeDef = ...,
         clusterDescription: str = ...,
-        vpcConfiguration: Union[VpcConfigurationTypeDef, VpcConfigurationOutputTypeDef] = ...,
+        vpcConfiguration: VpcConfigurationUnionTypeDef = ...,
         initializationScript: str = ...,
         commandLineArguments: Sequence[KxCommandLineArgumentTypeDef] = ...,
         code: CodeConfigurationTypeDef = ...,
         executionRole: str = ...,
         savedownStorageConfiguration: KxSavedownStorageConfigurationTypeDef = ...,
         availabilityZoneId: str = ...,
         tags: Mapping[str, str] = ...
@@ -469,33 +462,29 @@
     def update_environment(
         self,
         *,
         environmentId: str,
         name: str = ...,
         description: str = ...,
         federationMode: FederationModeType = ...,
-        federationParameters: Union[
-            FederationParametersTypeDef, FederationParametersOutputTypeDef
-        ] = ...
+        federationParameters: FederationParametersUnionTypeDef = ...
     ) -> UpdateEnvironmentResponseTypeDef:
         """
         Update your FinSpace environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.update_environment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/client/#update_environment)
         """
 
     def update_kx_cluster_databases(
         self,
         *,
         environmentId: str,
         clusterName: str,
-        databases: Sequence[
-            Union[KxDatabaseConfigurationTypeDef, KxDatabaseConfigurationOutputTypeDef]
-        ],
+        databases: Sequence[KxDatabaseConfigurationUnionTypeDef],
         clientToken: str = ...
     ) -> Dict[str, Any]:
         """
         Updates the databases mounted on a kdb cluster, which includes the `changesetId`
         and all the dbPaths to be cached.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.update_kx_cluster_databases)
```

### Comparing `mypy-boto3-finspace-1.28.15.post1/mypy_boto3_finspace/client.pyi` & `mypy-boto3-finspace-1.28.16/mypy_boto3_finspace/client.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_finspace.client import finspaceClient
 
     session = Session()
     client: finspaceClient = session.client("finspace")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import FederationModeType, KxAzModeType, KxClusterTypeType
 from .paginator import ListKxEnvironmentsPaginator
 from .type_defs import (
     AutoScalingConfigurationTypeDef,
@@ -28,27 +28,25 @@
     CreateEnvironmentResponseTypeDef,
     CreateKxChangesetResponseTypeDef,
     CreateKxClusterResponseTypeDef,
     CreateKxDatabaseResponseTypeDef,
     CreateKxEnvironmentResponseTypeDef,
     CreateKxUserResponseTypeDef,
     CustomDNSServerTypeDef,
-    FederationParametersOutputTypeDef,
-    FederationParametersTypeDef,
+    FederationParametersUnionTypeDef,
     GetEnvironmentResponseTypeDef,
     GetKxChangesetResponseTypeDef,
     GetKxClusterResponseTypeDef,
     GetKxConnectionStringResponseTypeDef,
     GetKxDatabaseResponseTypeDef,
     GetKxEnvironmentResponseTypeDef,
     GetKxUserResponseTypeDef,
     KxCacheStorageConfigurationTypeDef,
     KxCommandLineArgumentTypeDef,
-    KxDatabaseConfigurationOutputTypeDef,
-    KxDatabaseConfigurationTypeDef,
+    KxDatabaseConfigurationUnionTypeDef,
     KxSavedownStorageConfigurationTypeDef,
     ListEnvironmentsResponseTypeDef,
     ListKxChangesetsResponseTypeDef,
     ListKxClusterNodesResponseTypeDef,
     ListKxClustersResponseTypeDef,
     ListKxDatabasesResponseTypeDef,
     ListKxEnvironmentsResponseTypeDef,
@@ -57,16 +55,15 @@
     SuperuserParametersTypeDef,
     TransitGatewayConfigurationTypeDef,
     UpdateEnvironmentResponseTypeDef,
     UpdateKxDatabaseResponseTypeDef,
     UpdateKxEnvironmentNetworkResponseTypeDef,
     UpdateKxEnvironmentResponseTypeDef,
     UpdateKxUserResponseTypeDef,
-    VpcConfigurationOutputTypeDef,
-    VpcConfigurationTypeDef,
+    VpcConfigurationUnionTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -126,17 +123,15 @@
         self,
         *,
         name: str,
         description: str = ...,
         kmsKeyId: str = ...,
         tags: Mapping[str, str] = ...,
         federationMode: FederationModeType = ...,
-        federationParameters: Union[
-            FederationParametersTypeDef, FederationParametersOutputTypeDef
-        ] = ...,
+        federationParameters: FederationParametersUnionTypeDef = ...,
         superuserParameters: SuperuserParametersTypeDef = ...,
         dataBundles: Sequence[str] = ...
     ) -> CreateEnvironmentResponseTypeDef:
         """
         Create a new FinSpace environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.create_environment)
@@ -162,21 +157,19 @@
         environmentId: str,
         clusterName: str,
         clusterType: KxClusterTypeType,
         capacityConfiguration: CapacityConfigurationTypeDef,
         releaseLabel: str,
         azMode: KxAzModeType,
         clientToken: str = ...,
-        databases: Sequence[
-            Union[KxDatabaseConfigurationTypeDef, KxDatabaseConfigurationOutputTypeDef]
-        ] = ...,
+        databases: Sequence[KxDatabaseConfigurationUnionTypeDef] = ...,
         cacheStorageConfigurations: Sequence[KxCacheStorageConfigurationTypeDef] = ...,
         autoScalingConfiguration: AutoScalingConfigurationTypeDef = ...,
         clusterDescription: str = ...,
-        vpcConfiguration: Union[VpcConfigurationTypeDef, VpcConfigurationOutputTypeDef] = ...,
+        vpcConfiguration: VpcConfigurationUnionTypeDef = ...,
         initializationScript: str = ...,
         commandLineArguments: Sequence[KxCommandLineArgumentTypeDef] = ...,
         code: CodeConfigurationTypeDef = ...,
         executionRole: str = ...,
         savedownStorageConfiguration: KxSavedownStorageConfigurationTypeDef = ...,
         availabilityZoneId: str = ...,
         tags: Mapping[str, str] = ...
@@ -433,32 +426,28 @@
     def update_environment(
         self,
         *,
         environmentId: str,
         name: str = ...,
         description: str = ...,
         federationMode: FederationModeType = ...,
-        federationParameters: Union[
-            FederationParametersTypeDef, FederationParametersOutputTypeDef
-        ] = ...
+        federationParameters: FederationParametersUnionTypeDef = ...
     ) -> UpdateEnvironmentResponseTypeDef:
         """
         Update your FinSpace environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.update_environment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/client/#update_environment)
         """
     def update_kx_cluster_databases(
         self,
         *,
         environmentId: str,
         clusterName: str,
-        databases: Sequence[
-            Union[KxDatabaseConfigurationTypeDef, KxDatabaseConfigurationOutputTypeDef]
-        ],
+        databases: Sequence[KxDatabaseConfigurationUnionTypeDef],
         clientToken: str = ...
     ) -> Dict[str, Any]:
         """
         Updates the databases mounted on a kdb cluster, which includes the `changesetId`
         and all the dbPaths to be cached.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.update_kx_cluster_databases)
```

### Comparing `mypy-boto3-finspace-1.28.15.post1/mypy_boto3_finspace/literals.py` & `mypy-boto3-finspace-1.28.16/mypy_boto3_finspace/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-finspace-1.28.15.post1/mypy_boto3_finspace/literals.pyi` & `mypy-boto3-finspace-1.28.16/mypy_boto3_finspace/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-finspace-1.28.15.post1/mypy_boto3_finspace/paginator.py` & `mypy-boto3-finspace-1.28.16/mypy_boto3_finspace/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-finspace-1.28.15.post1/mypy_boto3_finspace/paginator.pyi` & `mypy-boto3-finspace-1.28.16/mypy_boto3_finspace/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-finspace-1.28.15.post1/mypy_boto3_finspace/type_defs.py` & `mypy-boto3-finspace-1.28.16/mypy_boto3_finspace/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_finspace.type_defs import AutoScalingConfigurationTypeDef
 
-    data: AutoScalingConfigurationTypeDef = {...}
+    data: AutoScalingConfigurationTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -102,15 +102,17 @@
     "GetKxDatabaseResponseTypeDef",
     "GetKxUserResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "UpdateKxDatabaseResponseTypeDef",
     "UpdateKxUserResponseTypeDef",
     "CreateKxChangesetResponseTypeDef",
     "GetKxChangesetResponseTypeDef",
+    "VpcConfigurationUnionTypeDef",
     "EnvironmentTypeDef",
+    "FederationParametersUnionTypeDef",
     "GetKxEnvironmentResponseTypeDef",
     "KxEnvironmentTypeDef",
     "UpdateKxEnvironmentNetworkRequestRequestTypeDef",
     "UpdateKxEnvironmentNetworkResponseTypeDef",
     "UpdateKxEnvironmentResponseTypeDef",
     "ListKxChangesetsResponseTypeDef",
     "ListKxClustersResponseTypeDef",
@@ -122,14 +124,15 @@
     "ListKxEnvironmentsRequestListKxEnvironmentsPaginateTypeDef",
     "GetEnvironmentResponseTypeDef",
     "ListEnvironmentsResponseTypeDef",
     "UpdateEnvironmentResponseTypeDef",
     "ListKxEnvironmentsResponseTypeDef",
     "CreateKxClusterResponseTypeDef",
     "GetKxClusterResponseTypeDef",
+    "KxDatabaseConfigurationUnionTypeDef",
     "CreateKxClusterRequestRequestTypeDef",
     "UpdateKxClusterDatabasesRequestRequestTypeDef",
 )
 
 AutoScalingConfigurationTypeDef = TypedDict(
     "AutoScalingConfigurationTypeDef",
     {
@@ -998,14 +1001,15 @@
         "lastModifiedTimestamp": datetime,
         "status": ChangesetStatusType,
         "errorInfo": ErrorInfoTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+VpcConfigurationUnionTypeDef = Union[VpcConfigurationTypeDef, VpcConfigurationOutputTypeDef]
 EnvironmentTypeDef = TypedDict(
     "EnvironmentTypeDef",
     {
         "name": str,
         "environmentId": str,
         "awsAccountId": str,
         "status": EnvironmentStatusType,
@@ -1017,14 +1021,17 @@
         "dedicatedServiceAccountId": str,
         "federationMode": FederationModeType,
         "federationParameters": FederationParametersOutputTypeDef,
     },
     total=False,
 )
 
+FederationParametersUnionTypeDef = Union[
+    FederationParametersTypeDef, FederationParametersOutputTypeDef
+]
 GetKxEnvironmentResponseTypeDef = TypedDict(
     "GetKxEnvironmentResponseTypeDef",
     {
         "name": str,
         "environmentId": str,
         "awsAccountId": str,
         "status": EnvironmentStatusType,
@@ -1321,14 +1328,17 @@
         "azMode": KxAzModeType,
         "availabilityZoneId": str,
         "createdTimestamp": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+KxDatabaseConfigurationUnionTypeDef = Union[
+    KxDatabaseConfigurationTypeDef, KxDatabaseConfigurationOutputTypeDef
+]
 _RequiredCreateKxClusterRequestRequestTypeDef = TypedDict(
     "_RequiredCreateKxClusterRequestRequestTypeDef",
     {
         "environmentId": str,
         "clusterName": str,
         "clusterType": KxClusterTypeType,
         "capacityConfiguration": CapacityConfigurationTypeDef,
@@ -1336,17 +1346,15 @@
         "azMode": KxAzModeType,
     },
 )
 _OptionalCreateKxClusterRequestRequestTypeDef = TypedDict(
     "_OptionalCreateKxClusterRequestRequestTypeDef",
     {
         "clientToken": str,
-        "databases": Sequence[
-            Union[KxDatabaseConfigurationTypeDef, KxDatabaseConfigurationOutputTypeDef]
-        ],
+        "databases": Sequence[KxDatabaseConfigurationUnionTypeDef],
         "cacheStorageConfigurations": Sequence[KxCacheStorageConfigurationTypeDef],
         "autoScalingConfiguration": AutoScalingConfigurationTypeDef,
         "clusterDescription": str,
         "vpcConfiguration": VpcConfigurationTypeDef,
         "initializationScript": str,
         "commandLineArguments": Sequence[KxCommandLineArgumentTypeDef],
         "code": CodeConfigurationTypeDef,
@@ -1366,17 +1374,15 @@
 
 
 _RequiredUpdateKxClusterDatabasesRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateKxClusterDatabasesRequestRequestTypeDef",
     {
         "environmentId": str,
         "clusterName": str,
-        "databases": Sequence[
-            Union[KxDatabaseConfigurationTypeDef, KxDatabaseConfigurationOutputTypeDef]
-        ],
+        "databases": Sequence[KxDatabaseConfigurationUnionTypeDef],
     },
 )
 _OptionalUpdateKxClusterDatabasesRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateKxClusterDatabasesRequestRequestTypeDef",
     {
         "clientToken": str,
     },
```

### Comparing `mypy-boto3-finspace-1.28.15.post1/mypy_boto3_finspace/type_defs.pyi` & `mypy-boto3-finspace-1.28.16/mypy_boto3_finspace/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_finspace.type_defs import AutoScalingConfigurationTypeDef
 
-    data: AutoScalingConfigurationTypeDef = {...}
+    data: AutoScalingConfigurationTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -101,15 +101,17 @@
     "GetKxDatabaseResponseTypeDef",
     "GetKxUserResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "UpdateKxDatabaseResponseTypeDef",
     "UpdateKxUserResponseTypeDef",
     "CreateKxChangesetResponseTypeDef",
     "GetKxChangesetResponseTypeDef",
+    "VpcConfigurationUnionTypeDef",
     "EnvironmentTypeDef",
+    "FederationParametersUnionTypeDef",
     "GetKxEnvironmentResponseTypeDef",
     "KxEnvironmentTypeDef",
     "UpdateKxEnvironmentNetworkRequestRequestTypeDef",
     "UpdateKxEnvironmentNetworkResponseTypeDef",
     "UpdateKxEnvironmentResponseTypeDef",
     "ListKxChangesetsResponseTypeDef",
     "ListKxClustersResponseTypeDef",
@@ -121,14 +123,15 @@
     "ListKxEnvironmentsRequestListKxEnvironmentsPaginateTypeDef",
     "GetEnvironmentResponseTypeDef",
     "ListEnvironmentsResponseTypeDef",
     "UpdateEnvironmentResponseTypeDef",
     "ListKxEnvironmentsResponseTypeDef",
     "CreateKxClusterResponseTypeDef",
     "GetKxClusterResponseTypeDef",
+    "KxDatabaseConfigurationUnionTypeDef",
     "CreateKxClusterRequestRequestTypeDef",
     "UpdateKxClusterDatabasesRequestRequestTypeDef",
 )
 
 AutoScalingConfigurationTypeDef = TypedDict(
     "AutoScalingConfigurationTypeDef",
     {
@@ -967,14 +970,15 @@
         "lastModifiedTimestamp": datetime,
         "status": ChangesetStatusType,
         "errorInfo": ErrorInfoTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+VpcConfigurationUnionTypeDef = Union[VpcConfigurationTypeDef, VpcConfigurationOutputTypeDef]
 EnvironmentTypeDef = TypedDict(
     "EnvironmentTypeDef",
     {
         "name": str,
         "environmentId": str,
         "awsAccountId": str,
         "status": EnvironmentStatusType,
@@ -986,14 +990,17 @@
         "dedicatedServiceAccountId": str,
         "federationMode": FederationModeType,
         "federationParameters": FederationParametersOutputTypeDef,
     },
     total=False,
 )
 
+FederationParametersUnionTypeDef = Union[
+    FederationParametersTypeDef, FederationParametersOutputTypeDef
+]
 GetKxEnvironmentResponseTypeDef = TypedDict(
     "GetKxEnvironmentResponseTypeDef",
     {
         "name": str,
         "environmentId": str,
         "awsAccountId": str,
         "status": EnvironmentStatusType,
@@ -1284,14 +1291,17 @@
         "azMode": KxAzModeType,
         "availabilityZoneId": str,
         "createdTimestamp": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+KxDatabaseConfigurationUnionTypeDef = Union[
+    KxDatabaseConfigurationTypeDef, KxDatabaseConfigurationOutputTypeDef
+]
 _RequiredCreateKxClusterRequestRequestTypeDef = TypedDict(
     "_RequiredCreateKxClusterRequestRequestTypeDef",
     {
         "environmentId": str,
         "clusterName": str,
         "clusterType": KxClusterTypeType,
         "capacityConfiguration": CapacityConfigurationTypeDef,
@@ -1299,17 +1309,15 @@
         "azMode": KxAzModeType,
     },
 )
 _OptionalCreateKxClusterRequestRequestTypeDef = TypedDict(
     "_OptionalCreateKxClusterRequestRequestTypeDef",
     {
         "clientToken": str,
-        "databases": Sequence[
-            Union[KxDatabaseConfigurationTypeDef, KxDatabaseConfigurationOutputTypeDef]
-        ],
+        "databases": Sequence[KxDatabaseConfigurationUnionTypeDef],
         "cacheStorageConfigurations": Sequence[KxCacheStorageConfigurationTypeDef],
         "autoScalingConfiguration": AutoScalingConfigurationTypeDef,
         "clusterDescription": str,
         "vpcConfiguration": VpcConfigurationTypeDef,
         "initializationScript": str,
         "commandLineArguments": Sequence[KxCommandLineArgumentTypeDef],
         "code": CodeConfigurationTypeDef,
@@ -1327,17 +1335,15 @@
     pass
 
 _RequiredUpdateKxClusterDatabasesRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateKxClusterDatabasesRequestRequestTypeDef",
     {
         "environmentId": str,
         "clusterName": str,
-        "databases": Sequence[
-            Union[KxDatabaseConfigurationTypeDef, KxDatabaseConfigurationOutputTypeDef]
-        ],
+        "databases": Sequence[KxDatabaseConfigurationUnionTypeDef],
     },
 )
 _OptionalUpdateKxClusterDatabasesRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateKxClusterDatabasesRequestRequestTypeDef",
     {
         "clientToken": str,
     },
```

### Comparing `mypy-boto3-finspace-1.28.15.post1/mypy_boto3_finspace.egg-info/PKG-INFO` & `mypy-boto3-finspace-1.28.16/mypy_boto3_finspace.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-finspace
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.finspace 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.finspace 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 finspace type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 finspace type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-finspace.svg?color=blue)](https://pypi.org/project/mypy-boto3-finspace)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-finspace)](https://pepy.tech/project/mypy-boto3-finspace)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.finspace 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace)
+[boto3.finspace 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace)
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
 [mypy-boto3-finspace docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/).
 
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
@@ -324,20 +324,20 @@
 )
 
 
 def check_value(value: AutoScalingMetricType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_finspace.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_finspace.type_defs import (
     AutoScalingConfigurationTypeDef,
     CapacityConfigurationTypeDef,
     ChangeRequestTypeDef,
     CodeConfigurationTypeDef,
@@ -400,15 +400,17 @@
     GetKxDatabaseResponseTypeDef,
     GetKxUserResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     UpdateKxDatabaseResponseTypeDef,
     UpdateKxUserResponseTypeDef,
     CreateKxChangesetResponseTypeDef,
     GetKxChangesetResponseTypeDef,
+    VpcConfigurationUnionTypeDef,
     EnvironmentTypeDef,
+    FederationParametersUnionTypeDef,
     GetKxEnvironmentResponseTypeDef,
     KxEnvironmentTypeDef,
     UpdateKxEnvironmentNetworkRequestRequestTypeDef,
     UpdateKxEnvironmentNetworkResponseTypeDef,
     UpdateKxEnvironmentResponseTypeDef,
     ListKxChangesetsResponseTypeDef,
     ListKxClustersResponseTypeDef,
@@ -420,20 +422,21 @@
     ListKxEnvironmentsRequestListKxEnvironmentsPaginateTypeDef,
     GetEnvironmentResponseTypeDef,
     ListEnvironmentsResponseTypeDef,
     UpdateEnvironmentResponseTypeDef,
     ListKxEnvironmentsResponseTypeDef,
     CreateKxClusterResponseTypeDef,
     GetKxClusterResponseTypeDef,
+    KxDatabaseConfigurationUnionTypeDef,
     CreateKxClusterRequestRequestTypeDef,
     UpdateKxClusterDatabasesRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AutoScalingConfigurationTypeDef:
+def get_value() -> AutoScalingConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-finspace-1.28.15.post1/mypy_boto3_finspace.egg-info/SOURCES.txt` & `mypy-boto3-finspace-1.28.16/mypy_boto3_finspace.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-finspace-1.28.15.post1/setup.py` & `mypy-boto3-finspace-1.28.16/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-finspace",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_finspace"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.finspace 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.2"
+        "Type annotations for boto3.finspace 1.28.16 service generated with mypy-boto3-builder"
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
-    keywords="boto3 finspace type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 finspace type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_finspace": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

