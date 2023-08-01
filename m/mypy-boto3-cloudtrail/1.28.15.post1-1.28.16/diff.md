# Comparing `tmp/mypy-boto3-cloudtrail-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-cloudtrail-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-cloudtrail-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:44 2023, max compression
+gzip compressed data, was "mypy-boto3-cloudtrail-1.28.16.tar", last modified: Tue Aug  1 11:36:25 2023, max compression
```

## Comparing `mypy-boto3-cloudtrail-1.28.15.post1.tar` & `mypy-boto3-cloudtrail-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:44.673062 mypy-boto3-cloudtrail-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:40:14.000000 mypy-boto3-cloudtrail-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17912 2023-07-29 10:02:44.673062 mypy-boto3-cloudtrail-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16407 2023-07-29 09:40:14.000000 mypy-boto3-cloudtrail-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:44.661062 mypy-boto3-cloudtrail-1.28.15.post1/mypy_boto3_cloudtrail/
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-29 09:40:14.000000 mypy-boto3-cloudtrail-1.28.15.post1/mypy_boto3_cloudtrail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-07-29 09:40:14.000000 mypy-boto3-cloudtrail-1.28.15.post1/mypy_boto3_cloudtrail/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-29 09:40:14.000000 mypy-boto3-cloudtrail-1.28.15.post1/mypy_boto3_cloudtrail/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39378 2023-07-29 09:40:15.000000 mypy-boto3-cloudtrail-1.28.15.post1/mypy_boto3_cloudtrail/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    39319 2023-07-29 09:40:14.000000 mypy-boto3-cloudtrail-1.28.15.post1/mypy_boto3_cloudtrail/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10189 2023-07-29 09:40:15.000000 mypy-boto3-cloudtrail-1.28.15.post1/mypy_boto3_cloudtrail/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10187 2023-07-29 09:40:15.000000 mypy-boto3-cloudtrail-1.28.15.post1/mypy_boto3_cloudtrail/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-07-29 09:40:15.000000 mypy-boto3-cloudtrail-1.28.15.post1/mypy_boto3_cloudtrail/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7598 2023-07-29 09:40:15.000000 mypy-boto3-cloudtrail-1.28.15.post1/mypy_boto3_cloudtrail/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:40:14.000000 mypy-boto3-cloudtrail-1.28.15.post1/mypy_boto3_cloudtrail/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    41778 2023-07-29 09:40:17.000000 mypy-boto3-cloudtrail-1.28.15.post1/mypy_boto3_cloudtrail/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    41739 2023-07-29 09:40:17.000000 mypy-boto3-cloudtrail-1.28.15.post1/mypy_boto3_cloudtrail/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:40:14.000000 mypy-boto3-cloudtrail-1.28.15.post1/mypy_boto3_cloudtrail/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:44.673062 mypy-boto3-cloudtrail-1.28.15.post1/mypy_boto3_cloudtrail.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17912 2023-07-29 10:02:44.000000 mypy-boto3-cloudtrail-1.28.15.post1/mypy_boto3_cloudtrail.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-29 10:02:44.000000 mypy-boto3-cloudtrail-1.28.15.post1/mypy_boto3_cloudtrail.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:44.000000 mypy-boto3-cloudtrail-1.28.15.post1/mypy_boto3_cloudtrail.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:44.000000 mypy-boto3-cloudtrail-1.28.15.post1/mypy_boto3_cloudtrail.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:44.000000 mypy-boto3-cloudtrail-1.28.15.post1/mypy_boto3_cloudtrail.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-29 10:02:44.000000 mypy-boto3-cloudtrail-1.28.15.post1/mypy_boto3_cloudtrail.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:44.673062 mypy-boto3-cloudtrail-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-07-29 09:40:14.000000 mypy-boto3-cloudtrail-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:25.524928 mypy-boto3-cloudtrail-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:12:48.000000 mypy-boto3-cloudtrail-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17994 2023-08-01 11:36:25.524928 mypy-boto3-cloudtrail-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16498 2023-08-01 11:12:48.000000 mypy-boto3-cloudtrail-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:25.524928 mypy-boto3-cloudtrail-1.28.16/mypy_boto3_cloudtrail/
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-08-01 11:12:48.000000 mypy-boto3-cloudtrail-1.28.16/mypy_boto3_cloudtrail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-08-01 11:12:48.000000 mypy-boto3-cloudtrail-1.28.16/mypy_boto3_cloudtrail/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-08-01 11:12:48.000000 mypy-boto3-cloudtrail-1.28.16/mypy_boto3_cloudtrail/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39059 2023-08-01 11:12:48.000000 mypy-boto3-cloudtrail-1.28.16/mypy_boto3_cloudtrail/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39000 2023-08-01 11:12:48.000000 mypy-boto3-cloudtrail-1.28.16/mypy_boto3_cloudtrail/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10189 2023-08-01 11:12:48.000000 mypy-boto3-cloudtrail-1.28.16/mypy_boto3_cloudtrail/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10187 2023-08-01 11:12:48.000000 mypy-boto3-cloudtrail-1.28.16/mypy_boto3_cloudtrail/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7576 2023-08-01 11:12:48.000000 mypy-boto3-cloudtrail-1.28.16/mypy_boto3_cloudtrail/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7567 2023-08-01 11:12:48.000000 mypy-boto3-cloudtrail-1.28.16/mypy_boto3_cloudtrail/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:12:48.000000 mypy-boto3-cloudtrail-1.28.16/mypy_boto3_cloudtrail/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    41853 2023-08-01 11:12:50.000000 mypy-boto3-cloudtrail-1.28.16/mypy_boto3_cloudtrail/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41815 2023-08-01 11:12:49.000000 mypy-boto3-cloudtrail-1.28.16/mypy_boto3_cloudtrail/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:12:48.000000 mypy-boto3-cloudtrail-1.28.16/mypy_boto3_cloudtrail/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:25.524928 mypy-boto3-cloudtrail-1.28.16/mypy_boto3_cloudtrail.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17994 2023-08-01 11:36:25.000000 mypy-boto3-cloudtrail-1.28.16/mypy_boto3_cloudtrail.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-08-01 11:36:25.000000 mypy-boto3-cloudtrail-1.28.16/mypy_boto3_cloudtrail.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:25.000000 mypy-boto3-cloudtrail-1.28.16/mypy_boto3_cloudtrail.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:25.000000 mypy-boto3-cloudtrail-1.28.16/mypy_boto3_cloudtrail.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:25.000000 mypy-boto3-cloudtrail-1.28.16/mypy_boto3_cloudtrail.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-01 11:36:25.000000 mypy-boto3-cloudtrail-1.28.16/mypy_boto3_cloudtrail.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:25.524928 mypy-boto3-cloudtrail-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-08-01 11:12:48.000000 mypy-boto3-cloudtrail-1.28.16/setup.py
```

### Comparing `mypy-boto3-cloudtrail-1.28.15.post1/LICENSE` & `mypy-boto3-cloudtrail-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudtrail-1.28.15.post1/PKG-INFO` & `mypy-boto3-cloudtrail-1.28.16/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cloudtrail
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.CloudTrail 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.CloudTrail 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 cloudtrail type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 cloudtrail type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudtrail.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudtrail)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cloudtrail)](https://pepy.tech/project/mypy-boto3-cloudtrail)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudTrail 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail)
+[boto3.CloudTrail 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail)
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
 [mypy-boto3-cloudtrail docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/).
 
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
@@ -338,20 +338,20 @@
 )
 
 
 def check_value(value: DeliveryStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_cloudtrail.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_cloudtrail.type_defs import (
     TagTypeDef,
     AdvancedFieldSelectorOutputTypeDef,
     AdvancedFieldSelectorTypeDef,
     CancelQueryRequestRequestTypeDef,
@@ -387,17 +387,16 @@
     S3ImportSourceTypeDef,
     ImportsListItemTypeDef,
     ListChannelsRequestRequestTypeDef,
     ListEventDataStoresRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     ListImportFailuresRequestRequestTypeDef,
     ListImportsRequestRequestTypeDef,
-    ListPublicKeysRequestRequestTypeDef,
+    TimestampTypeDef,
     PublicKeyTypeDef,
-    ListQueriesRequestRequestTypeDef,
     QueryTypeDef,
     ListTagsRequestRequestTypeDef,
     ListTrailsRequestRequestTypeDef,
     TrailInfoTypeDef,
     LookupAttributeTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
     RegisterOrganizationDelegatedAdminRequestRequestTypeDef,
@@ -438,45 +437,49 @@
     PutInsightSelectorsResponseTypeDef,
     GetQueryResultsResponseTypeDef,
     ListImportFailuresResponseTypeDef,
     ImportSourceTypeDef,
     ListImportsResponseTypeDef,
     ListImportFailuresRequestListImportFailuresPaginateTypeDef,
     ListImportsRequestListImportsPaginateTypeDef,
-    ListPublicKeysRequestListPublicKeysPaginateTypeDef,
     ListTagsRequestListTagsPaginateTypeDef,
     ListTrailsRequestListTrailsPaginateTypeDef,
+    ListPublicKeysRequestListPublicKeysPaginateTypeDef,
+    ListPublicKeysRequestRequestTypeDef,
+    ListQueriesRequestRequestTypeDef,
     ListPublicKeysResponseTypeDef,
     ListQueriesResponseTypeDef,
     ListTrailsResponseTypeDef,
     LookupEventsRequestLookupEventsPaginateTypeDef,
     LookupEventsRequestRequestTypeDef,
     ListTagsResponseTypeDef,
     CreateEventDataStoreResponseTypeDef,
     EventDataStoreTypeDef,
     GetEventDataStoreResponseTypeDef,
     RestoreEventDataStoreResponseTypeDef,
     SourceConfigTypeDef,
     UpdateEventDataStoreResponseTypeDef,
-    CreateEventDataStoreRequestRequestTypeDef,
-    UpdateEventDataStoreRequestRequestTypeDef,
+    AdvancedEventSelectorUnionTypeDef,
     GetEventSelectorsResponseTypeDef,
     PutEventSelectorsResponseTypeDef,
-    PutEventSelectorsRequestRequestTypeDef,
+    EventSelectorUnionTypeDef,
     LookupEventsResponseTypeDef,
     GetImportResponseTypeDef,
     StartImportRequestRequestTypeDef,
     StartImportResponseTypeDef,
     StopImportResponseTypeDef,
     ListEventDataStoresResponseTypeDef,
     GetChannelResponseTypeDef,
+    CreateEventDataStoreRequestRequestTypeDef,
+    UpdateEventDataStoreRequestRequestTypeDef,
+    PutEventSelectorsRequestRequestTypeDef,
 )
 
 
-def get_structure() -> TagTypeDef:
+def get_value() -> TagTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-cloudtrail-1.28.15.post1/README.md` & `mypy-boto3-cloudtrail-1.28.16/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudtrail.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudtrail)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cloudtrail)](https://pepy.tech/project/mypy-boto3-cloudtrail)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudTrail 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail)
+[boto3.CloudTrail 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail)
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
 [mypy-boto3-cloudtrail docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/).
 
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
@@ -306,20 +306,20 @@
 )
 
 
 def check_value(value: DeliveryStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_cloudtrail.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_cloudtrail.type_defs import (
     TagTypeDef,
     AdvancedFieldSelectorOutputTypeDef,
     AdvancedFieldSelectorTypeDef,
     CancelQueryRequestRequestTypeDef,
@@ -355,17 +355,16 @@
     S3ImportSourceTypeDef,
     ImportsListItemTypeDef,
     ListChannelsRequestRequestTypeDef,
     ListEventDataStoresRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     ListImportFailuresRequestRequestTypeDef,
     ListImportsRequestRequestTypeDef,
-    ListPublicKeysRequestRequestTypeDef,
+    TimestampTypeDef,
     PublicKeyTypeDef,
-    ListQueriesRequestRequestTypeDef,
     QueryTypeDef,
     ListTagsRequestRequestTypeDef,
     ListTrailsRequestRequestTypeDef,
     TrailInfoTypeDef,
     LookupAttributeTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
     RegisterOrganizationDelegatedAdminRequestRequestTypeDef,
@@ -406,45 +405,49 @@
     PutInsightSelectorsResponseTypeDef,
     GetQueryResultsResponseTypeDef,
     ListImportFailuresResponseTypeDef,
     ImportSourceTypeDef,
     ListImportsResponseTypeDef,
     ListImportFailuresRequestListImportFailuresPaginateTypeDef,
     ListImportsRequestListImportsPaginateTypeDef,
-    ListPublicKeysRequestListPublicKeysPaginateTypeDef,
     ListTagsRequestListTagsPaginateTypeDef,
     ListTrailsRequestListTrailsPaginateTypeDef,
+    ListPublicKeysRequestListPublicKeysPaginateTypeDef,
+    ListPublicKeysRequestRequestTypeDef,
+    ListQueriesRequestRequestTypeDef,
     ListPublicKeysResponseTypeDef,
     ListQueriesResponseTypeDef,
     ListTrailsResponseTypeDef,
     LookupEventsRequestLookupEventsPaginateTypeDef,
     LookupEventsRequestRequestTypeDef,
     ListTagsResponseTypeDef,
     CreateEventDataStoreResponseTypeDef,
     EventDataStoreTypeDef,
     GetEventDataStoreResponseTypeDef,
     RestoreEventDataStoreResponseTypeDef,
     SourceConfigTypeDef,
     UpdateEventDataStoreResponseTypeDef,
-    CreateEventDataStoreRequestRequestTypeDef,
-    UpdateEventDataStoreRequestRequestTypeDef,
+    AdvancedEventSelectorUnionTypeDef,
     GetEventSelectorsResponseTypeDef,
     PutEventSelectorsResponseTypeDef,
-    PutEventSelectorsRequestRequestTypeDef,
+    EventSelectorUnionTypeDef,
     LookupEventsResponseTypeDef,
     GetImportResponseTypeDef,
     StartImportRequestRequestTypeDef,
     StartImportResponseTypeDef,
     StopImportResponseTypeDef,
     ListEventDataStoresResponseTypeDef,
     GetChannelResponseTypeDef,
+    CreateEventDataStoreRequestRequestTypeDef,
+    UpdateEventDataStoreRequestRequestTypeDef,
+    PutEventSelectorsRequestRequestTypeDef,
 )
 
 
-def get_structure() -> TagTypeDef:
+def get_value() -> TagTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-cloudtrail-1.28.15.post1/mypy_boto3_cloudtrail/__init__.py` & `mypy-boto3-cloudtrail-1.28.16/mypy_boto3_cloudtrail/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudtrail-1.28.15.post1/mypy_boto3_cloudtrail/__init__.pyi` & `mypy-boto3-cloudtrail-1.28.16/mypy_boto3_cloudtrail/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudtrail-1.28.15.post1/mypy_boto3_cloudtrail/client.py` & `mypy-boto3-cloudtrail-1.28.16/mypy_boto3_cloudtrail/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -10,40 +10,37 @@
     from mypy_boto3_cloudtrail.client import CloudTrailClient
 
     session = Session()
     client: CloudTrailClient = session.client("cloudtrail")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import ImportStatusType, QueryStatusType
 from .paginator import (
     ListImportFailuresPaginator,
     ListImportsPaginator,
     ListPublicKeysPaginator,
     ListTagsPaginator,
     ListTrailsPaginator,
     LookupEventsPaginator,
 )
 from .type_defs import (
-    AdvancedEventSelectorOutputTypeDef,
-    AdvancedEventSelectorTypeDef,
+    AdvancedEventSelectorUnionTypeDef,
     CancelQueryResponseTypeDef,
     CreateChannelResponseTypeDef,
     CreateEventDataStoreResponseTypeDef,
     CreateTrailResponseTypeDef,
     DescribeQueryResponseTypeDef,
     DescribeTrailsResponseTypeDef,
     DestinationTypeDef,
-    EventSelectorOutputTypeDef,
-    EventSelectorTypeDef,
+    EventSelectorUnionTypeDef,
     GetChannelResponseTypeDef,
     GetEventDataStoreResponseTypeDef,
     GetEventSelectorsResponseTypeDef,
     GetImportResponseTypeDef,
     GetInsightSelectorsResponseTypeDef,
     GetQueryResultsResponseTypeDef,
     GetResourcePolicyResponseTypeDef,
@@ -65,36 +62,34 @@
     PutInsightSelectorsResponseTypeDef,
     PutResourcePolicyResponseTypeDef,
     RestoreEventDataStoreResponseTypeDef,
     StartImportResponseTypeDef,
     StartQueryResponseTypeDef,
     StopImportResponseTypeDef,
     TagTypeDef,
+    TimestampTypeDef,
     UpdateChannelResponseTypeDef,
     UpdateEventDataStoreResponseTypeDef,
     UpdateTrailResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("CloudTrailClient",)
 
-
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     AccountHasOngoingImportException: Type[BotocoreClientError]
     AccountNotFoundException: Type[BotocoreClientError]
     AccountNotRegisteredException: Type[BotocoreClientError]
     AccountRegisteredException: Type[BotocoreClientError]
     CannotDelegateManagementAccountException: Type[BotocoreClientError]
     ChannelARNInvalidException: Type[BotocoreClientError]
@@ -169,15 +164,14 @@
     S3BucketDoesNotExistException: Type[BotocoreClientError]
     TagsLimitExceededException: Type[BotocoreClientError]
     TrailAlreadyExistsException: Type[BotocoreClientError]
     TrailNotFoundException: Type[BotocoreClientError]
     TrailNotProvidedException: Type[BotocoreClientError]
     UnsupportedOperationException: Type[BotocoreClientError]
 
-
 class CloudTrailClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/)
     """
 
     meta: ClientMeta
@@ -186,51 +180,46 @@
     def exceptions(self) -> Exceptions:
         """
         CloudTrailClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#exceptions)
         """
-
     def add_tags(self, *, ResourceId: str, TagsList: Sequence[TagTypeDef]) -> Dict[str, Any]:
         """
         Adds one or more tags to a trail, event data store, or channel, up to a limit of
         50.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.add_tags)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#add_tags)
         """
-
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#can_paginate)
         """
-
     def cancel_query(
         self, *, QueryId: str, EventDataStore: str = ...
     ) -> CancelQueryResponseTypeDef:
         """
         Cancels a query if the query is not in a terminated state, such as `CANCELLED`,
         `FAILED`, `TIMED_OUT`, or `FINISHED`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.cancel_query)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#cancel_query)
         """
-
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#close)
         """
-
     def create_channel(
         self,
         *,
         Name: str,
         Source: str,
         Destinations: Sequence[DestinationTypeDef],
         Tags: Sequence[TagTypeDef] = ...
@@ -238,37 +227,33 @@
         """
         Creates a channel for CloudTrail to ingest events from a partner or external
         source.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.create_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#create_channel)
         """
-
     def create_event_data_store(
         self,
         *,
         Name: str,
-        AdvancedEventSelectors: Sequence[
-            Union[AdvancedEventSelectorTypeDef, AdvancedEventSelectorOutputTypeDef]
-        ] = ...,
+        AdvancedEventSelectors: Sequence[AdvancedEventSelectorUnionTypeDef] = ...,
         MultiRegionEnabled: bool = ...,
         OrganizationEnabled: bool = ...,
         RetentionPeriod: int = ...,
         TerminationProtectionEnabled: bool = ...,
         TagsList: Sequence[TagTypeDef] = ...,
         KmsKeyId: str = ...,
         StartIngestion: bool = ...
     ) -> CreateEventDataStoreResponseTypeDef:
         """
         Creates a new event data store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.create_event_data_store)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#create_event_data_store)
         """
-
     def create_trail(
         self,
         *,
         Name: str,
         S3BucketName: str,
         S3KeyPrefix: str = ...,
         SnsTopicName: str = ...,
@@ -284,209 +269,188 @@
         """
         Creates a trail that specifies the settings for delivery of log data to an
         Amazon S3 bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.create_trail)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#create_trail)
         """
-
     def delete_channel(self, *, Channel: str) -> Dict[str, Any]:
         """
         Deletes a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.delete_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#delete_channel)
         """
-
     def delete_event_data_store(self, *, EventDataStore: str) -> Dict[str, Any]:
         """
         Disables the event data store specified by `EventDataStore`, which accepts an
         event data store ARN.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.delete_event_data_store)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#delete_event_data_store)
         """
-
     def delete_resource_policy(self, *, ResourceArn: str) -> Dict[str, Any]:
         """
         Deletes the resource-based policy attached to the CloudTrail channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.delete_resource_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#delete_resource_policy)
         """
-
     def delete_trail(self, *, Name: str) -> Dict[str, Any]:
         """
         Deletes a trail.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.delete_trail)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#delete_trail)
         """
-
     def deregister_organization_delegated_admin(
         self, *, DelegatedAdminAccountId: str
     ) -> Dict[str, Any]:
         """
         Removes CloudTrail delegated administrator permissions from a member account in
         an organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.deregister_organization_delegated_admin)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#deregister_organization_delegated_admin)
         """
-
     def describe_query(
         self, *, EventDataStore: str = ..., QueryId: str = ..., QueryAlias: str = ...
     ) -> DescribeQueryResponseTypeDef:
         """
         Returns metadata about a query, including query run time in milliseconds, number
         of events scanned and matched, and query status.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.describe_query)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#describe_query)
         """
-
     def describe_trails(
         self, *, trailNameList: Sequence[str] = ..., includeShadowTrails: bool = ...
     ) -> DescribeTrailsResponseTypeDef:
         """
         Retrieves settings for one or more trails associated with the current Region for
         your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.describe_trails)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#describe_trails)
         """
-
     def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#generate_presigned_url)
         """
-
     def get_channel(self, *, Channel: str) -> GetChannelResponseTypeDef:
         """
         Returns information about a specific channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.get_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#get_channel)
         """
-
     def get_event_data_store(self, *, EventDataStore: str) -> GetEventDataStoreResponseTypeDef:
         """
         Returns information about an event data store specified as either an ARN or the
         ID portion of the ARN.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.get_event_data_store)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#get_event_data_store)
         """
-
     def get_event_selectors(self, *, TrailName: str) -> GetEventSelectorsResponseTypeDef:
         """
         Describes the settings for the event selectors that you configured for your
         trail.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.get_event_selectors)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#get_event_selectors)
         """
-
     def get_import(self, *, ImportId: str) -> GetImportResponseTypeDef:
         """
         Returns information about a specific import.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.get_import)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#get_import)
         """
-
     def get_insight_selectors(self, *, TrailName: str) -> GetInsightSelectorsResponseTypeDef:
         """
         Describes the settings for the Insights event selectors that you configured for
         your trail.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.get_insight_selectors)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#get_insight_selectors)
         """
-
     def get_query_results(
         self,
         *,
         QueryId: str,
         EventDataStore: str = ...,
         NextToken: str = ...,
         MaxQueryResults: int = ...
     ) -> GetQueryResultsResponseTypeDef:
         """
         Gets event data results of a query.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.get_query_results)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#get_query_results)
         """
-
     def get_resource_policy(self, *, ResourceArn: str) -> GetResourcePolicyResponseTypeDef:
         """
         Retrieves the JSON text of the resource-based policy document attached to the
         CloudTrail channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.get_resource_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#get_resource_policy)
         """
-
     def get_trail(self, *, Name: str) -> GetTrailResponseTypeDef:
         """
         Returns settings information for a specified trail.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.get_trail)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#get_trail)
         """
-
     def get_trail_status(self, *, Name: str) -> GetTrailStatusResponseTypeDef:
         """
         Returns a JSON-formatted list of information about the specified trail.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.get_trail_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#get_trail_status)
         """
-
     def list_channels(
         self, *, MaxResults: int = ..., NextToken: str = ...
     ) -> ListChannelsResponseTypeDef:
         """
         Lists the channels in the current account, and their source names.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.list_channels)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#list_channels)
         """
-
     def list_event_data_stores(
         self, *, NextToken: str = ..., MaxResults: int = ...
     ) -> ListEventDataStoresResponseTypeDef:
         """
         Returns information about all event data stores in the account, in the current
         Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.list_event_data_stores)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#list_event_data_stores)
         """
-
     def list_import_failures(
         self, *, ImportId: str, MaxResults: int = ..., NextToken: str = ...
     ) -> ListImportFailuresResponseTypeDef:
         """
         Returns a list of failures for the specified import.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.list_import_failures)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#list_import_failures)
         """
-
     def list_imports(
         self,
         *,
         MaxResults: int = ...,
         Destination: str = ...,
         ImportStatus: ImportStatusType = ...,
         NextToken: str = ...
@@ -494,260 +458,235 @@
         """
         Returns information on all imports, or a select set of imports by `ImportStatus`
         or `Destination`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.list_imports)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#list_imports)
         """
-
     def list_public_keys(
         self,
         *,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         NextToken: str = ...
     ) -> ListPublicKeysResponseTypeDef:
         """
         Returns all public keys whose private keys were used to sign the digest files
         within the specified time range.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.list_public_keys)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#list_public_keys)
         """
-
     def list_queries(
         self,
         *,
         EventDataStore: str,
         NextToken: str = ...,
         MaxResults: int = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         QueryStatus: QueryStatusType = ...
     ) -> ListQueriesResponseTypeDef:
         """
         Returns a list of queries and query statuses for the past seven days.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.list_queries)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#list_queries)
         """
-
     def list_tags(
         self, *, ResourceIdList: Sequence[str], NextToken: str = ...
     ) -> ListTagsResponseTypeDef:
         """
         Lists the tags for the specified trails, event data stores, or channels in the
         current Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.list_tags)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#list_tags)
         """
-
     def list_trails(self, *, NextToken: str = ...) -> ListTrailsResponseTypeDef:
         """
         Lists trails that are in the current account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.list_trails)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#list_trails)
         """
-
     def lookup_events(
         self,
         *,
         LookupAttributes: Sequence[LookupAttributeTypeDef] = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         EventCategory: Literal["insight"] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> LookupEventsResponseTypeDef:
         """
         Looks up [management
         events](https://docs.aws.amazon.com/awscloudtrail/latest/userguide/cloudtrail-
         concepts.html#cloudtrail-concepts-management-events)_ or `CloudTrail Insights
         events <https://docs.aws.amazon.com/awscloudtrail/latest/userguide/cloudtrail-
         concepts.html#cloudtrail-concepts-insigh...`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.lookup_events)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#lookup_events)
         """
-
     def put_event_selectors(
         self,
         *,
         TrailName: str,
-        EventSelectors: Sequence[Union[EventSelectorTypeDef, EventSelectorOutputTypeDef]] = ...,
-        AdvancedEventSelectors: Sequence[
-            Union[AdvancedEventSelectorTypeDef, AdvancedEventSelectorOutputTypeDef]
-        ] = ...
+        EventSelectors: Sequence[EventSelectorUnionTypeDef] = ...,
+        AdvancedEventSelectors: Sequence[AdvancedEventSelectorUnionTypeDef] = ...
     ) -> PutEventSelectorsResponseTypeDef:
         """
         Configures an event selector or advanced event selectors for your trail.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.put_event_selectors)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#put_event_selectors)
         """
-
     def put_insight_selectors(
         self, *, TrailName: str, InsightSelectors: Sequence[InsightSelectorTypeDef]
     ) -> PutInsightSelectorsResponseTypeDef:
         """
         Lets you enable Insights event logging by specifying the Insights selectors that
         you want to enable on an existing trail.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.put_insight_selectors)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#put_insight_selectors)
         """
-
     def put_resource_policy(
         self, *, ResourceArn: str, ResourcePolicy: str
     ) -> PutResourcePolicyResponseTypeDef:
         """
         Attaches a resource-based permission policy to a CloudTrail channel that is used
         for an integration with an event source outside of Amazon Web Services.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.put_resource_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#put_resource_policy)
         """
-
     def register_organization_delegated_admin(self, *, MemberAccountId: str) -> Dict[str, Any]:
         """
         Registers an organization’s member account as the CloudTrail delegated
         administrator.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.register_organization_delegated_admin)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#register_organization_delegated_admin)
         """
-
     def remove_tags(self, *, ResourceId: str, TagsList: Sequence[TagTypeDef]) -> Dict[str, Any]:
         """
         Removes the specified tags from a trail, event data store, or channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.remove_tags)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#remove_tags)
         """
-
     def restore_event_data_store(
         self, *, EventDataStore: str
     ) -> RestoreEventDataStoreResponseTypeDef:
         """
         Restores a deleted event data store specified by `EventDataStore`, which accepts
         an event data store ARN.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.restore_event_data_store)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#restore_event_data_store)
         """
-
     def start_event_data_store_ingestion(self, *, EventDataStore: str) -> Dict[str, Any]:
         """
         Starts the ingestion of live events on an event data store specified as either
         an ARN or the ID portion of the ARN.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.start_event_data_store_ingestion)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#start_event_data_store_ingestion)
         """
-
     def start_import(
         self,
         *,
         Destinations: Sequence[str] = ...,
         ImportSource: ImportSourceTypeDef = ...,
-        StartEventTime: Union[datetime, str] = ...,
-        EndEventTime: Union[datetime, str] = ...,
+        StartEventTime: TimestampTypeDef = ...,
+        EndEventTime: TimestampTypeDef = ...,
         ImportId: str = ...
     ) -> StartImportResponseTypeDef:
         """
         Starts an import of logged trail events from a source S3 bucket to a destination
         event data store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.start_import)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#start_import)
         """
-
     def start_logging(self, *, Name: str) -> Dict[str, Any]:
         """
         Starts the recording of Amazon Web Services API calls and log file delivery for
         a trail.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.start_logging)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#start_logging)
         """
-
     def start_query(
         self,
         *,
         QueryStatement: str = ...,
         DeliveryS3Uri: str = ...,
         QueryAlias: str = ...,
         QueryParameters: Sequence[str] = ...
     ) -> StartQueryResponseTypeDef:
         """
         Starts a CloudTrail Lake query.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.start_query)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#start_query)
         """
-
     def stop_event_data_store_ingestion(self, *, EventDataStore: str) -> Dict[str, Any]:
         """
         Stops the ingestion of live events on an event data store specified as either an
         ARN or the ID portion of the ARN.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.stop_event_data_store_ingestion)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#stop_event_data_store_ingestion)
         """
-
     def stop_import(self, *, ImportId: str) -> StopImportResponseTypeDef:
         """
         Stops a specified import.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.stop_import)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#stop_import)
         """
-
     def stop_logging(self, *, Name: str) -> Dict[str, Any]:
         """
         Suspends the recording of Amazon Web Services API calls and log file delivery
         for the specified trail.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.stop_logging)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#stop_logging)
         """
-
     def update_channel(
         self, *, Channel: str, Destinations: Sequence[DestinationTypeDef] = ..., Name: str = ...
     ) -> UpdateChannelResponseTypeDef:
         """
         Updates a channel specified by a required channel ARN or UUID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.update_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#update_channel)
         """
-
     def update_event_data_store(
         self,
         *,
         EventDataStore: str,
         Name: str = ...,
-        AdvancedEventSelectors: Sequence[
-            Union[AdvancedEventSelectorTypeDef, AdvancedEventSelectorOutputTypeDef]
-        ] = ...,
+        AdvancedEventSelectors: Sequence[AdvancedEventSelectorUnionTypeDef] = ...,
         MultiRegionEnabled: bool = ...,
         OrganizationEnabled: bool = ...,
         RetentionPeriod: int = ...,
         TerminationProtectionEnabled: bool = ...,
         KmsKeyId: str = ...
     ) -> UpdateEventDataStoreResponseTypeDef:
         """
         Updates an event data store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.update_event_data_store)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#update_event_data_store)
         """
-
     def update_trail(
         self,
         *,
         Name: str,
         S3BucketName: str = ...,
         S3KeyPrefix: str = ...,
         SnsTopicName: str = ...,
@@ -762,51 +701,45 @@
         """
         Updates trail settings that control what events you are logging, and how to
         handle log files.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.update_trail)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#update_trail)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_import_failures"]
     ) -> ListImportFailuresPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["list_imports"]) -> ListImportsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["list_public_keys"]) -> ListPublicKeysPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["list_tags"]) -> ListTagsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["list_trails"]) -> ListTrailsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["lookup_events"]) -> LookupEventsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#get_paginator)
         """
```

### Comparing `mypy-boto3-cloudtrail-1.28.15.post1/mypy_boto3_cloudtrail/client.pyi` & `mypy-boto3-cloudtrail-1.28.16/mypy_boto3_cloudtrail/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,40 +10,37 @@
     from mypy_boto3_cloudtrail.client import CloudTrailClient
 
     session = Session()
     client: CloudTrailClient = session.client("cloudtrail")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import ImportStatusType, QueryStatusType
 from .paginator import (
     ListImportFailuresPaginator,
     ListImportsPaginator,
     ListPublicKeysPaginator,
     ListTagsPaginator,
     ListTrailsPaginator,
     LookupEventsPaginator,
 )
 from .type_defs import (
-    AdvancedEventSelectorOutputTypeDef,
-    AdvancedEventSelectorTypeDef,
+    AdvancedEventSelectorUnionTypeDef,
     CancelQueryResponseTypeDef,
     CreateChannelResponseTypeDef,
     CreateEventDataStoreResponseTypeDef,
     CreateTrailResponseTypeDef,
     DescribeQueryResponseTypeDef,
     DescribeTrailsResponseTypeDef,
     DestinationTypeDef,
-    EventSelectorOutputTypeDef,
-    EventSelectorTypeDef,
+    EventSelectorUnionTypeDef,
     GetChannelResponseTypeDef,
     GetEventDataStoreResponseTypeDef,
     GetEventSelectorsResponseTypeDef,
     GetImportResponseTypeDef,
     GetInsightSelectorsResponseTypeDef,
     GetQueryResultsResponseTypeDef,
     GetResourcePolicyResponseTypeDef,
@@ -65,33 +62,37 @@
     PutInsightSelectorsResponseTypeDef,
     PutResourcePolicyResponseTypeDef,
     RestoreEventDataStoreResponseTypeDef,
     StartImportResponseTypeDef,
     StartQueryResponseTypeDef,
     StopImportResponseTypeDef,
     TagTypeDef,
+    TimestampTypeDef,
     UpdateChannelResponseTypeDef,
     UpdateEventDataStoreResponseTypeDef,
     UpdateTrailResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = ("CloudTrailClient",)
 
+
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     AccountHasOngoingImportException: Type[BotocoreClientError]
     AccountNotFoundException: Type[BotocoreClientError]
     AccountNotRegisteredException: Type[BotocoreClientError]
     AccountRegisteredException: Type[BotocoreClientError]
     CannotDelegateManagementAccountException: Type[BotocoreClientError]
     ChannelARNInvalidException: Type[BotocoreClientError]
@@ -166,14 +167,15 @@
     S3BucketDoesNotExistException: Type[BotocoreClientError]
     TagsLimitExceededException: Type[BotocoreClientError]
     TrailAlreadyExistsException: Type[BotocoreClientError]
     TrailNotFoundException: Type[BotocoreClientError]
     TrailNotProvidedException: Type[BotocoreClientError]
     UnsupportedOperationException: Type[BotocoreClientError]
 
+
 class CloudTrailClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/)
     """
 
     meta: ClientMeta
@@ -182,46 +184,51 @@
     def exceptions(self) -> Exceptions:
         """
         CloudTrailClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#exceptions)
         """
+
     def add_tags(self, *, ResourceId: str, TagsList: Sequence[TagTypeDef]) -> Dict[str, Any]:
         """
         Adds one or more tags to a trail, event data store, or channel, up to a limit of
         50.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.add_tags)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#add_tags)
         """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#can_paginate)
         """
+
     def cancel_query(
         self, *, QueryId: str, EventDataStore: str = ...
     ) -> CancelQueryResponseTypeDef:
         """
         Cancels a query if the query is not in a terminated state, such as `CANCELLED`,
         `FAILED`, `TIMED_OUT`, or `FINISHED`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.cancel_query)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#cancel_query)
         """
+
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#close)
         """
+
     def create_channel(
         self,
         *,
         Name: str,
         Source: str,
         Destinations: Sequence[DestinationTypeDef],
         Tags: Sequence[TagTypeDef] = ...
@@ -229,35 +236,35 @@
         """
         Creates a channel for CloudTrail to ingest events from a partner or external
         source.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.create_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#create_channel)
         """
+
     def create_event_data_store(
         self,
         *,
         Name: str,
-        AdvancedEventSelectors: Sequence[
-            Union[AdvancedEventSelectorTypeDef, AdvancedEventSelectorOutputTypeDef]
-        ] = ...,
+        AdvancedEventSelectors: Sequence[AdvancedEventSelectorUnionTypeDef] = ...,
         MultiRegionEnabled: bool = ...,
         OrganizationEnabled: bool = ...,
         RetentionPeriod: int = ...,
         TerminationProtectionEnabled: bool = ...,
         TagsList: Sequence[TagTypeDef] = ...,
         KmsKeyId: str = ...,
         StartIngestion: bool = ...
     ) -> CreateEventDataStoreResponseTypeDef:
         """
         Creates a new event data store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.create_event_data_store)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#create_event_data_store)
         """
+
     def create_trail(
         self,
         *,
         Name: str,
         S3BucketName: str,
         S3KeyPrefix: str = ...,
         SnsTopicName: str = ...,
@@ -273,188 +280,209 @@
         """
         Creates a trail that specifies the settings for delivery of log data to an
         Amazon S3 bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.create_trail)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#create_trail)
         """
+
     def delete_channel(self, *, Channel: str) -> Dict[str, Any]:
         """
         Deletes a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.delete_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#delete_channel)
         """
+
     def delete_event_data_store(self, *, EventDataStore: str) -> Dict[str, Any]:
         """
         Disables the event data store specified by `EventDataStore`, which accepts an
         event data store ARN.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.delete_event_data_store)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#delete_event_data_store)
         """
+
     def delete_resource_policy(self, *, ResourceArn: str) -> Dict[str, Any]:
         """
         Deletes the resource-based policy attached to the CloudTrail channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.delete_resource_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#delete_resource_policy)
         """
+
     def delete_trail(self, *, Name: str) -> Dict[str, Any]:
         """
         Deletes a trail.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.delete_trail)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#delete_trail)
         """
+
     def deregister_organization_delegated_admin(
         self, *, DelegatedAdminAccountId: str
     ) -> Dict[str, Any]:
         """
         Removes CloudTrail delegated administrator permissions from a member account in
         an organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.deregister_organization_delegated_admin)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#deregister_organization_delegated_admin)
         """
+
     def describe_query(
         self, *, EventDataStore: str = ..., QueryId: str = ..., QueryAlias: str = ...
     ) -> DescribeQueryResponseTypeDef:
         """
         Returns metadata about a query, including query run time in milliseconds, number
         of events scanned and matched, and query status.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.describe_query)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#describe_query)
         """
+
     def describe_trails(
         self, *, trailNameList: Sequence[str] = ..., includeShadowTrails: bool = ...
     ) -> DescribeTrailsResponseTypeDef:
         """
         Retrieves settings for one or more trails associated with the current Region for
         your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.describe_trails)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#describe_trails)
         """
+
     def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#generate_presigned_url)
         """
+
     def get_channel(self, *, Channel: str) -> GetChannelResponseTypeDef:
         """
         Returns information about a specific channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.get_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#get_channel)
         """
+
     def get_event_data_store(self, *, EventDataStore: str) -> GetEventDataStoreResponseTypeDef:
         """
         Returns information about an event data store specified as either an ARN or the
         ID portion of the ARN.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.get_event_data_store)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#get_event_data_store)
         """
+
     def get_event_selectors(self, *, TrailName: str) -> GetEventSelectorsResponseTypeDef:
         """
         Describes the settings for the event selectors that you configured for your
         trail.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.get_event_selectors)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#get_event_selectors)
         """
+
     def get_import(self, *, ImportId: str) -> GetImportResponseTypeDef:
         """
         Returns information about a specific import.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.get_import)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#get_import)
         """
+
     def get_insight_selectors(self, *, TrailName: str) -> GetInsightSelectorsResponseTypeDef:
         """
         Describes the settings for the Insights event selectors that you configured for
         your trail.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.get_insight_selectors)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#get_insight_selectors)
         """
+
     def get_query_results(
         self,
         *,
         QueryId: str,
         EventDataStore: str = ...,
         NextToken: str = ...,
         MaxQueryResults: int = ...
     ) -> GetQueryResultsResponseTypeDef:
         """
         Gets event data results of a query.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.get_query_results)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#get_query_results)
         """
+
     def get_resource_policy(self, *, ResourceArn: str) -> GetResourcePolicyResponseTypeDef:
         """
         Retrieves the JSON text of the resource-based policy document attached to the
         CloudTrail channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.get_resource_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#get_resource_policy)
         """
+
     def get_trail(self, *, Name: str) -> GetTrailResponseTypeDef:
         """
         Returns settings information for a specified trail.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.get_trail)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#get_trail)
         """
+
     def get_trail_status(self, *, Name: str) -> GetTrailStatusResponseTypeDef:
         """
         Returns a JSON-formatted list of information about the specified trail.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.get_trail_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#get_trail_status)
         """
+
     def list_channels(
         self, *, MaxResults: int = ..., NextToken: str = ...
     ) -> ListChannelsResponseTypeDef:
         """
         Lists the channels in the current account, and their source names.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.list_channels)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#list_channels)
         """
+
     def list_event_data_stores(
         self, *, NextToken: str = ..., MaxResults: int = ...
     ) -> ListEventDataStoresResponseTypeDef:
         """
         Returns information about all event data stores in the account, in the current
         Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.list_event_data_stores)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#list_event_data_stores)
         """
+
     def list_import_failures(
         self, *, ImportId: str, MaxResults: int = ..., NextToken: str = ...
     ) -> ListImportFailuresResponseTypeDef:
         """
         Returns a list of failures for the specified import.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.list_import_failures)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#list_import_failures)
         """
+
     def list_imports(
         self,
         *,
         MaxResults: int = ...,
         Destination: str = ...,
         ImportStatus: ImportStatusType = ...,
         NextToken: str = ...
@@ -462,239 +490,256 @@
         """
         Returns information on all imports, or a select set of imports by `ImportStatus`
         or `Destination`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.list_imports)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#list_imports)
         """
+
     def list_public_keys(
         self,
         *,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         NextToken: str = ...
     ) -> ListPublicKeysResponseTypeDef:
         """
         Returns all public keys whose private keys were used to sign the digest files
         within the specified time range.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.list_public_keys)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#list_public_keys)
         """
+
     def list_queries(
         self,
         *,
         EventDataStore: str,
         NextToken: str = ...,
         MaxResults: int = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         QueryStatus: QueryStatusType = ...
     ) -> ListQueriesResponseTypeDef:
         """
         Returns a list of queries and query statuses for the past seven days.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.list_queries)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#list_queries)
         """
+
     def list_tags(
         self, *, ResourceIdList: Sequence[str], NextToken: str = ...
     ) -> ListTagsResponseTypeDef:
         """
         Lists the tags for the specified trails, event data stores, or channels in the
         current Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.list_tags)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#list_tags)
         """
+
     def list_trails(self, *, NextToken: str = ...) -> ListTrailsResponseTypeDef:
         """
         Lists trails that are in the current account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.list_trails)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#list_trails)
         """
+
     def lookup_events(
         self,
         *,
         LookupAttributes: Sequence[LookupAttributeTypeDef] = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         EventCategory: Literal["insight"] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> LookupEventsResponseTypeDef:
         """
         Looks up [management
         events](https://docs.aws.amazon.com/awscloudtrail/latest/userguide/cloudtrail-
         concepts.html#cloudtrail-concepts-management-events)_ or `CloudTrail Insights
         events <https://docs.aws.amazon.com/awscloudtrail/latest/userguide/cloudtrail-
         concepts.html#cloudtrail-concepts-insigh...`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.lookup_events)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#lookup_events)
         """
+
     def put_event_selectors(
         self,
         *,
         TrailName: str,
-        EventSelectors: Sequence[Union[EventSelectorTypeDef, EventSelectorOutputTypeDef]] = ...,
-        AdvancedEventSelectors: Sequence[
-            Union[AdvancedEventSelectorTypeDef, AdvancedEventSelectorOutputTypeDef]
-        ] = ...
+        EventSelectors: Sequence[EventSelectorUnionTypeDef] = ...,
+        AdvancedEventSelectors: Sequence[AdvancedEventSelectorUnionTypeDef] = ...
     ) -> PutEventSelectorsResponseTypeDef:
         """
         Configures an event selector or advanced event selectors for your trail.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.put_event_selectors)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#put_event_selectors)
         """
+
     def put_insight_selectors(
         self, *, TrailName: str, InsightSelectors: Sequence[InsightSelectorTypeDef]
     ) -> PutInsightSelectorsResponseTypeDef:
         """
         Lets you enable Insights event logging by specifying the Insights selectors that
         you want to enable on an existing trail.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.put_insight_selectors)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#put_insight_selectors)
         """
+
     def put_resource_policy(
         self, *, ResourceArn: str, ResourcePolicy: str
     ) -> PutResourcePolicyResponseTypeDef:
         """
         Attaches a resource-based permission policy to a CloudTrail channel that is used
         for an integration with an event source outside of Amazon Web Services.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.put_resource_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#put_resource_policy)
         """
+
     def register_organization_delegated_admin(self, *, MemberAccountId: str) -> Dict[str, Any]:
         """
         Registers an organization’s member account as the CloudTrail delegated
         administrator.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.register_organization_delegated_admin)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#register_organization_delegated_admin)
         """
+
     def remove_tags(self, *, ResourceId: str, TagsList: Sequence[TagTypeDef]) -> Dict[str, Any]:
         """
         Removes the specified tags from a trail, event data store, or channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.remove_tags)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#remove_tags)
         """
+
     def restore_event_data_store(
         self, *, EventDataStore: str
     ) -> RestoreEventDataStoreResponseTypeDef:
         """
         Restores a deleted event data store specified by `EventDataStore`, which accepts
         an event data store ARN.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.restore_event_data_store)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#restore_event_data_store)
         """
+
     def start_event_data_store_ingestion(self, *, EventDataStore: str) -> Dict[str, Any]:
         """
         Starts the ingestion of live events on an event data store specified as either
         an ARN or the ID portion of the ARN.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.start_event_data_store_ingestion)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#start_event_data_store_ingestion)
         """
+
     def start_import(
         self,
         *,
         Destinations: Sequence[str] = ...,
         ImportSource: ImportSourceTypeDef = ...,
-        StartEventTime: Union[datetime, str] = ...,
-        EndEventTime: Union[datetime, str] = ...,
+        StartEventTime: TimestampTypeDef = ...,
+        EndEventTime: TimestampTypeDef = ...,
         ImportId: str = ...
     ) -> StartImportResponseTypeDef:
         """
         Starts an import of logged trail events from a source S3 bucket to a destination
         event data store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.start_import)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#start_import)
         """
+
     def start_logging(self, *, Name: str) -> Dict[str, Any]:
         """
         Starts the recording of Amazon Web Services API calls and log file delivery for
         a trail.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.start_logging)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#start_logging)
         """
+
     def start_query(
         self,
         *,
         QueryStatement: str = ...,
         DeliveryS3Uri: str = ...,
         QueryAlias: str = ...,
         QueryParameters: Sequence[str] = ...
     ) -> StartQueryResponseTypeDef:
         """
         Starts a CloudTrail Lake query.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.start_query)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#start_query)
         """
+
     def stop_event_data_store_ingestion(self, *, EventDataStore: str) -> Dict[str, Any]:
         """
         Stops the ingestion of live events on an event data store specified as either an
         ARN or the ID portion of the ARN.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.stop_event_data_store_ingestion)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#stop_event_data_store_ingestion)
         """
+
     def stop_import(self, *, ImportId: str) -> StopImportResponseTypeDef:
         """
         Stops a specified import.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.stop_import)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#stop_import)
         """
+
     def stop_logging(self, *, Name: str) -> Dict[str, Any]:
         """
         Suspends the recording of Amazon Web Services API calls and log file delivery
         for the specified trail.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.stop_logging)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#stop_logging)
         """
+
     def update_channel(
         self, *, Channel: str, Destinations: Sequence[DestinationTypeDef] = ..., Name: str = ...
     ) -> UpdateChannelResponseTypeDef:
         """
         Updates a channel specified by a required channel ARN or UUID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.update_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#update_channel)
         """
+
     def update_event_data_store(
         self,
         *,
         EventDataStore: str,
         Name: str = ...,
-        AdvancedEventSelectors: Sequence[
-            Union[AdvancedEventSelectorTypeDef, AdvancedEventSelectorOutputTypeDef]
-        ] = ...,
+        AdvancedEventSelectors: Sequence[AdvancedEventSelectorUnionTypeDef] = ...,
         MultiRegionEnabled: bool = ...,
         OrganizationEnabled: bool = ...,
         RetentionPeriod: int = ...,
         TerminationProtectionEnabled: bool = ...,
         KmsKeyId: str = ...
     ) -> UpdateEventDataStoreResponseTypeDef:
         """
         Updates an event data store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.update_event_data_store)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#update_event_data_store)
         """
+
     def update_trail(
         self,
         *,
         Name: str,
         S3BucketName: str = ...,
         S3KeyPrefix: str = ...,
         SnsTopicName: str = ...,
@@ -709,45 +754,51 @@
         """
         Updates trail settings that control what events you are logging, and how to
         handle log files.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.update_trail)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#update_trail)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_import_failures"]
     ) -> ListImportFailuresPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["list_imports"]) -> ListImportsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["list_public_keys"]) -> ListPublicKeysPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["list_tags"]) -> ListTagsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["list_trails"]) -> ListTrailsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["lookup_events"]) -> LookupEventsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/client/#get_paginator)
         """
```

### Comparing `mypy-boto3-cloudtrail-1.28.15.post1/mypy_boto3_cloudtrail/literals.py` & `mypy-boto3-cloudtrail-1.28.16/mypy_boto3_cloudtrail/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudtrail-1.28.15.post1/mypy_boto3_cloudtrail/literals.pyi` & `mypy-boto3-cloudtrail-1.28.16/mypy_boto3_cloudtrail/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudtrail-1.28.15.post1/mypy_boto3_cloudtrail/paginator.py` & `mypy-boto3-cloudtrail-1.28.16/mypy_boto3_cloudtrail/paginator.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,29 +26,29 @@
     list_public_keys_paginator: ListPublicKeysPaginator = client.get_paginator("list_public_keys")
     list_tags_paginator: ListTagsPaginator = client.get_paginator("list_tags")
     list_trails_paginator: ListTrailsPaginator = client.get_paginator("list_trails")
     lookup_events_paginator: LookupEventsPaginator = client.get_paginator("lookup_events")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Generic, Iterator, Sequence, TypeVar, Union
+from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import ImportStatusType
 from .type_defs import (
     ListImportFailuresResponseTypeDef,
     ListImportsResponseTypeDef,
     ListPublicKeysResponseTypeDef,
     ListTagsResponseTypeDef,
     ListTrailsResponseTypeDef,
     LookupAttributeTypeDef,
     LookupEventsResponseTypeDef,
     PaginatorConfigTypeDef,
+    TimestampTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -112,16 +112,16 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Paginator.ListPublicKeys)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/paginators/#listpublickeyspaginator)
     """
 
     def paginate(
         self,
         *,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPublicKeysResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Paginator.ListPublicKeys.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/paginators/#listpublickeyspaginator)
         """
 
@@ -162,16 +162,16 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/paginators/#lookupeventspaginator)
     """
 
     def paginate(
         self,
         *,
         LookupAttributes: Sequence[LookupAttributeTypeDef] = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         EventCategory: Literal["insight"] = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[LookupEventsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Paginator.LookupEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/paginators/#lookupeventspaginator)
         """
```

### Comparing `mypy-boto3-cloudtrail-1.28.15.post1/mypy_boto3_cloudtrail/paginator.pyi` & `mypy-boto3-cloudtrail-1.28.16/mypy_boto3_cloudtrail/paginator.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -26,29 +26,29 @@
     list_public_keys_paginator: ListPublicKeysPaginator = client.get_paginator("list_public_keys")
     list_tags_paginator: ListTagsPaginator = client.get_paginator("list_tags")
     list_trails_paginator: ListTrailsPaginator = client.get_paginator("list_trails")
     lookup_events_paginator: LookupEventsPaginator = client.get_paginator("lookup_events")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Generic, Iterator, Sequence, TypeVar, Union
+from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import ImportStatusType
 from .type_defs import (
     ListImportFailuresResponseTypeDef,
     ListImportsResponseTypeDef,
     ListPublicKeysResponseTypeDef,
     ListTagsResponseTypeDef,
     ListTrailsResponseTypeDef,
     LookupAttributeTypeDef,
     LookupEventsResponseTypeDef,
     PaginatorConfigTypeDef,
+    TimestampTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -106,16 +106,16 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Paginator.ListPublicKeys)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/paginators/#listpublickeyspaginator)
     """
 
     def paginate(
         self,
         *,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPublicKeysResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Paginator.ListPublicKeys.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/paginators/#listpublickeyspaginator)
         """
 
@@ -153,16 +153,16 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/paginators/#lookupeventspaginator)
     """
 
     def paginate(
         self,
         *,
         LookupAttributes: Sequence[LookupAttributeTypeDef] = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         EventCategory: Literal["insight"] = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[LookupEventsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Paginator.LookupEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/paginators/#lookupeventspaginator)
         """
```

### Comparing `mypy-boto3-cloudtrail-1.28.15.post1/mypy_boto3_cloudtrail/type_defs.py` & `mypy-boto3-cloudtrail-1.28.16/mypy_boto3_cloudtrail/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_cloudtrail.type_defs import TagTypeDef
 
-    data: TagTypeDef = {...}
+    data: TagTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -32,15 +32,14 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "TagTypeDef",
     "AdvancedFieldSelectorOutputTypeDef",
     "AdvancedFieldSelectorTypeDef",
     "CancelQueryRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "ChannelTypeDef",
@@ -74,17 +73,16 @@
     "S3ImportSourceTypeDef",
     "ImportsListItemTypeDef",
     "ListChannelsRequestRequestTypeDef",
     "ListEventDataStoresRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "ListImportFailuresRequestRequestTypeDef",
     "ListImportsRequestRequestTypeDef",
-    "ListPublicKeysRequestRequestTypeDef",
+    "TimestampTypeDef",
     "PublicKeyTypeDef",
-    "ListQueriesRequestRequestTypeDef",
     "QueryTypeDef",
     "ListTagsRequestRequestTypeDef",
     "ListTrailsRequestRequestTypeDef",
     "TrailInfoTypeDef",
     "LookupAttributeTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
     "RegisterOrganizationDelegatedAdminRequestRequestTypeDef",
@@ -125,41 +123,45 @@
     "PutInsightSelectorsResponseTypeDef",
     "GetQueryResultsResponseTypeDef",
     "ListImportFailuresResponseTypeDef",
     "ImportSourceTypeDef",
     "ListImportsResponseTypeDef",
     "ListImportFailuresRequestListImportFailuresPaginateTypeDef",
     "ListImportsRequestListImportsPaginateTypeDef",
-    "ListPublicKeysRequestListPublicKeysPaginateTypeDef",
     "ListTagsRequestListTagsPaginateTypeDef",
     "ListTrailsRequestListTrailsPaginateTypeDef",
+    "ListPublicKeysRequestListPublicKeysPaginateTypeDef",
+    "ListPublicKeysRequestRequestTypeDef",
+    "ListQueriesRequestRequestTypeDef",
     "ListPublicKeysResponseTypeDef",
     "ListQueriesResponseTypeDef",
     "ListTrailsResponseTypeDef",
     "LookupEventsRequestLookupEventsPaginateTypeDef",
     "LookupEventsRequestRequestTypeDef",
     "ListTagsResponseTypeDef",
     "CreateEventDataStoreResponseTypeDef",
     "EventDataStoreTypeDef",
     "GetEventDataStoreResponseTypeDef",
     "RestoreEventDataStoreResponseTypeDef",
     "SourceConfigTypeDef",
     "UpdateEventDataStoreResponseTypeDef",
-    "CreateEventDataStoreRequestRequestTypeDef",
-    "UpdateEventDataStoreRequestRequestTypeDef",
+    "AdvancedEventSelectorUnionTypeDef",
     "GetEventSelectorsResponseTypeDef",
     "PutEventSelectorsResponseTypeDef",
-    "PutEventSelectorsRequestRequestTypeDef",
+    "EventSelectorUnionTypeDef",
     "LookupEventsResponseTypeDef",
     "GetImportResponseTypeDef",
     "StartImportRequestRequestTypeDef",
     "StartImportResponseTypeDef",
     "StopImportResponseTypeDef",
     "ListEventDataStoresResponseTypeDef",
     "GetChannelResponseTypeDef",
+    "CreateEventDataStoreRequestRequestTypeDef",
+    "UpdateEventDataStoreRequestRequestTypeDef",
+    "PutEventSelectorsRequestRequestTypeDef",
 )
 
 _RequiredTagTypeDef = TypedDict(
     "_RequiredTagTypeDef",
     {
         "Key": str,
     },
@@ -168,19 +170,17 @@
     "_OptionalTagTypeDef",
     {
         "Value": str,
     },
     total=False,
 )
 
-
 class TagTypeDef(_RequiredTagTypeDef, _OptionalTagTypeDef):
     pass
 
-
 _RequiredAdvancedFieldSelectorOutputTypeDef = TypedDict(
     "_RequiredAdvancedFieldSelectorOutputTypeDef",
     {
         "Field": str,
     },
 )
 _OptionalAdvancedFieldSelectorOutputTypeDef = TypedDict(
@@ -192,21 +192,19 @@
         "NotEquals": List[str],
         "NotStartsWith": List[str],
         "NotEndsWith": List[str],
     },
     total=False,
 )
 
-
 class AdvancedFieldSelectorOutputTypeDef(
     _RequiredAdvancedFieldSelectorOutputTypeDef, _OptionalAdvancedFieldSelectorOutputTypeDef
 ):
     pass
 
-
 _RequiredAdvancedFieldSelectorTypeDef = TypedDict(
     "_RequiredAdvancedFieldSelectorTypeDef",
     {
         "Field": str,
     },
 )
 _OptionalAdvancedFieldSelectorTypeDef = TypedDict(
@@ -218,42 +216,38 @@
         "NotEquals": Sequence[str],
         "NotStartsWith": Sequence[str],
         "NotEndsWith": Sequence[str],
     },
     total=False,
 )
 
-
 class AdvancedFieldSelectorTypeDef(
     _RequiredAdvancedFieldSelectorTypeDef, _OptionalAdvancedFieldSelectorTypeDef
 ):
     pass
 
-
 _RequiredCancelQueryRequestRequestTypeDef = TypedDict(
     "_RequiredCancelQueryRequestRequestTypeDef",
     {
         "QueryId": str,
     },
 )
 _OptionalCancelQueryRequestRequestTypeDef = TypedDict(
     "_OptionalCancelQueryRequestRequestTypeDef",
     {
         "EventDataStore": str,
     },
     total=False,
 )
 
-
 class CancelQueryRequestRequestTypeDef(
     _RequiredCancelQueryRequestRequestTypeDef, _OptionalCancelQueryRequestRequestTypeDef
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
@@ -473,21 +467,19 @@
         "EventDataStore": str,
         "NextToken": str,
         "MaxQueryResults": int,
     },
     total=False,
 )
 
-
 class GetQueryResultsRequestRequestTypeDef(
     _RequiredGetQueryResultsRequestRequestTypeDef, _OptionalGetQueryResultsRequestRequestTypeDef
 ):
     pass
 
-
 QueryStatisticsTypeDef = TypedDict(
     "QueryStatisticsTypeDef",
     {
         "ResultsCount": int,
         "TotalResultsCount": int,
         "BytesScanned": int,
     },
@@ -587,79 +579,43 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListImportFailuresRequestRequestTypeDef(
     _RequiredListImportFailuresRequestRequestTypeDef,
     _OptionalListImportFailuresRequestRequestTypeDef,
 ):
     pass
 
-
 ListImportsRequestRequestTypeDef = TypedDict(
     "ListImportsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "Destination": str,
         "ImportStatus": ImportStatusType,
         "NextToken": str,
     },
     total=False,
 )
 
-ListPublicKeysRequestRequestTypeDef = TypedDict(
-    "ListPublicKeysRequestRequestTypeDef",
-    {
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "NextToken": str,
-    },
-    total=False,
-)
-
+TimestampTypeDef = Union[datetime, str]
 PublicKeyTypeDef = TypedDict(
     "PublicKeyTypeDef",
     {
         "Value": bytes,
         "ValidityStartTime": datetime,
         "ValidityEndTime": datetime,
         "Fingerprint": str,
     },
     total=False,
 )
 
-_RequiredListQueriesRequestRequestTypeDef = TypedDict(
-    "_RequiredListQueriesRequestRequestTypeDef",
-    {
-        "EventDataStore": str,
-    },
-)
-_OptionalListQueriesRequestRequestTypeDef = TypedDict(
-    "_OptionalListQueriesRequestRequestTypeDef",
-    {
-        "NextToken": str,
-        "MaxResults": int,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "QueryStatus": QueryStatusType,
-    },
-    total=False,
-)
-
-
-class ListQueriesRequestRequestTypeDef(
-    _RequiredListQueriesRequestRequestTypeDef, _OptionalListQueriesRequestRequestTypeDef
-):
-    pass
-
-
 QueryTypeDef = TypedDict(
     "QueryTypeDef",
     {
         "QueryId": str,
         "QueryStatus": QueryStatusType,
         "CreationTime": datetime,
     },
@@ -676,21 +632,19 @@
     "_OptionalListTagsRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListTagsRequestRequestTypeDef(
     _RequiredListTagsRequestRequestTypeDef, _OptionalListTagsRequestRequestTypeDef
 ):
     pass
 
-
 ListTrailsRequestRequestTypeDef = TypedDict(
     "ListTrailsRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
@@ -800,21 +754,19 @@
         "CloudWatchLogsRoleArn": str,
         "KmsKeyId": str,
         "IsOrganizationTrail": bool,
     },
     total=False,
 )
 
-
 class UpdateTrailRequestRequestTypeDef(
     _RequiredUpdateTrailRequestRequestTypeDef, _OptionalUpdateTrailRequestRequestTypeDef
 ):
     pass
 
-
 AddTagsRequestRequestTypeDef = TypedDict(
     "AddTagsRequestRequestTypeDef",
     {
         "ResourceId": str,
         "TagsList": Sequence[TagTypeDef],
     },
 )
@@ -839,21 +791,19 @@
         "KmsKeyId": str,
         "IsOrganizationTrail": bool,
         "TagsList": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateTrailRequestRequestTypeDef(
     _RequiredCreateTrailRequestRequestTypeDef, _OptionalCreateTrailRequestRequestTypeDef
 ):
     pass
 
-
 RemoveTagsRequestRequestTypeDef = TypedDict(
     "RemoveTagsRequestRequestTypeDef",
     {
         "ResourceId": str,
         "TagsList": Sequence[TagTypeDef],
     },
 )
@@ -877,42 +827,38 @@
     "_OptionalAdvancedEventSelectorOutputTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
 
-
 class AdvancedEventSelectorOutputTypeDef(
     _RequiredAdvancedEventSelectorOutputTypeDef, _OptionalAdvancedEventSelectorOutputTypeDef
 ):
     pass
 
-
 _RequiredAdvancedEventSelectorTypeDef = TypedDict(
     "_RequiredAdvancedEventSelectorTypeDef",
     {
         "FieldSelectors": Sequence[AdvancedFieldSelectorTypeDef],
     },
 )
 _OptionalAdvancedEventSelectorTypeDef = TypedDict(
     "_OptionalAdvancedEventSelectorTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
 
-
 class AdvancedEventSelectorTypeDef(
     _RequiredAdvancedEventSelectorTypeDef, _OptionalAdvancedEventSelectorTypeDef
 ):
     pass
 
-
 CancelQueryResponseTypeDef = TypedDict(
     "CancelQueryResponseTypeDef",
     {
         "QueryId": str,
         "QueryStatus": QueryStatusType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1029,21 +975,19 @@
     "_OptionalCreateChannelRequestRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateChannelRequestRequestTypeDef(
     _RequiredCreateChannelRequestRequestTypeDef, _OptionalCreateChannelRequestRequestTypeDef
 ):
     pass
 
-
 CreateChannelResponseTypeDef = TypedDict(
     "CreateChannelResponseTypeDef",
     {
         "ChannelArn": str,
         "Name": str,
         "Source": str,
         "Destinations": List[DestinationTypeDef],
@@ -1063,21 +1007,19 @@
     {
         "Destinations": Sequence[DestinationTypeDef],
         "Name": str,
     },
     total=False,
 )
 
-
 class UpdateChannelRequestRequestTypeDef(
     _RequiredUpdateChannelRequestRequestTypeDef, _OptionalUpdateChannelRequestRequestTypeDef
 ):
     pass
 
-
 UpdateChannelResponseTypeDef = TypedDict(
     "UpdateChannelResponseTypeDef",
     {
         "ChannelArn": str,
         "Name": str,
         "Source": str,
         "Destinations": List[DestinationTypeDef],
@@ -1226,71 +1168,100 @@
     "_OptionalListImportFailuresRequestListImportFailuresPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListImportFailuresRequestListImportFailuresPaginateTypeDef(
     _RequiredListImportFailuresRequestListImportFailuresPaginateTypeDef,
     _OptionalListImportFailuresRequestListImportFailuresPaginateTypeDef,
 ):
     pass
 
-
 ListImportsRequestListImportsPaginateTypeDef = TypedDict(
     "ListImportsRequestListImportsPaginateTypeDef",
     {
         "Destination": str,
         "ImportStatus": ImportStatusType,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListPublicKeysRequestListPublicKeysPaginateTypeDef = TypedDict(
-    "ListPublicKeysRequestListPublicKeysPaginateTypeDef",
-    {
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 _RequiredListTagsRequestListTagsPaginateTypeDef = TypedDict(
     "_RequiredListTagsRequestListTagsPaginateTypeDef",
     {
         "ResourceIdList": Sequence[str],
     },
 )
 _OptionalListTagsRequestListTagsPaginateTypeDef = TypedDict(
     "_OptionalListTagsRequestListTagsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListTagsRequestListTagsPaginateTypeDef(
     _RequiredListTagsRequestListTagsPaginateTypeDef, _OptionalListTagsRequestListTagsPaginateTypeDef
 ):
     pass
 
-
 ListTrailsRequestListTrailsPaginateTypeDef = TypedDict(
     "ListTrailsRequestListTrailsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+ListPublicKeysRequestListPublicKeysPaginateTypeDef = TypedDict(
+    "ListPublicKeysRequestListPublicKeysPaginateTypeDef",
+    {
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListPublicKeysRequestRequestTypeDef = TypedDict(
+    "ListPublicKeysRequestRequestTypeDef",
+    {
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "NextToken": str,
+    },
+    total=False,
+)
+
+_RequiredListQueriesRequestRequestTypeDef = TypedDict(
+    "_RequiredListQueriesRequestRequestTypeDef",
+    {
+        "EventDataStore": str,
+    },
+)
+_OptionalListQueriesRequestRequestTypeDef = TypedDict(
+    "_OptionalListQueriesRequestRequestTypeDef",
+    {
+        "NextToken": str,
+        "MaxResults": int,
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "QueryStatus": QueryStatusType,
+    },
+    total=False,
+)
+
+class ListQueriesRequestRequestTypeDef(
+    _RequiredListQueriesRequestRequestTypeDef, _OptionalListQueriesRequestRequestTypeDef
+):
+    pass
+
 ListPublicKeysResponseTypeDef = TypedDict(
     "ListPublicKeysResponseTypeDef",
     {
         "PublicKeyList": List[PublicKeyTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1314,28 +1285,28 @@
     },
 )
 
 LookupEventsRequestLookupEventsPaginateTypeDef = TypedDict(
     "LookupEventsRequestLookupEventsPaginateTypeDef",
     {
         "LookupAttributes": Sequence[LookupAttributeTypeDef],
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
         "EventCategory": Literal["insight"],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 LookupEventsRequestRequestTypeDef = TypedDict(
     "LookupEventsRequestRequestTypeDef",
     {
         "LookupAttributes": Sequence[LookupAttributeTypeDef],
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
         "EventCategory": Literal["insight"],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
@@ -1443,75 +1414,17 @@
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
         "KmsKeyId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateEventDataStoreRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateEventDataStoreRequestRequestTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalCreateEventDataStoreRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateEventDataStoreRequestRequestTypeDef",
-    {
-        "AdvancedEventSelectors": Sequence[
-            Union[AdvancedEventSelectorTypeDef, AdvancedEventSelectorOutputTypeDef]
-        ],
-        "MultiRegionEnabled": bool,
-        "OrganizationEnabled": bool,
-        "RetentionPeriod": int,
-        "TerminationProtectionEnabled": bool,
-        "TagsList": Sequence[TagTypeDef],
-        "KmsKeyId": str,
-        "StartIngestion": bool,
-    },
-    total=False,
-)
-
-
-class CreateEventDataStoreRequestRequestTypeDef(
-    _RequiredCreateEventDataStoreRequestRequestTypeDef,
-    _OptionalCreateEventDataStoreRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredUpdateEventDataStoreRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateEventDataStoreRequestRequestTypeDef",
-    {
-        "EventDataStore": str,
-    },
-)
-_OptionalUpdateEventDataStoreRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateEventDataStoreRequestRequestTypeDef",
-    {
-        "Name": str,
-        "AdvancedEventSelectors": Sequence[
-            Union[AdvancedEventSelectorTypeDef, AdvancedEventSelectorOutputTypeDef]
-        ],
-        "MultiRegionEnabled": bool,
-        "OrganizationEnabled": bool,
-        "RetentionPeriod": int,
-        "TerminationProtectionEnabled": bool,
-        "KmsKeyId": str,
-    },
-    total=False,
-)
-
-
-class UpdateEventDataStoreRequestRequestTypeDef(
-    _RequiredUpdateEventDataStoreRequestRequestTypeDef,
-    _OptionalUpdateEventDataStoreRequestRequestTypeDef,
-):
-    pass
-
-
+AdvancedEventSelectorUnionTypeDef = Union[
+    AdvancedEventSelectorTypeDef, AdvancedEventSelectorOutputTypeDef
+]
 GetEventSelectorsResponseTypeDef = TypedDict(
     "GetEventSelectorsResponseTypeDef",
     {
         "TrailARN": str,
         "EventSelectors": List[EventSelectorOutputTypeDef],
         "AdvancedEventSelectors": List[AdvancedEventSelectorOutputTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1524,38 +1437,15 @@
         "TrailARN": str,
         "EventSelectors": List[EventSelectorOutputTypeDef],
         "AdvancedEventSelectors": List[AdvancedEventSelectorOutputTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredPutEventSelectorsRequestRequestTypeDef = TypedDict(
-    "_RequiredPutEventSelectorsRequestRequestTypeDef",
-    {
-        "TrailName": str,
-    },
-)
-_OptionalPutEventSelectorsRequestRequestTypeDef = TypedDict(
-    "_OptionalPutEventSelectorsRequestRequestTypeDef",
-    {
-        "EventSelectors": Sequence[Union[EventSelectorTypeDef, EventSelectorOutputTypeDef]],
-        "AdvancedEventSelectors": Sequence[
-            Union[AdvancedEventSelectorTypeDef, AdvancedEventSelectorOutputTypeDef]
-        ],
-    },
-    total=False,
-)
-
-
-class PutEventSelectorsRequestRequestTypeDef(
-    _RequiredPutEventSelectorsRequestRequestTypeDef, _OptionalPutEventSelectorsRequestRequestTypeDef
-):
-    pass
-
-
+EventSelectorUnionTypeDef = Union[EventSelectorTypeDef, EventSelectorOutputTypeDef]
 LookupEventsResponseTypeDef = TypedDict(
     "LookupEventsResponseTypeDef",
     {
         "Events": List[EventTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1578,16 +1468,16 @@
 )
 
 StartImportRequestRequestTypeDef = TypedDict(
     "StartImportRequestRequestTypeDef",
     {
         "Destinations": Sequence[str],
         "ImportSource": ImportSourceTypeDef,
-        "StartEventTime": Union[datetime, str],
-        "EndEventTime": Union[datetime, str],
+        "StartEventTime": TimestampTypeDef,
+        "EndEventTime": TimestampTypeDef,
         "ImportId": str,
     },
     total=False,
 )
 
 StartImportResponseTypeDef = TypedDict(
     "StartImportResponseTypeDef",
@@ -1637,7 +1527,80 @@
         "Source": str,
         "SourceConfig": SourceConfigTypeDef,
         "Destinations": List[DestinationTypeDef],
         "IngestionStatus": IngestionStatusTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+
+_RequiredCreateEventDataStoreRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateEventDataStoreRequestRequestTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalCreateEventDataStoreRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateEventDataStoreRequestRequestTypeDef",
+    {
+        "AdvancedEventSelectors": Sequence[AdvancedEventSelectorUnionTypeDef],
+        "MultiRegionEnabled": bool,
+        "OrganizationEnabled": bool,
+        "RetentionPeriod": int,
+        "TerminationProtectionEnabled": bool,
+        "TagsList": Sequence[TagTypeDef],
+        "KmsKeyId": str,
+        "StartIngestion": bool,
+    },
+    total=False,
+)
+
+class CreateEventDataStoreRequestRequestTypeDef(
+    _RequiredCreateEventDataStoreRequestRequestTypeDef,
+    _OptionalCreateEventDataStoreRequestRequestTypeDef,
+):
+    pass
+
+_RequiredUpdateEventDataStoreRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateEventDataStoreRequestRequestTypeDef",
+    {
+        "EventDataStore": str,
+    },
+)
+_OptionalUpdateEventDataStoreRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateEventDataStoreRequestRequestTypeDef",
+    {
+        "Name": str,
+        "AdvancedEventSelectors": Sequence[AdvancedEventSelectorUnionTypeDef],
+        "MultiRegionEnabled": bool,
+        "OrganizationEnabled": bool,
+        "RetentionPeriod": int,
+        "TerminationProtectionEnabled": bool,
+        "KmsKeyId": str,
+    },
+    total=False,
+)
+
+class UpdateEventDataStoreRequestRequestTypeDef(
+    _RequiredUpdateEventDataStoreRequestRequestTypeDef,
+    _OptionalUpdateEventDataStoreRequestRequestTypeDef,
+):
+    pass
+
+_RequiredPutEventSelectorsRequestRequestTypeDef = TypedDict(
+    "_RequiredPutEventSelectorsRequestRequestTypeDef",
+    {
+        "TrailName": str,
+    },
+)
+_OptionalPutEventSelectorsRequestRequestTypeDef = TypedDict(
+    "_OptionalPutEventSelectorsRequestRequestTypeDef",
+    {
+        "EventSelectors": Sequence[EventSelectorUnionTypeDef],
+        "AdvancedEventSelectors": Sequence[AdvancedEventSelectorUnionTypeDef],
+    },
+    total=False,
+)
+
+class PutEventSelectorsRequestRequestTypeDef(
+    _RequiredPutEventSelectorsRequestRequestTypeDef, _OptionalPutEventSelectorsRequestRequestTypeDef
+):
+    pass
```

### Comparing `mypy-boto3-cloudtrail-1.28.15.post1/mypy_boto3_cloudtrail/type_defs.pyi` & `mypy-boto3-cloudtrail-1.28.16/mypy_boto3_cloudtrail/type_defs.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_cloudtrail.type_defs import TagTypeDef
 
-    data: TagTypeDef = {...}
+    data: TagTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -32,14 +32,15 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "TagTypeDef",
     "AdvancedFieldSelectorOutputTypeDef",
     "AdvancedFieldSelectorTypeDef",
     "CancelQueryRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "ChannelTypeDef",
@@ -73,17 +74,16 @@
     "S3ImportSourceTypeDef",
     "ImportsListItemTypeDef",
     "ListChannelsRequestRequestTypeDef",
     "ListEventDataStoresRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "ListImportFailuresRequestRequestTypeDef",
     "ListImportsRequestRequestTypeDef",
-    "ListPublicKeysRequestRequestTypeDef",
+    "TimestampTypeDef",
     "PublicKeyTypeDef",
-    "ListQueriesRequestRequestTypeDef",
     "QueryTypeDef",
     "ListTagsRequestRequestTypeDef",
     "ListTrailsRequestRequestTypeDef",
     "TrailInfoTypeDef",
     "LookupAttributeTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
     "RegisterOrganizationDelegatedAdminRequestRequestTypeDef",
@@ -124,41 +124,45 @@
     "PutInsightSelectorsResponseTypeDef",
     "GetQueryResultsResponseTypeDef",
     "ListImportFailuresResponseTypeDef",
     "ImportSourceTypeDef",
     "ListImportsResponseTypeDef",
     "ListImportFailuresRequestListImportFailuresPaginateTypeDef",
     "ListImportsRequestListImportsPaginateTypeDef",
-    "ListPublicKeysRequestListPublicKeysPaginateTypeDef",
     "ListTagsRequestListTagsPaginateTypeDef",
     "ListTrailsRequestListTrailsPaginateTypeDef",
+    "ListPublicKeysRequestListPublicKeysPaginateTypeDef",
+    "ListPublicKeysRequestRequestTypeDef",
+    "ListQueriesRequestRequestTypeDef",
     "ListPublicKeysResponseTypeDef",
     "ListQueriesResponseTypeDef",
     "ListTrailsResponseTypeDef",
     "LookupEventsRequestLookupEventsPaginateTypeDef",
     "LookupEventsRequestRequestTypeDef",
     "ListTagsResponseTypeDef",
     "CreateEventDataStoreResponseTypeDef",
     "EventDataStoreTypeDef",
     "GetEventDataStoreResponseTypeDef",
     "RestoreEventDataStoreResponseTypeDef",
     "SourceConfigTypeDef",
     "UpdateEventDataStoreResponseTypeDef",
-    "CreateEventDataStoreRequestRequestTypeDef",
-    "UpdateEventDataStoreRequestRequestTypeDef",
+    "AdvancedEventSelectorUnionTypeDef",
     "GetEventSelectorsResponseTypeDef",
     "PutEventSelectorsResponseTypeDef",
-    "PutEventSelectorsRequestRequestTypeDef",
+    "EventSelectorUnionTypeDef",
     "LookupEventsResponseTypeDef",
     "GetImportResponseTypeDef",
     "StartImportRequestRequestTypeDef",
     "StartImportResponseTypeDef",
     "StopImportResponseTypeDef",
     "ListEventDataStoresResponseTypeDef",
     "GetChannelResponseTypeDef",
+    "CreateEventDataStoreRequestRequestTypeDef",
+    "UpdateEventDataStoreRequestRequestTypeDef",
+    "PutEventSelectorsRequestRequestTypeDef",
 )
 
 _RequiredTagTypeDef = TypedDict(
     "_RequiredTagTypeDef",
     {
         "Key": str,
     },
@@ -167,17 +171,19 @@
     "_OptionalTagTypeDef",
     {
         "Value": str,
     },
     total=False,
 )
 
+
 class TagTypeDef(_RequiredTagTypeDef, _OptionalTagTypeDef):
     pass
 
+
 _RequiredAdvancedFieldSelectorOutputTypeDef = TypedDict(
     "_RequiredAdvancedFieldSelectorOutputTypeDef",
     {
         "Field": str,
     },
 )
 _OptionalAdvancedFieldSelectorOutputTypeDef = TypedDict(
@@ -189,19 +195,21 @@
         "NotEquals": List[str],
         "NotStartsWith": List[str],
         "NotEndsWith": List[str],
     },
     total=False,
 )
 
+
 class AdvancedFieldSelectorOutputTypeDef(
     _RequiredAdvancedFieldSelectorOutputTypeDef, _OptionalAdvancedFieldSelectorOutputTypeDef
 ):
     pass
 
+
 _RequiredAdvancedFieldSelectorTypeDef = TypedDict(
     "_RequiredAdvancedFieldSelectorTypeDef",
     {
         "Field": str,
     },
 )
 _OptionalAdvancedFieldSelectorTypeDef = TypedDict(
@@ -213,38 +221,42 @@
         "NotEquals": Sequence[str],
         "NotStartsWith": Sequence[str],
         "NotEndsWith": Sequence[str],
     },
     total=False,
 )
 
+
 class AdvancedFieldSelectorTypeDef(
     _RequiredAdvancedFieldSelectorTypeDef, _OptionalAdvancedFieldSelectorTypeDef
 ):
     pass
 
+
 _RequiredCancelQueryRequestRequestTypeDef = TypedDict(
     "_RequiredCancelQueryRequestRequestTypeDef",
     {
         "QueryId": str,
     },
 )
 _OptionalCancelQueryRequestRequestTypeDef = TypedDict(
     "_OptionalCancelQueryRequestRequestTypeDef",
     {
         "EventDataStore": str,
     },
     total=False,
 )
 
+
 class CancelQueryRequestRequestTypeDef(
     _RequiredCancelQueryRequestRequestTypeDef, _OptionalCancelQueryRequestRequestTypeDef
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
@@ -464,19 +476,21 @@
         "EventDataStore": str,
         "NextToken": str,
         "MaxQueryResults": int,
     },
     total=False,
 )
 
+
 class GetQueryResultsRequestRequestTypeDef(
     _RequiredGetQueryResultsRequestRequestTypeDef, _OptionalGetQueryResultsRequestRequestTypeDef
 ):
     pass
 
+
 QueryStatisticsTypeDef = TypedDict(
     "QueryStatisticsTypeDef",
     {
         "ResultsCount": int,
         "TotalResultsCount": int,
         "BytesScanned": int,
     },
@@ -576,75 +590,45 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListImportFailuresRequestRequestTypeDef(
     _RequiredListImportFailuresRequestRequestTypeDef,
     _OptionalListImportFailuresRequestRequestTypeDef,
 ):
     pass
 
+
 ListImportsRequestRequestTypeDef = TypedDict(
     "ListImportsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "Destination": str,
         "ImportStatus": ImportStatusType,
         "NextToken": str,
     },
     total=False,
 )
 
-ListPublicKeysRequestRequestTypeDef = TypedDict(
-    "ListPublicKeysRequestRequestTypeDef",
-    {
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "NextToken": str,
-    },
-    total=False,
-)
-
+TimestampTypeDef = Union[datetime, str]
 PublicKeyTypeDef = TypedDict(
     "PublicKeyTypeDef",
     {
         "Value": bytes,
         "ValidityStartTime": datetime,
         "ValidityEndTime": datetime,
         "Fingerprint": str,
     },
     total=False,
 )
 
-_RequiredListQueriesRequestRequestTypeDef = TypedDict(
-    "_RequiredListQueriesRequestRequestTypeDef",
-    {
-        "EventDataStore": str,
-    },
-)
-_OptionalListQueriesRequestRequestTypeDef = TypedDict(
-    "_OptionalListQueriesRequestRequestTypeDef",
-    {
-        "NextToken": str,
-        "MaxResults": int,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "QueryStatus": QueryStatusType,
-    },
-    total=False,
-)
-
-class ListQueriesRequestRequestTypeDef(
-    _RequiredListQueriesRequestRequestTypeDef, _OptionalListQueriesRequestRequestTypeDef
-):
-    pass
-
 QueryTypeDef = TypedDict(
     "QueryTypeDef",
     {
         "QueryId": str,
         "QueryStatus": QueryStatusType,
         "CreationTime": datetime,
     },
@@ -661,19 +645,21 @@
     "_OptionalListTagsRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListTagsRequestRequestTypeDef(
     _RequiredListTagsRequestRequestTypeDef, _OptionalListTagsRequestRequestTypeDef
 ):
     pass
 
+
 ListTrailsRequestRequestTypeDef = TypedDict(
     "ListTrailsRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
@@ -783,19 +769,21 @@
         "CloudWatchLogsRoleArn": str,
         "KmsKeyId": str,
         "IsOrganizationTrail": bool,
     },
     total=False,
 )
 
+
 class UpdateTrailRequestRequestTypeDef(
     _RequiredUpdateTrailRequestRequestTypeDef, _OptionalUpdateTrailRequestRequestTypeDef
 ):
     pass
 
+
 AddTagsRequestRequestTypeDef = TypedDict(
     "AddTagsRequestRequestTypeDef",
     {
         "ResourceId": str,
         "TagsList": Sequence[TagTypeDef],
     },
 )
@@ -820,19 +808,21 @@
         "KmsKeyId": str,
         "IsOrganizationTrail": bool,
         "TagsList": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateTrailRequestRequestTypeDef(
     _RequiredCreateTrailRequestRequestTypeDef, _OptionalCreateTrailRequestRequestTypeDef
 ):
     pass
 
+
 RemoveTagsRequestRequestTypeDef = TypedDict(
     "RemoveTagsRequestRequestTypeDef",
     {
         "ResourceId": str,
         "TagsList": Sequence[TagTypeDef],
     },
 )
@@ -856,38 +846,42 @@
     "_OptionalAdvancedEventSelectorOutputTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
 
+
 class AdvancedEventSelectorOutputTypeDef(
     _RequiredAdvancedEventSelectorOutputTypeDef, _OptionalAdvancedEventSelectorOutputTypeDef
 ):
     pass
 
+
 _RequiredAdvancedEventSelectorTypeDef = TypedDict(
     "_RequiredAdvancedEventSelectorTypeDef",
     {
         "FieldSelectors": Sequence[AdvancedFieldSelectorTypeDef],
     },
 )
 _OptionalAdvancedEventSelectorTypeDef = TypedDict(
     "_OptionalAdvancedEventSelectorTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
 
+
 class AdvancedEventSelectorTypeDef(
     _RequiredAdvancedEventSelectorTypeDef, _OptionalAdvancedEventSelectorTypeDef
 ):
     pass
 
+
 CancelQueryResponseTypeDef = TypedDict(
     "CancelQueryResponseTypeDef",
     {
         "QueryId": str,
         "QueryStatus": QueryStatusType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1004,19 +998,21 @@
     "_OptionalCreateChannelRequestRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateChannelRequestRequestTypeDef(
     _RequiredCreateChannelRequestRequestTypeDef, _OptionalCreateChannelRequestRequestTypeDef
 ):
     pass
 
+
 CreateChannelResponseTypeDef = TypedDict(
     "CreateChannelResponseTypeDef",
     {
         "ChannelArn": str,
         "Name": str,
         "Source": str,
         "Destinations": List[DestinationTypeDef],
@@ -1036,19 +1032,21 @@
     {
         "Destinations": Sequence[DestinationTypeDef],
         "Name": str,
     },
     total=False,
 )
 
+
 class UpdateChannelRequestRequestTypeDef(
     _RequiredUpdateChannelRequestRequestTypeDef, _OptionalUpdateChannelRequestRequestTypeDef
 ):
     pass
 
+
 UpdateChannelResponseTypeDef = TypedDict(
     "UpdateChannelResponseTypeDef",
     {
         "ChannelArn": str,
         "Name": str,
         "Source": str,
         "Destinations": List[DestinationTypeDef],
@@ -1197,67 +1195,106 @@
     "_OptionalListImportFailuresRequestListImportFailuresPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListImportFailuresRequestListImportFailuresPaginateTypeDef(
     _RequiredListImportFailuresRequestListImportFailuresPaginateTypeDef,
     _OptionalListImportFailuresRequestListImportFailuresPaginateTypeDef,
 ):
     pass
 
+
 ListImportsRequestListImportsPaginateTypeDef = TypedDict(
     "ListImportsRequestListImportsPaginateTypeDef",
     {
         "Destination": str,
         "ImportStatus": ImportStatusType,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListPublicKeysRequestListPublicKeysPaginateTypeDef = TypedDict(
-    "ListPublicKeysRequestListPublicKeysPaginateTypeDef",
-    {
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 _RequiredListTagsRequestListTagsPaginateTypeDef = TypedDict(
     "_RequiredListTagsRequestListTagsPaginateTypeDef",
     {
         "ResourceIdList": Sequence[str],
     },
 )
 _OptionalListTagsRequestListTagsPaginateTypeDef = TypedDict(
     "_OptionalListTagsRequestListTagsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListTagsRequestListTagsPaginateTypeDef(
     _RequiredListTagsRequestListTagsPaginateTypeDef, _OptionalListTagsRequestListTagsPaginateTypeDef
 ):
     pass
 
+
 ListTrailsRequestListTrailsPaginateTypeDef = TypedDict(
     "ListTrailsRequestListTrailsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+ListPublicKeysRequestListPublicKeysPaginateTypeDef = TypedDict(
+    "ListPublicKeysRequestListPublicKeysPaginateTypeDef",
+    {
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListPublicKeysRequestRequestTypeDef = TypedDict(
+    "ListPublicKeysRequestRequestTypeDef",
+    {
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "NextToken": str,
+    },
+    total=False,
+)
+
+_RequiredListQueriesRequestRequestTypeDef = TypedDict(
+    "_RequiredListQueriesRequestRequestTypeDef",
+    {
+        "EventDataStore": str,
+    },
+)
+_OptionalListQueriesRequestRequestTypeDef = TypedDict(
+    "_OptionalListQueriesRequestRequestTypeDef",
+    {
+        "NextToken": str,
+        "MaxResults": int,
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "QueryStatus": QueryStatusType,
+    },
+    total=False,
+)
+
+
+class ListQueriesRequestRequestTypeDef(
+    _RequiredListQueriesRequestRequestTypeDef, _OptionalListQueriesRequestRequestTypeDef
+):
+    pass
+
+
 ListPublicKeysResponseTypeDef = TypedDict(
     "ListPublicKeysResponseTypeDef",
     {
         "PublicKeyList": List[PublicKeyTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1281,28 +1318,28 @@
     },
 )
 
 LookupEventsRequestLookupEventsPaginateTypeDef = TypedDict(
     "LookupEventsRequestLookupEventsPaginateTypeDef",
     {
         "LookupAttributes": Sequence[LookupAttributeTypeDef],
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
         "EventCategory": Literal["insight"],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 LookupEventsRequestRequestTypeDef = TypedDict(
     "LookupEventsRequestRequestTypeDef",
     {
         "LookupAttributes": Sequence[LookupAttributeTypeDef],
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
         "EventCategory": Literal["insight"],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
@@ -1410,71 +1447,17 @@
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
         "KmsKeyId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateEventDataStoreRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateEventDataStoreRequestRequestTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalCreateEventDataStoreRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateEventDataStoreRequestRequestTypeDef",
-    {
-        "AdvancedEventSelectors": Sequence[
-            Union[AdvancedEventSelectorTypeDef, AdvancedEventSelectorOutputTypeDef]
-        ],
-        "MultiRegionEnabled": bool,
-        "OrganizationEnabled": bool,
-        "RetentionPeriod": int,
-        "TerminationProtectionEnabled": bool,
-        "TagsList": Sequence[TagTypeDef],
-        "KmsKeyId": str,
-        "StartIngestion": bool,
-    },
-    total=False,
-)
-
-class CreateEventDataStoreRequestRequestTypeDef(
-    _RequiredCreateEventDataStoreRequestRequestTypeDef,
-    _OptionalCreateEventDataStoreRequestRequestTypeDef,
-):
-    pass
-
-_RequiredUpdateEventDataStoreRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateEventDataStoreRequestRequestTypeDef",
-    {
-        "EventDataStore": str,
-    },
-)
-_OptionalUpdateEventDataStoreRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateEventDataStoreRequestRequestTypeDef",
-    {
-        "Name": str,
-        "AdvancedEventSelectors": Sequence[
-            Union[AdvancedEventSelectorTypeDef, AdvancedEventSelectorOutputTypeDef]
-        ],
-        "MultiRegionEnabled": bool,
-        "OrganizationEnabled": bool,
-        "RetentionPeriod": int,
-        "TerminationProtectionEnabled": bool,
-        "KmsKeyId": str,
-    },
-    total=False,
-)
-
-class UpdateEventDataStoreRequestRequestTypeDef(
-    _RequiredUpdateEventDataStoreRequestRequestTypeDef,
-    _OptionalUpdateEventDataStoreRequestRequestTypeDef,
-):
-    pass
-
+AdvancedEventSelectorUnionTypeDef = Union[
+    AdvancedEventSelectorTypeDef, AdvancedEventSelectorOutputTypeDef
+]
 GetEventSelectorsResponseTypeDef = TypedDict(
     "GetEventSelectorsResponseTypeDef",
     {
         "TrailARN": str,
         "EventSelectors": List[EventSelectorOutputTypeDef],
         "AdvancedEventSelectors": List[AdvancedEventSelectorOutputTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1487,36 +1470,15 @@
         "TrailARN": str,
         "EventSelectors": List[EventSelectorOutputTypeDef],
         "AdvancedEventSelectors": List[AdvancedEventSelectorOutputTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredPutEventSelectorsRequestRequestTypeDef = TypedDict(
-    "_RequiredPutEventSelectorsRequestRequestTypeDef",
-    {
-        "TrailName": str,
-    },
-)
-_OptionalPutEventSelectorsRequestRequestTypeDef = TypedDict(
-    "_OptionalPutEventSelectorsRequestRequestTypeDef",
-    {
-        "EventSelectors": Sequence[Union[EventSelectorTypeDef, EventSelectorOutputTypeDef]],
-        "AdvancedEventSelectors": Sequence[
-            Union[AdvancedEventSelectorTypeDef, AdvancedEventSelectorOutputTypeDef]
-        ],
-    },
-    total=False,
-)
-
-class PutEventSelectorsRequestRequestTypeDef(
-    _RequiredPutEventSelectorsRequestRequestTypeDef, _OptionalPutEventSelectorsRequestRequestTypeDef
-):
-    pass
-
+EventSelectorUnionTypeDef = Union[EventSelectorTypeDef, EventSelectorOutputTypeDef]
 LookupEventsResponseTypeDef = TypedDict(
     "LookupEventsResponseTypeDef",
     {
         "Events": List[EventTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1539,16 +1501,16 @@
 )
 
 StartImportRequestRequestTypeDef = TypedDict(
     "StartImportRequestRequestTypeDef",
     {
         "Destinations": Sequence[str],
         "ImportSource": ImportSourceTypeDef,
-        "StartEventTime": Union[datetime, str],
-        "EndEventTime": Union[datetime, str],
+        "StartEventTime": TimestampTypeDef,
+        "EndEventTime": TimestampTypeDef,
         "ImportId": str,
     },
     total=False,
 )
 
 StartImportResponseTypeDef = TypedDict(
     "StartImportResponseTypeDef",
@@ -1598,7 +1560,85 @@
         "Source": str,
         "SourceConfig": SourceConfigTypeDef,
         "Destinations": List[DestinationTypeDef],
         "IngestionStatus": IngestionStatusTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+
+_RequiredCreateEventDataStoreRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateEventDataStoreRequestRequestTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalCreateEventDataStoreRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateEventDataStoreRequestRequestTypeDef",
+    {
+        "AdvancedEventSelectors": Sequence[AdvancedEventSelectorUnionTypeDef],
+        "MultiRegionEnabled": bool,
+        "OrganizationEnabled": bool,
+        "RetentionPeriod": int,
+        "TerminationProtectionEnabled": bool,
+        "TagsList": Sequence[TagTypeDef],
+        "KmsKeyId": str,
+        "StartIngestion": bool,
+    },
+    total=False,
+)
+
+
+class CreateEventDataStoreRequestRequestTypeDef(
+    _RequiredCreateEventDataStoreRequestRequestTypeDef,
+    _OptionalCreateEventDataStoreRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredUpdateEventDataStoreRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateEventDataStoreRequestRequestTypeDef",
+    {
+        "EventDataStore": str,
+    },
+)
+_OptionalUpdateEventDataStoreRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateEventDataStoreRequestRequestTypeDef",
+    {
+        "Name": str,
+        "AdvancedEventSelectors": Sequence[AdvancedEventSelectorUnionTypeDef],
+        "MultiRegionEnabled": bool,
+        "OrganizationEnabled": bool,
+        "RetentionPeriod": int,
+        "TerminationProtectionEnabled": bool,
+        "KmsKeyId": str,
+    },
+    total=False,
+)
+
+
+class UpdateEventDataStoreRequestRequestTypeDef(
+    _RequiredUpdateEventDataStoreRequestRequestTypeDef,
+    _OptionalUpdateEventDataStoreRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredPutEventSelectorsRequestRequestTypeDef = TypedDict(
+    "_RequiredPutEventSelectorsRequestRequestTypeDef",
+    {
+        "TrailName": str,
+    },
+)
+_OptionalPutEventSelectorsRequestRequestTypeDef = TypedDict(
+    "_OptionalPutEventSelectorsRequestRequestTypeDef",
+    {
+        "EventSelectors": Sequence[EventSelectorUnionTypeDef],
+        "AdvancedEventSelectors": Sequence[AdvancedEventSelectorUnionTypeDef],
+    },
+    total=False,
+)
+
+
+class PutEventSelectorsRequestRequestTypeDef(
+    _RequiredPutEventSelectorsRequestRequestTypeDef, _OptionalPutEventSelectorsRequestRequestTypeDef
+):
+    pass
```

### Comparing `mypy-boto3-cloudtrail-1.28.15.post1/mypy_boto3_cloudtrail.egg-info/PKG-INFO` & `mypy-boto3-cloudtrail-1.28.16/mypy_boto3_cloudtrail.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cloudtrail
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.CloudTrail 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.CloudTrail 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 cloudtrail type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 cloudtrail type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudtrail.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudtrail)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cloudtrail)](https://pepy.tech/project/mypy-boto3-cloudtrail)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudTrail 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail)
+[boto3.CloudTrail 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail)
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
 [mypy-boto3-cloudtrail docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/).
 
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
@@ -338,20 +338,20 @@
 )
 
 
 def check_value(value: DeliveryStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_cloudtrail.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_cloudtrail.type_defs import (
     TagTypeDef,
     AdvancedFieldSelectorOutputTypeDef,
     AdvancedFieldSelectorTypeDef,
     CancelQueryRequestRequestTypeDef,
@@ -387,17 +387,16 @@
     S3ImportSourceTypeDef,
     ImportsListItemTypeDef,
     ListChannelsRequestRequestTypeDef,
     ListEventDataStoresRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     ListImportFailuresRequestRequestTypeDef,
     ListImportsRequestRequestTypeDef,
-    ListPublicKeysRequestRequestTypeDef,
+    TimestampTypeDef,
     PublicKeyTypeDef,
-    ListQueriesRequestRequestTypeDef,
     QueryTypeDef,
     ListTagsRequestRequestTypeDef,
     ListTrailsRequestRequestTypeDef,
     TrailInfoTypeDef,
     LookupAttributeTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
     RegisterOrganizationDelegatedAdminRequestRequestTypeDef,
@@ -438,45 +437,49 @@
     PutInsightSelectorsResponseTypeDef,
     GetQueryResultsResponseTypeDef,
     ListImportFailuresResponseTypeDef,
     ImportSourceTypeDef,
     ListImportsResponseTypeDef,
     ListImportFailuresRequestListImportFailuresPaginateTypeDef,
     ListImportsRequestListImportsPaginateTypeDef,
-    ListPublicKeysRequestListPublicKeysPaginateTypeDef,
     ListTagsRequestListTagsPaginateTypeDef,
     ListTrailsRequestListTrailsPaginateTypeDef,
+    ListPublicKeysRequestListPublicKeysPaginateTypeDef,
+    ListPublicKeysRequestRequestTypeDef,
+    ListQueriesRequestRequestTypeDef,
     ListPublicKeysResponseTypeDef,
     ListQueriesResponseTypeDef,
     ListTrailsResponseTypeDef,
     LookupEventsRequestLookupEventsPaginateTypeDef,
     LookupEventsRequestRequestTypeDef,
     ListTagsResponseTypeDef,
     CreateEventDataStoreResponseTypeDef,
     EventDataStoreTypeDef,
     GetEventDataStoreResponseTypeDef,
     RestoreEventDataStoreResponseTypeDef,
     SourceConfigTypeDef,
     UpdateEventDataStoreResponseTypeDef,
-    CreateEventDataStoreRequestRequestTypeDef,
-    UpdateEventDataStoreRequestRequestTypeDef,
+    AdvancedEventSelectorUnionTypeDef,
     GetEventSelectorsResponseTypeDef,
     PutEventSelectorsResponseTypeDef,
-    PutEventSelectorsRequestRequestTypeDef,
+    EventSelectorUnionTypeDef,
     LookupEventsResponseTypeDef,
     GetImportResponseTypeDef,
     StartImportRequestRequestTypeDef,
     StartImportResponseTypeDef,
     StopImportResponseTypeDef,
     ListEventDataStoresResponseTypeDef,
     GetChannelResponseTypeDef,
+    CreateEventDataStoreRequestRequestTypeDef,
+    UpdateEventDataStoreRequestRequestTypeDef,
+    PutEventSelectorsRequestRequestTypeDef,
 )
 
 
-def get_structure() -> TagTypeDef:
+def get_value() -> TagTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-cloudtrail-1.28.15.post1/mypy_boto3_cloudtrail.egg-info/SOURCES.txt` & `mypy-boto3-cloudtrail-1.28.16/mypy_boto3_cloudtrail.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudtrail-1.28.15.post1/setup.py` & `mypy-boto3-cloudtrail-1.28.16/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-cloudtrail",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_cloudtrail"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CloudTrail 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.2"
+        "Type annotations for boto3.CloudTrail 1.28.16 service generated with mypy-boto3-builder"
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
-    keywords="boto3 cloudtrail type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 cloudtrail type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_cloudtrail": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

