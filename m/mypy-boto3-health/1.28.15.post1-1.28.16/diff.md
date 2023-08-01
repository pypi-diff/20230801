# Comparing `tmp/mypy-boto3-health-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-health-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-health-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:14 2023, max compression
+gzip compressed data, was "mypy-boto3-health-1.28.16.tar", last modified: Tue Aug  1 11:36:55 2023, max compression
```

## Comparing `mypy-boto3-health-1.28.15.post1.tar` & `mypy-boto3-health-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:14.885172 mypy-boto3-health-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:46:49.000000 mypy-boto3-health-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16273 2023-07-29 10:03:14.885172 mypy-boto3-health-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14784 2023-07-29 09:46:49.000000 mypy-boto3-health-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:14.877172 mypy-boto3-health-1.28.15.post1/mypy_boto3_health/
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-07-29 09:46:49.000000 mypy-boto3-health-1.28.15.post1/mypy_boto3_health/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-07-29 09:46:49.000000 mypy-boto3-health-1.28.15.post1/mypy_boto3_health/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-29 09:46:49.000000 mypy-boto3-health-1.28.15.post1/mypy_boto3_health/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15699 2023-07-29 09:46:49.000000 mypy-boto3-health-1.28.15.post1/mypy_boto3_health/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15672 2023-07-29 09:46:49.000000 mypy-boto3-health-1.28.15.post1/mypy_boto3_health/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9475 2023-07-29 09:46:52.000000 mypy-boto3-health-1.28.15.post1/mypy_boto3_health/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9473 2023-07-29 09:46:51.000000 mypy-boto3-health-1.28.15.post1/mypy_boto3_health/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9810 2023-07-29 09:46:49.000000 mypy-boto3-health-1.28.15.post1/mypy_boto3_health/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9800 2023-07-29 09:46:49.000000 mypy-boto3-health-1.28.15.post1/mypy_boto3_health/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:46:49.000000 mypy-boto3-health-1.28.15.post1/mypy_boto3_health/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    21615 2023-07-29 09:46:52.000000 mypy-boto3-health-1.28.15.post1/mypy_boto3_health/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    21590 2023-07-29 09:46:52.000000 mypy-boto3-health-1.28.15.post1/mypy_boto3_health/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:46:49.000000 mypy-boto3-health-1.28.15.post1/mypy_boto3_health/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:14.885172 mypy-boto3-health-1.28.15.post1/mypy_boto3_health.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16273 2023-07-29 10:03:14.000000 mypy-boto3-health-1.28.15.post1/mypy_boto3_health.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-29 10:03:14.000000 mypy-boto3-health-1.28.15.post1/mypy_boto3_health.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:14.000000 mypy-boto3-health-1.28.15.post1/mypy_boto3_health.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:14.000000 mypy-boto3-health-1.28.15.post1/mypy_boto3_health.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:14.000000 mypy-boto3-health-1.28.15.post1/mypy_boto3_health.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-29 10:03:14.000000 mypy-boto3-health-1.28.15.post1/mypy_boto3_health.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:14.885172 mypy-boto3-health-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-29 09:46:49.000000 mypy-boto3-health-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:55.480875 mypy-boto3-health-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:19:29.000000 mypy-boto3-health-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16285 2023-08-01 11:36:55.480875 mypy-boto3-health-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14805 2023-08-01 11:19:29.000000 mypy-boto3-health-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:55.468875 mypy-boto3-health-1.28.16/mypy_boto3_health/
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-08-01 11:19:29.000000 mypy-boto3-health-1.28.16/mypy_boto3_health/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-08-01 11:19:29.000000 mypy-boto3-health-1.28.16/mypy_boto3_health/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-08-01 11:19:29.000000 mypy-boto3-health-1.28.16/mypy_boto3_health/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15699 2023-08-01 11:19:30.000000 mypy-boto3-health-1.28.16/mypy_boto3_health/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15672 2023-08-01 11:19:29.000000 mypy-boto3-health-1.28.16/mypy_boto3_health/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9475 2023-08-01 11:19:30.000000 mypy-boto3-health-1.28.16/mypy_boto3_health/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9473 2023-08-01 11:19:30.000000 mypy-boto3-health-1.28.16/mypy_boto3_health/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9810 2023-08-01 11:19:30.000000 mypy-boto3-health-1.28.16/mypy_boto3_health/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9800 2023-08-01 11:19:30.000000 mypy-boto3-health-1.28.16/mypy_boto3_health/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:19:29.000000 mypy-boto3-health-1.28.16/mypy_boto3_health/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    21669 2023-08-01 11:19:30.000000 mypy-boto3-health-1.28.16/mypy_boto3_health/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21644 2023-08-01 11:19:30.000000 mypy-boto3-health-1.28.16/mypy_boto3_health/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:19:29.000000 mypy-boto3-health-1.28.16/mypy_boto3_health/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:55.480875 mypy-boto3-health-1.28.16/mypy_boto3_health.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16285 2023-08-01 11:36:55.000000 mypy-boto3-health-1.28.16/mypy_boto3_health.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-08-01 11:36:55.000000 mypy-boto3-health-1.28.16/mypy_boto3_health.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:55.000000 mypy-boto3-health-1.28.16/mypy_boto3_health.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:55.000000 mypy-boto3-health-1.28.16/mypy_boto3_health.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:55.000000 mypy-boto3-health-1.28.16/mypy_boto3_health.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-01 11:36:55.000000 mypy-boto3-health-1.28.16/mypy_boto3_health.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:55.480875 mypy-boto3-health-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-08-01 11:19:29.000000 mypy-boto3-health-1.28.16/setup.py
```

### Comparing `mypy-boto3-health-1.28.15.post1/LICENSE` & `mypy-boto3-health-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-health-1.28.15.post1/PKG-INFO` & `mypy-boto3-health-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-health
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.Health 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.Health 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_health/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 health type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 health type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-health.svg?color=blue)](https://pypi.org/project/mypy-boto3-health)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_health/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-health)](https://pepy.tech/project/mypy-boto3-health)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Health 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health)
+[boto3.Health 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health)
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
 [mypy-boto3-health docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_health/).
 
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
@@ -346,25 +346,25 @@
 )
 
 
 def check_value(value: DescribeAffectedAccountsForOrganizationPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_health.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_health.type_defs import (
     AffectedEntityTypeDef,
-    DateTimeRangeTypeDef,
+    TimestampTypeDef,
     PaginatorConfigTypeDef,
     DescribeAffectedAccountsForOrganizationRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     EventAccountFilterTypeDef,
     OrganizationAffectedEntitiesErrorItemTypeDef,
     DescribeEntityAggregatesRequestRequestTypeDef,
     EntityAggregateTypeDef,
@@ -373,17 +373,15 @@
     DescribeEventDetailsRequestRequestTypeDef,
     EventDetailsErrorItemTypeDef,
     EventTypeFilterTypeDef,
     EventTypeTypeDef,
     OrganizationEventTypeDef,
     EventTypeDef,
     EventDescriptionTypeDef,
-    EntityFilterTypeDef,
-    EventFilterTypeDef,
-    OrganizationEventFilterTypeDef,
+    DateTimeRangeTypeDef,
     DescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef,
     DescribeAffectedAccountsForOrganizationResponseTypeDef,
     DescribeAffectedEntitiesResponseTypeDef,
     DescribeHealthServiceStatusForOrganizationResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     DescribeAffectedEntitiesForOrganizationRequestDescribeAffectedEntitiesForOrganizationPaginateTypeDef,
     DescribeAffectedEntitiesForOrganizationRequestRequestTypeDef,
@@ -394,28 +392,31 @@
     DescribeEventTypesRequestDescribeEventTypesPaginateTypeDef,
     DescribeEventTypesRequestRequestTypeDef,
     DescribeEventTypesResponseTypeDef,
     DescribeEventsForOrganizationResponseTypeDef,
     DescribeEventsResponseTypeDef,
     EventDetailsTypeDef,
     OrganizationEventDetailsTypeDef,
+    EntityFilterTypeDef,
+    EventFilterTypeDef,
+    OrganizationEventFilterTypeDef,
+    DescribeEventDetailsResponseTypeDef,
+    DescribeEventDetailsForOrganizationResponseTypeDef,
     DescribeAffectedEntitiesRequestDescribeAffectedEntitiesPaginateTypeDef,
     DescribeAffectedEntitiesRequestRequestTypeDef,
     DescribeEventAggregatesRequestDescribeEventAggregatesPaginateTypeDef,
     DescribeEventAggregatesRequestRequestTypeDef,
     DescribeEventsRequestDescribeEventsPaginateTypeDef,
     DescribeEventsRequestRequestTypeDef,
     DescribeEventsForOrganizationRequestDescribeEventsForOrganizationPaginateTypeDef,
     DescribeEventsForOrganizationRequestRequestTypeDef,
-    DescribeEventDetailsResponseTypeDef,
-    DescribeEventDetailsForOrganizationResponseTypeDef,
 )
 
 
-def get_structure() -> AffectedEntityTypeDef:
+def get_value() -> AffectedEntityTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-health-1.28.15.post1/README.md` & `mypy-boto3-health-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-health.svg?color=blue)](https://pypi.org/project/mypy-boto3-health)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_health/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-health)](https://pepy.tech/project/mypy-boto3-health)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Health 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health)
+[boto3.Health 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health)
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
 [mypy-boto3-health docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_health/).
 
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
@@ -314,25 +314,25 @@
 )
 
 
 def check_value(value: DescribeAffectedAccountsForOrganizationPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_health.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_health.type_defs import (
     AffectedEntityTypeDef,
-    DateTimeRangeTypeDef,
+    TimestampTypeDef,
     PaginatorConfigTypeDef,
     DescribeAffectedAccountsForOrganizationRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     EventAccountFilterTypeDef,
     OrganizationAffectedEntitiesErrorItemTypeDef,
     DescribeEntityAggregatesRequestRequestTypeDef,
     EntityAggregateTypeDef,
@@ -341,17 +341,15 @@
     DescribeEventDetailsRequestRequestTypeDef,
     EventDetailsErrorItemTypeDef,
     EventTypeFilterTypeDef,
     EventTypeTypeDef,
     OrganizationEventTypeDef,
     EventTypeDef,
     EventDescriptionTypeDef,
-    EntityFilterTypeDef,
-    EventFilterTypeDef,
-    OrganizationEventFilterTypeDef,
+    DateTimeRangeTypeDef,
     DescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef,
     DescribeAffectedAccountsForOrganizationResponseTypeDef,
     DescribeAffectedEntitiesResponseTypeDef,
     DescribeHealthServiceStatusForOrganizationResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     DescribeAffectedEntitiesForOrganizationRequestDescribeAffectedEntitiesForOrganizationPaginateTypeDef,
     DescribeAffectedEntitiesForOrganizationRequestRequestTypeDef,
@@ -362,28 +360,31 @@
     DescribeEventTypesRequestDescribeEventTypesPaginateTypeDef,
     DescribeEventTypesRequestRequestTypeDef,
     DescribeEventTypesResponseTypeDef,
     DescribeEventsForOrganizationResponseTypeDef,
     DescribeEventsResponseTypeDef,
     EventDetailsTypeDef,
     OrganizationEventDetailsTypeDef,
+    EntityFilterTypeDef,
+    EventFilterTypeDef,
+    OrganizationEventFilterTypeDef,
+    DescribeEventDetailsResponseTypeDef,
+    DescribeEventDetailsForOrganizationResponseTypeDef,
     DescribeAffectedEntitiesRequestDescribeAffectedEntitiesPaginateTypeDef,
     DescribeAffectedEntitiesRequestRequestTypeDef,
     DescribeEventAggregatesRequestDescribeEventAggregatesPaginateTypeDef,
     DescribeEventAggregatesRequestRequestTypeDef,
     DescribeEventsRequestDescribeEventsPaginateTypeDef,
     DescribeEventsRequestRequestTypeDef,
     DescribeEventsForOrganizationRequestDescribeEventsForOrganizationPaginateTypeDef,
     DescribeEventsForOrganizationRequestRequestTypeDef,
-    DescribeEventDetailsResponseTypeDef,
-    DescribeEventDetailsForOrganizationResponseTypeDef,
 )
 
 
-def get_structure() -> AffectedEntityTypeDef:
+def get_value() -> AffectedEntityTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-health-1.28.15.post1/mypy_boto3_health/__init__.py` & `mypy-boto3-health-1.28.16/mypy_boto3_health/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-health-1.28.15.post1/mypy_boto3_health/__init__.pyi` & `mypy-boto3-health-1.28.16/mypy_boto3_health/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-health-1.28.15.post1/mypy_boto3_health/__main__.py` & `mypy-boto3-health-1.28.16/mypy_boto3_health/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Health 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.Health 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_health//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health\nOther"
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

### Comparing `mypy-boto3-health-1.28.15.post1/mypy_boto3_health/client.py` & `mypy-boto3-health-1.28.16/mypy_boto3_health/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-health-1.28.15.post1/mypy_boto3_health/client.pyi` & `mypy-boto3-health-1.28.16/mypy_boto3_health/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-health-1.28.15.post1/mypy_boto3_health/literals.py` & `mypy-boto3-health-1.28.16/mypy_boto3_health/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-health-1.28.15.post1/mypy_boto3_health/literals.pyi` & `mypy-boto3-health-1.28.16/mypy_boto3_health/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-health-1.28.15.post1/mypy_boto3_health/paginator.py` & `mypy-boto3-health-1.28.16/mypy_boto3_health/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-health-1.28.15.post1/mypy_boto3_health/paginator.pyi` & `mypy-boto3-health-1.28.16/mypy_boto3_health/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-health-1.28.15.post1/mypy_boto3_health/type_defs.py` & `mypy-boto3-health-1.28.16/mypy_boto3_health/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_health/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_health.type_defs import AffectedEntityTypeDef
 
-    data: AffectedEntityTypeDef = {...}
+    data: AffectedEntityTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -27,18 +27,17 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AffectedEntityTypeDef",
-    "DateTimeRangeTypeDef",
+    "TimestampTypeDef",
     "PaginatorConfigTypeDef",
     "DescribeAffectedAccountsForOrganizationRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "EventAccountFilterTypeDef",
     "OrganizationAffectedEntitiesErrorItemTypeDef",
     "DescribeEntityAggregatesRequestRequestTypeDef",
     "EntityAggregateTypeDef",
@@ -47,17 +46,15 @@
     "DescribeEventDetailsRequestRequestTypeDef",
     "EventDetailsErrorItemTypeDef",
     "EventTypeFilterTypeDef",
     "EventTypeTypeDef",
     "OrganizationEventTypeDef",
     "EventTypeDef",
     "EventDescriptionTypeDef",
-    "EntityFilterTypeDef",
-    "EventFilterTypeDef",
-    "OrganizationEventFilterTypeDef",
+    "DateTimeRangeTypeDef",
     "DescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef",
     "DescribeAffectedAccountsForOrganizationResponseTypeDef",
     "DescribeAffectedEntitiesResponseTypeDef",
     "DescribeHealthServiceStatusForOrganizationResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "DescribeAffectedEntitiesForOrganizationRequestDescribeAffectedEntitiesForOrganizationPaginateTypeDef",
     "DescribeAffectedEntitiesForOrganizationRequestRequestTypeDef",
@@ -68,24 +65,27 @@
     "DescribeEventTypesRequestDescribeEventTypesPaginateTypeDef",
     "DescribeEventTypesRequestRequestTypeDef",
     "DescribeEventTypesResponseTypeDef",
     "DescribeEventsForOrganizationResponseTypeDef",
     "DescribeEventsResponseTypeDef",
     "EventDetailsTypeDef",
     "OrganizationEventDetailsTypeDef",
+    "EntityFilterTypeDef",
+    "EventFilterTypeDef",
+    "OrganizationEventFilterTypeDef",
+    "DescribeEventDetailsResponseTypeDef",
+    "DescribeEventDetailsForOrganizationResponseTypeDef",
     "DescribeAffectedEntitiesRequestDescribeAffectedEntitiesPaginateTypeDef",
     "DescribeAffectedEntitiesRequestRequestTypeDef",
     "DescribeEventAggregatesRequestDescribeEventAggregatesPaginateTypeDef",
     "DescribeEventAggregatesRequestRequestTypeDef",
     "DescribeEventsRequestDescribeEventsPaginateTypeDef",
     "DescribeEventsRequestRequestTypeDef",
     "DescribeEventsForOrganizationRequestDescribeEventsForOrganizationPaginateTypeDef",
     "DescribeEventsForOrganizationRequestRequestTypeDef",
-    "DescribeEventDetailsResponseTypeDef",
-    "DescribeEventDetailsForOrganizationResponseTypeDef",
 )
 
 AffectedEntityTypeDef = TypedDict(
     "AffectedEntityTypeDef",
     {
         "entityArn": str,
         "eventArn": str,
@@ -95,23 +95,15 @@
         "lastUpdatedTime": datetime,
         "statusCode": entityStatusCodeType,
         "tags": Dict[str, str],
     },
     total=False,
 )
 
-DateTimeRangeTypeDef = TypedDict(
-    "DateTimeRangeTypeDef",
-    {
-        "from": Union[datetime, str],
-        "to": Union[datetime, str],
-    },
-    total=False,
-)
-
+TimestampTypeDef = Union[datetime, str]
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
@@ -129,22 +121,20 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class DescribeAffectedAccountsForOrganizationRequestRequestTypeDef(
     _RequiredDescribeAffectedAccountsForOrganizationRequestRequestTypeDef,
     _OptionalDescribeAffectedAccountsForOrganizationRequestRequestTypeDef,
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
@@ -162,21 +152,19 @@
     "_OptionalEventAccountFilterTypeDef",
     {
         "awsAccountId": str,
     },
     total=False,
 )
 
-
 class EventAccountFilterTypeDef(
     _RequiredEventAccountFilterTypeDef, _OptionalEventAccountFilterTypeDef
 ):
     pass
 
-
 OrganizationAffectedEntitiesErrorItemTypeDef = TypedDict(
     "OrganizationAffectedEntitiesErrorItemTypeDef",
     {
         "awsAccountId": str,
         "eventArn": str,
         "errorName": str,
         "errorMessage": str,
@@ -231,22 +219,20 @@
     "_OptionalDescribeEventDetailsRequestRequestTypeDef",
     {
         "locale": str,
     },
     total=False,
 )
 
-
 class DescribeEventDetailsRequestRequestTypeDef(
     _RequiredDescribeEventDetailsRequestRequestTypeDef,
     _OptionalDescribeEventDetailsRequestRequestTypeDef,
 ):
     pass
 
-
 EventDetailsErrorItemTypeDef = TypedDict(
     "EventDetailsErrorItemTypeDef",
     {
         "eventArn": str,
         "errorName": str,
         "errorMessage": str,
     },
@@ -312,71 +298,19 @@
     "EventDescriptionTypeDef",
     {
         "latestDescription": str,
     },
     total=False,
 )
 
-_RequiredEntityFilterTypeDef = TypedDict(
-    "_RequiredEntityFilterTypeDef",
-    {
-        "eventArns": Sequence[str],
-    },
-)
-_OptionalEntityFilterTypeDef = TypedDict(
-    "_OptionalEntityFilterTypeDef",
-    {
-        "entityArns": Sequence[str],
-        "entityValues": Sequence[str],
-        "lastUpdatedTimes": Sequence[DateTimeRangeTypeDef],
-        "tags": Sequence[Mapping[str, str]],
-        "statusCodes": Sequence[entityStatusCodeType],
-    },
-    total=False,
-)
-
-
-class EntityFilterTypeDef(_RequiredEntityFilterTypeDef, _OptionalEntityFilterTypeDef):
-    pass
-
-
-EventFilterTypeDef = TypedDict(
-    "EventFilterTypeDef",
-    {
-        "eventArns": Sequence[str],
-        "eventTypeCodes": Sequence[str],
-        "services": Sequence[str],
-        "regions": Sequence[str],
-        "availabilityZones": Sequence[str],
-        "startTimes": Sequence[DateTimeRangeTypeDef],
-        "endTimes": Sequence[DateTimeRangeTypeDef],
-        "lastUpdatedTimes": Sequence[DateTimeRangeTypeDef],
-        "entityArns": Sequence[str],
-        "entityValues": Sequence[str],
-        "eventTypeCategories": Sequence[eventTypeCategoryType],
-        "tags": Sequence[Mapping[str, str]],
-        "eventStatusCodes": Sequence[eventStatusCodeType],
-    },
-    total=False,
-)
-
-OrganizationEventFilterTypeDef = TypedDict(
-    "OrganizationEventFilterTypeDef",
+DateTimeRangeTypeDef = TypedDict(
+    "DateTimeRangeTypeDef",
     {
-        "eventTypeCodes": Sequence[str],
-        "awsAccountIds": Sequence[str],
-        "services": Sequence[str],
-        "regions": Sequence[str],
-        "startTime": DateTimeRangeTypeDef,
-        "endTime": DateTimeRangeTypeDef,
-        "lastUpdatedTime": DateTimeRangeTypeDef,
-        "entityArns": Sequence[str],
-        "entityValues": Sequence[str],
-        "eventTypeCategories": Sequence[eventTypeCategoryType],
-        "eventStatusCodes": Sequence[eventStatusCodeType],
+        "from": TimestampTypeDef,
+        "to": TimestampTypeDef,
     },
     total=False,
 )
 
 _RequiredDescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef = TypedDict(
     "_RequiredDescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef",
     {
@@ -387,22 +321,20 @@
     "_OptionalDescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef(
     _RequiredDescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef,
     _OptionalDescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef,
 ):
     pass
 
-
 DescribeAffectedAccountsForOrganizationResponseTypeDef = TypedDict(
     "DescribeAffectedAccountsForOrganizationResponseTypeDef",
     {
         "affectedAccounts": List[str],
         "eventScopeCode": eventScopeCodeType,
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -444,22 +376,20 @@
     {
         "locale": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeAffectedEntitiesForOrganizationRequestDescribeAffectedEntitiesForOrganizationPaginateTypeDef(
     _RequiredDescribeAffectedEntitiesForOrganizationRequestDescribeAffectedEntitiesForOrganizationPaginateTypeDef,
     _OptionalDescribeAffectedEntitiesForOrganizationRequestDescribeAffectedEntitiesForOrganizationPaginateTypeDef,
 ):
     pass
 
-
 _RequiredDescribeAffectedEntitiesForOrganizationRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeAffectedEntitiesForOrganizationRequestRequestTypeDef",
     {
         "organizationEntityFilters": Sequence[EventAccountFilterTypeDef],
     },
 )
 _OptionalDescribeAffectedEntitiesForOrganizationRequestRequestTypeDef = TypedDict(
@@ -468,44 +398,40 @@
         "locale": str,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class DescribeAffectedEntitiesForOrganizationRequestRequestTypeDef(
     _RequiredDescribeAffectedEntitiesForOrganizationRequestRequestTypeDef,
     _OptionalDescribeAffectedEntitiesForOrganizationRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDescribeEventDetailsForOrganizationRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeEventDetailsForOrganizationRequestRequestTypeDef",
     {
         "organizationEventDetailFilters": Sequence[EventAccountFilterTypeDef],
     },
 )
 _OptionalDescribeEventDetailsForOrganizationRequestRequestTypeDef = TypedDict(
     "_OptionalDescribeEventDetailsForOrganizationRequestRequestTypeDef",
     {
         "locale": str,
     },
     total=False,
 )
 
-
 class DescribeEventDetailsForOrganizationRequestRequestTypeDef(
     _RequiredDescribeEventDetailsForOrganizationRequestRequestTypeDef,
     _OptionalDescribeEventDetailsForOrganizationRequestRequestTypeDef,
 ):
     pass
 
-
 DescribeAffectedEntitiesForOrganizationResponseTypeDef = TypedDict(
     "DescribeAffectedEntitiesForOrganizationResponseTypeDef",
     {
         "entities": List[AffectedEntityTypeDef],
         "failedSet": List[OrganizationAffectedEntitiesErrorItemTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -594,14 +520,91 @@
         "event": EventTypeDef,
         "eventDescription": EventDescriptionTypeDef,
         "eventMetadata": Dict[str, str],
     },
     total=False,
 )
 
+_RequiredEntityFilterTypeDef = TypedDict(
+    "_RequiredEntityFilterTypeDef",
+    {
+        "eventArns": Sequence[str],
+    },
+)
+_OptionalEntityFilterTypeDef = TypedDict(
+    "_OptionalEntityFilterTypeDef",
+    {
+        "entityArns": Sequence[str],
+        "entityValues": Sequence[str],
+        "lastUpdatedTimes": Sequence[DateTimeRangeTypeDef],
+        "tags": Sequence[Mapping[str, str]],
+        "statusCodes": Sequence[entityStatusCodeType],
+    },
+    total=False,
+)
+
+class EntityFilterTypeDef(_RequiredEntityFilterTypeDef, _OptionalEntityFilterTypeDef):
+    pass
+
+EventFilterTypeDef = TypedDict(
+    "EventFilterTypeDef",
+    {
+        "eventArns": Sequence[str],
+        "eventTypeCodes": Sequence[str],
+        "services": Sequence[str],
+        "regions": Sequence[str],
+        "availabilityZones": Sequence[str],
+        "startTimes": Sequence[DateTimeRangeTypeDef],
+        "endTimes": Sequence[DateTimeRangeTypeDef],
+        "lastUpdatedTimes": Sequence[DateTimeRangeTypeDef],
+        "entityArns": Sequence[str],
+        "entityValues": Sequence[str],
+        "eventTypeCategories": Sequence[eventTypeCategoryType],
+        "tags": Sequence[Mapping[str, str]],
+        "eventStatusCodes": Sequence[eventStatusCodeType],
+    },
+    total=False,
+)
+
+OrganizationEventFilterTypeDef = TypedDict(
+    "OrganizationEventFilterTypeDef",
+    {
+        "eventTypeCodes": Sequence[str],
+        "awsAccountIds": Sequence[str],
+        "services": Sequence[str],
+        "regions": Sequence[str],
+        "startTime": DateTimeRangeTypeDef,
+        "endTime": DateTimeRangeTypeDef,
+        "lastUpdatedTime": DateTimeRangeTypeDef,
+        "entityArns": Sequence[str],
+        "entityValues": Sequence[str],
+        "eventTypeCategories": Sequence[eventTypeCategoryType],
+        "eventStatusCodes": Sequence[eventStatusCodeType],
+    },
+    total=False,
+)
+
+DescribeEventDetailsResponseTypeDef = TypedDict(
+    "DescribeEventDetailsResponseTypeDef",
+    {
+        "successfulSet": List[EventDetailsTypeDef],
+        "failedSet": List[EventDetailsErrorItemTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeEventDetailsForOrganizationResponseTypeDef = TypedDict(
+    "DescribeEventDetailsForOrganizationResponseTypeDef",
+    {
+        "successfulSet": List[OrganizationEventDetailsTypeDef],
+        "failedSet": List[OrganizationEventDetailsErrorItemTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredDescribeAffectedEntitiesRequestDescribeAffectedEntitiesPaginateTypeDef = TypedDict(
     "_RequiredDescribeAffectedEntitiesRequestDescribeAffectedEntitiesPaginateTypeDef",
     {
         "filter": EntityFilterTypeDef,
     },
 )
 _OptionalDescribeAffectedEntitiesRequestDescribeAffectedEntitiesPaginateTypeDef = TypedDict(
@@ -609,22 +612,20 @@
     {
         "locale": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeAffectedEntitiesRequestDescribeAffectedEntitiesPaginateTypeDef(
     _RequiredDescribeAffectedEntitiesRequestDescribeAffectedEntitiesPaginateTypeDef,
     _OptionalDescribeAffectedEntitiesRequestDescribeAffectedEntitiesPaginateTypeDef,
 ):
     pass
 
-
 _RequiredDescribeAffectedEntitiesRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeAffectedEntitiesRequestRequestTypeDef",
     {
         "filter": EntityFilterTypeDef,
     },
 )
 _OptionalDescribeAffectedEntitiesRequestRequestTypeDef = TypedDict(
@@ -633,22 +634,20 @@
         "locale": str,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class DescribeAffectedEntitiesRequestRequestTypeDef(
     _RequiredDescribeAffectedEntitiesRequestRequestTypeDef,
     _OptionalDescribeAffectedEntitiesRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDescribeEventAggregatesRequestDescribeEventAggregatesPaginateTypeDef = TypedDict(
     "_RequiredDescribeEventAggregatesRequestDescribeEventAggregatesPaginateTypeDef",
     {
         "aggregateField": Literal["eventTypeCategory"],
     },
 )
 _OptionalDescribeEventAggregatesRequestDescribeEventAggregatesPaginateTypeDef = TypedDict(
@@ -656,22 +655,20 @@
     {
         "filter": EventFilterTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeEventAggregatesRequestDescribeEventAggregatesPaginateTypeDef(
     _RequiredDescribeEventAggregatesRequestDescribeEventAggregatesPaginateTypeDef,
     _OptionalDescribeEventAggregatesRequestDescribeEventAggregatesPaginateTypeDef,
 ):
     pass
 
-
 _RequiredDescribeEventAggregatesRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeEventAggregatesRequestRequestTypeDef",
     {
         "aggregateField": Literal["eventTypeCategory"],
     },
 )
 _OptionalDescribeEventAggregatesRequestRequestTypeDef = TypedDict(
@@ -680,22 +677,20 @@
         "filter": EventFilterTypeDef,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class DescribeEventAggregatesRequestRequestTypeDef(
     _RequiredDescribeEventAggregatesRequestRequestTypeDef,
     _OptionalDescribeEventAggregatesRequestRequestTypeDef,
 ):
     pass
 
-
 DescribeEventsRequestDescribeEventsPaginateTypeDef = TypedDict(
     "DescribeEventsRequestDescribeEventsPaginateTypeDef",
     {
         "filter": EventFilterTypeDef,
         "locale": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
@@ -729,25 +724,7 @@
         "filter": OrganizationEventFilterTypeDef,
         "nextToken": str,
         "maxResults": int,
         "locale": str,
     },
     total=False,
 )
-
-DescribeEventDetailsResponseTypeDef = TypedDict(
-    "DescribeEventDetailsResponseTypeDef",
-    {
-        "successfulSet": List[EventDetailsTypeDef],
-        "failedSet": List[EventDetailsErrorItemTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeEventDetailsForOrganizationResponseTypeDef = TypedDict(
-    "DescribeEventDetailsForOrganizationResponseTypeDef",
-    {
-        "successfulSet": List[OrganizationEventDetailsTypeDef],
-        "failedSet": List[OrganizationEventDetailsErrorItemTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
```

### Comparing `mypy-boto3-health-1.28.15.post1/mypy_boto3_health/type_defs.pyi` & `mypy-boto3-health-1.28.16/mypy_boto3_health/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_health/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_health.type_defs import AffectedEntityTypeDef
 
-    data: AffectedEntityTypeDef = {...}
+    data: AffectedEntityTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -27,17 +27,18 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AffectedEntityTypeDef",
-    "DateTimeRangeTypeDef",
+    "TimestampTypeDef",
     "PaginatorConfigTypeDef",
     "DescribeAffectedAccountsForOrganizationRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "EventAccountFilterTypeDef",
     "OrganizationAffectedEntitiesErrorItemTypeDef",
     "DescribeEntityAggregatesRequestRequestTypeDef",
     "EntityAggregateTypeDef",
@@ -46,17 +47,15 @@
     "DescribeEventDetailsRequestRequestTypeDef",
     "EventDetailsErrorItemTypeDef",
     "EventTypeFilterTypeDef",
     "EventTypeTypeDef",
     "OrganizationEventTypeDef",
     "EventTypeDef",
     "EventDescriptionTypeDef",
-    "EntityFilterTypeDef",
-    "EventFilterTypeDef",
-    "OrganizationEventFilterTypeDef",
+    "DateTimeRangeTypeDef",
     "DescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef",
     "DescribeAffectedAccountsForOrganizationResponseTypeDef",
     "DescribeAffectedEntitiesResponseTypeDef",
     "DescribeHealthServiceStatusForOrganizationResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "DescribeAffectedEntitiesForOrganizationRequestDescribeAffectedEntitiesForOrganizationPaginateTypeDef",
     "DescribeAffectedEntitiesForOrganizationRequestRequestTypeDef",
@@ -67,24 +66,27 @@
     "DescribeEventTypesRequestDescribeEventTypesPaginateTypeDef",
     "DescribeEventTypesRequestRequestTypeDef",
     "DescribeEventTypesResponseTypeDef",
     "DescribeEventsForOrganizationResponseTypeDef",
     "DescribeEventsResponseTypeDef",
     "EventDetailsTypeDef",
     "OrganizationEventDetailsTypeDef",
+    "EntityFilterTypeDef",
+    "EventFilterTypeDef",
+    "OrganizationEventFilterTypeDef",
+    "DescribeEventDetailsResponseTypeDef",
+    "DescribeEventDetailsForOrganizationResponseTypeDef",
     "DescribeAffectedEntitiesRequestDescribeAffectedEntitiesPaginateTypeDef",
     "DescribeAffectedEntitiesRequestRequestTypeDef",
     "DescribeEventAggregatesRequestDescribeEventAggregatesPaginateTypeDef",
     "DescribeEventAggregatesRequestRequestTypeDef",
     "DescribeEventsRequestDescribeEventsPaginateTypeDef",
     "DescribeEventsRequestRequestTypeDef",
     "DescribeEventsForOrganizationRequestDescribeEventsForOrganizationPaginateTypeDef",
     "DescribeEventsForOrganizationRequestRequestTypeDef",
-    "DescribeEventDetailsResponseTypeDef",
-    "DescribeEventDetailsForOrganizationResponseTypeDef",
 )
 
 AffectedEntityTypeDef = TypedDict(
     "AffectedEntityTypeDef",
     {
         "entityArn": str,
         "eventArn": str,
@@ -94,23 +96,15 @@
         "lastUpdatedTime": datetime,
         "statusCode": entityStatusCodeType,
         "tags": Dict[str, str],
     },
     total=False,
 )
 
-DateTimeRangeTypeDef = TypedDict(
-    "DateTimeRangeTypeDef",
-    {
-        "from": Union[datetime, str],
-        "to": Union[datetime, str],
-    },
-    total=False,
-)
-
+TimestampTypeDef = Union[datetime, str]
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
@@ -128,20 +122,22 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class DescribeAffectedAccountsForOrganizationRequestRequestTypeDef(
     _RequiredDescribeAffectedAccountsForOrganizationRequestRequestTypeDef,
     _OptionalDescribeAffectedAccountsForOrganizationRequestRequestTypeDef,
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
@@ -159,19 +155,21 @@
     "_OptionalEventAccountFilterTypeDef",
     {
         "awsAccountId": str,
     },
     total=False,
 )
 
+
 class EventAccountFilterTypeDef(
     _RequiredEventAccountFilterTypeDef, _OptionalEventAccountFilterTypeDef
 ):
     pass
 
+
 OrganizationAffectedEntitiesErrorItemTypeDef = TypedDict(
     "OrganizationAffectedEntitiesErrorItemTypeDef",
     {
         "awsAccountId": str,
         "eventArn": str,
         "errorName": str,
         "errorMessage": str,
@@ -226,20 +224,22 @@
     "_OptionalDescribeEventDetailsRequestRequestTypeDef",
     {
         "locale": str,
     },
     total=False,
 )
 
+
 class DescribeEventDetailsRequestRequestTypeDef(
     _RequiredDescribeEventDetailsRequestRequestTypeDef,
     _OptionalDescribeEventDetailsRequestRequestTypeDef,
 ):
     pass
 
+
 EventDetailsErrorItemTypeDef = TypedDict(
     "EventDetailsErrorItemTypeDef",
     {
         "eventArn": str,
         "errorName": str,
         "errorMessage": str,
     },
@@ -305,69 +305,19 @@
     "EventDescriptionTypeDef",
     {
         "latestDescription": str,
     },
     total=False,
 )
 
-_RequiredEntityFilterTypeDef = TypedDict(
-    "_RequiredEntityFilterTypeDef",
-    {
-        "eventArns": Sequence[str],
-    },
-)
-_OptionalEntityFilterTypeDef = TypedDict(
-    "_OptionalEntityFilterTypeDef",
-    {
-        "entityArns": Sequence[str],
-        "entityValues": Sequence[str],
-        "lastUpdatedTimes": Sequence[DateTimeRangeTypeDef],
-        "tags": Sequence[Mapping[str, str]],
-        "statusCodes": Sequence[entityStatusCodeType],
-    },
-    total=False,
-)
-
-class EntityFilterTypeDef(_RequiredEntityFilterTypeDef, _OptionalEntityFilterTypeDef):
-    pass
-
-EventFilterTypeDef = TypedDict(
-    "EventFilterTypeDef",
-    {
-        "eventArns": Sequence[str],
-        "eventTypeCodes": Sequence[str],
-        "services": Sequence[str],
-        "regions": Sequence[str],
-        "availabilityZones": Sequence[str],
-        "startTimes": Sequence[DateTimeRangeTypeDef],
-        "endTimes": Sequence[DateTimeRangeTypeDef],
-        "lastUpdatedTimes": Sequence[DateTimeRangeTypeDef],
-        "entityArns": Sequence[str],
-        "entityValues": Sequence[str],
-        "eventTypeCategories": Sequence[eventTypeCategoryType],
-        "tags": Sequence[Mapping[str, str]],
-        "eventStatusCodes": Sequence[eventStatusCodeType],
-    },
-    total=False,
-)
-
-OrganizationEventFilterTypeDef = TypedDict(
-    "OrganizationEventFilterTypeDef",
+DateTimeRangeTypeDef = TypedDict(
+    "DateTimeRangeTypeDef",
     {
-        "eventTypeCodes": Sequence[str],
-        "awsAccountIds": Sequence[str],
-        "services": Sequence[str],
-        "regions": Sequence[str],
-        "startTime": DateTimeRangeTypeDef,
-        "endTime": DateTimeRangeTypeDef,
-        "lastUpdatedTime": DateTimeRangeTypeDef,
-        "entityArns": Sequence[str],
-        "entityValues": Sequence[str],
-        "eventTypeCategories": Sequence[eventTypeCategoryType],
-        "eventStatusCodes": Sequence[eventStatusCodeType],
+        "from": TimestampTypeDef,
+        "to": TimestampTypeDef,
     },
     total=False,
 )
 
 _RequiredDescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef = TypedDict(
     "_RequiredDescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef",
     {
@@ -378,20 +328,22 @@
     "_OptionalDescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef(
     _RequiredDescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef,
     _OptionalDescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef,
 ):
     pass
 
+
 DescribeAffectedAccountsForOrganizationResponseTypeDef = TypedDict(
     "DescribeAffectedAccountsForOrganizationResponseTypeDef",
     {
         "affectedAccounts": List[str],
         "eventScopeCode": eventScopeCodeType,
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -433,20 +385,22 @@
     {
         "locale": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeAffectedEntitiesForOrganizationRequestDescribeAffectedEntitiesForOrganizationPaginateTypeDef(
     _RequiredDescribeAffectedEntitiesForOrganizationRequestDescribeAffectedEntitiesForOrganizationPaginateTypeDef,
     _OptionalDescribeAffectedEntitiesForOrganizationRequestDescribeAffectedEntitiesForOrganizationPaginateTypeDef,
 ):
     pass
 
+
 _RequiredDescribeAffectedEntitiesForOrganizationRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeAffectedEntitiesForOrganizationRequestRequestTypeDef",
     {
         "organizationEntityFilters": Sequence[EventAccountFilterTypeDef],
     },
 )
 _OptionalDescribeAffectedEntitiesForOrganizationRequestRequestTypeDef = TypedDict(
@@ -455,40 +409,44 @@
         "locale": str,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class DescribeAffectedEntitiesForOrganizationRequestRequestTypeDef(
     _RequiredDescribeAffectedEntitiesForOrganizationRequestRequestTypeDef,
     _OptionalDescribeAffectedEntitiesForOrganizationRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDescribeEventDetailsForOrganizationRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeEventDetailsForOrganizationRequestRequestTypeDef",
     {
         "organizationEventDetailFilters": Sequence[EventAccountFilterTypeDef],
     },
 )
 _OptionalDescribeEventDetailsForOrganizationRequestRequestTypeDef = TypedDict(
     "_OptionalDescribeEventDetailsForOrganizationRequestRequestTypeDef",
     {
         "locale": str,
     },
     total=False,
 )
 
+
 class DescribeEventDetailsForOrganizationRequestRequestTypeDef(
     _RequiredDescribeEventDetailsForOrganizationRequestRequestTypeDef,
     _OptionalDescribeEventDetailsForOrganizationRequestRequestTypeDef,
 ):
     pass
 
+
 DescribeAffectedEntitiesForOrganizationResponseTypeDef = TypedDict(
     "DescribeAffectedEntitiesForOrganizationResponseTypeDef",
     {
         "entities": List[AffectedEntityTypeDef],
         "failedSet": List[OrganizationAffectedEntitiesErrorItemTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -577,14 +535,93 @@
         "event": EventTypeDef,
         "eventDescription": EventDescriptionTypeDef,
         "eventMetadata": Dict[str, str],
     },
     total=False,
 )
 
+_RequiredEntityFilterTypeDef = TypedDict(
+    "_RequiredEntityFilterTypeDef",
+    {
+        "eventArns": Sequence[str],
+    },
+)
+_OptionalEntityFilterTypeDef = TypedDict(
+    "_OptionalEntityFilterTypeDef",
+    {
+        "entityArns": Sequence[str],
+        "entityValues": Sequence[str],
+        "lastUpdatedTimes": Sequence[DateTimeRangeTypeDef],
+        "tags": Sequence[Mapping[str, str]],
+        "statusCodes": Sequence[entityStatusCodeType],
+    },
+    total=False,
+)
+
+
+class EntityFilterTypeDef(_RequiredEntityFilterTypeDef, _OptionalEntityFilterTypeDef):
+    pass
+
+
+EventFilterTypeDef = TypedDict(
+    "EventFilterTypeDef",
+    {
+        "eventArns": Sequence[str],
+        "eventTypeCodes": Sequence[str],
+        "services": Sequence[str],
+        "regions": Sequence[str],
+        "availabilityZones": Sequence[str],
+        "startTimes": Sequence[DateTimeRangeTypeDef],
+        "endTimes": Sequence[DateTimeRangeTypeDef],
+        "lastUpdatedTimes": Sequence[DateTimeRangeTypeDef],
+        "entityArns": Sequence[str],
+        "entityValues": Sequence[str],
+        "eventTypeCategories": Sequence[eventTypeCategoryType],
+        "tags": Sequence[Mapping[str, str]],
+        "eventStatusCodes": Sequence[eventStatusCodeType],
+    },
+    total=False,
+)
+
+OrganizationEventFilterTypeDef = TypedDict(
+    "OrganizationEventFilterTypeDef",
+    {
+        "eventTypeCodes": Sequence[str],
+        "awsAccountIds": Sequence[str],
+        "services": Sequence[str],
+        "regions": Sequence[str],
+        "startTime": DateTimeRangeTypeDef,
+        "endTime": DateTimeRangeTypeDef,
+        "lastUpdatedTime": DateTimeRangeTypeDef,
+        "entityArns": Sequence[str],
+        "entityValues": Sequence[str],
+        "eventTypeCategories": Sequence[eventTypeCategoryType],
+        "eventStatusCodes": Sequence[eventStatusCodeType],
+    },
+    total=False,
+)
+
+DescribeEventDetailsResponseTypeDef = TypedDict(
+    "DescribeEventDetailsResponseTypeDef",
+    {
+        "successfulSet": List[EventDetailsTypeDef],
+        "failedSet": List[EventDetailsErrorItemTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeEventDetailsForOrganizationResponseTypeDef = TypedDict(
+    "DescribeEventDetailsForOrganizationResponseTypeDef",
+    {
+        "successfulSet": List[OrganizationEventDetailsTypeDef],
+        "failedSet": List[OrganizationEventDetailsErrorItemTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredDescribeAffectedEntitiesRequestDescribeAffectedEntitiesPaginateTypeDef = TypedDict(
     "_RequiredDescribeAffectedEntitiesRequestDescribeAffectedEntitiesPaginateTypeDef",
     {
         "filter": EntityFilterTypeDef,
     },
 )
 _OptionalDescribeAffectedEntitiesRequestDescribeAffectedEntitiesPaginateTypeDef = TypedDict(
@@ -592,20 +629,22 @@
     {
         "locale": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeAffectedEntitiesRequestDescribeAffectedEntitiesPaginateTypeDef(
     _RequiredDescribeAffectedEntitiesRequestDescribeAffectedEntitiesPaginateTypeDef,
     _OptionalDescribeAffectedEntitiesRequestDescribeAffectedEntitiesPaginateTypeDef,
 ):
     pass
 
+
 _RequiredDescribeAffectedEntitiesRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeAffectedEntitiesRequestRequestTypeDef",
     {
         "filter": EntityFilterTypeDef,
     },
 )
 _OptionalDescribeAffectedEntitiesRequestRequestTypeDef = TypedDict(
@@ -614,20 +653,22 @@
         "locale": str,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class DescribeAffectedEntitiesRequestRequestTypeDef(
     _RequiredDescribeAffectedEntitiesRequestRequestTypeDef,
     _OptionalDescribeAffectedEntitiesRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDescribeEventAggregatesRequestDescribeEventAggregatesPaginateTypeDef = TypedDict(
     "_RequiredDescribeEventAggregatesRequestDescribeEventAggregatesPaginateTypeDef",
     {
         "aggregateField": Literal["eventTypeCategory"],
     },
 )
 _OptionalDescribeEventAggregatesRequestDescribeEventAggregatesPaginateTypeDef = TypedDict(
@@ -635,20 +676,22 @@
     {
         "filter": EventFilterTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeEventAggregatesRequestDescribeEventAggregatesPaginateTypeDef(
     _RequiredDescribeEventAggregatesRequestDescribeEventAggregatesPaginateTypeDef,
     _OptionalDescribeEventAggregatesRequestDescribeEventAggregatesPaginateTypeDef,
 ):
     pass
 
+
 _RequiredDescribeEventAggregatesRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeEventAggregatesRequestRequestTypeDef",
     {
         "aggregateField": Literal["eventTypeCategory"],
     },
 )
 _OptionalDescribeEventAggregatesRequestRequestTypeDef = TypedDict(
@@ -657,20 +700,22 @@
         "filter": EventFilterTypeDef,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class DescribeEventAggregatesRequestRequestTypeDef(
     _RequiredDescribeEventAggregatesRequestRequestTypeDef,
     _OptionalDescribeEventAggregatesRequestRequestTypeDef,
 ):
     pass
 
+
 DescribeEventsRequestDescribeEventsPaginateTypeDef = TypedDict(
     "DescribeEventsRequestDescribeEventsPaginateTypeDef",
     {
         "filter": EventFilterTypeDef,
         "locale": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
@@ -704,25 +749,7 @@
         "filter": OrganizationEventFilterTypeDef,
         "nextToken": str,
         "maxResults": int,
         "locale": str,
     },
     total=False,
 )
-
-DescribeEventDetailsResponseTypeDef = TypedDict(
-    "DescribeEventDetailsResponseTypeDef",
-    {
-        "successfulSet": List[EventDetailsTypeDef],
-        "failedSet": List[EventDetailsErrorItemTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeEventDetailsForOrganizationResponseTypeDef = TypedDict(
-    "DescribeEventDetailsForOrganizationResponseTypeDef",
-    {
-        "successfulSet": List[OrganizationEventDetailsTypeDef],
-        "failedSet": List[OrganizationEventDetailsErrorItemTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
```

### Comparing `mypy-boto3-health-1.28.15.post1/mypy_boto3_health.egg-info/PKG-INFO` & `mypy-boto3-health-1.28.16/mypy_boto3_health.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-health
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.Health 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.Health 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_health/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 health type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 health type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-health.svg?color=blue)](https://pypi.org/project/mypy-boto3-health)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_health/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-health)](https://pepy.tech/project/mypy-boto3-health)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Health 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health)
+[boto3.Health 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health)
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
 [mypy-boto3-health docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_health/).
 
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
@@ -346,25 +346,25 @@
 )
 
 
 def check_value(value: DescribeAffectedAccountsForOrganizationPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_health.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_health.type_defs import (
     AffectedEntityTypeDef,
-    DateTimeRangeTypeDef,
+    TimestampTypeDef,
     PaginatorConfigTypeDef,
     DescribeAffectedAccountsForOrganizationRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     EventAccountFilterTypeDef,
     OrganizationAffectedEntitiesErrorItemTypeDef,
     DescribeEntityAggregatesRequestRequestTypeDef,
     EntityAggregateTypeDef,
@@ -373,17 +373,15 @@
     DescribeEventDetailsRequestRequestTypeDef,
     EventDetailsErrorItemTypeDef,
     EventTypeFilterTypeDef,
     EventTypeTypeDef,
     OrganizationEventTypeDef,
     EventTypeDef,
     EventDescriptionTypeDef,
-    EntityFilterTypeDef,
-    EventFilterTypeDef,
-    OrganizationEventFilterTypeDef,
+    DateTimeRangeTypeDef,
     DescribeAffectedAccountsForOrganizationRequestDescribeAffectedAccountsForOrganizationPaginateTypeDef,
     DescribeAffectedAccountsForOrganizationResponseTypeDef,
     DescribeAffectedEntitiesResponseTypeDef,
     DescribeHealthServiceStatusForOrganizationResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     DescribeAffectedEntitiesForOrganizationRequestDescribeAffectedEntitiesForOrganizationPaginateTypeDef,
     DescribeAffectedEntitiesForOrganizationRequestRequestTypeDef,
@@ -394,28 +392,31 @@
     DescribeEventTypesRequestDescribeEventTypesPaginateTypeDef,
     DescribeEventTypesRequestRequestTypeDef,
     DescribeEventTypesResponseTypeDef,
     DescribeEventsForOrganizationResponseTypeDef,
     DescribeEventsResponseTypeDef,
     EventDetailsTypeDef,
     OrganizationEventDetailsTypeDef,
+    EntityFilterTypeDef,
+    EventFilterTypeDef,
+    OrganizationEventFilterTypeDef,
+    DescribeEventDetailsResponseTypeDef,
+    DescribeEventDetailsForOrganizationResponseTypeDef,
     DescribeAffectedEntitiesRequestDescribeAffectedEntitiesPaginateTypeDef,
     DescribeAffectedEntitiesRequestRequestTypeDef,
     DescribeEventAggregatesRequestDescribeEventAggregatesPaginateTypeDef,
     DescribeEventAggregatesRequestRequestTypeDef,
     DescribeEventsRequestDescribeEventsPaginateTypeDef,
     DescribeEventsRequestRequestTypeDef,
     DescribeEventsForOrganizationRequestDescribeEventsForOrganizationPaginateTypeDef,
     DescribeEventsForOrganizationRequestRequestTypeDef,
-    DescribeEventDetailsResponseTypeDef,
-    DescribeEventDetailsForOrganizationResponseTypeDef,
 )
 
 
-def get_structure() -> AffectedEntityTypeDef:
+def get_value() -> AffectedEntityTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-health-1.28.15.post1/mypy_boto3_health.egg-info/SOURCES.txt` & `mypy-boto3-health-1.28.16/mypy_boto3_health.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-health-1.28.15.post1/setup.py` & `mypy-boto3-health-1.28.16/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-health",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_health"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Health 1.28.15 service generated with mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.Health 1.28.16 service generated with mypy-boto3-builder 7.17.1"
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
-    keywords="boto3 health type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 health type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_health": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_health/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

