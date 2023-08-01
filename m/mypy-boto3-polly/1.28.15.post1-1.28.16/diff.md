# Comparing `tmp/mypy-boto3-polly-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-polly-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-polly-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:54 2023, max compression
+gzip compressed data, was "mypy-boto3-polly-1.28.16.tar", last modified: Tue Aug  1 11:37:34 2023, max compression
```

## Comparing `mypy-boto3-polly-1.28.15.post1.tar` & `mypy-boto3-polly-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:54.653343 mypy-boto3-polly-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:53:28.000000 mypy-boto3-polly-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13866 2023-07-29 10:03:54.653343 mypy-boto3-polly-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12381 2023-07-29 09:53:28.000000 mypy-boto3-polly-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:54.641343 mypy-boto3-polly-1.28.15.post1/mypy_boto3_polly/
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-29 09:53:28.000000 mypy-boto3-polly-1.28.15.post1/mypy_boto3_polly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-07-29 09:53:28.000000 mypy-boto3-polly-1.28.15.post1/mypy_boto3_polly/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-29 09:53:28.000000 mypy-boto3-polly-1.28.15.post1/mypy_boto3_polly/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11430 2023-07-29 09:53:28.000000 mypy-boto3-polly-1.28.15.post1/mypy_boto3_polly/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11411 2023-07-29 09:53:28.000000 mypy-boto3-polly-1.28.15.post1/mypy_boto3_polly/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10709 2023-07-29 09:53:28.000000 mypy-boto3-polly-1.28.15.post1/mypy_boto3_polly/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10707 2023-07-29 09:53:28.000000 mypy-boto3-polly-1.28.15.post1/mypy_boto3_polly/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-07-29 09:53:28.000000 mypy-boto3-polly-1.28.15.post1/mypy_boto3_polly/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-07-29 09:53:28.000000 mypy-boto3-polly-1.28.15.post1/mypy_boto3_polly/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:53:28.000000 mypy-boto3-polly-1.28.15.post1/mypy_boto3_polly/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     8900 2023-07-29 09:53:28.000000 mypy-boto3-polly-1.28.15.post1/mypy_boto3_polly/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8895 2023-07-29 09:53:28.000000 mypy-boto3-polly-1.28.15.post1/mypy_boto3_polly/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:53:28.000000 mypy-boto3-polly-1.28.15.post1/mypy_boto3_polly/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:54.653343 mypy-boto3-polly-1.28.15.post1/mypy_boto3_polly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13866 2023-07-29 10:03:54.000000 mypy-boto3-polly-1.28.15.post1/mypy_boto3_polly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-29 10:03:54.000000 mypy-boto3-polly-1.28.15.post1/mypy_boto3_polly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:54.000000 mypy-boto3-polly-1.28.15.post1/mypy_boto3_polly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:54.000000 mypy-boto3-polly-1.28.15.post1/mypy_boto3_polly.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:54.000000 mypy-boto3-polly-1.28.15.post1/mypy_boto3_polly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-29 10:03:54.000000 mypy-boto3-polly-1.28.15.post1/mypy_boto3_polly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:54.653343 mypy-boto3-polly-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-07-29 09:53:28.000000 mypy-boto3-polly-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:34.324786 mypy-boto3-polly-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:26:31.000000 mypy-boto3-polly-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13856 2023-08-01 11:37:34.324786 mypy-boto3-polly-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12380 2023-08-01 11:26:31.000000 mypy-boto3-polly-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:34.320786 mypy-boto3-polly-1.28.16/mypy_boto3_polly/
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-08-01 11:26:31.000000 mypy-boto3-polly-1.28.16/mypy_boto3_polly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-08-01 11:26:31.000000 mypy-boto3-polly-1.28.16/mypy_boto3_polly/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-08-01 11:26:31.000000 mypy-boto3-polly-1.28.16/mypy_boto3_polly/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11430 2023-08-01 11:26:31.000000 mypy-boto3-polly-1.28.16/mypy_boto3_polly/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11411 2023-08-01 11:26:31.000000 mypy-boto3-polly-1.28.16/mypy_boto3_polly/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10709 2023-08-01 11:26:31.000000 mypy-boto3-polly-1.28.16/mypy_boto3_polly/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10707 2023-08-01 11:26:31.000000 mypy-boto3-polly-1.28.16/mypy_boto3_polly/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-08-01 11:26:31.000000 mypy-boto3-polly-1.28.16/mypy_boto3_polly/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-08-01 11:26:31.000000 mypy-boto3-polly-1.28.16/mypy_boto3_polly/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:26:31.000000 mypy-boto3-polly-1.28.16/mypy_boto3_polly/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     8898 2023-08-01 11:26:31.000000 mypy-boto3-polly-1.28.16/mypy_boto3_polly/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8893 2023-08-01 11:26:31.000000 mypy-boto3-polly-1.28.16/mypy_boto3_polly/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:26:31.000000 mypy-boto3-polly-1.28.16/mypy_boto3_polly/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:34.324786 mypy-boto3-polly-1.28.16/mypy_boto3_polly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13856 2023-08-01 11:37:34.000000 mypy-boto3-polly-1.28.16/mypy_boto3_polly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-08-01 11:37:34.000000 mypy-boto3-polly-1.28.16/mypy_boto3_polly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:34.000000 mypy-boto3-polly-1.28.16/mypy_boto3_polly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:34.000000 mypy-boto3-polly-1.28.16/mypy_boto3_polly.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:34.000000 mypy-boto3-polly-1.28.16/mypy_boto3_polly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-01 11:37:34.000000 mypy-boto3-polly-1.28.16/mypy_boto3_polly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:34.324786 mypy-boto3-polly-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-08-01 11:26:30.000000 mypy-boto3-polly-1.28.16/setup.py
```

### Comparing `mypy-boto3-polly-1.28.15.post1/LICENSE` & `mypy-boto3-polly-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-polly-1.28.15.post1/PKG-INFO` & `mypy-boto3-polly-1.28.16/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-polly
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.Polly 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.Polly 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_polly/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 polly type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 polly type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-polly.svg?color=blue)](https://pypi.org/project/mypy-boto3-polly)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_polly/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-polly)](https://pepy.tech/project/mypy-boto3-polly)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Polly 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly)
+[boto3.Polly 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly)
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
 [mypy-boto3-polly docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_polly/).
 
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
 
 
 def check_value(value: DescribeVoicesPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_polly.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_polly.type_defs import (
     DeleteLexiconInputRequestTypeDef,
     PaginatorConfigTypeDef,
     DescribeVoicesInputRequestTypeDef,
     ResponseMetadataTypeDef,
@@ -365,15 +365,15 @@
     GetSpeechSynthesisTaskOutputTypeDef,
     ListSpeechSynthesisTasksOutputTypeDef,
     StartSpeechSynthesisTaskOutputTypeDef,
     ListLexiconsOutputTypeDef,
 )
 
 
-def get_structure() -> DeleteLexiconInputRequestTypeDef:
+def get_value() -> DeleteLexiconInputRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-polly-1.28.15.post1/README.md` & `mypy-boto3-polly-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-polly.svg?color=blue)](https://pypi.org/project/mypy-boto3-polly)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_polly/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-polly)](https://pepy.tech/project/mypy-boto3-polly)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Polly 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly)
+[boto3.Polly 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly)
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
 [mypy-boto3-polly docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_polly/).
 
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
 
 
 def check_value(value: DescribeVoicesPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_polly.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_polly.type_defs import (
     DeleteLexiconInputRequestTypeDef,
     PaginatorConfigTypeDef,
     DescribeVoicesInputRequestTypeDef,
     ResponseMetadataTypeDef,
@@ -333,15 +333,15 @@
     GetSpeechSynthesisTaskOutputTypeDef,
     ListSpeechSynthesisTasksOutputTypeDef,
     StartSpeechSynthesisTaskOutputTypeDef,
     ListLexiconsOutputTypeDef,
 )
 
 
-def get_structure() -> DeleteLexiconInputRequestTypeDef:
+def get_value() -> DeleteLexiconInputRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-polly-1.28.15.post1/mypy_boto3_polly/__init__.py` & `mypy-boto3-polly-1.28.16/mypy_boto3_polly/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-polly-1.28.15.post1/mypy_boto3_polly/__init__.pyi` & `mypy-boto3-polly-1.28.16/mypy_boto3_polly/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-polly-1.28.15.post1/mypy_boto3_polly/client.py` & `mypy-boto3-polly-1.28.16/mypy_boto3_polly/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-polly-1.28.15.post1/mypy_boto3_polly/client.pyi` & `mypy-boto3-polly-1.28.16/mypy_boto3_polly/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-polly-1.28.15.post1/mypy_boto3_polly/literals.py` & `mypy-boto3-polly-1.28.16/mypy_boto3_polly/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-polly-1.28.15.post1/mypy_boto3_polly/literals.pyi` & `mypy-boto3-polly-1.28.16/mypy_boto3_polly/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-polly-1.28.15.post1/mypy_boto3_polly/paginator.py` & `mypy-boto3-polly-1.28.16/mypy_boto3_polly/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-polly-1.28.15.post1/mypy_boto3_polly/paginator.pyi` & `mypy-boto3-polly-1.28.16/mypy_boto3_polly/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-polly-1.28.15.post1/mypy_boto3_polly/type_defs.py` & `mypy-boto3-polly-1.28.16/mypy_boto3_polly/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_polly/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_polly.type_defs import DeleteLexiconInputRequestTypeDef
 
-    data: DeleteLexiconInputRequestTypeDef = {...}
+    data: DeleteLexiconInputRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence
 
 from botocore.response import StreamingBody
```

### Comparing `mypy-boto3-polly-1.28.15.post1/mypy_boto3_polly/type_defs.pyi` & `mypy-boto3-polly-1.28.16/mypy_boto3_polly/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_polly/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_polly.type_defs import DeleteLexiconInputRequestTypeDef
 
-    data: DeleteLexiconInputRequestTypeDef = {...}
+    data: DeleteLexiconInputRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence
 
 from botocore.response import StreamingBody
```

### Comparing `mypy-boto3-polly-1.28.15.post1/mypy_boto3_polly.egg-info/PKG-INFO` & `mypy-boto3-polly-1.28.16/mypy_boto3_polly.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-polly
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.Polly 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.Polly 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_polly/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 polly type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 polly type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-polly.svg?color=blue)](https://pypi.org/project/mypy-boto3-polly)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_polly/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-polly)](https://pepy.tech/project/mypy-boto3-polly)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Polly 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly)
+[boto3.Polly 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly)
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
 [mypy-boto3-polly docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_polly/).
 
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
 
 
 def check_value(value: DescribeVoicesPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_polly.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_polly.type_defs import (
     DeleteLexiconInputRequestTypeDef,
     PaginatorConfigTypeDef,
     DescribeVoicesInputRequestTypeDef,
     ResponseMetadataTypeDef,
@@ -365,15 +365,15 @@
     GetSpeechSynthesisTaskOutputTypeDef,
     ListSpeechSynthesisTasksOutputTypeDef,
     StartSpeechSynthesisTaskOutputTypeDef,
     ListLexiconsOutputTypeDef,
 )
 
 
-def get_structure() -> DeleteLexiconInputRequestTypeDef:
+def get_value() -> DeleteLexiconInputRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-polly-1.28.15.post1/mypy_boto3_polly.egg-info/SOURCES.txt` & `mypy-boto3-polly-1.28.16/mypy_boto3_polly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-polly-1.28.15.post1/setup.py` & `mypy-boto3-polly-1.28.16/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-polly",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_polly"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Polly 1.28.15 service generated with mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.Polly 1.28.16 service generated with mypy-boto3-builder 7.17.1"
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
-    keywords="boto3 polly type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 polly type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_polly": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_polly/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

