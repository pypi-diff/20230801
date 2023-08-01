# Comparing `tmp/mypy-boto3-amplifyuibuilder-1.28.16.tar.gz` & `tmp/mypy-boto3-amplifyuibuilder-1.28.16.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-amplifyuibuilder-1.28.16.tar", last modified: Mon Jul 31 19:32:46 2023, max compression
+gzip compressed data, was "mypy-boto3-amplifyuibuilder-1.28.16.post1.tar", last modified: Tue Aug  1 11:36:08 2023, max compression
```

## Comparing `mypy-boto3-amplifyuibuilder-1.28.16.tar` & `mypy-boto3-amplifyuibuilder-1.28.16.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:32:46.246207 mypy-boto3-amplifyuibuilder-1.28.16/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-31 19:32:02.000000 mypy-boto3-amplifyuibuilder-1.28.16/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19423 2023-07-31 19:32:46.246207 mypy-boto3-amplifyuibuilder-1.28.16/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17900 2023-07-31 19:32:02.000000 mypy-boto3-amplifyuibuilder-1.28.16/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:32:46.242207 mypy-boto3-amplifyuibuilder-1.28.16/mypy_boto3_amplifyuibuilder/
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-07-31 19:32:02.000000 mypy-boto3-amplifyuibuilder-1.28.16/mypy_boto3_amplifyuibuilder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-07-31 19:32:02.000000 mypy-boto3-amplifyuibuilder-1.28.16/mypy_boto3_amplifyuibuilder/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-31 19:32:02.000000 mypy-boto3-amplifyuibuilder-1.28.16/mypy_boto3_amplifyuibuilder/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22014 2023-07-31 19:32:02.000000 mypy-boto3-amplifyuibuilder-1.28.16/mypy_boto3_amplifyuibuilder/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    21975 2023-07-31 19:32:02.000000 mypy-boto3-amplifyuibuilder-1.28.16/mypy_boto3_amplifyuibuilder/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10363 2023-07-31 19:32:03.000000 mypy-boto3-amplifyuibuilder-1.28.16/mypy_boto3_amplifyuibuilder/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10361 2023-07-31 19:32:03.000000 mypy-boto3-amplifyuibuilder-1.28.16/mypy_boto3_amplifyuibuilder/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8460 2023-07-31 19:32:03.000000 mypy-boto3-amplifyuibuilder-1.28.16/mypy_boto3_amplifyuibuilder/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8451 2023-07-31 19:32:03.000000 mypy-boto3-amplifyuibuilder-1.28.16/mypy_boto3_amplifyuibuilder/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 19:32:02.000000 mypy-boto3-amplifyuibuilder-1.28.16/mypy_boto3_amplifyuibuilder/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    60153 2023-07-31 19:32:04.000000 mypy-boto3-amplifyuibuilder-1.28.16/mypy_boto3_amplifyuibuilder/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    60043 2023-07-31 19:32:04.000000 mypy-boto3-amplifyuibuilder-1.28.16/mypy_boto3_amplifyuibuilder/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-31 19:32:02.000000 mypy-boto3-amplifyuibuilder-1.28.16/mypy_boto3_amplifyuibuilder/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:32:46.246207 mypy-boto3-amplifyuibuilder-1.28.16/mypy_boto3_amplifyuibuilder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19423 2023-07-31 19:32:46.000000 mypy-boto3-amplifyuibuilder-1.28.16/mypy_boto3_amplifyuibuilder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-31 19:32:46.000000 mypy-boto3-amplifyuibuilder-1.28.16/mypy_boto3_amplifyuibuilder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 19:32:46.000000 mypy-boto3-amplifyuibuilder-1.28.16/mypy_boto3_amplifyuibuilder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 19:32:46.000000 mypy-boto3-amplifyuibuilder-1.28.16/mypy_boto3_amplifyuibuilder.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-31 19:32:46.000000 mypy-boto3-amplifyuibuilder-1.28.16/mypy_boto3_amplifyuibuilder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-31 19:32:46.000000 mypy-boto3-amplifyuibuilder-1.28.16/mypy_boto3_amplifyuibuilder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 19:32:46.246207 mypy-boto3-amplifyuibuilder-1.28.16/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-07-31 19:32:02.000000 mypy-boto3-amplifyuibuilder-1.28.16/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:08.432956 mypy-boto3-amplifyuibuilder-1.28.16.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:10:17.000000 mypy-boto3-amplifyuibuilder-1.28.16.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19425 2023-08-01 11:36:08.432956 mypy-boto3-amplifyuibuilder-1.28.16.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17899 2023-08-01 11:10:17.000000 mypy-boto3-amplifyuibuilder-1.28.16.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:08.428956 mypy-boto3-amplifyuibuilder-1.28.16.post1/mypy_boto3_amplifyuibuilder/
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-08-01 11:10:17.000000 mypy-boto3-amplifyuibuilder-1.28.16.post1/mypy_boto3_amplifyuibuilder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-08-01 11:10:17.000000 mypy-boto3-amplifyuibuilder-1.28.16.post1/mypy_boto3_amplifyuibuilder/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-01 11:10:17.000000 mypy-boto3-amplifyuibuilder-1.28.16.post1/mypy_boto3_amplifyuibuilder/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22014 2023-08-01 11:10:17.000000 mypy-boto3-amplifyuibuilder-1.28.16.post1/mypy_boto3_amplifyuibuilder/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21975 2023-08-01 11:10:17.000000 mypy-boto3-amplifyuibuilder-1.28.16.post1/mypy_boto3_amplifyuibuilder/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10363 2023-08-01 11:10:17.000000 mypy-boto3-amplifyuibuilder-1.28.16.post1/mypy_boto3_amplifyuibuilder/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10361 2023-08-01 11:10:17.000000 mypy-boto3-amplifyuibuilder-1.28.16.post1/mypy_boto3_amplifyuibuilder/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8460 2023-08-01 11:10:17.000000 mypy-boto3-amplifyuibuilder-1.28.16.post1/mypy_boto3_amplifyuibuilder/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8451 2023-08-01 11:10:17.000000 mypy-boto3-amplifyuibuilder-1.28.16.post1/mypy_boto3_amplifyuibuilder/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:10:17.000000 mypy-boto3-amplifyuibuilder-1.28.16.post1/mypy_boto3_amplifyuibuilder/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    60151 2023-08-01 11:10:19.000000 mypy-boto3-amplifyuibuilder-1.28.16.post1/mypy_boto3_amplifyuibuilder/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60041 2023-08-01 11:10:18.000000 mypy-boto3-amplifyuibuilder-1.28.16.post1/mypy_boto3_amplifyuibuilder/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-01 11:10:17.000000 mypy-boto3-amplifyuibuilder-1.28.16.post1/mypy_boto3_amplifyuibuilder/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:08.432956 mypy-boto3-amplifyuibuilder-1.28.16.post1/mypy_boto3_amplifyuibuilder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19425 2023-08-01 11:36:08.000000 mypy-boto3-amplifyuibuilder-1.28.16.post1/mypy_boto3_amplifyuibuilder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-08-01 11:36:08.000000 mypy-boto3-amplifyuibuilder-1.28.16.post1/mypy_boto3_amplifyuibuilder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:08.000000 mypy-boto3-amplifyuibuilder-1.28.16.post1/mypy_boto3_amplifyuibuilder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:08.000000 mypy-boto3-amplifyuibuilder-1.28.16.post1/mypy_boto3_amplifyuibuilder.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:08.000000 mypy-boto3-amplifyuibuilder-1.28.16.post1/mypy_boto3_amplifyuibuilder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-01 11:36:08.000000 mypy-boto3-amplifyuibuilder-1.28.16.post1/mypy_boto3_amplifyuibuilder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:08.432956 mypy-boto3-amplifyuibuilder-1.28.16.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-08-01 11:10:17.000000 mypy-boto3-amplifyuibuilder-1.28.16.post1/setup.py
```

### Comparing `mypy-boto3-amplifyuibuilder-1.28.16/LICENSE` & `mypy-boto3-amplifyuibuilder-1.28.16.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplifyuibuilder-1.28.16/PKG-INFO` & `mypy-boto3-amplifyuibuilder-1.28.16.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-amplifyuibuilder
-Version: 1.28.16
-Summary: Type annotations for boto3.AmplifyUIBuilder 1.28.16 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16.post1
+Summary: Type annotations for boto3.AmplifyUIBuilder 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 amplifyuibuilder type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 amplifyuibuilder type-annotations botocore mypy typeshed autocomplete
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
 [mypy-boto3-amplifyuibuilder docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/).
 
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
@@ -346,20 +346,20 @@
 )
 
 
 def check_value(value: CodegenGenericDataFieldDataTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_amplifyuibuilder.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_amplifyuibuilder.type_defs import (
     MutationActionSetStateParameterTypeDef,
     GraphQLRenderConfigTypeDef,
     CodegenFeatureFlagsTypeDef,
     CodegenGenericDataEnumOutputTypeDef,
@@ -502,15 +502,15 @@
     GetFormResponseTypeDef,
     UpdateFormResponseTypeDef,
     CreateFormRequestRequestTypeDef,
     UpdateFormRequestRequestTypeDef,
 )
 
 
-def get_structure() -> MutationActionSetStateParameterTypeDef:
+def get_value() -> MutationActionSetStateParameterTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-amplifyuibuilder-1.28.16/README.md` & `mypy-boto3-amplifyuibuilder-1.28.16.post1/README.md`

 * *Files 1% similar despite different names*

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
 [mypy-boto3-amplifyuibuilder docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/).
 
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
@@ -314,20 +314,20 @@
 )
 
 
 def check_value(value: CodegenGenericDataFieldDataTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_amplifyuibuilder.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_amplifyuibuilder.type_defs import (
     MutationActionSetStateParameterTypeDef,
     GraphQLRenderConfigTypeDef,
     CodegenFeatureFlagsTypeDef,
     CodegenGenericDataEnumOutputTypeDef,
@@ -470,15 +470,15 @@
     GetFormResponseTypeDef,
     UpdateFormResponseTypeDef,
     CreateFormRequestRequestTypeDef,
     UpdateFormRequestRequestTypeDef,
 )
 
 
-def get_structure() -> MutationActionSetStateParameterTypeDef:
+def get_value() -> MutationActionSetStateParameterTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-amplifyuibuilder-1.28.16/mypy_boto3_amplifyuibuilder/__init__.py` & `mypy-boto3-amplifyuibuilder-1.28.16.post1/mypy_boto3_amplifyuibuilder/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplifyuibuilder-1.28.16/mypy_boto3_amplifyuibuilder/__init__.pyi` & `mypy-boto3-amplifyuibuilder-1.28.16.post1/mypy_boto3_amplifyuibuilder/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplifyuibuilder-1.28.16/mypy_boto3_amplifyuibuilder/__main__.py` & `mypy-boto3-amplifyuibuilder-1.28.16.post1/mypy_boto3_amplifyuibuilder/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.AmplifyUIBuilder 1.28.16\nVersion:         1.28.16\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.AmplifyUIBuilder 1.28.16\nVersion:        "
+        " 1.28.16.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder\nOther"
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

### Comparing `mypy-boto3-amplifyuibuilder-1.28.16/mypy_boto3_amplifyuibuilder/client.py` & `mypy-boto3-amplifyuibuilder-1.28.16.post1/mypy_boto3_amplifyuibuilder/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplifyuibuilder-1.28.16/mypy_boto3_amplifyuibuilder/client.pyi` & `mypy-boto3-amplifyuibuilder-1.28.16.post1/mypy_boto3_amplifyuibuilder/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplifyuibuilder-1.28.16/mypy_boto3_amplifyuibuilder/literals.py` & `mypy-boto3-amplifyuibuilder-1.28.16.post1/mypy_boto3_amplifyuibuilder/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplifyuibuilder-1.28.16/mypy_boto3_amplifyuibuilder/literals.pyi` & `mypy-boto3-amplifyuibuilder-1.28.16.post1/mypy_boto3_amplifyuibuilder/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplifyuibuilder-1.28.16/mypy_boto3_amplifyuibuilder/paginator.py` & `mypy-boto3-amplifyuibuilder-1.28.16.post1/mypy_boto3_amplifyuibuilder/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplifyuibuilder-1.28.16/mypy_boto3_amplifyuibuilder/paginator.pyi` & `mypy-boto3-amplifyuibuilder-1.28.16.post1/mypy_boto3_amplifyuibuilder/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplifyuibuilder-1.28.16/mypy_boto3_amplifyuibuilder/type_defs.py` & `mypy-boto3-amplifyuibuilder-1.28.16.post1/mypy_boto3_amplifyuibuilder/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_amplifyuibuilder.type_defs import MutationActionSetStateParameterTypeDef
 
-    data: MutationActionSetStateParameterTypeDef = {...}
+    data: MutationActionSetStateParameterTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence
 
 from .literals import (
```

### Comparing `mypy-boto3-amplifyuibuilder-1.28.16/mypy_boto3_amplifyuibuilder/type_defs.pyi` & `mypy-boto3-amplifyuibuilder-1.28.16.post1/mypy_boto3_amplifyuibuilder/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_amplifyuibuilder.type_defs import MutationActionSetStateParameterTypeDef
 
-    data: MutationActionSetStateParameterTypeDef = {...}
+    data: MutationActionSetStateParameterTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence
 
 from .literals import (
```

### Comparing `mypy-boto3-amplifyuibuilder-1.28.16/mypy_boto3_amplifyuibuilder.egg-info/PKG-INFO` & `mypy-boto3-amplifyuibuilder-1.28.16.post1/mypy_boto3_amplifyuibuilder.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-amplifyuibuilder
-Version: 1.28.16
-Summary: Type annotations for boto3.AmplifyUIBuilder 1.28.16 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16.post1
+Summary: Type annotations for boto3.AmplifyUIBuilder 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 amplifyuibuilder type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 amplifyuibuilder type-annotations botocore mypy typeshed autocomplete
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
 [mypy-boto3-amplifyuibuilder docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/).
 
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
@@ -346,20 +346,20 @@
 )
 
 
 def check_value(value: CodegenGenericDataFieldDataTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_amplifyuibuilder.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_amplifyuibuilder.type_defs import (
     MutationActionSetStateParameterTypeDef,
     GraphQLRenderConfigTypeDef,
     CodegenFeatureFlagsTypeDef,
     CodegenGenericDataEnumOutputTypeDef,
@@ -502,15 +502,15 @@
     GetFormResponseTypeDef,
     UpdateFormResponseTypeDef,
     CreateFormRequestRequestTypeDef,
     UpdateFormRequestRequestTypeDef,
 )
 
 
-def get_structure() -> MutationActionSetStateParameterTypeDef:
+def get_value() -> MutationActionSetStateParameterTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-amplifyuibuilder-1.28.16/mypy_boto3_amplifyuibuilder.egg-info/SOURCES.txt` & `mypy-boto3-amplifyuibuilder-1.28.16.post1/mypy_boto3_amplifyuibuilder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplifyuibuilder-1.28.16/setup.py` & `mypy-boto3-amplifyuibuilder-1.28.16.post1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-amplifyuibuilder",
-    version="1.28.16",
+    version="1.28.16.post1",
     packages=["mypy_boto3_amplifyuibuilder"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.AmplifyUIBuilder 1.28.16 service generated with"
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
-    keywords="boto3 amplifyuibuilder type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 amplifyuibuilder type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_amplifyuibuilder": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

