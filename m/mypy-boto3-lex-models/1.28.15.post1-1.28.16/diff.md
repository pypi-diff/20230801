# Comparing `tmp/mypy-boto3-lex-models-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-lex-models-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-lex-models-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:30 2023, max compression
+gzip compressed data, was "mypy-boto3-lex-models-1.28.16.tar", last modified: Tue Aug  1 11:37:10 2023, max compression
```

## Comparing `mypy-boto3-lex-models-1.28.15.post1.tar` & `mypy-boto3-lex-models-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:30.541232 mypy-boto3-lex-models-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:49:16.000000 mypy-boto3-lex-models-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19431 2023-07-29 10:03:30.541232 mypy-boto3-lex-models-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17913 2023-07-29 09:49:16.000000 mypy-boto3-lex-models-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:30.525232 mypy-boto3-lex-models-1.28.15.post1/mypy_boto3_lex_models/
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-07-29 09:49:16.000000 mypy-boto3-lex-models-1.28.15.post1/mypy_boto3_lex_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-07-29 09:49:16.000000 mypy-boto3-lex-models-1.28.15.post1/mypy_boto3_lex_models/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-29 09:49:16.000000 mypy-boto3-lex-models-1.28.15.post1/mypy_boto3_lex_models/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35521 2023-07-29 09:49:16.000000 mypy-boto3-lex-models-1.28.15.post1/mypy_boto3_lex_models/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    35462 2023-07-29 09:49:16.000000 mypy-boto3-lex-models-1.28.15.post1/mypy_boto3_lex_models/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11225 2023-07-29 09:49:17.000000 mypy-boto3-lex-models-1.28.15.post1/mypy_boto3_lex_models/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11223 2023-07-29 09:49:17.000000 mypy-boto3-lex-models-1.28.15.post1/mypy_boto3_lex_models/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12097 2023-07-29 09:49:16.000000 mypy-boto3-lex-models-1.28.15.post1/mypy_boto3_lex_models/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12085 2023-07-29 09:49:16.000000 mypy-boto3-lex-models-1.28.15.post1/mypy_boto3_lex_models/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:49:16.000000 mypy-boto3-lex-models-1.28.15.post1/mypy_boto3_lex_models/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    48713 2023-07-29 09:49:18.000000 mypy-boto3-lex-models-1.28.15.post1/mypy_boto3_lex_models/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    48653 2023-07-29 09:49:17.000000 mypy-boto3-lex-models-1.28.15.post1/mypy_boto3_lex_models/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:49:16.000000 mypy-boto3-lex-models-1.28.15.post1/mypy_boto3_lex_models/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:30.537232 mypy-boto3-lex-models-1.28.15.post1/mypy_boto3_lex_models.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19431 2023-07-29 10:03:30.000000 mypy-boto3-lex-models-1.28.15.post1/mypy_boto3_lex_models.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-29 10:03:30.000000 mypy-boto3-lex-models-1.28.15.post1/mypy_boto3_lex_models.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:30.000000 mypy-boto3-lex-models-1.28.15.post1/mypy_boto3_lex_models.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:30.000000 mypy-boto3-lex-models-1.28.15.post1/mypy_boto3_lex_models.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:30.000000 mypy-boto3-lex-models-1.28.15.post1/mypy_boto3_lex_models.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-29 10:03:30.000000 mypy-boto3-lex-models-1.28.15.post1/mypy_boto3_lex_models.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:30.541232 mypy-boto3-lex-models-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-07-29 09:49:16.000000 mypy-boto3-lex-models-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:10.500844 mypy-boto3-lex-models-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:22:04.000000 mypy-boto3-lex-models-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19560 2023-08-01 11:37:10.500844 mypy-boto3-lex-models-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18051 2023-08-01 11:22:04.000000 mypy-boto3-lex-models-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:10.500844 mypy-boto3-lex-models-1.28.16/mypy_boto3_lex_models/
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-08-01 11:22:04.000000 mypy-boto3-lex-models-1.28.16/mypy_boto3_lex_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-08-01 11:22:04.000000 mypy-boto3-lex-models-1.28.16/mypy_boto3_lex_models/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-08-01 11:22:04.000000 mypy-boto3-lex-models-1.28.16/mypy_boto3_lex_models/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35103 2023-08-01 11:22:04.000000 mypy-boto3-lex-models-1.28.16/mypy_boto3_lex_models/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35044 2023-08-01 11:22:04.000000 mypy-boto3-lex-models-1.28.16/mypy_boto3_lex_models/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11225 2023-08-01 11:22:05.000000 mypy-boto3-lex-models-1.28.16/mypy_boto3_lex_models/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11223 2023-08-01 11:22:05.000000 mypy-boto3-lex-models-1.28.16/mypy_boto3_lex_models/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12097 2023-08-01 11:22:05.000000 mypy-boto3-lex-models-1.28.16/mypy_boto3_lex_models/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12085 2023-08-01 11:22:04.000000 mypy-boto3-lex-models-1.28.16/mypy_boto3_lex_models/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:22:04.000000 mypy-boto3-lex-models-1.28.16/mypy_boto3_lex_models/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    49167 2023-08-01 11:22:08.000000 mypy-boto3-lex-models-1.28.16/mypy_boto3_lex_models/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49107 2023-08-01 11:22:08.000000 mypy-boto3-lex-models-1.28.16/mypy_boto3_lex_models/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:22:04.000000 mypy-boto3-lex-models-1.28.16/mypy_boto3_lex_models/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:10.500844 mypy-boto3-lex-models-1.28.16/mypy_boto3_lex_models.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19560 2023-08-01 11:37:10.000000 mypy-boto3-lex-models-1.28.16/mypy_boto3_lex_models.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-08-01 11:37:10.000000 mypy-boto3-lex-models-1.28.16/mypy_boto3_lex_models.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:10.000000 mypy-boto3-lex-models-1.28.16/mypy_boto3_lex_models.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:10.000000 mypy-boto3-lex-models-1.28.16/mypy_boto3_lex_models.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:10.000000 mypy-boto3-lex-models-1.28.16/mypy_boto3_lex_models.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-01 11:37:10.000000 mypy-boto3-lex-models-1.28.16/mypy_boto3_lex_models.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:10.500844 mypy-boto3-lex-models-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-08-01 11:22:04.000000 mypy-boto3-lex-models-1.28.16/setup.py
```

### Comparing `mypy-boto3-lex-models-1.28.15.post1/LICENSE` & `mypy-boto3-lex-models-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lex-models-1.28.15.post1/PKG-INFO` & `mypy-boto3-lex-models-1.28.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-lex-models
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.LexModelBuildingService 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.LexModelBuildingService 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 lex-models type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 lex-models type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lex-models.svg?color=blue)](https://pypi.org/project/mypy-boto3-lex-models)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-lex-models)](https://pepy.tech/project/mypy-boto3-lex-models)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LexModelBuildingService 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService)
+[boto3.LexModelBuildingService 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService)
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
 [mypy-boto3-lex-models docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/).
 
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
@@ -372,23 +372,24 @@
 )
 
 
 def check_value(value: ChannelStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_lex_models.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_lex_models.type_defs import (
+    BlobTypeDef,
     BotChannelAssociationTypeDef,
     BotMetadataTypeDef,
     BuiltinIntentMetadataTypeDef,
     BuiltinIntentSlotTypeDef,
     BuiltinSlotTypeMetadataTypeDef,
     CodeHookTypeDef,
     LogSettingsRequestTypeDef,
@@ -456,14 +457,15 @@
     GetBotsResponseTypeDef,
     GetBuiltinIntentResponseTypeDef,
     GetBuiltinIntentsResponseTypeDef,
     GetBuiltinSlotTypesResponseTypeDef,
     GetExportResponseTypeDef,
     GetImportResponseTypeDef,
     StartMigrationResponseTypeDef,
+    EnumerationValueUnionTypeDef,
     GetBotAliasesRequestGetBotAliasesPaginateTypeDef,
     GetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef,
     GetBotVersionsRequestGetBotVersionsPaginateTypeDef,
     GetBotsRequestGetBotsPaginateTypeDef,
     GetBuiltinIntentsRequestGetBuiltinIntentsPaginateTypeDef,
     GetBuiltinSlotTypesRequestGetBuiltinSlotTypesPaginateTypeDef,
     GetIntentVersionsRequestGetIntentVersionsPaginateTypeDef,
@@ -488,36 +490,40 @@
     SlotDefaultValueSpecTypeDef,
     SlotTypeConfigurationTypeDef,
     UtteranceListTypeDef,
     PutBotAliasRequestRequestTypeDef,
     BotAliasMetadataTypeDef,
     GetBotAliasResponseTypeDef,
     PutBotAliasResponseTypeDef,
+    PromptUnionTypeDef,
     CreateBotVersionResponseTypeDef,
     FollowUpPromptOutputTypeDef,
     GetBotResponseTypeDef,
     PutBotResponseTypeDef,
     FollowUpPromptTypeDef,
     PutBotRequestRequestTypeDef,
+    StatementUnionTypeDef,
     SlotOutputTypeDef,
     SlotTypeDef,
     CreateSlotTypeVersionResponseTypeDef,
     GetSlotTypeResponseTypeDef,
     PutSlotTypeRequestRequestTypeDef,
     PutSlotTypeResponseTypeDef,
     GetUtterancesViewResponseTypeDef,
     GetBotAliasesResponseTypeDef,
+    FollowUpPromptUnionTypeDef,
     CreateIntentVersionResponseTypeDef,
     GetIntentResponseTypeDef,
     PutIntentResponseTypeDef,
+    SlotUnionTypeDef,
     PutIntentRequestRequestTypeDef,
 )
 
 
-def get_structure() -> BotChannelAssociationTypeDef:
+def get_value() -> BlobTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-lex-models-1.28.15.post1/README.md` & `mypy-boto3-lex-models-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lex-models.svg?color=blue)](https://pypi.org/project/mypy-boto3-lex-models)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-lex-models)](https://pepy.tech/project/mypy-boto3-lex-models)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LexModelBuildingService 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService)
+[boto3.LexModelBuildingService 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService)
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
 [mypy-boto3-lex-models docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/).
 
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
@@ -340,23 +340,24 @@
 )
 
 
 def check_value(value: ChannelStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_lex_models.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_lex_models.type_defs import (
+    BlobTypeDef,
     BotChannelAssociationTypeDef,
     BotMetadataTypeDef,
     BuiltinIntentMetadataTypeDef,
     BuiltinIntentSlotTypeDef,
     BuiltinSlotTypeMetadataTypeDef,
     CodeHookTypeDef,
     LogSettingsRequestTypeDef,
@@ -424,14 +425,15 @@
     GetBotsResponseTypeDef,
     GetBuiltinIntentResponseTypeDef,
     GetBuiltinIntentsResponseTypeDef,
     GetBuiltinSlotTypesResponseTypeDef,
     GetExportResponseTypeDef,
     GetImportResponseTypeDef,
     StartMigrationResponseTypeDef,
+    EnumerationValueUnionTypeDef,
     GetBotAliasesRequestGetBotAliasesPaginateTypeDef,
     GetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef,
     GetBotVersionsRequestGetBotVersionsPaginateTypeDef,
     GetBotsRequestGetBotsPaginateTypeDef,
     GetBuiltinIntentsRequestGetBuiltinIntentsPaginateTypeDef,
     GetBuiltinSlotTypesRequestGetBuiltinSlotTypesPaginateTypeDef,
     GetIntentVersionsRequestGetIntentVersionsPaginateTypeDef,
@@ -456,36 +458,40 @@
     SlotDefaultValueSpecTypeDef,
     SlotTypeConfigurationTypeDef,
     UtteranceListTypeDef,
     PutBotAliasRequestRequestTypeDef,
     BotAliasMetadataTypeDef,
     GetBotAliasResponseTypeDef,
     PutBotAliasResponseTypeDef,
+    PromptUnionTypeDef,
     CreateBotVersionResponseTypeDef,
     FollowUpPromptOutputTypeDef,
     GetBotResponseTypeDef,
     PutBotResponseTypeDef,
     FollowUpPromptTypeDef,
     PutBotRequestRequestTypeDef,
+    StatementUnionTypeDef,
     SlotOutputTypeDef,
     SlotTypeDef,
     CreateSlotTypeVersionResponseTypeDef,
     GetSlotTypeResponseTypeDef,
     PutSlotTypeRequestRequestTypeDef,
     PutSlotTypeResponseTypeDef,
     GetUtterancesViewResponseTypeDef,
     GetBotAliasesResponseTypeDef,
+    FollowUpPromptUnionTypeDef,
     CreateIntentVersionResponseTypeDef,
     GetIntentResponseTypeDef,
     PutIntentResponseTypeDef,
+    SlotUnionTypeDef,
     PutIntentRequestRequestTypeDef,
 )
 
 
-def get_structure() -> BotChannelAssociationTypeDef:
+def get_value() -> BlobTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-lex-models-1.28.15.post1/mypy_boto3_lex_models/__init__.py` & `mypy-boto3-lex-models-1.28.16/mypy_boto3_lex_models/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lex-models-1.28.15.post1/mypy_boto3_lex_models/__init__.pyi` & `mypy-boto3-lex-models-1.28.16/mypy_boto3_lex_models/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lex-models-1.28.15.post1/mypy_boto3_lex_models/__main__.py` & `mypy-boto3-lex-models-1.28.16/mypy_boto3_lex_models/__main__.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.LexModelBuildingService 1.28.15\nVersion:        "
-        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.LexModelBuildingService 1.28.16\nVersion:        "
+        " 1.28.16\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService\nOther"
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

### Comparing `mypy-boto3-lex-models-1.28.15.post1/mypy_boto3_lex_models/client.py` & `mypy-boto3-lex-models-1.28.16/mypy_boto3_lex_models/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,18 +10,17 @@
     from mypy_boto3_lex_models.client import LexModelBuildingServiceClient
 
     session = Session()
     client: LexModelBuildingServiceClient = session.client("lex-models")
     ```
 """
 import sys
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
-from botocore.response import StreamingBody
 
 from .literals import (
     ExportTypeType,
     LocaleType,
     MergeStrategyType,
     MigrationSortAttributeType,
     MigrationStatusType,
@@ -41,24 +40,23 @@
     GetBuiltinSlotTypesPaginator,
     GetIntentsPaginator,
     GetIntentVersionsPaginator,
     GetSlotTypesPaginator,
     GetSlotTypeVersionsPaginator,
 )
 from .type_defs import (
+    BlobTypeDef,
     CodeHookTypeDef,
     ConversationLogsRequestTypeDef,
     CreateBotVersionResponseTypeDef,
     CreateIntentVersionResponseTypeDef,
     CreateSlotTypeVersionResponseTypeDef,
     EmptyResponseMetadataTypeDef,
-    EnumerationValueOutputTypeDef,
-    EnumerationValueTypeDef,
-    FollowUpPromptOutputTypeDef,
-    FollowUpPromptTypeDef,
+    EnumerationValueUnionTypeDef,
+    FollowUpPromptUnionTypeDef,
     FulfillmentActivityTypeDef,
     GetBotAliasesResponseTypeDef,
     GetBotAliasResponseTypeDef,
     GetBotChannelAssociationResponseTypeDef,
     GetBotChannelAssociationsResponseTypeDef,
     GetBotResponseTypeDef,
     GetBotsResponseTypeDef,
@@ -78,27 +76,24 @@
     GetSlotTypeVersionsResponseTypeDef,
     GetUtterancesViewResponseTypeDef,
     InputContextTypeDef,
     IntentTypeDef,
     KendraConfigurationTypeDef,
     ListTagsForResourceResponseTypeDef,
     OutputContextTypeDef,
-    PromptOutputTypeDef,
-    PromptTypeDef,
+    PromptUnionTypeDef,
     PutBotAliasResponseTypeDef,
     PutBotResponseTypeDef,
     PutIntentResponseTypeDef,
     PutSlotTypeResponseTypeDef,
-    SlotOutputTypeDef,
     SlotTypeConfigurationTypeDef,
-    SlotTypeDef,
+    SlotUnionTypeDef,
     StartImportResponseTypeDef,
     StartMigrationResponseTypeDef,
-    StatementOutputTypeDef,
-    StatementTypeDef,
+    StatementUnionTypeDef,
     TagTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -521,16 +516,16 @@
         name: str,
         locale: LocaleType,
         childDirected: bool,
         description: str = ...,
         intents: Sequence[IntentTypeDef] = ...,
         enableModelImprovements: bool = ...,
         nluIntentConfidenceThreshold: float = ...,
-        clarificationPrompt: Union[PromptTypeDef, PromptOutputTypeDef] = ...,
-        abortStatement: Union[StatementTypeDef, StatementOutputTypeDef] = ...,
+        clarificationPrompt: PromptUnionTypeDef = ...,
+        abortStatement: StatementUnionTypeDef = ...,
         idleSessionTTLInSeconds: int = ...,
         voiceId: str = ...,
         checksum: str = ...,
         processBehavior: ProcessBehaviorType = ...,
         detectSentiment: bool = ...,
         createVersion: bool = ...,
         tags: Sequence[TagTypeDef] = ...
@@ -562,20 +557,20 @@
         """
 
     def put_intent(
         self,
         *,
         name: str,
         description: str = ...,
-        slots: Sequence[Union[SlotTypeDef, SlotOutputTypeDef]] = ...,
+        slots: Sequence[SlotUnionTypeDef] = ...,
         sampleUtterances: Sequence[str] = ...,
-        confirmationPrompt: Union[PromptTypeDef, PromptOutputTypeDef] = ...,
-        rejectionStatement: Union[StatementTypeDef, StatementOutputTypeDef] = ...,
-        followUpPrompt: Union[FollowUpPromptTypeDef, FollowUpPromptOutputTypeDef] = ...,
-        conclusionStatement: Union[StatementTypeDef, StatementOutputTypeDef] = ...,
+        confirmationPrompt: PromptUnionTypeDef = ...,
+        rejectionStatement: StatementUnionTypeDef = ...,
+        followUpPrompt: FollowUpPromptUnionTypeDef = ...,
+        conclusionStatement: StatementUnionTypeDef = ...,
         dialogCodeHook: CodeHookTypeDef = ...,
         fulfillmentActivity: FulfillmentActivityTypeDef = ...,
         parentIntentSignature: str = ...,
         checksum: str = ...,
         createVersion: bool = ...,
         kendraConfiguration: KendraConfigurationTypeDef = ...,
         inputContexts: Sequence[InputContextTypeDef] = ...,
@@ -589,17 +584,15 @@
         """
 
     def put_slot_type(
         self,
         *,
         name: str,
         description: str = ...,
-        enumerationValues: Sequence[
-            Union[EnumerationValueTypeDef, EnumerationValueOutputTypeDef]
-        ] = ...,
+        enumerationValues: Sequence[EnumerationValueUnionTypeDef] = ...,
         checksum: str = ...,
         valueSelectionStrategy: SlotValueSelectionStrategyType = ...,
         createVersion: bool = ...,
         parentSlotTypeSignature: str = ...,
         slotTypeConfigurations: Sequence[SlotTypeConfigurationTypeDef] = ...
     ) -> PutSlotTypeResponseTypeDef:
         """
@@ -608,15 +601,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Client.put_slot_type)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/client/#put_slot_type)
         """
 
     def start_import(
         self,
         *,
-        payload: Union[str, bytes, IO[Any], StreamingBody],
+        payload: BlobTypeDef,
         resourceType: ResourceTypeType,
         mergeStrategy: MergeStrategyType,
         tags: Sequence[TagTypeDef] = ...
     ) -> StartImportResponseTypeDef:
         """
         Starts a job to import a resource to Amazon Lex.
```

### Comparing `mypy-boto3-lex-models-1.28.15.post1/mypy_boto3_lex_models/client.pyi` & `mypy-boto3-lex-models-1.28.16/mypy_boto3_lex_models/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,18 +10,17 @@
     from mypy_boto3_lex_models.client import LexModelBuildingServiceClient
 
     session = Session()
     client: LexModelBuildingServiceClient = session.client("lex-models")
     ```
 """
 import sys
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
-from botocore.response import StreamingBody
 
 from .literals import (
     ExportTypeType,
     LocaleType,
     MergeStrategyType,
     MigrationSortAttributeType,
     MigrationStatusType,
@@ -41,24 +40,23 @@
     GetBuiltinSlotTypesPaginator,
     GetIntentsPaginator,
     GetIntentVersionsPaginator,
     GetSlotTypesPaginator,
     GetSlotTypeVersionsPaginator,
 )
 from .type_defs import (
+    BlobTypeDef,
     CodeHookTypeDef,
     ConversationLogsRequestTypeDef,
     CreateBotVersionResponseTypeDef,
     CreateIntentVersionResponseTypeDef,
     CreateSlotTypeVersionResponseTypeDef,
     EmptyResponseMetadataTypeDef,
-    EnumerationValueOutputTypeDef,
-    EnumerationValueTypeDef,
-    FollowUpPromptOutputTypeDef,
-    FollowUpPromptTypeDef,
+    EnumerationValueUnionTypeDef,
+    FollowUpPromptUnionTypeDef,
     FulfillmentActivityTypeDef,
     GetBotAliasesResponseTypeDef,
     GetBotAliasResponseTypeDef,
     GetBotChannelAssociationResponseTypeDef,
     GetBotChannelAssociationsResponseTypeDef,
     GetBotResponseTypeDef,
     GetBotsResponseTypeDef,
@@ -78,27 +76,24 @@
     GetSlotTypeVersionsResponseTypeDef,
     GetUtterancesViewResponseTypeDef,
     InputContextTypeDef,
     IntentTypeDef,
     KendraConfigurationTypeDef,
     ListTagsForResourceResponseTypeDef,
     OutputContextTypeDef,
-    PromptOutputTypeDef,
-    PromptTypeDef,
+    PromptUnionTypeDef,
     PutBotAliasResponseTypeDef,
     PutBotResponseTypeDef,
     PutIntentResponseTypeDef,
     PutSlotTypeResponseTypeDef,
-    SlotOutputTypeDef,
     SlotTypeConfigurationTypeDef,
-    SlotTypeDef,
+    SlotUnionTypeDef,
     StartImportResponseTypeDef,
     StartMigrationResponseTypeDef,
-    StatementOutputTypeDef,
-    StatementTypeDef,
+    StatementUnionTypeDef,
     TagTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -479,16 +474,16 @@
         name: str,
         locale: LocaleType,
         childDirected: bool,
         description: str = ...,
         intents: Sequence[IntentTypeDef] = ...,
         enableModelImprovements: bool = ...,
         nluIntentConfidenceThreshold: float = ...,
-        clarificationPrompt: Union[PromptTypeDef, PromptOutputTypeDef] = ...,
-        abortStatement: Union[StatementTypeDef, StatementOutputTypeDef] = ...,
+        clarificationPrompt: PromptUnionTypeDef = ...,
+        abortStatement: StatementUnionTypeDef = ...,
         idleSessionTTLInSeconds: int = ...,
         voiceId: str = ...,
         checksum: str = ...,
         processBehavior: ProcessBehaviorType = ...,
         detectSentiment: bool = ...,
         createVersion: bool = ...,
         tags: Sequence[TagTypeDef] = ...
@@ -518,20 +513,20 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/client/#put_bot_alias)
         """
     def put_intent(
         self,
         *,
         name: str,
         description: str = ...,
-        slots: Sequence[Union[SlotTypeDef, SlotOutputTypeDef]] = ...,
+        slots: Sequence[SlotUnionTypeDef] = ...,
         sampleUtterances: Sequence[str] = ...,
-        confirmationPrompt: Union[PromptTypeDef, PromptOutputTypeDef] = ...,
-        rejectionStatement: Union[StatementTypeDef, StatementOutputTypeDef] = ...,
-        followUpPrompt: Union[FollowUpPromptTypeDef, FollowUpPromptOutputTypeDef] = ...,
-        conclusionStatement: Union[StatementTypeDef, StatementOutputTypeDef] = ...,
+        confirmationPrompt: PromptUnionTypeDef = ...,
+        rejectionStatement: StatementUnionTypeDef = ...,
+        followUpPrompt: FollowUpPromptUnionTypeDef = ...,
+        conclusionStatement: StatementUnionTypeDef = ...,
         dialogCodeHook: CodeHookTypeDef = ...,
         fulfillmentActivity: FulfillmentActivityTypeDef = ...,
         parentIntentSignature: str = ...,
         checksum: str = ...,
         createVersion: bool = ...,
         kendraConfiguration: KendraConfigurationTypeDef = ...,
         inputContexts: Sequence[InputContextTypeDef] = ...,
@@ -544,17 +539,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/client/#put_intent)
         """
     def put_slot_type(
         self,
         *,
         name: str,
         description: str = ...,
-        enumerationValues: Sequence[
-            Union[EnumerationValueTypeDef, EnumerationValueOutputTypeDef]
-        ] = ...,
+        enumerationValues: Sequence[EnumerationValueUnionTypeDef] = ...,
         checksum: str = ...,
         valueSelectionStrategy: SlotValueSelectionStrategyType = ...,
         createVersion: bool = ...,
         parentSlotTypeSignature: str = ...,
         slotTypeConfigurations: Sequence[SlotTypeConfigurationTypeDef] = ...
     ) -> PutSlotTypeResponseTypeDef:
         """
@@ -562,15 +555,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Client.put_slot_type)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/client/#put_slot_type)
         """
     def start_import(
         self,
         *,
-        payload: Union[str, bytes, IO[Any], StreamingBody],
+        payload: BlobTypeDef,
         resourceType: ResourceTypeType,
         mergeStrategy: MergeStrategyType,
         tags: Sequence[TagTypeDef] = ...
     ) -> StartImportResponseTypeDef:
         """
         Starts a job to import a resource to Amazon Lex.
```

### Comparing `mypy-boto3-lex-models-1.28.15.post1/mypy_boto3_lex_models/literals.py` & `mypy-boto3-lex-models-1.28.16/mypy_boto3_lex_models/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lex-models-1.28.15.post1/mypy_boto3_lex_models/literals.pyi` & `mypy-boto3-lex-models-1.28.16/mypy_boto3_lex_models/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lex-models-1.28.15.post1/mypy_boto3_lex_models/paginator.py` & `mypy-boto3-lex-models-1.28.16/mypy_boto3_lex_models/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lex-models-1.28.15.post1/mypy_boto3_lex_models/paginator.pyi` & `mypy-boto3-lex-models-1.28.16/mypy_boto3_lex_models/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lex-models-1.28.15.post1/mypy_boto3_lex_models/type_defs.py` & `mypy-boto3-lex-models-1.28.16/mypy_boto3_lex_models/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for lex-models service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_lex_models.type_defs import BotChannelAssociationTypeDef
+    from mypy_boto3_lex_models.type_defs import BlobTypeDef
 
-    data: BotChannelAssociationTypeDef = {...}
+    data: BlobTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -46,14 +46,15 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
+    "BlobTypeDef",
     "BotChannelAssociationTypeDef",
     "BotMetadataTypeDef",
     "BuiltinIntentMetadataTypeDef",
     "BuiltinIntentSlotTypeDef",
     "BuiltinSlotTypeMetadataTypeDef",
     "CodeHookTypeDef",
     "LogSettingsRequestTypeDef",
@@ -121,14 +122,15 @@
     "GetBotsResponseTypeDef",
     "GetBuiltinIntentResponseTypeDef",
     "GetBuiltinIntentsResponseTypeDef",
     "GetBuiltinSlotTypesResponseTypeDef",
     "GetExportResponseTypeDef",
     "GetImportResponseTypeDef",
     "StartMigrationResponseTypeDef",
+    "EnumerationValueUnionTypeDef",
     "GetBotAliasesRequestGetBotAliasesPaginateTypeDef",
     "GetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef",
     "GetBotVersionsRequestGetBotVersionsPaginateTypeDef",
     "GetBotsRequestGetBotsPaginateTypeDef",
     "GetBuiltinIntentsRequestGetBuiltinIntentsPaginateTypeDef",
     "GetBuiltinSlotTypesRequestGetBuiltinSlotTypesPaginateTypeDef",
     "GetIntentVersionsRequestGetIntentVersionsPaginateTypeDef",
@@ -153,34 +155,39 @@
     "SlotDefaultValueSpecTypeDef",
     "SlotTypeConfigurationTypeDef",
     "UtteranceListTypeDef",
     "PutBotAliasRequestRequestTypeDef",
     "BotAliasMetadataTypeDef",
     "GetBotAliasResponseTypeDef",
     "PutBotAliasResponseTypeDef",
+    "PromptUnionTypeDef",
     "CreateBotVersionResponseTypeDef",
     "FollowUpPromptOutputTypeDef",
     "GetBotResponseTypeDef",
     "PutBotResponseTypeDef",
     "FollowUpPromptTypeDef",
     "PutBotRequestRequestTypeDef",
+    "StatementUnionTypeDef",
     "SlotOutputTypeDef",
     "SlotTypeDef",
     "CreateSlotTypeVersionResponseTypeDef",
     "GetSlotTypeResponseTypeDef",
     "PutSlotTypeRequestRequestTypeDef",
     "PutSlotTypeResponseTypeDef",
     "GetUtterancesViewResponseTypeDef",
     "GetBotAliasesResponseTypeDef",
+    "FollowUpPromptUnionTypeDef",
     "CreateIntentVersionResponseTypeDef",
     "GetIntentResponseTypeDef",
     "PutIntentResponseTypeDef",
+    "SlotUnionTypeDef",
     "PutIntentRequestRequestTypeDef",
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 BotChannelAssociationTypeDef = TypedDict(
     "BotChannelAssociationTypeDef",
     {
         "name": str,
         "description": str,
         "botAlias": str,
         "botName": str,
@@ -1064,14 +1071,15 @@
         "migrationId": str,
         "migrationStrategy": MigrationStrategyType,
         "migrationTimestamp": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+EnumerationValueUnionTypeDef = Union[EnumerationValueTypeDef, EnumerationValueOutputTypeDef]
 _RequiredGetBotAliasesRequestGetBotAliasesPaginateTypeDef = TypedDict(
     "_RequiredGetBotAliasesRequestGetBotAliasesPaginateTypeDef",
     {
         "botName": str,
     },
 )
 _OptionalGetBotAliasesRequestGetBotAliasesPaginateTypeDef = TypedDict(
@@ -1297,15 +1305,15 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredStartImportRequestRequestTypeDef = TypedDict(
     "_RequiredStartImportRequestRequestTypeDef",
     {
-        "payload": Union[str, bytes, IO[Any], StreamingBody],
+        "payload": BlobTypeDef,
         "resourceType": ResourceTypeType,
         "mergeStrategy": MergeStrategyType,
     },
 )
 _OptionalStartImportRequestRequestTypeDef = TypedDict(
     "_OptionalStartImportRequestRequestTypeDef",
     {
@@ -1520,14 +1528,15 @@
         "checksum": str,
         "conversationLogs": ConversationLogsResponseTypeDef,
         "tags": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+PromptUnionTypeDef = Union[PromptTypeDef, PromptOutputTypeDef]
 CreateBotVersionResponseTypeDef = TypedDict(
     "CreateBotVersionResponseTypeDef",
     {
         "name": str,
         "description": str,
         "intents": List[IntentTypeDef],
         "clarificationPrompt": PromptOutputTypeDef,
@@ -1647,14 +1656,15 @@
 
 class PutBotRequestRequestTypeDef(
     _RequiredPutBotRequestRequestTypeDef, _OptionalPutBotRequestRequestTypeDef
 ):
     pass
 
 
+StatementUnionTypeDef = Union[StatementTypeDef, StatementOutputTypeDef]
 _RequiredSlotOutputTypeDef = TypedDict(
     "_RequiredSlotOutputTypeDef",
     {
         "name": str,
         "slotConstraint": SlotConstraintType,
     },
 )
@@ -1747,17 +1757,15 @@
         "name": str,
     },
 )
 _OptionalPutSlotTypeRequestRequestTypeDef = TypedDict(
     "_OptionalPutSlotTypeRequestRequestTypeDef",
     {
         "description": str,
-        "enumerationValues": Sequence[
-            Union[EnumerationValueTypeDef, EnumerationValueOutputTypeDef]
-        ],
+        "enumerationValues": Sequence[EnumerationValueUnionTypeDef],
         "checksum": str,
         "valueSelectionStrategy": SlotValueSelectionStrategyType,
         "createVersion": bool,
         "parentSlotTypeSignature": str,
         "slotTypeConfigurations": Sequence[SlotTypeConfigurationTypeDef],
     },
     total=False,
@@ -1802,14 +1810,15 @@
     {
         "BotAliases": List[BotAliasMetadataTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+FollowUpPromptUnionTypeDef = Union[FollowUpPromptTypeDef, FollowUpPromptOutputTypeDef]
 CreateIntentVersionResponseTypeDef = TypedDict(
     "CreateIntentVersionResponseTypeDef",
     {
         "name": str,
         "description": str,
         "slots": List[SlotOutputTypeDef],
         "sampleUtterances": List[str],
@@ -1878,25 +1887,26 @@
         "kendraConfiguration": KendraConfigurationTypeDef,
         "inputContexts": List[InputContextTypeDef],
         "outputContexts": List[OutputContextTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+SlotUnionTypeDef = Union[SlotTypeDef, SlotOutputTypeDef]
 _RequiredPutIntentRequestRequestTypeDef = TypedDict(
     "_RequiredPutIntentRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalPutIntentRequestRequestTypeDef = TypedDict(
     "_OptionalPutIntentRequestRequestTypeDef",
     {
         "description": str,
-        "slots": Sequence[Union[SlotTypeDef, SlotOutputTypeDef]],
+        "slots": Sequence[SlotUnionTypeDef],
         "sampleUtterances": Sequence[str],
         "confirmationPrompt": PromptTypeDef,
         "rejectionStatement": StatementTypeDef,
         "followUpPrompt": FollowUpPromptTypeDef,
         "conclusionStatement": StatementTypeDef,
         "dialogCodeHook": CodeHookTypeDef,
         "fulfillmentActivity": FulfillmentActivityTypeDef,
```

### Comparing `mypy-boto3-lex-models-1.28.15.post1/mypy_boto3_lex_models/type_defs.pyi` & `mypy-boto3-lex-models-1.28.16/mypy_boto3_lex_models/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for lex-models service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_lex_models.type_defs import BotChannelAssociationTypeDef
+    from mypy_boto3_lex_models.type_defs import BlobTypeDef
 
-    data: BotChannelAssociationTypeDef = {...}
+    data: BlobTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -45,14 +45,15 @@
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
+    "BlobTypeDef",
     "BotChannelAssociationTypeDef",
     "BotMetadataTypeDef",
     "BuiltinIntentMetadataTypeDef",
     "BuiltinIntentSlotTypeDef",
     "BuiltinSlotTypeMetadataTypeDef",
     "CodeHookTypeDef",
     "LogSettingsRequestTypeDef",
@@ -120,14 +121,15 @@
     "GetBotsResponseTypeDef",
     "GetBuiltinIntentResponseTypeDef",
     "GetBuiltinIntentsResponseTypeDef",
     "GetBuiltinSlotTypesResponseTypeDef",
     "GetExportResponseTypeDef",
     "GetImportResponseTypeDef",
     "StartMigrationResponseTypeDef",
+    "EnumerationValueUnionTypeDef",
     "GetBotAliasesRequestGetBotAliasesPaginateTypeDef",
     "GetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef",
     "GetBotVersionsRequestGetBotVersionsPaginateTypeDef",
     "GetBotsRequestGetBotsPaginateTypeDef",
     "GetBuiltinIntentsRequestGetBuiltinIntentsPaginateTypeDef",
     "GetBuiltinSlotTypesRequestGetBuiltinSlotTypesPaginateTypeDef",
     "GetIntentVersionsRequestGetIntentVersionsPaginateTypeDef",
@@ -152,34 +154,39 @@
     "SlotDefaultValueSpecTypeDef",
     "SlotTypeConfigurationTypeDef",
     "UtteranceListTypeDef",
     "PutBotAliasRequestRequestTypeDef",
     "BotAliasMetadataTypeDef",
     "GetBotAliasResponseTypeDef",
     "PutBotAliasResponseTypeDef",
+    "PromptUnionTypeDef",
     "CreateBotVersionResponseTypeDef",
     "FollowUpPromptOutputTypeDef",
     "GetBotResponseTypeDef",
     "PutBotResponseTypeDef",
     "FollowUpPromptTypeDef",
     "PutBotRequestRequestTypeDef",
+    "StatementUnionTypeDef",
     "SlotOutputTypeDef",
     "SlotTypeDef",
     "CreateSlotTypeVersionResponseTypeDef",
     "GetSlotTypeResponseTypeDef",
     "PutSlotTypeRequestRequestTypeDef",
     "PutSlotTypeResponseTypeDef",
     "GetUtterancesViewResponseTypeDef",
     "GetBotAliasesResponseTypeDef",
+    "FollowUpPromptUnionTypeDef",
     "CreateIntentVersionResponseTypeDef",
     "GetIntentResponseTypeDef",
     "PutIntentResponseTypeDef",
+    "SlotUnionTypeDef",
     "PutIntentRequestRequestTypeDef",
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 BotChannelAssociationTypeDef = TypedDict(
     "BotChannelAssociationTypeDef",
     {
         "name": str,
         "description": str,
         "botAlias": str,
         "botName": str,
@@ -1035,14 +1042,15 @@
         "migrationId": str,
         "migrationStrategy": MigrationStrategyType,
         "migrationTimestamp": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+EnumerationValueUnionTypeDef = Union[EnumerationValueTypeDef, EnumerationValueOutputTypeDef]
 _RequiredGetBotAliasesRequestGetBotAliasesPaginateTypeDef = TypedDict(
     "_RequiredGetBotAliasesRequestGetBotAliasesPaginateTypeDef",
     {
         "botName": str,
     },
 )
 _OptionalGetBotAliasesRequestGetBotAliasesPaginateTypeDef = TypedDict(
@@ -1258,15 +1266,15 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredStartImportRequestRequestTypeDef = TypedDict(
     "_RequiredStartImportRequestRequestTypeDef",
     {
-        "payload": Union[str, bytes, IO[Any], StreamingBody],
+        "payload": BlobTypeDef,
         "resourceType": ResourceTypeType,
         "mergeStrategy": MergeStrategyType,
     },
 )
 _OptionalStartImportRequestRequestTypeDef = TypedDict(
     "_OptionalStartImportRequestRequestTypeDef",
     {
@@ -1469,14 +1477,15 @@
         "checksum": str,
         "conversationLogs": ConversationLogsResponseTypeDef,
         "tags": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+PromptUnionTypeDef = Union[PromptTypeDef, PromptOutputTypeDef]
 CreateBotVersionResponseTypeDef = TypedDict(
     "CreateBotVersionResponseTypeDef",
     {
         "name": str,
         "description": str,
         "intents": List[IntentTypeDef],
         "clarificationPrompt": PromptOutputTypeDef,
@@ -1594,14 +1603,15 @@
 )
 
 class PutBotRequestRequestTypeDef(
     _RequiredPutBotRequestRequestTypeDef, _OptionalPutBotRequestRequestTypeDef
 ):
     pass
 
+StatementUnionTypeDef = Union[StatementTypeDef, StatementOutputTypeDef]
 _RequiredSlotOutputTypeDef = TypedDict(
     "_RequiredSlotOutputTypeDef",
     {
         "name": str,
         "slotConstraint": SlotConstraintType,
     },
 )
@@ -1690,17 +1700,15 @@
         "name": str,
     },
 )
 _OptionalPutSlotTypeRequestRequestTypeDef = TypedDict(
     "_OptionalPutSlotTypeRequestRequestTypeDef",
     {
         "description": str,
-        "enumerationValues": Sequence[
-            Union[EnumerationValueTypeDef, EnumerationValueOutputTypeDef]
-        ],
+        "enumerationValues": Sequence[EnumerationValueUnionTypeDef],
         "checksum": str,
         "valueSelectionStrategy": SlotValueSelectionStrategyType,
         "createVersion": bool,
         "parentSlotTypeSignature": str,
         "slotTypeConfigurations": Sequence[SlotTypeConfigurationTypeDef],
     },
     total=False,
@@ -1743,14 +1751,15 @@
     {
         "BotAliases": List[BotAliasMetadataTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+FollowUpPromptUnionTypeDef = Union[FollowUpPromptTypeDef, FollowUpPromptOutputTypeDef]
 CreateIntentVersionResponseTypeDef = TypedDict(
     "CreateIntentVersionResponseTypeDef",
     {
         "name": str,
         "description": str,
         "slots": List[SlotOutputTypeDef],
         "sampleUtterances": List[str],
@@ -1819,25 +1828,26 @@
         "kendraConfiguration": KendraConfigurationTypeDef,
         "inputContexts": List[InputContextTypeDef],
         "outputContexts": List[OutputContextTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+SlotUnionTypeDef = Union[SlotTypeDef, SlotOutputTypeDef]
 _RequiredPutIntentRequestRequestTypeDef = TypedDict(
     "_RequiredPutIntentRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalPutIntentRequestRequestTypeDef = TypedDict(
     "_OptionalPutIntentRequestRequestTypeDef",
     {
         "description": str,
-        "slots": Sequence[Union[SlotTypeDef, SlotOutputTypeDef]],
+        "slots": Sequence[SlotUnionTypeDef],
         "sampleUtterances": Sequence[str],
         "confirmationPrompt": PromptTypeDef,
         "rejectionStatement": StatementTypeDef,
         "followUpPrompt": FollowUpPromptTypeDef,
         "conclusionStatement": StatementTypeDef,
         "dialogCodeHook": CodeHookTypeDef,
         "fulfillmentActivity": FulfillmentActivityTypeDef,
```

### Comparing `mypy-boto3-lex-models-1.28.15.post1/mypy_boto3_lex_models.egg-info/PKG-INFO` & `mypy-boto3-lex-models-1.28.16/mypy_boto3_lex_models.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-lex-models
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.LexModelBuildingService 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.LexModelBuildingService 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 lex-models type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 lex-models type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lex-models.svg?color=blue)](https://pypi.org/project/mypy-boto3-lex-models)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-lex-models)](https://pepy.tech/project/mypy-boto3-lex-models)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LexModelBuildingService 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService)
+[boto3.LexModelBuildingService 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService)
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
 [mypy-boto3-lex-models docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/).
 
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
@@ -372,23 +372,24 @@
 )
 
 
 def check_value(value: ChannelStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_lex_models.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_lex_models.type_defs import (
+    BlobTypeDef,
     BotChannelAssociationTypeDef,
     BotMetadataTypeDef,
     BuiltinIntentMetadataTypeDef,
     BuiltinIntentSlotTypeDef,
     BuiltinSlotTypeMetadataTypeDef,
     CodeHookTypeDef,
     LogSettingsRequestTypeDef,
@@ -456,14 +457,15 @@
     GetBotsResponseTypeDef,
     GetBuiltinIntentResponseTypeDef,
     GetBuiltinIntentsResponseTypeDef,
     GetBuiltinSlotTypesResponseTypeDef,
     GetExportResponseTypeDef,
     GetImportResponseTypeDef,
     StartMigrationResponseTypeDef,
+    EnumerationValueUnionTypeDef,
     GetBotAliasesRequestGetBotAliasesPaginateTypeDef,
     GetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef,
     GetBotVersionsRequestGetBotVersionsPaginateTypeDef,
     GetBotsRequestGetBotsPaginateTypeDef,
     GetBuiltinIntentsRequestGetBuiltinIntentsPaginateTypeDef,
     GetBuiltinSlotTypesRequestGetBuiltinSlotTypesPaginateTypeDef,
     GetIntentVersionsRequestGetIntentVersionsPaginateTypeDef,
@@ -488,36 +490,40 @@
     SlotDefaultValueSpecTypeDef,
     SlotTypeConfigurationTypeDef,
     UtteranceListTypeDef,
     PutBotAliasRequestRequestTypeDef,
     BotAliasMetadataTypeDef,
     GetBotAliasResponseTypeDef,
     PutBotAliasResponseTypeDef,
+    PromptUnionTypeDef,
     CreateBotVersionResponseTypeDef,
     FollowUpPromptOutputTypeDef,
     GetBotResponseTypeDef,
     PutBotResponseTypeDef,
     FollowUpPromptTypeDef,
     PutBotRequestRequestTypeDef,
+    StatementUnionTypeDef,
     SlotOutputTypeDef,
     SlotTypeDef,
     CreateSlotTypeVersionResponseTypeDef,
     GetSlotTypeResponseTypeDef,
     PutSlotTypeRequestRequestTypeDef,
     PutSlotTypeResponseTypeDef,
     GetUtterancesViewResponseTypeDef,
     GetBotAliasesResponseTypeDef,
+    FollowUpPromptUnionTypeDef,
     CreateIntentVersionResponseTypeDef,
     GetIntentResponseTypeDef,
     PutIntentResponseTypeDef,
+    SlotUnionTypeDef,
     PutIntentRequestRequestTypeDef,
 )
 
 
-def get_structure() -> BotChannelAssociationTypeDef:
+def get_value() -> BlobTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-lex-models-1.28.15.post1/mypy_boto3_lex_models.egg-info/SOURCES.txt` & `mypy-boto3-lex-models-1.28.16/mypy_boto3_lex_models.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lex-models-1.28.15.post1/setup.py` & `mypy-boto3-lex-models-1.28.16/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-lex-models",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_lex_models"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.LexModelBuildingService 1.28.15 service generated with"
-        " mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.LexModelBuildingService 1.28.16 service generated with"
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
-    keywords="boto3 lex-models type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 lex-models type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_lex_models": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

