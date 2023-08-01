# Comparing `tmp/mypy-boto3-entityresolution-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-entityresolution-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-entityresolution-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:06 2023, max compression
+gzip compressed data, was "mypy-boto3-entityresolution-1.28.16.tar", last modified: Tue Aug  1 11:36:45 2023, max compression
```

## Comparing `mypy-boto3-entityresolution-1.28.15.post1.tar` & `mypy-boto3-entityresolution-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:06.165143 mypy-boto3-entityresolution-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:45:04.000000 mypy-boto3-entityresolution-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15435 2023-07-29 10:03:06.165143 mypy-boto3-entityresolution-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13906 2023-07-29 09:45:04.000000 mypy-boto3-entityresolution-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:06.157143 mypy-boto3-entityresolution-1.28.15.post1/mypy_boto3_entityresolution/
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-07-29 09:45:04.000000 mypy-boto3-entityresolution-1.28.15.post1/mypy_boto3_entityresolution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-29 09:45:04.000000 mypy-boto3-entityresolution-1.28.15.post1/mypy_boto3_entityresolution/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-29 09:45:04.000000 mypy-boto3-entityresolution-1.28.15.post1/mypy_boto3_entityresolution/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15352 2023-07-29 09:45:04.000000 mypy-boto3-entityresolution-1.28.15.post1/mypy_boto3_entityresolution/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15326 2023-07-29 09:45:04.000000 mypy-boto3-entityresolution-1.28.15.post1/mypy_boto3_entityresolution/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8889 2023-07-29 09:45:04.000000 mypy-boto3-entityresolution-1.28.15.post1/mypy_boto3_entityresolution/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8887 2023-07-29 09:45:04.000000 mypy-boto3-entityresolution-1.28.15.post1/mypy_boto3_entityresolution/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4253 2023-07-29 09:45:04.000000 mypy-boto3-entityresolution-1.28.15.post1/mypy_boto3_entityresolution/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4248 2023-07-29 09:45:04.000000 mypy-boto3-entityresolution-1.28.15.post1/mypy_boto3_entityresolution/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:45:04.000000 mypy-boto3-entityresolution-1.28.15.post1/mypy_boto3_entityresolution/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    17808 2023-07-29 09:45:05.000000 mypy-boto3-entityresolution-1.28.15.post1/mypy_boto3_entityresolution/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    17786 2023-07-29 09:45:05.000000 mypy-boto3-entityresolution-1.28.15.post1/mypy_boto3_entityresolution/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:45:04.000000 mypy-boto3-entityresolution-1.28.15.post1/mypy_boto3_entityresolution/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:06.165143 mypy-boto3-entityresolution-1.28.15.post1/mypy_boto3_entityresolution.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15435 2023-07-29 10:03:05.000000 mypy-boto3-entityresolution-1.28.15.post1/mypy_boto3_entityresolution.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-29 10:03:05.000000 mypy-boto3-entityresolution-1.28.15.post1/mypy_boto3_entityresolution.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:05.000000 mypy-boto3-entityresolution-1.28.15.post1/mypy_boto3_entityresolution.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:05.000000 mypy-boto3-entityresolution-1.28.15.post1/mypy_boto3_entityresolution.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:05.000000 mypy-boto3-entityresolution-1.28.15.post1/mypy_boto3_entityresolution.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-29 10:03:05.000000 mypy-boto3-entityresolution-1.28.15.post1/mypy_boto3_entityresolution.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:06.165143 mypy-boto3-entityresolution-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-07-29 09:45:04.000000 mypy-boto3-entityresolution-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:45.796894 mypy-boto3-entityresolution-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:17:40.000000 mypy-boto3-entityresolution-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15493 2023-08-01 11:36:45.796894 mypy-boto3-entityresolution-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13973 2023-08-01 11:17:40.000000 mypy-boto3-entityresolution-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:45.796894 mypy-boto3-entityresolution-1.28.16/mypy_boto3_entityresolution/
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-08-01 11:17:40.000000 mypy-boto3-entityresolution-1.28.16/mypy_boto3_entityresolution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-08-01 11:17:40.000000 mypy-boto3-entityresolution-1.28.16/mypy_boto3_entityresolution/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-08-01 11:17:40.000000 mypy-boto3-entityresolution-1.28.16/mypy_boto3_entityresolution/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15153 2023-08-01 11:17:40.000000 mypy-boto3-entityresolution-1.28.16/mypy_boto3_entityresolution/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15127 2023-08-01 11:17:40.000000 mypy-boto3-entityresolution-1.28.16/mypy_boto3_entityresolution/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8889 2023-08-01 11:17:41.000000 mypy-boto3-entityresolution-1.28.16/mypy_boto3_entityresolution/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8887 2023-08-01 11:17:41.000000 mypy-boto3-entityresolution-1.28.16/mypy_boto3_entityresolution/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4253 2023-08-01 11:17:40.000000 mypy-boto3-entityresolution-1.28.16/mypy_boto3_entityresolution/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4248 2023-08-01 11:17:40.000000 mypy-boto3-entityresolution-1.28.16/mypy_boto3_entityresolution/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:17:40.000000 mypy-boto3-entityresolution-1.28.16/mypy_boto3_entityresolution/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    18012 2023-08-01 11:17:41.000000 mypy-boto3-entityresolution-1.28.16/mypy_boto3_entityresolution/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17990 2023-08-01 11:17:41.000000 mypy-boto3-entityresolution-1.28.16/mypy_boto3_entityresolution/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:17:40.000000 mypy-boto3-entityresolution-1.28.16/mypy_boto3_entityresolution/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:45.796894 mypy-boto3-entityresolution-1.28.16/mypy_boto3_entityresolution.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15493 2023-08-01 11:36:45.000000 mypy-boto3-entityresolution-1.28.16/mypy_boto3_entityresolution.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-08-01 11:36:45.000000 mypy-boto3-entityresolution-1.28.16/mypy_boto3_entityresolution.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:45.000000 mypy-boto3-entityresolution-1.28.16/mypy_boto3_entityresolution.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:45.000000 mypy-boto3-entityresolution-1.28.16/mypy_boto3_entityresolution.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:45.000000 mypy-boto3-entityresolution-1.28.16/mypy_boto3_entityresolution.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-01 11:36:45.000000 mypy-boto3-entityresolution-1.28.16/mypy_boto3_entityresolution.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:45.796894 mypy-boto3-entityresolution-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-08-01 11:17:40.000000 mypy-boto3-entityresolution-1.28.16/setup.py
```

### Comparing `mypy-boto3-entityresolution-1.28.15.post1/LICENSE` & `mypy-boto3-entityresolution-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-entityresolution-1.28.15.post1/PKG-INFO` & `mypy-boto3-entityresolution-1.28.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-entityresolution
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.EntityResolution 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.EntityResolution 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 entityresolution type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 entityresolution type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-entityresolution.svg?color=blue)](https://pypi.org/project/mypy-boto3-entityresolution)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-entityresolution)](https://pepy.tech/project/mypy-boto3-entityresolution)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EntityResolution 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution)
+[boto3.EntityResolution 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution)
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
 [mypy-boto3-entityresolution docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/).
 
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
@@ -327,20 +327,20 @@
 )
 
 
 def check_value(value: AttributeMatchingModelType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_entityresolution.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_entityresolution.type_defs import (
     IncrementalRunConfigTypeDef,
     InputSourceTypeDef,
     ResponseMetadataTypeDef,
     SchemaInputAttributeTypeDef,
@@ -381,25 +381,27 @@
     ListSchemaMappingsInputListSchemaMappingsPaginateTypeDef,
     ListMatchingWorkflowsOutputTypeDef,
     ListSchemaMappingsOutputTypeDef,
     OutputSourceOutputTypeDef,
     OutputSourceTypeDef,
     RuleBasedPropertiesOutputTypeDef,
     RuleBasedPropertiesTypeDef,
+    OutputSourceUnionTypeDef,
     ResolutionTechniquesOutputTypeDef,
     ResolutionTechniquesTypeDef,
     CreateMatchingWorkflowOutputTypeDef,
     GetMatchingWorkflowOutputTypeDef,
     UpdateMatchingWorkflowOutputTypeDef,
     CreateMatchingWorkflowInputRequestTypeDef,
+    ResolutionTechniquesUnionTypeDef,
     UpdateMatchingWorkflowInputRequestTypeDef,
 )
 
 
-def get_structure() -> IncrementalRunConfigTypeDef:
+def get_value() -> IncrementalRunConfigTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-entityresolution-1.28.15.post1/README.md` & `mypy-boto3-entityresolution-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-entityresolution.svg?color=blue)](https://pypi.org/project/mypy-boto3-entityresolution)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-entityresolution)](https://pepy.tech/project/mypy-boto3-entityresolution)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EntityResolution 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution)
+[boto3.EntityResolution 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution)
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
 [mypy-boto3-entityresolution docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/).
 
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
@@ -295,20 +295,20 @@
 )
 
 
 def check_value(value: AttributeMatchingModelType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_entityresolution.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_entityresolution.type_defs import (
     IncrementalRunConfigTypeDef,
     InputSourceTypeDef,
     ResponseMetadataTypeDef,
     SchemaInputAttributeTypeDef,
@@ -349,25 +349,27 @@
     ListSchemaMappingsInputListSchemaMappingsPaginateTypeDef,
     ListMatchingWorkflowsOutputTypeDef,
     ListSchemaMappingsOutputTypeDef,
     OutputSourceOutputTypeDef,
     OutputSourceTypeDef,
     RuleBasedPropertiesOutputTypeDef,
     RuleBasedPropertiesTypeDef,
+    OutputSourceUnionTypeDef,
     ResolutionTechniquesOutputTypeDef,
     ResolutionTechniquesTypeDef,
     CreateMatchingWorkflowOutputTypeDef,
     GetMatchingWorkflowOutputTypeDef,
     UpdateMatchingWorkflowOutputTypeDef,
     CreateMatchingWorkflowInputRequestTypeDef,
+    ResolutionTechniquesUnionTypeDef,
     UpdateMatchingWorkflowInputRequestTypeDef,
 )
 
 
-def get_structure() -> IncrementalRunConfigTypeDef:
+def get_value() -> IncrementalRunConfigTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-entityresolution-1.28.15.post1/mypy_boto3_entityresolution/__init__.py` & `mypy-boto3-entityresolution-1.28.16/mypy_boto3_entityresolution/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-entityresolution-1.28.15.post1/mypy_boto3_entityresolution/__init__.pyi` & `mypy-boto3-entityresolution-1.28.16/mypy_boto3_entityresolution/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-entityresolution-1.28.15.post1/mypy_boto3_entityresolution/__main__.py` & `mypy-boto3-entityresolution-1.28.16/mypy_boto3_entityresolution/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.EntityResolution 1.28.15\nVersion:        "
-        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.EntityResolution 1.28.16\nVersion:         1.28.16\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution\nOther"
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

### Comparing `mypy-boto3-entityresolution-1.28.15.post1/mypy_boto3_entityresolution/client.py` & `mypy-boto3-entityresolution-1.28.16/mypy_boto3_entityresolution/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_entityresolution.client import EntityResolutionClient
 
     session = Session()
     client: EntityResolutionClient = session.client("entityresolution")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .paginator import (
     ListMatchingJobsPaginator,
     ListMatchingWorkflowsPaginator,
     ListSchemaMappingsPaginator,
@@ -34,18 +34,16 @@
     GetSchemaMappingOutputTypeDef,
     IncrementalRunConfigTypeDef,
     InputSourceTypeDef,
     ListMatchingJobsOutputTypeDef,
     ListMatchingWorkflowsOutputTypeDef,
     ListSchemaMappingsOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
-    OutputSourceOutputTypeDef,
-    OutputSourceTypeDef,
-    ResolutionTechniquesOutputTypeDef,
-    ResolutionTechniquesTypeDef,
+    OutputSourceUnionTypeDef,
+    ResolutionTechniquesUnionTypeDef,
     SchemaInputAttributeTypeDef,
     StartMatchingJobOutputTypeDef,
     UpdateMatchingWorkflowOutputTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
@@ -108,16 +106,16 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/client/#close)
         """
 
     def create_matching_workflow(
         self,
         *,
         inputSourceConfig: Sequence[InputSourceTypeDef],
-        outputSourceConfig: Sequence[Union[OutputSourceTypeDef, OutputSourceOutputTypeDef]],
-        resolutionTechniques: Union[ResolutionTechniquesTypeDef, ResolutionTechniquesOutputTypeDef],
+        outputSourceConfig: Sequence[OutputSourceUnionTypeDef],
+        resolutionTechniques: ResolutionTechniquesUnionTypeDef,
         roleArn: str,
         workflowName: str,
         description: str = ...,
         incrementalRunConfig: IncrementalRunConfigTypeDef = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateMatchingWorkflowOutputTypeDef:
         """
@@ -275,16 +273,16 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/client/#untag_resource)
         """
 
     def update_matching_workflow(
         self,
         *,
         inputSourceConfig: Sequence[InputSourceTypeDef],
-        outputSourceConfig: Sequence[Union[OutputSourceTypeDef, OutputSourceOutputTypeDef]],
-        resolutionTechniques: Union[ResolutionTechniquesTypeDef, ResolutionTechniquesOutputTypeDef],
+        outputSourceConfig: Sequence[OutputSourceUnionTypeDef],
+        resolutionTechniques: ResolutionTechniquesUnionTypeDef,
         roleArn: str,
         workflowName: str,
         description: str = ...,
         incrementalRunConfig: IncrementalRunConfigTypeDef = ...
     ) -> UpdateMatchingWorkflowOutputTypeDef:
         """
         Updates an existing `MatchingWorkflow`.
```

### Comparing `mypy-boto3-entityresolution-1.28.15.post1/mypy_boto3_entityresolution/client.pyi` & `mypy-boto3-entityresolution-1.28.16/mypy_boto3_entityresolution/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_entityresolution.client import EntityResolutionClient
 
     session = Session()
     client: EntityResolutionClient = session.client("entityresolution")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .paginator import (
     ListMatchingJobsPaginator,
     ListMatchingWorkflowsPaginator,
     ListSchemaMappingsPaginator,
@@ -34,18 +34,16 @@
     GetSchemaMappingOutputTypeDef,
     IncrementalRunConfigTypeDef,
     InputSourceTypeDef,
     ListMatchingJobsOutputTypeDef,
     ListMatchingWorkflowsOutputTypeDef,
     ListSchemaMappingsOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
-    OutputSourceOutputTypeDef,
-    OutputSourceTypeDef,
-    ResolutionTechniquesOutputTypeDef,
-    ResolutionTechniquesTypeDef,
+    OutputSourceUnionTypeDef,
+    ResolutionTechniquesUnionTypeDef,
     SchemaInputAttributeTypeDef,
     StartMatchingJobOutputTypeDef,
     UpdateMatchingWorkflowOutputTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
@@ -101,16 +99,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/client/#close)
         """
     def create_matching_workflow(
         self,
         *,
         inputSourceConfig: Sequence[InputSourceTypeDef],
-        outputSourceConfig: Sequence[Union[OutputSourceTypeDef, OutputSourceOutputTypeDef]],
-        resolutionTechniques: Union[ResolutionTechniquesTypeDef, ResolutionTechniquesOutputTypeDef],
+        outputSourceConfig: Sequence[OutputSourceUnionTypeDef],
+        resolutionTechniques: ResolutionTechniquesUnionTypeDef,
         roleArn: str,
         workflowName: str,
         description: str = ...,
         incrementalRunConfig: IncrementalRunConfigTypeDef = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateMatchingWorkflowOutputTypeDef:
         """
@@ -252,16 +250,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/client/#untag_resource)
         """
     def update_matching_workflow(
         self,
         *,
         inputSourceConfig: Sequence[InputSourceTypeDef],
-        outputSourceConfig: Sequence[Union[OutputSourceTypeDef, OutputSourceOutputTypeDef]],
-        resolutionTechniques: Union[ResolutionTechniquesTypeDef, ResolutionTechniquesOutputTypeDef],
+        outputSourceConfig: Sequence[OutputSourceUnionTypeDef],
+        resolutionTechniques: ResolutionTechniquesUnionTypeDef,
         roleArn: str,
         workflowName: str,
         description: str = ...,
         incrementalRunConfig: IncrementalRunConfigTypeDef = ...
     ) -> UpdateMatchingWorkflowOutputTypeDef:
         """
         Updates an existing `MatchingWorkflow`.
```

### Comparing `mypy-boto3-entityresolution-1.28.15.post1/mypy_boto3_entityresolution/literals.py` & `mypy-boto3-entityresolution-1.28.16/mypy_boto3_entityresolution/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-entityresolution-1.28.15.post1/mypy_boto3_entityresolution/literals.pyi` & `mypy-boto3-entityresolution-1.28.16/mypy_boto3_entityresolution/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-entityresolution-1.28.15.post1/mypy_boto3_entityresolution/paginator.py` & `mypy-boto3-entityresolution-1.28.16/mypy_boto3_entityresolution/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-entityresolution-1.28.15.post1/mypy_boto3_entityresolution/paginator.pyi` & `mypy-boto3-entityresolution-1.28.16/mypy_boto3_entityresolution/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-entityresolution-1.28.15.post1/mypy_boto3_entityresolution/type_defs.py` & `mypy-boto3-entityresolution-1.28.16/mypy_boto3_entityresolution/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_entityresolution.type_defs import IncrementalRunConfigTypeDef
 
-    data: IncrementalRunConfigTypeDef = {...}
+    data: IncrementalRunConfigTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -27,15 +27,14 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "IncrementalRunConfigTypeDef",
     "InputSourceTypeDef",
     "ResponseMetadataTypeDef",
     "SchemaInputAttributeTypeDef",
     "DeleteMatchingWorkflowInputRequestTypeDef",
     "DeleteSchemaMappingInputRequestTypeDef",
@@ -74,20 +73,22 @@
     "ListSchemaMappingsInputListSchemaMappingsPaginateTypeDef",
     "ListMatchingWorkflowsOutputTypeDef",
     "ListSchemaMappingsOutputTypeDef",
     "OutputSourceOutputTypeDef",
     "OutputSourceTypeDef",
     "RuleBasedPropertiesOutputTypeDef",
     "RuleBasedPropertiesTypeDef",
+    "OutputSourceUnionTypeDef",
     "ResolutionTechniquesOutputTypeDef",
     "ResolutionTechniquesTypeDef",
     "CreateMatchingWorkflowOutputTypeDef",
     "GetMatchingWorkflowOutputTypeDef",
     "UpdateMatchingWorkflowOutputTypeDef",
     "CreateMatchingWorkflowInputRequestTypeDef",
+    "ResolutionTechniquesUnionTypeDef",
     "UpdateMatchingWorkflowInputRequestTypeDef",
 )
 
 IncrementalRunConfigTypeDef = TypedDict(
     "IncrementalRunConfigTypeDef",
     {
         "incrementalRunType": Literal["IMMEDIATE"],
@@ -106,19 +107,17 @@
     "_OptionalInputSourceTypeDef",
     {
         "applyNormalization": bool,
     },
     total=False,
 )
 
-
 class InputSourceTypeDef(_RequiredInputSourceTypeDef, _OptionalInputSourceTypeDef):
     pass
 
-
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -138,21 +137,19 @@
     {
         "groupName": str,
         "matchKey": str,
     },
     total=False,
 )
 
-
 class SchemaInputAttributeTypeDef(
     _RequiredSchemaInputAttributeTypeDef, _OptionalSchemaInputAttributeTypeDef
 ):
     pass
 
-
 DeleteMatchingWorkflowInputRequestTypeDef = TypedDict(
     "DeleteMatchingWorkflowInputRequestTypeDef",
     {
         "workflowName": str,
     },
 )
 
@@ -224,19 +221,17 @@
     "_OptionalJobSummaryTypeDef",
     {
         "endTime": datetime,
     },
     total=False,
 )
 
-
 class JobSummaryTypeDef(_RequiredJobSummaryTypeDef, _OptionalJobSummaryTypeDef):
     pass
 
-
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
@@ -254,21 +249,19 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListMatchingJobsInputRequestTypeDef(
     _RequiredListMatchingJobsInputRequestTypeDef, _OptionalListMatchingJobsInputRequestTypeDef
 ):
     pass
 
-
 ListMatchingWorkflowsInputRequestTypeDef = TypedDict(
     "ListMatchingWorkflowsInputRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -320,19 +313,17 @@
     "_OptionalOutputAttributeTypeDef",
     {
         "hashed": bool,
     },
     total=False,
 )
 
-
 class OutputAttributeTypeDef(_RequiredOutputAttributeTypeDef, _OptionalOutputAttributeTypeDef):
     pass
 
-
 RuleOutputTypeDef = TypedDict(
     "RuleOutputTypeDef",
     {
         "matchingKeys": List[str],
         "ruleName": str,
     },
 )
@@ -420,21 +411,19 @@
         "description": str,
         "mappedInputFields": Sequence[SchemaInputAttributeTypeDef],
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateSchemaMappingInputRequestTypeDef(
     _RequiredCreateSchemaMappingInputRequestTypeDef, _OptionalCreateSchemaMappingInputRequestTypeDef
 ):
     pass
 
-
 CreateSchemaMappingOutputTypeDef = TypedDict(
     "CreateSchemaMappingOutputTypeDef",
     {
         "description": str,
         "mappedInputFields": List[SchemaInputAttributeTypeDef],
         "schemaArn": str,
         "schemaName": str,
@@ -488,22 +477,20 @@
     "_OptionalListMatchingJobsInputListMatchingJobsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListMatchingJobsInputListMatchingJobsPaginateTypeDef(
     _RequiredListMatchingJobsInputListMatchingJobsPaginateTypeDef,
     _OptionalListMatchingJobsInputListMatchingJobsPaginateTypeDef,
 ):
     pass
 
-
 ListMatchingWorkflowsInputListMatchingWorkflowsPaginateTypeDef = TypedDict(
     "ListMatchingWorkflowsInputListMatchingWorkflowsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -546,21 +533,19 @@
     {
         "KMSArn": str,
         "applyNormalization": bool,
     },
     total=False,
 )
 
-
 class OutputSourceOutputTypeDef(
     _RequiredOutputSourceOutputTypeDef, _OptionalOutputSourceOutputTypeDef
 ):
     pass
 
-
 _RequiredOutputSourceTypeDef = TypedDict(
     "_RequiredOutputSourceTypeDef",
     {
         "output": Sequence[OutputAttributeTypeDef],
         "outputS3Path": str,
     },
 )
@@ -569,19 +554,17 @@
     {
         "KMSArn": str,
         "applyNormalization": bool,
     },
     total=False,
 )
 
-
 class OutputSourceTypeDef(_RequiredOutputSourceTypeDef, _OptionalOutputSourceTypeDef):
     pass
 
-
 RuleBasedPropertiesOutputTypeDef = TypedDict(
     "RuleBasedPropertiesOutputTypeDef",
     {
         "attributeMatchingModel": AttributeMatchingModelType,
         "rules": List[RuleOutputTypeDef],
     },
 )
@@ -590,14 +573,15 @@
     "RuleBasedPropertiesTypeDef",
     {
         "attributeMatchingModel": AttributeMatchingModelType,
         "rules": Sequence[RuleTypeDef],
     },
 )
 
+OutputSourceUnionTypeDef = Union[OutputSourceTypeDef, OutputSourceOutputTypeDef]
 ResolutionTechniquesOutputTypeDef = TypedDict(
     "ResolutionTechniquesOutputTypeDef",
     {
         "resolutionType": ResolutionTypeType,
         "ruleBasedProperties": RuleBasedPropertiesOutputTypeDef,
     },
     total=False,
@@ -659,15 +643,15 @@
     },
 )
 
 _RequiredCreateMatchingWorkflowInputRequestTypeDef = TypedDict(
     "_RequiredCreateMatchingWorkflowInputRequestTypeDef",
     {
         "inputSourceConfig": Sequence[InputSourceTypeDef],
-        "outputSourceConfig": Sequence[Union[OutputSourceTypeDef, OutputSourceOutputTypeDef]],
+        "outputSourceConfig": Sequence[OutputSourceUnionTypeDef],
         "resolutionTechniques": ResolutionTechniquesTypeDef,
         "roleArn": str,
         "workflowName": str,
     },
 )
 _OptionalCreateMatchingWorkflowInputRequestTypeDef = TypedDict(
     "_OptionalCreateMatchingWorkflowInputRequestTypeDef",
@@ -675,40 +659,40 @@
         "description": str,
         "incrementalRunConfig": IncrementalRunConfigTypeDef,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateMatchingWorkflowInputRequestTypeDef(
     _RequiredCreateMatchingWorkflowInputRequestTypeDef,
     _OptionalCreateMatchingWorkflowInputRequestTypeDef,
 ):
     pass
 
-
+ResolutionTechniquesUnionTypeDef = Union[
+    ResolutionTechniquesTypeDef, ResolutionTechniquesOutputTypeDef
+]
 _RequiredUpdateMatchingWorkflowInputRequestTypeDef = TypedDict(
     "_RequiredUpdateMatchingWorkflowInputRequestTypeDef",
     {
         "inputSourceConfig": Sequence[InputSourceTypeDef],
-        "outputSourceConfig": Sequence[Union[OutputSourceTypeDef, OutputSourceOutputTypeDef]],
+        "outputSourceConfig": Sequence[OutputSourceUnionTypeDef],
         "resolutionTechniques": ResolutionTechniquesTypeDef,
         "roleArn": str,
         "workflowName": str,
     },
 )
 _OptionalUpdateMatchingWorkflowInputRequestTypeDef = TypedDict(
     "_OptionalUpdateMatchingWorkflowInputRequestTypeDef",
     {
         "description": str,
         "incrementalRunConfig": IncrementalRunConfigTypeDef,
     },
     total=False,
 )
 
-
 class UpdateMatchingWorkflowInputRequestTypeDef(
     _RequiredUpdateMatchingWorkflowInputRequestTypeDef,
     _OptionalUpdateMatchingWorkflowInputRequestTypeDef,
 ):
     pass
```

### Comparing `mypy-boto3-entityresolution-1.28.15.post1/mypy_boto3_entityresolution/type_defs.pyi` & `mypy-boto3-entityresolution-1.28.16/mypy_boto3_entityresolution/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_entityresolution.type_defs import IncrementalRunConfigTypeDef
 
-    data: IncrementalRunConfigTypeDef = {...}
+    data: IncrementalRunConfigTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -27,14 +27,15 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "IncrementalRunConfigTypeDef",
     "InputSourceTypeDef",
     "ResponseMetadataTypeDef",
     "SchemaInputAttributeTypeDef",
     "DeleteMatchingWorkflowInputRequestTypeDef",
     "DeleteSchemaMappingInputRequestTypeDef",
@@ -73,20 +74,22 @@
     "ListSchemaMappingsInputListSchemaMappingsPaginateTypeDef",
     "ListMatchingWorkflowsOutputTypeDef",
     "ListSchemaMappingsOutputTypeDef",
     "OutputSourceOutputTypeDef",
     "OutputSourceTypeDef",
     "RuleBasedPropertiesOutputTypeDef",
     "RuleBasedPropertiesTypeDef",
+    "OutputSourceUnionTypeDef",
     "ResolutionTechniquesOutputTypeDef",
     "ResolutionTechniquesTypeDef",
     "CreateMatchingWorkflowOutputTypeDef",
     "GetMatchingWorkflowOutputTypeDef",
     "UpdateMatchingWorkflowOutputTypeDef",
     "CreateMatchingWorkflowInputRequestTypeDef",
+    "ResolutionTechniquesUnionTypeDef",
     "UpdateMatchingWorkflowInputRequestTypeDef",
 )
 
 IncrementalRunConfigTypeDef = TypedDict(
     "IncrementalRunConfigTypeDef",
     {
         "incrementalRunType": Literal["IMMEDIATE"],
@@ -105,17 +108,19 @@
     "_OptionalInputSourceTypeDef",
     {
         "applyNormalization": bool,
     },
     total=False,
 )
 
+
 class InputSourceTypeDef(_RequiredInputSourceTypeDef, _OptionalInputSourceTypeDef):
     pass
 
+
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -135,19 +140,21 @@
     {
         "groupName": str,
         "matchKey": str,
     },
     total=False,
 )
 
+
 class SchemaInputAttributeTypeDef(
     _RequiredSchemaInputAttributeTypeDef, _OptionalSchemaInputAttributeTypeDef
 ):
     pass
 
+
 DeleteMatchingWorkflowInputRequestTypeDef = TypedDict(
     "DeleteMatchingWorkflowInputRequestTypeDef",
     {
         "workflowName": str,
     },
 )
 
@@ -219,17 +226,19 @@
     "_OptionalJobSummaryTypeDef",
     {
         "endTime": datetime,
     },
     total=False,
 )
 
+
 class JobSummaryTypeDef(_RequiredJobSummaryTypeDef, _OptionalJobSummaryTypeDef):
     pass
 
+
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
@@ -247,19 +256,21 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListMatchingJobsInputRequestTypeDef(
     _RequiredListMatchingJobsInputRequestTypeDef, _OptionalListMatchingJobsInputRequestTypeDef
 ):
     pass
 
+
 ListMatchingWorkflowsInputRequestTypeDef = TypedDict(
     "ListMatchingWorkflowsInputRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -311,17 +322,19 @@
     "_OptionalOutputAttributeTypeDef",
     {
         "hashed": bool,
     },
     total=False,
 )
 
+
 class OutputAttributeTypeDef(_RequiredOutputAttributeTypeDef, _OptionalOutputAttributeTypeDef):
     pass
 
+
 RuleOutputTypeDef = TypedDict(
     "RuleOutputTypeDef",
     {
         "matchingKeys": List[str],
         "ruleName": str,
     },
 )
@@ -409,19 +422,21 @@
         "description": str,
         "mappedInputFields": Sequence[SchemaInputAttributeTypeDef],
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateSchemaMappingInputRequestTypeDef(
     _RequiredCreateSchemaMappingInputRequestTypeDef, _OptionalCreateSchemaMappingInputRequestTypeDef
 ):
     pass
 
+
 CreateSchemaMappingOutputTypeDef = TypedDict(
     "CreateSchemaMappingOutputTypeDef",
     {
         "description": str,
         "mappedInputFields": List[SchemaInputAttributeTypeDef],
         "schemaArn": str,
         "schemaName": str,
@@ -475,20 +490,22 @@
     "_OptionalListMatchingJobsInputListMatchingJobsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListMatchingJobsInputListMatchingJobsPaginateTypeDef(
     _RequiredListMatchingJobsInputListMatchingJobsPaginateTypeDef,
     _OptionalListMatchingJobsInputListMatchingJobsPaginateTypeDef,
 ):
     pass
 
+
 ListMatchingWorkflowsInputListMatchingWorkflowsPaginateTypeDef = TypedDict(
     "ListMatchingWorkflowsInputListMatchingWorkflowsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -531,19 +548,21 @@
     {
         "KMSArn": str,
         "applyNormalization": bool,
     },
     total=False,
 )
 
+
 class OutputSourceOutputTypeDef(
     _RequiredOutputSourceOutputTypeDef, _OptionalOutputSourceOutputTypeDef
 ):
     pass
 
+
 _RequiredOutputSourceTypeDef = TypedDict(
     "_RequiredOutputSourceTypeDef",
     {
         "output": Sequence[OutputAttributeTypeDef],
         "outputS3Path": str,
     },
 )
@@ -552,17 +571,19 @@
     {
         "KMSArn": str,
         "applyNormalization": bool,
     },
     total=False,
 )
 
+
 class OutputSourceTypeDef(_RequiredOutputSourceTypeDef, _OptionalOutputSourceTypeDef):
     pass
 
+
 RuleBasedPropertiesOutputTypeDef = TypedDict(
     "RuleBasedPropertiesOutputTypeDef",
     {
         "attributeMatchingModel": AttributeMatchingModelType,
         "rules": List[RuleOutputTypeDef],
     },
 )
@@ -571,14 +592,15 @@
     "RuleBasedPropertiesTypeDef",
     {
         "attributeMatchingModel": AttributeMatchingModelType,
         "rules": Sequence[RuleTypeDef],
     },
 )
 
+OutputSourceUnionTypeDef = Union[OutputSourceTypeDef, OutputSourceOutputTypeDef]
 ResolutionTechniquesOutputTypeDef = TypedDict(
     "ResolutionTechniquesOutputTypeDef",
     {
         "resolutionType": ResolutionTypeType,
         "ruleBasedProperties": RuleBasedPropertiesOutputTypeDef,
     },
     total=False,
@@ -640,15 +662,15 @@
     },
 )
 
 _RequiredCreateMatchingWorkflowInputRequestTypeDef = TypedDict(
     "_RequiredCreateMatchingWorkflowInputRequestTypeDef",
     {
         "inputSourceConfig": Sequence[InputSourceTypeDef],
-        "outputSourceConfig": Sequence[Union[OutputSourceTypeDef, OutputSourceOutputTypeDef]],
+        "outputSourceConfig": Sequence[OutputSourceUnionTypeDef],
         "resolutionTechniques": ResolutionTechniquesTypeDef,
         "roleArn": str,
         "workflowName": str,
     },
 )
 _OptionalCreateMatchingWorkflowInputRequestTypeDef = TypedDict(
     "_OptionalCreateMatchingWorkflowInputRequestTypeDef",
@@ -656,37 +678,43 @@
         "description": str,
         "incrementalRunConfig": IncrementalRunConfigTypeDef,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateMatchingWorkflowInputRequestTypeDef(
     _RequiredCreateMatchingWorkflowInputRequestTypeDef,
     _OptionalCreateMatchingWorkflowInputRequestTypeDef,
 ):
     pass
 
+
+ResolutionTechniquesUnionTypeDef = Union[
+    ResolutionTechniquesTypeDef, ResolutionTechniquesOutputTypeDef
+]
 _RequiredUpdateMatchingWorkflowInputRequestTypeDef = TypedDict(
     "_RequiredUpdateMatchingWorkflowInputRequestTypeDef",
     {
         "inputSourceConfig": Sequence[InputSourceTypeDef],
-        "outputSourceConfig": Sequence[Union[OutputSourceTypeDef, OutputSourceOutputTypeDef]],
+        "outputSourceConfig": Sequence[OutputSourceUnionTypeDef],
         "resolutionTechniques": ResolutionTechniquesTypeDef,
         "roleArn": str,
         "workflowName": str,
     },
 )
 _OptionalUpdateMatchingWorkflowInputRequestTypeDef = TypedDict(
     "_OptionalUpdateMatchingWorkflowInputRequestTypeDef",
     {
         "description": str,
         "incrementalRunConfig": IncrementalRunConfigTypeDef,
     },
     total=False,
 )
 
+
 class UpdateMatchingWorkflowInputRequestTypeDef(
     _RequiredUpdateMatchingWorkflowInputRequestTypeDef,
     _OptionalUpdateMatchingWorkflowInputRequestTypeDef,
 ):
     pass
```

### Comparing `mypy-boto3-entityresolution-1.28.15.post1/mypy_boto3_entityresolution.egg-info/PKG-INFO` & `mypy-boto3-entityresolution-1.28.16/mypy_boto3_entityresolution.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-entityresolution
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.EntityResolution 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.EntityResolution 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 entityresolution type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 entityresolution type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-entityresolution.svg?color=blue)](https://pypi.org/project/mypy-boto3-entityresolution)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-entityresolution)](https://pepy.tech/project/mypy-boto3-entityresolution)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EntityResolution 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution)
+[boto3.EntityResolution 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution)
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
 [mypy-boto3-entityresolution docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/).
 
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
@@ -327,20 +327,20 @@
 )
 
 
 def check_value(value: AttributeMatchingModelType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_entityresolution.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_entityresolution.type_defs import (
     IncrementalRunConfigTypeDef,
     InputSourceTypeDef,
     ResponseMetadataTypeDef,
     SchemaInputAttributeTypeDef,
@@ -381,25 +381,27 @@
     ListSchemaMappingsInputListSchemaMappingsPaginateTypeDef,
     ListMatchingWorkflowsOutputTypeDef,
     ListSchemaMappingsOutputTypeDef,
     OutputSourceOutputTypeDef,
     OutputSourceTypeDef,
     RuleBasedPropertiesOutputTypeDef,
     RuleBasedPropertiesTypeDef,
+    OutputSourceUnionTypeDef,
     ResolutionTechniquesOutputTypeDef,
     ResolutionTechniquesTypeDef,
     CreateMatchingWorkflowOutputTypeDef,
     GetMatchingWorkflowOutputTypeDef,
     UpdateMatchingWorkflowOutputTypeDef,
     CreateMatchingWorkflowInputRequestTypeDef,
+    ResolutionTechniquesUnionTypeDef,
     UpdateMatchingWorkflowInputRequestTypeDef,
 )
 
 
-def get_structure() -> IncrementalRunConfigTypeDef:
+def get_value() -> IncrementalRunConfigTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-entityresolution-1.28.15.post1/mypy_boto3_entityresolution.egg-info/SOURCES.txt` & `mypy-boto3-entityresolution-1.28.16/mypy_boto3_entityresolution.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-entityresolution-1.28.15.post1/setup.py` & `mypy-boto3-entityresolution-1.28.16/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-entityresolution",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_entityresolution"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.EntityResolution 1.28.15 service generated with"
-        " mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.EntityResolution 1.28.16 service generated with"
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
-    keywords="boto3 entityresolution type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 entityresolution type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_entityresolution": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

