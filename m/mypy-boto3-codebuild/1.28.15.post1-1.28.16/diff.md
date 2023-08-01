# Comparing `tmp/mypy-boto3-codebuild-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-codebuild-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-codebuild-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:45 2023, max compression
+gzip compressed data, was "mypy-boto3-codebuild-1.28.16.tar", last modified: Tue Aug  1 11:36:25 2023, max compression
```

## Comparing `mypy-boto3-codebuild-1.28.15.post1.tar` & `mypy-boto3-codebuild-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:45.141064 mypy-boto3-codebuild-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:40:28.000000 mypy-boto3-codebuild-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21235 2023-07-29 10:02:45.141064 mypy-boto3-codebuild-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19734 2023-07-29 09:40:28.000000 mypy-boto3-codebuild-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:45.141064 mypy-boto3-codebuild-1.28.15.post1/mypy_boto3_codebuild/
--rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-07-29 09:40:28.000000 mypy-boto3-codebuild-1.28.15.post1/mypy_boto3_codebuild/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-07-29 09:40:28.000000 mypy-boto3-codebuild-1.28.15.post1/mypy_boto3_codebuild/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-29 09:40:28.000000 mypy-boto3-codebuild-1.28.15.post1/mypy_boto3_codebuild/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42055 2023-07-29 09:40:28.000000 mypy-boto3-codebuild-1.28.15.post1/mypy_boto3_codebuild/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    41991 2023-07-29 09:40:28.000000 mypy-boto3-codebuild-1.28.15.post1/mypy_boto3_codebuild/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14183 2023-07-29 09:40:29.000000 mypy-boto3-codebuild-1.28.15.post1/mypy_boto3_codebuild/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14181 2023-07-29 09:40:28.000000 mypy-boto3-codebuild-1.28.15.post1/mypy_boto3_codebuild/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15290 2023-07-29 09:40:28.000000 mypy-boto3-codebuild-1.28.15.post1/mypy_boto3_codebuild/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    15276 2023-07-29 09:40:28.000000 mypy-boto3-codebuild-1.28.15.post1/mypy_boto3_codebuild/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:40:28.000000 mypy-boto3-codebuild-1.28.15.post1/mypy_boto3_codebuild/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    59346 2023-07-29 09:40:31.000000 mypy-boto3-codebuild-1.28.15.post1/mypy_boto3_codebuild/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    59283 2023-07-29 09:40:29.000000 mypy-boto3-codebuild-1.28.15.post1/mypy_boto3_codebuild/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:40:28.000000 mypy-boto3-codebuild-1.28.15.post1/mypy_boto3_codebuild/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:45.141064 mypy-boto3-codebuild-1.28.15.post1/mypy_boto3_codebuild.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21235 2023-07-29 10:02:44.000000 mypy-boto3-codebuild-1.28.15.post1/mypy_boto3_codebuild.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-29 10:02:44.000000 mypy-boto3-codebuild-1.28.15.post1/mypy_boto3_codebuild.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:44.000000 mypy-boto3-codebuild-1.28.15.post1/mypy_boto3_codebuild.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:44.000000 mypy-boto3-codebuild-1.28.15.post1/mypy_boto3_codebuild.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:44.000000 mypy-boto3-codebuild-1.28.15.post1/mypy_boto3_codebuild.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-29 10:02:44.000000 mypy-boto3-codebuild-1.28.15.post1/mypy_boto3_codebuild.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:45.141064 mypy-boto3-codebuild-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-07-29 09:40:27.000000 mypy-boto3-codebuild-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:25.672928 mypy-boto3-codebuild-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:13:00.000000 mypy-boto3-codebuild-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21359 2023-08-01 11:36:25.672928 mypy-boto3-codebuild-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19867 2023-08-01 11:13:00.000000 mypy-boto3-codebuild-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:25.668928 mypy-boto3-codebuild-1.28.16/mypy_boto3_codebuild/
+-rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-08-01 11:13:00.000000 mypy-boto3-codebuild-1.28.16/mypy_boto3_codebuild/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-08-01 11:13:00.000000 mypy-boto3-codebuild-1.28.16/mypy_boto3_codebuild/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-08-01 11:13:00.000000 mypy-boto3-codebuild-1.28.16/mypy_boto3_codebuild/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41506 2023-08-01 11:13:00.000000 mypy-boto3-codebuild-1.28.16/mypy_boto3_codebuild/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41442 2023-08-01 11:13:00.000000 mypy-boto3-codebuild-1.28.16/mypy_boto3_codebuild/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14183 2023-08-01 11:13:02.000000 mypy-boto3-codebuild-1.28.16/mypy_boto3_codebuild/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14181 2023-08-01 11:13:02.000000 mypy-boto3-codebuild-1.28.16/mypy_boto3_codebuild/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15290 2023-08-01 11:13:00.000000 mypy-boto3-codebuild-1.28.16/mypy_boto3_codebuild/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15276 2023-08-01 11:13:00.000000 mypy-boto3-codebuild-1.28.16/mypy_boto3_codebuild/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:13:00.000000 mypy-boto3-codebuild-1.28.16/mypy_boto3_codebuild/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    59865 2023-08-01 11:13:03.000000 mypy-boto3-codebuild-1.28.16/mypy_boto3_codebuild/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59802 2023-08-01 11:13:03.000000 mypy-boto3-codebuild-1.28.16/mypy_boto3_codebuild/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:13:00.000000 mypy-boto3-codebuild-1.28.16/mypy_boto3_codebuild/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:25.672928 mypy-boto3-codebuild-1.28.16/mypy_boto3_codebuild.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21359 2023-08-01 11:36:25.000000 mypy-boto3-codebuild-1.28.16/mypy_boto3_codebuild.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-08-01 11:36:25.000000 mypy-boto3-codebuild-1.28.16/mypy_boto3_codebuild.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:25.000000 mypy-boto3-codebuild-1.28.16/mypy_boto3_codebuild.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:25.000000 mypy-boto3-codebuild-1.28.16/mypy_boto3_codebuild.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:25.000000 mypy-boto3-codebuild-1.28.16/mypy_boto3_codebuild.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-01 11:36:25.000000 mypy-boto3-codebuild-1.28.16/mypy_boto3_codebuild.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:25.672928 mypy-boto3-codebuild-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-08-01 11:13:00.000000 mypy-boto3-codebuild-1.28.16/setup.py
```

### Comparing `mypy-boto3-codebuild-1.28.15.post1/LICENSE` & `mypy-boto3-codebuild-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codebuild-1.28.15.post1/PKG-INFO` & `mypy-boto3-codebuild-1.28.16/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-codebuild
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.CodeBuild 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.CodeBuild 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 codebuild type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 codebuild type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codebuild.svg?color=blue)](https://pypi.org/project/mypy-boto3-codebuild)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codebuild)](https://pepy.tech/project/mypy-boto3-codebuild)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeBuild 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild)
+[boto3.CodeBuild 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild)
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
 [mypy-boto3-codebuild docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild/).
 
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
@@ -396,20 +396,20 @@
 )
 
 
 def check_value(value: ArtifactNamespaceType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_codebuild.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_codebuild.type_defs import (
     BatchDeleteBuildsInputRequestTypeDef,
     BuildNotDeletedTypeDef,
     ResponseMetadataTypeDef,
     BatchGetBuildBatchesInputRequestTypeDef,
@@ -500,14 +500,16 @@
     ProjectBuildBatchConfigTypeDef,
     ListBuildBatchesForProjectInputRequestTypeDef,
     ListBuildBatchesInputRequestTypeDef,
     BuildBatchPhaseTypeDef,
     BuildPhaseTypeDef,
     BuildSummaryTypeDef,
     DescribeCodeCoveragesOutputTypeDef,
+    ProjectCacheUnionTypeDef,
+    VpcConfigUnionTypeDef,
     CreateWebhookInputRequestTypeDef,
     UpdateWebhookInputRequestTypeDef,
     WebhookTypeDef,
     DescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef,
     ListBuildBatchesForProjectInputListBuildBatchesForProjectPaginateTypeDef,
     ListBuildBatchesInputListBuildBatchesPaginateTypeDef,
     ListBuildsForProjectInputListBuildsForProjectPaginateTypeDef,
@@ -528,18 +530,20 @@
     ListSourceCredentialsOutputTypeDef,
     LogsConfigTypeDef,
     LogsLocationTypeDef,
     ProjectEnvironmentOutputTypeDef,
     ProjectEnvironmentTypeDef,
     ProjectSourceTypeDef,
     ReportExportConfigTypeDef,
+    ProjectBuildBatchConfigUnionTypeDef,
     BuildGroupTypeDef,
     CreateWebhookOutputTypeDef,
     UpdateWebhookOutputTypeDef,
     EnvironmentPlatformTypeDef,
+    ProjectEnvironmentUnionTypeDef,
     BuildTypeDef,
     CreateProjectInputRequestTypeDef,
     ProjectTypeDef,
     StartBuildBatchInputRequestTypeDef,
     StartBuildInputRequestTypeDef,
     UpdateProjectInputRequestTypeDef,
     CreateReportGroupInputRequestTypeDef,
@@ -562,15 +566,15 @@
     BatchGetBuildBatchesOutputTypeDef,
     RetryBuildBatchOutputTypeDef,
     StartBuildBatchOutputTypeDef,
     StopBuildBatchOutputTypeDef,
 )
 
 
-def get_structure() -> BatchDeleteBuildsInputRequestTypeDef:
+def get_value() -> BatchDeleteBuildsInputRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-codebuild-1.28.15.post1/README.md` & `mypy-boto3-codebuild-1.28.16/mypy_boto3_codebuild.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-codebuild
+Version: 1.28.16
+Summary: Type annotations for boto3.CodeBuild 1.28.16 service generated with mypy-boto3-builder 7.17.1
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 codebuild type-annotations botocore mypy typeshed autocomplete
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
 <a id="mypy-boto3-codebuild"></a>
 
 # mypy-boto3-codebuild
 
 [![PyPI - mypy-boto3-codebuild](https://img.shields.io/pypi/v/mypy-boto3-codebuild.svg?color=blue)](https://pypi.org/project/mypy-boto3-codebuild)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codebuild.svg?color=blue)](https://pypi.org/project/mypy-boto3-codebuild)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codebuild)](https://pepy.tech/project/mypy-boto3-codebuild)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeBuild 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild)
+[boto3.CodeBuild 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild)
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
 [mypy-boto3-codebuild docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild/).
 
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
@@ -364,20 +396,20 @@
 )
 
 
 def check_value(value: ArtifactNamespaceType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_codebuild.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_codebuild.type_defs import (
     BatchDeleteBuildsInputRequestTypeDef,
     BuildNotDeletedTypeDef,
     ResponseMetadataTypeDef,
     BatchGetBuildBatchesInputRequestTypeDef,
@@ -468,14 +500,16 @@
     ProjectBuildBatchConfigTypeDef,
     ListBuildBatchesForProjectInputRequestTypeDef,
     ListBuildBatchesInputRequestTypeDef,
     BuildBatchPhaseTypeDef,
     BuildPhaseTypeDef,
     BuildSummaryTypeDef,
     DescribeCodeCoveragesOutputTypeDef,
+    ProjectCacheUnionTypeDef,
+    VpcConfigUnionTypeDef,
     CreateWebhookInputRequestTypeDef,
     UpdateWebhookInputRequestTypeDef,
     WebhookTypeDef,
     DescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef,
     ListBuildBatchesForProjectInputListBuildBatchesForProjectPaginateTypeDef,
     ListBuildBatchesInputListBuildBatchesPaginateTypeDef,
     ListBuildsForProjectInputListBuildsForProjectPaginateTypeDef,
@@ -496,18 +530,20 @@
     ListSourceCredentialsOutputTypeDef,
     LogsConfigTypeDef,
     LogsLocationTypeDef,
     ProjectEnvironmentOutputTypeDef,
     ProjectEnvironmentTypeDef,
     ProjectSourceTypeDef,
     ReportExportConfigTypeDef,
+    ProjectBuildBatchConfigUnionTypeDef,
     BuildGroupTypeDef,
     CreateWebhookOutputTypeDef,
     UpdateWebhookOutputTypeDef,
     EnvironmentPlatformTypeDef,
+    ProjectEnvironmentUnionTypeDef,
     BuildTypeDef,
     CreateProjectInputRequestTypeDef,
     ProjectTypeDef,
     StartBuildBatchInputRequestTypeDef,
     StartBuildInputRequestTypeDef,
     UpdateProjectInputRequestTypeDef,
     CreateReportGroupInputRequestTypeDef,
@@ -530,15 +566,15 @@
     BatchGetBuildBatchesOutputTypeDef,
     RetryBuildBatchOutputTypeDef,
     StartBuildBatchOutputTypeDef,
     StopBuildBatchOutputTypeDef,
 )
 
 
-def get_structure() -> BatchDeleteBuildsInputRequestTypeDef:
+def get_value() -> BatchDeleteBuildsInputRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-codebuild-1.28.15.post1/mypy_boto3_codebuild/__init__.py` & `mypy-boto3-codebuild-1.28.16/mypy_boto3_codebuild/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codebuild-1.28.15.post1/mypy_boto3_codebuild/__init__.pyi` & `mypy-boto3-codebuild-1.28.16/mypy_boto3_codebuild/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codebuild-1.28.15.post1/mypy_boto3_codebuild/__main__.py` & `mypy-boto3-codebuild-1.28.16/mypy_boto3_codebuild/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CodeBuild 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.CodeBuild 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild\nOther"
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

### Comparing `mypy-boto3-codebuild-1.28.15.post1/mypy_boto3_codebuild/client.py` & `mypy-boto3-codebuild-1.28.16/mypy_boto3_codebuild/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_codebuild.client import CodeBuildClient
 
     session = Session()
     client: CodeBuildClient = session.client("codebuild")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AuthTypeType,
     ComputeTypeType,
     EnvironmentTypeType,
@@ -81,20 +81,17 @@
     ListReportsForReportGroupOutputTypeDef,
     ListReportsOutputTypeDef,
     ListSharedProjectsOutputTypeDef,
     ListSharedReportGroupsOutputTypeDef,
     ListSourceCredentialsOutputTypeDef,
     LogsConfigTypeDef,
     ProjectArtifactsTypeDef,
-    ProjectBuildBatchConfigOutputTypeDef,
-    ProjectBuildBatchConfigTypeDef,
-    ProjectCacheOutputTypeDef,
-    ProjectCacheTypeDef,
-    ProjectEnvironmentOutputTypeDef,
-    ProjectEnvironmentTypeDef,
+    ProjectBuildBatchConfigUnionTypeDef,
+    ProjectCacheUnionTypeDef,
+    ProjectEnvironmentUnionTypeDef,
     ProjectFileSystemLocationTypeDef,
     ProjectSourceTypeDef,
     ProjectSourceVersionTypeDef,
     PutResourcePolicyOutputTypeDef,
     RegistryCredentialTypeDef,
     ReportExportConfigTypeDef,
     ReportFilterTypeDef,
@@ -107,16 +104,15 @@
     StopBuildOutputTypeDef,
     TagTypeDef,
     TestCaseFilterTypeDef,
     UpdateProjectOutputTypeDef,
     UpdateProjectVisibilityOutputTypeDef,
     UpdateReportGroupOutputTypeDef,
     UpdateWebhookOutputTypeDef,
-    VpcConfigOutputTypeDef,
-    VpcConfigTypeDef,
+    VpcConfigUnionTypeDef,
     WebhookFilterTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -227,33 +223,31 @@
 
     def create_project(
         self,
         *,
         name: str,
         source: ProjectSourceTypeDef,
         artifacts: ProjectArtifactsTypeDef,
-        environment: Union[ProjectEnvironmentTypeDef, ProjectEnvironmentOutputTypeDef],
+        environment: ProjectEnvironmentUnionTypeDef,
         serviceRole: str,
         description: str = ...,
         secondarySources: Sequence[ProjectSourceTypeDef] = ...,
         sourceVersion: str = ...,
         secondarySourceVersions: Sequence[ProjectSourceVersionTypeDef] = ...,
         secondaryArtifacts: Sequence[ProjectArtifactsTypeDef] = ...,
-        cache: Union[ProjectCacheTypeDef, ProjectCacheOutputTypeDef] = ...,
+        cache: ProjectCacheUnionTypeDef = ...,
         timeoutInMinutes: int = ...,
         queuedTimeoutInMinutes: int = ...,
         encryptionKey: str = ...,
         tags: Sequence[TagTypeDef] = ...,
-        vpcConfig: Union[VpcConfigTypeDef, VpcConfigOutputTypeDef] = ...,
+        vpcConfig: VpcConfigUnionTypeDef = ...,
         badgeEnabled: bool = ...,
         logsConfig: LogsConfigTypeDef = ...,
         fileSystemLocations: Sequence[ProjectFileSystemLocationTypeDef] = ...,
-        buildBatchConfig: Union[
-            ProjectBuildBatchConfigTypeDef, ProjectBuildBatchConfigOutputTypeDef
-        ] = ...,
+        buildBatchConfig: ProjectBuildBatchConfigUnionTypeDef = ...,
         concurrentBuildLimit: int = ...
     ) -> CreateProjectOutputTypeDef:
         """
         Creates a build project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Client.create_project)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild/client/#create_project)
@@ -657,15 +651,15 @@
         insecureSslOverride: bool = ...,
         reportBuildStatusOverride: bool = ...,
         buildStatusConfigOverride: BuildStatusConfigTypeDef = ...,
         environmentTypeOverride: EnvironmentTypeType = ...,
         imageOverride: str = ...,
         computeTypeOverride: ComputeTypeType = ...,
         certificateOverride: str = ...,
-        cacheOverride: Union[ProjectCacheTypeDef, ProjectCacheOutputTypeDef] = ...,
+        cacheOverride: ProjectCacheUnionTypeDef = ...,
         serviceRoleOverride: str = ...,
         privilegedModeOverride: bool = ...,
         timeoutInMinutesOverride: int = ...,
         queuedTimeoutInMinutesOverride: int = ...,
         encryptionKeyOverride: str = ...,
         idempotencyToken: str = ...,
         logsConfigOverride: LogsConfigTypeDef = ...,
@@ -698,27 +692,25 @@
         buildspecOverride: str = ...,
         insecureSslOverride: bool = ...,
         reportBuildBatchStatusOverride: bool = ...,
         environmentTypeOverride: EnvironmentTypeType = ...,
         imageOverride: str = ...,
         computeTypeOverride: ComputeTypeType = ...,
         certificateOverride: str = ...,
-        cacheOverride: Union[ProjectCacheTypeDef, ProjectCacheOutputTypeDef] = ...,
+        cacheOverride: ProjectCacheUnionTypeDef = ...,
         serviceRoleOverride: str = ...,
         privilegedModeOverride: bool = ...,
         buildTimeoutInMinutesOverride: int = ...,
         queuedTimeoutInMinutesOverride: int = ...,
         encryptionKeyOverride: str = ...,
         idempotencyToken: str = ...,
         logsConfigOverride: LogsConfigTypeDef = ...,
         registryCredentialOverride: RegistryCredentialTypeDef = ...,
         imagePullCredentialsTypeOverride: ImagePullCredentialsTypeType = ...,
-        buildBatchConfigOverride: Union[
-            ProjectBuildBatchConfigTypeDef, ProjectBuildBatchConfigOutputTypeDef
-        ] = ...,
+        buildBatchConfigOverride: ProjectBuildBatchConfigUnionTypeDef = ...,
         debugSessionEnabled: bool = ...
     ) -> StartBuildBatchOutputTypeDef:
         """
         Starts a batch build for a project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Client.start_build_batch)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild/client/#start_build_batch)
@@ -747,28 +739,26 @@
         description: str = ...,
         source: ProjectSourceTypeDef = ...,
         secondarySources: Sequence[ProjectSourceTypeDef] = ...,
         sourceVersion: str = ...,
         secondarySourceVersions: Sequence[ProjectSourceVersionTypeDef] = ...,
         artifacts: ProjectArtifactsTypeDef = ...,
         secondaryArtifacts: Sequence[ProjectArtifactsTypeDef] = ...,
-        cache: Union[ProjectCacheTypeDef, ProjectCacheOutputTypeDef] = ...,
-        environment: Union[ProjectEnvironmentTypeDef, ProjectEnvironmentOutputTypeDef] = ...,
+        cache: ProjectCacheUnionTypeDef = ...,
+        environment: ProjectEnvironmentUnionTypeDef = ...,
         serviceRole: str = ...,
         timeoutInMinutes: int = ...,
         queuedTimeoutInMinutes: int = ...,
         encryptionKey: str = ...,
         tags: Sequence[TagTypeDef] = ...,
-        vpcConfig: Union[VpcConfigTypeDef, VpcConfigOutputTypeDef] = ...,
+        vpcConfig: VpcConfigUnionTypeDef = ...,
         badgeEnabled: bool = ...,
         logsConfig: LogsConfigTypeDef = ...,
         fileSystemLocations: Sequence[ProjectFileSystemLocationTypeDef] = ...,
-        buildBatchConfig: Union[
-            ProjectBuildBatchConfigTypeDef, ProjectBuildBatchConfigOutputTypeDef
-        ] = ...,
+        buildBatchConfig: ProjectBuildBatchConfigUnionTypeDef = ...,
         concurrentBuildLimit: int = ...
     ) -> UpdateProjectOutputTypeDef:
         """
         Changes the settings of a build project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Client.update_project)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild/client/#update_project)
```

### Comparing `mypy-boto3-codebuild-1.28.15.post1/mypy_boto3_codebuild/client.pyi` & `mypy-boto3-codebuild-1.28.16/mypy_boto3_codebuild/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_codebuild.client import CodeBuildClient
 
     session = Session()
     client: CodeBuildClient = session.client("codebuild")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AuthTypeType,
     ComputeTypeType,
     EnvironmentTypeType,
@@ -81,20 +81,17 @@
     ListReportsForReportGroupOutputTypeDef,
     ListReportsOutputTypeDef,
     ListSharedProjectsOutputTypeDef,
     ListSharedReportGroupsOutputTypeDef,
     ListSourceCredentialsOutputTypeDef,
     LogsConfigTypeDef,
     ProjectArtifactsTypeDef,
-    ProjectBuildBatchConfigOutputTypeDef,
-    ProjectBuildBatchConfigTypeDef,
-    ProjectCacheOutputTypeDef,
-    ProjectCacheTypeDef,
-    ProjectEnvironmentOutputTypeDef,
-    ProjectEnvironmentTypeDef,
+    ProjectBuildBatchConfigUnionTypeDef,
+    ProjectCacheUnionTypeDef,
+    ProjectEnvironmentUnionTypeDef,
     ProjectFileSystemLocationTypeDef,
     ProjectSourceTypeDef,
     ProjectSourceVersionTypeDef,
     PutResourcePolicyOutputTypeDef,
     RegistryCredentialTypeDef,
     ReportExportConfigTypeDef,
     ReportFilterTypeDef,
@@ -107,16 +104,15 @@
     StopBuildOutputTypeDef,
     TagTypeDef,
     TestCaseFilterTypeDef,
     UpdateProjectOutputTypeDef,
     UpdateProjectVisibilityOutputTypeDef,
     UpdateReportGroupOutputTypeDef,
     UpdateWebhookOutputTypeDef,
-    VpcConfigOutputTypeDef,
-    VpcConfigTypeDef,
+    VpcConfigUnionTypeDef,
     WebhookFilterTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -214,33 +210,31 @@
         """
     def create_project(
         self,
         *,
         name: str,
         source: ProjectSourceTypeDef,
         artifacts: ProjectArtifactsTypeDef,
-        environment: Union[ProjectEnvironmentTypeDef, ProjectEnvironmentOutputTypeDef],
+        environment: ProjectEnvironmentUnionTypeDef,
         serviceRole: str,
         description: str = ...,
         secondarySources: Sequence[ProjectSourceTypeDef] = ...,
         sourceVersion: str = ...,
         secondarySourceVersions: Sequence[ProjectSourceVersionTypeDef] = ...,
         secondaryArtifacts: Sequence[ProjectArtifactsTypeDef] = ...,
-        cache: Union[ProjectCacheTypeDef, ProjectCacheOutputTypeDef] = ...,
+        cache: ProjectCacheUnionTypeDef = ...,
         timeoutInMinutes: int = ...,
         queuedTimeoutInMinutes: int = ...,
         encryptionKey: str = ...,
         tags: Sequence[TagTypeDef] = ...,
-        vpcConfig: Union[VpcConfigTypeDef, VpcConfigOutputTypeDef] = ...,
+        vpcConfig: VpcConfigUnionTypeDef = ...,
         badgeEnabled: bool = ...,
         logsConfig: LogsConfigTypeDef = ...,
         fileSystemLocations: Sequence[ProjectFileSystemLocationTypeDef] = ...,
-        buildBatchConfig: Union[
-            ProjectBuildBatchConfigTypeDef, ProjectBuildBatchConfigOutputTypeDef
-        ] = ...,
+        buildBatchConfig: ProjectBuildBatchConfigUnionTypeDef = ...,
         concurrentBuildLimit: int = ...
     ) -> CreateProjectOutputTypeDef:
         """
         Creates a build project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Client.create_project)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild/client/#create_project)
@@ -612,15 +606,15 @@
         insecureSslOverride: bool = ...,
         reportBuildStatusOverride: bool = ...,
         buildStatusConfigOverride: BuildStatusConfigTypeDef = ...,
         environmentTypeOverride: EnvironmentTypeType = ...,
         imageOverride: str = ...,
         computeTypeOverride: ComputeTypeType = ...,
         certificateOverride: str = ...,
-        cacheOverride: Union[ProjectCacheTypeDef, ProjectCacheOutputTypeDef] = ...,
+        cacheOverride: ProjectCacheUnionTypeDef = ...,
         serviceRoleOverride: str = ...,
         privilegedModeOverride: bool = ...,
         timeoutInMinutesOverride: int = ...,
         queuedTimeoutInMinutesOverride: int = ...,
         encryptionKeyOverride: str = ...,
         idempotencyToken: str = ...,
         logsConfigOverride: LogsConfigTypeDef = ...,
@@ -652,27 +646,25 @@
         buildspecOverride: str = ...,
         insecureSslOverride: bool = ...,
         reportBuildBatchStatusOverride: bool = ...,
         environmentTypeOverride: EnvironmentTypeType = ...,
         imageOverride: str = ...,
         computeTypeOverride: ComputeTypeType = ...,
         certificateOverride: str = ...,
-        cacheOverride: Union[ProjectCacheTypeDef, ProjectCacheOutputTypeDef] = ...,
+        cacheOverride: ProjectCacheUnionTypeDef = ...,
         serviceRoleOverride: str = ...,
         privilegedModeOverride: bool = ...,
         buildTimeoutInMinutesOverride: int = ...,
         queuedTimeoutInMinutesOverride: int = ...,
         encryptionKeyOverride: str = ...,
         idempotencyToken: str = ...,
         logsConfigOverride: LogsConfigTypeDef = ...,
         registryCredentialOverride: RegistryCredentialTypeDef = ...,
         imagePullCredentialsTypeOverride: ImagePullCredentialsTypeType = ...,
-        buildBatchConfigOverride: Union[
-            ProjectBuildBatchConfigTypeDef, ProjectBuildBatchConfigOutputTypeDef
-        ] = ...,
+        buildBatchConfigOverride: ProjectBuildBatchConfigUnionTypeDef = ...,
         debugSessionEnabled: bool = ...
     ) -> StartBuildBatchOutputTypeDef:
         """
         Starts a batch build for a project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Client.start_build_batch)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild/client/#start_build_batch)
@@ -698,28 +690,26 @@
         description: str = ...,
         source: ProjectSourceTypeDef = ...,
         secondarySources: Sequence[ProjectSourceTypeDef] = ...,
         sourceVersion: str = ...,
         secondarySourceVersions: Sequence[ProjectSourceVersionTypeDef] = ...,
         artifacts: ProjectArtifactsTypeDef = ...,
         secondaryArtifacts: Sequence[ProjectArtifactsTypeDef] = ...,
-        cache: Union[ProjectCacheTypeDef, ProjectCacheOutputTypeDef] = ...,
-        environment: Union[ProjectEnvironmentTypeDef, ProjectEnvironmentOutputTypeDef] = ...,
+        cache: ProjectCacheUnionTypeDef = ...,
+        environment: ProjectEnvironmentUnionTypeDef = ...,
         serviceRole: str = ...,
         timeoutInMinutes: int = ...,
         queuedTimeoutInMinutes: int = ...,
         encryptionKey: str = ...,
         tags: Sequence[TagTypeDef] = ...,
-        vpcConfig: Union[VpcConfigTypeDef, VpcConfigOutputTypeDef] = ...,
+        vpcConfig: VpcConfigUnionTypeDef = ...,
         badgeEnabled: bool = ...,
         logsConfig: LogsConfigTypeDef = ...,
         fileSystemLocations: Sequence[ProjectFileSystemLocationTypeDef] = ...,
-        buildBatchConfig: Union[
-            ProjectBuildBatchConfigTypeDef, ProjectBuildBatchConfigOutputTypeDef
-        ] = ...,
+        buildBatchConfig: ProjectBuildBatchConfigUnionTypeDef = ...,
         concurrentBuildLimit: int = ...
     ) -> UpdateProjectOutputTypeDef:
         """
         Changes the settings of a build project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Client.update_project)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild/client/#update_project)
```

### Comparing `mypy-boto3-codebuild-1.28.15.post1/mypy_boto3_codebuild/literals.py` & `mypy-boto3-codebuild-1.28.16/mypy_boto3_codebuild/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codebuild-1.28.15.post1/mypy_boto3_codebuild/literals.pyi` & `mypy-boto3-codebuild-1.28.16/mypy_boto3_codebuild/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codebuild-1.28.15.post1/mypy_boto3_codebuild/paginator.py` & `mypy-boto3-codebuild-1.28.16/mypy_boto3_codebuild/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codebuild-1.28.15.post1/mypy_boto3_codebuild/paginator.pyi` & `mypy-boto3-codebuild-1.28.16/mypy_boto3_codebuild/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codebuild-1.28.15.post1/mypy_boto3_codebuild/type_defs.py` & `mypy-boto3-codebuild-1.28.16/mypy_boto3_codebuild/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_codebuild.type_defs import BatchDeleteBuildsInputRequestTypeDef
 
-    data: BatchDeleteBuildsInputRequestTypeDef = {...}
+    data: BatchDeleteBuildsInputRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence
+from typing import Dict, List, Sequence, Union
 
 from .literals import (
     ArtifactNamespaceType,
     ArtifactPackagingType,
     ArtifactsTypeType,
     AuthTypeType,
     BatchReportModeTypeType,
@@ -155,14 +155,16 @@
     "ProjectBuildBatchConfigTypeDef",
     "ListBuildBatchesForProjectInputRequestTypeDef",
     "ListBuildBatchesInputRequestTypeDef",
     "BuildBatchPhaseTypeDef",
     "BuildPhaseTypeDef",
     "BuildSummaryTypeDef",
     "DescribeCodeCoveragesOutputTypeDef",
+    "ProjectCacheUnionTypeDef",
+    "VpcConfigUnionTypeDef",
     "CreateWebhookInputRequestTypeDef",
     "UpdateWebhookInputRequestTypeDef",
     "WebhookTypeDef",
     "DescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef",
     "ListBuildBatchesForProjectInputListBuildBatchesForProjectPaginateTypeDef",
     "ListBuildBatchesInputListBuildBatchesPaginateTypeDef",
     "ListBuildsForProjectInputListBuildsForProjectPaginateTypeDef",
@@ -183,18 +185,20 @@
     "ListSourceCredentialsOutputTypeDef",
     "LogsConfigTypeDef",
     "LogsLocationTypeDef",
     "ProjectEnvironmentOutputTypeDef",
     "ProjectEnvironmentTypeDef",
     "ProjectSourceTypeDef",
     "ReportExportConfigTypeDef",
+    "ProjectBuildBatchConfigUnionTypeDef",
     "BuildGroupTypeDef",
     "CreateWebhookOutputTypeDef",
     "UpdateWebhookOutputTypeDef",
     "EnvironmentPlatformTypeDef",
+    "ProjectEnvironmentUnionTypeDef",
     "BuildTypeDef",
     "CreateProjectInputRequestTypeDef",
     "ProjectTypeDef",
     "StartBuildBatchInputRequestTypeDef",
     "StartBuildInputRequestTypeDef",
     "UpdateProjectInputRequestTypeDef",
     "CreateReportGroupInputRequestTypeDef",
@@ -1287,14 +1291,16 @@
     {
         "nextToken": str,
         "codeCoverages": List[CodeCoverageTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ProjectCacheUnionTypeDef = Union[ProjectCacheTypeDef, ProjectCacheOutputTypeDef]
+VpcConfigUnionTypeDef = Union[VpcConfigTypeDef, VpcConfigOutputTypeDef]
 _RequiredCreateWebhookInputRequestTypeDef = TypedDict(
     "_RequiredCreateWebhookInputRequestTypeDef",
     {
         "projectName": str,
     },
 )
 _OptionalCreateWebhookInputRequestTypeDef = TypedDict(
@@ -1732,14 +1738,17 @@
     {
         "exportConfigType": ReportExportConfigTypeType,
         "s3Destination": S3ReportExportConfigTypeDef,
     },
     total=False,
 )
 
+ProjectBuildBatchConfigUnionTypeDef = Union[
+    ProjectBuildBatchConfigTypeDef, ProjectBuildBatchConfigOutputTypeDef
+]
 BuildGroupTypeDef = TypedDict(
     "BuildGroupTypeDef",
     {
         "identifier": str,
         "dependsOn": List[str],
         "ignoreFailure": bool,
         "currentBuildSummary": BuildSummaryTypeDef,
@@ -1769,14 +1778,15 @@
     {
         "platform": PlatformTypeType,
         "languages": List[EnvironmentLanguageTypeDef],
     },
     total=False,
 )
 
+ProjectEnvironmentUnionTypeDef = Union[ProjectEnvironmentTypeDef, ProjectEnvironmentOutputTypeDef]
 BuildTypeDef = TypedDict(
     "BuildTypeDef",
     {
         "id": str,
         "arn": str,
         "buildNumber": int,
         "startTime": datetime,
```

### Comparing `mypy-boto3-codebuild-1.28.15.post1/mypy_boto3_codebuild/type_defs.pyi` & `mypy-boto3-codebuild-1.28.16/mypy_boto3_codebuild/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_codebuild.type_defs import BatchDeleteBuildsInputRequestTypeDef
 
-    data: BatchDeleteBuildsInputRequestTypeDef = {...}
+    data: BatchDeleteBuildsInputRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence
+from typing import Dict, List, Sequence, Union
 
 from .literals import (
     ArtifactNamespaceType,
     ArtifactPackagingType,
     ArtifactsTypeType,
     AuthTypeType,
     BatchReportModeTypeType,
@@ -154,14 +154,16 @@
     "ProjectBuildBatchConfigTypeDef",
     "ListBuildBatchesForProjectInputRequestTypeDef",
     "ListBuildBatchesInputRequestTypeDef",
     "BuildBatchPhaseTypeDef",
     "BuildPhaseTypeDef",
     "BuildSummaryTypeDef",
     "DescribeCodeCoveragesOutputTypeDef",
+    "ProjectCacheUnionTypeDef",
+    "VpcConfigUnionTypeDef",
     "CreateWebhookInputRequestTypeDef",
     "UpdateWebhookInputRequestTypeDef",
     "WebhookTypeDef",
     "DescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef",
     "ListBuildBatchesForProjectInputListBuildBatchesForProjectPaginateTypeDef",
     "ListBuildBatchesInputListBuildBatchesPaginateTypeDef",
     "ListBuildsForProjectInputListBuildsForProjectPaginateTypeDef",
@@ -182,18 +184,20 @@
     "ListSourceCredentialsOutputTypeDef",
     "LogsConfigTypeDef",
     "LogsLocationTypeDef",
     "ProjectEnvironmentOutputTypeDef",
     "ProjectEnvironmentTypeDef",
     "ProjectSourceTypeDef",
     "ReportExportConfigTypeDef",
+    "ProjectBuildBatchConfigUnionTypeDef",
     "BuildGroupTypeDef",
     "CreateWebhookOutputTypeDef",
     "UpdateWebhookOutputTypeDef",
     "EnvironmentPlatformTypeDef",
+    "ProjectEnvironmentUnionTypeDef",
     "BuildTypeDef",
     "CreateProjectInputRequestTypeDef",
     "ProjectTypeDef",
     "StartBuildBatchInputRequestTypeDef",
     "StartBuildInputRequestTypeDef",
     "UpdateProjectInputRequestTypeDef",
     "CreateReportGroupInputRequestTypeDef",
@@ -1258,14 +1262,16 @@
     {
         "nextToken": str,
         "codeCoverages": List[CodeCoverageTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ProjectCacheUnionTypeDef = Union[ProjectCacheTypeDef, ProjectCacheOutputTypeDef]
+VpcConfigUnionTypeDef = Union[VpcConfigTypeDef, VpcConfigOutputTypeDef]
 _RequiredCreateWebhookInputRequestTypeDef = TypedDict(
     "_RequiredCreateWebhookInputRequestTypeDef",
     {
         "projectName": str,
     },
 )
 _OptionalCreateWebhookInputRequestTypeDef = TypedDict(
@@ -1681,14 +1687,17 @@
     {
         "exportConfigType": ReportExportConfigTypeType,
         "s3Destination": S3ReportExportConfigTypeDef,
     },
     total=False,
 )
 
+ProjectBuildBatchConfigUnionTypeDef = Union[
+    ProjectBuildBatchConfigTypeDef, ProjectBuildBatchConfigOutputTypeDef
+]
 BuildGroupTypeDef = TypedDict(
     "BuildGroupTypeDef",
     {
         "identifier": str,
         "dependsOn": List[str],
         "ignoreFailure": bool,
         "currentBuildSummary": BuildSummaryTypeDef,
@@ -1718,14 +1727,15 @@
     {
         "platform": PlatformTypeType,
         "languages": List[EnvironmentLanguageTypeDef],
     },
     total=False,
 )
 
+ProjectEnvironmentUnionTypeDef = Union[ProjectEnvironmentTypeDef, ProjectEnvironmentOutputTypeDef]
 BuildTypeDef = TypedDict(
     "BuildTypeDef",
     {
         "id": str,
         "arn": str,
         "buildNumber": int,
         "startTime": datetime,
```

### Comparing `mypy-boto3-codebuild-1.28.15.post1/mypy_boto3_codebuild.egg-info/PKG-INFO` & `mypy-boto3-codebuild-1.28.16/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,61 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-codebuild
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.CodeBuild 1.28.15 service generated with mypy-boto3-builder 7.16.2
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 codebuild type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-codebuild"></a>
 
 # mypy-boto3-codebuild
 
 [![PyPI - mypy-boto3-codebuild](https://img.shields.io/pypi/v/mypy-boto3-codebuild.svg?color=blue)](https://pypi.org/project/mypy-boto3-codebuild)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codebuild.svg?color=blue)](https://pypi.org/project/mypy-boto3-codebuild)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codebuild)](https://pepy.tech/project/mypy-boto3-codebuild)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeBuild 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild)
+[boto3.CodeBuild 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild)
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
 [mypy-boto3-codebuild docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild/).
 
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
@@ -396,20 +364,20 @@
 )
 
 
 def check_value(value: ArtifactNamespaceType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_codebuild.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_codebuild.type_defs import (
     BatchDeleteBuildsInputRequestTypeDef,
     BuildNotDeletedTypeDef,
     ResponseMetadataTypeDef,
     BatchGetBuildBatchesInputRequestTypeDef,
@@ -500,14 +468,16 @@
     ProjectBuildBatchConfigTypeDef,
     ListBuildBatchesForProjectInputRequestTypeDef,
     ListBuildBatchesInputRequestTypeDef,
     BuildBatchPhaseTypeDef,
     BuildPhaseTypeDef,
     BuildSummaryTypeDef,
     DescribeCodeCoveragesOutputTypeDef,
+    ProjectCacheUnionTypeDef,
+    VpcConfigUnionTypeDef,
     CreateWebhookInputRequestTypeDef,
     UpdateWebhookInputRequestTypeDef,
     WebhookTypeDef,
     DescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef,
     ListBuildBatchesForProjectInputListBuildBatchesForProjectPaginateTypeDef,
     ListBuildBatchesInputListBuildBatchesPaginateTypeDef,
     ListBuildsForProjectInputListBuildsForProjectPaginateTypeDef,
@@ -528,18 +498,20 @@
     ListSourceCredentialsOutputTypeDef,
     LogsConfigTypeDef,
     LogsLocationTypeDef,
     ProjectEnvironmentOutputTypeDef,
     ProjectEnvironmentTypeDef,
     ProjectSourceTypeDef,
     ReportExportConfigTypeDef,
+    ProjectBuildBatchConfigUnionTypeDef,
     BuildGroupTypeDef,
     CreateWebhookOutputTypeDef,
     UpdateWebhookOutputTypeDef,
     EnvironmentPlatformTypeDef,
+    ProjectEnvironmentUnionTypeDef,
     BuildTypeDef,
     CreateProjectInputRequestTypeDef,
     ProjectTypeDef,
     StartBuildBatchInputRequestTypeDef,
     StartBuildInputRequestTypeDef,
     UpdateProjectInputRequestTypeDef,
     CreateReportGroupInputRequestTypeDef,
@@ -562,15 +534,15 @@
     BatchGetBuildBatchesOutputTypeDef,
     RetryBuildBatchOutputTypeDef,
     StartBuildBatchOutputTypeDef,
     StopBuildBatchOutputTypeDef,
 )
 
 
-def get_structure() -> BatchDeleteBuildsInputRequestTypeDef:
+def get_value() -> BatchDeleteBuildsInputRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-codebuild-1.28.15.post1/mypy_boto3_codebuild.egg-info/SOURCES.txt` & `mypy-boto3-codebuild-1.28.16/mypy_boto3_codebuild.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codebuild-1.28.15.post1/setup.py` & `mypy-boto3-codebuild-1.28.16/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-codebuild",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_codebuild"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CodeBuild 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.2"
+        "Type annotations for boto3.CodeBuild 1.28.16 service generated with mypy-boto3-builder"
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
-    keywords="boto3 codebuild type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 codebuild type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_codebuild": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

