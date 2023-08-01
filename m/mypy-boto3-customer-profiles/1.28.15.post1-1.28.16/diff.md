# Comparing `tmp/mypy-boto3-customer-profiles-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-customer-profiles-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-customer-profiles-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:54 2023, max compression
+gzip compressed data, was "mypy-boto3-customer-profiles-1.28.16.tar", last modified: Tue Aug  1 11:36:35 2023, max compression
```

## Comparing `mypy-boto3-customer-profiles-1.28.15.post1.tar` & `mypy-boto3-customer-profiles-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:54.341096 mypy-boto3-customer-profiles-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:41:50.000000 mypy-boto3-customer-profiles-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20351 2023-07-29 10:02:54.329096 mypy-boto3-customer-profiles-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18819 2023-07-29 09:41:50.000000 mypy-boto3-customer-profiles-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:54.317096 mypy-boto3-customer-profiles-1.28.15.post1/mypy_boto3_customer_profiles/
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-29 09:41:50.000000 mypy-boto3-customer-profiles-1.28.15.post1/mypy_boto3_customer_profiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-29 09:41:50.000000 mypy-boto3-customer-profiles-1.28.15.post1/mypy_boto3_customer_profiles/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-29 09:41:50.000000 mypy-boto3-customer-profiles-1.28.15.post1/mypy_boto3_customer_profiles/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40567 2023-07-29 09:41:50.000000 mypy-boto3-customer-profiles-1.28.15.post1/mypy_boto3_customer_profiles/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    40508 2023-07-29 09:41:50.000000 mypy-boto3-customer-profiles-1.28.15.post1/mypy_boto3_customer_profiles/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13058 2023-07-29 09:41:51.000000 mypy-boto3-customer-profiles-1.28.15.post1/mypy_boto3_customer_profiles/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13056 2023-07-29 09:41:51.000000 mypy-boto3-customer-profiles-1.28.15.post1/mypy_boto3_customer_profiles/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-29 09:41:51.000000 mypy-boto3-customer-profiles-1.28.15.post1/mypy_boto3_customer_profiles/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-07-29 09:41:50.000000 mypy-boto3-customer-profiles-1.28.15.post1/mypy_boto3_customer_profiles/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:41:50.000000 mypy-boto3-customer-profiles-1.28.15.post1/mypy_boto3_customer_profiles/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    69344 2023-07-29 09:41:54.000000 mypy-boto3-customer-profiles-1.28.15.post1/mypy_boto3_customer_profiles/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    69244 2023-07-29 09:41:53.000000 mypy-boto3-customer-profiles-1.28.15.post1/mypy_boto3_customer_profiles/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:41:50.000000 mypy-boto3-customer-profiles-1.28.15.post1/mypy_boto3_customer_profiles/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:54.329096 mypy-boto3-customer-profiles-1.28.15.post1/mypy_boto3_customer_profiles.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20351 2023-07-29 10:02:54.000000 mypy-boto3-customer-profiles-1.28.15.post1/mypy_boto3_customer_profiles.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-29 10:02:54.000000 mypy-boto3-customer-profiles-1.28.15.post1/mypy_boto3_customer_profiles.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:54.000000 mypy-boto3-customer-profiles-1.28.15.post1/mypy_boto3_customer_profiles.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:54.000000 mypy-boto3-customer-profiles-1.28.15.post1/mypy_boto3_customer_profiles.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:54.000000 mypy-boto3-customer-profiles-1.28.15.post1/mypy_boto3_customer_profiles.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-29 10:02:54.000000 mypy-boto3-customer-profiles-1.28.15.post1/mypy_boto3_customer_profiles.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:54.341096 mypy-boto3-customer-profiles-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-07-29 09:41:50.000000 mypy-boto3-customer-profiles-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:35.296913 mypy-boto3-customer-profiles-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:14:23.000000 mypy-boto3-customer-profiles-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20459 2023-08-01 11:36:35.296913 mypy-boto3-customer-profiles-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18936 2023-08-01 11:14:23.000000 mypy-boto3-customer-profiles-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:35.288913 mypy-boto3-customer-profiles-1.28.16/mypy_boto3_customer_profiles/
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-08-01 11:14:23.000000 mypy-boto3-customer-profiles-1.28.16/mypy_boto3_customer_profiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-08-01 11:14:23.000000 mypy-boto3-customer-profiles-1.28.16/mypy_boto3_customer_profiles/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-08-01 11:14:23.000000 mypy-boto3-customer-profiles-1.28.16/mypy_boto3_customer_profiles/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40367 2023-08-01 11:14:24.000000 mypy-boto3-customer-profiles-1.28.16/mypy_boto3_customer_profiles/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40308 2023-08-01 11:14:24.000000 mypy-boto3-customer-profiles-1.28.16/mypy_boto3_customer_profiles/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13058 2023-08-01 11:14:25.000000 mypy-boto3-customer-profiles-1.28.16/mypy_boto3_customer_profiles/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13056 2023-08-01 11:14:25.000000 mypy-boto3-customer-profiles-1.28.16/mypy_boto3_customer_profiles/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-08-01 11:14:24.000000 mypy-boto3-customer-profiles-1.28.16/mypy_boto3_customer_profiles/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-08-01 11:14:24.000000 mypy-boto3-customer-profiles-1.28.16/mypy_boto3_customer_profiles/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:14:23.000000 mypy-boto3-customer-profiles-1.28.16/mypy_boto3_customer_profiles/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    69711 2023-08-01 11:14:27.000000 mypy-boto3-customer-profiles-1.28.16/mypy_boto3_customer_profiles/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69611 2023-08-01 11:14:26.000000 mypy-boto3-customer-profiles-1.28.16/mypy_boto3_customer_profiles/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:14:23.000000 mypy-boto3-customer-profiles-1.28.16/mypy_boto3_customer_profiles/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:35.296913 mypy-boto3-customer-profiles-1.28.16/mypy_boto3_customer_profiles.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20459 2023-08-01 11:36:35.000000 mypy-boto3-customer-profiles-1.28.16/mypy_boto3_customer_profiles.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-08-01 11:36:35.000000 mypy-boto3-customer-profiles-1.28.16/mypy_boto3_customer_profiles.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:35.000000 mypy-boto3-customer-profiles-1.28.16/mypy_boto3_customer_profiles.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:35.000000 mypy-boto3-customer-profiles-1.28.16/mypy_boto3_customer_profiles.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:35.000000 mypy-boto3-customer-profiles-1.28.16/mypy_boto3_customer_profiles.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-01 11:36:35.000000 mypy-boto3-customer-profiles-1.28.16/mypy_boto3_customer_profiles.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:35.296913 mypy-boto3-customer-profiles-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-08-01 11:14:23.000000 mypy-boto3-customer-profiles-1.28.16/setup.py
```

### Comparing `mypy-boto3-customer-profiles-1.28.15.post1/LICENSE` & `mypy-boto3-customer-profiles-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-customer-profiles-1.28.15.post1/PKG-INFO` & `mypy-boto3-customer-profiles-1.28.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-customer-profiles
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.CustomerProfiles 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.CustomerProfiles 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 customer-profiles type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 customer-profiles type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-customer-profiles.svg?color=blue)](https://pypi.org/project/mypy-boto3-customer-profiles)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-customer-profiles)](https://pepy.tech/project/mypy-boto3-customer-profiles)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CustomerProfiles 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles)
+[boto3.CustomerProfiles 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles)
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
 [mypy-boto3-customer-profiles docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/).
 
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
@@ -339,37 +339,37 @@
 )
 
 
 def check_value(value: AttributeMatchingModelType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_customer_profiles.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_customer_profiles.type_defs import (
     AddProfileKeyRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     AdditionalSearchKeyTypeDef,
     AddressTypeDef,
-    BatchTypeDef,
     AppflowIntegrationWorkflowAttributesTypeDef,
     AppflowIntegrationWorkflowMetricsTypeDef,
     AppflowIntegrationWorkflowStepTypeDef,
     AttributeItemTypeDef,
     AttributeTypesSelectorOutputTypeDef,
     AttributeTypesSelectorTypeDef,
     ConflictResolutionTypeDef,
     ConsolidationOutputTypeDef,
     ConsolidationTypeDef,
+    TimestampTypeDef,
     RangeTypeDef,
     ThresholdTypeDef,
     ConnectorOperatorTypeDef,
     CreateEventStreamRequestRequestTypeDef,
     DeleteCalculatedAttributeDefinitionRequestRequestTypeDef,
     DeleteDomainRequestRequestTypeDef,
     DeleteEventStreamRequestRequestTypeDef,
@@ -421,23 +421,21 @@
     ListProfileObjectTypeTemplatesRequestRequestTypeDef,
     ListProfileObjectTypesRequestRequestTypeDef,
     ListProfileObjectsItemTypeDef,
     ObjectFilterTypeDef,
     ListRuleBasedMatchesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListWorkflowsItemTypeDef,
-    ListWorkflowsRequestRequestTypeDef,
     MarketoSourcePropertiesTypeDef,
     MatchingRuleOutputTypeDef,
     MatchingRuleTypeDef,
     ObjectTypeKeyTypeDef,
     PutProfileObjectRequestRequestTypeDef,
     S3SourcePropertiesTypeDef,
     SalesforceSourcePropertiesTypeDef,
-    ScheduledTriggerPropertiesTypeDef,
     ServiceNowSourcePropertiesTypeDef,
     ZendeskSourcePropertiesTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAddressTypeDef,
     AddProfileKeyResponseTypeDef,
     CreateEventStreamResponseTypeDef,
@@ -464,15 +462,19 @@
     WorkflowAttributesTypeDef,
     WorkflowMetricsTypeDef,
     WorkflowStepItemTypeDef,
     AttributeDetailsOutputTypeDef,
     AttributeDetailsTypeDef,
     AutoMergingOutputTypeDef,
     AutoMergingTypeDef,
+    ConsolidationUnionTypeDef,
     GetAutoMergingPreviewRequestRequestTypeDef,
+    BatchTypeDef,
+    ListWorkflowsRequestRequestTypeDef,
+    ScheduledTriggerPropertiesTypeDef,
     ConditionsTypeDef,
     TaskTypeDef,
     EventStreamSummaryTypeDef,
     GetEventStreamResponseTypeDef,
     ExportingConfigTypeDef,
     ExportingLocationTypeDef,
     MergeProfilesRequestRequestTypeDef,
@@ -488,50 +490,52 @@
     ListDomainsResponseTypeDef,
     ListEventStreamsRequestListEventStreamsPaginateTypeDef,
     ListProfileObjectTypesResponseTypeDef,
     ListProfileObjectTypeTemplatesResponseTypeDef,
     ListProfileObjectsResponseTypeDef,
     ListProfileObjectsRequestRequestTypeDef,
     ListWorkflowsResponseTypeDef,
-    PutProfileObjectTypeRequestRequestTypeDef,
-    TriggerPropertiesTypeDef,
+    ObjectTypeKeyUnionTypeDef,
     SourceConnectorPropertiesTypeDef,
     UpdateProfileRequestRequestTypeDef,
     GetWorkflowResponseTypeDef,
     GetWorkflowStepsResponseTypeDef,
+    AttributeDetailsUnionTypeDef,
+    TriggerPropertiesTypeDef,
     CreateCalculatedAttributeDefinitionRequestRequestTypeDef,
     CreateCalculatedAttributeDefinitionResponseTypeDef,
     GetCalculatedAttributeDefinitionResponseTypeDef,
     UpdateCalculatedAttributeDefinitionRequestRequestTypeDef,
     UpdateCalculatedAttributeDefinitionResponseTypeDef,
     ListEventStreamsResponseTypeDef,
     MatchingRequestTypeDef,
     MatchingResponseTypeDef,
     RuleBasedMatchingRequestTypeDef,
     RuleBasedMatchingResponseTypeDef,
     GetIdentityResolutionJobResponseTypeDef,
     IdentityResolutionJobTypeDef,
     SearchProfilesResponseTypeDef,
-    TriggerConfigTypeDef,
+    PutProfileObjectTypeRequestRequestTypeDef,
     SourceFlowConfigTypeDef,
+    TriggerConfigTypeDef,
     CreateDomainRequestRequestTypeDef,
     UpdateDomainRequestRequestTypeDef,
     CreateDomainResponseTypeDef,
     GetDomainResponseTypeDef,
     UpdateDomainResponseTypeDef,
     ListIdentityResolutionJobsResponseTypeDef,
     FlowDefinitionTypeDef,
     AppflowIntegrationTypeDef,
     PutIntegrationRequestRequestTypeDef,
     IntegrationConfigTypeDef,
     CreateIntegrationWorkflowRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AddProfileKeyRequestRequestTypeDef:
+def get_value() -> AddProfileKeyRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-customer-profiles-1.28.15.post1/README.md` & `mypy-boto3-customer-profiles-1.28.16/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-customer-profiles.svg?color=blue)](https://pypi.org/project/mypy-boto3-customer-profiles)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-customer-profiles)](https://pepy.tech/project/mypy-boto3-customer-profiles)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CustomerProfiles 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles)
+[boto3.CustomerProfiles 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles)
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
 [mypy-boto3-customer-profiles docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/).
 
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
@@ -307,37 +307,37 @@
 )
 
 
 def check_value(value: AttributeMatchingModelType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_customer_profiles.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_customer_profiles.type_defs import (
     AddProfileKeyRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     AdditionalSearchKeyTypeDef,
     AddressTypeDef,
-    BatchTypeDef,
     AppflowIntegrationWorkflowAttributesTypeDef,
     AppflowIntegrationWorkflowMetricsTypeDef,
     AppflowIntegrationWorkflowStepTypeDef,
     AttributeItemTypeDef,
     AttributeTypesSelectorOutputTypeDef,
     AttributeTypesSelectorTypeDef,
     ConflictResolutionTypeDef,
     ConsolidationOutputTypeDef,
     ConsolidationTypeDef,
+    TimestampTypeDef,
     RangeTypeDef,
     ThresholdTypeDef,
     ConnectorOperatorTypeDef,
     CreateEventStreamRequestRequestTypeDef,
     DeleteCalculatedAttributeDefinitionRequestRequestTypeDef,
     DeleteDomainRequestRequestTypeDef,
     DeleteEventStreamRequestRequestTypeDef,
@@ -389,23 +389,21 @@
     ListProfileObjectTypeTemplatesRequestRequestTypeDef,
     ListProfileObjectTypesRequestRequestTypeDef,
     ListProfileObjectsItemTypeDef,
     ObjectFilterTypeDef,
     ListRuleBasedMatchesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListWorkflowsItemTypeDef,
-    ListWorkflowsRequestRequestTypeDef,
     MarketoSourcePropertiesTypeDef,
     MatchingRuleOutputTypeDef,
     MatchingRuleTypeDef,
     ObjectTypeKeyTypeDef,
     PutProfileObjectRequestRequestTypeDef,
     S3SourcePropertiesTypeDef,
     SalesforceSourcePropertiesTypeDef,
-    ScheduledTriggerPropertiesTypeDef,
     ServiceNowSourcePropertiesTypeDef,
     ZendeskSourcePropertiesTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAddressTypeDef,
     AddProfileKeyResponseTypeDef,
     CreateEventStreamResponseTypeDef,
@@ -432,15 +430,19 @@
     WorkflowAttributesTypeDef,
     WorkflowMetricsTypeDef,
     WorkflowStepItemTypeDef,
     AttributeDetailsOutputTypeDef,
     AttributeDetailsTypeDef,
     AutoMergingOutputTypeDef,
     AutoMergingTypeDef,
+    ConsolidationUnionTypeDef,
     GetAutoMergingPreviewRequestRequestTypeDef,
+    BatchTypeDef,
+    ListWorkflowsRequestRequestTypeDef,
+    ScheduledTriggerPropertiesTypeDef,
     ConditionsTypeDef,
     TaskTypeDef,
     EventStreamSummaryTypeDef,
     GetEventStreamResponseTypeDef,
     ExportingConfigTypeDef,
     ExportingLocationTypeDef,
     MergeProfilesRequestRequestTypeDef,
@@ -456,50 +458,52 @@
     ListDomainsResponseTypeDef,
     ListEventStreamsRequestListEventStreamsPaginateTypeDef,
     ListProfileObjectTypesResponseTypeDef,
     ListProfileObjectTypeTemplatesResponseTypeDef,
     ListProfileObjectsResponseTypeDef,
     ListProfileObjectsRequestRequestTypeDef,
     ListWorkflowsResponseTypeDef,
-    PutProfileObjectTypeRequestRequestTypeDef,
-    TriggerPropertiesTypeDef,
+    ObjectTypeKeyUnionTypeDef,
     SourceConnectorPropertiesTypeDef,
     UpdateProfileRequestRequestTypeDef,
     GetWorkflowResponseTypeDef,
     GetWorkflowStepsResponseTypeDef,
+    AttributeDetailsUnionTypeDef,
+    TriggerPropertiesTypeDef,
     CreateCalculatedAttributeDefinitionRequestRequestTypeDef,
     CreateCalculatedAttributeDefinitionResponseTypeDef,
     GetCalculatedAttributeDefinitionResponseTypeDef,
     UpdateCalculatedAttributeDefinitionRequestRequestTypeDef,
     UpdateCalculatedAttributeDefinitionResponseTypeDef,
     ListEventStreamsResponseTypeDef,
     MatchingRequestTypeDef,
     MatchingResponseTypeDef,
     RuleBasedMatchingRequestTypeDef,
     RuleBasedMatchingResponseTypeDef,
     GetIdentityResolutionJobResponseTypeDef,
     IdentityResolutionJobTypeDef,
     SearchProfilesResponseTypeDef,
-    TriggerConfigTypeDef,
+    PutProfileObjectTypeRequestRequestTypeDef,
     SourceFlowConfigTypeDef,
+    TriggerConfigTypeDef,
     CreateDomainRequestRequestTypeDef,
     UpdateDomainRequestRequestTypeDef,
     CreateDomainResponseTypeDef,
     GetDomainResponseTypeDef,
     UpdateDomainResponseTypeDef,
     ListIdentityResolutionJobsResponseTypeDef,
     FlowDefinitionTypeDef,
     AppflowIntegrationTypeDef,
     PutIntegrationRequestRequestTypeDef,
     IntegrationConfigTypeDef,
     CreateIntegrationWorkflowRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AddProfileKeyRequestRequestTypeDef:
+def get_value() -> AddProfileKeyRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-customer-profiles-1.28.15.post1/mypy_boto3_customer_profiles/__init__.py` & `mypy-boto3-customer-profiles-1.28.16/mypy_boto3_customer_profiles/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-customer-profiles-1.28.15.post1/mypy_boto3_customer_profiles/__init__.pyi` & `mypy-boto3-customer-profiles-1.28.16/mypy_boto3_customer_profiles/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-customer-profiles-1.28.15.post1/mypy_boto3_customer_profiles/__main__.py` & `mypy-boto3-customer-profiles-1.28.16/mypy_boto3_customer_profiles/__main__.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CustomerProfiles 1.28.15\nVersion:        "
-        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.CustomerProfiles 1.28.16\nVersion:         1.28.16\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles//\nBoto3 docs:   "
         "   https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles\nOther"
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

### Comparing `mypy-boto3-customer-profiles-1.28.15.post1/mypy_boto3_customer_profiles/client.py` & `mypy-boto3-customer-profiles-1.28.16/mypy_boto3_customer_profiles/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from mypy_boto3_customer_profiles.client import CustomerProfilesClient
 
     session = Session()
     client: CustomerProfilesClient = session.client("customer-profiles")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     GenderType,
     MatchTypeType,
     PartyTypeType,
@@ -28,20 +27,18 @@
     logicalOperatorType,
 )
 from .paginator import ListEventStreamsPaginator
 from .type_defs import (
     AdditionalSearchKeyTypeDef,
     AddProfileKeyResponseTypeDef,
     AddressTypeDef,
-    AttributeDetailsOutputTypeDef,
-    AttributeDetailsTypeDef,
+    AttributeDetailsUnionTypeDef,
     ConditionsTypeDef,
     ConflictResolutionTypeDef,
-    ConsolidationOutputTypeDef,
-    ConsolidationTypeDef,
+    ConsolidationUnionTypeDef,
     CreateCalculatedAttributeDefinitionResponseTypeDef,
     CreateDomainResponseTypeDef,
     CreateEventStreamResponseTypeDef,
     CreateIntegrationWorkflowResponseTypeDef,
     CreateProfileResponseTypeDef,
     DeleteDomainResponseTypeDef,
     DeleteIntegrationResponseTypeDef,
@@ -78,21 +75,21 @@
     ListRuleBasedMatchesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListWorkflowsResponseTypeDef,
     MatchingRequestTypeDef,
     MergeProfilesResponseTypeDef,
     ObjectFilterTypeDef,
     ObjectTypeFieldTypeDef,
-    ObjectTypeKeyOutputTypeDef,
-    ObjectTypeKeyTypeDef,
+    ObjectTypeKeyUnionTypeDef,
     PutIntegrationResponseTypeDef,
     PutProfileObjectResponseTypeDef,
     PutProfileObjectTypeResponseTypeDef,
     RuleBasedMatchingRequestTypeDef,
     SearchProfilesResponseTypeDef,
+    TimestampTypeDef,
     UpdateAddressTypeDef,
     UpdateCalculatedAttributeDefinitionResponseTypeDef,
     UpdateDomainResponseTypeDef,
     UpdateProfileResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
@@ -166,15 +163,15 @@
         """
 
     def create_calculated_attribute_definition(
         self,
         *,
         DomainName: str,
         CalculatedAttributeName: str,
-        AttributeDetails: Union[AttributeDetailsTypeDef, AttributeDetailsOutputTypeDef],
+        AttributeDetails: AttributeDetailsUnionTypeDef,
         Statistic: StatisticType,
         DisplayName: str = ...,
         Description: str = ...,
         Conditions: ConditionsTypeDef = ...,
         Tags: Mapping[str, str] = ...
     ) -> CreateCalculatedAttributeDefinitionResponseTypeDef:
         """
@@ -362,15 +359,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#generate_presigned_url)
         """
 
     def get_auto_merging_preview(
         self,
         *,
         DomainName: str,
-        Consolidation: Union[ConsolidationTypeDef, ConsolidationOutputTypeDef],
+        Consolidation: ConsolidationUnionTypeDef,
         ConflictResolution: ConflictResolutionTypeDef,
         MinAllowedConfidenceScoreForMerging: float = ...
     ) -> GetAutoMergingPreviewResponseTypeDef:
         """
         Tests the auto-merging settings of your Identity Resolution Job without merging
         your data.
 
@@ -640,16 +637,16 @@
 
     def list_workflows(
         self,
         *,
         DomainName: str,
         WorkflowType: Literal["APPFLOW_INTEGRATION"] = ...,
         Status: StatusType = ...,
-        QueryStartDate: Union[datetime, str] = ...,
-        QueryEndDate: Union[datetime, str] = ...,
+        QueryStartDate: TimestampTypeDef = ...,
+        QueryEndDate: TimestampTypeDef = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListWorkflowsResponseTypeDef:
         """
         Query to list all workflows.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.list_workflows)
@@ -708,15 +705,15 @@
         Description: str,
         TemplateId: str = ...,
         ExpirationDays: int = ...,
         EncryptionKey: str = ...,
         AllowProfileCreation: bool = ...,
         SourceLastUpdatedTimestampFormat: str = ...,
         Fields: Mapping[str, ObjectTypeFieldTypeDef] = ...,
-        Keys: Mapping[str, Sequence[Union[ObjectTypeKeyTypeDef, ObjectTypeKeyOutputTypeDef]]] = ...,
+        Keys: Mapping[str, Sequence[ObjectTypeKeyUnionTypeDef]] = ...,
         Tags: Mapping[str, str] = ...
     ) -> PutProfileObjectTypeResponseTypeDef:
         """
         Defines a ProfileObjectType.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.put_profile_object_type)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#put_profile_object_type)
```

### Comparing `mypy-boto3-customer-profiles-1.28.15.post1/mypy_boto3_customer_profiles/client.pyi` & `mypy-boto3-customer-profiles-1.28.16/mypy_boto3_customer_profiles/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from mypy_boto3_customer_profiles.client import CustomerProfilesClient
 
     session = Session()
     client: CustomerProfilesClient = session.client("customer-profiles")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     GenderType,
     MatchTypeType,
     PartyTypeType,
@@ -28,20 +27,18 @@
     logicalOperatorType,
 )
 from .paginator import ListEventStreamsPaginator
 from .type_defs import (
     AdditionalSearchKeyTypeDef,
     AddProfileKeyResponseTypeDef,
     AddressTypeDef,
-    AttributeDetailsOutputTypeDef,
-    AttributeDetailsTypeDef,
+    AttributeDetailsUnionTypeDef,
     ConditionsTypeDef,
     ConflictResolutionTypeDef,
-    ConsolidationOutputTypeDef,
-    ConsolidationTypeDef,
+    ConsolidationUnionTypeDef,
     CreateCalculatedAttributeDefinitionResponseTypeDef,
     CreateDomainResponseTypeDef,
     CreateEventStreamResponseTypeDef,
     CreateIntegrationWorkflowResponseTypeDef,
     CreateProfileResponseTypeDef,
     DeleteDomainResponseTypeDef,
     DeleteIntegrationResponseTypeDef,
@@ -78,21 +75,21 @@
     ListRuleBasedMatchesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListWorkflowsResponseTypeDef,
     MatchingRequestTypeDef,
     MergeProfilesResponseTypeDef,
     ObjectFilterTypeDef,
     ObjectTypeFieldTypeDef,
-    ObjectTypeKeyOutputTypeDef,
-    ObjectTypeKeyTypeDef,
+    ObjectTypeKeyUnionTypeDef,
     PutIntegrationResponseTypeDef,
     PutProfileObjectResponseTypeDef,
     PutProfileObjectTypeResponseTypeDef,
     RuleBasedMatchingRequestTypeDef,
     SearchProfilesResponseTypeDef,
+    TimestampTypeDef,
     UpdateAddressTypeDef,
     UpdateCalculatedAttributeDefinitionResponseTypeDef,
     UpdateDomainResponseTypeDef,
     UpdateProfileResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
@@ -158,15 +155,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#close)
         """
     def create_calculated_attribute_definition(
         self,
         *,
         DomainName: str,
         CalculatedAttributeName: str,
-        AttributeDetails: Union[AttributeDetailsTypeDef, AttributeDetailsOutputTypeDef],
+        AttributeDetails: AttributeDetailsUnionTypeDef,
         Statistic: StatisticType,
         DisplayName: str = ...,
         Description: str = ...,
         Conditions: ConditionsTypeDef = ...,
         Tags: Mapping[str, str] = ...
     ) -> CreateCalculatedAttributeDefinitionResponseTypeDef:
         """
@@ -339,15 +336,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#generate_presigned_url)
         """
     def get_auto_merging_preview(
         self,
         *,
         DomainName: str,
-        Consolidation: Union[ConsolidationTypeDef, ConsolidationOutputTypeDef],
+        Consolidation: ConsolidationUnionTypeDef,
         ConflictResolution: ConflictResolutionTypeDef,
         MinAllowedConfidenceScoreForMerging: float = ...
     ) -> GetAutoMergingPreviewResponseTypeDef:
         """
         Tests the auto-merging settings of your Identity Resolution Job without merging
         your data.
 
@@ -592,16 +589,16 @@
         """
     def list_workflows(
         self,
         *,
         DomainName: str,
         WorkflowType: Literal["APPFLOW_INTEGRATION"] = ...,
         Status: StatusType = ...,
-        QueryStartDate: Union[datetime, str] = ...,
-        QueryEndDate: Union[datetime, str] = ...,
+        QueryStartDate: TimestampTypeDef = ...,
+        QueryEndDate: TimestampTypeDef = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListWorkflowsResponseTypeDef:
         """
         Query to list all workflows.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.list_workflows)
@@ -656,15 +653,15 @@
         Description: str,
         TemplateId: str = ...,
         ExpirationDays: int = ...,
         EncryptionKey: str = ...,
         AllowProfileCreation: bool = ...,
         SourceLastUpdatedTimestampFormat: str = ...,
         Fields: Mapping[str, ObjectTypeFieldTypeDef] = ...,
-        Keys: Mapping[str, Sequence[Union[ObjectTypeKeyTypeDef, ObjectTypeKeyOutputTypeDef]]] = ...,
+        Keys: Mapping[str, Sequence[ObjectTypeKeyUnionTypeDef]] = ...,
         Tags: Mapping[str, str] = ...
     ) -> PutProfileObjectTypeResponseTypeDef:
         """
         Defines a ProfileObjectType.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.put_profile_object_type)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#put_profile_object_type)
```

### Comparing `mypy-boto3-customer-profiles-1.28.15.post1/mypy_boto3_customer_profiles/literals.py` & `mypy-boto3-customer-profiles-1.28.16/mypy_boto3_customer_profiles/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-customer-profiles-1.28.15.post1/mypy_boto3_customer_profiles/literals.pyi` & `mypy-boto3-customer-profiles-1.28.16/mypy_boto3_customer_profiles/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-customer-profiles-1.28.15.post1/mypy_boto3_customer_profiles/paginator.py` & `mypy-boto3-customer-profiles-1.28.16/mypy_boto3_customer_profiles/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-customer-profiles-1.28.15.post1/mypy_boto3_customer_profiles/paginator.pyi` & `mypy-boto3-customer-profiles-1.28.16/mypy_boto3_customer_profiles/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-customer-profiles-1.28.15.post1/mypy_boto3_customer_profiles/type_defs.py` & `mypy-boto3-customer-profiles-1.28.16/mypy_boto3_customer_profiles/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_customer_profiles.type_defs import AddProfileKeyRequestRequestTypeDef
 
-    data: AddProfileKeyRequestRequestTypeDef = {...}
+    data: AddProfileKeyRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -55,24 +55,24 @@
 
 
 __all__ = (
     "AddProfileKeyRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "AdditionalSearchKeyTypeDef",
     "AddressTypeDef",
-    "BatchTypeDef",
     "AppflowIntegrationWorkflowAttributesTypeDef",
     "AppflowIntegrationWorkflowMetricsTypeDef",
     "AppflowIntegrationWorkflowStepTypeDef",
     "AttributeItemTypeDef",
     "AttributeTypesSelectorOutputTypeDef",
     "AttributeTypesSelectorTypeDef",
     "ConflictResolutionTypeDef",
     "ConsolidationOutputTypeDef",
     "ConsolidationTypeDef",
+    "TimestampTypeDef",
     "RangeTypeDef",
     "ThresholdTypeDef",
     "ConnectorOperatorTypeDef",
     "CreateEventStreamRequestRequestTypeDef",
     "DeleteCalculatedAttributeDefinitionRequestRequestTypeDef",
     "DeleteDomainRequestRequestTypeDef",
     "DeleteEventStreamRequestRequestTypeDef",
@@ -124,23 +124,21 @@
     "ListProfileObjectTypeTemplatesRequestRequestTypeDef",
     "ListProfileObjectTypesRequestRequestTypeDef",
     "ListProfileObjectsItemTypeDef",
     "ObjectFilterTypeDef",
     "ListRuleBasedMatchesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListWorkflowsItemTypeDef",
-    "ListWorkflowsRequestRequestTypeDef",
     "MarketoSourcePropertiesTypeDef",
     "MatchingRuleOutputTypeDef",
     "MatchingRuleTypeDef",
     "ObjectTypeKeyTypeDef",
     "PutProfileObjectRequestRequestTypeDef",
     "S3SourcePropertiesTypeDef",
     "SalesforceSourcePropertiesTypeDef",
-    "ScheduledTriggerPropertiesTypeDef",
     "ServiceNowSourcePropertiesTypeDef",
     "ZendeskSourcePropertiesTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAddressTypeDef",
     "AddProfileKeyResponseTypeDef",
     "CreateEventStreamResponseTypeDef",
@@ -167,15 +165,19 @@
     "WorkflowAttributesTypeDef",
     "WorkflowMetricsTypeDef",
     "WorkflowStepItemTypeDef",
     "AttributeDetailsOutputTypeDef",
     "AttributeDetailsTypeDef",
     "AutoMergingOutputTypeDef",
     "AutoMergingTypeDef",
+    "ConsolidationUnionTypeDef",
     "GetAutoMergingPreviewRequestRequestTypeDef",
+    "BatchTypeDef",
+    "ListWorkflowsRequestRequestTypeDef",
+    "ScheduledTriggerPropertiesTypeDef",
     "ConditionsTypeDef",
     "TaskTypeDef",
     "EventStreamSummaryTypeDef",
     "GetEventStreamResponseTypeDef",
     "ExportingConfigTypeDef",
     "ExportingLocationTypeDef",
     "MergeProfilesRequestRequestTypeDef",
@@ -191,35 +193,37 @@
     "ListDomainsResponseTypeDef",
     "ListEventStreamsRequestListEventStreamsPaginateTypeDef",
     "ListProfileObjectTypesResponseTypeDef",
     "ListProfileObjectTypeTemplatesResponseTypeDef",
     "ListProfileObjectsResponseTypeDef",
     "ListProfileObjectsRequestRequestTypeDef",
     "ListWorkflowsResponseTypeDef",
-    "PutProfileObjectTypeRequestRequestTypeDef",
-    "TriggerPropertiesTypeDef",
+    "ObjectTypeKeyUnionTypeDef",
     "SourceConnectorPropertiesTypeDef",
     "UpdateProfileRequestRequestTypeDef",
     "GetWorkflowResponseTypeDef",
     "GetWorkflowStepsResponseTypeDef",
+    "AttributeDetailsUnionTypeDef",
+    "TriggerPropertiesTypeDef",
     "CreateCalculatedAttributeDefinitionRequestRequestTypeDef",
     "CreateCalculatedAttributeDefinitionResponseTypeDef",
     "GetCalculatedAttributeDefinitionResponseTypeDef",
     "UpdateCalculatedAttributeDefinitionRequestRequestTypeDef",
     "UpdateCalculatedAttributeDefinitionResponseTypeDef",
     "ListEventStreamsResponseTypeDef",
     "MatchingRequestTypeDef",
     "MatchingResponseTypeDef",
     "RuleBasedMatchingRequestTypeDef",
     "RuleBasedMatchingResponseTypeDef",
     "GetIdentityResolutionJobResponseTypeDef",
     "IdentityResolutionJobTypeDef",
     "SearchProfilesResponseTypeDef",
-    "TriggerConfigTypeDef",
+    "PutProfileObjectTypeRequestRequestTypeDef",
     "SourceFlowConfigTypeDef",
+    "TriggerConfigTypeDef",
     "CreateDomainRequestRequestTypeDef",
     "UpdateDomainRequestRequestTypeDef",
     "CreateDomainResponseTypeDef",
     "GetDomainResponseTypeDef",
     "UpdateDomainResponseTypeDef",
     "ListIdentityResolutionJobsResponseTypeDef",
     "FlowDefinitionTypeDef",
@@ -271,22 +275,14 @@
         "Province": str,
         "Country": str,
         "PostalCode": str,
     },
     total=False,
 )
 
-BatchTypeDef = TypedDict(
-    "BatchTypeDef",
-    {
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-    },
-)
-
 _RequiredAppflowIntegrationWorkflowAttributesTypeDef = TypedDict(
     "_RequiredAppflowIntegrationWorkflowAttributesTypeDef",
     {
         "SourceConnectorType": SourceConnectorTypeType,
         "ConnectorProfileName": str,
     },
 )
@@ -413,14 +409,15 @@
 ConsolidationTypeDef = TypedDict(
     "ConsolidationTypeDef",
     {
         "MatchingAttributesList": Sequence[Sequence[str]],
     },
 )
 
+TimestampTypeDef = Union[datetime, str]
 RangeTypeDef = TypedDict(
     "RangeTypeDef",
     {
         "Value": int,
         "Unit": Literal["DAYS"],
     },
 )
@@ -1216,40 +1213,14 @@
         "Status": StatusType,
         "StatusDescription": str,
         "CreatedAt": datetime,
         "LastUpdatedAt": datetime,
     },
 )
 
-_RequiredListWorkflowsRequestRequestTypeDef = TypedDict(
-    "_RequiredListWorkflowsRequestRequestTypeDef",
-    {
-        "DomainName": str,
-    },
-)
-_OptionalListWorkflowsRequestRequestTypeDef = TypedDict(
-    "_OptionalListWorkflowsRequestRequestTypeDef",
-    {
-        "WorkflowType": Literal["APPFLOW_INTEGRATION"],
-        "Status": StatusType,
-        "QueryStartDate": Union[datetime, str],
-        "QueryEndDate": Union[datetime, str],
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
-
-class ListWorkflowsRequestRequestTypeDef(
-    _RequiredListWorkflowsRequestRequestTypeDef, _OptionalListWorkflowsRequestRequestTypeDef
-):
-    pass
-
-
 MarketoSourcePropertiesTypeDef = TypedDict(
     "MarketoSourcePropertiesTypeDef",
     {
         "Object": str,
     },
 )
 
@@ -1324,40 +1295,14 @@
 
 class SalesforceSourcePropertiesTypeDef(
     _RequiredSalesforceSourcePropertiesTypeDef, _OptionalSalesforceSourcePropertiesTypeDef
 ):
     pass
 
 
-_RequiredScheduledTriggerPropertiesTypeDef = TypedDict(
-    "_RequiredScheduledTriggerPropertiesTypeDef",
-    {
-        "ScheduleExpression": str,
-    },
-)
-_OptionalScheduledTriggerPropertiesTypeDef = TypedDict(
-    "_OptionalScheduledTriggerPropertiesTypeDef",
-    {
-        "DataPullMode": DataPullModeType,
-        "ScheduleStartTime": Union[datetime, str],
-        "ScheduleEndTime": Union[datetime, str],
-        "Timezone": str,
-        "ScheduleOffset": int,
-        "FirstExecutionFrom": Union[datetime, str],
-    },
-    total=False,
-)
-
-
-class ScheduledTriggerPropertiesTypeDef(
-    _RequiredScheduledTriggerPropertiesTypeDef, _OptionalScheduledTriggerPropertiesTypeDef
-):
-    pass
-
-
 ServiceNowSourcePropertiesTypeDef = TypedDict(
     "ServiceNowSourcePropertiesTypeDef",
     {
         "Object": str,
     },
 )
 
@@ -1741,14 +1686,15 @@
 )
 
 
 class AutoMergingTypeDef(_RequiredAutoMergingTypeDef, _OptionalAutoMergingTypeDef):
     pass
 
 
+ConsolidationUnionTypeDef = Union[ConsolidationTypeDef, ConsolidationOutputTypeDef]
 _RequiredGetAutoMergingPreviewRequestRequestTypeDef = TypedDict(
     "_RequiredGetAutoMergingPreviewRequestRequestTypeDef",
     {
         "DomainName": str,
         "Consolidation": ConsolidationTypeDef,
         "ConflictResolution": ConflictResolutionTypeDef,
     },
@@ -1765,14 +1711,74 @@
 class GetAutoMergingPreviewRequestRequestTypeDef(
     _RequiredGetAutoMergingPreviewRequestRequestTypeDef,
     _OptionalGetAutoMergingPreviewRequestRequestTypeDef,
 ):
     pass
 
 
+BatchTypeDef = TypedDict(
+    "BatchTypeDef",
+    {
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+    },
+)
+
+_RequiredListWorkflowsRequestRequestTypeDef = TypedDict(
+    "_RequiredListWorkflowsRequestRequestTypeDef",
+    {
+        "DomainName": str,
+    },
+)
+_OptionalListWorkflowsRequestRequestTypeDef = TypedDict(
+    "_OptionalListWorkflowsRequestRequestTypeDef",
+    {
+        "WorkflowType": Literal["APPFLOW_INTEGRATION"],
+        "Status": StatusType,
+        "QueryStartDate": TimestampTypeDef,
+        "QueryEndDate": TimestampTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+
+class ListWorkflowsRequestRequestTypeDef(
+    _RequiredListWorkflowsRequestRequestTypeDef, _OptionalListWorkflowsRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredScheduledTriggerPropertiesTypeDef = TypedDict(
+    "_RequiredScheduledTriggerPropertiesTypeDef",
+    {
+        "ScheduleExpression": str,
+    },
+)
+_OptionalScheduledTriggerPropertiesTypeDef = TypedDict(
+    "_OptionalScheduledTriggerPropertiesTypeDef",
+    {
+        "DataPullMode": DataPullModeType,
+        "ScheduleStartTime": TimestampTypeDef,
+        "ScheduleEndTime": TimestampTypeDef,
+        "Timezone": str,
+        "ScheduleOffset": int,
+        "FirstExecutionFrom": TimestampTypeDef,
+    },
+    total=False,
+)
+
+
+class ScheduledTriggerPropertiesTypeDef(
+    _RequiredScheduledTriggerPropertiesTypeDef, _OptionalScheduledTriggerPropertiesTypeDef
+):
+    pass
+
+
 ConditionsTypeDef = TypedDict(
     "ConditionsTypeDef",
     {
         "Range": RangeTypeDef,
         "ObjectCount": int,
         "Threshold": ThresholdTypeDef,
     },
@@ -2100,53 +2106,15 @@
     {
         "Items": List[ListWorkflowsItemTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredPutProfileObjectTypeRequestRequestTypeDef = TypedDict(
-    "_RequiredPutProfileObjectTypeRequestRequestTypeDef",
-    {
-        "DomainName": str,
-        "ObjectTypeName": str,
-        "Description": str,
-    },
-)
-_OptionalPutProfileObjectTypeRequestRequestTypeDef = TypedDict(
-    "_OptionalPutProfileObjectTypeRequestRequestTypeDef",
-    {
-        "TemplateId": str,
-        "ExpirationDays": int,
-        "EncryptionKey": str,
-        "AllowProfileCreation": bool,
-        "SourceLastUpdatedTimestampFormat": str,
-        "Fields": Mapping[str, ObjectTypeFieldTypeDef],
-        "Keys": Mapping[str, Sequence[Union[ObjectTypeKeyTypeDef, ObjectTypeKeyOutputTypeDef]]],
-        "Tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-
-class PutProfileObjectTypeRequestRequestTypeDef(
-    _RequiredPutProfileObjectTypeRequestRequestTypeDef,
-    _OptionalPutProfileObjectTypeRequestRequestTypeDef,
-):
-    pass
-
-
-TriggerPropertiesTypeDef = TypedDict(
-    "TriggerPropertiesTypeDef",
-    {
-        "Scheduled": ScheduledTriggerPropertiesTypeDef,
-    },
-    total=False,
-)
-
+ObjectTypeKeyUnionTypeDef = Union[ObjectTypeKeyTypeDef, ObjectTypeKeyOutputTypeDef]
 SourceConnectorPropertiesTypeDef = TypedDict(
     "SourceConnectorPropertiesTypeDef",
     {
         "Marketo": MarketoSourcePropertiesTypeDef,
         "S3": S3SourcePropertiesTypeDef,
         "Salesforce": SalesforceSourcePropertiesTypeDef,
         "ServiceNow": ServiceNowSourcePropertiesTypeDef,
@@ -2221,14 +2189,23 @@
         "WorkflowType": Literal["APPFLOW_INTEGRATION"],
         "Items": List[WorkflowStepItemTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+AttributeDetailsUnionTypeDef = Union[AttributeDetailsTypeDef, AttributeDetailsOutputTypeDef]
+TriggerPropertiesTypeDef = TypedDict(
+    "TriggerPropertiesTypeDef",
+    {
+        "Scheduled": ScheduledTriggerPropertiesTypeDef,
+    },
+    total=False,
+)
+
 _RequiredCreateCalculatedAttributeDefinitionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCalculatedAttributeDefinitionRequestRequestTypeDef",
     {
         "DomainName": str,
         "CalculatedAttributeName": str,
         "AttributeDetails": AttributeDetailsTypeDef,
         "Statistic": StatisticType,
@@ -2446,30 +2423,42 @@
     {
         "Items": List[ProfileTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredTriggerConfigTypeDef = TypedDict(
-    "_RequiredTriggerConfigTypeDef",
+_RequiredPutProfileObjectTypeRequestRequestTypeDef = TypedDict(
+    "_RequiredPutProfileObjectTypeRequestRequestTypeDef",
     {
-        "TriggerType": TriggerTypeType,
+        "DomainName": str,
+        "ObjectTypeName": str,
+        "Description": str,
     },
 )
-_OptionalTriggerConfigTypeDef = TypedDict(
-    "_OptionalTriggerConfigTypeDef",
+_OptionalPutProfileObjectTypeRequestRequestTypeDef = TypedDict(
+    "_OptionalPutProfileObjectTypeRequestRequestTypeDef",
     {
-        "TriggerProperties": TriggerPropertiesTypeDef,
+        "TemplateId": str,
+        "ExpirationDays": int,
+        "EncryptionKey": str,
+        "AllowProfileCreation": bool,
+        "SourceLastUpdatedTimestampFormat": str,
+        "Fields": Mapping[str, ObjectTypeFieldTypeDef],
+        "Keys": Mapping[str, Sequence[ObjectTypeKeyUnionTypeDef]],
+        "Tags": Mapping[str, str],
     },
     total=False,
 )
 
 
-class TriggerConfigTypeDef(_RequiredTriggerConfigTypeDef, _OptionalTriggerConfigTypeDef):
+class PutProfileObjectTypeRequestRequestTypeDef(
+    _RequiredPutProfileObjectTypeRequestRequestTypeDef,
+    _OptionalPutProfileObjectTypeRequestRequestTypeDef,
+):
     pass
 
 
 _RequiredSourceFlowConfigTypeDef = TypedDict(
     "_RequiredSourceFlowConfigTypeDef",
     {
         "ConnectorType": SourceConnectorTypeType,
@@ -2486,14 +2475,33 @@
 )
 
 
 class SourceFlowConfigTypeDef(_RequiredSourceFlowConfigTypeDef, _OptionalSourceFlowConfigTypeDef):
     pass
 
 
+_RequiredTriggerConfigTypeDef = TypedDict(
+    "_RequiredTriggerConfigTypeDef",
+    {
+        "TriggerType": TriggerTypeType,
+    },
+)
+_OptionalTriggerConfigTypeDef = TypedDict(
+    "_OptionalTriggerConfigTypeDef",
+    {
+        "TriggerProperties": TriggerPropertiesTypeDef,
+    },
+    total=False,
+)
+
+
+class TriggerConfigTypeDef(_RequiredTriggerConfigTypeDef, _OptionalTriggerConfigTypeDef):
+    pass
+
+
 _RequiredCreateDomainRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDomainRequestRequestTypeDef",
     {
         "DomainName": str,
         "DefaultExpirationDays": int,
     },
 )
```

### Comparing `mypy-boto3-customer-profiles-1.28.15.post1/mypy_boto3_customer_profiles/type_defs.pyi` & `mypy-boto3-customer-profiles-1.28.16/mypy_boto3_customer_profiles/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_customer_profiles.type_defs import AddProfileKeyRequestRequestTypeDef
 
-    data: AddProfileKeyRequestRequestTypeDef = {...}
+    data: AddProfileKeyRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -54,24 +54,24 @@
     from typing_extensions import TypedDict
 
 __all__ = (
     "AddProfileKeyRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "AdditionalSearchKeyTypeDef",
     "AddressTypeDef",
-    "BatchTypeDef",
     "AppflowIntegrationWorkflowAttributesTypeDef",
     "AppflowIntegrationWorkflowMetricsTypeDef",
     "AppflowIntegrationWorkflowStepTypeDef",
     "AttributeItemTypeDef",
     "AttributeTypesSelectorOutputTypeDef",
     "AttributeTypesSelectorTypeDef",
     "ConflictResolutionTypeDef",
     "ConsolidationOutputTypeDef",
     "ConsolidationTypeDef",
+    "TimestampTypeDef",
     "RangeTypeDef",
     "ThresholdTypeDef",
     "ConnectorOperatorTypeDef",
     "CreateEventStreamRequestRequestTypeDef",
     "DeleteCalculatedAttributeDefinitionRequestRequestTypeDef",
     "DeleteDomainRequestRequestTypeDef",
     "DeleteEventStreamRequestRequestTypeDef",
@@ -123,23 +123,21 @@
     "ListProfileObjectTypeTemplatesRequestRequestTypeDef",
     "ListProfileObjectTypesRequestRequestTypeDef",
     "ListProfileObjectsItemTypeDef",
     "ObjectFilterTypeDef",
     "ListRuleBasedMatchesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListWorkflowsItemTypeDef",
-    "ListWorkflowsRequestRequestTypeDef",
     "MarketoSourcePropertiesTypeDef",
     "MatchingRuleOutputTypeDef",
     "MatchingRuleTypeDef",
     "ObjectTypeKeyTypeDef",
     "PutProfileObjectRequestRequestTypeDef",
     "S3SourcePropertiesTypeDef",
     "SalesforceSourcePropertiesTypeDef",
-    "ScheduledTriggerPropertiesTypeDef",
     "ServiceNowSourcePropertiesTypeDef",
     "ZendeskSourcePropertiesTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAddressTypeDef",
     "AddProfileKeyResponseTypeDef",
     "CreateEventStreamResponseTypeDef",
@@ -166,15 +164,19 @@
     "WorkflowAttributesTypeDef",
     "WorkflowMetricsTypeDef",
     "WorkflowStepItemTypeDef",
     "AttributeDetailsOutputTypeDef",
     "AttributeDetailsTypeDef",
     "AutoMergingOutputTypeDef",
     "AutoMergingTypeDef",
+    "ConsolidationUnionTypeDef",
     "GetAutoMergingPreviewRequestRequestTypeDef",
+    "BatchTypeDef",
+    "ListWorkflowsRequestRequestTypeDef",
+    "ScheduledTriggerPropertiesTypeDef",
     "ConditionsTypeDef",
     "TaskTypeDef",
     "EventStreamSummaryTypeDef",
     "GetEventStreamResponseTypeDef",
     "ExportingConfigTypeDef",
     "ExportingLocationTypeDef",
     "MergeProfilesRequestRequestTypeDef",
@@ -190,35 +192,37 @@
     "ListDomainsResponseTypeDef",
     "ListEventStreamsRequestListEventStreamsPaginateTypeDef",
     "ListProfileObjectTypesResponseTypeDef",
     "ListProfileObjectTypeTemplatesResponseTypeDef",
     "ListProfileObjectsResponseTypeDef",
     "ListProfileObjectsRequestRequestTypeDef",
     "ListWorkflowsResponseTypeDef",
-    "PutProfileObjectTypeRequestRequestTypeDef",
-    "TriggerPropertiesTypeDef",
+    "ObjectTypeKeyUnionTypeDef",
     "SourceConnectorPropertiesTypeDef",
     "UpdateProfileRequestRequestTypeDef",
     "GetWorkflowResponseTypeDef",
     "GetWorkflowStepsResponseTypeDef",
+    "AttributeDetailsUnionTypeDef",
+    "TriggerPropertiesTypeDef",
     "CreateCalculatedAttributeDefinitionRequestRequestTypeDef",
     "CreateCalculatedAttributeDefinitionResponseTypeDef",
     "GetCalculatedAttributeDefinitionResponseTypeDef",
     "UpdateCalculatedAttributeDefinitionRequestRequestTypeDef",
     "UpdateCalculatedAttributeDefinitionResponseTypeDef",
     "ListEventStreamsResponseTypeDef",
     "MatchingRequestTypeDef",
     "MatchingResponseTypeDef",
     "RuleBasedMatchingRequestTypeDef",
     "RuleBasedMatchingResponseTypeDef",
     "GetIdentityResolutionJobResponseTypeDef",
     "IdentityResolutionJobTypeDef",
     "SearchProfilesResponseTypeDef",
-    "TriggerConfigTypeDef",
+    "PutProfileObjectTypeRequestRequestTypeDef",
     "SourceFlowConfigTypeDef",
+    "TriggerConfigTypeDef",
     "CreateDomainRequestRequestTypeDef",
     "UpdateDomainRequestRequestTypeDef",
     "CreateDomainResponseTypeDef",
     "GetDomainResponseTypeDef",
     "UpdateDomainResponseTypeDef",
     "ListIdentityResolutionJobsResponseTypeDef",
     "FlowDefinitionTypeDef",
@@ -270,22 +274,14 @@
         "Province": str,
         "Country": str,
         "PostalCode": str,
     },
     total=False,
 )
 
-BatchTypeDef = TypedDict(
-    "BatchTypeDef",
-    {
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-    },
-)
-
 _RequiredAppflowIntegrationWorkflowAttributesTypeDef = TypedDict(
     "_RequiredAppflowIntegrationWorkflowAttributesTypeDef",
     {
         "SourceConnectorType": SourceConnectorTypeType,
         "ConnectorProfileName": str,
     },
 )
@@ -404,14 +400,15 @@
 ConsolidationTypeDef = TypedDict(
     "ConsolidationTypeDef",
     {
         "MatchingAttributesList": Sequence[Sequence[str]],
     },
 )
 
+TimestampTypeDef = Union[datetime, str]
 RangeTypeDef = TypedDict(
     "RangeTypeDef",
     {
         "Value": int,
         "Unit": Literal["DAYS"],
     },
 )
@@ -1171,38 +1168,14 @@
         "Status": StatusType,
         "StatusDescription": str,
         "CreatedAt": datetime,
         "LastUpdatedAt": datetime,
     },
 )
 
-_RequiredListWorkflowsRequestRequestTypeDef = TypedDict(
-    "_RequiredListWorkflowsRequestRequestTypeDef",
-    {
-        "DomainName": str,
-    },
-)
-_OptionalListWorkflowsRequestRequestTypeDef = TypedDict(
-    "_OptionalListWorkflowsRequestRequestTypeDef",
-    {
-        "WorkflowType": Literal["APPFLOW_INTEGRATION"],
-        "Status": StatusType,
-        "QueryStartDate": Union[datetime, str],
-        "QueryEndDate": Union[datetime, str],
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
-class ListWorkflowsRequestRequestTypeDef(
-    _RequiredListWorkflowsRequestRequestTypeDef, _OptionalListWorkflowsRequestRequestTypeDef
-):
-    pass
-
 MarketoSourcePropertiesTypeDef = TypedDict(
     "MarketoSourcePropertiesTypeDef",
     {
         "Object": str,
     },
 )
 
@@ -1273,38 +1246,14 @@
 )
 
 class SalesforceSourcePropertiesTypeDef(
     _RequiredSalesforceSourcePropertiesTypeDef, _OptionalSalesforceSourcePropertiesTypeDef
 ):
     pass
 
-_RequiredScheduledTriggerPropertiesTypeDef = TypedDict(
-    "_RequiredScheduledTriggerPropertiesTypeDef",
-    {
-        "ScheduleExpression": str,
-    },
-)
-_OptionalScheduledTriggerPropertiesTypeDef = TypedDict(
-    "_OptionalScheduledTriggerPropertiesTypeDef",
-    {
-        "DataPullMode": DataPullModeType,
-        "ScheduleStartTime": Union[datetime, str],
-        "ScheduleEndTime": Union[datetime, str],
-        "Timezone": str,
-        "ScheduleOffset": int,
-        "FirstExecutionFrom": Union[datetime, str],
-    },
-    total=False,
-)
-
-class ScheduledTriggerPropertiesTypeDef(
-    _RequiredScheduledTriggerPropertiesTypeDef, _OptionalScheduledTriggerPropertiesTypeDef
-):
-    pass
-
 ServiceNowSourcePropertiesTypeDef = TypedDict(
     "ServiceNowSourcePropertiesTypeDef",
     {
         "Object": str,
     },
 )
 
@@ -1680,14 +1629,15 @@
     },
     total=False,
 )
 
 class AutoMergingTypeDef(_RequiredAutoMergingTypeDef, _OptionalAutoMergingTypeDef):
     pass
 
+ConsolidationUnionTypeDef = Union[ConsolidationTypeDef, ConsolidationOutputTypeDef]
 _RequiredGetAutoMergingPreviewRequestRequestTypeDef = TypedDict(
     "_RequiredGetAutoMergingPreviewRequestRequestTypeDef",
     {
         "DomainName": str,
         "Consolidation": ConsolidationTypeDef,
         "ConflictResolution": ConflictResolutionTypeDef,
     },
@@ -1702,14 +1652,70 @@
 
 class GetAutoMergingPreviewRequestRequestTypeDef(
     _RequiredGetAutoMergingPreviewRequestRequestTypeDef,
     _OptionalGetAutoMergingPreviewRequestRequestTypeDef,
 ):
     pass
 
+BatchTypeDef = TypedDict(
+    "BatchTypeDef",
+    {
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+    },
+)
+
+_RequiredListWorkflowsRequestRequestTypeDef = TypedDict(
+    "_RequiredListWorkflowsRequestRequestTypeDef",
+    {
+        "DomainName": str,
+    },
+)
+_OptionalListWorkflowsRequestRequestTypeDef = TypedDict(
+    "_OptionalListWorkflowsRequestRequestTypeDef",
+    {
+        "WorkflowType": Literal["APPFLOW_INTEGRATION"],
+        "Status": StatusType,
+        "QueryStartDate": TimestampTypeDef,
+        "QueryEndDate": TimestampTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+class ListWorkflowsRequestRequestTypeDef(
+    _RequiredListWorkflowsRequestRequestTypeDef, _OptionalListWorkflowsRequestRequestTypeDef
+):
+    pass
+
+_RequiredScheduledTriggerPropertiesTypeDef = TypedDict(
+    "_RequiredScheduledTriggerPropertiesTypeDef",
+    {
+        "ScheduleExpression": str,
+    },
+)
+_OptionalScheduledTriggerPropertiesTypeDef = TypedDict(
+    "_OptionalScheduledTriggerPropertiesTypeDef",
+    {
+        "DataPullMode": DataPullModeType,
+        "ScheduleStartTime": TimestampTypeDef,
+        "ScheduleEndTime": TimestampTypeDef,
+        "Timezone": str,
+        "ScheduleOffset": int,
+        "FirstExecutionFrom": TimestampTypeDef,
+    },
+    total=False,
+)
+
+class ScheduledTriggerPropertiesTypeDef(
+    _RequiredScheduledTriggerPropertiesTypeDef, _OptionalScheduledTriggerPropertiesTypeDef
+):
+    pass
+
 ConditionsTypeDef = TypedDict(
     "ConditionsTypeDef",
     {
         "Range": RangeTypeDef,
         "ObjectCount": int,
         "Threshold": ThresholdTypeDef,
     },
@@ -2027,51 +2033,15 @@
     {
         "Items": List[ListWorkflowsItemTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredPutProfileObjectTypeRequestRequestTypeDef = TypedDict(
-    "_RequiredPutProfileObjectTypeRequestRequestTypeDef",
-    {
-        "DomainName": str,
-        "ObjectTypeName": str,
-        "Description": str,
-    },
-)
-_OptionalPutProfileObjectTypeRequestRequestTypeDef = TypedDict(
-    "_OptionalPutProfileObjectTypeRequestRequestTypeDef",
-    {
-        "TemplateId": str,
-        "ExpirationDays": int,
-        "EncryptionKey": str,
-        "AllowProfileCreation": bool,
-        "SourceLastUpdatedTimestampFormat": str,
-        "Fields": Mapping[str, ObjectTypeFieldTypeDef],
-        "Keys": Mapping[str, Sequence[Union[ObjectTypeKeyTypeDef, ObjectTypeKeyOutputTypeDef]]],
-        "Tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-class PutProfileObjectTypeRequestRequestTypeDef(
-    _RequiredPutProfileObjectTypeRequestRequestTypeDef,
-    _OptionalPutProfileObjectTypeRequestRequestTypeDef,
-):
-    pass
-
-TriggerPropertiesTypeDef = TypedDict(
-    "TriggerPropertiesTypeDef",
-    {
-        "Scheduled": ScheduledTriggerPropertiesTypeDef,
-    },
-    total=False,
-)
-
+ObjectTypeKeyUnionTypeDef = Union[ObjectTypeKeyTypeDef, ObjectTypeKeyOutputTypeDef]
 SourceConnectorPropertiesTypeDef = TypedDict(
     "SourceConnectorPropertiesTypeDef",
     {
         "Marketo": MarketoSourcePropertiesTypeDef,
         "S3": S3SourcePropertiesTypeDef,
         "Salesforce": SalesforceSourcePropertiesTypeDef,
         "ServiceNow": ServiceNowSourcePropertiesTypeDef,
@@ -2144,14 +2114,23 @@
         "WorkflowType": Literal["APPFLOW_INTEGRATION"],
         "Items": List[WorkflowStepItemTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+AttributeDetailsUnionTypeDef = Union[AttributeDetailsTypeDef, AttributeDetailsOutputTypeDef]
+TriggerPropertiesTypeDef = TypedDict(
+    "TriggerPropertiesTypeDef",
+    {
+        "Scheduled": ScheduledTriggerPropertiesTypeDef,
+    },
+    total=False,
+)
+
 _RequiredCreateCalculatedAttributeDefinitionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCalculatedAttributeDefinitionRequestRequestTypeDef",
     {
         "DomainName": str,
         "CalculatedAttributeName": str,
         "AttributeDetails": AttributeDetailsTypeDef,
         "Statistic": StatisticType,
@@ -2361,29 +2340,41 @@
     {
         "Items": List[ProfileTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredTriggerConfigTypeDef = TypedDict(
-    "_RequiredTriggerConfigTypeDef",
+_RequiredPutProfileObjectTypeRequestRequestTypeDef = TypedDict(
+    "_RequiredPutProfileObjectTypeRequestRequestTypeDef",
     {
-        "TriggerType": TriggerTypeType,
+        "DomainName": str,
+        "ObjectTypeName": str,
+        "Description": str,
     },
 )
-_OptionalTriggerConfigTypeDef = TypedDict(
-    "_OptionalTriggerConfigTypeDef",
+_OptionalPutProfileObjectTypeRequestRequestTypeDef = TypedDict(
+    "_OptionalPutProfileObjectTypeRequestRequestTypeDef",
     {
-        "TriggerProperties": TriggerPropertiesTypeDef,
+        "TemplateId": str,
+        "ExpirationDays": int,
+        "EncryptionKey": str,
+        "AllowProfileCreation": bool,
+        "SourceLastUpdatedTimestampFormat": str,
+        "Fields": Mapping[str, ObjectTypeFieldTypeDef],
+        "Keys": Mapping[str, Sequence[ObjectTypeKeyUnionTypeDef]],
+        "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-class TriggerConfigTypeDef(_RequiredTriggerConfigTypeDef, _OptionalTriggerConfigTypeDef):
+class PutProfileObjectTypeRequestRequestTypeDef(
+    _RequiredPutProfileObjectTypeRequestRequestTypeDef,
+    _OptionalPutProfileObjectTypeRequestRequestTypeDef,
+):
     pass
 
 _RequiredSourceFlowConfigTypeDef = TypedDict(
     "_RequiredSourceFlowConfigTypeDef",
     {
         "ConnectorType": SourceConnectorTypeType,
         "SourceConnectorProperties": SourceConnectorPropertiesTypeDef,
@@ -2397,14 +2388,31 @@
     },
     total=False,
 )
 
 class SourceFlowConfigTypeDef(_RequiredSourceFlowConfigTypeDef, _OptionalSourceFlowConfigTypeDef):
     pass
 
+_RequiredTriggerConfigTypeDef = TypedDict(
+    "_RequiredTriggerConfigTypeDef",
+    {
+        "TriggerType": TriggerTypeType,
+    },
+)
+_OptionalTriggerConfigTypeDef = TypedDict(
+    "_OptionalTriggerConfigTypeDef",
+    {
+        "TriggerProperties": TriggerPropertiesTypeDef,
+    },
+    total=False,
+)
+
+class TriggerConfigTypeDef(_RequiredTriggerConfigTypeDef, _OptionalTriggerConfigTypeDef):
+    pass
+
 _RequiredCreateDomainRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDomainRequestRequestTypeDef",
     {
         "DomainName": str,
         "DefaultExpirationDays": int,
     },
 )
```

### Comparing `mypy-boto3-customer-profiles-1.28.15.post1/mypy_boto3_customer_profiles.egg-info/PKG-INFO` & `mypy-boto3-customer-profiles-1.28.16/mypy_boto3_customer_profiles.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-customer-profiles
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.CustomerProfiles 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.CustomerProfiles 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 customer-profiles type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 customer-profiles type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-customer-profiles.svg?color=blue)](https://pypi.org/project/mypy-boto3-customer-profiles)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-customer-profiles)](https://pepy.tech/project/mypy-boto3-customer-profiles)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CustomerProfiles 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles)
+[boto3.CustomerProfiles 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles)
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
 [mypy-boto3-customer-profiles docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/).
 
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
@@ -339,37 +339,37 @@
 )
 
 
 def check_value(value: AttributeMatchingModelType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_customer_profiles.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_customer_profiles.type_defs import (
     AddProfileKeyRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     AdditionalSearchKeyTypeDef,
     AddressTypeDef,
-    BatchTypeDef,
     AppflowIntegrationWorkflowAttributesTypeDef,
     AppflowIntegrationWorkflowMetricsTypeDef,
     AppflowIntegrationWorkflowStepTypeDef,
     AttributeItemTypeDef,
     AttributeTypesSelectorOutputTypeDef,
     AttributeTypesSelectorTypeDef,
     ConflictResolutionTypeDef,
     ConsolidationOutputTypeDef,
     ConsolidationTypeDef,
+    TimestampTypeDef,
     RangeTypeDef,
     ThresholdTypeDef,
     ConnectorOperatorTypeDef,
     CreateEventStreamRequestRequestTypeDef,
     DeleteCalculatedAttributeDefinitionRequestRequestTypeDef,
     DeleteDomainRequestRequestTypeDef,
     DeleteEventStreamRequestRequestTypeDef,
@@ -421,23 +421,21 @@
     ListProfileObjectTypeTemplatesRequestRequestTypeDef,
     ListProfileObjectTypesRequestRequestTypeDef,
     ListProfileObjectsItemTypeDef,
     ObjectFilterTypeDef,
     ListRuleBasedMatchesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListWorkflowsItemTypeDef,
-    ListWorkflowsRequestRequestTypeDef,
     MarketoSourcePropertiesTypeDef,
     MatchingRuleOutputTypeDef,
     MatchingRuleTypeDef,
     ObjectTypeKeyTypeDef,
     PutProfileObjectRequestRequestTypeDef,
     S3SourcePropertiesTypeDef,
     SalesforceSourcePropertiesTypeDef,
-    ScheduledTriggerPropertiesTypeDef,
     ServiceNowSourcePropertiesTypeDef,
     ZendeskSourcePropertiesTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAddressTypeDef,
     AddProfileKeyResponseTypeDef,
     CreateEventStreamResponseTypeDef,
@@ -464,15 +462,19 @@
     WorkflowAttributesTypeDef,
     WorkflowMetricsTypeDef,
     WorkflowStepItemTypeDef,
     AttributeDetailsOutputTypeDef,
     AttributeDetailsTypeDef,
     AutoMergingOutputTypeDef,
     AutoMergingTypeDef,
+    ConsolidationUnionTypeDef,
     GetAutoMergingPreviewRequestRequestTypeDef,
+    BatchTypeDef,
+    ListWorkflowsRequestRequestTypeDef,
+    ScheduledTriggerPropertiesTypeDef,
     ConditionsTypeDef,
     TaskTypeDef,
     EventStreamSummaryTypeDef,
     GetEventStreamResponseTypeDef,
     ExportingConfigTypeDef,
     ExportingLocationTypeDef,
     MergeProfilesRequestRequestTypeDef,
@@ -488,50 +490,52 @@
     ListDomainsResponseTypeDef,
     ListEventStreamsRequestListEventStreamsPaginateTypeDef,
     ListProfileObjectTypesResponseTypeDef,
     ListProfileObjectTypeTemplatesResponseTypeDef,
     ListProfileObjectsResponseTypeDef,
     ListProfileObjectsRequestRequestTypeDef,
     ListWorkflowsResponseTypeDef,
-    PutProfileObjectTypeRequestRequestTypeDef,
-    TriggerPropertiesTypeDef,
+    ObjectTypeKeyUnionTypeDef,
     SourceConnectorPropertiesTypeDef,
     UpdateProfileRequestRequestTypeDef,
     GetWorkflowResponseTypeDef,
     GetWorkflowStepsResponseTypeDef,
+    AttributeDetailsUnionTypeDef,
+    TriggerPropertiesTypeDef,
     CreateCalculatedAttributeDefinitionRequestRequestTypeDef,
     CreateCalculatedAttributeDefinitionResponseTypeDef,
     GetCalculatedAttributeDefinitionResponseTypeDef,
     UpdateCalculatedAttributeDefinitionRequestRequestTypeDef,
     UpdateCalculatedAttributeDefinitionResponseTypeDef,
     ListEventStreamsResponseTypeDef,
     MatchingRequestTypeDef,
     MatchingResponseTypeDef,
     RuleBasedMatchingRequestTypeDef,
     RuleBasedMatchingResponseTypeDef,
     GetIdentityResolutionJobResponseTypeDef,
     IdentityResolutionJobTypeDef,
     SearchProfilesResponseTypeDef,
-    TriggerConfigTypeDef,
+    PutProfileObjectTypeRequestRequestTypeDef,
     SourceFlowConfigTypeDef,
+    TriggerConfigTypeDef,
     CreateDomainRequestRequestTypeDef,
     UpdateDomainRequestRequestTypeDef,
     CreateDomainResponseTypeDef,
     GetDomainResponseTypeDef,
     UpdateDomainResponseTypeDef,
     ListIdentityResolutionJobsResponseTypeDef,
     FlowDefinitionTypeDef,
     AppflowIntegrationTypeDef,
     PutIntegrationRequestRequestTypeDef,
     IntegrationConfigTypeDef,
     CreateIntegrationWorkflowRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AddProfileKeyRequestRequestTypeDef:
+def get_value() -> AddProfileKeyRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-customer-profiles-1.28.15.post1/mypy_boto3_customer_profiles.egg-info/SOURCES.txt` & `mypy-boto3-customer-profiles-1.28.16/mypy_boto3_customer_profiles.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-customer-profiles-1.28.15.post1/setup.py` & `mypy-boto3-customer-profiles-1.28.16/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-customer-profiles",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_customer_profiles"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CustomerProfiles 1.28.15 service generated with"
-        " mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.CustomerProfiles 1.28.16 service generated with"
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
-    keywords="boto3 customer-profiles type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 customer-profiles type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_customer_profiles": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

