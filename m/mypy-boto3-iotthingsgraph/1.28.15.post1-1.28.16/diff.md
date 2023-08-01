# Comparing `tmp/mypy-boto3-iotthingsgraph-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-iotthingsgraph-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-iotthingsgraph-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:23 2023, max compression
+gzip compressed data, was "mypy-boto3-iotthingsgraph-1.28.16.tar", last modified: Tue Aug  1 11:37:03 2023, max compression
```

## Comparing `mypy-boto3-iotthingsgraph-1.28.15.post1.tar` & `mypy-boto3-iotthingsgraph-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:23.329197 mypy-boto3-iotthingsgraph-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:48:11.000000 mypy-boto3-iotthingsgraph-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18915 2023-07-29 10:03:23.329197 mypy-boto3-iotthingsgraph-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17394 2023-07-29 09:48:11.000000 mypy-boto3-iotthingsgraph-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:23.317196 mypy-boto3-iotthingsgraph-1.28.15.post1/mypy_boto3_iotthingsgraph/
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-07-29 09:48:11.000000 mypy-boto3-iotthingsgraph-1.28.15.post1/mypy_boto3_iotthingsgraph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-07-29 09:48:11.000000 mypy-boto3-iotthingsgraph-1.28.15.post1/mypy_boto3_iotthingsgraph/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-29 09:48:11.000000 mypy-boto3-iotthingsgraph-1.28.15.post1/mypy_boto3_iotthingsgraph/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29250 2023-07-29 09:48:12.000000 mypy-boto3-iotthingsgraph-1.28.15.post1/mypy_boto3_iotthingsgraph/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    29198 2023-07-29 09:48:11.000000 mypy-boto3-iotthingsgraph-1.28.15.post1/mypy_boto3_iotthingsgraph/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11270 2023-07-29 09:48:12.000000 mypy-boto3-iotthingsgraph-1.28.15.post1/mypy_boto3_iotthingsgraph/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11268 2023-07-29 09:48:12.000000 mypy-boto3-iotthingsgraph-1.28.15.post1/mypy_boto3_iotthingsgraph/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13076 2023-07-29 09:48:12.000000 mypy-boto3-iotthingsgraph-1.28.15.post1/mypy_boto3_iotthingsgraph/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13064 2023-07-29 09:48:12.000000 mypy-boto3-iotthingsgraph-1.28.15.post1/mypy_boto3_iotthingsgraph/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:48:11.000000 mypy-boto3-iotthingsgraph-1.28.15.post1/mypy_boto3_iotthingsgraph/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    33685 2023-07-29 09:48:15.000000 mypy-boto3-iotthingsgraph-1.28.15.post1/mypy_boto3_iotthingsgraph/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    33638 2023-07-29 09:48:12.000000 mypy-boto3-iotthingsgraph-1.28.15.post1/mypy_boto3_iotthingsgraph/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:48:11.000000 mypy-boto3-iotthingsgraph-1.28.15.post1/mypy_boto3_iotthingsgraph/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:23.329197 mypy-boto3-iotthingsgraph-1.28.15.post1/mypy_boto3_iotthingsgraph.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18915 2023-07-29 10:03:23.000000 mypy-boto3-iotthingsgraph-1.28.15.post1/mypy_boto3_iotthingsgraph.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-29 10:03:23.000000 mypy-boto3-iotthingsgraph-1.28.15.post1/mypy_boto3_iotthingsgraph.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:23.000000 mypy-boto3-iotthingsgraph-1.28.15.post1/mypy_boto3_iotthingsgraph.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:23.000000 mypy-boto3-iotthingsgraph-1.28.15.post1/mypy_boto3_iotthingsgraph.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:23.000000 mypy-boto3-iotthingsgraph-1.28.15.post1/mypy_boto3_iotthingsgraph.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-29 10:03:23.000000 mypy-boto3-iotthingsgraph-1.28.15.post1/mypy_boto3_iotthingsgraph.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:23.329197 mypy-boto3-iotthingsgraph-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-07-29 09:48:11.000000 mypy-boto3-iotthingsgraph-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:03.196859 mypy-boto3-iotthingsgraph-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:20:57.000000 mypy-boto3-iotthingsgraph-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18927 2023-08-01 11:37:03.192859 mypy-boto3-iotthingsgraph-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17415 2023-08-01 11:20:57.000000 mypy-boto3-iotthingsgraph-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:03.184859 mypy-boto3-iotthingsgraph-1.28.16/mypy_boto3_iotthingsgraph/
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-08-01 11:20:57.000000 mypy-boto3-iotthingsgraph-1.28.16/mypy_boto3_iotthingsgraph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-08-01 11:20:57.000000 mypy-boto3-iotthingsgraph-1.28.16/mypy_boto3_iotthingsgraph/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-08-01 11:20:57.000000 mypy-boto3-iotthingsgraph-1.28.16/mypy_boto3_iotthingsgraph/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29227 2023-08-01 11:20:58.000000 mypy-boto3-iotthingsgraph-1.28.16/mypy_boto3_iotthingsgraph/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29175 2023-08-01 11:20:57.000000 mypy-boto3-iotthingsgraph-1.28.16/mypy_boto3_iotthingsgraph/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11270 2023-08-01 11:20:58.000000 mypy-boto3-iotthingsgraph-1.28.16/mypy_boto3_iotthingsgraph/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11268 2023-08-01 11:20:58.000000 mypy-boto3-iotthingsgraph-1.28.16/mypy_boto3_iotthingsgraph/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13053 2023-08-01 11:20:58.000000 mypy-boto3-iotthingsgraph-1.28.16/mypy_boto3_iotthingsgraph/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13041 2023-08-01 11:20:58.000000 mypy-boto3-iotthingsgraph-1.28.16/mypy_boto3_iotthingsgraph/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:20:57.000000 mypy-boto3-iotthingsgraph-1.28.16/mypy_boto3_iotthingsgraph/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    33731 2023-08-01 11:20:59.000000 mypy-boto3-iotthingsgraph-1.28.16/mypy_boto3_iotthingsgraph/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33684 2023-08-01 11:20:58.000000 mypy-boto3-iotthingsgraph-1.28.16/mypy_boto3_iotthingsgraph/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:20:57.000000 mypy-boto3-iotthingsgraph-1.28.16/mypy_boto3_iotthingsgraph/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:03.192859 mypy-boto3-iotthingsgraph-1.28.16/mypy_boto3_iotthingsgraph.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18927 2023-08-01 11:37:02.000000 mypy-boto3-iotthingsgraph-1.28.16/mypy_boto3_iotthingsgraph.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-08-01 11:37:02.000000 mypy-boto3-iotthingsgraph-1.28.16/mypy_boto3_iotthingsgraph.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:02.000000 mypy-boto3-iotthingsgraph-1.28.16/mypy_boto3_iotthingsgraph.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:02.000000 mypy-boto3-iotthingsgraph-1.28.16/mypy_boto3_iotthingsgraph.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:02.000000 mypy-boto3-iotthingsgraph-1.28.16/mypy_boto3_iotthingsgraph.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-01 11:37:02.000000 mypy-boto3-iotthingsgraph-1.28.16/mypy_boto3_iotthingsgraph.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:03.196859 mypy-boto3-iotthingsgraph-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-08-01 11:20:57.000000 mypy-boto3-iotthingsgraph-1.28.16/setup.py
```

### Comparing `mypy-boto3-iotthingsgraph-1.28.15.post1/LICENSE` & `mypy-boto3-iotthingsgraph-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotthingsgraph-1.28.15.post1/PKG-INFO` & `mypy-boto3-iotthingsgraph-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iotthingsgraph
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.IoTThingsGraph 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.IoTThingsGraph 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 iotthingsgraph type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 iotthingsgraph type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotthingsgraph.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotthingsgraph)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iotthingsgraph)](https://pepy.tech/project/mypy-boto3-iotthingsgraph)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTThingsGraph 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph)
+[boto3.IoTThingsGraph 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph)
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
 [mypy-boto3-iotthingsgraph docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/).
 
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
@@ -369,20 +369,20 @@
 )
 
 
 def check_value(value: DefinitionLanguageType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_iotthingsgraph.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_iotthingsgraph.type_defs import (
     AssociateEntityToThingRequestRequestTypeDef,
     DefinitionDocumentTypeDef,
     FlowTemplateSummaryTypeDef,
     ResponseMetadataTypeDef,
@@ -409,15 +409,15 @@
     GetFlowTemplateRevisionsRequestRequestTypeDef,
     GetSystemInstanceRequestRequestTypeDef,
     GetSystemTemplateRequestRequestTypeDef,
     GetSystemTemplateRevisionsRequestRequestTypeDef,
     GetUploadStatusRequestRequestTypeDef,
     ListFlowExecutionMessagesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    SearchFlowExecutionsRequestRequestTypeDef,
+    TimestampTypeDef,
     SystemInstanceFilterTypeDef,
     SystemTemplateFilterTypeDef,
     SearchThingsRequestRequestTypeDef,
     ThingTypeDef,
     UndeploySystemInstanceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     CreateFlowTemplateRequestRequestTypeDef,
@@ -454,31 +454,32 @@
     SearchFlowExecutionsResponseTypeDef,
     SearchFlowTemplatesRequestRequestTypeDef,
     GetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef,
     GetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef,
     ListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef,
     ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     SearchEntitiesRequestSearchEntitiesPaginateTypeDef,
-    SearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef,
     SearchFlowTemplatesRequestSearchFlowTemplatesPaginateTypeDef,
     SearchThingsRequestSearchThingsPaginateTypeDef,
+    SearchFlowExecutionsRequestRequestTypeDef,
+    SearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef,
     SearchSystemInstancesRequestRequestTypeDef,
     SearchSystemInstancesRequestSearchSystemInstancesPaginateTypeDef,
     SearchSystemTemplatesRequestRequestTypeDef,
     SearchSystemTemplatesRequestSearchSystemTemplatesPaginateTypeDef,
     SearchThingsResponseTypeDef,
     GetEntitiesResponseTypeDef,
     SearchEntitiesResponseTypeDef,
     GetFlowTemplateResponseTypeDef,
     GetSystemTemplateResponseTypeDef,
     GetSystemInstanceResponseTypeDef,
 )
 
 
-def get_structure() -> AssociateEntityToThingRequestRequestTypeDef:
+def get_value() -> AssociateEntityToThingRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-iotthingsgraph-1.28.15.post1/README.md` & `mypy-boto3-iotthingsgraph-1.28.16/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotthingsgraph.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotthingsgraph)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iotthingsgraph)](https://pepy.tech/project/mypy-boto3-iotthingsgraph)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTThingsGraph 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph)
+[boto3.IoTThingsGraph 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph)
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
 [mypy-boto3-iotthingsgraph docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/).
 
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
@@ -337,20 +337,20 @@
 )
 
 
 def check_value(value: DefinitionLanguageType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_iotthingsgraph.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_iotthingsgraph.type_defs import (
     AssociateEntityToThingRequestRequestTypeDef,
     DefinitionDocumentTypeDef,
     FlowTemplateSummaryTypeDef,
     ResponseMetadataTypeDef,
@@ -377,15 +377,15 @@
     GetFlowTemplateRevisionsRequestRequestTypeDef,
     GetSystemInstanceRequestRequestTypeDef,
     GetSystemTemplateRequestRequestTypeDef,
     GetSystemTemplateRevisionsRequestRequestTypeDef,
     GetUploadStatusRequestRequestTypeDef,
     ListFlowExecutionMessagesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    SearchFlowExecutionsRequestRequestTypeDef,
+    TimestampTypeDef,
     SystemInstanceFilterTypeDef,
     SystemTemplateFilterTypeDef,
     SearchThingsRequestRequestTypeDef,
     ThingTypeDef,
     UndeploySystemInstanceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     CreateFlowTemplateRequestRequestTypeDef,
@@ -422,31 +422,32 @@
     SearchFlowExecutionsResponseTypeDef,
     SearchFlowTemplatesRequestRequestTypeDef,
     GetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef,
     GetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef,
     ListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef,
     ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     SearchEntitiesRequestSearchEntitiesPaginateTypeDef,
-    SearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef,
     SearchFlowTemplatesRequestSearchFlowTemplatesPaginateTypeDef,
     SearchThingsRequestSearchThingsPaginateTypeDef,
+    SearchFlowExecutionsRequestRequestTypeDef,
+    SearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef,
     SearchSystemInstancesRequestRequestTypeDef,
     SearchSystemInstancesRequestSearchSystemInstancesPaginateTypeDef,
     SearchSystemTemplatesRequestRequestTypeDef,
     SearchSystemTemplatesRequestSearchSystemTemplatesPaginateTypeDef,
     SearchThingsResponseTypeDef,
     GetEntitiesResponseTypeDef,
     SearchEntitiesResponseTypeDef,
     GetFlowTemplateResponseTypeDef,
     GetSystemTemplateResponseTypeDef,
     GetSystemInstanceResponseTypeDef,
 )
 
 
-def get_structure() -> AssociateEntityToThingRequestRequestTypeDef:
+def get_value() -> AssociateEntityToThingRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-iotthingsgraph-1.28.15.post1/mypy_boto3_iotthingsgraph/__init__.py` & `mypy-boto3-iotthingsgraph-1.28.16/mypy_boto3_iotthingsgraph/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotthingsgraph-1.28.15.post1/mypy_boto3_iotthingsgraph/__init__.pyi` & `mypy-boto3-iotthingsgraph-1.28.16/mypy_boto3_iotthingsgraph/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotthingsgraph-1.28.15.post1/mypy_boto3_iotthingsgraph/__main__.py` & `mypy-boto3-iotthingsgraph-1.28.16/mypy_boto3_iotthingsgraph/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.IoTThingsGraph 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.IoTThingsGraph 1.28.16\nVersion:         1.28.16\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph\nOther"
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

### Comparing `mypy-boto3-iotthingsgraph-1.28.15.post1/mypy_boto3_iotthingsgraph/client.py` & `mypy-boto3-iotthingsgraph-1.28.16/mypy_boto3_iotthingsgraph/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from mypy_boto3_iotthingsgraph.client import IoTThingsGraphClient
 
     session = Session()
     client: IoTThingsGraphClient = session.client("iotthingsgraph")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import DeploymentTargetType, EntityTypeType
 from .paginator import (
     GetFlowTemplateRevisionsPaginator,
     GetSystemTemplateRevisionsPaginator,
@@ -58,14 +57,15 @@
     SearchFlowTemplatesResponseTypeDef,
     SearchSystemInstancesResponseTypeDef,
     SearchSystemTemplatesResponseTypeDef,
     SearchThingsResponseTypeDef,
     SystemInstanceFilterTypeDef,
     SystemTemplateFilterTypeDef,
     TagTypeDef,
+    TimestampTypeDef,
     UndeploySystemInstanceResponseTypeDef,
     UpdateFlowTemplateResponseTypeDef,
     UpdateSystemTemplateResponseTypeDef,
     UploadEntityDefinitionsResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
@@ -380,16 +380,16 @@
         """
 
     def search_flow_executions(
         self,
         *,
         systemInstanceId: str,
         flowExecutionId: str = ...,
-        startTime: Union[datetime, str] = ...,
-        endTime: Union[datetime, str] = ...,
+        startTime: TimestampTypeDef = ...,
+        endTime: TimestampTypeDef = ...,
         nextToken: str = ...,
         maxResults: int = ...
     ) -> SearchFlowExecutionsResponseTypeDef:
         """
         Searches for AWS IoT Things Graph workflow execution instances.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Client.search_flow_executions)
```

### Comparing `mypy-boto3-iotthingsgraph-1.28.15.post1/mypy_boto3_iotthingsgraph/client.pyi` & `mypy-boto3-iotthingsgraph-1.28.16/mypy_boto3_iotthingsgraph/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from mypy_boto3_iotthingsgraph.client import IoTThingsGraphClient
 
     session = Session()
     client: IoTThingsGraphClient = session.client("iotthingsgraph")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import DeploymentTargetType, EntityTypeType
 from .paginator import (
     GetFlowTemplateRevisionsPaginator,
     GetSystemTemplateRevisionsPaginator,
@@ -58,14 +57,15 @@
     SearchFlowTemplatesResponseTypeDef,
     SearchSystemInstancesResponseTypeDef,
     SearchSystemTemplatesResponseTypeDef,
     SearchThingsResponseTypeDef,
     SystemInstanceFilterTypeDef,
     SystemTemplateFilterTypeDef,
     TagTypeDef,
+    TimestampTypeDef,
     UndeploySystemInstanceResponseTypeDef,
     UpdateFlowTemplateResponseTypeDef,
     UpdateSystemTemplateResponseTypeDef,
     UploadEntityDefinitionsResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
@@ -348,16 +348,16 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/client/#search_entities)
         """
     def search_flow_executions(
         self,
         *,
         systemInstanceId: str,
         flowExecutionId: str = ...,
-        startTime: Union[datetime, str] = ...,
-        endTime: Union[datetime, str] = ...,
+        startTime: TimestampTypeDef = ...,
+        endTime: TimestampTypeDef = ...,
         nextToken: str = ...,
         maxResults: int = ...
     ) -> SearchFlowExecutionsResponseTypeDef:
         """
         Searches for AWS IoT Things Graph workflow execution instances.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Client.search_flow_executions)
```

### Comparing `mypy-boto3-iotthingsgraph-1.28.15.post1/mypy_boto3_iotthingsgraph/literals.py` & `mypy-boto3-iotthingsgraph-1.28.16/mypy_boto3_iotthingsgraph/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotthingsgraph-1.28.15.post1/mypy_boto3_iotthingsgraph/literals.pyi` & `mypy-boto3-iotthingsgraph-1.28.16/mypy_boto3_iotthingsgraph/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotthingsgraph-1.28.15.post1/mypy_boto3_iotthingsgraph/paginator.py` & `mypy-boto3-iotthingsgraph-1.28.16/mypy_boto3_iotthingsgraph/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,16 +33,15 @@
     search_flow_executions_paginator: SearchFlowExecutionsPaginator = client.get_paginator("search_flow_executions")
     search_flow_templates_paginator: SearchFlowTemplatesPaginator = client.get_paginator("search_flow_templates")
     search_system_instances_paginator: SearchSystemInstancesPaginator = client.get_paginator("search_system_instances")
     search_system_templates_paginator: SearchSystemTemplatesPaginator = client.get_paginator("search_system_templates")
     search_things_paginator: SearchThingsPaginator = client.get_paginator("search_things")
     ```
 """
-from datetime import datetime
-from typing import Generic, Iterator, Sequence, TypeVar, Union
+from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import EntityTypeType
 from .type_defs import (
     EntityFilterTypeDef,
     FlowTemplateFilterTypeDef,
@@ -55,14 +54,15 @@
     SearchFlowExecutionsResponseTypeDef,
     SearchFlowTemplatesResponseTypeDef,
     SearchSystemInstancesResponseTypeDef,
     SearchSystemTemplatesResponseTypeDef,
     SearchThingsResponseTypeDef,
     SystemInstanceFilterTypeDef,
     SystemTemplateFilterTypeDef,
+    TimestampTypeDef,
 )
 
 __all__ = (
     "GetFlowTemplateRevisionsPaginator",
     "GetSystemTemplateRevisionsPaginator",
     "ListFlowExecutionMessagesPaginator",
     "ListTagsForResourcePaginator",
@@ -172,16 +172,16 @@
     """
 
     def paginate(
         self,
         *,
         systemInstanceId: str,
         flowExecutionId: str = ...,
-        startTime: Union[datetime, str] = ...,
-        endTime: Union[datetime, str] = ...,
+        startTime: TimestampTypeDef = ...,
+        endTime: TimestampTypeDef = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[SearchFlowExecutionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.SearchFlowExecutions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/paginators/#searchflowexecutionspaginator)
         """
```

### Comparing `mypy-boto3-iotthingsgraph-1.28.15.post1/mypy_boto3_iotthingsgraph/paginator.pyi` & `mypy-boto3-iotthingsgraph-1.28.16/mypy_boto3_iotthingsgraph/paginator.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -33,16 +33,15 @@
     search_flow_executions_paginator: SearchFlowExecutionsPaginator = client.get_paginator("search_flow_executions")
     search_flow_templates_paginator: SearchFlowTemplatesPaginator = client.get_paginator("search_flow_templates")
     search_system_instances_paginator: SearchSystemInstancesPaginator = client.get_paginator("search_system_instances")
     search_system_templates_paginator: SearchSystemTemplatesPaginator = client.get_paginator("search_system_templates")
     search_things_paginator: SearchThingsPaginator = client.get_paginator("search_things")
     ```
 """
-from datetime import datetime
-from typing import Generic, Iterator, Sequence, TypeVar, Union
+from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import EntityTypeType
 from .type_defs import (
     EntityFilterTypeDef,
     FlowTemplateFilterTypeDef,
@@ -55,14 +54,15 @@
     SearchFlowExecutionsResponseTypeDef,
     SearchFlowTemplatesResponseTypeDef,
     SearchSystemInstancesResponseTypeDef,
     SearchSystemTemplatesResponseTypeDef,
     SearchThingsResponseTypeDef,
     SystemInstanceFilterTypeDef,
     SystemTemplateFilterTypeDef,
+    TimestampTypeDef,
 )
 
 __all__ = (
     "GetFlowTemplateRevisionsPaginator",
     "GetSystemTemplateRevisionsPaginator",
     "ListFlowExecutionMessagesPaginator",
     "ListTagsForResourcePaginator",
@@ -164,16 +164,16 @@
     """
 
     def paginate(
         self,
         *,
         systemInstanceId: str,
         flowExecutionId: str = ...,
-        startTime: Union[datetime, str] = ...,
-        endTime: Union[datetime, str] = ...,
+        startTime: TimestampTypeDef = ...,
+        endTime: TimestampTypeDef = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[SearchFlowExecutionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.SearchFlowExecutions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/paginators/#searchflowexecutionspaginator)
         """
```

### Comparing `mypy-boto3-iotthingsgraph-1.28.15.post1/mypy_boto3_iotthingsgraph/type_defs.py` & `mypy-boto3-iotthingsgraph-1.28.16/mypy_boto3_iotthingsgraph/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_iotthingsgraph.type_defs import AssociateEntityToThingRequestRequestTypeDef
 
-    data: AssociateEntityToThingRequestRequestTypeDef = {...}
+    data: AssociateEntityToThingRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -65,15 +65,15 @@
     "GetFlowTemplateRevisionsRequestRequestTypeDef",
     "GetSystemInstanceRequestRequestTypeDef",
     "GetSystemTemplateRequestRequestTypeDef",
     "GetSystemTemplateRevisionsRequestRequestTypeDef",
     "GetUploadStatusRequestRequestTypeDef",
     "ListFlowExecutionMessagesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "SearchFlowExecutionsRequestRequestTypeDef",
+    "TimestampTypeDef",
     "SystemInstanceFilterTypeDef",
     "SystemTemplateFilterTypeDef",
     "SearchThingsRequestRequestTypeDef",
     "ThingTypeDef",
     "UndeploySystemInstanceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "CreateFlowTemplateRequestRequestTypeDef",
@@ -110,17 +110,18 @@
     "SearchFlowExecutionsResponseTypeDef",
     "SearchFlowTemplatesRequestRequestTypeDef",
     "GetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef",
     "GetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef",
     "ListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef",
     "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "SearchEntitiesRequestSearchEntitiesPaginateTypeDef",
-    "SearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef",
     "SearchFlowTemplatesRequestSearchFlowTemplatesPaginateTypeDef",
     "SearchThingsRequestSearchThingsPaginateTypeDef",
+    "SearchFlowExecutionsRequestRequestTypeDef",
+    "SearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef",
     "SearchSystemInstancesRequestRequestTypeDef",
     "SearchSystemInstancesRequestSearchSystemInstancesPaginateTypeDef",
     "SearchSystemTemplatesRequestRequestTypeDef",
     "SearchSystemTemplatesRequestSearchSystemTemplatesPaginateTypeDef",
     "SearchThingsResponseTypeDef",
     "GetEntitiesResponseTypeDef",
     "SearchEntitiesResponseTypeDef",
@@ -511,40 +512,15 @@
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredSearchFlowExecutionsRequestRequestTypeDef = TypedDict(
-    "_RequiredSearchFlowExecutionsRequestRequestTypeDef",
-    {
-        "systemInstanceId": str,
-    },
-)
-_OptionalSearchFlowExecutionsRequestRequestTypeDef = TypedDict(
-    "_OptionalSearchFlowExecutionsRequestRequestTypeDef",
-    {
-        "flowExecutionId": str,
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-        "nextToken": str,
-        "maxResults": int,
-    },
-    total=False,
-)
-
-
-class SearchFlowExecutionsRequestRequestTypeDef(
-    _RequiredSearchFlowExecutionsRequestRequestTypeDef,
-    _OptionalSearchFlowExecutionsRequestRequestTypeDef,
-):
-    pass
-
-
+TimestampTypeDef = Union[datetime, str]
 SystemInstanceFilterTypeDef = TypedDict(
     "SystemInstanceFilterTypeDef",
     {
         "name": SystemInstanceFilterNameType,
         "value": Sequence[str],
     },
     total=False,
@@ -1113,67 +1089,93 @@
 class SearchEntitiesRequestSearchEntitiesPaginateTypeDef(
     _RequiredSearchEntitiesRequestSearchEntitiesPaginateTypeDef,
     _OptionalSearchEntitiesRequestSearchEntitiesPaginateTypeDef,
 ):
     pass
 
 
-_RequiredSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef = TypedDict(
-    "_RequiredSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef",
+SearchFlowTemplatesRequestSearchFlowTemplatesPaginateTypeDef = TypedDict(
+    "SearchFlowTemplatesRequestSearchFlowTemplatesPaginateTypeDef",
     {
-        "systemInstanceId": str,
+        "filters": Sequence[FlowTemplateFilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredSearchThingsRequestSearchThingsPaginateTypeDef = TypedDict(
+    "_RequiredSearchThingsRequestSearchThingsPaginateTypeDef",
+    {
+        "entityId": str,
     },
 )
-_OptionalSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef = TypedDict(
-    "_OptionalSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef",
+_OptionalSearchThingsRequestSearchThingsPaginateTypeDef = TypedDict(
+    "_OptionalSearchThingsRequestSearchThingsPaginateTypeDef",
     {
-        "flowExecutionId": str,
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
+        "namespaceVersion": int,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
-class SearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef(
-    _RequiredSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef,
-    _OptionalSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef,
+class SearchThingsRequestSearchThingsPaginateTypeDef(
+    _RequiredSearchThingsRequestSearchThingsPaginateTypeDef,
+    _OptionalSearchThingsRequestSearchThingsPaginateTypeDef,
 ):
     pass
 
 
-SearchFlowTemplatesRequestSearchFlowTemplatesPaginateTypeDef = TypedDict(
-    "SearchFlowTemplatesRequestSearchFlowTemplatesPaginateTypeDef",
+_RequiredSearchFlowExecutionsRequestRequestTypeDef = TypedDict(
+    "_RequiredSearchFlowExecutionsRequestRequestTypeDef",
     {
-        "filters": Sequence[FlowTemplateFilterTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "systemInstanceId": str,
+    },
+)
+_OptionalSearchFlowExecutionsRequestRequestTypeDef = TypedDict(
+    "_OptionalSearchFlowExecutionsRequestRequestTypeDef",
+    {
+        "flowExecutionId": str,
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
+        "nextToken": str,
+        "maxResults": int,
     },
     total=False,
 )
 
-_RequiredSearchThingsRequestSearchThingsPaginateTypeDef = TypedDict(
-    "_RequiredSearchThingsRequestSearchThingsPaginateTypeDef",
+
+class SearchFlowExecutionsRequestRequestTypeDef(
+    _RequiredSearchFlowExecutionsRequestRequestTypeDef,
+    _OptionalSearchFlowExecutionsRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef = TypedDict(
+    "_RequiredSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef",
     {
-        "entityId": str,
+        "systemInstanceId": str,
     },
 )
-_OptionalSearchThingsRequestSearchThingsPaginateTypeDef = TypedDict(
-    "_OptionalSearchThingsRequestSearchThingsPaginateTypeDef",
+_OptionalSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef = TypedDict(
+    "_OptionalSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef",
     {
-        "namespaceVersion": int,
+        "flowExecutionId": str,
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
-class SearchThingsRequestSearchThingsPaginateTypeDef(
-    _RequiredSearchThingsRequestSearchThingsPaginateTypeDef,
-    _OptionalSearchThingsRequestSearchThingsPaginateTypeDef,
+class SearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef(
+    _RequiredSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef,
+    _OptionalSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef,
 ):
     pass
 
 
 SearchSystemInstancesRequestRequestTypeDef = TypedDict(
     "SearchSystemInstancesRequestRequestTypeDef",
     {
```

### Comparing `mypy-boto3-iotthingsgraph-1.28.15.post1/mypy_boto3_iotthingsgraph/type_defs.pyi` & `mypy-boto3-iotthingsgraph-1.28.16/mypy_boto3_iotthingsgraph/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_iotthingsgraph.type_defs import AssociateEntityToThingRequestRequestTypeDef
 
-    data: AssociateEntityToThingRequestRequestTypeDef = {...}
+    data: AssociateEntityToThingRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -64,15 +64,15 @@
     "GetFlowTemplateRevisionsRequestRequestTypeDef",
     "GetSystemInstanceRequestRequestTypeDef",
     "GetSystemTemplateRequestRequestTypeDef",
     "GetSystemTemplateRevisionsRequestRequestTypeDef",
     "GetUploadStatusRequestRequestTypeDef",
     "ListFlowExecutionMessagesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "SearchFlowExecutionsRequestRequestTypeDef",
+    "TimestampTypeDef",
     "SystemInstanceFilterTypeDef",
     "SystemTemplateFilterTypeDef",
     "SearchThingsRequestRequestTypeDef",
     "ThingTypeDef",
     "UndeploySystemInstanceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "CreateFlowTemplateRequestRequestTypeDef",
@@ -109,17 +109,18 @@
     "SearchFlowExecutionsResponseTypeDef",
     "SearchFlowTemplatesRequestRequestTypeDef",
     "GetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef",
     "GetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef",
     "ListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef",
     "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "SearchEntitiesRequestSearchEntitiesPaginateTypeDef",
-    "SearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef",
     "SearchFlowTemplatesRequestSearchFlowTemplatesPaginateTypeDef",
     "SearchThingsRequestSearchThingsPaginateTypeDef",
+    "SearchFlowExecutionsRequestRequestTypeDef",
+    "SearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef",
     "SearchSystemInstancesRequestRequestTypeDef",
     "SearchSystemInstancesRequestSearchSystemInstancesPaginateTypeDef",
     "SearchSystemTemplatesRequestRequestTypeDef",
     "SearchSystemTemplatesRequestSearchSystemTemplatesPaginateTypeDef",
     "SearchThingsResponseTypeDef",
     "GetEntitiesResponseTypeDef",
     "SearchEntitiesResponseTypeDef",
@@ -494,38 +495,15 @@
 
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
-_RequiredSearchFlowExecutionsRequestRequestTypeDef = TypedDict(
-    "_RequiredSearchFlowExecutionsRequestRequestTypeDef",
-    {
-        "systemInstanceId": str,
-    },
-)
-_OptionalSearchFlowExecutionsRequestRequestTypeDef = TypedDict(
-    "_OptionalSearchFlowExecutionsRequestRequestTypeDef",
-    {
-        "flowExecutionId": str,
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-        "nextToken": str,
-        "maxResults": int,
-    },
-    total=False,
-)
-
-class SearchFlowExecutionsRequestRequestTypeDef(
-    _RequiredSearchFlowExecutionsRequestRequestTypeDef,
-    _OptionalSearchFlowExecutionsRequestRequestTypeDef,
-):
-    pass
-
+TimestampTypeDef = Union[datetime, str]
 SystemInstanceFilterTypeDef = TypedDict(
     "SystemInstanceFilterTypeDef",
     {
         "name": SystemInstanceFilterNameType,
         "value": Sequence[str],
     },
     total=False,
@@ -1070,37 +1048,14 @@
 
 class SearchEntitiesRequestSearchEntitiesPaginateTypeDef(
     _RequiredSearchEntitiesRequestSearchEntitiesPaginateTypeDef,
     _OptionalSearchEntitiesRequestSearchEntitiesPaginateTypeDef,
 ):
     pass
 
-_RequiredSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef = TypedDict(
-    "_RequiredSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef",
-    {
-        "systemInstanceId": str,
-    },
-)
-_OptionalSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef = TypedDict(
-    "_OptionalSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef",
-    {
-        "flowExecutionId": str,
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class SearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef(
-    _RequiredSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef,
-    _OptionalSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef,
-):
-    pass
-
 SearchFlowTemplatesRequestSearchFlowTemplatesPaginateTypeDef = TypedDict(
     "SearchFlowTemplatesRequestSearchFlowTemplatesPaginateTypeDef",
     {
         "filters": Sequence[FlowTemplateFilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -1123,14 +1078,61 @@
 
 class SearchThingsRequestSearchThingsPaginateTypeDef(
     _RequiredSearchThingsRequestSearchThingsPaginateTypeDef,
     _OptionalSearchThingsRequestSearchThingsPaginateTypeDef,
 ):
     pass
 
+_RequiredSearchFlowExecutionsRequestRequestTypeDef = TypedDict(
+    "_RequiredSearchFlowExecutionsRequestRequestTypeDef",
+    {
+        "systemInstanceId": str,
+    },
+)
+_OptionalSearchFlowExecutionsRequestRequestTypeDef = TypedDict(
+    "_OptionalSearchFlowExecutionsRequestRequestTypeDef",
+    {
+        "flowExecutionId": str,
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
+        "nextToken": str,
+        "maxResults": int,
+    },
+    total=False,
+)
+
+class SearchFlowExecutionsRequestRequestTypeDef(
+    _RequiredSearchFlowExecutionsRequestRequestTypeDef,
+    _OptionalSearchFlowExecutionsRequestRequestTypeDef,
+):
+    pass
+
+_RequiredSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef = TypedDict(
+    "_RequiredSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef",
+    {
+        "systemInstanceId": str,
+    },
+)
+_OptionalSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef = TypedDict(
+    "_OptionalSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef",
+    {
+        "flowExecutionId": str,
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class SearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef(
+    _RequiredSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef,
+    _OptionalSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef,
+):
+    pass
+
 SearchSystemInstancesRequestRequestTypeDef = TypedDict(
     "SearchSystemInstancesRequestRequestTypeDef",
     {
         "filters": Sequence[SystemInstanceFilterTypeDef],
         "nextToken": str,
         "maxResults": int,
     },
```

### Comparing `mypy-boto3-iotthingsgraph-1.28.15.post1/mypy_boto3_iotthingsgraph.egg-info/PKG-INFO` & `mypy-boto3-iotthingsgraph-1.28.16/mypy_boto3_iotthingsgraph.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iotthingsgraph
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.IoTThingsGraph 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.IoTThingsGraph 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 iotthingsgraph type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 iotthingsgraph type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotthingsgraph.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotthingsgraph)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iotthingsgraph)](https://pepy.tech/project/mypy-boto3-iotthingsgraph)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTThingsGraph 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph)
+[boto3.IoTThingsGraph 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph)
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
 [mypy-boto3-iotthingsgraph docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/).
 
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
@@ -369,20 +369,20 @@
 )
 
 
 def check_value(value: DefinitionLanguageType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_iotthingsgraph.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_iotthingsgraph.type_defs import (
     AssociateEntityToThingRequestRequestTypeDef,
     DefinitionDocumentTypeDef,
     FlowTemplateSummaryTypeDef,
     ResponseMetadataTypeDef,
@@ -409,15 +409,15 @@
     GetFlowTemplateRevisionsRequestRequestTypeDef,
     GetSystemInstanceRequestRequestTypeDef,
     GetSystemTemplateRequestRequestTypeDef,
     GetSystemTemplateRevisionsRequestRequestTypeDef,
     GetUploadStatusRequestRequestTypeDef,
     ListFlowExecutionMessagesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    SearchFlowExecutionsRequestRequestTypeDef,
+    TimestampTypeDef,
     SystemInstanceFilterTypeDef,
     SystemTemplateFilterTypeDef,
     SearchThingsRequestRequestTypeDef,
     ThingTypeDef,
     UndeploySystemInstanceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     CreateFlowTemplateRequestRequestTypeDef,
@@ -454,31 +454,32 @@
     SearchFlowExecutionsResponseTypeDef,
     SearchFlowTemplatesRequestRequestTypeDef,
     GetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef,
     GetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef,
     ListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef,
     ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     SearchEntitiesRequestSearchEntitiesPaginateTypeDef,
-    SearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef,
     SearchFlowTemplatesRequestSearchFlowTemplatesPaginateTypeDef,
     SearchThingsRequestSearchThingsPaginateTypeDef,
+    SearchFlowExecutionsRequestRequestTypeDef,
+    SearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef,
     SearchSystemInstancesRequestRequestTypeDef,
     SearchSystemInstancesRequestSearchSystemInstancesPaginateTypeDef,
     SearchSystemTemplatesRequestRequestTypeDef,
     SearchSystemTemplatesRequestSearchSystemTemplatesPaginateTypeDef,
     SearchThingsResponseTypeDef,
     GetEntitiesResponseTypeDef,
     SearchEntitiesResponseTypeDef,
     GetFlowTemplateResponseTypeDef,
     GetSystemTemplateResponseTypeDef,
     GetSystemInstanceResponseTypeDef,
 )
 
 
-def get_structure() -> AssociateEntityToThingRequestRequestTypeDef:
+def get_value() -> AssociateEntityToThingRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-iotthingsgraph-1.28.15.post1/mypy_boto3_iotthingsgraph.egg-info/SOURCES.txt` & `mypy-boto3-iotthingsgraph-1.28.16/mypy_boto3_iotthingsgraph.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotthingsgraph-1.28.15.post1/setup.py` & `mypy-boto3-iotthingsgraph-1.28.16/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-iotthingsgraph",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_iotthingsgraph"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.IoTThingsGraph 1.28.15 service generated with"
-        " mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.IoTThingsGraph 1.28.16 service generated with"
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
-    keywords="boto3 iotthingsgraph type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 iotthingsgraph type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_iotthingsgraph": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

