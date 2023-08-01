# Comparing `tmp/mypy-boto3-inspector-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-inspector-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-inspector-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:17 2023, max compression
+gzip compressed data, was "mypy-boto3-inspector-1.28.16.tar", last modified: Tue Aug  1 11:36:56 2023, max compression
```

## Comparing `mypy-boto3-inspector-1.28.15.post1.tar` & `mypy-boto3-inspector-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:17.033174 mypy-boto3-inspector-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:47:15.000000 mypy-boto3-inspector-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18838 2023-07-29 10:03:17.033174 mypy-boto3-inspector-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17337 2023-07-29 09:47:15.000000 mypy-boto3-inspector-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:17.029174 mypy-boto3-inspector-1.28.15.post1/mypy_boto3_inspector/
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-07-29 09:47:15.000000 mypy-boto3-inspector-1.28.15.post1/mypy_boto3_inspector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-07-29 09:47:15.000000 mypy-boto3-inspector-1.28.15.post1/mypy_boto3_inspector/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-29 09:47:15.000000 mypy-boto3-inspector-1.28.15.post1/mypy_boto3_inspector/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31933 2023-07-29 09:47:15.000000 mypy-boto3-inspector-1.28.15.post1/mypy_boto3_inspector/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    31880 2023-07-29 09:47:15.000000 mypy-boto3-inspector-1.28.15.post1/mypy_boto3_inspector/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10983 2023-07-29 09:47:16.000000 mypy-boto3-inspector-1.28.15.post1/mypy_boto3_inspector/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10981 2023-07-29 09:47:15.000000 mypy-boto3-inspector-1.28.15.post1/mypy_boto3_inspector/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11258 2023-07-29 09:47:15.000000 mypy-boto3-inspector-1.28.15.post1/mypy_boto3_inspector/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11247 2023-07-29 09:47:15.000000 mypy-boto3-inspector-1.28.15.post1/mypy_boto3_inspector/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:47:15.000000 mypy-boto3-inspector-1.28.15.post1/mypy_boto3_inspector/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    40434 2023-07-29 09:47:17.000000 mypy-boto3-inspector-1.28.15.post1/mypy_boto3_inspector/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    40369 2023-07-29 09:47:16.000000 mypy-boto3-inspector-1.28.15.post1/mypy_boto3_inspector/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:47:15.000000 mypy-boto3-inspector-1.28.15.post1/mypy_boto3_inspector/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:17.033174 mypy-boto3-inspector-1.28.15.post1/mypy_boto3_inspector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18838 2023-07-29 10:03:16.000000 mypy-boto3-inspector-1.28.15.post1/mypy_boto3_inspector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-29 10:03:16.000000 mypy-boto3-inspector-1.28.15.post1/mypy_boto3_inspector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:16.000000 mypy-boto3-inspector-1.28.15.post1/mypy_boto3_inspector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:16.000000 mypy-boto3-inspector-1.28.15.post1/mypy_boto3_inspector.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:16.000000 mypy-boto3-inspector-1.28.15.post1/mypy_boto3_inspector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-29 10:03:16.000000 mypy-boto3-inspector-1.28.15.post1/mypy_boto3_inspector.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:17.033174 mypy-boto3-inspector-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-07-29 09:47:15.000000 mypy-boto3-inspector-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:56.952872 mypy-boto3-inspector-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:19:55.000000 mypy-boto3-inspector-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18850 2023-08-01 11:36:56.952872 mypy-boto3-inspector-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17358 2023-08-01 11:19:55.000000 mypy-boto3-inspector-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:56.948872 mypy-boto3-inspector-1.28.16/mypy_boto3_inspector/
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-08-01 11:19:55.000000 mypy-boto3-inspector-1.28.16/mypy_boto3_inspector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-08-01 11:19:55.000000 mypy-boto3-inspector-1.28.16/mypy_boto3_inspector/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-08-01 11:19:55.000000 mypy-boto3-inspector-1.28.16/mypy_boto3_inspector/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31933 2023-08-01 11:19:55.000000 mypy-boto3-inspector-1.28.16/mypy_boto3_inspector/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31880 2023-08-01 11:19:55.000000 mypy-boto3-inspector-1.28.16/mypy_boto3_inspector/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10983 2023-08-01 11:19:56.000000 mypy-boto3-inspector-1.28.16/mypy_boto3_inspector/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10981 2023-08-01 11:19:55.000000 mypy-boto3-inspector-1.28.16/mypy_boto3_inspector/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11258 2023-08-01 11:19:55.000000 mypy-boto3-inspector-1.28.16/mypy_boto3_inspector/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11247 2023-08-01 11:19:55.000000 mypy-boto3-inspector-1.28.16/mypy_boto3_inspector/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:19:55.000000 mypy-boto3-inspector-1.28.16/mypy_boto3_inspector/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    40488 2023-08-01 11:19:57.000000 mypy-boto3-inspector-1.28.16/mypy_boto3_inspector/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40423 2023-08-01 11:19:56.000000 mypy-boto3-inspector-1.28.16/mypy_boto3_inspector/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:19:55.000000 mypy-boto3-inspector-1.28.16/mypy_boto3_inspector/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:56.952872 mypy-boto3-inspector-1.28.16/mypy_boto3_inspector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18850 2023-08-01 11:36:56.000000 mypy-boto3-inspector-1.28.16/mypy_boto3_inspector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-08-01 11:36:56.000000 mypy-boto3-inspector-1.28.16/mypy_boto3_inspector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:56.000000 mypy-boto3-inspector-1.28.16/mypy_boto3_inspector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:56.000000 mypy-boto3-inspector-1.28.16/mypy_boto3_inspector.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:56.000000 mypy-boto3-inspector-1.28.16/mypy_boto3_inspector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-01 11:36:56.000000 mypy-boto3-inspector-1.28.16/mypy_boto3_inspector.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:56.952872 mypy-boto3-inspector-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-08-01 11:19:55.000000 mypy-boto3-inspector-1.28.16/setup.py
```

### Comparing `mypy-boto3-inspector-1.28.15.post1/LICENSE` & `mypy-boto3-inspector-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-inspector-1.28.15.post1/PKG-INFO` & `mypy-boto3-inspector-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-inspector
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.Inspector 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.Inspector 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 inspector type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 inspector type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-inspector.svg?color=blue)](https://pypi.org/project/mypy-boto3-inspector)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-inspector)](https://pepy.tech/project/mypy-boto3-inspector)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Inspector 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector)
+[boto3.Inspector 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector)
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
 [mypy-boto3-inspector docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/).
 
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
@@ -362,31 +362,30 @@
 )
 
 
 def check_value(value: AgentHealthCodeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_inspector.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_inspector.type_defs import (
     AttributeTypeDef,
     FailedItemDetailsTypeDef,
     ResponseMetadataTypeDef,
     AgentFilterTypeDef,
     AgentPreviewTypeDef,
     TelemetryMetadataTypeDef,
     DurationRangeTypeDef,
-    TimestampRangeTypeDef,
     AssessmentRunNotificationTypeDef,
     AssessmentRunStateChangeTypeDef,
     AssessmentTargetFilterTypeDef,
     AssessmentTargetTypeDef,
     TagTypeDef,
     CreateAssessmentTargetRequestRequestTypeDef,
     CreateExclusionsPreviewRequestRequestTypeDef,
@@ -417,14 +416,15 @@
     SecurityGroupTypeDef,
     PreviewAgentsRequestRequestTypeDef,
     RegisterCrossAccountAccessRoleRequestRequestTypeDef,
     RemoveAttributesFromFindingsRequestRequestTypeDef,
     StartAssessmentRunRequestRequestTypeDef,
     StopAssessmentRunRequestRequestTypeDef,
     SubscribeToEventRequestRequestTypeDef,
+    TimestampTypeDef,
     UnsubscribeFromEventRequestRequestTypeDef,
     UpdateAssessmentTargetRequestRequestTypeDef,
     AddAttributesToFindingsRequestRequestTypeDef,
     AssessmentTemplateTypeDef,
     CreateAssessmentTemplateRequestRequestTypeDef,
     AddAttributesToFindingsResponseTypeDef,
     CreateAssessmentTargetResponseTypeDef,
@@ -443,16 +443,14 @@
     RemoveAttributesFromFindingsResponseTypeDef,
     StartAssessmentRunResponseTypeDef,
     ListAssessmentRunAgentsRequestRequestTypeDef,
     PreviewAgentsResponseTypeDef,
     AssessmentRunAgentTypeDef,
     GetTelemetryMetadataResponseTypeDef,
     AssessmentTemplateFilterTypeDef,
-    AssessmentRunFilterTypeDef,
-    FindingFilterTypeDef,
     AssessmentRunTypeDef,
     ListAssessmentTargetsRequestRequestTypeDef,
     DescribeAssessmentTargetsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     SetTagsForResourceRequestRequestTypeDef,
     CreateResourceGroupRequestRequestTypeDef,
     ResourceGroupTypeDef,
@@ -463,34 +461,37 @@
     ListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef,
     ListAssessmentTargetsRequestListAssessmentTargetsPaginateTypeDef,
     ListEventSubscriptionsRequestListEventSubscriptionsPaginateTypeDef,
     ListExclusionsRequestListExclusionsPaginateTypeDef,
     ListRulesPackagesRequestListRulesPackagesPaginateTypeDef,
     PreviewAgentsRequestPreviewAgentsPaginateTypeDef,
     NetworkInterfaceTypeDef,
+    TimestampRangeTypeDef,
     DescribeAssessmentTemplatesResponseTypeDef,
     ListAssessmentRunAgentsResponseTypeDef,
     ListAssessmentTemplatesRequestListAssessmentTemplatesPaginateTypeDef,
     ListAssessmentTemplatesRequestRequestTypeDef,
-    ListAssessmentRunsRequestListAssessmentRunsPaginateTypeDef,
-    ListAssessmentRunsRequestRequestTypeDef,
-    ListFindingsRequestListFindingsPaginateTypeDef,
-    ListFindingsRequestRequestTypeDef,
     DescribeAssessmentRunsResponseTypeDef,
     DescribeResourceGroupsResponseTypeDef,
     ListEventSubscriptionsResponseTypeDef,
     GetExclusionsPreviewResponseTypeDef,
     DescribeExclusionsResponseTypeDef,
     AssetAttributesTypeDef,
+    AssessmentRunFilterTypeDef,
+    FindingFilterTypeDef,
     FindingTypeDef,
+    ListAssessmentRunsRequestListAssessmentRunsPaginateTypeDef,
+    ListAssessmentRunsRequestRequestTypeDef,
+    ListFindingsRequestListFindingsPaginateTypeDef,
+    ListFindingsRequestRequestTypeDef,
     DescribeFindingsResponseTypeDef,
 )
 
 
-def get_structure() -> AttributeTypeDef:
+def get_value() -> AttributeTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-inspector-1.28.15.post1/README.md` & `mypy-boto3-inspector-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-inspector.svg?color=blue)](https://pypi.org/project/mypy-boto3-inspector)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-inspector)](https://pepy.tech/project/mypy-boto3-inspector)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Inspector 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector)
+[boto3.Inspector 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector)
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
 [mypy-boto3-inspector docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/).
 
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
@@ -330,31 +330,30 @@
 )
 
 
 def check_value(value: AgentHealthCodeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_inspector.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_inspector.type_defs import (
     AttributeTypeDef,
     FailedItemDetailsTypeDef,
     ResponseMetadataTypeDef,
     AgentFilterTypeDef,
     AgentPreviewTypeDef,
     TelemetryMetadataTypeDef,
     DurationRangeTypeDef,
-    TimestampRangeTypeDef,
     AssessmentRunNotificationTypeDef,
     AssessmentRunStateChangeTypeDef,
     AssessmentTargetFilterTypeDef,
     AssessmentTargetTypeDef,
     TagTypeDef,
     CreateAssessmentTargetRequestRequestTypeDef,
     CreateExclusionsPreviewRequestRequestTypeDef,
@@ -385,14 +384,15 @@
     SecurityGroupTypeDef,
     PreviewAgentsRequestRequestTypeDef,
     RegisterCrossAccountAccessRoleRequestRequestTypeDef,
     RemoveAttributesFromFindingsRequestRequestTypeDef,
     StartAssessmentRunRequestRequestTypeDef,
     StopAssessmentRunRequestRequestTypeDef,
     SubscribeToEventRequestRequestTypeDef,
+    TimestampTypeDef,
     UnsubscribeFromEventRequestRequestTypeDef,
     UpdateAssessmentTargetRequestRequestTypeDef,
     AddAttributesToFindingsRequestRequestTypeDef,
     AssessmentTemplateTypeDef,
     CreateAssessmentTemplateRequestRequestTypeDef,
     AddAttributesToFindingsResponseTypeDef,
     CreateAssessmentTargetResponseTypeDef,
@@ -411,16 +411,14 @@
     RemoveAttributesFromFindingsResponseTypeDef,
     StartAssessmentRunResponseTypeDef,
     ListAssessmentRunAgentsRequestRequestTypeDef,
     PreviewAgentsResponseTypeDef,
     AssessmentRunAgentTypeDef,
     GetTelemetryMetadataResponseTypeDef,
     AssessmentTemplateFilterTypeDef,
-    AssessmentRunFilterTypeDef,
-    FindingFilterTypeDef,
     AssessmentRunTypeDef,
     ListAssessmentTargetsRequestRequestTypeDef,
     DescribeAssessmentTargetsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     SetTagsForResourceRequestRequestTypeDef,
     CreateResourceGroupRequestRequestTypeDef,
     ResourceGroupTypeDef,
@@ -431,34 +429,37 @@
     ListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef,
     ListAssessmentTargetsRequestListAssessmentTargetsPaginateTypeDef,
     ListEventSubscriptionsRequestListEventSubscriptionsPaginateTypeDef,
     ListExclusionsRequestListExclusionsPaginateTypeDef,
     ListRulesPackagesRequestListRulesPackagesPaginateTypeDef,
     PreviewAgentsRequestPreviewAgentsPaginateTypeDef,
     NetworkInterfaceTypeDef,
+    TimestampRangeTypeDef,
     DescribeAssessmentTemplatesResponseTypeDef,
     ListAssessmentRunAgentsResponseTypeDef,
     ListAssessmentTemplatesRequestListAssessmentTemplatesPaginateTypeDef,
     ListAssessmentTemplatesRequestRequestTypeDef,
-    ListAssessmentRunsRequestListAssessmentRunsPaginateTypeDef,
-    ListAssessmentRunsRequestRequestTypeDef,
-    ListFindingsRequestListFindingsPaginateTypeDef,
-    ListFindingsRequestRequestTypeDef,
     DescribeAssessmentRunsResponseTypeDef,
     DescribeResourceGroupsResponseTypeDef,
     ListEventSubscriptionsResponseTypeDef,
     GetExclusionsPreviewResponseTypeDef,
     DescribeExclusionsResponseTypeDef,
     AssetAttributesTypeDef,
+    AssessmentRunFilterTypeDef,
+    FindingFilterTypeDef,
     FindingTypeDef,
+    ListAssessmentRunsRequestListAssessmentRunsPaginateTypeDef,
+    ListAssessmentRunsRequestRequestTypeDef,
+    ListFindingsRequestListFindingsPaginateTypeDef,
+    ListFindingsRequestRequestTypeDef,
     DescribeFindingsResponseTypeDef,
 )
 
 
-def get_structure() -> AttributeTypeDef:
+def get_value() -> AttributeTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-inspector-1.28.15.post1/mypy_boto3_inspector/__init__.py` & `mypy-boto3-inspector-1.28.16/mypy_boto3_inspector/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-inspector-1.28.15.post1/mypy_boto3_inspector/__init__.pyi` & `mypy-boto3-inspector-1.28.16/mypy_boto3_inspector/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-inspector-1.28.15.post1/mypy_boto3_inspector/__main__.py` & `mypy-boto3-inspector-1.28.16/mypy_boto3_inspector/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Inspector 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.Inspector 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector\nOther"
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

### Comparing `mypy-boto3-inspector-1.28.15.post1/mypy_boto3_inspector/client.py` & `mypy-boto3-inspector-1.28.16/mypy_boto3_inspector/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-inspector-1.28.15.post1/mypy_boto3_inspector/client.pyi` & `mypy-boto3-inspector-1.28.16/mypy_boto3_inspector/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-inspector-1.28.15.post1/mypy_boto3_inspector/literals.py` & `mypy-boto3-inspector-1.28.16/mypy_boto3_inspector/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-inspector-1.28.15.post1/mypy_boto3_inspector/literals.pyi` & `mypy-boto3-inspector-1.28.16/mypy_boto3_inspector/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-inspector-1.28.15.post1/mypy_boto3_inspector/paginator.py` & `mypy-boto3-inspector-1.28.16/mypy_boto3_inspector/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-inspector-1.28.15.post1/mypy_boto3_inspector/paginator.pyi` & `mypy-boto3-inspector-1.28.16/mypy_boto3_inspector/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-inspector-1.28.15.post1/mypy_boto3_inspector/type_defs.py` & `mypy-boto3-inspector-1.28.16/mypy_boto3_inspector/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_inspector.type_defs import AttributeTypeDef
 
-    data: AttributeTypeDef = {...}
+    data: AttributeTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -45,15 +45,14 @@
     "AttributeTypeDef",
     "FailedItemDetailsTypeDef",
     "ResponseMetadataTypeDef",
     "AgentFilterTypeDef",
     "AgentPreviewTypeDef",
     "TelemetryMetadataTypeDef",
     "DurationRangeTypeDef",
-    "TimestampRangeTypeDef",
     "AssessmentRunNotificationTypeDef",
     "AssessmentRunStateChangeTypeDef",
     "AssessmentTargetFilterTypeDef",
     "AssessmentTargetTypeDef",
     "TagTypeDef",
     "CreateAssessmentTargetRequestRequestTypeDef",
     "CreateExclusionsPreviewRequestRequestTypeDef",
@@ -84,14 +83,15 @@
     "SecurityGroupTypeDef",
     "PreviewAgentsRequestRequestTypeDef",
     "RegisterCrossAccountAccessRoleRequestRequestTypeDef",
     "RemoveAttributesFromFindingsRequestRequestTypeDef",
     "StartAssessmentRunRequestRequestTypeDef",
     "StopAssessmentRunRequestRequestTypeDef",
     "SubscribeToEventRequestRequestTypeDef",
+    "TimestampTypeDef",
     "UnsubscribeFromEventRequestRequestTypeDef",
     "UpdateAssessmentTargetRequestRequestTypeDef",
     "AddAttributesToFindingsRequestRequestTypeDef",
     "AssessmentTemplateTypeDef",
     "CreateAssessmentTemplateRequestRequestTypeDef",
     "AddAttributesToFindingsResponseTypeDef",
     "CreateAssessmentTargetResponseTypeDef",
@@ -110,16 +110,14 @@
     "RemoveAttributesFromFindingsResponseTypeDef",
     "StartAssessmentRunResponseTypeDef",
     "ListAssessmentRunAgentsRequestRequestTypeDef",
     "PreviewAgentsResponseTypeDef",
     "AssessmentRunAgentTypeDef",
     "GetTelemetryMetadataResponseTypeDef",
     "AssessmentTemplateFilterTypeDef",
-    "AssessmentRunFilterTypeDef",
-    "FindingFilterTypeDef",
     "AssessmentRunTypeDef",
     "ListAssessmentTargetsRequestRequestTypeDef",
     "DescribeAssessmentTargetsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "SetTagsForResourceRequestRequestTypeDef",
     "CreateResourceGroupRequestRequestTypeDef",
     "ResourceGroupTypeDef",
@@ -130,29 +128,32 @@
     "ListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef",
     "ListAssessmentTargetsRequestListAssessmentTargetsPaginateTypeDef",
     "ListEventSubscriptionsRequestListEventSubscriptionsPaginateTypeDef",
     "ListExclusionsRequestListExclusionsPaginateTypeDef",
     "ListRulesPackagesRequestListRulesPackagesPaginateTypeDef",
     "PreviewAgentsRequestPreviewAgentsPaginateTypeDef",
     "NetworkInterfaceTypeDef",
+    "TimestampRangeTypeDef",
     "DescribeAssessmentTemplatesResponseTypeDef",
     "ListAssessmentRunAgentsResponseTypeDef",
     "ListAssessmentTemplatesRequestListAssessmentTemplatesPaginateTypeDef",
     "ListAssessmentTemplatesRequestRequestTypeDef",
-    "ListAssessmentRunsRequestListAssessmentRunsPaginateTypeDef",
-    "ListAssessmentRunsRequestRequestTypeDef",
-    "ListFindingsRequestListFindingsPaginateTypeDef",
-    "ListFindingsRequestRequestTypeDef",
     "DescribeAssessmentRunsResponseTypeDef",
     "DescribeResourceGroupsResponseTypeDef",
     "ListEventSubscriptionsResponseTypeDef",
     "GetExclusionsPreviewResponseTypeDef",
     "DescribeExclusionsResponseTypeDef",
     "AssetAttributesTypeDef",
+    "AssessmentRunFilterTypeDef",
+    "FindingFilterTypeDef",
     "FindingTypeDef",
+    "ListAssessmentRunsRequestListAssessmentRunsPaginateTypeDef",
+    "ListAssessmentRunsRequestRequestTypeDef",
+    "ListFindingsRequestListFindingsPaginateTypeDef",
+    "ListFindingsRequestRequestTypeDef",
     "DescribeFindingsResponseTypeDef",
 )
 
 _RequiredAttributeTypeDef = TypedDict(
     "_RequiredAttributeTypeDef",
     {
         "key": str,
@@ -250,23 +251,14 @@
     {
         "minSeconds": int,
         "maxSeconds": int,
     },
     total=False,
 )
 
-TimestampRangeTypeDef = TypedDict(
-    "TimestampRangeTypeDef",
-    {
-        "beginDate": Union[datetime, str],
-        "endDate": Union[datetime, str],
-    },
-    total=False,
-)
-
 _RequiredAssessmentRunNotificationTypeDef = TypedDict(
     "_RequiredAssessmentRunNotificationTypeDef",
     {
         "date": datetime,
         "event": InspectorEventType,
         "error": bool,
     },
@@ -770,14 +762,15 @@
     {
         "resourceArn": str,
         "event": InspectorEventType,
         "topicArn": str,
     },
 )
 
+TimestampTypeDef = Union[datetime, str]
 UnsubscribeFromEventRequestRequestTypeDef = TypedDict(
     "UnsubscribeFromEventRequestRequestTypeDef",
     {
         "resourceArn": str,
         "event": InspectorEventType,
         "topicArn": str,
     },
@@ -1076,43 +1069,14 @@
         "namePattern": str,
         "durationRange": DurationRangeTypeDef,
         "rulesPackageArns": Sequence[str],
     },
     total=False,
 )
 
-AssessmentRunFilterTypeDef = TypedDict(
-    "AssessmentRunFilterTypeDef",
-    {
-        "namePattern": str,
-        "states": Sequence[AssessmentRunStateType],
-        "durationRange": DurationRangeTypeDef,
-        "rulesPackageArns": Sequence[str],
-        "startTimeRange": TimestampRangeTypeDef,
-        "completionTimeRange": TimestampRangeTypeDef,
-        "stateChangeTimeRange": TimestampRangeTypeDef,
-    },
-    total=False,
-)
-
-FindingFilterTypeDef = TypedDict(
-    "FindingFilterTypeDef",
-    {
-        "agentIds": Sequence[str],
-        "autoScalingGroups": Sequence[str],
-        "ruleNames": Sequence[str],
-        "severities": Sequence[SeverityType],
-        "rulesPackageArns": Sequence[str],
-        "attributes": Sequence[AttributeTypeDef],
-        "userAttributes": Sequence[AttributeTypeDef],
-        "creationTimeRange": TimestampRangeTypeDef,
-    },
-    total=False,
-)
-
 _RequiredAssessmentRunTypeDef = TypedDict(
     "_RequiredAssessmentRunTypeDef",
     {
         "arn": str,
         "name": str,
         "assessmentTemplateArn": str,
         "state": AssessmentRunStateType,
@@ -1375,14 +1339,23 @@
         "publicIp": str,
         "ipv6Addresses": List[str],
         "securityGroups": List[SecurityGroupTypeDef],
     },
     total=False,
 )
 
+TimestampRangeTypeDef = TypedDict(
+    "TimestampRangeTypeDef",
+    {
+        "beginDate": TimestampTypeDef,
+        "endDate": TimestampTypeDef,
+    },
+    total=False,
+)
+
 DescribeAssessmentTemplatesResponseTypeDef = TypedDict(
     "DescribeAssessmentTemplatesResponseTypeDef",
     {
         "assessmentTemplates": List[AssessmentTemplateTypeDef],
         "failedItems": Dict[str, FailedItemDetailsTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1414,56 +1387,14 @@
         "filter": AssessmentTemplateFilterTypeDef,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-ListAssessmentRunsRequestListAssessmentRunsPaginateTypeDef = TypedDict(
-    "ListAssessmentRunsRequestListAssessmentRunsPaginateTypeDef",
-    {
-        "assessmentTemplateArns": Sequence[str],
-        "filter": AssessmentRunFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListAssessmentRunsRequestRequestTypeDef = TypedDict(
-    "ListAssessmentRunsRequestRequestTypeDef",
-    {
-        "assessmentTemplateArns": Sequence[str],
-        "filter": AssessmentRunFilterTypeDef,
-        "nextToken": str,
-        "maxResults": int,
-    },
-    total=False,
-)
-
-ListFindingsRequestListFindingsPaginateTypeDef = TypedDict(
-    "ListFindingsRequestListFindingsPaginateTypeDef",
-    {
-        "assessmentRunArns": Sequence[str],
-        "filter": FindingFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListFindingsRequestRequestTypeDef = TypedDict(
-    "ListFindingsRequestRequestTypeDef",
-    {
-        "assessmentRunArns": Sequence[str],
-        "filter": FindingFilterTypeDef,
-        "nextToken": str,
-        "maxResults": int,
-    },
-    total=False,
-)
-
 DescribeAssessmentRunsResponseTypeDef = TypedDict(
     "DescribeAssessmentRunsResponseTypeDef",
     {
         "assessmentRuns": List[AssessmentRunTypeDef],
         "failedItems": Dict[str, FailedItemDetailsTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1527,14 +1458,43 @@
 )
 
 
 class AssetAttributesTypeDef(_RequiredAssetAttributesTypeDef, _OptionalAssetAttributesTypeDef):
     pass
 
 
+AssessmentRunFilterTypeDef = TypedDict(
+    "AssessmentRunFilterTypeDef",
+    {
+        "namePattern": str,
+        "states": Sequence[AssessmentRunStateType],
+        "durationRange": DurationRangeTypeDef,
+        "rulesPackageArns": Sequence[str],
+        "startTimeRange": TimestampRangeTypeDef,
+        "completionTimeRange": TimestampRangeTypeDef,
+        "stateChangeTimeRange": TimestampRangeTypeDef,
+    },
+    total=False,
+)
+
+FindingFilterTypeDef = TypedDict(
+    "FindingFilterTypeDef",
+    {
+        "agentIds": Sequence[str],
+        "autoScalingGroups": Sequence[str],
+        "ruleNames": Sequence[str],
+        "severities": Sequence[SeverityType],
+        "rulesPackageArns": Sequence[str],
+        "attributes": Sequence[AttributeTypeDef],
+        "userAttributes": Sequence[AttributeTypeDef],
+        "creationTimeRange": TimestampRangeTypeDef,
+    },
+    total=False,
+)
+
 _RequiredFindingTypeDef = TypedDict(
     "_RequiredFindingTypeDef",
     {
         "arn": str,
         "attributes": List[AttributeTypeDef],
         "userAttributes": List[AttributeTypeDef],
         "createdAt": datetime,
@@ -1562,14 +1522,56 @@
 )
 
 
 class FindingTypeDef(_RequiredFindingTypeDef, _OptionalFindingTypeDef):
     pass
 
 
+ListAssessmentRunsRequestListAssessmentRunsPaginateTypeDef = TypedDict(
+    "ListAssessmentRunsRequestListAssessmentRunsPaginateTypeDef",
+    {
+        "assessmentTemplateArns": Sequence[str],
+        "filter": AssessmentRunFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListAssessmentRunsRequestRequestTypeDef = TypedDict(
+    "ListAssessmentRunsRequestRequestTypeDef",
+    {
+        "assessmentTemplateArns": Sequence[str],
+        "filter": AssessmentRunFilterTypeDef,
+        "nextToken": str,
+        "maxResults": int,
+    },
+    total=False,
+)
+
+ListFindingsRequestListFindingsPaginateTypeDef = TypedDict(
+    "ListFindingsRequestListFindingsPaginateTypeDef",
+    {
+        "assessmentRunArns": Sequence[str],
+        "filter": FindingFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListFindingsRequestRequestTypeDef = TypedDict(
+    "ListFindingsRequestRequestTypeDef",
+    {
+        "assessmentRunArns": Sequence[str],
+        "filter": FindingFilterTypeDef,
+        "nextToken": str,
+        "maxResults": int,
+    },
+    total=False,
+)
+
 DescribeFindingsResponseTypeDef = TypedDict(
     "DescribeFindingsResponseTypeDef",
     {
         "findings": List[FindingTypeDef],
         "failedItems": Dict[str, FailedItemDetailsTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-inspector-1.28.15.post1/mypy_boto3_inspector/type_defs.pyi` & `mypy-boto3-inspector-1.28.16/mypy_boto3_inspector/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_inspector.type_defs import AttributeTypeDef
 
-    data: AttributeTypeDef = {...}
+    data: AttributeTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -44,15 +44,14 @@
     "AttributeTypeDef",
     "FailedItemDetailsTypeDef",
     "ResponseMetadataTypeDef",
     "AgentFilterTypeDef",
     "AgentPreviewTypeDef",
     "TelemetryMetadataTypeDef",
     "DurationRangeTypeDef",
-    "TimestampRangeTypeDef",
     "AssessmentRunNotificationTypeDef",
     "AssessmentRunStateChangeTypeDef",
     "AssessmentTargetFilterTypeDef",
     "AssessmentTargetTypeDef",
     "TagTypeDef",
     "CreateAssessmentTargetRequestRequestTypeDef",
     "CreateExclusionsPreviewRequestRequestTypeDef",
@@ -83,14 +82,15 @@
     "SecurityGroupTypeDef",
     "PreviewAgentsRequestRequestTypeDef",
     "RegisterCrossAccountAccessRoleRequestRequestTypeDef",
     "RemoveAttributesFromFindingsRequestRequestTypeDef",
     "StartAssessmentRunRequestRequestTypeDef",
     "StopAssessmentRunRequestRequestTypeDef",
     "SubscribeToEventRequestRequestTypeDef",
+    "TimestampTypeDef",
     "UnsubscribeFromEventRequestRequestTypeDef",
     "UpdateAssessmentTargetRequestRequestTypeDef",
     "AddAttributesToFindingsRequestRequestTypeDef",
     "AssessmentTemplateTypeDef",
     "CreateAssessmentTemplateRequestRequestTypeDef",
     "AddAttributesToFindingsResponseTypeDef",
     "CreateAssessmentTargetResponseTypeDef",
@@ -109,16 +109,14 @@
     "RemoveAttributesFromFindingsResponseTypeDef",
     "StartAssessmentRunResponseTypeDef",
     "ListAssessmentRunAgentsRequestRequestTypeDef",
     "PreviewAgentsResponseTypeDef",
     "AssessmentRunAgentTypeDef",
     "GetTelemetryMetadataResponseTypeDef",
     "AssessmentTemplateFilterTypeDef",
-    "AssessmentRunFilterTypeDef",
-    "FindingFilterTypeDef",
     "AssessmentRunTypeDef",
     "ListAssessmentTargetsRequestRequestTypeDef",
     "DescribeAssessmentTargetsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "SetTagsForResourceRequestRequestTypeDef",
     "CreateResourceGroupRequestRequestTypeDef",
     "ResourceGroupTypeDef",
@@ -129,29 +127,32 @@
     "ListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef",
     "ListAssessmentTargetsRequestListAssessmentTargetsPaginateTypeDef",
     "ListEventSubscriptionsRequestListEventSubscriptionsPaginateTypeDef",
     "ListExclusionsRequestListExclusionsPaginateTypeDef",
     "ListRulesPackagesRequestListRulesPackagesPaginateTypeDef",
     "PreviewAgentsRequestPreviewAgentsPaginateTypeDef",
     "NetworkInterfaceTypeDef",
+    "TimestampRangeTypeDef",
     "DescribeAssessmentTemplatesResponseTypeDef",
     "ListAssessmentRunAgentsResponseTypeDef",
     "ListAssessmentTemplatesRequestListAssessmentTemplatesPaginateTypeDef",
     "ListAssessmentTemplatesRequestRequestTypeDef",
-    "ListAssessmentRunsRequestListAssessmentRunsPaginateTypeDef",
-    "ListAssessmentRunsRequestRequestTypeDef",
-    "ListFindingsRequestListFindingsPaginateTypeDef",
-    "ListFindingsRequestRequestTypeDef",
     "DescribeAssessmentRunsResponseTypeDef",
     "DescribeResourceGroupsResponseTypeDef",
     "ListEventSubscriptionsResponseTypeDef",
     "GetExclusionsPreviewResponseTypeDef",
     "DescribeExclusionsResponseTypeDef",
     "AssetAttributesTypeDef",
+    "AssessmentRunFilterTypeDef",
+    "FindingFilterTypeDef",
     "FindingTypeDef",
+    "ListAssessmentRunsRequestListAssessmentRunsPaginateTypeDef",
+    "ListAssessmentRunsRequestRequestTypeDef",
+    "ListFindingsRequestListFindingsPaginateTypeDef",
+    "ListFindingsRequestRequestTypeDef",
     "DescribeFindingsResponseTypeDef",
 )
 
 _RequiredAttributeTypeDef = TypedDict(
     "_RequiredAttributeTypeDef",
     {
         "key": str,
@@ -243,23 +244,14 @@
     {
         "minSeconds": int,
         "maxSeconds": int,
     },
     total=False,
 )
 
-TimestampRangeTypeDef = TypedDict(
-    "TimestampRangeTypeDef",
-    {
-        "beginDate": Union[datetime, str],
-        "endDate": Union[datetime, str],
-    },
-    total=False,
-)
-
 _RequiredAssessmentRunNotificationTypeDef = TypedDict(
     "_RequiredAssessmentRunNotificationTypeDef",
     {
         "date": datetime,
         "event": InspectorEventType,
         "error": bool,
     },
@@ -733,14 +725,15 @@
     {
         "resourceArn": str,
         "event": InspectorEventType,
         "topicArn": str,
     },
 )
 
+TimestampTypeDef = Union[datetime, str]
 UnsubscribeFromEventRequestRequestTypeDef = TypedDict(
     "UnsubscribeFromEventRequestRequestTypeDef",
     {
         "resourceArn": str,
         "event": InspectorEventType,
         "topicArn": str,
     },
@@ -1029,43 +1022,14 @@
         "namePattern": str,
         "durationRange": DurationRangeTypeDef,
         "rulesPackageArns": Sequence[str],
     },
     total=False,
 )
 
-AssessmentRunFilterTypeDef = TypedDict(
-    "AssessmentRunFilterTypeDef",
-    {
-        "namePattern": str,
-        "states": Sequence[AssessmentRunStateType],
-        "durationRange": DurationRangeTypeDef,
-        "rulesPackageArns": Sequence[str],
-        "startTimeRange": TimestampRangeTypeDef,
-        "completionTimeRange": TimestampRangeTypeDef,
-        "stateChangeTimeRange": TimestampRangeTypeDef,
-    },
-    total=False,
-)
-
-FindingFilterTypeDef = TypedDict(
-    "FindingFilterTypeDef",
-    {
-        "agentIds": Sequence[str],
-        "autoScalingGroups": Sequence[str],
-        "ruleNames": Sequence[str],
-        "severities": Sequence[SeverityType],
-        "rulesPackageArns": Sequence[str],
-        "attributes": Sequence[AttributeTypeDef],
-        "userAttributes": Sequence[AttributeTypeDef],
-        "creationTimeRange": TimestampRangeTypeDef,
-    },
-    total=False,
-)
-
 _RequiredAssessmentRunTypeDef = TypedDict(
     "_RequiredAssessmentRunTypeDef",
     {
         "arn": str,
         "name": str,
         "assessmentTemplateArn": str,
         "state": AssessmentRunStateType,
@@ -1314,14 +1278,23 @@
         "publicIp": str,
         "ipv6Addresses": List[str],
         "securityGroups": List[SecurityGroupTypeDef],
     },
     total=False,
 )
 
+TimestampRangeTypeDef = TypedDict(
+    "TimestampRangeTypeDef",
+    {
+        "beginDate": TimestampTypeDef,
+        "endDate": TimestampTypeDef,
+    },
+    total=False,
+)
+
 DescribeAssessmentTemplatesResponseTypeDef = TypedDict(
     "DescribeAssessmentTemplatesResponseTypeDef",
     {
         "assessmentTemplates": List[AssessmentTemplateTypeDef],
         "failedItems": Dict[str, FailedItemDetailsTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1353,56 +1326,14 @@
         "filter": AssessmentTemplateFilterTypeDef,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-ListAssessmentRunsRequestListAssessmentRunsPaginateTypeDef = TypedDict(
-    "ListAssessmentRunsRequestListAssessmentRunsPaginateTypeDef",
-    {
-        "assessmentTemplateArns": Sequence[str],
-        "filter": AssessmentRunFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListAssessmentRunsRequestRequestTypeDef = TypedDict(
-    "ListAssessmentRunsRequestRequestTypeDef",
-    {
-        "assessmentTemplateArns": Sequence[str],
-        "filter": AssessmentRunFilterTypeDef,
-        "nextToken": str,
-        "maxResults": int,
-    },
-    total=False,
-)
-
-ListFindingsRequestListFindingsPaginateTypeDef = TypedDict(
-    "ListFindingsRequestListFindingsPaginateTypeDef",
-    {
-        "assessmentRunArns": Sequence[str],
-        "filter": FindingFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListFindingsRequestRequestTypeDef = TypedDict(
-    "ListFindingsRequestRequestTypeDef",
-    {
-        "assessmentRunArns": Sequence[str],
-        "filter": FindingFilterTypeDef,
-        "nextToken": str,
-        "maxResults": int,
-    },
-    total=False,
-)
-
 DescribeAssessmentRunsResponseTypeDef = TypedDict(
     "DescribeAssessmentRunsResponseTypeDef",
     {
         "assessmentRuns": List[AssessmentRunTypeDef],
         "failedItems": Dict[str, FailedItemDetailsTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1464,14 +1395,43 @@
     },
     total=False,
 )
 
 class AssetAttributesTypeDef(_RequiredAssetAttributesTypeDef, _OptionalAssetAttributesTypeDef):
     pass
 
+AssessmentRunFilterTypeDef = TypedDict(
+    "AssessmentRunFilterTypeDef",
+    {
+        "namePattern": str,
+        "states": Sequence[AssessmentRunStateType],
+        "durationRange": DurationRangeTypeDef,
+        "rulesPackageArns": Sequence[str],
+        "startTimeRange": TimestampRangeTypeDef,
+        "completionTimeRange": TimestampRangeTypeDef,
+        "stateChangeTimeRange": TimestampRangeTypeDef,
+    },
+    total=False,
+)
+
+FindingFilterTypeDef = TypedDict(
+    "FindingFilterTypeDef",
+    {
+        "agentIds": Sequence[str],
+        "autoScalingGroups": Sequence[str],
+        "ruleNames": Sequence[str],
+        "severities": Sequence[SeverityType],
+        "rulesPackageArns": Sequence[str],
+        "attributes": Sequence[AttributeTypeDef],
+        "userAttributes": Sequence[AttributeTypeDef],
+        "creationTimeRange": TimestampRangeTypeDef,
+    },
+    total=False,
+)
+
 _RequiredFindingTypeDef = TypedDict(
     "_RequiredFindingTypeDef",
     {
         "arn": str,
         "attributes": List[AttributeTypeDef],
         "userAttributes": List[AttributeTypeDef],
         "createdAt": datetime,
@@ -1497,14 +1457,56 @@
     },
     total=False,
 )
 
 class FindingTypeDef(_RequiredFindingTypeDef, _OptionalFindingTypeDef):
     pass
 
+ListAssessmentRunsRequestListAssessmentRunsPaginateTypeDef = TypedDict(
+    "ListAssessmentRunsRequestListAssessmentRunsPaginateTypeDef",
+    {
+        "assessmentTemplateArns": Sequence[str],
+        "filter": AssessmentRunFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListAssessmentRunsRequestRequestTypeDef = TypedDict(
+    "ListAssessmentRunsRequestRequestTypeDef",
+    {
+        "assessmentTemplateArns": Sequence[str],
+        "filter": AssessmentRunFilterTypeDef,
+        "nextToken": str,
+        "maxResults": int,
+    },
+    total=False,
+)
+
+ListFindingsRequestListFindingsPaginateTypeDef = TypedDict(
+    "ListFindingsRequestListFindingsPaginateTypeDef",
+    {
+        "assessmentRunArns": Sequence[str],
+        "filter": FindingFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListFindingsRequestRequestTypeDef = TypedDict(
+    "ListFindingsRequestRequestTypeDef",
+    {
+        "assessmentRunArns": Sequence[str],
+        "filter": FindingFilterTypeDef,
+        "nextToken": str,
+        "maxResults": int,
+    },
+    total=False,
+)
+
 DescribeFindingsResponseTypeDef = TypedDict(
     "DescribeFindingsResponseTypeDef",
     {
         "findings": List[FindingTypeDef],
         "failedItems": Dict[str, FailedItemDetailsTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-inspector-1.28.15.post1/mypy_boto3_inspector.egg-info/PKG-INFO` & `mypy-boto3-inspector-1.28.16/mypy_boto3_inspector.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-inspector
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.Inspector 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.Inspector 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 inspector type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 inspector type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-inspector.svg?color=blue)](https://pypi.org/project/mypy-boto3-inspector)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-inspector)](https://pepy.tech/project/mypy-boto3-inspector)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Inspector 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector)
+[boto3.Inspector 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector)
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
 [mypy-boto3-inspector docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/).
 
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
@@ -362,31 +362,30 @@
 )
 
 
 def check_value(value: AgentHealthCodeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_inspector.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_inspector.type_defs import (
     AttributeTypeDef,
     FailedItemDetailsTypeDef,
     ResponseMetadataTypeDef,
     AgentFilterTypeDef,
     AgentPreviewTypeDef,
     TelemetryMetadataTypeDef,
     DurationRangeTypeDef,
-    TimestampRangeTypeDef,
     AssessmentRunNotificationTypeDef,
     AssessmentRunStateChangeTypeDef,
     AssessmentTargetFilterTypeDef,
     AssessmentTargetTypeDef,
     TagTypeDef,
     CreateAssessmentTargetRequestRequestTypeDef,
     CreateExclusionsPreviewRequestRequestTypeDef,
@@ -417,14 +416,15 @@
     SecurityGroupTypeDef,
     PreviewAgentsRequestRequestTypeDef,
     RegisterCrossAccountAccessRoleRequestRequestTypeDef,
     RemoveAttributesFromFindingsRequestRequestTypeDef,
     StartAssessmentRunRequestRequestTypeDef,
     StopAssessmentRunRequestRequestTypeDef,
     SubscribeToEventRequestRequestTypeDef,
+    TimestampTypeDef,
     UnsubscribeFromEventRequestRequestTypeDef,
     UpdateAssessmentTargetRequestRequestTypeDef,
     AddAttributesToFindingsRequestRequestTypeDef,
     AssessmentTemplateTypeDef,
     CreateAssessmentTemplateRequestRequestTypeDef,
     AddAttributesToFindingsResponseTypeDef,
     CreateAssessmentTargetResponseTypeDef,
@@ -443,16 +443,14 @@
     RemoveAttributesFromFindingsResponseTypeDef,
     StartAssessmentRunResponseTypeDef,
     ListAssessmentRunAgentsRequestRequestTypeDef,
     PreviewAgentsResponseTypeDef,
     AssessmentRunAgentTypeDef,
     GetTelemetryMetadataResponseTypeDef,
     AssessmentTemplateFilterTypeDef,
-    AssessmentRunFilterTypeDef,
-    FindingFilterTypeDef,
     AssessmentRunTypeDef,
     ListAssessmentTargetsRequestRequestTypeDef,
     DescribeAssessmentTargetsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     SetTagsForResourceRequestRequestTypeDef,
     CreateResourceGroupRequestRequestTypeDef,
     ResourceGroupTypeDef,
@@ -463,34 +461,37 @@
     ListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef,
     ListAssessmentTargetsRequestListAssessmentTargetsPaginateTypeDef,
     ListEventSubscriptionsRequestListEventSubscriptionsPaginateTypeDef,
     ListExclusionsRequestListExclusionsPaginateTypeDef,
     ListRulesPackagesRequestListRulesPackagesPaginateTypeDef,
     PreviewAgentsRequestPreviewAgentsPaginateTypeDef,
     NetworkInterfaceTypeDef,
+    TimestampRangeTypeDef,
     DescribeAssessmentTemplatesResponseTypeDef,
     ListAssessmentRunAgentsResponseTypeDef,
     ListAssessmentTemplatesRequestListAssessmentTemplatesPaginateTypeDef,
     ListAssessmentTemplatesRequestRequestTypeDef,
-    ListAssessmentRunsRequestListAssessmentRunsPaginateTypeDef,
-    ListAssessmentRunsRequestRequestTypeDef,
-    ListFindingsRequestListFindingsPaginateTypeDef,
-    ListFindingsRequestRequestTypeDef,
     DescribeAssessmentRunsResponseTypeDef,
     DescribeResourceGroupsResponseTypeDef,
     ListEventSubscriptionsResponseTypeDef,
     GetExclusionsPreviewResponseTypeDef,
     DescribeExclusionsResponseTypeDef,
     AssetAttributesTypeDef,
+    AssessmentRunFilterTypeDef,
+    FindingFilterTypeDef,
     FindingTypeDef,
+    ListAssessmentRunsRequestListAssessmentRunsPaginateTypeDef,
+    ListAssessmentRunsRequestRequestTypeDef,
+    ListFindingsRequestListFindingsPaginateTypeDef,
+    ListFindingsRequestRequestTypeDef,
     DescribeFindingsResponseTypeDef,
 )
 
 
-def get_structure() -> AttributeTypeDef:
+def get_value() -> AttributeTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-inspector-1.28.15.post1/mypy_boto3_inspector.egg-info/SOURCES.txt` & `mypy-boto3-inspector-1.28.16/mypy_boto3_inspector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-inspector-1.28.15.post1/setup.py` & `mypy-boto3-inspector-1.28.16/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-inspector",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_inspector"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Inspector 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.2"
+        "Type annotations for boto3.Inspector 1.28.16 service generated with mypy-boto3-builder"
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
-    keywords="boto3 inspector type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 inspector type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_inspector": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

