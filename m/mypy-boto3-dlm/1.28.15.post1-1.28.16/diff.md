# Comparing `tmp/mypy-boto3-dlm-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-dlm-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-dlm-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:58 2023, max compression
+gzip compressed data, was "mypy-boto3-dlm-1.28.16.tar", last modified: Tue Aug  1 11:36:38 2023, max compression
```

## Comparing `mypy-boto3-dlm-1.28.15.post1.tar` & `mypy-boto3-dlm-1.28.16.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:58.353111 mypy-boto3-dlm-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:42:29.000000 mypy-boto3-dlm-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13315 2023-07-29 10:02:58.349111 mypy-boto3-dlm-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11838 2023-07-29 09:42:29.000000 mypy-boto3-dlm-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:58.337111 mypy-boto3-dlm-1.28.15.post1/mypy_boto3_dlm/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-29 09:42:29.000000 mypy-boto3-dlm-1.28.15.post1/mypy_boto3_dlm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-29 09:42:29.000000 mypy-boto3-dlm-1.28.15.post1/mypy_boto3_dlm/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-29 09:42:29.000000 mypy-boto3-dlm-1.28.15.post1/mypy_boto3_dlm/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7825 2023-07-29 09:42:29.000000 mypy-boto3-dlm-1.28.15.post1/mypy_boto3_dlm/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7811 2023-07-29 09:42:29.000000 mypy-boto3-dlm-1.28.15.post1/mypy_boto3_dlm/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9051 2023-07-29 09:42:29.000000 mypy-boto3-dlm-1.28.15.post1/mypy_boto3_dlm/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9049 2023-07-29 09:42:29.000000 mypy-boto3-dlm-1.28.15.post1/mypy_boto3_dlm/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:42:29.000000 mypy-boto3-dlm-1.28.15.post1/mypy_boto3_dlm/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    16011 2023-07-29 09:42:30.000000 mypy-boto3-dlm-1.28.15.post1/mypy_boto3_dlm/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    15988 2023-07-29 09:42:30.000000 mypy-boto3-dlm-1.28.15.post1/mypy_boto3_dlm/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:42:29.000000 mypy-boto3-dlm-1.28.15.post1/mypy_boto3_dlm/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:58.349111 mypy-boto3-dlm-1.28.15.post1/mypy_boto3_dlm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13315 2023-07-29 10:02:58.000000 mypy-boto3-dlm-1.28.15.post1/mypy_boto3_dlm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-29 10:02:58.000000 mypy-boto3-dlm-1.28.15.post1/mypy_boto3_dlm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:58.000000 mypy-boto3-dlm-1.28.15.post1/mypy_boto3_dlm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:58.000000 mypy-boto3-dlm-1.28.15.post1/mypy_boto3_dlm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:58.000000 mypy-boto3-dlm-1.28.15.post1/mypy_boto3_dlm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-29 10:02:58.000000 mypy-boto3-dlm-1.28.15.post1/mypy_boto3_dlm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:58.353111 mypy-boto3-dlm-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-29 09:42:29.000000 mypy-boto3-dlm-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:38.608908 mypy-boto3-dlm-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:15:01.000000 mypy-boto3-dlm-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13336 2023-08-01 11:36:38.608908 mypy-boto3-dlm-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11868 2023-08-01 11:15:01.000000 mypy-boto3-dlm-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:38.608908 mypy-boto3-dlm-1.28.16/mypy_boto3_dlm/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-08-01 11:15:01.000000 mypy-boto3-dlm-1.28.16/mypy_boto3_dlm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-08-01 11:15:01.000000 mypy-boto3-dlm-1.28.16/mypy_boto3_dlm/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-08-01 11:15:01.000000 mypy-boto3-dlm-1.28.16/mypy_boto3_dlm/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7731 2023-08-01 11:15:01.000000 mypy-boto3-dlm-1.28.16/mypy_boto3_dlm/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7717 2023-08-01 11:15:01.000000 mypy-boto3-dlm-1.28.16/mypy_boto3_dlm/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9051 2023-08-01 11:15:03.000000 mypy-boto3-dlm-1.28.16/mypy_boto3_dlm/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9049 2023-08-01 11:15:01.000000 mypy-boto3-dlm-1.28.16/mypy_boto3_dlm/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:15:01.000000 mypy-boto3-dlm-1.28.16/mypy_boto3_dlm/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    16133 2023-08-01 11:15:03.000000 mypy-boto3-dlm-1.28.16/mypy_boto3_dlm/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16110 2023-08-01 11:15:03.000000 mypy-boto3-dlm-1.28.16/mypy_boto3_dlm/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:15:01.000000 mypy-boto3-dlm-1.28.16/mypy_boto3_dlm/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:38.608908 mypy-boto3-dlm-1.28.16/mypy_boto3_dlm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13336 2023-08-01 11:36:38.000000 mypy-boto3-dlm-1.28.16/mypy_boto3_dlm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-08-01 11:36:38.000000 mypy-boto3-dlm-1.28.16/mypy_boto3_dlm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:38.000000 mypy-boto3-dlm-1.28.16/mypy_boto3_dlm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:38.000000 mypy-boto3-dlm-1.28.16/mypy_boto3_dlm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:38.000000 mypy-boto3-dlm-1.28.16/mypy_boto3_dlm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-01 11:36:38.000000 mypy-boto3-dlm-1.28.16/mypy_boto3_dlm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:38.608908 mypy-boto3-dlm-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-08-01 11:15:01.000000 mypy-boto3-dlm-1.28.16/setup.py
```

### Comparing `mypy-boto3-dlm-1.28.15.post1/LICENSE` & `mypy-boto3-dlm-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dlm-1.28.15.post1/PKG-INFO` & `mypy-boto3-dlm-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-dlm
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.DLM 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.DLM 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dlm/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 dlm type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 dlm type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-dlm.svg?color=blue)](https://pypi.org/project/mypy-boto3-dlm)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dlm/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-dlm)](https://pepy.tech/project/mypy-boto3-dlm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DLM 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dlm.html#DLM)
+[boto3.DLM 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dlm.html#DLM)
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
 [mypy-boto3-dlm docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dlm/).
 
 See how it helps to find and fix potential bugs:
 
@@ -73,15 +73,15 @@
     - [Sublime Text](#sublime-text)
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
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
@@ -296,20 +296,20 @@
 )
 
 
 def check_value(value: EventSourceValuesType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_dlm.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_dlm.type_defs import (
     RetentionArchiveTierTypeDef,
     ResponseMetadataTypeDef,
     CreateRuleOutputTypeDef,
     CreateRuleTypeDef,
@@ -347,20 +347,21 @@
     ActionTypeDef,
     ScheduleOutputTypeDef,
     ScheduleTypeDef,
     PolicyDetailsOutputTypeDef,
     PolicyDetailsTypeDef,
     LifecyclePolicyTypeDef,
     CreateLifecyclePolicyRequestRequestTypeDef,
+    PolicyDetailsUnionTypeDef,
     UpdateLifecyclePolicyRequestRequestTypeDef,
     GetLifecyclePolicyResponseTypeDef,
 )
 
 
-def get_structure() -> RetentionArchiveTierTypeDef:
+def get_value() -> RetentionArchiveTierTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-dlm-1.28.15.post1/README.md` & `mypy-boto3-dlm-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-dlm.svg?color=blue)](https://pypi.org/project/mypy-boto3-dlm)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dlm/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-dlm)](https://pepy.tech/project/mypy-boto3-dlm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DLM 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dlm.html#DLM)
+[boto3.DLM 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dlm.html#DLM)
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
 [mypy-boto3-dlm docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dlm/).
 
 See how it helps to find and fix potential bugs:
 
@@ -41,15 +41,15 @@
     - [Sublime Text](#sublime-text)
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
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
@@ -264,20 +264,20 @@
 )
 
 
 def check_value(value: EventSourceValuesType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_dlm.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_dlm.type_defs import (
     RetentionArchiveTierTypeDef,
     ResponseMetadataTypeDef,
     CreateRuleOutputTypeDef,
     CreateRuleTypeDef,
@@ -315,20 +315,21 @@
     ActionTypeDef,
     ScheduleOutputTypeDef,
     ScheduleTypeDef,
     PolicyDetailsOutputTypeDef,
     PolicyDetailsTypeDef,
     LifecyclePolicyTypeDef,
     CreateLifecyclePolicyRequestRequestTypeDef,
+    PolicyDetailsUnionTypeDef,
     UpdateLifecyclePolicyRequestRequestTypeDef,
     GetLifecyclePolicyResponseTypeDef,
 )
 
 
-def get_structure() -> RetentionArchiveTierTypeDef:
+def get_value() -> RetentionArchiveTierTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-dlm-1.28.15.post1/mypy_boto3_dlm/__main__.py` & `mypy-boto3-dlm-1.28.16/mypy_boto3_dlm/__main__.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.DLM 1.28.15\nVersion:         1.28.15.post1\nBuilder version:"
-        " 7.16.2\nDocs:           "
+        "Type annotations for boto3.DLM 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dlm//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dlm.html#DLM\nOther"
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

### Comparing `mypy-boto3-dlm-1.28.15.post1/mypy_boto3_dlm/client.py` & `mypy-boto3-dlm-1.28.16/mypy_boto3_dlm/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,30 +9,29 @@
     from boto3.session import Session
     from mypy_boto3_dlm.client import DLMClient
 
     session = Session()
     client: DLMClient = session.client("dlm")
     ```
 """
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     GettablePolicyStateValuesType,
     ResourceTypeValuesType,
     SettablePolicyStateValuesType,
 )
 from .type_defs import (
     CreateLifecyclePolicyResponseTypeDef,
     GetLifecyclePoliciesResponseTypeDef,
     GetLifecyclePolicyResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    PolicyDetailsOutputTypeDef,
-    PolicyDetailsTypeDef,
+    PolicyDetailsUnionTypeDef,
 )
 
 __all__ = ("DLMClient",)
 
 
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
@@ -85,15 +84,15 @@
 
     def create_lifecycle_policy(
         self,
         *,
         ExecutionRoleArn: str,
         Description: str,
         State: SettablePolicyStateValuesType,
-        PolicyDetails: Union[PolicyDetailsTypeDef, PolicyDetailsOutputTypeDef],
+        PolicyDetails: PolicyDetailsUnionTypeDef,
         Tags: Mapping[str, str] = ...
     ) -> CreateLifecyclePolicyResponseTypeDef:
         """
         Creates a policy to manage the lifecycle of the specified Amazon Web Services
         resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dlm.html#DLM.Client.create_lifecycle_policy)
@@ -174,15 +173,15 @@
     def update_lifecycle_policy(
         self,
         *,
         PolicyId: str,
         ExecutionRoleArn: str = ...,
         State: SettablePolicyStateValuesType = ...,
         Description: str = ...,
-        PolicyDetails: Union[PolicyDetailsTypeDef, PolicyDetailsOutputTypeDef] = ...
+        PolicyDetails: PolicyDetailsUnionTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Updates the specified lifecycle policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dlm.html#DLM.Client.update_lifecycle_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dlm/client/#update_lifecycle_policy)
         """
```

### Comparing `mypy-boto3-dlm-1.28.15.post1/mypy_boto3_dlm/client.pyi` & `mypy-boto3-dlm-1.28.16/mypy_boto3_dlm/client.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -9,30 +9,29 @@
     from boto3.session import Session
     from mypy_boto3_dlm.client import DLMClient
 
     session = Session()
     client: DLMClient = session.client("dlm")
     ```
 """
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     GettablePolicyStateValuesType,
     ResourceTypeValuesType,
     SettablePolicyStateValuesType,
 )
 from .type_defs import (
     CreateLifecyclePolicyResponseTypeDef,
     GetLifecyclePoliciesResponseTypeDef,
     GetLifecyclePolicyResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    PolicyDetailsOutputTypeDef,
-    PolicyDetailsTypeDef,
+    PolicyDetailsUnionTypeDef,
 )
 
 __all__ = ("DLMClient",)
 
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
@@ -79,15 +78,15 @@
         """
     def create_lifecycle_policy(
         self,
         *,
         ExecutionRoleArn: str,
         Description: str,
         State: SettablePolicyStateValuesType,
-        PolicyDetails: Union[PolicyDetailsTypeDef, PolicyDetailsOutputTypeDef],
+        PolicyDetails: PolicyDetailsUnionTypeDef,
         Tags: Mapping[str, str] = ...
     ) -> CreateLifecyclePolicyResponseTypeDef:
         """
         Creates a policy to manage the lifecycle of the specified Amazon Web Services
         resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dlm.html#DLM.Client.create_lifecycle_policy)
@@ -160,15 +159,15 @@
     def update_lifecycle_policy(
         self,
         *,
         PolicyId: str,
         ExecutionRoleArn: str = ...,
         State: SettablePolicyStateValuesType = ...,
         Description: str = ...,
-        PolicyDetails: Union[PolicyDetailsTypeDef, PolicyDetailsOutputTypeDef] = ...
+        PolicyDetails: PolicyDetailsUnionTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Updates the specified lifecycle policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dlm.html#DLM.Client.update_lifecycle_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dlm/client/#update_lifecycle_policy)
         """
```

### Comparing `mypy-boto3-dlm-1.28.15.post1/mypy_boto3_dlm/literals.py` & `mypy-boto3-dlm-1.28.16/mypy_boto3_dlm/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dlm-1.28.15.post1/mypy_boto3_dlm/literals.pyi` & `mypy-boto3-dlm-1.28.16/mypy_boto3_dlm/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dlm-1.28.15.post1/mypy_boto3_dlm/type_defs.py` & `mypy-boto3-dlm-1.28.16/mypy_boto3_dlm/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dlm/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_dlm.type_defs import RetentionArchiveTierTypeDef
 
-    data: RetentionArchiveTierTypeDef = {...}
+    data: RetentionArchiveTierTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     GettablePolicyStateValuesType,
     LocationValuesType,
     PolicyTypeValuesType,
     ResourceLocationValuesType,
     ResourceTypeValuesType,
@@ -74,14 +74,15 @@
     "ActionTypeDef",
     "ScheduleOutputTypeDef",
     "ScheduleTypeDef",
     "PolicyDetailsOutputTypeDef",
     "PolicyDetailsTypeDef",
     "LifecyclePolicyTypeDef",
     "CreateLifecyclePolicyRequestRequestTypeDef",
+    "PolicyDetailsUnionTypeDef",
     "UpdateLifecyclePolicyRequestRequestTypeDef",
     "GetLifecyclePolicyResponseTypeDef",
 )
 
 RetentionArchiveTierTypeDef = TypedDict(
     "RetentionArchiveTierTypeDef",
     {
@@ -623,14 +624,15 @@
 class CreateLifecyclePolicyRequestRequestTypeDef(
     _RequiredCreateLifecyclePolicyRequestRequestTypeDef,
     _OptionalCreateLifecyclePolicyRequestRequestTypeDef,
 ):
     pass
 
 
+PolicyDetailsUnionTypeDef = Union[PolicyDetailsTypeDef, PolicyDetailsOutputTypeDef]
 _RequiredUpdateLifecyclePolicyRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateLifecyclePolicyRequestRequestTypeDef",
     {
         "PolicyId": str,
     },
 )
 _OptionalUpdateLifecyclePolicyRequestRequestTypeDef = TypedDict(
```

### Comparing `mypy-boto3-dlm-1.28.15.post1/mypy_boto3_dlm/type_defs.pyi` & `mypy-boto3-dlm-1.28.16/mypy_boto3_dlm/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dlm/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_dlm.type_defs import RetentionArchiveTierTypeDef
 
-    data: RetentionArchiveTierTypeDef = {...}
+    data: RetentionArchiveTierTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     GettablePolicyStateValuesType,
     LocationValuesType,
     PolicyTypeValuesType,
     ResourceLocationValuesType,
     ResourceTypeValuesType,
@@ -73,14 +73,15 @@
     "ActionTypeDef",
     "ScheduleOutputTypeDef",
     "ScheduleTypeDef",
     "PolicyDetailsOutputTypeDef",
     "PolicyDetailsTypeDef",
     "LifecyclePolicyTypeDef",
     "CreateLifecyclePolicyRequestRequestTypeDef",
+    "PolicyDetailsUnionTypeDef",
     "UpdateLifecyclePolicyRequestRequestTypeDef",
     "GetLifecyclePolicyResponseTypeDef",
 )
 
 RetentionArchiveTierTypeDef = TypedDict(
     "RetentionArchiveTierTypeDef",
     {
@@ -602,14 +603,15 @@
 
 class CreateLifecyclePolicyRequestRequestTypeDef(
     _RequiredCreateLifecyclePolicyRequestRequestTypeDef,
     _OptionalCreateLifecyclePolicyRequestRequestTypeDef,
 ):
     pass
 
+PolicyDetailsUnionTypeDef = Union[PolicyDetailsTypeDef, PolicyDetailsOutputTypeDef]
 _RequiredUpdateLifecyclePolicyRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateLifecyclePolicyRequestRequestTypeDef",
     {
         "PolicyId": str,
     },
 )
 _OptionalUpdateLifecyclePolicyRequestRequestTypeDef = TypedDict(
```

### Comparing `mypy-boto3-dlm-1.28.15.post1/mypy_boto3_dlm.egg-info/PKG-INFO` & `mypy-boto3-dlm-1.28.16/mypy_boto3_dlm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-dlm
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.DLM 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.DLM 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dlm/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 dlm type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 dlm type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-dlm.svg?color=blue)](https://pypi.org/project/mypy-boto3-dlm)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dlm/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-dlm)](https://pepy.tech/project/mypy-boto3-dlm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DLM 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dlm.html#DLM)
+[boto3.DLM 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dlm.html#DLM)
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
 [mypy-boto3-dlm docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dlm/).
 
 See how it helps to find and fix potential bugs:
 
@@ -73,15 +73,15 @@
     - [Sublime Text](#sublime-text)
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
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
@@ -296,20 +296,20 @@
 )
 
 
 def check_value(value: EventSourceValuesType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_dlm.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_dlm.type_defs import (
     RetentionArchiveTierTypeDef,
     ResponseMetadataTypeDef,
     CreateRuleOutputTypeDef,
     CreateRuleTypeDef,
@@ -347,20 +347,21 @@
     ActionTypeDef,
     ScheduleOutputTypeDef,
     ScheduleTypeDef,
     PolicyDetailsOutputTypeDef,
     PolicyDetailsTypeDef,
     LifecyclePolicyTypeDef,
     CreateLifecyclePolicyRequestRequestTypeDef,
+    PolicyDetailsUnionTypeDef,
     UpdateLifecyclePolicyRequestRequestTypeDef,
     GetLifecyclePolicyResponseTypeDef,
 )
 
 
-def get_structure() -> RetentionArchiveTierTypeDef:
+def get_value() -> RetentionArchiveTierTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-dlm-1.28.15.post1/mypy_boto3_dlm.egg-info/SOURCES.txt` & `mypy-boto3-dlm-1.28.16/mypy_boto3_dlm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dlm-1.28.15.post1/setup.py` & `mypy-boto3-dlm-1.28.16/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-dlm",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_dlm"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.DLM 1.28.15 service generated with mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.DLM 1.28.16 service generated with mypy-boto3-builder 7.17.1"
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
-    keywords="boto3 dlm type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 dlm type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_dlm": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dlm/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

