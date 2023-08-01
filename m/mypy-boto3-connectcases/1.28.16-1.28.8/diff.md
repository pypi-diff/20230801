# Comparing `tmp/mypy-boto3-connectcases-1.28.16.tar.gz` & `tmp/mypy-boto3-connectcases-1.28.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-connectcases-1.28.16.tar", last modified: Tue Aug  1 11:36:32 2023, max compression
+gzip compressed data, was "mypy-boto3-connectcases-1.28.8.tar", last modified: Thu Jul 20 19:47:56 2023, max compression
```

## Comparing `mypy-boto3-connectcases-1.28.16.tar` & `mypy-boto3-connectcases-1.28.8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:32.416918 mypy-boto3-connectcases-1.28.16/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:14:17.000000 mypy-boto3-connectcases-1.28.16/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16641 2023-08-01 11:36:32.416918 mypy-boto3-connectcases-1.28.16/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15137 2023-08-01 11:14:17.000000 mypy-boto3-connectcases-1.28.16/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:32.408918 mypy-boto3-connectcases-1.28.16/mypy_boto3_connectcases/
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-08-01 11:14:17.000000 mypy-boto3-connectcases-1.28.16/mypy_boto3_connectcases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-08-01 11:14:17.000000 mypy-boto3-connectcases-1.28.16/mypy_boto3_connectcases/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-08-01 11:14:17.000000 mypy-boto3-connectcases-1.28.16/mypy_boto3_connectcases/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22189 2023-08-01 11:14:18.000000 mypy-boto3-connectcases-1.28.16/mypy_boto3_connectcases/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    22150 2023-08-01 11:14:18.000000 mypy-boto3-connectcases-1.28.16/mypy_boto3_connectcases/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8660 2023-08-01 11:14:18.000000 mypy-boto3-connectcases-1.28.16/mypy_boto3_connectcases/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8658 2023-08-01 11:14:18.000000 mypy-boto3-connectcases-1.28.16/mypy_boto3_connectcases/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-08-01 11:14:18.000000 mypy-boto3-connectcases-1.28.16/mypy_boto3_connectcases/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-08-01 11:14:18.000000 mypy-boto3-connectcases-1.28.16/mypy_boto3_connectcases/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:14:17.000000 mypy-boto3-connectcases-1.28.16/mypy_boto3_connectcases/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    32414 2023-08-01 11:14:19.000000 mypy-boto3-connectcases-1.28.16/mypy_boto3_connectcases/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    32366 2023-08-01 11:14:19.000000 mypy-boto3-connectcases-1.28.16/mypy_boto3_connectcases/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:14:17.000000 mypy-boto3-connectcases-1.28.16/mypy_boto3_connectcases/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:32.416918 mypy-boto3-connectcases-1.28.16/mypy_boto3_connectcases.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16641 2023-08-01 11:36:32.000000 mypy-boto3-connectcases-1.28.16/mypy_boto3_connectcases.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-08-01 11:36:32.000000 mypy-boto3-connectcases-1.28.16/mypy_boto3_connectcases.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:32.000000 mypy-boto3-connectcases-1.28.16/mypy_boto3_connectcases.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:32.000000 mypy-boto3-connectcases-1.28.16/mypy_boto3_connectcases.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:32.000000 mypy-boto3-connectcases-1.28.16/mypy_boto3_connectcases.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-01 11:36:32.000000 mypy-boto3-connectcases-1.28.16/mypy_boto3_connectcases.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:32.416918 mypy-boto3-connectcases-1.28.16/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-08-01 11:14:16.000000 mypy-boto3-connectcases-1.28.16/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:47:56.012775 mypy-boto3-connectcases-1.28.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-20 19:46:46.000000 mypy-boto3-connectcases-1.28.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16827 2023-07-20 19:47:56.004775 mypy-boto3-connectcases-1.28.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15322 2023-07-20 19:46:46.000000 mypy-boto3-connectcases-1.28.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:47:56.000775 mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases/
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-20 19:46:46.000000 mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-20 19:46:46.000000 mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-20 19:46:46.000000 mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22107 2023-07-20 19:46:47.000000 mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22068 2023-07-20 19:46:47.000000 mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8605 2023-07-20 19:46:47.000000 mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8603 2023-07-20 19:46:47.000000 mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-07-20 19:46:47.000000 mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-07-20 19:46:47.000000 mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 19:46:46.000000 mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    31710 2023-07-20 19:46:48.000000 mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31674 2023-07-20 19:46:48.000000 mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-20 19:46:46.000000 mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:47:56.004775 mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16827 2023-07-20 19:47:55.000000 mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-20 19:47:55.000000 mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 19:47:55.000000 mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 19:47:55.000000 mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-20 19:47:55.000000 mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-20 19:47:55.000000 mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 19:47:56.012775 mypy-boto3-connectcases-1.28.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-20 19:46:46.000000 mypy-boto3-connectcases-1.28.8/setup.py
```

### Comparing `mypy-boto3-connectcases-1.28.16/LICENSE` & `mypy-boto3-connectcases-1.28.8/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connectcases-1.28.16/PKG-INFO` & `mypy-boto3-connectcases-1.28.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-connectcases
-Version: 1.28.16
-Summary: Type annotations for boto3.ConnectCases 1.28.16 service generated with mypy-boto3-builder 7.17.1
+Version: 1.28.8
+Summary: Type annotations for boto3.ConnectCases 1.28.8 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 connectcases type-annotations botocore mypy typeshed autocomplete
+Keywords: boto3 connectcases type-annotations boto3-stubs mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-connectcases"></a>
 
 # mypy-boto3-connectcases
 
 [![PyPI - mypy-boto3-connectcases](https://img.shields.io/pypi/v/mypy-boto3-connectcases.svg?color=blue)](https://pypi.org/project/mypy-boto3-connectcases)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-connectcases.svg?color=blue)](https://pypi.org/project/mypy-boto3-connectcases)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-connectcases)](https://pepy.tech/project/mypy-boto3-connectcases)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-connectcases?color=blue)](https://pypistats.org/packages/mypy-boto3-connectcases)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ConnectCases 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases)
+[boto3.ConnectCases 1.28.8](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.17.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-connectcases docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/).
 
 See how it helps to find and fix potential bugs:
 
@@ -74,15 +74,15 @@
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Literals](#literals)
-    - [Type definitions](#type-definitions)
+    - [Typed dictionaries](#typed-dictionaries)
   - [How it works](#how-it-works)
   - [What's new](#what's-new)
     - [Implemented features](#implemented-features)
     - [Latest changes](#latest-changes)
   - [Versioning](#versioning)
   - [Thank you](#thank-you)
   - [Documentation](#documentation)
@@ -321,50 +321,56 @@
 )
 
 
 def check_value(value: CommentBodyTextTypeType) -> bool:
     ...
 ```
 
-<a id="type-definitions"></a>
+<a id="typed-dictionaries"></a>
 
-### Type definitions
+### Typed dictionaries
 
 `mypy_boto3_connectcases.type_defs` module contains structures and shapes
-assembled to typed dictionaries and unions for additional type checking.
+assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_connectcases.type_defs import (
     FieldIdentifierTypeDef,
     FieldErrorTypeDef,
     GetFieldResponseTypeDef,
     ResponseMetadataTypeDef,
     FieldOptionTypeDef,
     FieldOptionErrorTypeDef,
-    FieldFilterTypeDef,
+    FieldIdentifierOutputTypeDef,
     CaseSummaryTypeDef,
+    CommentContentOutputTypeDef,
     CommentContentTypeDef,
     ContactContentTypeDef,
     ContactFilterTypeDef,
     ContactTypeDef,
-    CreateCaseRequestRequestTypeDef,
     CreateDomainRequestRequestTypeDef,
     CreateFieldRequestRequestTypeDef,
     LayoutConfigurationTypeDef,
     RequiredFieldTypeDef,
     DeleteDomainRequestRequestTypeDef,
     DomainSummaryTypeDef,
+    RelatedItemEventIncludedDataOutputTypeDef,
     RelatedItemEventIncludedDataTypeDef,
+    FieldItemOutputTypeDef,
     FieldItemTypeDef,
+    FieldOptionOutputTypeDef,
     FieldSummaryTypeDef,
     FieldValueUnionOutputTypeDef,
+    FieldValueUnionTypeDef,
     GetCaseEventConfigurationRequestRequestTypeDef,
     GetDomainRequestRequestTypeDef,
     GetLayoutRequestRequestTypeDef,
     GetTemplateRequestRequestTypeDef,
+    LayoutConfigurationOutputTypeDef,
+    RequiredFieldOutputTypeDef,
     LayoutSummaryTypeDef,
     ListCasesForContactRequestRequestTypeDef,
     ListDomainsRequestRequestTypeDef,
     ListFieldOptionsRequestRequestTypeDef,
     ListFieldsRequestRequestTypeDef,
     ListLayoutsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
@@ -372,81 +378,80 @@
     TemplateSummaryTypeDef,
     PaginatorConfigTypeDef,
     SortTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateFieldRequestRequestTypeDef,
     BatchGetFieldRequestRequestTypeDef,
-    CaseEventIncludedDataOutputTypeDef,
     CaseEventIncludedDataTypeDef,
     GetCaseRequestRequestTypeDef,
     BatchGetFieldResponseTypeDef,
     CreateCaseResponseTypeDef,
     CreateDomainResponseTypeDef,
     CreateFieldResponseTypeDef,
     CreateLayoutResponseTypeDef,
     CreateRelatedItemResponseTypeDef,
     CreateTemplateResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetDomainResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     BatchPutFieldOptionsRequestRequestTypeDef,
-    ListFieldOptionsResponseTypeDef,
     BatchPutFieldOptionsResponseTypeDef,
-    CaseFilterTypeDef,
+    CaseEventIncludedDataOutputTypeDef,
     ListCasesForContactResponseTypeDef,
     RelatedItemContentTypeDef,
     RelatedItemTypeFilterTypeDef,
     RelatedItemInputContentTypeDef,
     CreateTemplateRequestRequestTypeDef,
-    GetTemplateResponseTypeDef,
     UpdateTemplateRequestRequestTypeDef,
     ListDomainsResponseTypeDef,
     FieldGroupOutputTypeDef,
     FieldGroupTypeDef,
+    ListFieldOptionsResponseTypeDef,
     ListFieldsResponseTypeDef,
     FieldValueOutputTypeDef,
+    FieldValueTypeDef,
+    GetTemplateResponseTypeDef,
     ListLayoutsResponseTypeDef,
     ListTemplatesResponseTypeDef,
     SearchCasesRequestRequestTypeDef,
     SearchCasesRequestSearchCasesPaginateTypeDef,
-    EventIncludedDataOutputTypeDef,
     EventIncludedDataTypeDef,
+    EventIncludedDataOutputTypeDef,
     SearchRelatedItemsResponseItemTypeDef,
     SearchRelatedItemsRequestRequestTypeDef,
     SearchRelatedItemsRequestSearchRelatedItemsPaginateTypeDef,
     CreateRelatedItemRequestRequestTypeDef,
     SectionOutputTypeDef,
     SectionTypeDef,
-    FieldValueUnionTypeDef,
     GetCaseResponseTypeDef,
     SearchCasesResponseItemTypeDef,
-    EventBridgeConfigurationOutputTypeDef,
+    CreateCaseRequestRequestTypeDef,
+    FieldFilterTypeDef,
+    UpdateCaseRequestRequestTypeDef,
     EventBridgeConfigurationTypeDef,
+    EventBridgeConfigurationOutputTypeDef,
     SearchRelatedItemsResponseTypeDef,
     LayoutSectionsOutputTypeDef,
     LayoutSectionsTypeDef,
-    FieldValueTypeDef,
-    UpdateCaseRequestRequestTypeDef,
     SearchCasesResponseTypeDef,
-    GetCaseEventConfigurationResponseTypeDef,
-    EventBridgeConfigurationUnionTypeDef,
+    CaseFilterTypeDef,
     PutCaseEventConfigurationRequestRequestTypeDef,
+    GetCaseEventConfigurationResponseTypeDef,
     BasicLayoutOutputTypeDef,
     BasicLayoutTypeDef,
     LayoutContentOutputTypeDef,
     LayoutContentTypeDef,
     GetLayoutResponseTypeDef,
     CreateLayoutRequestRequestTypeDef,
-    LayoutContentUnionTypeDef,
     UpdateLayoutRequestRequestTypeDef,
 )
 
 
-def get_value() -> FieldIdentifierTypeDef:
+def get_structure() -> FieldIdentifierTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-connectcases-1.28.16/README.md` & `mypy-boto3-connectcases-1.28.8/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-connectcases"></a>
 
 # mypy-boto3-connectcases
 
 [![PyPI - mypy-boto3-connectcases](https://img.shields.io/pypi/v/mypy-boto3-connectcases.svg?color=blue)](https://pypi.org/project/mypy-boto3-connectcases)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-connectcases.svg?color=blue)](https://pypi.org/project/mypy-boto3-connectcases)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-connectcases)](https://pepy.tech/project/mypy-boto3-connectcases)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-connectcases?color=blue)](https://pypistats.org/packages/mypy-boto3-connectcases)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ConnectCases 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases)
+[boto3.ConnectCases 1.28.8](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.17.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-connectcases docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/).
 
 See how it helps to find and fix potential bugs:
 
@@ -42,15 +42,15 @@
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Literals](#literals)
-    - [Type definitions](#type-definitions)
+    - [Typed dictionaries](#typed-dictionaries)
   - [How it works](#how-it-works)
   - [What's new](#what's-new)
     - [Implemented features](#implemented-features)
     - [Latest changes](#latest-changes)
   - [Versioning](#versioning)
   - [Thank you](#thank-you)
   - [Documentation](#documentation)
@@ -289,50 +289,56 @@
 )
 
 
 def check_value(value: CommentBodyTextTypeType) -> bool:
     ...
 ```
 
-<a id="type-definitions"></a>
+<a id="typed-dictionaries"></a>
 
-### Type definitions
+### Typed dictionaries
 
 `mypy_boto3_connectcases.type_defs` module contains structures and shapes
-assembled to typed dictionaries and unions for additional type checking.
+assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_connectcases.type_defs import (
     FieldIdentifierTypeDef,
     FieldErrorTypeDef,
     GetFieldResponseTypeDef,
     ResponseMetadataTypeDef,
     FieldOptionTypeDef,
     FieldOptionErrorTypeDef,
-    FieldFilterTypeDef,
+    FieldIdentifierOutputTypeDef,
     CaseSummaryTypeDef,
+    CommentContentOutputTypeDef,
     CommentContentTypeDef,
     ContactContentTypeDef,
     ContactFilterTypeDef,
     ContactTypeDef,
-    CreateCaseRequestRequestTypeDef,
     CreateDomainRequestRequestTypeDef,
     CreateFieldRequestRequestTypeDef,
     LayoutConfigurationTypeDef,
     RequiredFieldTypeDef,
     DeleteDomainRequestRequestTypeDef,
     DomainSummaryTypeDef,
+    RelatedItemEventIncludedDataOutputTypeDef,
     RelatedItemEventIncludedDataTypeDef,
+    FieldItemOutputTypeDef,
     FieldItemTypeDef,
+    FieldOptionOutputTypeDef,
     FieldSummaryTypeDef,
     FieldValueUnionOutputTypeDef,
+    FieldValueUnionTypeDef,
     GetCaseEventConfigurationRequestRequestTypeDef,
     GetDomainRequestRequestTypeDef,
     GetLayoutRequestRequestTypeDef,
     GetTemplateRequestRequestTypeDef,
+    LayoutConfigurationOutputTypeDef,
+    RequiredFieldOutputTypeDef,
     LayoutSummaryTypeDef,
     ListCasesForContactRequestRequestTypeDef,
     ListDomainsRequestRequestTypeDef,
     ListFieldOptionsRequestRequestTypeDef,
     ListFieldsRequestRequestTypeDef,
     ListLayoutsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
@@ -340,81 +346,80 @@
     TemplateSummaryTypeDef,
     PaginatorConfigTypeDef,
     SortTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateFieldRequestRequestTypeDef,
     BatchGetFieldRequestRequestTypeDef,
-    CaseEventIncludedDataOutputTypeDef,
     CaseEventIncludedDataTypeDef,
     GetCaseRequestRequestTypeDef,
     BatchGetFieldResponseTypeDef,
     CreateCaseResponseTypeDef,
     CreateDomainResponseTypeDef,
     CreateFieldResponseTypeDef,
     CreateLayoutResponseTypeDef,
     CreateRelatedItemResponseTypeDef,
     CreateTemplateResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetDomainResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     BatchPutFieldOptionsRequestRequestTypeDef,
-    ListFieldOptionsResponseTypeDef,
     BatchPutFieldOptionsResponseTypeDef,
-    CaseFilterTypeDef,
+    CaseEventIncludedDataOutputTypeDef,
     ListCasesForContactResponseTypeDef,
     RelatedItemContentTypeDef,
     RelatedItemTypeFilterTypeDef,
     RelatedItemInputContentTypeDef,
     CreateTemplateRequestRequestTypeDef,
-    GetTemplateResponseTypeDef,
     UpdateTemplateRequestRequestTypeDef,
     ListDomainsResponseTypeDef,
     FieldGroupOutputTypeDef,
     FieldGroupTypeDef,
+    ListFieldOptionsResponseTypeDef,
     ListFieldsResponseTypeDef,
     FieldValueOutputTypeDef,
+    FieldValueTypeDef,
+    GetTemplateResponseTypeDef,
     ListLayoutsResponseTypeDef,
     ListTemplatesResponseTypeDef,
     SearchCasesRequestRequestTypeDef,
     SearchCasesRequestSearchCasesPaginateTypeDef,
-    EventIncludedDataOutputTypeDef,
     EventIncludedDataTypeDef,
+    EventIncludedDataOutputTypeDef,
     SearchRelatedItemsResponseItemTypeDef,
     SearchRelatedItemsRequestRequestTypeDef,
     SearchRelatedItemsRequestSearchRelatedItemsPaginateTypeDef,
     CreateRelatedItemRequestRequestTypeDef,
     SectionOutputTypeDef,
     SectionTypeDef,
-    FieldValueUnionTypeDef,
     GetCaseResponseTypeDef,
     SearchCasesResponseItemTypeDef,
-    EventBridgeConfigurationOutputTypeDef,
+    CreateCaseRequestRequestTypeDef,
+    FieldFilterTypeDef,
+    UpdateCaseRequestRequestTypeDef,
     EventBridgeConfigurationTypeDef,
+    EventBridgeConfigurationOutputTypeDef,
     SearchRelatedItemsResponseTypeDef,
     LayoutSectionsOutputTypeDef,
     LayoutSectionsTypeDef,
-    FieldValueTypeDef,
-    UpdateCaseRequestRequestTypeDef,
     SearchCasesResponseTypeDef,
-    GetCaseEventConfigurationResponseTypeDef,
-    EventBridgeConfigurationUnionTypeDef,
+    CaseFilterTypeDef,
     PutCaseEventConfigurationRequestRequestTypeDef,
+    GetCaseEventConfigurationResponseTypeDef,
     BasicLayoutOutputTypeDef,
     BasicLayoutTypeDef,
     LayoutContentOutputTypeDef,
     LayoutContentTypeDef,
     GetLayoutResponseTypeDef,
     CreateLayoutRequestRequestTypeDef,
-    LayoutContentUnionTypeDef,
     UpdateLayoutRequestRequestTypeDef,
 )
 
 
-def get_value() -> FieldIdentifierTypeDef:
+def get_structure() -> FieldIdentifierTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-connectcases-1.28.16/mypy_boto3_connectcases/__init__.py` & `mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connectcases-1.28.16/mypy_boto3_connectcases/__init__.pyi` & `mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connectcases-1.28.16/mypy_boto3_connectcases/__main__.py` & `mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ConnectCases 1.28.16\nVersion:         1.28.16\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for boto3.ConnectCases 1.28.8\nVersion:         1.28.8\nBuilder version:"
+        " 7.15.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.16")
+    print("1.28.8")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-connectcases-1.28.16/mypy_boto3_connectcases/client.py` & `mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -27,25 +27,25 @@
     CreateCaseResponseTypeDef,
     CreateDomainResponseTypeDef,
     CreateFieldResponseTypeDef,
     CreateLayoutResponseTypeDef,
     CreateRelatedItemResponseTypeDef,
     CreateTemplateResponseTypeDef,
     EmptyResponseMetadataTypeDef,
-    EventBridgeConfigurationUnionTypeDef,
+    EventBridgeConfigurationTypeDef,
     FieldIdentifierTypeDef,
     FieldOptionTypeDef,
-    FieldValueUnionTypeDef,
+    FieldValueTypeDef,
     GetCaseEventConfigurationResponseTypeDef,
     GetCaseResponseTypeDef,
     GetDomainResponseTypeDef,
     GetLayoutResponseTypeDef,
     GetTemplateResponseTypeDef,
     LayoutConfigurationTypeDef,
-    LayoutContentUnionTypeDef,
+    LayoutContentTypeDef,
     ListCasesForContactResponseTypeDef,
     ListDomainsResponseTypeDef,
     ListFieldOptionsResponseTypeDef,
     ListFieldsResponseTypeDef,
     ListLayoutsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTemplatesResponseTypeDef,
@@ -58,37 +58,33 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("ConnectCasesClient",)
 
-
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ServiceQuotaExceededException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
-
 class ConnectCasesClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/)
     """
 
     meta: ClientMeta
@@ -97,96 +93,87 @@
     def exceptions(self) -> Exceptions:
         """
         ConnectCasesClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#exceptions)
         """
-
     def batch_get_field(
         self, *, domainId: str, fields: Sequence[FieldIdentifierTypeDef]
     ) -> BatchGetFieldResponseTypeDef:
         """
         Returns the description for the list of fields in the request parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.batch_get_field)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#batch_get_field)
         """
-
     def batch_put_field_options(
         self, *, domainId: str, fieldId: str, options: Sequence[FieldOptionTypeDef]
     ) -> BatchPutFieldOptionsResponseTypeDef:
         """
         Creates and updates a set of field options for a single select field in a Cases
         domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.batch_put_field_options)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#batch_put_field_options)
         """
-
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#can_paginate)
         """
-
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#close)
         """
-
     def create_case(
         self,
         *,
         domainId: str,
-        fields: Sequence["FieldValueUnionTypeDef"],
+        fields: Sequence[FieldValueTypeDef],
         templateId: str,
         clientToken: str = ...
     ) -> CreateCaseResponseTypeDef:
         """
         Creates a case in the specified Cases domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.create_case)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#create_case)
         """
-
     def create_domain(self, *, name: str) -> CreateDomainResponseTypeDef:
         """
         Creates a domain, which is a container for all case data, such as cases, fields,
         templates and layouts.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.create_domain)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#create_domain)
         """
-
     def create_field(
         self, *, domainId: str, name: str, type: FieldTypeType, description: str = ...
     ) -> CreateFieldResponseTypeDef:
         """
         Creates a field in the Cases domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.create_field)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#create_field)
         """
-
     def create_layout(
-        self, *, content: LayoutContentUnionTypeDef, domainId: str, name: str
+        self, *, content: LayoutContentTypeDef, domainId: str, name: str
     ) -> CreateLayoutResponseTypeDef:
         """
         Creates a layout in the Cases domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.create_layout)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#create_layout)
         """
-
     def create_related_item(
         self,
         *,
         caseId: str,
         content: RelatedItemInputContentTypeDef,
         domainId: str,
         type: RelatedItemTypeType
@@ -194,15 +181,14 @@
         """
         Creates a related item (comments, tasks, and contacts) and associates it with a
         case.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.create_related_item)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#create_related_item)
         """
-
     def create_template(
         self,
         *,
         domainId: str,
         name: str,
         description: str = ...,
         layoutConfiguration: LayoutConfigurationTypeDef = ...,
@@ -211,106 +197,96 @@
     ) -> CreateTemplateResponseTypeDef:
         """
         Creates a template in the Cases domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.create_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#create_template)
         """
-
     def delete_domain(self, *, domainId: str) -> Dict[str, Any]:
         """
         Deletes a Cases domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.delete_domain)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#delete_domain)
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
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#generate_presigned_url)
         """
-
     def get_case(
         self,
         *,
         caseId: str,
         domainId: str,
         fields: Sequence[FieldIdentifierTypeDef],
         nextToken: str = ...
     ) -> GetCaseResponseTypeDef:
         """
         Returns information about a specific case if it exists.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.get_case)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#get_case)
         """
-
     def get_case_event_configuration(
         self, *, domainId: str
     ) -> GetCaseEventConfigurationResponseTypeDef:
         """
         Returns the case event publishing configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.get_case_event_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#get_case_event_configuration)
         """
-
     def get_domain(self, *, domainId: str) -> GetDomainResponseTypeDef:
         """
         Returns information about a specific domain if it exists.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.get_domain)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#get_domain)
         """
-
     def get_layout(self, *, domainId: str, layoutId: str) -> GetLayoutResponseTypeDef:
         """
         Returns the details for the requested layout.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.get_layout)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#get_layout)
         """
-
     def get_template(self, *, domainId: str, templateId: str) -> GetTemplateResponseTypeDef:
         """
         Returns the details for the requested template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.get_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#get_template)
         """
-
     def list_cases_for_contact(
         self, *, contactArn: str, domainId: str, maxResults: int = ..., nextToken: str = ...
     ) -> ListCasesForContactResponseTypeDef:
         """
         Lists cases for a given contact.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.list_cases_for_contact)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#list_cases_for_contact)
         """
-
     def list_domains(
         self, *, maxResults: int = ..., nextToken: str = ...
     ) -> ListDomainsResponseTypeDef:
         """
         Lists all cases domains in the Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.list_domains)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#list_domains)
         """
-
     def list_field_options(
         self,
         *,
         domainId: str,
         fieldId: str,
         maxResults: int = ...,
         nextToken: str = ...,
@@ -318,69 +294,63 @@
     ) -> ListFieldOptionsResponseTypeDef:
         """
         Lists all of the field options for a field identifier in the domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.list_field_options)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#list_field_options)
         """
-
     def list_fields(
         self, *, domainId: str, maxResults: int = ..., nextToken: str = ...
     ) -> ListFieldsResponseTypeDef:
         """
         Lists all fields in a Cases domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.list_fields)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#list_fields)
         """
-
     def list_layouts(
         self, *, domainId: str, maxResults: int = ..., nextToken: str = ...
     ) -> ListLayoutsResponseTypeDef:
         """
         Lists all layouts in the given cases domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.list_layouts)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#list_layouts)
         """
-
     def list_tags_for_resource(self, *, arn: str) -> ListTagsForResourceResponseTypeDef:
         """
         Lists tags for a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#list_tags_for_resource)
         """
-
     def list_templates(
         self,
         *,
         domainId: str,
         maxResults: int = ...,
         nextToken: str = ...,
         status: Sequence[TemplateStatusType] = ...
     ) -> ListTemplatesResponseTypeDef:
         """
         Lists all of the templates in a Cases domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.list_templates)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#list_templates)
         """
-
     def put_case_event_configuration(
-        self, *, domainId: str, eventBridge: EventBridgeConfigurationUnionTypeDef
+        self, *, domainId: str, eventBridge: EventBridgeConfigurationTypeDef
     ) -> Dict[str, Any]:
         """
         API for adding case event publishing configuration See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/connectcases-2022-10-03/PutCaseEventConfiguration).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.put_case_event_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#put_case_event_configuration)
         """
-
     def search_cases(
         self,
         *,
         domainId: str,
         fields: Sequence[FieldIdentifierTypeDef] = ...,
         filter: "CaseFilterTypeDef" = ...,
         maxResults: int = ...,
@@ -390,15 +360,14 @@
     ) -> SearchCasesResponseTypeDef:
         """
         Searches for cases within their associated Cases domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.search_cases)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#search_cases)
         """
-
     def search_related_items(
         self,
         *,
         caseId: str,
         domainId: str,
         filters: Sequence[RelatedItemTypeFilterTypeDef] = ...,
         maxResults: int = ...,
@@ -406,66 +375,55 @@
     ) -> SearchRelatedItemsResponseTypeDef:
         """
         Searches for related items that are associated with a case.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.search_related_items)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#search_related_items)
         """
-
     def tag_resource(self, *, arn: str, tags: Mapping[str, str]) -> EmptyResponseMetadataTypeDef:
         """
         Adds tags to a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#tag_resource)
         """
-
     def untag_resource(self, *, arn: str, tagKeys: Sequence[str]) -> EmptyResponseMetadataTypeDef:
         """
         Untags a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#untag_resource)
         """
-
     def update_case(
-        self, *, caseId: str, domainId: str, fields: Sequence[FieldValueUnionTypeDef]
+        self, *, caseId: str, domainId: str, fields: Sequence[FieldValueTypeDef]
     ) -> Dict[str, Any]:
         """
         Updates the values of fields on a case.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.update_case)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#update_case)
         """
-
     def update_field(
         self, *, domainId: str, fieldId: str, description: str = ..., name: str = ...
     ) -> Dict[str, Any]:
         """
         Updates the properties of an existing field.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.update_field)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#update_field)
         """
-
     def update_layout(
-        self,
-        *,
-        domainId: str,
-        layoutId: str,
-        content: LayoutContentUnionTypeDef = ...,
-        name: str = ...
+        self, *, domainId: str, layoutId: str, content: LayoutContentTypeDef = ..., name: str = ...
     ) -> Dict[str, Any]:
         """
         Updates the attributes of an existing layout.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.update_layout)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#update_layout)
         """
-
     def update_template(
         self,
         *,
         domainId: str,
         templateId: str,
         description: str = ...,
         layoutConfiguration: LayoutConfigurationTypeDef = ...,
@@ -475,22 +433,20 @@
     ) -> Dict[str, Any]:
         """
         Updates the attributes of an existing template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.update_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#update_template)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["search_cases"]) -> SearchCasesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["search_related_items"]
     ) -> SearchRelatedItemsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#get_paginator)
```

### Comparing `mypy-boto3-connectcases-1.28.16/mypy_boto3_connectcases/client.pyi` & `mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,25 +27,25 @@
     CreateCaseResponseTypeDef,
     CreateDomainResponseTypeDef,
     CreateFieldResponseTypeDef,
     CreateLayoutResponseTypeDef,
     CreateRelatedItemResponseTypeDef,
     CreateTemplateResponseTypeDef,
     EmptyResponseMetadataTypeDef,
-    EventBridgeConfigurationUnionTypeDef,
+    EventBridgeConfigurationTypeDef,
     FieldIdentifierTypeDef,
     FieldOptionTypeDef,
-    FieldValueUnionTypeDef,
+    FieldValueTypeDef,
     GetCaseEventConfigurationResponseTypeDef,
     GetCaseResponseTypeDef,
     GetDomainResponseTypeDef,
     GetLayoutResponseTypeDef,
     GetTemplateResponseTypeDef,
     LayoutConfigurationTypeDef,
-    LayoutContentUnionTypeDef,
+    LayoutContentTypeDef,
     ListCasesForContactResponseTypeDef,
     ListDomainsResponseTypeDef,
     ListFieldOptionsResponseTypeDef,
     ListFieldsResponseTypeDef,
     ListLayoutsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTemplatesResponseTypeDef,
@@ -58,33 +58,37 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = ("ConnectCasesClient",)
 
+
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ServiceQuotaExceededException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
+
 class ConnectCasesClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/)
     """
 
     meta: ClientMeta
@@ -93,87 +97,96 @@
     def exceptions(self) -> Exceptions:
         """
         ConnectCasesClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#exceptions)
         """
+
     def batch_get_field(
         self, *, domainId: str, fields: Sequence[FieldIdentifierTypeDef]
     ) -> BatchGetFieldResponseTypeDef:
         """
         Returns the description for the list of fields in the request parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.batch_get_field)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#batch_get_field)
         """
+
     def batch_put_field_options(
         self, *, domainId: str, fieldId: str, options: Sequence[FieldOptionTypeDef]
     ) -> BatchPutFieldOptionsResponseTypeDef:
         """
         Creates and updates a set of field options for a single select field in a Cases
         domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.batch_put_field_options)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#batch_put_field_options)
         """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#can_paginate)
         """
+
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#close)
         """
+
     def create_case(
         self,
         *,
         domainId: str,
-        fields: Sequence["FieldValueUnionTypeDef"],
+        fields: Sequence[FieldValueTypeDef],
         templateId: str,
         clientToken: str = ...
     ) -> CreateCaseResponseTypeDef:
         """
         Creates a case in the specified Cases domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.create_case)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#create_case)
         """
+
     def create_domain(self, *, name: str) -> CreateDomainResponseTypeDef:
         """
         Creates a domain, which is a container for all case data, such as cases, fields,
         templates and layouts.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.create_domain)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#create_domain)
         """
+
     def create_field(
         self, *, domainId: str, name: str, type: FieldTypeType, description: str = ...
     ) -> CreateFieldResponseTypeDef:
         """
         Creates a field in the Cases domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.create_field)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#create_field)
         """
+
     def create_layout(
-        self, *, content: LayoutContentUnionTypeDef, domainId: str, name: str
+        self, *, content: LayoutContentTypeDef, domainId: str, name: str
     ) -> CreateLayoutResponseTypeDef:
         """
         Creates a layout in the Cases domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.create_layout)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#create_layout)
         """
+
     def create_related_item(
         self,
         *,
         caseId: str,
         content: RelatedItemInputContentTypeDef,
         domainId: str,
         type: RelatedItemTypeType
@@ -181,14 +194,15 @@
         """
         Creates a related item (comments, tasks, and contacts) and associates it with a
         case.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.create_related_item)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#create_related_item)
         """
+
     def create_template(
         self,
         *,
         domainId: str,
         name: str,
         description: str = ...,
         layoutConfiguration: LayoutConfigurationTypeDef = ...,
@@ -197,96 +211,106 @@
     ) -> CreateTemplateResponseTypeDef:
         """
         Creates a template in the Cases domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.create_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#create_template)
         """
+
     def delete_domain(self, *, domainId: str) -> Dict[str, Any]:
         """
         Deletes a Cases domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.delete_domain)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#delete_domain)
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
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#generate_presigned_url)
         """
+
     def get_case(
         self,
         *,
         caseId: str,
         domainId: str,
         fields: Sequence[FieldIdentifierTypeDef],
         nextToken: str = ...
     ) -> GetCaseResponseTypeDef:
         """
         Returns information about a specific case if it exists.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.get_case)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#get_case)
         """
+
     def get_case_event_configuration(
         self, *, domainId: str
     ) -> GetCaseEventConfigurationResponseTypeDef:
         """
         Returns the case event publishing configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.get_case_event_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#get_case_event_configuration)
         """
+
     def get_domain(self, *, domainId: str) -> GetDomainResponseTypeDef:
         """
         Returns information about a specific domain if it exists.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.get_domain)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#get_domain)
         """
+
     def get_layout(self, *, domainId: str, layoutId: str) -> GetLayoutResponseTypeDef:
         """
         Returns the details for the requested layout.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.get_layout)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#get_layout)
         """
+
     def get_template(self, *, domainId: str, templateId: str) -> GetTemplateResponseTypeDef:
         """
         Returns the details for the requested template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.get_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#get_template)
         """
+
     def list_cases_for_contact(
         self, *, contactArn: str, domainId: str, maxResults: int = ..., nextToken: str = ...
     ) -> ListCasesForContactResponseTypeDef:
         """
         Lists cases for a given contact.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.list_cases_for_contact)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#list_cases_for_contact)
         """
+
     def list_domains(
         self, *, maxResults: int = ..., nextToken: str = ...
     ) -> ListDomainsResponseTypeDef:
         """
         Lists all cases domains in the Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.list_domains)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#list_domains)
         """
+
     def list_field_options(
         self,
         *,
         domainId: str,
         fieldId: str,
         maxResults: int = ...,
         nextToken: str = ...,
@@ -294,63 +318,69 @@
     ) -> ListFieldOptionsResponseTypeDef:
         """
         Lists all of the field options for a field identifier in the domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.list_field_options)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#list_field_options)
         """
+
     def list_fields(
         self, *, domainId: str, maxResults: int = ..., nextToken: str = ...
     ) -> ListFieldsResponseTypeDef:
         """
         Lists all fields in a Cases domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.list_fields)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#list_fields)
         """
+
     def list_layouts(
         self, *, domainId: str, maxResults: int = ..., nextToken: str = ...
     ) -> ListLayoutsResponseTypeDef:
         """
         Lists all layouts in the given cases domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.list_layouts)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#list_layouts)
         """
+
     def list_tags_for_resource(self, *, arn: str) -> ListTagsForResourceResponseTypeDef:
         """
         Lists tags for a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#list_tags_for_resource)
         """
+
     def list_templates(
         self,
         *,
         domainId: str,
         maxResults: int = ...,
         nextToken: str = ...,
         status: Sequence[TemplateStatusType] = ...
     ) -> ListTemplatesResponseTypeDef:
         """
         Lists all of the templates in a Cases domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.list_templates)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#list_templates)
         """
+
     def put_case_event_configuration(
-        self, *, domainId: str, eventBridge: EventBridgeConfigurationUnionTypeDef
+        self, *, domainId: str, eventBridge: EventBridgeConfigurationTypeDef
     ) -> Dict[str, Any]:
         """
         API for adding case event publishing configuration See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/connectcases-2022-10-03/PutCaseEventConfiguration).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.put_case_event_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#put_case_event_configuration)
         """
+
     def search_cases(
         self,
         *,
         domainId: str,
         fields: Sequence[FieldIdentifierTypeDef] = ...,
         filter: "CaseFilterTypeDef" = ...,
         maxResults: int = ...,
@@ -360,14 +390,15 @@
     ) -> SearchCasesResponseTypeDef:
         """
         Searches for cases within their associated Cases domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.search_cases)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#search_cases)
         """
+
     def search_related_items(
         self,
         *,
         caseId: str,
         domainId: str,
         filters: Sequence[RelatedItemTypeFilterTypeDef] = ...,
         maxResults: int = ...,
@@ -375,60 +406,61 @@
     ) -> SearchRelatedItemsResponseTypeDef:
         """
         Searches for related items that are associated with a case.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.search_related_items)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#search_related_items)
         """
+
     def tag_resource(self, *, arn: str, tags: Mapping[str, str]) -> EmptyResponseMetadataTypeDef:
         """
         Adds tags to a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#tag_resource)
         """
+
     def untag_resource(self, *, arn: str, tagKeys: Sequence[str]) -> EmptyResponseMetadataTypeDef:
         """
         Untags a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#untag_resource)
         """
+
     def update_case(
-        self, *, caseId: str, domainId: str, fields: Sequence[FieldValueUnionTypeDef]
+        self, *, caseId: str, domainId: str, fields: Sequence[FieldValueTypeDef]
     ) -> Dict[str, Any]:
         """
         Updates the values of fields on a case.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.update_case)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#update_case)
         """
+
     def update_field(
         self, *, domainId: str, fieldId: str, description: str = ..., name: str = ...
     ) -> Dict[str, Any]:
         """
         Updates the properties of an existing field.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.update_field)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#update_field)
         """
+
     def update_layout(
-        self,
-        *,
-        domainId: str,
-        layoutId: str,
-        content: LayoutContentUnionTypeDef = ...,
-        name: str = ...
+        self, *, domainId: str, layoutId: str, content: LayoutContentTypeDef = ..., name: str = ...
     ) -> Dict[str, Any]:
         """
         Updates the attributes of an existing layout.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.update_layout)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#update_layout)
         """
+
     def update_template(
         self,
         *,
         domainId: str,
         templateId: str,
         description: str = ...,
         layoutConfiguration: LayoutConfigurationTypeDef = ...,
@@ -438,20 +470,22 @@
     ) -> Dict[str, Any]:
         """
         Updates the attributes of an existing template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.update_template)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#update_template)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["search_cases"]) -> SearchCasesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["search_related_items"]
     ) -> SearchRelatedItemsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/client/#get_paginator)
```

### Comparing `mypy-boto3-connectcases-1.28.16/mypy_boto3_connectcases/literals.py` & `mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,15 +162,14 @@
     "elasticbeanstalk",
     "elastictranscoder",
     "elb",
     "elbv2",
     "emr",
     "emr-containers",
     "emr-serverless",
-    "entityresolution",
     "es",
     "events",
     "evidently",
     "finspace",
     "finspace-data",
     "firehose",
     "fis",
@@ -249,15 +248,14 @@
     "lookoutmetrics",
     "lookoutvision",
     "m2",
     "machinelearning",
     "macie",
     "macie2",
     "managedblockchain",
-    "managedblockchain-query",
     "marketplace-catalog",
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
```

### Comparing `mypy-boto3-connectcases-1.28.16/mypy_boto3_connectcases/literals.pyi` & `mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -160,15 +160,14 @@
     "elasticbeanstalk",
     "elastictranscoder",
     "elb",
     "elbv2",
     "emr",
     "emr-containers",
     "emr-serverless",
-    "entityresolution",
     "es",
     "events",
     "evidently",
     "finspace",
     "finspace-data",
     "firehose",
     "fis",
@@ -247,15 +246,14 @@
     "lookoutmetrics",
     "lookoutvision",
     "m2",
     "machinelearning",
     "macie",
     "macie2",
     "managedblockchain",
-    "managedblockchain-query",
     "marketplace-catalog",
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
```

### Comparing `mypy-boto3-connectcases-1.28.16/mypy_boto3_connectcases/paginator.py` & `mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connectcases-1.28.16/mypy_boto3_connectcases/paginator.pyi` & `mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connectcases-1.28.16/mypy_boto3_connectcases/type_defs.py` & `mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_connectcases.type_defs import FieldIdentifierTypeDef
 
-    data: FieldIdentifierTypeDef = ...
+    data: FieldIdentifierTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
-from typing import Any, Dict, List, Mapping, Sequence, Union
+from typing import Any, Dict, List, Mapping, Sequence
 
 from .literals import (
     DomainStatusType,
     FieldNamespaceType,
     FieldTypeType,
     OrderType,
     RelatedItemTypeType,
@@ -37,35 +37,41 @@
 __all__ = (
     "FieldIdentifierTypeDef",
     "FieldErrorTypeDef",
     "GetFieldResponseTypeDef",
     "ResponseMetadataTypeDef",
     "FieldOptionTypeDef",
     "FieldOptionErrorTypeDef",
-    "FieldFilterTypeDef",
+    "FieldIdentifierOutputTypeDef",
     "CaseSummaryTypeDef",
+    "CommentContentOutputTypeDef",
     "CommentContentTypeDef",
     "ContactContentTypeDef",
     "ContactFilterTypeDef",
     "ContactTypeDef",
-    "CreateCaseRequestRequestTypeDef",
     "CreateDomainRequestRequestTypeDef",
     "CreateFieldRequestRequestTypeDef",
     "LayoutConfigurationTypeDef",
     "RequiredFieldTypeDef",
     "DeleteDomainRequestRequestTypeDef",
     "DomainSummaryTypeDef",
+    "RelatedItemEventIncludedDataOutputTypeDef",
     "RelatedItemEventIncludedDataTypeDef",
+    "FieldItemOutputTypeDef",
     "FieldItemTypeDef",
+    "FieldOptionOutputTypeDef",
     "FieldSummaryTypeDef",
     "FieldValueUnionOutputTypeDef",
+    "FieldValueUnionTypeDef",
     "GetCaseEventConfigurationRequestRequestTypeDef",
     "GetDomainRequestRequestTypeDef",
     "GetLayoutRequestRequestTypeDef",
     "GetTemplateRequestRequestTypeDef",
+    "LayoutConfigurationOutputTypeDef",
+    "RequiredFieldOutputTypeDef",
     "LayoutSummaryTypeDef",
     "ListCasesForContactRequestRequestTypeDef",
     "ListDomainsRequestRequestTypeDef",
     "ListFieldOptionsRequestRequestTypeDef",
     "ListFieldsRequestRequestTypeDef",
     "ListLayoutsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
@@ -73,130 +79,107 @@
     "TemplateSummaryTypeDef",
     "PaginatorConfigTypeDef",
     "SortTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateFieldRequestRequestTypeDef",
     "BatchGetFieldRequestRequestTypeDef",
-    "CaseEventIncludedDataOutputTypeDef",
     "CaseEventIncludedDataTypeDef",
     "GetCaseRequestRequestTypeDef",
     "BatchGetFieldResponseTypeDef",
     "CreateCaseResponseTypeDef",
     "CreateDomainResponseTypeDef",
     "CreateFieldResponseTypeDef",
     "CreateLayoutResponseTypeDef",
     "CreateRelatedItemResponseTypeDef",
     "CreateTemplateResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetDomainResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "BatchPutFieldOptionsRequestRequestTypeDef",
-    "ListFieldOptionsResponseTypeDef",
     "BatchPutFieldOptionsResponseTypeDef",
-    "CaseFilterTypeDef",
+    "CaseEventIncludedDataOutputTypeDef",
     "ListCasesForContactResponseTypeDef",
     "RelatedItemContentTypeDef",
     "RelatedItemTypeFilterTypeDef",
     "RelatedItemInputContentTypeDef",
     "CreateTemplateRequestRequestTypeDef",
-    "GetTemplateResponseTypeDef",
     "UpdateTemplateRequestRequestTypeDef",
     "ListDomainsResponseTypeDef",
     "FieldGroupOutputTypeDef",
     "FieldGroupTypeDef",
+    "ListFieldOptionsResponseTypeDef",
     "ListFieldsResponseTypeDef",
     "FieldValueOutputTypeDef",
+    "FieldValueTypeDef",
+    "GetTemplateResponseTypeDef",
     "ListLayoutsResponseTypeDef",
     "ListTemplatesResponseTypeDef",
     "SearchCasesRequestRequestTypeDef",
     "SearchCasesRequestSearchCasesPaginateTypeDef",
-    "EventIncludedDataOutputTypeDef",
     "EventIncludedDataTypeDef",
+    "EventIncludedDataOutputTypeDef",
     "SearchRelatedItemsResponseItemTypeDef",
     "SearchRelatedItemsRequestRequestTypeDef",
     "SearchRelatedItemsRequestSearchRelatedItemsPaginateTypeDef",
     "CreateRelatedItemRequestRequestTypeDef",
     "SectionOutputTypeDef",
     "SectionTypeDef",
-    "FieldValueUnionTypeDef",
     "GetCaseResponseTypeDef",
     "SearchCasesResponseItemTypeDef",
-    "EventBridgeConfigurationOutputTypeDef",
+    "CreateCaseRequestRequestTypeDef",
+    "FieldFilterTypeDef",
+    "UpdateCaseRequestRequestTypeDef",
     "EventBridgeConfigurationTypeDef",
+    "EventBridgeConfigurationOutputTypeDef",
     "SearchRelatedItemsResponseTypeDef",
     "LayoutSectionsOutputTypeDef",
     "LayoutSectionsTypeDef",
-    "FieldValueTypeDef",
-    "UpdateCaseRequestRequestTypeDef",
     "SearchCasesResponseTypeDef",
-    "GetCaseEventConfigurationResponseTypeDef",
-    "EventBridgeConfigurationUnionTypeDef",
+    "CaseFilterTypeDef",
     "PutCaseEventConfigurationRequestRequestTypeDef",
+    "GetCaseEventConfigurationResponseTypeDef",
     "BasicLayoutOutputTypeDef",
     "BasicLayoutTypeDef",
     "LayoutContentOutputTypeDef",
     "LayoutContentTypeDef",
     "GetLayoutResponseTypeDef",
     "CreateLayoutRequestRequestTypeDef",
-    "LayoutContentUnionTypeDef",
     "UpdateLayoutRequestRequestTypeDef",
 )
 
 FieldIdentifierTypeDef = TypedDict(
     "FieldIdentifierTypeDef",
     {
         "id": str,
     },
 )
 
-_RequiredFieldErrorTypeDef = TypedDict(
-    "_RequiredFieldErrorTypeDef",
+FieldErrorTypeDef = TypedDict(
+    "FieldErrorTypeDef",
     {
         "errorCode": str,
         "id": str,
-    },
-)
-_OptionalFieldErrorTypeDef = TypedDict(
-    "_OptionalFieldErrorTypeDef",
-    {
         "message": str,
     },
-    total=False,
 )
 
-
-class FieldErrorTypeDef(_RequiredFieldErrorTypeDef, _OptionalFieldErrorTypeDef):
-    pass
-
-
-_RequiredGetFieldResponseTypeDef = TypedDict(
-    "_RequiredGetFieldResponseTypeDef",
+GetFieldResponseTypeDef = TypedDict(
+    "GetFieldResponseTypeDef",
     {
+        "description": str,
         "fieldArn": str,
         "fieldId": str,
         "name": str,
         "namespace": FieldNamespaceType,
-        "type": FieldTypeType,
-    },
-)
-_OptionalGetFieldResponseTypeDef = TypedDict(
-    "_OptionalGetFieldResponseTypeDef",
-    {
-        "description": str,
         "tags": Dict[str, str],
+        "type": FieldTypeType,
     },
-    total=False,
 )
 
-
-class GetFieldResponseTypeDef(_RequiredGetFieldResponseTypeDef, _OptionalGetFieldResponseTypeDef):
-    pass
-
-
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -218,35 +201,37 @@
     {
         "errorCode": str,
         "message": str,
         "value": str,
     },
 )
 
-FieldFilterTypeDef = TypedDict(
-    "FieldFilterTypeDef",
+FieldIdentifierOutputTypeDef = TypedDict(
+    "FieldIdentifierOutputTypeDef",
     {
-        "contains": "FieldValueTypeDef",
-        "equalTo": "FieldValueTypeDef",
-        "greaterThan": "FieldValueTypeDef",
-        "greaterThanOrEqualTo": "FieldValueTypeDef",
-        "lessThan": "FieldValueTypeDef",
-        "lessThanOrEqualTo": "FieldValueTypeDef",
+        "id": str,
     },
-    total=False,
 )
 
 CaseSummaryTypeDef = TypedDict(
     "CaseSummaryTypeDef",
     {
         "caseId": str,
         "templateId": str,
     },
 )
 
+CommentContentOutputTypeDef = TypedDict(
+    "CommentContentOutputTypeDef",
+    {
+        "body": str,
+        "contentType": Literal["Text/Plain"],
+    },
+)
+
 CommentContentTypeDef = TypedDict(
     "CommentContentTypeDef",
     {
         "body": str,
         "contentType": Literal["Text/Plain"],
     },
 )
@@ -272,37 +257,14 @@
 ContactTypeDef = TypedDict(
     "ContactTypeDef",
     {
         "contactArn": str,
     },
 )
 
-_RequiredCreateCaseRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateCaseRequestRequestTypeDef",
-    {
-        "domainId": str,
-        "fields": Sequence["FieldValueUnionTypeDef"],
-        "templateId": str,
-    },
-)
-_OptionalCreateCaseRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateCaseRequestRequestTypeDef",
-    {
-        "clientToken": str,
-    },
-    total=False,
-)
-
-
-class CreateCaseRequestRequestTypeDef(
-    _RequiredCreateCaseRequestRequestTypeDef, _OptionalCreateCaseRequestRequestTypeDef
-):
-    pass
-
-
 CreateDomainRequestRequestTypeDef = TypedDict(
     "CreateDomainRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 
@@ -356,28 +318,51 @@
     {
         "domainArn": str,
         "domainId": str,
         "name": str,
     },
 )
 
+RelatedItemEventIncludedDataOutputTypeDef = TypedDict(
+    "RelatedItemEventIncludedDataOutputTypeDef",
+    {
+        "includeContent": bool,
+    },
+)
+
 RelatedItemEventIncludedDataTypeDef = TypedDict(
     "RelatedItemEventIncludedDataTypeDef",
     {
         "includeContent": bool,
     },
 )
 
+FieldItemOutputTypeDef = TypedDict(
+    "FieldItemOutputTypeDef",
+    {
+        "id": str,
+    },
+)
+
 FieldItemTypeDef = TypedDict(
     "FieldItemTypeDef",
     {
         "id": str,
     },
 )
 
+FieldOptionOutputTypeDef = TypedDict(
+    "FieldOptionOutputTypeDef",
+    {
+        "active": bool,
+        "name": str,
+        "value": str,
+    },
+)
+
 FieldSummaryTypeDef = TypedDict(
     "FieldSummaryTypeDef",
     {
         "fieldArn": str,
         "fieldId": str,
         "name": str,
         "namespace": FieldNamespaceType,
@@ -389,14 +374,24 @@
     "FieldValueUnionOutputTypeDef",
     {
         "booleanValue": bool,
         "doubleValue": float,
         "emptyValue": Dict[str, Any],
         "stringValue": str,
     },
+)
+
+FieldValueUnionTypeDef = TypedDict(
+    "FieldValueUnionTypeDef",
+    {
+        "booleanValue": bool,
+        "doubleValue": float,
+        "emptyValue": Mapping[str, Any],
+        "stringValue": str,
+    },
     total=False,
 )
 
 GetCaseEventConfigurationRequestRequestTypeDef = TypedDict(
     "GetCaseEventConfigurationRequestRequestTypeDef",
     {
         "domainId": str,
@@ -422,14 +417,28 @@
     "GetTemplateRequestRequestTypeDef",
     {
         "domainId": str,
         "templateId": str,
     },
 )
 
+LayoutConfigurationOutputTypeDef = TypedDict(
+    "LayoutConfigurationOutputTypeDef",
+    {
+        "defaultLayout": str,
+    },
+)
+
+RequiredFieldOutputTypeDef = TypedDict(
+    "RequiredFieldOutputTypeDef",
+    {
+        "fieldId": str,
+    },
+)
+
 LayoutSummaryTypeDef = TypedDict(
     "LayoutSummaryTypeDef",
     {
         "layoutArn": str,
         "layoutId": str,
         "name": str,
     },
@@ -637,21 +646,14 @@
     "BatchGetFieldRequestRequestTypeDef",
     {
         "domainId": str,
         "fields": Sequence[FieldIdentifierTypeDef],
     },
 )
 
-CaseEventIncludedDataOutputTypeDef = TypedDict(
-    "CaseEventIncludedDataOutputTypeDef",
-    {
-        "fields": List[FieldIdentifierTypeDef],
-    },
-)
-
 CaseEventIncludedDataTypeDef = TypedDict(
     "CaseEventIncludedDataTypeDef",
     {
         "fields": Sequence[FieldIdentifierTypeDef],
     },
 )
 
@@ -775,58 +777,44 @@
     {
         "domainId": str,
         "fieldId": str,
         "options": Sequence[FieldOptionTypeDef],
     },
 )
 
-ListFieldOptionsResponseTypeDef = TypedDict(
-    "ListFieldOptionsResponseTypeDef",
-    {
-        "nextToken": str,
-        "options": List[FieldOptionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 BatchPutFieldOptionsResponseTypeDef = TypedDict(
     "BatchPutFieldOptionsResponseTypeDef",
     {
         "errors": List[FieldOptionErrorTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CaseFilterTypeDef = TypedDict(
-    "CaseFilterTypeDef",
+CaseEventIncludedDataOutputTypeDef = TypedDict(
+    "CaseEventIncludedDataOutputTypeDef",
     {
-        "andAll": Sequence[Dict[str, Any]],
-        "field": FieldFilterTypeDef,
-        "not": Dict[str, Any],
-        "orAll": Sequence[Dict[str, Any]],
+        "fields": List[FieldIdentifierOutputTypeDef],
     },
-    total=False,
 )
 
 ListCasesForContactResponseTypeDef = TypedDict(
     "ListCasesForContactResponseTypeDef",
     {
         "cases": List[CaseSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RelatedItemContentTypeDef = TypedDict(
     "RelatedItemContentTypeDef",
     {
-        "comment": CommentContentTypeDef,
+        "comment": CommentContentOutputTypeDef,
         "contact": ContactContentTypeDef,
     },
-    total=False,
 )
 
 RelatedItemTypeFilterTypeDef = TypedDict(
     "RelatedItemTypeFilterTypeDef",
     {
         "comment": Mapping[str, Any],
         "contact": ContactFilterTypeDef,
@@ -864,29 +852,14 @@
 
 class CreateTemplateRequestRequestTypeDef(
     _RequiredCreateTemplateRequestRequestTypeDef, _OptionalCreateTemplateRequestRequestTypeDef
 ):
     pass
 
 
-GetTemplateResponseTypeDef = TypedDict(
-    "GetTemplateResponseTypeDef",
-    {
-        "description": str,
-        "layoutConfiguration": LayoutConfigurationTypeDef,
-        "name": str,
-        "requiredFields": List[RequiredFieldTypeDef],
-        "status": TemplateStatusType,
-        "tags": Dict[str, str],
-        "templateArn": str,
-        "templateId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredUpdateTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateTemplateRequestRequestTypeDef",
     {
         "domainId": str,
         "templateId": str,
     },
 )
@@ -914,33 +887,22 @@
     {
         "domains": List[DomainSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredFieldGroupOutputTypeDef = TypedDict(
-    "_RequiredFieldGroupOutputTypeDef",
-    {
-        "fields": List[FieldItemTypeDef],
-    },
-)
-_OptionalFieldGroupOutputTypeDef = TypedDict(
-    "_OptionalFieldGroupOutputTypeDef",
+FieldGroupOutputTypeDef = TypedDict(
+    "FieldGroupOutputTypeDef",
     {
+        "fields": List[FieldItemOutputTypeDef],
         "name": str,
     },
-    total=False,
 )
 
-
-class FieldGroupOutputTypeDef(_RequiredFieldGroupOutputTypeDef, _OptionalFieldGroupOutputTypeDef):
-    pass
-
-
 _RequiredFieldGroupTypeDef = TypedDict(
     "_RequiredFieldGroupTypeDef",
     {
         "fields": Sequence[FieldItemTypeDef],
     },
 )
 _OptionalFieldGroupTypeDef = TypedDict(
@@ -952,14 +914,23 @@
 )
 
 
 class FieldGroupTypeDef(_RequiredFieldGroupTypeDef, _OptionalFieldGroupTypeDef):
     pass
 
 
+ListFieldOptionsResponseTypeDef = TypedDict(
+    "ListFieldOptionsResponseTypeDef",
+    {
+        "nextToken": str,
+        "options": List[FieldOptionOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListFieldsResponseTypeDef = TypedDict(
     "ListFieldsResponseTypeDef",
     {
         "fields": List[FieldSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -969,14 +940,37 @@
     "FieldValueOutputTypeDef",
     {
         "id": str,
         "value": FieldValueUnionOutputTypeDef,
     },
 )
 
+FieldValueTypeDef = TypedDict(
+    "FieldValueTypeDef",
+    {
+        "id": str,
+        "value": FieldValueUnionTypeDef,
+    },
+)
+
+GetTemplateResponseTypeDef = TypedDict(
+    "GetTemplateResponseTypeDef",
+    {
+        "description": str,
+        "layoutConfiguration": LayoutConfigurationOutputTypeDef,
+        "name": str,
+        "requiredFields": List[RequiredFieldOutputTypeDef],
+        "status": TemplateStatusType,
+        "tags": Dict[str, str],
+        "templateArn": str,
+        "templateId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListLayoutsResponseTypeDef = TypedDict(
     "ListLayoutsResponseTypeDef",
     {
         "layouts": List[LayoutSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1039,56 +1033,42 @@
 class SearchCasesRequestSearchCasesPaginateTypeDef(
     _RequiredSearchCasesRequestSearchCasesPaginateTypeDef,
     _OptionalSearchCasesRequestSearchCasesPaginateTypeDef,
 ):
     pass
 
 
-EventIncludedDataOutputTypeDef = TypedDict(
-    "EventIncludedDataOutputTypeDef",
+EventIncludedDataTypeDef = TypedDict(
+    "EventIncludedDataTypeDef",
     {
-        "caseData": CaseEventIncludedDataOutputTypeDef,
+        "caseData": CaseEventIncludedDataTypeDef,
         "relatedItemData": RelatedItemEventIncludedDataTypeDef,
     },
     total=False,
 )
 
-EventIncludedDataTypeDef = TypedDict(
-    "EventIncludedDataTypeDef",
+EventIncludedDataOutputTypeDef = TypedDict(
+    "EventIncludedDataOutputTypeDef",
     {
-        "caseData": CaseEventIncludedDataTypeDef,
-        "relatedItemData": RelatedItemEventIncludedDataTypeDef,
+        "caseData": CaseEventIncludedDataOutputTypeDef,
+        "relatedItemData": RelatedItemEventIncludedDataOutputTypeDef,
     },
-    total=False,
 )
 
-_RequiredSearchRelatedItemsResponseItemTypeDef = TypedDict(
-    "_RequiredSearchRelatedItemsResponseItemTypeDef",
+SearchRelatedItemsResponseItemTypeDef = TypedDict(
+    "SearchRelatedItemsResponseItemTypeDef",
     {
         "associationTime": datetime,
         "content": RelatedItemContentTypeDef,
         "relatedItemId": str,
-        "type": RelatedItemTypeType,
-    },
-)
-_OptionalSearchRelatedItemsResponseItemTypeDef = TypedDict(
-    "_OptionalSearchRelatedItemsResponseItemTypeDef",
-    {
         "tags": Dict[str, str],
+        "type": RelatedItemTypeType,
     },
-    total=False,
 )
 
-
-class SearchRelatedItemsResponseItemTypeDef(
-    _RequiredSearchRelatedItemsResponseItemTypeDef, _OptionalSearchRelatedItemsResponseItemTypeDef
-):
-    pass
-
-
 _RequiredSearchRelatedItemsRequestRequestTypeDef = TypedDict(
     "_RequiredSearchRelatedItemsRequestRequestTypeDef",
     {
         "caseId": str,
         "domainId": str,
     },
 )
@@ -1145,81 +1125,90 @@
 )
 
 SectionOutputTypeDef = TypedDict(
     "SectionOutputTypeDef",
     {
         "fieldGroup": FieldGroupOutputTypeDef,
     },
-    total=False,
 )
 
 SectionTypeDef = TypedDict(
     "SectionTypeDef",
     {
         "fieldGroup": FieldGroupTypeDef,
     },
     total=False,
 )
 
-FieldValueUnionTypeDef = Union["FieldValueTypeDef", FieldValueOutputTypeDef]
 GetCaseResponseTypeDef = TypedDict(
     "GetCaseResponseTypeDef",
     {
         "fields": List[FieldValueOutputTypeDef],
         "nextToken": str,
         "tags": Dict[str, str],
         "templateId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredSearchCasesResponseItemTypeDef = TypedDict(
-    "_RequiredSearchCasesResponseItemTypeDef",
+SearchCasesResponseItemTypeDef = TypedDict(
+    "SearchCasesResponseItemTypeDef",
     {
         "caseId": str,
         "fields": List[FieldValueOutputTypeDef],
+        "tags": Dict[str, str],
         "templateId": str,
     },
 )
-_OptionalSearchCasesResponseItemTypeDef = TypedDict(
-    "_OptionalSearchCasesResponseItemTypeDef",
+
+_RequiredCreateCaseRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateCaseRequestRequestTypeDef",
     {
-        "tags": Dict[str, str],
+        "domainId": str,
+        "fields": Sequence[FieldValueTypeDef],
+        "templateId": str,
+    },
+)
+_OptionalCreateCaseRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateCaseRequestRequestTypeDef",
+    {
+        "clientToken": str,
     },
     total=False,
 )
 
 
-class SearchCasesResponseItemTypeDef(
-    _RequiredSearchCasesResponseItemTypeDef, _OptionalSearchCasesResponseItemTypeDef
+class CreateCaseRequestRequestTypeDef(
+    _RequiredCreateCaseRequestRequestTypeDef, _OptionalCreateCaseRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredEventBridgeConfigurationOutputTypeDef = TypedDict(
-    "_RequiredEventBridgeConfigurationOutputTypeDef",
+FieldFilterTypeDef = TypedDict(
+    "FieldFilterTypeDef",
     {
-        "enabled": bool,
+        "contains": FieldValueTypeDef,
+        "equalTo": FieldValueTypeDef,
+        "greaterThan": FieldValueTypeDef,
+        "greaterThanOrEqualTo": FieldValueTypeDef,
+        "lessThan": FieldValueTypeDef,
+        "lessThanOrEqualTo": FieldValueTypeDef,
     },
+    total=False,
 )
-_OptionalEventBridgeConfigurationOutputTypeDef = TypedDict(
-    "_OptionalEventBridgeConfigurationOutputTypeDef",
+
+UpdateCaseRequestRequestTypeDef = TypedDict(
+    "UpdateCaseRequestRequestTypeDef",
     {
-        "includedData": EventIncludedDataOutputTypeDef,
+        "caseId": str,
+        "domainId": str,
+        "fields": Sequence[FieldValueTypeDef],
     },
-    total=False,
 )
 
-
-class EventBridgeConfigurationOutputTypeDef(
-    _RequiredEventBridgeConfigurationOutputTypeDef, _OptionalEventBridgeConfigurationOutputTypeDef
-):
-    pass
-
-
 _RequiredEventBridgeConfigurationTypeDef = TypedDict(
     "_RequiredEventBridgeConfigurationTypeDef",
     {
         "enabled": bool,
     },
 )
 _OptionalEventBridgeConfigurationTypeDef = TypedDict(
@@ -1233,91 +1222,88 @@
 
 class EventBridgeConfigurationTypeDef(
     _RequiredEventBridgeConfigurationTypeDef, _OptionalEventBridgeConfigurationTypeDef
 ):
     pass
 
 
+EventBridgeConfigurationOutputTypeDef = TypedDict(
+    "EventBridgeConfigurationOutputTypeDef",
+    {
+        "enabled": bool,
+        "includedData": EventIncludedDataOutputTypeDef,
+    },
+)
+
 SearchRelatedItemsResponseTypeDef = TypedDict(
     "SearchRelatedItemsResponseTypeDef",
     {
         "nextToken": str,
         "relatedItems": List[SearchRelatedItemsResponseItemTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LayoutSectionsOutputTypeDef = TypedDict(
     "LayoutSectionsOutputTypeDef",
     {
         "sections": List[SectionOutputTypeDef],
     },
-    total=False,
 )
 
 LayoutSectionsTypeDef = TypedDict(
     "LayoutSectionsTypeDef",
     {
         "sections": Sequence[SectionTypeDef],
     },
     total=False,
 )
 
-FieldValueTypeDef = TypedDict(
-    "FieldValueTypeDef",
-    {
-        "id": str,
-        "value": FieldValueUnionTypeDef,
-    },
-)
-
-UpdateCaseRequestRequestTypeDef = TypedDict(
-    "UpdateCaseRequestRequestTypeDef",
-    {
-        "caseId": str,
-        "domainId": str,
-        "fields": Sequence[FieldValueUnionTypeDef],
-    },
-)
-
 SearchCasesResponseTypeDef = TypedDict(
     "SearchCasesResponseTypeDef",
     {
         "cases": List[SearchCasesResponseItemTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetCaseEventConfigurationResponseTypeDef = TypedDict(
-    "GetCaseEventConfigurationResponseTypeDef",
+CaseFilterTypeDef = TypedDict(
+    "CaseFilterTypeDef",
     {
-        "eventBridge": EventBridgeConfigurationOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "andAll": Sequence[Dict[str, Any]],
+        "field": FieldFilterTypeDef,
+        "not": Dict[str, Any],
+        "orAll": Sequence[Dict[str, Any]],
     },
+    total=False,
 )
 
-EventBridgeConfigurationUnionTypeDef = Union[
-    EventBridgeConfigurationTypeDef, EventBridgeConfigurationOutputTypeDef
-]
 PutCaseEventConfigurationRequestRequestTypeDef = TypedDict(
     "PutCaseEventConfigurationRequestRequestTypeDef",
     {
         "domainId": str,
         "eventBridge": EventBridgeConfigurationTypeDef,
     },
 )
 
+GetCaseEventConfigurationResponseTypeDef = TypedDict(
+    "GetCaseEventConfigurationResponseTypeDef",
+    {
+        "eventBridge": EventBridgeConfigurationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 BasicLayoutOutputTypeDef = TypedDict(
     "BasicLayoutOutputTypeDef",
     {
         "moreInfo": LayoutSectionsOutputTypeDef,
         "topPanel": LayoutSectionsOutputTypeDef,
     },
-    total=False,
 )
 
 BasicLayoutTypeDef = TypedDict(
     "BasicLayoutTypeDef",
     {
         "moreInfo": LayoutSectionsTypeDef,
         "topPanel": LayoutSectionsTypeDef,
@@ -1326,15 +1312,14 @@
 )
 
 LayoutContentOutputTypeDef = TypedDict(
     "LayoutContentOutputTypeDef",
     {
         "basic": BasicLayoutOutputTypeDef,
     },
-    total=False,
 )
 
 LayoutContentTypeDef = TypedDict(
     "LayoutContentTypeDef",
     {
         "basic": BasicLayoutTypeDef,
     },
@@ -1358,15 +1343,14 @@
     {
         "content": LayoutContentTypeDef,
         "domainId": str,
         "name": str,
     },
 )
 
-LayoutContentUnionTypeDef = Union[LayoutContentTypeDef, LayoutContentOutputTypeDef]
 _RequiredUpdateLayoutRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateLayoutRequestRequestTypeDef",
     {
         "domainId": str,
         "layoutId": str,
     },
 )
```

### Comparing `mypy-boto3-connectcases-1.28.16/mypy_boto3_connectcases/type_defs.pyi` & `mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_connectcases.type_defs import FieldIdentifierTypeDef
 
-    data: FieldIdentifierTypeDef = ...
+    data: FieldIdentifierTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
-from typing import Any, Dict, List, Mapping, Sequence, Union
+from typing import Any, Dict, List, Mapping, Sequence
 
 from .literals import (
     DomainStatusType,
     FieldNamespaceType,
     FieldTypeType,
     OrderType,
     RelatedItemTypeType,
@@ -36,35 +36,41 @@
 __all__ = (
     "FieldIdentifierTypeDef",
     "FieldErrorTypeDef",
     "GetFieldResponseTypeDef",
     "ResponseMetadataTypeDef",
     "FieldOptionTypeDef",
     "FieldOptionErrorTypeDef",
-    "FieldFilterTypeDef",
+    "FieldIdentifierOutputTypeDef",
     "CaseSummaryTypeDef",
+    "CommentContentOutputTypeDef",
     "CommentContentTypeDef",
     "ContactContentTypeDef",
     "ContactFilterTypeDef",
     "ContactTypeDef",
-    "CreateCaseRequestRequestTypeDef",
     "CreateDomainRequestRequestTypeDef",
     "CreateFieldRequestRequestTypeDef",
     "LayoutConfigurationTypeDef",
     "RequiredFieldTypeDef",
     "DeleteDomainRequestRequestTypeDef",
     "DomainSummaryTypeDef",
+    "RelatedItemEventIncludedDataOutputTypeDef",
     "RelatedItemEventIncludedDataTypeDef",
+    "FieldItemOutputTypeDef",
     "FieldItemTypeDef",
+    "FieldOptionOutputTypeDef",
     "FieldSummaryTypeDef",
     "FieldValueUnionOutputTypeDef",
+    "FieldValueUnionTypeDef",
     "GetCaseEventConfigurationRequestRequestTypeDef",
     "GetDomainRequestRequestTypeDef",
     "GetLayoutRequestRequestTypeDef",
     "GetTemplateRequestRequestTypeDef",
+    "LayoutConfigurationOutputTypeDef",
+    "RequiredFieldOutputTypeDef",
     "LayoutSummaryTypeDef",
     "ListCasesForContactRequestRequestTypeDef",
     "ListDomainsRequestRequestTypeDef",
     "ListFieldOptionsRequestRequestTypeDef",
     "ListFieldsRequestRequestTypeDef",
     "ListLayoutsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
@@ -72,126 +78,107 @@
     "TemplateSummaryTypeDef",
     "PaginatorConfigTypeDef",
     "SortTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateFieldRequestRequestTypeDef",
     "BatchGetFieldRequestRequestTypeDef",
-    "CaseEventIncludedDataOutputTypeDef",
     "CaseEventIncludedDataTypeDef",
     "GetCaseRequestRequestTypeDef",
     "BatchGetFieldResponseTypeDef",
     "CreateCaseResponseTypeDef",
     "CreateDomainResponseTypeDef",
     "CreateFieldResponseTypeDef",
     "CreateLayoutResponseTypeDef",
     "CreateRelatedItemResponseTypeDef",
     "CreateTemplateResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetDomainResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "BatchPutFieldOptionsRequestRequestTypeDef",
-    "ListFieldOptionsResponseTypeDef",
     "BatchPutFieldOptionsResponseTypeDef",
-    "CaseFilterTypeDef",
+    "CaseEventIncludedDataOutputTypeDef",
     "ListCasesForContactResponseTypeDef",
     "RelatedItemContentTypeDef",
     "RelatedItemTypeFilterTypeDef",
     "RelatedItemInputContentTypeDef",
     "CreateTemplateRequestRequestTypeDef",
-    "GetTemplateResponseTypeDef",
     "UpdateTemplateRequestRequestTypeDef",
     "ListDomainsResponseTypeDef",
     "FieldGroupOutputTypeDef",
     "FieldGroupTypeDef",
+    "ListFieldOptionsResponseTypeDef",
     "ListFieldsResponseTypeDef",
     "FieldValueOutputTypeDef",
+    "FieldValueTypeDef",
+    "GetTemplateResponseTypeDef",
     "ListLayoutsResponseTypeDef",
     "ListTemplatesResponseTypeDef",
     "SearchCasesRequestRequestTypeDef",
     "SearchCasesRequestSearchCasesPaginateTypeDef",
-    "EventIncludedDataOutputTypeDef",
     "EventIncludedDataTypeDef",
+    "EventIncludedDataOutputTypeDef",
     "SearchRelatedItemsResponseItemTypeDef",
     "SearchRelatedItemsRequestRequestTypeDef",
     "SearchRelatedItemsRequestSearchRelatedItemsPaginateTypeDef",
     "CreateRelatedItemRequestRequestTypeDef",
     "SectionOutputTypeDef",
     "SectionTypeDef",
-    "FieldValueUnionTypeDef",
     "GetCaseResponseTypeDef",
     "SearchCasesResponseItemTypeDef",
-    "EventBridgeConfigurationOutputTypeDef",
+    "CreateCaseRequestRequestTypeDef",
+    "FieldFilterTypeDef",
+    "UpdateCaseRequestRequestTypeDef",
     "EventBridgeConfigurationTypeDef",
+    "EventBridgeConfigurationOutputTypeDef",
     "SearchRelatedItemsResponseTypeDef",
     "LayoutSectionsOutputTypeDef",
     "LayoutSectionsTypeDef",
-    "FieldValueTypeDef",
-    "UpdateCaseRequestRequestTypeDef",
     "SearchCasesResponseTypeDef",
-    "GetCaseEventConfigurationResponseTypeDef",
-    "EventBridgeConfigurationUnionTypeDef",
+    "CaseFilterTypeDef",
     "PutCaseEventConfigurationRequestRequestTypeDef",
+    "GetCaseEventConfigurationResponseTypeDef",
     "BasicLayoutOutputTypeDef",
     "BasicLayoutTypeDef",
     "LayoutContentOutputTypeDef",
     "LayoutContentTypeDef",
     "GetLayoutResponseTypeDef",
     "CreateLayoutRequestRequestTypeDef",
-    "LayoutContentUnionTypeDef",
     "UpdateLayoutRequestRequestTypeDef",
 )
 
 FieldIdentifierTypeDef = TypedDict(
     "FieldIdentifierTypeDef",
     {
         "id": str,
     },
 )
 
-_RequiredFieldErrorTypeDef = TypedDict(
-    "_RequiredFieldErrorTypeDef",
+FieldErrorTypeDef = TypedDict(
+    "FieldErrorTypeDef",
     {
         "errorCode": str,
         "id": str,
-    },
-)
-_OptionalFieldErrorTypeDef = TypedDict(
-    "_OptionalFieldErrorTypeDef",
-    {
         "message": str,
     },
-    total=False,
 )
 
-class FieldErrorTypeDef(_RequiredFieldErrorTypeDef, _OptionalFieldErrorTypeDef):
-    pass
-
-_RequiredGetFieldResponseTypeDef = TypedDict(
-    "_RequiredGetFieldResponseTypeDef",
+GetFieldResponseTypeDef = TypedDict(
+    "GetFieldResponseTypeDef",
     {
+        "description": str,
         "fieldArn": str,
         "fieldId": str,
         "name": str,
         "namespace": FieldNamespaceType,
-        "type": FieldTypeType,
-    },
-)
-_OptionalGetFieldResponseTypeDef = TypedDict(
-    "_OptionalGetFieldResponseTypeDef",
-    {
-        "description": str,
         "tags": Dict[str, str],
+        "type": FieldTypeType,
     },
-    total=False,
 )
 
-class GetFieldResponseTypeDef(_RequiredGetFieldResponseTypeDef, _OptionalGetFieldResponseTypeDef):
-    pass
-
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -213,35 +200,37 @@
     {
         "errorCode": str,
         "message": str,
         "value": str,
     },
 )
 
-FieldFilterTypeDef = TypedDict(
-    "FieldFilterTypeDef",
+FieldIdentifierOutputTypeDef = TypedDict(
+    "FieldIdentifierOutputTypeDef",
     {
-        "contains": "FieldValueTypeDef",
-        "equalTo": "FieldValueTypeDef",
-        "greaterThan": "FieldValueTypeDef",
-        "greaterThanOrEqualTo": "FieldValueTypeDef",
-        "lessThan": "FieldValueTypeDef",
-        "lessThanOrEqualTo": "FieldValueTypeDef",
+        "id": str,
     },
-    total=False,
 )
 
 CaseSummaryTypeDef = TypedDict(
     "CaseSummaryTypeDef",
     {
         "caseId": str,
         "templateId": str,
     },
 )
 
+CommentContentOutputTypeDef = TypedDict(
+    "CommentContentOutputTypeDef",
+    {
+        "body": str,
+        "contentType": Literal["Text/Plain"],
+    },
+)
+
 CommentContentTypeDef = TypedDict(
     "CommentContentTypeDef",
     {
         "body": str,
         "contentType": Literal["Text/Plain"],
     },
 )
@@ -267,35 +256,14 @@
 ContactTypeDef = TypedDict(
     "ContactTypeDef",
     {
         "contactArn": str,
     },
 )
 
-_RequiredCreateCaseRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateCaseRequestRequestTypeDef",
-    {
-        "domainId": str,
-        "fields": Sequence["FieldValueUnionTypeDef"],
-        "templateId": str,
-    },
-)
-_OptionalCreateCaseRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateCaseRequestRequestTypeDef",
-    {
-        "clientToken": str,
-    },
-    total=False,
-)
-
-class CreateCaseRequestRequestTypeDef(
-    _RequiredCreateCaseRequestRequestTypeDef, _OptionalCreateCaseRequestRequestTypeDef
-):
-    pass
-
 CreateDomainRequestRequestTypeDef = TypedDict(
     "CreateDomainRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 
@@ -347,28 +315,51 @@
     {
         "domainArn": str,
         "domainId": str,
         "name": str,
     },
 )
 
+RelatedItemEventIncludedDataOutputTypeDef = TypedDict(
+    "RelatedItemEventIncludedDataOutputTypeDef",
+    {
+        "includeContent": bool,
+    },
+)
+
 RelatedItemEventIncludedDataTypeDef = TypedDict(
     "RelatedItemEventIncludedDataTypeDef",
     {
         "includeContent": bool,
     },
 )
 
+FieldItemOutputTypeDef = TypedDict(
+    "FieldItemOutputTypeDef",
+    {
+        "id": str,
+    },
+)
+
 FieldItemTypeDef = TypedDict(
     "FieldItemTypeDef",
     {
         "id": str,
     },
 )
 
+FieldOptionOutputTypeDef = TypedDict(
+    "FieldOptionOutputTypeDef",
+    {
+        "active": bool,
+        "name": str,
+        "value": str,
+    },
+)
+
 FieldSummaryTypeDef = TypedDict(
     "FieldSummaryTypeDef",
     {
         "fieldArn": str,
         "fieldId": str,
         "name": str,
         "namespace": FieldNamespaceType,
@@ -380,14 +371,24 @@
     "FieldValueUnionOutputTypeDef",
     {
         "booleanValue": bool,
         "doubleValue": float,
         "emptyValue": Dict[str, Any],
         "stringValue": str,
     },
+)
+
+FieldValueUnionTypeDef = TypedDict(
+    "FieldValueUnionTypeDef",
+    {
+        "booleanValue": bool,
+        "doubleValue": float,
+        "emptyValue": Mapping[str, Any],
+        "stringValue": str,
+    },
     total=False,
 )
 
 GetCaseEventConfigurationRequestRequestTypeDef = TypedDict(
     "GetCaseEventConfigurationRequestRequestTypeDef",
     {
         "domainId": str,
@@ -413,14 +414,28 @@
     "GetTemplateRequestRequestTypeDef",
     {
         "domainId": str,
         "templateId": str,
     },
 )
 
+LayoutConfigurationOutputTypeDef = TypedDict(
+    "LayoutConfigurationOutputTypeDef",
+    {
+        "defaultLayout": str,
+    },
+)
+
+RequiredFieldOutputTypeDef = TypedDict(
+    "RequiredFieldOutputTypeDef",
+    {
+        "fieldId": str,
+    },
+)
+
 LayoutSummaryTypeDef = TypedDict(
     "LayoutSummaryTypeDef",
     {
         "layoutArn": str,
         "layoutId": str,
         "name": str,
     },
@@ -616,21 +631,14 @@
     "BatchGetFieldRequestRequestTypeDef",
     {
         "domainId": str,
         "fields": Sequence[FieldIdentifierTypeDef],
     },
 )
 
-CaseEventIncludedDataOutputTypeDef = TypedDict(
-    "CaseEventIncludedDataOutputTypeDef",
-    {
-        "fields": List[FieldIdentifierTypeDef],
-    },
-)
-
 CaseEventIncludedDataTypeDef = TypedDict(
     "CaseEventIncludedDataTypeDef",
     {
         "fields": Sequence[FieldIdentifierTypeDef],
     },
 )
 
@@ -752,58 +760,44 @@
     {
         "domainId": str,
         "fieldId": str,
         "options": Sequence[FieldOptionTypeDef],
     },
 )
 
-ListFieldOptionsResponseTypeDef = TypedDict(
-    "ListFieldOptionsResponseTypeDef",
-    {
-        "nextToken": str,
-        "options": List[FieldOptionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 BatchPutFieldOptionsResponseTypeDef = TypedDict(
     "BatchPutFieldOptionsResponseTypeDef",
     {
         "errors": List[FieldOptionErrorTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CaseFilterTypeDef = TypedDict(
-    "CaseFilterTypeDef",
+CaseEventIncludedDataOutputTypeDef = TypedDict(
+    "CaseEventIncludedDataOutputTypeDef",
     {
-        "andAll": Sequence[Dict[str, Any]],
-        "field": FieldFilterTypeDef,
-        "not": Dict[str, Any],
-        "orAll": Sequence[Dict[str, Any]],
+        "fields": List[FieldIdentifierOutputTypeDef],
     },
-    total=False,
 )
 
 ListCasesForContactResponseTypeDef = TypedDict(
     "ListCasesForContactResponseTypeDef",
     {
         "cases": List[CaseSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RelatedItemContentTypeDef = TypedDict(
     "RelatedItemContentTypeDef",
     {
-        "comment": CommentContentTypeDef,
+        "comment": CommentContentOutputTypeDef,
         "contact": ContactContentTypeDef,
     },
-    total=False,
 )
 
 RelatedItemTypeFilterTypeDef = TypedDict(
     "RelatedItemTypeFilterTypeDef",
     {
         "comment": Mapping[str, Any],
         "contact": ContactFilterTypeDef,
@@ -839,29 +833,14 @@
 )
 
 class CreateTemplateRequestRequestTypeDef(
     _RequiredCreateTemplateRequestRequestTypeDef, _OptionalCreateTemplateRequestRequestTypeDef
 ):
     pass
 
-GetTemplateResponseTypeDef = TypedDict(
-    "GetTemplateResponseTypeDef",
-    {
-        "description": str,
-        "layoutConfiguration": LayoutConfigurationTypeDef,
-        "name": str,
-        "requiredFields": List[RequiredFieldTypeDef],
-        "status": TemplateStatusType,
-        "tags": Dict[str, str],
-        "templateArn": str,
-        "templateId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredUpdateTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateTemplateRequestRequestTypeDef",
     {
         "domainId": str,
         "templateId": str,
     },
 )
@@ -887,31 +866,22 @@
     {
         "domains": List[DomainSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredFieldGroupOutputTypeDef = TypedDict(
-    "_RequiredFieldGroupOutputTypeDef",
-    {
-        "fields": List[FieldItemTypeDef],
-    },
-)
-_OptionalFieldGroupOutputTypeDef = TypedDict(
-    "_OptionalFieldGroupOutputTypeDef",
+FieldGroupOutputTypeDef = TypedDict(
+    "FieldGroupOutputTypeDef",
     {
+        "fields": List[FieldItemOutputTypeDef],
         "name": str,
     },
-    total=False,
 )
 
-class FieldGroupOutputTypeDef(_RequiredFieldGroupOutputTypeDef, _OptionalFieldGroupOutputTypeDef):
-    pass
-
 _RequiredFieldGroupTypeDef = TypedDict(
     "_RequiredFieldGroupTypeDef",
     {
         "fields": Sequence[FieldItemTypeDef],
     },
 )
 _OptionalFieldGroupTypeDef = TypedDict(
@@ -921,14 +891,23 @@
     },
     total=False,
 )
 
 class FieldGroupTypeDef(_RequiredFieldGroupTypeDef, _OptionalFieldGroupTypeDef):
     pass
 
+ListFieldOptionsResponseTypeDef = TypedDict(
+    "ListFieldOptionsResponseTypeDef",
+    {
+        "nextToken": str,
+        "options": List[FieldOptionOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListFieldsResponseTypeDef = TypedDict(
     "ListFieldsResponseTypeDef",
     {
         "fields": List[FieldSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -938,14 +917,37 @@
     "FieldValueOutputTypeDef",
     {
         "id": str,
         "value": FieldValueUnionOutputTypeDef,
     },
 )
 
+FieldValueTypeDef = TypedDict(
+    "FieldValueTypeDef",
+    {
+        "id": str,
+        "value": FieldValueUnionTypeDef,
+    },
+)
+
+GetTemplateResponseTypeDef = TypedDict(
+    "GetTemplateResponseTypeDef",
+    {
+        "description": str,
+        "layoutConfiguration": LayoutConfigurationOutputTypeDef,
+        "name": str,
+        "requiredFields": List[RequiredFieldOutputTypeDef],
+        "status": TemplateStatusType,
+        "tags": Dict[str, str],
+        "templateArn": str,
+        "templateId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListLayoutsResponseTypeDef = TypedDict(
     "ListLayoutsResponseTypeDef",
     {
         "layouts": List[LayoutSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1004,54 +1006,42 @@
 
 class SearchCasesRequestSearchCasesPaginateTypeDef(
     _RequiredSearchCasesRequestSearchCasesPaginateTypeDef,
     _OptionalSearchCasesRequestSearchCasesPaginateTypeDef,
 ):
     pass
 
-EventIncludedDataOutputTypeDef = TypedDict(
-    "EventIncludedDataOutputTypeDef",
+EventIncludedDataTypeDef = TypedDict(
+    "EventIncludedDataTypeDef",
     {
-        "caseData": CaseEventIncludedDataOutputTypeDef,
+        "caseData": CaseEventIncludedDataTypeDef,
         "relatedItemData": RelatedItemEventIncludedDataTypeDef,
     },
     total=False,
 )
 
-EventIncludedDataTypeDef = TypedDict(
-    "EventIncludedDataTypeDef",
+EventIncludedDataOutputTypeDef = TypedDict(
+    "EventIncludedDataOutputTypeDef",
     {
-        "caseData": CaseEventIncludedDataTypeDef,
-        "relatedItemData": RelatedItemEventIncludedDataTypeDef,
+        "caseData": CaseEventIncludedDataOutputTypeDef,
+        "relatedItemData": RelatedItemEventIncludedDataOutputTypeDef,
     },
-    total=False,
 )
 
-_RequiredSearchRelatedItemsResponseItemTypeDef = TypedDict(
-    "_RequiredSearchRelatedItemsResponseItemTypeDef",
+SearchRelatedItemsResponseItemTypeDef = TypedDict(
+    "SearchRelatedItemsResponseItemTypeDef",
     {
         "associationTime": datetime,
         "content": RelatedItemContentTypeDef,
         "relatedItemId": str,
-        "type": RelatedItemTypeType,
-    },
-)
-_OptionalSearchRelatedItemsResponseItemTypeDef = TypedDict(
-    "_OptionalSearchRelatedItemsResponseItemTypeDef",
-    {
         "tags": Dict[str, str],
+        "type": RelatedItemTypeType,
     },
-    total=False,
 )
 
-class SearchRelatedItemsResponseItemTypeDef(
-    _RequiredSearchRelatedItemsResponseItemTypeDef, _OptionalSearchRelatedItemsResponseItemTypeDef
-):
-    pass
-
 _RequiredSearchRelatedItemsRequestRequestTypeDef = TypedDict(
     "_RequiredSearchRelatedItemsRequestRequestTypeDef",
     {
         "caseId": str,
         "domainId": str,
     },
 )
@@ -1104,77 +1094,88 @@
 )
 
 SectionOutputTypeDef = TypedDict(
     "SectionOutputTypeDef",
     {
         "fieldGroup": FieldGroupOutputTypeDef,
     },
-    total=False,
 )
 
 SectionTypeDef = TypedDict(
     "SectionTypeDef",
     {
         "fieldGroup": FieldGroupTypeDef,
     },
     total=False,
 )
 
-FieldValueUnionTypeDef = Union["FieldValueTypeDef", FieldValueOutputTypeDef]
 GetCaseResponseTypeDef = TypedDict(
     "GetCaseResponseTypeDef",
     {
         "fields": List[FieldValueOutputTypeDef],
         "nextToken": str,
         "tags": Dict[str, str],
         "templateId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredSearchCasesResponseItemTypeDef = TypedDict(
-    "_RequiredSearchCasesResponseItemTypeDef",
+SearchCasesResponseItemTypeDef = TypedDict(
+    "SearchCasesResponseItemTypeDef",
     {
         "caseId": str,
         "fields": List[FieldValueOutputTypeDef],
+        "tags": Dict[str, str],
         "templateId": str,
     },
 )
-_OptionalSearchCasesResponseItemTypeDef = TypedDict(
-    "_OptionalSearchCasesResponseItemTypeDef",
+
+_RequiredCreateCaseRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateCaseRequestRequestTypeDef",
     {
-        "tags": Dict[str, str],
+        "domainId": str,
+        "fields": Sequence[FieldValueTypeDef],
+        "templateId": str,
+    },
+)
+_OptionalCreateCaseRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateCaseRequestRequestTypeDef",
+    {
+        "clientToken": str,
     },
     total=False,
 )
 
-class SearchCasesResponseItemTypeDef(
-    _RequiredSearchCasesResponseItemTypeDef, _OptionalSearchCasesResponseItemTypeDef
+class CreateCaseRequestRequestTypeDef(
+    _RequiredCreateCaseRequestRequestTypeDef, _OptionalCreateCaseRequestRequestTypeDef
 ):
     pass
 
-_RequiredEventBridgeConfigurationOutputTypeDef = TypedDict(
-    "_RequiredEventBridgeConfigurationOutputTypeDef",
+FieldFilterTypeDef = TypedDict(
+    "FieldFilterTypeDef",
     {
-        "enabled": bool,
+        "contains": FieldValueTypeDef,
+        "equalTo": FieldValueTypeDef,
+        "greaterThan": FieldValueTypeDef,
+        "greaterThanOrEqualTo": FieldValueTypeDef,
+        "lessThan": FieldValueTypeDef,
+        "lessThanOrEqualTo": FieldValueTypeDef,
     },
+    total=False,
 )
-_OptionalEventBridgeConfigurationOutputTypeDef = TypedDict(
-    "_OptionalEventBridgeConfigurationOutputTypeDef",
+
+UpdateCaseRequestRequestTypeDef = TypedDict(
+    "UpdateCaseRequestRequestTypeDef",
     {
-        "includedData": EventIncludedDataOutputTypeDef,
+        "caseId": str,
+        "domainId": str,
+        "fields": Sequence[FieldValueTypeDef],
     },
-    total=False,
 )
 
-class EventBridgeConfigurationOutputTypeDef(
-    _RequiredEventBridgeConfigurationOutputTypeDef, _OptionalEventBridgeConfigurationOutputTypeDef
-):
-    pass
-
 _RequiredEventBridgeConfigurationTypeDef = TypedDict(
     "_RequiredEventBridgeConfigurationTypeDef",
     {
         "enabled": bool,
     },
 )
 _OptionalEventBridgeConfigurationTypeDef = TypedDict(
@@ -1186,91 +1187,88 @@
 )
 
 class EventBridgeConfigurationTypeDef(
     _RequiredEventBridgeConfigurationTypeDef, _OptionalEventBridgeConfigurationTypeDef
 ):
     pass
 
+EventBridgeConfigurationOutputTypeDef = TypedDict(
+    "EventBridgeConfigurationOutputTypeDef",
+    {
+        "enabled": bool,
+        "includedData": EventIncludedDataOutputTypeDef,
+    },
+)
+
 SearchRelatedItemsResponseTypeDef = TypedDict(
     "SearchRelatedItemsResponseTypeDef",
     {
         "nextToken": str,
         "relatedItems": List[SearchRelatedItemsResponseItemTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LayoutSectionsOutputTypeDef = TypedDict(
     "LayoutSectionsOutputTypeDef",
     {
         "sections": List[SectionOutputTypeDef],
     },
-    total=False,
 )
 
 LayoutSectionsTypeDef = TypedDict(
     "LayoutSectionsTypeDef",
     {
         "sections": Sequence[SectionTypeDef],
     },
     total=False,
 )
 
-FieldValueTypeDef = TypedDict(
-    "FieldValueTypeDef",
-    {
-        "id": str,
-        "value": FieldValueUnionTypeDef,
-    },
-)
-
-UpdateCaseRequestRequestTypeDef = TypedDict(
-    "UpdateCaseRequestRequestTypeDef",
-    {
-        "caseId": str,
-        "domainId": str,
-        "fields": Sequence[FieldValueUnionTypeDef],
-    },
-)
-
 SearchCasesResponseTypeDef = TypedDict(
     "SearchCasesResponseTypeDef",
     {
         "cases": List[SearchCasesResponseItemTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetCaseEventConfigurationResponseTypeDef = TypedDict(
-    "GetCaseEventConfigurationResponseTypeDef",
+CaseFilterTypeDef = TypedDict(
+    "CaseFilterTypeDef",
     {
-        "eventBridge": EventBridgeConfigurationOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "andAll": Sequence[Dict[str, Any]],
+        "field": FieldFilterTypeDef,
+        "not": Dict[str, Any],
+        "orAll": Sequence[Dict[str, Any]],
     },
+    total=False,
 )
 
-EventBridgeConfigurationUnionTypeDef = Union[
-    EventBridgeConfigurationTypeDef, EventBridgeConfigurationOutputTypeDef
-]
 PutCaseEventConfigurationRequestRequestTypeDef = TypedDict(
     "PutCaseEventConfigurationRequestRequestTypeDef",
     {
         "domainId": str,
         "eventBridge": EventBridgeConfigurationTypeDef,
     },
 )
 
+GetCaseEventConfigurationResponseTypeDef = TypedDict(
+    "GetCaseEventConfigurationResponseTypeDef",
+    {
+        "eventBridge": EventBridgeConfigurationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 BasicLayoutOutputTypeDef = TypedDict(
     "BasicLayoutOutputTypeDef",
     {
         "moreInfo": LayoutSectionsOutputTypeDef,
         "topPanel": LayoutSectionsOutputTypeDef,
     },
-    total=False,
 )
 
 BasicLayoutTypeDef = TypedDict(
     "BasicLayoutTypeDef",
     {
         "moreInfo": LayoutSectionsTypeDef,
         "topPanel": LayoutSectionsTypeDef,
@@ -1279,15 +1277,14 @@
 )
 
 LayoutContentOutputTypeDef = TypedDict(
     "LayoutContentOutputTypeDef",
     {
         "basic": BasicLayoutOutputTypeDef,
     },
-    total=False,
 )
 
 LayoutContentTypeDef = TypedDict(
     "LayoutContentTypeDef",
     {
         "basic": BasicLayoutTypeDef,
     },
@@ -1311,15 +1308,14 @@
     {
         "content": LayoutContentTypeDef,
         "domainId": str,
         "name": str,
     },
 )
 
-LayoutContentUnionTypeDef = Union[LayoutContentTypeDef, LayoutContentOutputTypeDef]
 _RequiredUpdateLayoutRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateLayoutRequestRequestTypeDef",
     {
         "domainId": str,
         "layoutId": str,
     },
 )
```

### Comparing `mypy-boto3-connectcases-1.28.16/mypy_boto3_connectcases.egg-info/PKG-INFO` & `mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-connectcases
-Version: 1.28.16
-Summary: Type annotations for boto3.ConnectCases 1.28.16 service generated with mypy-boto3-builder 7.17.1
+Version: 1.28.8
+Summary: Type annotations for boto3.ConnectCases 1.28.8 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 connectcases type-annotations botocore mypy typeshed autocomplete
+Keywords: boto3 connectcases type-annotations boto3-stubs mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-connectcases"></a>
 
 # mypy-boto3-connectcases
 
 [![PyPI - mypy-boto3-connectcases](https://img.shields.io/pypi/v/mypy-boto3-connectcases.svg?color=blue)](https://pypi.org/project/mypy-boto3-connectcases)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-connectcases.svg?color=blue)](https://pypi.org/project/mypy-boto3-connectcases)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-connectcases)](https://pepy.tech/project/mypy-boto3-connectcases)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-connectcases?color=blue)](https://pypistats.org/packages/mypy-boto3-connectcases)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ConnectCases 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases)
+[boto3.ConnectCases 1.28.8](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.17.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-connectcases docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/).
 
 See how it helps to find and fix potential bugs:
 
@@ -74,15 +74,15 @@
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Literals](#literals)
-    - [Type definitions](#type-definitions)
+    - [Typed dictionaries](#typed-dictionaries)
   - [How it works](#how-it-works)
   - [What's new](#what's-new)
     - [Implemented features](#implemented-features)
     - [Latest changes](#latest-changes)
   - [Versioning](#versioning)
   - [Thank you](#thank-you)
   - [Documentation](#documentation)
@@ -321,50 +321,56 @@
 )
 
 
 def check_value(value: CommentBodyTextTypeType) -> bool:
     ...
 ```
 
-<a id="type-definitions"></a>
+<a id="typed-dictionaries"></a>
 
-### Type definitions
+### Typed dictionaries
 
 `mypy_boto3_connectcases.type_defs` module contains structures and shapes
-assembled to typed dictionaries and unions for additional type checking.
+assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_connectcases.type_defs import (
     FieldIdentifierTypeDef,
     FieldErrorTypeDef,
     GetFieldResponseTypeDef,
     ResponseMetadataTypeDef,
     FieldOptionTypeDef,
     FieldOptionErrorTypeDef,
-    FieldFilterTypeDef,
+    FieldIdentifierOutputTypeDef,
     CaseSummaryTypeDef,
+    CommentContentOutputTypeDef,
     CommentContentTypeDef,
     ContactContentTypeDef,
     ContactFilterTypeDef,
     ContactTypeDef,
-    CreateCaseRequestRequestTypeDef,
     CreateDomainRequestRequestTypeDef,
     CreateFieldRequestRequestTypeDef,
     LayoutConfigurationTypeDef,
     RequiredFieldTypeDef,
     DeleteDomainRequestRequestTypeDef,
     DomainSummaryTypeDef,
+    RelatedItemEventIncludedDataOutputTypeDef,
     RelatedItemEventIncludedDataTypeDef,
+    FieldItemOutputTypeDef,
     FieldItemTypeDef,
+    FieldOptionOutputTypeDef,
     FieldSummaryTypeDef,
     FieldValueUnionOutputTypeDef,
+    FieldValueUnionTypeDef,
     GetCaseEventConfigurationRequestRequestTypeDef,
     GetDomainRequestRequestTypeDef,
     GetLayoutRequestRequestTypeDef,
     GetTemplateRequestRequestTypeDef,
+    LayoutConfigurationOutputTypeDef,
+    RequiredFieldOutputTypeDef,
     LayoutSummaryTypeDef,
     ListCasesForContactRequestRequestTypeDef,
     ListDomainsRequestRequestTypeDef,
     ListFieldOptionsRequestRequestTypeDef,
     ListFieldsRequestRequestTypeDef,
     ListLayoutsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
@@ -372,81 +378,80 @@
     TemplateSummaryTypeDef,
     PaginatorConfigTypeDef,
     SortTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateFieldRequestRequestTypeDef,
     BatchGetFieldRequestRequestTypeDef,
-    CaseEventIncludedDataOutputTypeDef,
     CaseEventIncludedDataTypeDef,
     GetCaseRequestRequestTypeDef,
     BatchGetFieldResponseTypeDef,
     CreateCaseResponseTypeDef,
     CreateDomainResponseTypeDef,
     CreateFieldResponseTypeDef,
     CreateLayoutResponseTypeDef,
     CreateRelatedItemResponseTypeDef,
     CreateTemplateResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetDomainResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     BatchPutFieldOptionsRequestRequestTypeDef,
-    ListFieldOptionsResponseTypeDef,
     BatchPutFieldOptionsResponseTypeDef,
-    CaseFilterTypeDef,
+    CaseEventIncludedDataOutputTypeDef,
     ListCasesForContactResponseTypeDef,
     RelatedItemContentTypeDef,
     RelatedItemTypeFilterTypeDef,
     RelatedItemInputContentTypeDef,
     CreateTemplateRequestRequestTypeDef,
-    GetTemplateResponseTypeDef,
     UpdateTemplateRequestRequestTypeDef,
     ListDomainsResponseTypeDef,
     FieldGroupOutputTypeDef,
     FieldGroupTypeDef,
+    ListFieldOptionsResponseTypeDef,
     ListFieldsResponseTypeDef,
     FieldValueOutputTypeDef,
+    FieldValueTypeDef,
+    GetTemplateResponseTypeDef,
     ListLayoutsResponseTypeDef,
     ListTemplatesResponseTypeDef,
     SearchCasesRequestRequestTypeDef,
     SearchCasesRequestSearchCasesPaginateTypeDef,
-    EventIncludedDataOutputTypeDef,
     EventIncludedDataTypeDef,
+    EventIncludedDataOutputTypeDef,
     SearchRelatedItemsResponseItemTypeDef,
     SearchRelatedItemsRequestRequestTypeDef,
     SearchRelatedItemsRequestSearchRelatedItemsPaginateTypeDef,
     CreateRelatedItemRequestRequestTypeDef,
     SectionOutputTypeDef,
     SectionTypeDef,
-    FieldValueUnionTypeDef,
     GetCaseResponseTypeDef,
     SearchCasesResponseItemTypeDef,
-    EventBridgeConfigurationOutputTypeDef,
+    CreateCaseRequestRequestTypeDef,
+    FieldFilterTypeDef,
+    UpdateCaseRequestRequestTypeDef,
     EventBridgeConfigurationTypeDef,
+    EventBridgeConfigurationOutputTypeDef,
     SearchRelatedItemsResponseTypeDef,
     LayoutSectionsOutputTypeDef,
     LayoutSectionsTypeDef,
-    FieldValueTypeDef,
-    UpdateCaseRequestRequestTypeDef,
     SearchCasesResponseTypeDef,
-    GetCaseEventConfigurationResponseTypeDef,
-    EventBridgeConfigurationUnionTypeDef,
+    CaseFilterTypeDef,
     PutCaseEventConfigurationRequestRequestTypeDef,
+    GetCaseEventConfigurationResponseTypeDef,
     BasicLayoutOutputTypeDef,
     BasicLayoutTypeDef,
     LayoutContentOutputTypeDef,
     LayoutContentTypeDef,
     GetLayoutResponseTypeDef,
     CreateLayoutRequestRequestTypeDef,
-    LayoutContentUnionTypeDef,
     UpdateLayoutRequestRequestTypeDef,
 )
 
 
-def get_value() -> FieldIdentifierTypeDef:
+def get_structure() -> FieldIdentifierTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-connectcases-1.28.16/mypy_boto3_connectcases.egg-info/SOURCES.txt` & `mypy-boto3-connectcases-1.28.8/mypy_boto3_connectcases.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connectcases-1.28.16/setup.py` & `mypy-boto3-connectcases-1.28.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-connectcases",
-    version="1.28.16",
+    version="1.28.8",
     packages=["mypy_boto3_connectcases"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ConnectCases 1.28.16 service generated with mypy-boto3-builder"
-        " 7.17.1"
+        "Type annotations for boto3.ConnectCases 1.28.8 service generated with mypy-boto3-builder"
+        " 7.15.1"
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
-    keywords="boto3 connectcases type-annotations botocore mypy typeshed autocomplete",
+    keywords="boto3 connectcases type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_connectcases": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcases/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

