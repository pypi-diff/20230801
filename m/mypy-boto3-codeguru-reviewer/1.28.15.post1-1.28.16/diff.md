# Comparing `tmp/mypy-boto3-codeguru-reviewer-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-codeguru-reviewer-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-codeguru-reviewer-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:47 2023, max compression
+gzip compressed data, was "mypy-boto3-codeguru-reviewer-1.28.16.tar", last modified: Tue Aug  1 11:36:28 2023, max compression
```

## Comparing `mypy-boto3-codeguru-reviewer-1.28.15.post1.tar` & `mypy-boto3-codeguru-reviewer-1.28.16.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:47.141071 mypy-boto3-codeguru-reviewer-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:40:44.000000 mypy-boto3-codeguru-reviewer-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16516 2023-07-29 10:02:47.137071 mypy-boto3-codeguru-reviewer-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14984 2023-07-29 09:40:44.000000 mypy-boto3-codeguru-reviewer-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:47.121071 mypy-boto3-codeguru-reviewer-1.28.15.post1/mypy_boto3_codeguru_reviewer/
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-29 09:40:44.000000 mypy-boto3-codeguru-reviewer-1.28.15.post1/mypy_boto3_codeguru_reviewer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-29 09:40:44.000000 mypy-boto3-codeguru-reviewer-1.28.15.post1/mypy_boto3_codeguru_reviewer/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-29 09:40:44.000000 mypy-boto3-codeguru-reviewer-1.28.15.post1/mypy_boto3_codeguru_reviewer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15164 2023-07-29 09:40:44.000000 mypy-boto3-codeguru-reviewer-1.28.15.post1/mypy_boto3_codeguru_reviewer/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15140 2023-07-29 09:40:44.000000 mypy-boto3-codeguru-reviewer-1.28.15.post1/mypy_boto3_codeguru_reviewer/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9742 2023-07-29 09:40:44.000000 mypy-boto3-codeguru-reviewer-1.28.15.post1/mypy_boto3_codeguru_reviewer/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9740 2023-07-29 09:40:44.000000 mypy-boto3-codeguru-reviewer-1.28.15.post1/mypy_boto3_codeguru_reviewer/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-07-29 09:40:44.000000 mypy-boto3-codeguru-reviewer-1.28.15.post1/mypy_boto3_codeguru_reviewer/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-07-29 09:40:44.000000 mypy-boto3-codeguru-reviewer-1.28.15.post1/mypy_boto3_codeguru_reviewer/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:40:44.000000 mypy-boto3-codeguru-reviewer-1.28.15.post1/mypy_boto3_codeguru_reviewer/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    20981 2023-07-29 09:40:46.000000 mypy-boto3-codeguru-reviewer-1.28.15.post1/mypy_boto3_codeguru_reviewer/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    20959 2023-07-29 09:40:46.000000 mypy-boto3-codeguru-reviewer-1.28.15.post1/mypy_boto3_codeguru_reviewer/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:40:44.000000 mypy-boto3-codeguru-reviewer-1.28.15.post1/mypy_boto3_codeguru_reviewer/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-07-29 09:40:44.000000 mypy-boto3-codeguru-reviewer-1.28.15.post1/mypy_boto3_codeguru_reviewer/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-07-29 09:40:44.000000 mypy-boto3-codeguru-reviewer-1.28.15.post1/mypy_boto3_codeguru_reviewer/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:47.137071 mypy-boto3-codeguru-reviewer-1.28.15.post1/mypy_boto3_codeguru_reviewer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16516 2023-07-29 10:02:46.000000 mypy-boto3-codeguru-reviewer-1.28.15.post1/mypy_boto3_codeguru_reviewer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-29 10:02:46.000000 mypy-boto3-codeguru-reviewer-1.28.15.post1/mypy_boto3_codeguru_reviewer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:46.000000 mypy-boto3-codeguru-reviewer-1.28.15.post1/mypy_boto3_codeguru_reviewer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:46.000000 mypy-boto3-codeguru-reviewer-1.28.15.post1/mypy_boto3_codeguru_reviewer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:46.000000 mypy-boto3-codeguru-reviewer-1.28.15.post1/mypy_boto3_codeguru_reviewer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-29 10:02:46.000000 mypy-boto3-codeguru-reviewer-1.28.15.post1/mypy_boto3_codeguru_reviewer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:47.141071 mypy-boto3-codeguru-reviewer-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-07-29 09:40:44.000000 mypy-boto3-codeguru-reviewer-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:28.396924 mypy-boto3-codeguru-reviewer-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:13:17.000000 mypy-boto3-codeguru-reviewer-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16506 2023-08-01 11:36:28.396924 mypy-boto3-codeguru-reviewer-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14983 2023-08-01 11:13:17.000000 mypy-boto3-codeguru-reviewer-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:28.380924 mypy-boto3-codeguru-reviewer-1.28.16/mypy_boto3_codeguru_reviewer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-08-01 11:13:17.000000 mypy-boto3-codeguru-reviewer-1.28.16/mypy_boto3_codeguru_reviewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-08-01 11:13:17.000000 mypy-boto3-codeguru-reviewer-1.28.16/mypy_boto3_codeguru_reviewer/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-08-01 11:13:17.000000 mypy-boto3-codeguru-reviewer-1.28.16/mypy_boto3_codeguru_reviewer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15164 2023-08-01 11:13:17.000000 mypy-boto3-codeguru-reviewer-1.28.16/mypy_boto3_codeguru_reviewer/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15140 2023-08-01 11:13:17.000000 mypy-boto3-codeguru-reviewer-1.28.16/mypy_boto3_codeguru_reviewer/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9742 2023-08-01 11:13:17.000000 mypy-boto3-codeguru-reviewer-1.28.16/mypy_boto3_codeguru_reviewer/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9740 2023-08-01 11:13:17.000000 mypy-boto3-codeguru-reviewer-1.28.16/mypy_boto3_codeguru_reviewer/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-08-01 11:13:17.000000 mypy-boto3-codeguru-reviewer-1.28.16/mypy_boto3_codeguru_reviewer/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-08-01 11:13:17.000000 mypy-boto3-codeguru-reviewer-1.28.16/mypy_boto3_codeguru_reviewer/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:13:17.000000 mypy-boto3-codeguru-reviewer-1.28.16/mypy_boto3_codeguru_reviewer/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    20979 2023-08-01 11:13:18.000000 mypy-boto3-codeguru-reviewer-1.28.16/mypy_boto3_codeguru_reviewer/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20957 2023-08-01 11:13:17.000000 mypy-boto3-codeguru-reviewer-1.28.16/mypy_boto3_codeguru_reviewer/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:13:17.000000 mypy-boto3-codeguru-reviewer-1.28.16/mypy_boto3_codeguru_reviewer/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-08-01 11:13:17.000000 mypy-boto3-codeguru-reviewer-1.28.16/mypy_boto3_codeguru_reviewer/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-08-01 11:13:17.000000 mypy-boto3-codeguru-reviewer-1.28.16/mypy_boto3_codeguru_reviewer/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:28.396924 mypy-boto3-codeguru-reviewer-1.28.16/mypy_boto3_codeguru_reviewer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16506 2023-08-01 11:36:28.000000 mypy-boto3-codeguru-reviewer-1.28.16/mypy_boto3_codeguru_reviewer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-08-01 11:36:28.000000 mypy-boto3-codeguru-reviewer-1.28.16/mypy_boto3_codeguru_reviewer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:28.000000 mypy-boto3-codeguru-reviewer-1.28.16/mypy_boto3_codeguru_reviewer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:28.000000 mypy-boto3-codeguru-reviewer-1.28.16/mypy_boto3_codeguru_reviewer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:28.000000 mypy-boto3-codeguru-reviewer-1.28.16/mypy_boto3_codeguru_reviewer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-01 11:36:28.000000 mypy-boto3-codeguru-reviewer-1.28.16/mypy_boto3_codeguru_reviewer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:28.396924 mypy-boto3-codeguru-reviewer-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-08-01 11:13:17.000000 mypy-boto3-codeguru-reviewer-1.28.16/setup.py
```

### Comparing `mypy-boto3-codeguru-reviewer-1.28.15.post1/LICENSE` & `mypy-boto3-codeguru-reviewer-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguru-reviewer-1.28.15.post1/PKG-INFO` & `mypy-boto3-codeguru-reviewer-1.28.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-codeguru-reviewer
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.CodeGuruReviewer 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.CodeGuruReviewer 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_reviewer/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 codeguru-reviewer type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 codeguru-reviewer type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codeguru-reviewer.svg?color=blue)](https://pypi.org/project/mypy-boto3-codeguru-reviewer)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_reviewer/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codeguru-reviewer)](https://pepy.tech/project/mypy-boto3-codeguru-reviewer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeGuruReviewer 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer)
+[boto3.CodeGuruReviewer 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer)
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
 [mypy-boto3-codeguru-reviewer docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_reviewer/).
 
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
@@ -354,20 +354,20 @@
 )
 
 
 def check_value(value: AnalysisTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_codeguru_reviewer.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_codeguru_reviewer.type_defs import (
     KMSKeyDetailsTypeDef,
     ResponseMetadataTypeDef,
     BranchDiffSourceCodeTypeTypeDef,
     CodeArtifactsTypeDef,
@@ -423,15 +423,15 @@
     CreateCodeReviewResponseTypeDef,
     DescribeCodeReviewResponseTypeDef,
     CodeReviewTypeTypeDef,
     CreateCodeReviewRequestRequestTypeDef,
 )
 
 
-def get_structure() -> KMSKeyDetailsTypeDef:
+def get_value() -> KMSKeyDetailsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-codeguru-reviewer-1.28.15.post1/README.md` & `mypy-boto3-codeguru-reviewer-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codeguru-reviewer.svg?color=blue)](https://pypi.org/project/mypy-boto3-codeguru-reviewer)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_reviewer/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codeguru-reviewer)](https://pepy.tech/project/mypy-boto3-codeguru-reviewer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeGuruReviewer 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer)
+[boto3.CodeGuruReviewer 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer)
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
 [mypy-boto3-codeguru-reviewer docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_reviewer/).
 
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
@@ -322,20 +322,20 @@
 )
 
 
 def check_value(value: AnalysisTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_codeguru_reviewer.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_codeguru_reviewer.type_defs import (
     KMSKeyDetailsTypeDef,
     ResponseMetadataTypeDef,
     BranchDiffSourceCodeTypeTypeDef,
     CodeArtifactsTypeDef,
@@ -391,15 +391,15 @@
     CreateCodeReviewResponseTypeDef,
     DescribeCodeReviewResponseTypeDef,
     CodeReviewTypeTypeDef,
     CreateCodeReviewRequestRequestTypeDef,
 )
 
 
-def get_structure() -> KMSKeyDetailsTypeDef:
+def get_value() -> KMSKeyDetailsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-codeguru-reviewer-1.28.15.post1/mypy_boto3_codeguru_reviewer/__init__.py` & `mypy-boto3-codeguru-reviewer-1.28.16/mypy_boto3_codeguru_reviewer/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguru-reviewer-1.28.15.post1/mypy_boto3_codeguru_reviewer/__init__.pyi` & `mypy-boto3-codeguru-reviewer-1.28.16/mypy_boto3_codeguru_reviewer/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguru-reviewer-1.28.15.post1/mypy_boto3_codeguru_reviewer/client.py` & `mypy-boto3-codeguru-reviewer-1.28.16/mypy_boto3_codeguru_reviewer/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguru-reviewer-1.28.15.post1/mypy_boto3_codeguru_reviewer/client.pyi` & `mypy-boto3-codeguru-reviewer-1.28.16/mypy_boto3_codeguru_reviewer/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguru-reviewer-1.28.15.post1/mypy_boto3_codeguru_reviewer/literals.py` & `mypy-boto3-codeguru-reviewer-1.28.16/mypy_boto3_codeguru_reviewer/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguru-reviewer-1.28.15.post1/mypy_boto3_codeguru_reviewer/literals.pyi` & `mypy-boto3-codeguru-reviewer-1.28.16/mypy_boto3_codeguru_reviewer/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguru-reviewer-1.28.15.post1/mypy_boto3_codeguru_reviewer/paginator.py` & `mypy-boto3-codeguru-reviewer-1.28.16/mypy_boto3_codeguru_reviewer/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguru-reviewer-1.28.15.post1/mypy_boto3_codeguru_reviewer/paginator.pyi` & `mypy-boto3-codeguru-reviewer-1.28.16/mypy_boto3_codeguru_reviewer/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguru-reviewer-1.28.15.post1/mypy_boto3_codeguru_reviewer/type_defs.py` & `mypy-boto3-codeguru-reviewer-1.28.16/mypy_boto3_codeguru_reviewer/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_reviewer/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_codeguru_reviewer.type_defs import KMSKeyDetailsTypeDef
 
-    data: KMSKeyDetailsTypeDef = {...}
+    data: KMSKeyDetailsTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
```

### Comparing `mypy-boto3-codeguru-reviewer-1.28.15.post1/mypy_boto3_codeguru_reviewer/type_defs.pyi` & `mypy-boto3-codeguru-reviewer-1.28.16/mypy_boto3_codeguru_reviewer/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_reviewer/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_codeguru_reviewer.type_defs import KMSKeyDetailsTypeDef
 
-    data: KMSKeyDetailsTypeDef = {...}
+    data: KMSKeyDetailsTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
```

### Comparing `mypy-boto3-codeguru-reviewer-1.28.15.post1/mypy_boto3_codeguru_reviewer/waiter.py` & `mypy-boto3-codeguru-reviewer-1.28.16/mypy_boto3_codeguru_reviewer/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguru-reviewer-1.28.15.post1/mypy_boto3_codeguru_reviewer/waiter.pyi` & `mypy-boto3-codeguru-reviewer-1.28.16/mypy_boto3_codeguru_reviewer/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguru-reviewer-1.28.15.post1/mypy_boto3_codeguru_reviewer.egg-info/PKG-INFO` & `mypy-boto3-codeguru-reviewer-1.28.16/mypy_boto3_codeguru_reviewer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-codeguru-reviewer
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.CodeGuruReviewer 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.CodeGuruReviewer 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_reviewer/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 codeguru-reviewer type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 codeguru-reviewer type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codeguru-reviewer.svg?color=blue)](https://pypi.org/project/mypy-boto3-codeguru-reviewer)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_reviewer/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codeguru-reviewer)](https://pepy.tech/project/mypy-boto3-codeguru-reviewer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeGuruReviewer 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer)
+[boto3.CodeGuruReviewer 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer)
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
 [mypy-boto3-codeguru-reviewer docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_reviewer/).
 
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
@@ -354,20 +354,20 @@
 )
 
 
 def check_value(value: AnalysisTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_codeguru_reviewer.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_codeguru_reviewer.type_defs import (
     KMSKeyDetailsTypeDef,
     ResponseMetadataTypeDef,
     BranchDiffSourceCodeTypeTypeDef,
     CodeArtifactsTypeDef,
@@ -423,15 +423,15 @@
     CreateCodeReviewResponseTypeDef,
     DescribeCodeReviewResponseTypeDef,
     CodeReviewTypeTypeDef,
     CreateCodeReviewRequestRequestTypeDef,
 )
 
 
-def get_structure() -> KMSKeyDetailsTypeDef:
+def get_value() -> KMSKeyDetailsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-codeguru-reviewer-1.28.15.post1/mypy_boto3_codeguru_reviewer.egg-info/SOURCES.txt` & `mypy-boto3-codeguru-reviewer-1.28.16/mypy_boto3_codeguru_reviewer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguru-reviewer-1.28.15.post1/setup.py` & `mypy-boto3-codeguru-reviewer-1.28.16/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-codeguru-reviewer",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_codeguru_reviewer"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CodeGuruReviewer 1.28.15 service generated with"
-        " mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.CodeGuruReviewer 1.28.16 service generated with"
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
-    keywords="boto3 codeguru-reviewer type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 codeguru-reviewer type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_codeguru_reviewer": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_reviewer/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

