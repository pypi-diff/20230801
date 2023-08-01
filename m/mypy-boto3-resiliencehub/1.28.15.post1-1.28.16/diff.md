# Comparing `tmp/mypy-boto3-resiliencehub-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-resiliencehub-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-resiliencehub-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:59 2023, max compression
+gzip compressed data, was "mypy-boto3-resiliencehub-1.28.16.tar", last modified: Tue Aug  1 11:37:40 2023, max compression
```

## Comparing `mypy-boto3-resiliencehub-1.28.15.post1.tar` & `mypy-boto3-resiliencehub-1.28.16.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:59.649360 mypy-boto3-resiliencehub-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:57:00.000000 mypy-boto3-resiliencehub-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18742 2023-07-29 10:03:59.629359 mypy-boto3-resiliencehub-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17225 2023-07-29 09:57:00.000000 mypy-boto3-resiliencehub-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:59.629359 mypy-boto3-resiliencehub-1.28.15.post1/mypy_boto3_resiliencehub/
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-07-29 09:57:00.000000 mypy-boto3-resiliencehub-1.28.15.post1/mypy_boto3_resiliencehub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-29 09:57:00.000000 mypy-boto3-resiliencehub-1.28.15.post1/mypy_boto3_resiliencehub/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-29 09:57:00.000000 mypy-boto3-resiliencehub-1.28.15.post1/mypy_boto3_resiliencehub/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39638 2023-07-29 09:57:01.000000 mypy-boto3-resiliencehub-1.28.15.post1/mypy_boto3_resiliencehub/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    39580 2023-07-29 09:57:00.000000 mypy-boto3-resiliencehub-1.28.15.post1/mypy_boto3_resiliencehub/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10983 2023-07-29 09:57:01.000000 mypy-boto3-resiliencehub-1.28.15.post1/mypy_boto3_resiliencehub/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10981 2023-07-29 09:57:01.000000 mypy-boto3-resiliencehub-1.28.15.post1/mypy_boto3_resiliencehub/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:57:00.000000 mypy-boto3-resiliencehub-1.28.15.post1/mypy_boto3_resiliencehub/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    60998 2023-07-29 09:57:03.000000 mypy-boto3-resiliencehub-1.28.15.post1/mypy_boto3_resiliencehub/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    60893 2023-07-29 09:57:02.000000 mypy-boto3-resiliencehub-1.28.15.post1/mypy_boto3_resiliencehub/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:57:00.000000 mypy-boto3-resiliencehub-1.28.15.post1/mypy_boto3_resiliencehub/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:59.629359 mypy-boto3-resiliencehub-1.28.15.post1/mypy_boto3_resiliencehub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18742 2023-07-29 10:03:59.000000 mypy-boto3-resiliencehub-1.28.15.post1/mypy_boto3_resiliencehub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-29 10:03:59.000000 mypy-boto3-resiliencehub-1.28.15.post1/mypy_boto3_resiliencehub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:59.000000 mypy-boto3-resiliencehub-1.28.15.post1/mypy_boto3_resiliencehub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:59.000000 mypy-boto3-resiliencehub-1.28.15.post1/mypy_boto3_resiliencehub.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:59.000000 mypy-boto3-resiliencehub-1.28.15.post1/mypy_boto3_resiliencehub.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-29 10:03:59.000000 mypy-boto3-resiliencehub-1.28.15.post1/mypy_boto3_resiliencehub.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:59.649360 mypy-boto3-resiliencehub-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-29 09:57:00.000000 mypy-boto3-resiliencehub-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:40.264770 mypy-boto3-resiliencehub-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:30:22.000000 mypy-boto3-resiliencehub-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18759 2023-08-01 11:37:40.260770 mypy-boto3-resiliencehub-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17251 2023-08-01 11:30:22.000000 mypy-boto3-resiliencehub-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:40.248770 mypy-boto3-resiliencehub-1.28.16/mypy_boto3_resiliencehub/
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-08-01 11:30:22.000000 mypy-boto3-resiliencehub-1.28.16/mypy_boto3_resiliencehub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-08-01 11:30:22.000000 mypy-boto3-resiliencehub-1.28.16/mypy_boto3_resiliencehub/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-08-01 11:30:22.000000 mypy-boto3-resiliencehub-1.28.16/mypy_boto3_resiliencehub/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39582 2023-08-01 11:30:22.000000 mypy-boto3-resiliencehub-1.28.16/mypy_boto3_resiliencehub/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39524 2023-08-01 11:30:22.000000 mypy-boto3-resiliencehub-1.28.16/mypy_boto3_resiliencehub/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10983 2023-08-01 11:30:23.000000 mypy-boto3-resiliencehub-1.28.16/mypy_boto3_resiliencehub/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10981 2023-08-01 11:30:23.000000 mypy-boto3-resiliencehub-1.28.16/mypy_boto3_resiliencehub/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:30:22.000000 mypy-boto3-resiliencehub-1.28.16/mypy_boto3_resiliencehub/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    61071 2023-08-01 11:30:24.000000 mypy-boto3-resiliencehub-1.28.16/mypy_boto3_resiliencehub/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60966 2023-08-01 11:30:24.000000 mypy-boto3-resiliencehub-1.28.16/mypy_boto3_resiliencehub/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:30:22.000000 mypy-boto3-resiliencehub-1.28.16/mypy_boto3_resiliencehub/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:40.260770 mypy-boto3-resiliencehub-1.28.16/mypy_boto3_resiliencehub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18759 2023-08-01 11:37:39.000000 mypy-boto3-resiliencehub-1.28.16/mypy_boto3_resiliencehub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-08-01 11:37:40.000000 mypy-boto3-resiliencehub-1.28.16/mypy_boto3_resiliencehub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:39.000000 mypy-boto3-resiliencehub-1.28.16/mypy_boto3_resiliencehub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:39.000000 mypy-boto3-resiliencehub-1.28.16/mypy_boto3_resiliencehub.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:39.000000 mypy-boto3-resiliencehub-1.28.16/mypy_boto3_resiliencehub.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-01 11:37:39.000000 mypy-boto3-resiliencehub-1.28.16/mypy_boto3_resiliencehub.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:40.264770 mypy-boto3-resiliencehub-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-08-01 11:30:22.000000 mypy-boto3-resiliencehub-1.28.16/setup.py
```

### Comparing `mypy-boto3-resiliencehub-1.28.15.post1/LICENSE` & `mypy-boto3-resiliencehub-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-resiliencehub-1.28.15.post1/PKG-INFO` & `mypy-boto3-resiliencehub-1.28.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-resiliencehub
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.ResilienceHub 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.ResilienceHub 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 resiliencehub type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 resiliencehub type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-resiliencehub.svg?color=blue)](https://pypi.org/project/mypy-boto3-resiliencehub)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-resiliencehub)](https://pepy.tech/project/mypy-boto3-resiliencehub)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ResilienceHub 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub)
+[boto3.ResilienceHub 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub)
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
 [mypy-boto3-resiliencehub docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/).
 
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
@@ -314,20 +314,20 @@
 )
 
 
 def check_value(value: AlarmTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_resiliencehub.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_resiliencehub.type_defs import (
     ResponseMetadataTypeDef,
     RecommendationItemTypeDef,
     CostTypeDef,
     DisruptionComplianceTypeDef,
@@ -425,15 +425,15 @@
     DeleteAppVersionResourceRequestRequestTypeDef,
     DescribeAppVersionResourceRequestRequestTypeDef,
     UpdateAppVersionResourceRequestRequestTypeDef,
     CreateResiliencyPolicyRequestRequestTypeDef,
     ResiliencyPolicyTypeDef,
     UpdateResiliencyPolicyRequestRequestTypeDef,
     ImportResourcesToDraftAppVersionResponseTypeDef,
-    ImportResourcesToDraftAppVersionRequestRequestTypeDef,
+    EksSourceUnionTypeDef,
     PhysicalResourceTypeDef,
     ResourceMappingTypeDef,
     UnsupportedResourceTypeDef,
     RecommendationTemplateTypeDef,
     ResourceErrorsDetailsTypeDef,
     ListAlarmRecommendationsResponseTypeDef,
     ListSopRecommendationsResponseTypeDef,
@@ -444,14 +444,15 @@
     ListAppInputSourcesResponseTypeDef,
     ComponentRecommendationTypeDef,
     CreateResiliencyPolicyResponseTypeDef,
     DescribeResiliencyPolicyResponseTypeDef,
     ListResiliencyPoliciesResponseTypeDef,
     ListSuggestedResiliencyPoliciesResponseTypeDef,
     UpdateResiliencyPolicyResponseTypeDef,
+    ImportResourcesToDraftAppVersionRequestRequestTypeDef,
     CreateAppVersionResourceResponseTypeDef,
     DeleteAppVersionResourceResponseTypeDef,
     DescribeAppVersionResourceResponseTypeDef,
     ListAppVersionResourcesResponseTypeDef,
     UpdateAppVersionResourceResponseTypeDef,
     AddDraftAppVersionResourceMappingsRequestRequestTypeDef,
     AddDraftAppVersionResourceMappingsResponseTypeDef,
@@ -462,15 +463,15 @@
     AppAssessmentTypeDef,
     ListAppComponentRecommendationsResponseTypeDef,
     DescribeAppAssessmentResponseTypeDef,
     StartAppAssessmentResponseTypeDef,
 )
 
 
-def get_structure() -> ResponseMetadataTypeDef:
+def get_value() -> ResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-resiliencehub-1.28.15.post1/README.md` & `mypy-boto3-resiliencehub-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-resiliencehub.svg?color=blue)](https://pypi.org/project/mypy-boto3-resiliencehub)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-resiliencehub)](https://pepy.tech/project/mypy-boto3-resiliencehub)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ResilienceHub 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub)
+[boto3.ResilienceHub 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub)
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
 [mypy-boto3-resiliencehub docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/).
 
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
@@ -282,20 +282,20 @@
 )
 
 
 def check_value(value: AlarmTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_resiliencehub.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_resiliencehub.type_defs import (
     ResponseMetadataTypeDef,
     RecommendationItemTypeDef,
     CostTypeDef,
     DisruptionComplianceTypeDef,
@@ -393,15 +393,15 @@
     DeleteAppVersionResourceRequestRequestTypeDef,
     DescribeAppVersionResourceRequestRequestTypeDef,
     UpdateAppVersionResourceRequestRequestTypeDef,
     CreateResiliencyPolicyRequestRequestTypeDef,
     ResiliencyPolicyTypeDef,
     UpdateResiliencyPolicyRequestRequestTypeDef,
     ImportResourcesToDraftAppVersionResponseTypeDef,
-    ImportResourcesToDraftAppVersionRequestRequestTypeDef,
+    EksSourceUnionTypeDef,
     PhysicalResourceTypeDef,
     ResourceMappingTypeDef,
     UnsupportedResourceTypeDef,
     RecommendationTemplateTypeDef,
     ResourceErrorsDetailsTypeDef,
     ListAlarmRecommendationsResponseTypeDef,
     ListSopRecommendationsResponseTypeDef,
@@ -412,14 +412,15 @@
     ListAppInputSourcesResponseTypeDef,
     ComponentRecommendationTypeDef,
     CreateResiliencyPolicyResponseTypeDef,
     DescribeResiliencyPolicyResponseTypeDef,
     ListResiliencyPoliciesResponseTypeDef,
     ListSuggestedResiliencyPoliciesResponseTypeDef,
     UpdateResiliencyPolicyResponseTypeDef,
+    ImportResourcesToDraftAppVersionRequestRequestTypeDef,
     CreateAppVersionResourceResponseTypeDef,
     DeleteAppVersionResourceResponseTypeDef,
     DescribeAppVersionResourceResponseTypeDef,
     ListAppVersionResourcesResponseTypeDef,
     UpdateAppVersionResourceResponseTypeDef,
     AddDraftAppVersionResourceMappingsRequestRequestTypeDef,
     AddDraftAppVersionResourceMappingsResponseTypeDef,
@@ -430,15 +431,15 @@
     AppAssessmentTypeDef,
     ListAppComponentRecommendationsResponseTypeDef,
     DescribeAppAssessmentResponseTypeDef,
     StartAppAssessmentResponseTypeDef,
 )
 
 
-def get_structure() -> ResponseMetadataTypeDef:
+def get_value() -> ResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-resiliencehub-1.28.15.post1/mypy_boto3_resiliencehub/__main__.py` & `mypy-boto3-resiliencehub-1.28.16/mypy_boto3_resiliencehub/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ResilienceHub 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.ResilienceHub 1.28.16\nVersion:         1.28.16\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub\nOther"
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

### Comparing `mypy-boto3-resiliencehub-1.28.15.post1/mypy_boto3_resiliencehub/client.py` & `mypy-boto3-resiliencehub-1.28.16/mypy_boto3_resiliencehub/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from boto3.session import Session
     from mypy_boto3_resiliencehub.client import ResilienceHubClient
 
     session = Session()
     client: ResilienceHubClient = session.client("resiliencehub")
     ```
 """
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AppAssessmentScheduleTypeType,
     AssessmentInvokerType,
     AssessmentStatusType,
@@ -50,16 +50,15 @@
     DescribeAppVersionResourceResponseTypeDef,
     DescribeAppVersionResourcesResolutionStatusResponseTypeDef,
     DescribeAppVersionResponseTypeDef,
     DescribeAppVersionTemplateResponseTypeDef,
     DescribeDraftAppVersionResourcesImportStatusResponseTypeDef,
     DescribeResiliencyPolicyResponseTypeDef,
     EksSourceClusterNamespaceTypeDef,
-    EksSourceOutputTypeDef,
-    EksSourceTypeDef,
+    EksSourceUnionTypeDef,
     FailurePolicyTypeDef,
     ImportResourcesToDraftAppVersionResponseTypeDef,
     ListAlarmRecommendationsResponseTypeDef,
     ListAppAssessmentsResponseTypeDef,
     ListAppComponentCompliancesResponseTypeDef,
     ListAppComponentRecommendationsResponseTypeDef,
     ListAppInputSourcesResponseTypeDef,
@@ -444,15 +443,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#generate_presigned_url)
         """
 
     def import_resources_to_draft_app_version(
         self,
         *,
         appArn: str,
-        eksSources: Sequence[Union[EksSourceTypeDef, EksSourceOutputTypeDef]] = ...,
+        eksSources: Sequence[EksSourceUnionTypeDef] = ...,
         importStrategy: ResourceImportStrategyTypeType = ...,
         sourceArns: Sequence[str] = ...,
         terraformSources: Sequence[TerraformSourceTypeDef] = ...
     ) -> ImportResourcesToDraftAppVersionResponseTypeDef:
         """
         Imports resources to Resilience Hub application draft version from different
         input sources.
```

### Comparing `mypy-boto3-resiliencehub-1.28.15.post1/mypy_boto3_resiliencehub/client.pyi` & `mypy-boto3-resiliencehub-1.28.16/mypy_boto3_resiliencehub/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from boto3.session import Session
     from mypy_boto3_resiliencehub.client import ResilienceHubClient
 
     session = Session()
     client: ResilienceHubClient = session.client("resiliencehub")
     ```
 """
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AppAssessmentScheduleTypeType,
     AssessmentInvokerType,
     AssessmentStatusType,
@@ -50,16 +50,15 @@
     DescribeAppVersionResourceResponseTypeDef,
     DescribeAppVersionResourcesResolutionStatusResponseTypeDef,
     DescribeAppVersionResponseTypeDef,
     DescribeAppVersionTemplateResponseTypeDef,
     DescribeDraftAppVersionResourcesImportStatusResponseTypeDef,
     DescribeResiliencyPolicyResponseTypeDef,
     EksSourceClusterNamespaceTypeDef,
-    EksSourceOutputTypeDef,
-    EksSourceTypeDef,
+    EksSourceUnionTypeDef,
     FailurePolicyTypeDef,
     ImportResourcesToDraftAppVersionResponseTypeDef,
     ListAlarmRecommendationsResponseTypeDef,
     ListAppAssessmentsResponseTypeDef,
     ListAppComponentCompliancesResponseTypeDef,
     ListAppComponentRecommendationsResponseTypeDef,
     ListAppInputSourcesResponseTypeDef,
@@ -415,15 +414,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/client/#generate_presigned_url)
         """
     def import_resources_to_draft_app_version(
         self,
         *,
         appArn: str,
-        eksSources: Sequence[Union[EksSourceTypeDef, EksSourceOutputTypeDef]] = ...,
+        eksSources: Sequence[EksSourceUnionTypeDef] = ...,
         importStrategy: ResourceImportStrategyTypeType = ...,
         sourceArns: Sequence[str] = ...,
         terraformSources: Sequence[TerraformSourceTypeDef] = ...
     ) -> ImportResourcesToDraftAppVersionResponseTypeDef:
         """
         Imports resources to Resilience Hub application draft version from different
         input sources.
```

### Comparing `mypy-boto3-resiliencehub-1.28.15.post1/mypy_boto3_resiliencehub/literals.py` & `mypy-boto3-resiliencehub-1.28.16/mypy_boto3_resiliencehub/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-resiliencehub-1.28.15.post1/mypy_boto3_resiliencehub/literals.pyi` & `mypy-boto3-resiliencehub-1.28.16/mypy_boto3_resiliencehub/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-resiliencehub-1.28.15.post1/mypy_boto3_resiliencehub/type_defs.py` & `mypy-boto3-resiliencehub-1.28.16/mypy_boto3_resiliencehub/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_resiliencehub.type_defs import ResponseMetadataTypeDef
 
-    data: ResponseMetadataTypeDef = {...}
+    data: ResponseMetadataTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -153,15 +153,15 @@
     "DeleteAppVersionResourceRequestRequestTypeDef",
     "DescribeAppVersionResourceRequestRequestTypeDef",
     "UpdateAppVersionResourceRequestRequestTypeDef",
     "CreateResiliencyPolicyRequestRequestTypeDef",
     "ResiliencyPolicyTypeDef",
     "UpdateResiliencyPolicyRequestRequestTypeDef",
     "ImportResourcesToDraftAppVersionResponseTypeDef",
-    "ImportResourcesToDraftAppVersionRequestRequestTypeDef",
+    "EksSourceUnionTypeDef",
     "PhysicalResourceTypeDef",
     "ResourceMappingTypeDef",
     "UnsupportedResourceTypeDef",
     "RecommendationTemplateTypeDef",
     "ResourceErrorsDetailsTypeDef",
     "ListAlarmRecommendationsResponseTypeDef",
     "ListSopRecommendationsResponseTypeDef",
@@ -172,14 +172,15 @@
     "ListAppInputSourcesResponseTypeDef",
     "ComponentRecommendationTypeDef",
     "CreateResiliencyPolicyResponseTypeDef",
     "DescribeResiliencyPolicyResponseTypeDef",
     "ListResiliencyPoliciesResponseTypeDef",
     "ListSuggestedResiliencyPoliciesResponseTypeDef",
     "UpdateResiliencyPolicyResponseTypeDef",
+    "ImportResourcesToDraftAppVersionRequestRequestTypeDef",
     "CreateAppVersionResourceResponseTypeDef",
     "DeleteAppVersionResourceResponseTypeDef",
     "DescribeAppVersionResourceResponseTypeDef",
     "ListAppVersionResourcesResponseTypeDef",
     "UpdateAppVersionResourceResponseTypeDef",
     "AddDraftAppVersionResourceMappingsRequestRequestTypeDef",
     "AddDraftAppVersionResourceMappingsResponseTypeDef",
@@ -1864,39 +1865,15 @@
         "sourceArns": List[str],
         "status": ResourceImportStatusTypeType,
         "terraformSources": List[TerraformSourceTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredImportResourcesToDraftAppVersionRequestRequestTypeDef = TypedDict(
-    "_RequiredImportResourcesToDraftAppVersionRequestRequestTypeDef",
-    {
-        "appArn": str,
-    },
-)
-_OptionalImportResourcesToDraftAppVersionRequestRequestTypeDef = TypedDict(
-    "_OptionalImportResourcesToDraftAppVersionRequestRequestTypeDef",
-    {
-        "eksSources": Sequence[Union[EksSourceTypeDef, EksSourceOutputTypeDef]],
-        "importStrategy": ResourceImportStrategyTypeType,
-        "sourceArns": Sequence[str],
-        "terraformSources": Sequence[TerraformSourceTypeDef],
-    },
-    total=False,
-)
-
-
-class ImportResourcesToDraftAppVersionRequestRequestTypeDef(
-    _RequiredImportResourcesToDraftAppVersionRequestRequestTypeDef,
-    _OptionalImportResourcesToDraftAppVersionRequestRequestTypeDef,
-):
-    pass
-
-
+EksSourceUnionTypeDef = Union[EksSourceTypeDef, EksSourceOutputTypeDef]
 _RequiredPhysicalResourceTypeDef = TypedDict(
     "_RequiredPhysicalResourceTypeDef",
     {
         "logicalResourceId": LogicalResourceIdTypeDef,
         "physicalResourceId": PhysicalResourceIdTypeDef,
         "resourceType": str,
     },
@@ -2119,14 +2096,39 @@
     "UpdateResiliencyPolicyResponseTypeDef",
     {
         "policy": ResiliencyPolicyTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredImportResourcesToDraftAppVersionRequestRequestTypeDef = TypedDict(
+    "_RequiredImportResourcesToDraftAppVersionRequestRequestTypeDef",
+    {
+        "appArn": str,
+    },
+)
+_OptionalImportResourcesToDraftAppVersionRequestRequestTypeDef = TypedDict(
+    "_OptionalImportResourcesToDraftAppVersionRequestRequestTypeDef",
+    {
+        "eksSources": Sequence[EksSourceUnionTypeDef],
+        "importStrategy": ResourceImportStrategyTypeType,
+        "sourceArns": Sequence[str],
+        "terraformSources": Sequence[TerraformSourceTypeDef],
+    },
+    total=False,
+)
+
+
+class ImportResourcesToDraftAppVersionRequestRequestTypeDef(
+    _RequiredImportResourcesToDraftAppVersionRequestRequestTypeDef,
+    _OptionalImportResourcesToDraftAppVersionRequestRequestTypeDef,
+):
+    pass
+
+
 CreateAppVersionResourceResponseTypeDef = TypedDict(
     "CreateAppVersionResourceResponseTypeDef",
     {
         "appArn": str,
         "appVersion": str,
         "physicalResource": PhysicalResourceTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
```

### Comparing `mypy-boto3-resiliencehub-1.28.15.post1/mypy_boto3_resiliencehub/type_defs.pyi` & `mypy-boto3-resiliencehub-1.28.16/mypy_boto3_resiliencehub/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_resiliencehub.type_defs import ResponseMetadataTypeDef
 
-    data: ResponseMetadataTypeDef = {...}
+    data: ResponseMetadataTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -152,15 +152,15 @@
     "DeleteAppVersionResourceRequestRequestTypeDef",
     "DescribeAppVersionResourceRequestRequestTypeDef",
     "UpdateAppVersionResourceRequestRequestTypeDef",
     "CreateResiliencyPolicyRequestRequestTypeDef",
     "ResiliencyPolicyTypeDef",
     "UpdateResiliencyPolicyRequestRequestTypeDef",
     "ImportResourcesToDraftAppVersionResponseTypeDef",
-    "ImportResourcesToDraftAppVersionRequestRequestTypeDef",
+    "EksSourceUnionTypeDef",
     "PhysicalResourceTypeDef",
     "ResourceMappingTypeDef",
     "UnsupportedResourceTypeDef",
     "RecommendationTemplateTypeDef",
     "ResourceErrorsDetailsTypeDef",
     "ListAlarmRecommendationsResponseTypeDef",
     "ListSopRecommendationsResponseTypeDef",
@@ -171,14 +171,15 @@
     "ListAppInputSourcesResponseTypeDef",
     "ComponentRecommendationTypeDef",
     "CreateResiliencyPolicyResponseTypeDef",
     "DescribeResiliencyPolicyResponseTypeDef",
     "ListResiliencyPoliciesResponseTypeDef",
     "ListSuggestedResiliencyPoliciesResponseTypeDef",
     "UpdateResiliencyPolicyResponseTypeDef",
+    "ImportResourcesToDraftAppVersionRequestRequestTypeDef",
     "CreateAppVersionResourceResponseTypeDef",
     "DeleteAppVersionResourceResponseTypeDef",
     "DescribeAppVersionResourceResponseTypeDef",
     "ListAppVersionResourcesResponseTypeDef",
     "UpdateAppVersionResourceResponseTypeDef",
     "AddDraftAppVersionResourceMappingsRequestRequestTypeDef",
     "AddDraftAppVersionResourceMappingsResponseTypeDef",
@@ -1771,37 +1772,15 @@
         "sourceArns": List[str],
         "status": ResourceImportStatusTypeType,
         "terraformSources": List[TerraformSourceTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredImportResourcesToDraftAppVersionRequestRequestTypeDef = TypedDict(
-    "_RequiredImportResourcesToDraftAppVersionRequestRequestTypeDef",
-    {
-        "appArn": str,
-    },
-)
-_OptionalImportResourcesToDraftAppVersionRequestRequestTypeDef = TypedDict(
-    "_OptionalImportResourcesToDraftAppVersionRequestRequestTypeDef",
-    {
-        "eksSources": Sequence[Union[EksSourceTypeDef, EksSourceOutputTypeDef]],
-        "importStrategy": ResourceImportStrategyTypeType,
-        "sourceArns": Sequence[str],
-        "terraformSources": Sequence[TerraformSourceTypeDef],
-    },
-    total=False,
-)
-
-class ImportResourcesToDraftAppVersionRequestRequestTypeDef(
-    _RequiredImportResourcesToDraftAppVersionRequestRequestTypeDef,
-    _OptionalImportResourcesToDraftAppVersionRequestRequestTypeDef,
-):
-    pass
-
+EksSourceUnionTypeDef = Union[EksSourceTypeDef, EksSourceOutputTypeDef]
 _RequiredPhysicalResourceTypeDef = TypedDict(
     "_RequiredPhysicalResourceTypeDef",
     {
         "logicalResourceId": LogicalResourceIdTypeDef,
         "physicalResourceId": PhysicalResourceIdTypeDef,
         "resourceType": str,
     },
@@ -2016,14 +1995,37 @@
     "UpdateResiliencyPolicyResponseTypeDef",
     {
         "policy": ResiliencyPolicyTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredImportResourcesToDraftAppVersionRequestRequestTypeDef = TypedDict(
+    "_RequiredImportResourcesToDraftAppVersionRequestRequestTypeDef",
+    {
+        "appArn": str,
+    },
+)
+_OptionalImportResourcesToDraftAppVersionRequestRequestTypeDef = TypedDict(
+    "_OptionalImportResourcesToDraftAppVersionRequestRequestTypeDef",
+    {
+        "eksSources": Sequence[EksSourceUnionTypeDef],
+        "importStrategy": ResourceImportStrategyTypeType,
+        "sourceArns": Sequence[str],
+        "terraformSources": Sequence[TerraformSourceTypeDef],
+    },
+    total=False,
+)
+
+class ImportResourcesToDraftAppVersionRequestRequestTypeDef(
+    _RequiredImportResourcesToDraftAppVersionRequestRequestTypeDef,
+    _OptionalImportResourcesToDraftAppVersionRequestRequestTypeDef,
+):
+    pass
+
 CreateAppVersionResourceResponseTypeDef = TypedDict(
     "CreateAppVersionResourceResponseTypeDef",
     {
         "appArn": str,
         "appVersion": str,
         "physicalResource": PhysicalResourceTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
```

### Comparing `mypy-boto3-resiliencehub-1.28.15.post1/mypy_boto3_resiliencehub.egg-info/PKG-INFO` & `mypy-boto3-resiliencehub-1.28.16/mypy_boto3_resiliencehub.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-resiliencehub
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.ResilienceHub 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.ResilienceHub 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 resiliencehub type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 resiliencehub type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-resiliencehub.svg?color=blue)](https://pypi.org/project/mypy-boto3-resiliencehub)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-resiliencehub)](https://pepy.tech/project/mypy-boto3-resiliencehub)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ResilienceHub 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub)
+[boto3.ResilienceHub 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub)
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
 [mypy-boto3-resiliencehub docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/).
 
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
@@ -314,20 +314,20 @@
 )
 
 
 def check_value(value: AlarmTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_resiliencehub.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_resiliencehub.type_defs import (
     ResponseMetadataTypeDef,
     RecommendationItemTypeDef,
     CostTypeDef,
     DisruptionComplianceTypeDef,
@@ -425,15 +425,15 @@
     DeleteAppVersionResourceRequestRequestTypeDef,
     DescribeAppVersionResourceRequestRequestTypeDef,
     UpdateAppVersionResourceRequestRequestTypeDef,
     CreateResiliencyPolicyRequestRequestTypeDef,
     ResiliencyPolicyTypeDef,
     UpdateResiliencyPolicyRequestRequestTypeDef,
     ImportResourcesToDraftAppVersionResponseTypeDef,
-    ImportResourcesToDraftAppVersionRequestRequestTypeDef,
+    EksSourceUnionTypeDef,
     PhysicalResourceTypeDef,
     ResourceMappingTypeDef,
     UnsupportedResourceTypeDef,
     RecommendationTemplateTypeDef,
     ResourceErrorsDetailsTypeDef,
     ListAlarmRecommendationsResponseTypeDef,
     ListSopRecommendationsResponseTypeDef,
@@ -444,14 +444,15 @@
     ListAppInputSourcesResponseTypeDef,
     ComponentRecommendationTypeDef,
     CreateResiliencyPolicyResponseTypeDef,
     DescribeResiliencyPolicyResponseTypeDef,
     ListResiliencyPoliciesResponseTypeDef,
     ListSuggestedResiliencyPoliciesResponseTypeDef,
     UpdateResiliencyPolicyResponseTypeDef,
+    ImportResourcesToDraftAppVersionRequestRequestTypeDef,
     CreateAppVersionResourceResponseTypeDef,
     DeleteAppVersionResourceResponseTypeDef,
     DescribeAppVersionResourceResponseTypeDef,
     ListAppVersionResourcesResponseTypeDef,
     UpdateAppVersionResourceResponseTypeDef,
     AddDraftAppVersionResourceMappingsRequestRequestTypeDef,
     AddDraftAppVersionResourceMappingsResponseTypeDef,
@@ -462,15 +463,15 @@
     AppAssessmentTypeDef,
     ListAppComponentRecommendationsResponseTypeDef,
     DescribeAppAssessmentResponseTypeDef,
     StartAppAssessmentResponseTypeDef,
 )
 
 
-def get_structure() -> ResponseMetadataTypeDef:
+def get_value() -> ResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-resiliencehub-1.28.15.post1/mypy_boto3_resiliencehub.egg-info/SOURCES.txt` & `mypy-boto3-resiliencehub-1.28.16/mypy_boto3_resiliencehub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-resiliencehub-1.28.15.post1/setup.py` & `mypy-boto3-resiliencehub-1.28.16/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-resiliencehub",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_resiliencehub"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ResilienceHub 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.2"
+        "Type annotations for boto3.ResilienceHub 1.28.16 service generated with mypy-boto3-builder"
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
-    keywords="boto3 resiliencehub type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 resiliencehub type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_resiliencehub": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

