# Comparing `tmp/mypy-boto3-appintegrations-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-appintegrations-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-appintegrations-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:30 2023, max compression
+gzip compressed data, was "mypy-boto3-appintegrations-1.28.16.tar", last modified: Tue Aug  1 11:36:11 2023, max compression
```

## Comparing `mypy-boto3-appintegrations-1.28.15.post1.tar` & `mypy-boto3-appintegrations-1.28.16.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:30.953007 mypy-boto3-appintegrations-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:38:12.000000 mypy-boto3-appintegrations-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13688 2023-07-29 10:02:30.949007 mypy-boto3-appintegrations-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12156 2023-07-29 09:38:12.000000 mypy-boto3-appintegrations-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:30.941007 mypy-boto3-appintegrations-1.28.15.post1/mypy_boto3_appintegrations/
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-29 09:38:12.000000 mypy-boto3-appintegrations-1.28.15.post1/mypy_boto3_appintegrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-29 09:38:12.000000 mypy-boto3-appintegrations-1.28.15.post1/mypy_boto3_appintegrations/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-07-29 09:38:12.000000 mypy-boto3-appintegrations-1.28.15.post1/mypy_boto3_appintegrations/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12764 2023-07-29 09:38:12.000000 mypy-boto3-appintegrations-1.28.15.post1/mypy_boto3_appintegrations/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12743 2023-07-29 09:38:12.000000 mypy-boto3-appintegrations-1.28.15.post1/mypy_boto3_appintegrations/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7915 2023-07-29 09:38:12.000000 mypy-boto3-appintegrations-1.28.15.post1/mypy_boto3_appintegrations/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7913 2023-07-29 09:38:12.000000 mypy-boto3-appintegrations-1.28.15.post1/mypy_boto3_appintegrations/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:38:12.000000 mypy-boto3-appintegrations-1.28.15.post1/mypy_boto3_appintegrations/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    12956 2023-07-29 09:38:13.000000 mypy-boto3-appintegrations-1.28.15.post1/mypy_boto3_appintegrations/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    12937 2023-07-29 09:38:13.000000 mypy-boto3-appintegrations-1.28.15.post1/mypy_boto3_appintegrations/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:38:12.000000 mypy-boto3-appintegrations-1.28.15.post1/mypy_boto3_appintegrations/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:30.949007 mypy-boto3-appintegrations-1.28.15.post1/mypy_boto3_appintegrations.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13688 2023-07-29 10:02:30.000000 mypy-boto3-appintegrations-1.28.15.post1/mypy_boto3_appintegrations.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-29 10:02:30.000000 mypy-boto3-appintegrations-1.28.15.post1/mypy_boto3_appintegrations.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:30.000000 mypy-boto3-appintegrations-1.28.15.post1/mypy_boto3_appintegrations.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:30.000000 mypy-boto3-appintegrations-1.28.15.post1/mypy_boto3_appintegrations.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:30.000000 mypy-boto3-appintegrations-1.28.15.post1/mypy_boto3_appintegrations.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-29 10:02:30.000000 mypy-boto3-appintegrations-1.28.15.post1/mypy_boto3_appintegrations.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:30.953007 mypy-boto3-appintegrations-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-07-29 09:38:12.000000 mypy-boto3-appintegrations-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:11.788950 mypy-boto3-appintegrations-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:10:43.000000 mypy-boto3-appintegrations-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13713 2023-08-01 11:36:11.784950 mypy-boto3-appintegrations-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12190 2023-08-01 11:10:43.000000 mypy-boto3-appintegrations-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:11.772951 mypy-boto3-appintegrations-1.28.16/mypy_boto3_appintegrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-08-01 11:10:43.000000 mypy-boto3-appintegrations-1.28.16/mypy_boto3_appintegrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-08-01 11:10:43.000000 mypy-boto3-appintegrations-1.28.16/mypy_boto3_appintegrations/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-08-01 11:10:43.000000 mypy-boto3-appintegrations-1.28.16/mypy_boto3_appintegrations/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12692 2023-08-01 11:10:43.000000 mypy-boto3-appintegrations-1.28.16/mypy_boto3_appintegrations/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12671 2023-08-01 11:10:43.000000 mypy-boto3-appintegrations-1.28.16/mypy_boto3_appintegrations/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7915 2023-08-01 11:10:44.000000 mypy-boto3-appintegrations-1.28.16/mypy_boto3_appintegrations/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7913 2023-08-01 11:10:43.000000 mypy-boto3-appintegrations-1.28.16/mypy_boto3_appintegrations/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:10:43.000000 mypy-boto3-appintegrations-1.28.16/mypy_boto3_appintegrations/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    13094 2023-08-01 11:10:44.000000 mypy-boto3-appintegrations-1.28.16/mypy_boto3_appintegrations/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13075 2023-08-01 11:10:44.000000 mypy-boto3-appintegrations-1.28.16/mypy_boto3_appintegrations/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:10:43.000000 mypy-boto3-appintegrations-1.28.16/mypy_boto3_appintegrations/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:11.784950 mypy-boto3-appintegrations-1.28.16/mypy_boto3_appintegrations.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13713 2023-08-01 11:36:11.000000 mypy-boto3-appintegrations-1.28.16/mypy_boto3_appintegrations.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-08-01 11:36:11.000000 mypy-boto3-appintegrations-1.28.16/mypy_boto3_appintegrations.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:11.000000 mypy-boto3-appintegrations-1.28.16/mypy_boto3_appintegrations.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:11.000000 mypy-boto3-appintegrations-1.28.16/mypy_boto3_appintegrations.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:11.000000 mypy-boto3-appintegrations-1.28.16/mypy_boto3_appintegrations.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-01 11:36:11.000000 mypy-boto3-appintegrations-1.28.16/mypy_boto3_appintegrations.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:11.788950 mypy-boto3-appintegrations-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-08-01 11:10:43.000000 mypy-boto3-appintegrations-1.28.16/setup.py
```

### Comparing `mypy-boto3-appintegrations-1.28.15.post1/LICENSE` & `mypy-boto3-appintegrations-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appintegrations-1.28.15.post1/PKG-INFO` & `mypy-boto3-appintegrations-1.28.16/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-appintegrations
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.AppIntegrationsService 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.AppIntegrationsService 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appintegrations/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 appintegrations type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 appintegrations type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-appintegrations.svg?color=blue)](https://pypi.org/project/mypy-boto3-appintegrations)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appintegrations/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-appintegrations)](https://pepy.tech/project/mypy-boto3-appintegrations)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AppIntegrationsService 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations.html#AppIntegrationsService)
+[boto3.AppIntegrationsService 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations.html#AppIntegrationsService)
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
 [mypy-boto3-appintegrations docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appintegrations/).
 
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
@@ -288,20 +288,20 @@
 )
 
 
 def check_value(value: AppIntegrationsServiceServiceName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_appintegrations.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_appintegrations.type_defs import (
     FileConfigurationTypeDef,
     ScheduleConfigurationTypeDef,
     FileConfigurationOutputTypeDef,
     ResponseMetadataTypeDef,
@@ -319,29 +319,30 @@
     ListEventIntegrationsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDataIntegrationRequestRequestTypeDef,
     UpdateEventIntegrationRequestRequestTypeDef,
     CreateDataIntegrationRequestRequestTypeDef,
+    FileConfigurationUnionTypeDef,
     CreateDataIntegrationResponseTypeDef,
     CreateEventIntegrationResponseTypeDef,
     GetDataIntegrationResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     CreateEventIntegrationRequestRequestTypeDef,
     EventIntegrationTypeDef,
     GetEventIntegrationResponseTypeDef,
     ListDataIntegrationAssociationsResponseTypeDef,
     ListDataIntegrationsResponseTypeDef,
     ListEventIntegrationAssociationsResponseTypeDef,
     ListEventIntegrationsResponseTypeDef,
 )
 
 
-def get_structure() -> FileConfigurationTypeDef:
+def get_value() -> FileConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-appintegrations-1.28.15.post1/README.md` & `mypy-boto3-appintegrations-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-appintegrations.svg?color=blue)](https://pypi.org/project/mypy-boto3-appintegrations)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appintegrations/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-appintegrations)](https://pepy.tech/project/mypy-boto3-appintegrations)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AppIntegrationsService 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations.html#AppIntegrationsService)
+[boto3.AppIntegrationsService 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations.html#AppIntegrationsService)
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
 [mypy-boto3-appintegrations docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appintegrations/).
 
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
@@ -256,20 +256,20 @@
 )
 
 
 def check_value(value: AppIntegrationsServiceServiceName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_appintegrations.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_appintegrations.type_defs import (
     FileConfigurationTypeDef,
     ScheduleConfigurationTypeDef,
     FileConfigurationOutputTypeDef,
     ResponseMetadataTypeDef,
@@ -287,29 +287,30 @@
     ListEventIntegrationsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDataIntegrationRequestRequestTypeDef,
     UpdateEventIntegrationRequestRequestTypeDef,
     CreateDataIntegrationRequestRequestTypeDef,
+    FileConfigurationUnionTypeDef,
     CreateDataIntegrationResponseTypeDef,
     CreateEventIntegrationResponseTypeDef,
     GetDataIntegrationResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     CreateEventIntegrationRequestRequestTypeDef,
     EventIntegrationTypeDef,
     GetEventIntegrationResponseTypeDef,
     ListDataIntegrationAssociationsResponseTypeDef,
     ListDataIntegrationsResponseTypeDef,
     ListEventIntegrationAssociationsResponseTypeDef,
     ListEventIntegrationsResponseTypeDef,
 )
 
 
-def get_structure() -> FileConfigurationTypeDef:
+def get_value() -> FileConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-appintegrations-1.28.15.post1/mypy_boto3_appintegrations/__main__.py` & `mypy-boto3-appintegrations-1.28.16/mypy_boto3_appintegrations/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.AppIntegrationsService 1.28.15\nVersion:        "
-        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.AppIntegrationsService 1.28.16\nVersion:        "
+        " 1.28.16\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appintegrations//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations.html#AppIntegrationsService\nOther"
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

### Comparing `mypy-boto3-appintegrations-1.28.15.post1/mypy_boto3_appintegrations/client.py` & `mypy-boto3-appintegrations-1.28.16/mypy_boto3_appintegrations/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,24 +9,23 @@
     from boto3.session import Session
     from mypy_boto3_appintegrations.client import AppIntegrationsServiceClient
 
     session = Session()
     client: AppIntegrationsServiceClient = session.client("appintegrations")
     ```
 """
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .type_defs import (
     CreateDataIntegrationResponseTypeDef,
     CreateEventIntegrationResponseTypeDef,
     EventFilterTypeDef,
-    FileConfigurationOutputTypeDef,
-    FileConfigurationTypeDef,
+    FileConfigurationUnionTypeDef,
     GetDataIntegrationResponseTypeDef,
     GetEventIntegrationResponseTypeDef,
     ListDataIntegrationAssociationsResponseTypeDef,
     ListDataIntegrationsResponseTypeDef,
     ListEventIntegrationAssociationsResponseTypeDef,
     ListEventIntegrationsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
@@ -94,15 +93,15 @@
         Name: str,
         KmsKey: str,
         SourceURI: str,
         ScheduleConfig: ScheduleConfigurationTypeDef,
         Description: str = ...,
         Tags: Mapping[str, str] = ...,
         ClientToken: str = ...,
-        FileConfiguration: Union[FileConfigurationTypeDef, FileConfigurationOutputTypeDef] = ...,
+        FileConfiguration: FileConfigurationUnionTypeDef = ...,
         ObjectConfiguration: Mapping[str, Mapping[str, Sequence[str]]] = ...
     ) -> CreateDataIntegrationResponseTypeDef:
         """
         Creates and persists a DataIntegration resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations.html#AppIntegrationsService.Client.create_data_integration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appintegrations/client/#create_data_integration)
```

### Comparing `mypy-boto3-appintegrations-1.28.15.post1/mypy_boto3_appintegrations/client.pyi` & `mypy-boto3-appintegrations-1.28.16/mypy_boto3_appintegrations/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -9,24 +9,23 @@
     from boto3.session import Session
     from mypy_boto3_appintegrations.client import AppIntegrationsServiceClient
 
     session = Session()
     client: AppIntegrationsServiceClient = session.client("appintegrations")
     ```
 """
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .type_defs import (
     CreateDataIntegrationResponseTypeDef,
     CreateEventIntegrationResponseTypeDef,
     EventFilterTypeDef,
-    FileConfigurationOutputTypeDef,
-    FileConfigurationTypeDef,
+    FileConfigurationUnionTypeDef,
     GetDataIntegrationResponseTypeDef,
     GetEventIntegrationResponseTypeDef,
     ListDataIntegrationAssociationsResponseTypeDef,
     ListDataIntegrationsResponseTypeDef,
     ListEventIntegrationAssociationsResponseTypeDef,
     ListEventIntegrationsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
@@ -88,15 +87,15 @@
         Name: str,
         KmsKey: str,
         SourceURI: str,
         ScheduleConfig: ScheduleConfigurationTypeDef,
         Description: str = ...,
         Tags: Mapping[str, str] = ...,
         ClientToken: str = ...,
-        FileConfiguration: Union[FileConfigurationTypeDef, FileConfigurationOutputTypeDef] = ...,
+        FileConfiguration: FileConfigurationUnionTypeDef = ...,
         ObjectConfiguration: Mapping[str, Mapping[str, Sequence[str]]] = ...
     ) -> CreateDataIntegrationResponseTypeDef:
         """
         Creates and persists a DataIntegration resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations.html#AppIntegrationsService.Client.create_data_integration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appintegrations/client/#create_data_integration)
```

### Comparing `mypy-boto3-appintegrations-1.28.15.post1/mypy_boto3_appintegrations/literals.py` & `mypy-boto3-appintegrations-1.28.16/mypy_boto3_appintegrations/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appintegrations-1.28.15.post1/mypy_boto3_appintegrations/literals.pyi` & `mypy-boto3-appintegrations-1.28.16/mypy_boto3_appintegrations/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appintegrations-1.28.15.post1/mypy_boto3_appintegrations/type_defs.py` & `mypy-boto3-appintegrations-1.28.16/mypy_boto3_appintegrations/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -4,26 +4,25 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appintegrations/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_appintegrations.type_defs import FileConfigurationTypeDef
 
-    data: FileConfigurationTypeDef = {...}
+    data: FileConfigurationTypeDef = ...
     ```
 """
 import sys
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "FileConfigurationTypeDef",
     "ScheduleConfigurationTypeDef",
     "FileConfigurationOutputTypeDef",
     "ResponseMetadataTypeDef",
     "EventFilterTypeDef",
     "DataIntegrationAssociationSummaryTypeDef",
@@ -39,14 +38,15 @@
     "ListEventIntegrationsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDataIntegrationRequestRequestTypeDef",
     "UpdateEventIntegrationRequestRequestTypeDef",
     "CreateDataIntegrationRequestRequestTypeDef",
+    "FileConfigurationUnionTypeDef",
     "CreateDataIntegrationResponseTypeDef",
     "CreateEventIntegrationResponseTypeDef",
     "GetDataIntegrationResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "CreateEventIntegrationRequestRequestTypeDef",
     "EventIntegrationTypeDef",
     "GetEventIntegrationResponseTypeDef",
@@ -66,21 +66,19 @@
     "_OptionalFileConfigurationTypeDef",
     {
         "Filters": Mapping[str, Sequence[str]],
     },
     total=False,
 )
 
-
 class FileConfigurationTypeDef(
     _RequiredFileConfigurationTypeDef, _OptionalFileConfigurationTypeDef
 ):
     pass
 
-
 _RequiredScheduleConfigurationTypeDef = TypedDict(
     "_RequiredScheduleConfigurationTypeDef",
     {
         "ScheduleExpression": str,
     },
 )
 _OptionalScheduleConfigurationTypeDef = TypedDict(
@@ -88,42 +86,38 @@
     {
         "FirstExecutionFrom": str,
         "Object": str,
     },
     total=False,
 )
 
-
 class ScheduleConfigurationTypeDef(
     _RequiredScheduleConfigurationTypeDef, _OptionalScheduleConfigurationTypeDef
 ):
     pass
 
-
 _RequiredFileConfigurationOutputTypeDef = TypedDict(
     "_RequiredFileConfigurationOutputTypeDef",
     {
         "Folders": List[str],
     },
 )
 _OptionalFileConfigurationOutputTypeDef = TypedDict(
     "_OptionalFileConfigurationOutputTypeDef",
     {
         "Filters": Dict[str, List[str]],
     },
     total=False,
 )
 
-
 class FileConfigurationOutputTypeDef(
     _RequiredFileConfigurationOutputTypeDef, _OptionalFileConfigurationOutputTypeDef
 ):
     pass
 
-
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -210,22 +204,20 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListDataIntegrationAssociationsRequestRequestTypeDef(
     _RequiredListDataIntegrationAssociationsRequestRequestTypeDef,
     _OptionalListDataIntegrationAssociationsRequestRequestTypeDef,
 ):
     pass
 
-
 ListDataIntegrationsRequestRequestTypeDef = TypedDict(
     "ListDataIntegrationsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -242,22 +234,20 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListEventIntegrationAssociationsRequestRequestTypeDef(
     _RequiredListEventIntegrationAssociationsRequestRequestTypeDef,
     _OptionalListEventIntegrationAssociationsRequestRequestTypeDef,
 ):
     pass
 
-
 ListEventIntegrationsRequestRequestTypeDef = TypedDict(
     "ListEventIntegrationsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -297,44 +287,40 @@
     {
         "Name": str,
         "Description": str,
     },
     total=False,
 )
 
-
 class UpdateDataIntegrationRequestRequestTypeDef(
     _RequiredUpdateDataIntegrationRequestRequestTypeDef,
     _OptionalUpdateDataIntegrationRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateEventIntegrationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateEventIntegrationRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalUpdateEventIntegrationRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateEventIntegrationRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
-
 class UpdateEventIntegrationRequestRequestTypeDef(
     _RequiredUpdateEventIntegrationRequestRequestTypeDef,
     _OptionalUpdateEventIntegrationRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateDataIntegrationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDataIntegrationRequestRequestTypeDef",
     {
         "Name": str,
         "KmsKey": str,
         "SourceURI": str,
         "ScheduleConfig": ScheduleConfigurationTypeDef,
@@ -348,22 +334,21 @@
         "ClientToken": str,
         "FileConfiguration": FileConfigurationTypeDef,
         "ObjectConfiguration": Mapping[str, Mapping[str, Sequence[str]]],
     },
     total=False,
 )
 
-
 class CreateDataIntegrationRequestRequestTypeDef(
     _RequiredCreateDataIntegrationRequestRequestTypeDef,
     _OptionalCreateDataIntegrationRequestRequestTypeDef,
 ):
     pass
 
-
+FileConfigurationUnionTypeDef = Union[FileConfigurationTypeDef, FileConfigurationOutputTypeDef]
 CreateDataIntegrationResponseTypeDef = TypedDict(
     "CreateDataIntegrationResponseTypeDef",
     {
         "Arn": str,
         "Id": str,
         "Name": str,
         "Description": str,
@@ -425,22 +410,20 @@
         "Description": str,
         "ClientToken": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateEventIntegrationRequestRequestTypeDef(
     _RequiredCreateEventIntegrationRequestRequestTypeDef,
     _OptionalCreateEventIntegrationRequestRequestTypeDef,
 ):
     pass
 
-
 EventIntegrationTypeDef = TypedDict(
     "EventIntegrationTypeDef",
     {
         "EventIntegrationArn": str,
         "Name": str,
         "Description": str,
         "EventFilter": EventFilterTypeDef,
```

### Comparing `mypy-boto3-appintegrations-1.28.15.post1/mypy_boto3_appintegrations/type_defs.pyi` & `mypy-boto3-appintegrations-1.28.16/mypy_boto3_appintegrations/type_defs.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,25 +4,26 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appintegrations/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_appintegrations.type_defs import FileConfigurationTypeDef
 
-    data: FileConfigurationTypeDef = {...}
+    data: FileConfigurationTypeDef = ...
     ```
 """
 import sys
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "FileConfigurationTypeDef",
     "ScheduleConfigurationTypeDef",
     "FileConfigurationOutputTypeDef",
     "ResponseMetadataTypeDef",
     "EventFilterTypeDef",
     "DataIntegrationAssociationSummaryTypeDef",
@@ -38,14 +39,15 @@
     "ListEventIntegrationsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDataIntegrationRequestRequestTypeDef",
     "UpdateEventIntegrationRequestRequestTypeDef",
     "CreateDataIntegrationRequestRequestTypeDef",
+    "FileConfigurationUnionTypeDef",
     "CreateDataIntegrationResponseTypeDef",
     "CreateEventIntegrationResponseTypeDef",
     "GetDataIntegrationResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "CreateEventIntegrationRequestRequestTypeDef",
     "EventIntegrationTypeDef",
     "GetEventIntegrationResponseTypeDef",
@@ -65,19 +67,21 @@
     "_OptionalFileConfigurationTypeDef",
     {
         "Filters": Mapping[str, Sequence[str]],
     },
     total=False,
 )
 
+
 class FileConfigurationTypeDef(
     _RequiredFileConfigurationTypeDef, _OptionalFileConfigurationTypeDef
 ):
     pass
 
+
 _RequiredScheduleConfigurationTypeDef = TypedDict(
     "_RequiredScheduleConfigurationTypeDef",
     {
         "ScheduleExpression": str,
     },
 )
 _OptionalScheduleConfigurationTypeDef = TypedDict(
@@ -85,38 +89,42 @@
     {
         "FirstExecutionFrom": str,
         "Object": str,
     },
     total=False,
 )
 
+
 class ScheduleConfigurationTypeDef(
     _RequiredScheduleConfigurationTypeDef, _OptionalScheduleConfigurationTypeDef
 ):
     pass
 
+
 _RequiredFileConfigurationOutputTypeDef = TypedDict(
     "_RequiredFileConfigurationOutputTypeDef",
     {
         "Folders": List[str],
     },
 )
 _OptionalFileConfigurationOutputTypeDef = TypedDict(
     "_OptionalFileConfigurationOutputTypeDef",
     {
         "Filters": Dict[str, List[str]],
     },
     total=False,
 )
 
+
 class FileConfigurationOutputTypeDef(
     _RequiredFileConfigurationOutputTypeDef, _OptionalFileConfigurationOutputTypeDef
 ):
     pass
 
+
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -203,20 +211,22 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListDataIntegrationAssociationsRequestRequestTypeDef(
     _RequiredListDataIntegrationAssociationsRequestRequestTypeDef,
     _OptionalListDataIntegrationAssociationsRequestRequestTypeDef,
 ):
     pass
 
+
 ListDataIntegrationsRequestRequestTypeDef = TypedDict(
     "ListDataIntegrationsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -233,20 +243,22 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListEventIntegrationAssociationsRequestRequestTypeDef(
     _RequiredListEventIntegrationAssociationsRequestRequestTypeDef,
     _OptionalListEventIntegrationAssociationsRequestRequestTypeDef,
 ):
     pass
 
+
 ListEventIntegrationsRequestRequestTypeDef = TypedDict(
     "ListEventIntegrationsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -286,40 +298,44 @@
     {
         "Name": str,
         "Description": str,
     },
     total=False,
 )
 
+
 class UpdateDataIntegrationRequestRequestTypeDef(
     _RequiredUpdateDataIntegrationRequestRequestTypeDef,
     _OptionalUpdateDataIntegrationRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateEventIntegrationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateEventIntegrationRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalUpdateEventIntegrationRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateEventIntegrationRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
+
 class UpdateEventIntegrationRequestRequestTypeDef(
     _RequiredUpdateEventIntegrationRequestRequestTypeDef,
     _OptionalUpdateEventIntegrationRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateDataIntegrationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDataIntegrationRequestRequestTypeDef",
     {
         "Name": str,
         "KmsKey": str,
         "SourceURI": str,
         "ScheduleConfig": ScheduleConfigurationTypeDef,
@@ -333,20 +349,23 @@
         "ClientToken": str,
         "FileConfiguration": FileConfigurationTypeDef,
         "ObjectConfiguration": Mapping[str, Mapping[str, Sequence[str]]],
     },
     total=False,
 )
 
+
 class CreateDataIntegrationRequestRequestTypeDef(
     _RequiredCreateDataIntegrationRequestRequestTypeDef,
     _OptionalCreateDataIntegrationRequestRequestTypeDef,
 ):
     pass
 
+
+FileConfigurationUnionTypeDef = Union[FileConfigurationTypeDef, FileConfigurationOutputTypeDef]
 CreateDataIntegrationResponseTypeDef = TypedDict(
     "CreateDataIntegrationResponseTypeDef",
     {
         "Arn": str,
         "Id": str,
         "Name": str,
         "Description": str,
@@ -408,20 +427,22 @@
         "Description": str,
         "ClientToken": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateEventIntegrationRequestRequestTypeDef(
     _RequiredCreateEventIntegrationRequestRequestTypeDef,
     _OptionalCreateEventIntegrationRequestRequestTypeDef,
 ):
     pass
 
+
 EventIntegrationTypeDef = TypedDict(
     "EventIntegrationTypeDef",
     {
         "EventIntegrationArn": str,
         "Name": str,
         "Description": str,
         "EventFilter": EventFilterTypeDef,
```

### Comparing `mypy-boto3-appintegrations-1.28.15.post1/mypy_boto3_appintegrations.egg-info/PKG-INFO` & `mypy-boto3-appintegrations-1.28.16/mypy_boto3_appintegrations.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-appintegrations
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.AppIntegrationsService 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.AppIntegrationsService 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appintegrations/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 appintegrations type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 appintegrations type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-appintegrations.svg?color=blue)](https://pypi.org/project/mypy-boto3-appintegrations)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appintegrations/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-appintegrations)](https://pepy.tech/project/mypy-boto3-appintegrations)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AppIntegrationsService 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations.html#AppIntegrationsService)
+[boto3.AppIntegrationsService 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations.html#AppIntegrationsService)
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
 [mypy-boto3-appintegrations docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appintegrations/).
 
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
@@ -288,20 +288,20 @@
 )
 
 
 def check_value(value: AppIntegrationsServiceServiceName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_appintegrations.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_appintegrations.type_defs import (
     FileConfigurationTypeDef,
     ScheduleConfigurationTypeDef,
     FileConfigurationOutputTypeDef,
     ResponseMetadataTypeDef,
@@ -319,29 +319,30 @@
     ListEventIntegrationsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDataIntegrationRequestRequestTypeDef,
     UpdateEventIntegrationRequestRequestTypeDef,
     CreateDataIntegrationRequestRequestTypeDef,
+    FileConfigurationUnionTypeDef,
     CreateDataIntegrationResponseTypeDef,
     CreateEventIntegrationResponseTypeDef,
     GetDataIntegrationResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     CreateEventIntegrationRequestRequestTypeDef,
     EventIntegrationTypeDef,
     GetEventIntegrationResponseTypeDef,
     ListDataIntegrationAssociationsResponseTypeDef,
     ListDataIntegrationsResponseTypeDef,
     ListEventIntegrationAssociationsResponseTypeDef,
     ListEventIntegrationsResponseTypeDef,
 )
 
 
-def get_structure() -> FileConfigurationTypeDef:
+def get_value() -> FileConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-appintegrations-1.28.15.post1/mypy_boto3_appintegrations.egg-info/SOURCES.txt` & `mypy-boto3-appintegrations-1.28.16/mypy_boto3_appintegrations.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appintegrations-1.28.15.post1/setup.py` & `mypy-boto3-appintegrations-1.28.16/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-appintegrations",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_appintegrations"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.AppIntegrationsService 1.28.15 service generated with"
-        " mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.AppIntegrationsService 1.28.16 service generated with"
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
-    keywords="boto3 appintegrations type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 appintegrations type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_appintegrations": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appintegrations/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

