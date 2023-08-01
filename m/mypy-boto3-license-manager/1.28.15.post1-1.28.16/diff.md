# Comparing `tmp/mypy-boto3-license-manager-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-license-manager-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-license-manager-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:32 2023, max compression
+gzip compressed data, was "mypy-boto3-license-manager-1.28.16.tar", last modified: Tue Aug  1 11:37:12 2023, max compression
```

## Comparing `mypy-boto3-license-manager-1.28.15.post1.tar` & `mypy-boto3-license-manager-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:32.189242 mypy-boto3-license-manager-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:49:45.000000 mypy-boto3-license-manager-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20368 2023-07-29 10:03:32.189242 mypy-boto3-license-manager-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18844 2023-07-29 09:49:45.000000 mypy-boto3-license-manager-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:32.181242 mypy-boto3-license-manager-1.28.15.post1/mypy_boto3_license_manager/
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-07-29 09:49:45.000000 mypy-boto3-license-manager-1.28.15.post1/mypy_boto3_license_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-07-29 09:49:45.000000 mypy-boto3-license-manager-1.28.15.post1/mypy_boto3_license_manager/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-29 09:49:45.000000 mypy-boto3-license-manager-1.28.15.post1/mypy_boto3_license_manager/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40977 2023-07-29 09:49:45.000000 mypy-boto3-license-manager-1.28.15.post1/mypy_boto3_license_manager/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    40915 2023-07-29 09:49:45.000000 mypy-boto3-license-manager-1.28.15.post1/mypy_boto3_license_manager/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12467 2023-07-29 09:49:45.000000 mypy-boto3-license-manager-1.28.15.post1/mypy_boto3_license_manager/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12465 2023-07-29 09:49:45.000000 mypy-boto3-license-manager-1.28.15.post1/mypy_boto3_license_manager/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7586 2023-07-29 09:49:45.000000 mypy-boto3-license-manager-1.28.15.post1/mypy_boto3_license_manager/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7579 2023-07-29 09:49:45.000000 mypy-boto3-license-manager-1.28.15.post1/mypy_boto3_license_manager/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:49:45.000000 mypy-boto3-license-manager-1.28.15.post1/mypy_boto3_license_manager/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    56262 2023-07-29 09:49:47.000000 mypy-boto3-license-manager-1.28.15.post1/mypy_boto3_license_manager/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    56189 2023-07-29 09:49:46.000000 mypy-boto3-license-manager-1.28.15.post1/mypy_boto3_license_manager/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:49:45.000000 mypy-boto3-license-manager-1.28.15.post1/mypy_boto3_license_manager/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:32.189242 mypy-boto3-license-manager-1.28.15.post1/mypy_boto3_license_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20368 2023-07-29 10:03:31.000000 mypy-boto3-license-manager-1.28.15.post1/mypy_boto3_license_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-29 10:03:31.000000 mypy-boto3-license-manager-1.28.15.post1/mypy_boto3_license_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:31.000000 mypy-boto3-license-manager-1.28.15.post1/mypy_boto3_license_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:31.000000 mypy-boto3-license-manager-1.28.15.post1/mypy_boto3_license_manager.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:31.000000 mypy-boto3-license-manager-1.28.15.post1/mypy_boto3_license_manager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-29 10:03:31.000000 mypy-boto3-license-manager-1.28.15.post1/mypy_boto3_license_manager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:32.189242 mypy-boto3-license-manager-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-07-29 09:49:44.000000 mypy-boto3-license-manager-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:12.852839 mypy-boto3-license-manager-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:22:34.000000 mypy-boto3-license-manager-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20425 2023-08-01 11:37:12.844838 mypy-boto3-license-manager-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18910 2023-08-01 11:22:34.000000 mypy-boto3-license-manager-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:12.844838 mypy-boto3-license-manager-1.28.16/mypy_boto3_license_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-08-01 11:22:34.000000 mypy-boto3-license-manager-1.28.16/mypy_boto3_license_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-08-01 11:22:34.000000 mypy-boto3-license-manager-1.28.16/mypy_boto3_license_manager/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-08-01 11:22:34.000000 mypy-boto3-license-manager-1.28.16/mypy_boto3_license_manager/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40737 2023-08-01 11:22:34.000000 mypy-boto3-license-manager-1.28.16/mypy_boto3_license_manager/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40675 2023-08-01 11:22:34.000000 mypy-boto3-license-manager-1.28.16/mypy_boto3_license_manager/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12467 2023-08-01 11:22:35.000000 mypy-boto3-license-manager-1.28.16/mypy_boto3_license_manager/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12465 2023-08-01 11:22:34.000000 mypy-boto3-license-manager-1.28.16/mypy_boto3_license_manager/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7586 2023-08-01 11:22:34.000000 mypy-boto3-license-manager-1.28.16/mypy_boto3_license_manager/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7579 2023-08-01 11:22:34.000000 mypy-boto3-license-manager-1.28.16/mypy_boto3_license_manager/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:22:34.000000 mypy-boto3-license-manager-1.28.16/mypy_boto3_license_manager/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    56399 2023-08-01 11:22:36.000000 mypy-boto3-license-manager-1.28.16/mypy_boto3_license_manager/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56327 2023-08-01 11:22:35.000000 mypy-boto3-license-manager-1.28.16/mypy_boto3_license_manager/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:22:34.000000 mypy-boto3-license-manager-1.28.16/mypy_boto3_license_manager/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:12.844838 mypy-boto3-license-manager-1.28.16/mypy_boto3_license_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20425 2023-08-01 11:37:12.000000 mypy-boto3-license-manager-1.28.16/mypy_boto3_license_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-08-01 11:37:12.000000 mypy-boto3-license-manager-1.28.16/mypy_boto3_license_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:12.000000 mypy-boto3-license-manager-1.28.16/mypy_boto3_license_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:12.000000 mypy-boto3-license-manager-1.28.16/mypy_boto3_license_manager.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:12.000000 mypy-boto3-license-manager-1.28.16/mypy_boto3_license_manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-01 11:37:12.000000 mypy-boto3-license-manager-1.28.16/mypy_boto3_license_manager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:12.852839 mypy-boto3-license-manager-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-08-01 11:22:34.000000 mypy-boto3-license-manager-1.28.16/setup.py
```

### Comparing `mypy-boto3-license-manager-1.28.15.post1/LICENSE` & `mypy-boto3-license-manager-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-1.28.15.post1/PKG-INFO` & `mypy-boto3-license-manager-1.28.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-license-manager
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.LicenseManager 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.LicenseManager 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 license-manager type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 license-manager type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-license-manager.svg?color=blue)](https://pypi.org/project/mypy-boto3-license-manager)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-license-manager)](https://pepy.tech/project/mypy-boto3-license-manager)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LicenseManager 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager)
+[boto3.LicenseManager 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager)
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
 [mypy-boto3-license-manager docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager/).
 
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
@@ -354,20 +354,20 @@
 )
 
 
 def check_value(value: ActivationOverrideBehaviorType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_license_manager.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_license_manager.type_defs import (
     AcceptGrantRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     AutomatedDiscoveryInformationTypeDef,
     BorrowConfigurationTypeDef,
@@ -476,42 +476,44 @@
     ListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef,
     ListResourceInventoryRequestListResourceInventoryPaginateTypeDef,
     ListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef,
     ListResourceInventoryResponseTypeDef,
     ListTokensResponseTypeDef,
     ProductInformationOutputTypeDef,
     ProductInformationTypeDef,
+    ReportContextUnionTypeDef,
     ReportGeneratorTypeDef,
     ListFailuresForLicenseConfigurationOperationsResponseTypeDef,
     CreateLicenseRequestRequestTypeDef,
     CreateLicenseVersionRequestRequestTypeDef,
     GrantedLicenseTypeDef,
     LicenseTypeDef,
     GetGrantResponseTypeDef,
     ListDistributedGrantsResponseTypeDef,
     ListReceivedGrantsForOrganizationResponseTypeDef,
     ListReceivedGrantsResponseTypeDef,
     ListLicenseConversionTasksResponseTypeDef,
     GetLicenseUsageResponseTypeDef,
     GetLicenseConfigurationResponseTypeDef,
     LicenseConfigurationTypeDef,
-    CreateLicenseConfigurationRequestRequestTypeDef,
-    UpdateLicenseConfigurationRequestRequestTypeDef,
+    ProductInformationUnionTypeDef,
     GetLicenseManagerReportGeneratorResponseTypeDef,
     ListLicenseManagerReportGeneratorsResponseTypeDef,
     ListReceivedLicensesForOrganizationResponseTypeDef,
     ListReceivedLicensesResponseTypeDef,
     GetLicenseResponseTypeDef,
     ListLicenseVersionsResponseTypeDef,
     ListLicensesResponseTypeDef,
     ListLicenseConfigurationsResponseTypeDef,
+    CreateLicenseConfigurationRequestRequestTypeDef,
+    UpdateLicenseConfigurationRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AcceptGrantRequestRequestTypeDef:
+def get_value() -> AcceptGrantRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-license-manager-1.28.15.post1/README.md` & `mypy-boto3-license-manager-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-license-manager.svg?color=blue)](https://pypi.org/project/mypy-boto3-license-manager)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-license-manager)](https://pepy.tech/project/mypy-boto3-license-manager)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LicenseManager 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager)
+[boto3.LicenseManager 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager)
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
 [mypy-boto3-license-manager docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager/).
 
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
@@ -322,20 +322,20 @@
 )
 
 
 def check_value(value: ActivationOverrideBehaviorType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_license_manager.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_license_manager.type_defs import (
     AcceptGrantRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     AutomatedDiscoveryInformationTypeDef,
     BorrowConfigurationTypeDef,
@@ -444,42 +444,44 @@
     ListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef,
     ListResourceInventoryRequestListResourceInventoryPaginateTypeDef,
     ListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef,
     ListResourceInventoryResponseTypeDef,
     ListTokensResponseTypeDef,
     ProductInformationOutputTypeDef,
     ProductInformationTypeDef,
+    ReportContextUnionTypeDef,
     ReportGeneratorTypeDef,
     ListFailuresForLicenseConfigurationOperationsResponseTypeDef,
     CreateLicenseRequestRequestTypeDef,
     CreateLicenseVersionRequestRequestTypeDef,
     GrantedLicenseTypeDef,
     LicenseTypeDef,
     GetGrantResponseTypeDef,
     ListDistributedGrantsResponseTypeDef,
     ListReceivedGrantsForOrganizationResponseTypeDef,
     ListReceivedGrantsResponseTypeDef,
     ListLicenseConversionTasksResponseTypeDef,
     GetLicenseUsageResponseTypeDef,
     GetLicenseConfigurationResponseTypeDef,
     LicenseConfigurationTypeDef,
-    CreateLicenseConfigurationRequestRequestTypeDef,
-    UpdateLicenseConfigurationRequestRequestTypeDef,
+    ProductInformationUnionTypeDef,
     GetLicenseManagerReportGeneratorResponseTypeDef,
     ListLicenseManagerReportGeneratorsResponseTypeDef,
     ListReceivedLicensesForOrganizationResponseTypeDef,
     ListReceivedLicensesResponseTypeDef,
     GetLicenseResponseTypeDef,
     ListLicenseVersionsResponseTypeDef,
     ListLicensesResponseTypeDef,
     ListLicenseConfigurationsResponseTypeDef,
+    CreateLicenseConfigurationRequestRequestTypeDef,
+    UpdateLicenseConfigurationRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AcceptGrantRequestRequestTypeDef:
+def get_value() -> AcceptGrantRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-license-manager-1.28.15.post1/mypy_boto3_license_manager/__init__.py` & `mypy-boto3-license-manager-1.28.16/mypy_boto3_license_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-1.28.15.post1/mypy_boto3_license_manager/__init__.pyi` & `mypy-boto3-license-manager-1.28.16/mypy_boto3_license_manager/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-1.28.15.post1/mypy_boto3_license_manager/__main__.py` & `mypy-boto3-license-manager-1.28.16/mypy_boto3_license_manager/__main__.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.LicenseManager 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.LicenseManager 1.28.16\nVersion:         1.28.16\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager\nOther"
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

### Comparing `mypy-boto3-license-manager-1.28.15.post1/mypy_boto3_license_manager/client.py` & `mypy-boto3-license-manager-1.28.16/mypy_boto3_license_manager/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_license_manager.client import LicenseManagerClient
 
     session = Session()
     client: LicenseManagerClient = session.client("license-manager")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AllowedOperationType,
     CheckoutTypeType,
     GrantStatusType,
@@ -82,19 +82,17 @@
     ListResourceInventoryResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTokensResponseTypeDef,
     ListUsageForLicenseConfigurationResponseTypeDef,
     MetadataTypeDef,
     OptionsTypeDef,
     OrganizationConfigurationTypeDef,
-    ProductInformationOutputTypeDef,
-    ProductInformationTypeDef,
+    ProductInformationUnionTypeDef,
     RejectGrantResponseTypeDef,
-    ReportContextOutputTypeDef,
-    ReportContextTypeDef,
+    ReportContextUnionTypeDef,
     ReportFrequencyTypeDef,
     TagTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -284,17 +282,15 @@
         LicenseCountingType: LicenseCountingTypeType,
         Description: str = ...,
         LicenseCount: int = ...,
         LicenseCountHardLimit: bool = ...,
         LicenseRules: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         DisassociateWhenNotFound: bool = ...,
-        ProductInformationList: Sequence[
-            Union[ProductInformationTypeDef, ProductInformationOutputTypeDef]
-        ] = ...
+        ProductInformationList: Sequence[ProductInformationUnionTypeDef] = ...
     ) -> CreateLicenseConfigurationResponseTypeDef:
         """
         Creates a license configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.create_license_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager/client/#create_license_configuration)
         """
@@ -314,15 +310,15 @@
         """
 
     def create_license_manager_report_generator(
         self,
         *,
         ReportGeneratorName: str,
         Type: Sequence[ReportTypeType],
-        ReportContext: Union[ReportContextTypeDef, ReportContextOutputTypeDef],
+        ReportContext: ReportContextUnionTypeDef,
         ReportFrequency: ReportFrequencyTypeDef,
         ClientToken: str,
         Description: str = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateLicenseManagerReportGeneratorResponseTypeDef:
         """
         Creates a report generator.
@@ -755,17 +751,15 @@
         LicenseConfigurationArn: str,
         LicenseConfigurationStatus: LicenseConfigurationStatusType = ...,
         LicenseRules: Sequence[str] = ...,
         LicenseCount: int = ...,
         LicenseCountHardLimit: bool = ...,
         Name: str = ...,
         Description: str = ...,
-        ProductInformationList: Sequence[
-            Union[ProductInformationTypeDef, ProductInformationOutputTypeDef]
-        ] = ...,
+        ProductInformationList: Sequence[ProductInformationUnionTypeDef] = ...,
         DisassociateWhenNotFound: bool = ...
     ) -> Dict[str, Any]:
         """
         Modifies the attributes of an existing license configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.update_license_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager/client/#update_license_configuration)
@@ -773,15 +767,15 @@
 
     def update_license_manager_report_generator(
         self,
         *,
         LicenseManagerReportGeneratorArn: str,
         ReportGeneratorName: str,
         Type: Sequence[ReportTypeType],
-        ReportContext: Union[ReportContextTypeDef, ReportContextOutputTypeDef],
+        ReportContext: ReportContextUnionTypeDef,
         ReportFrequency: ReportFrequencyTypeDef,
         ClientToken: str,
         Description: str = ...
     ) -> Dict[str, Any]:
         """
         Updates a report generator.
```

### Comparing `mypy-boto3-license-manager-1.28.15.post1/mypy_boto3_license_manager/client.pyi` & `mypy-boto3-license-manager-1.28.16/mypy_boto3_license_manager/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_license_manager.client import LicenseManagerClient
 
     session = Session()
     client: LicenseManagerClient = session.client("license-manager")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AllowedOperationType,
     CheckoutTypeType,
     GrantStatusType,
@@ -82,19 +82,17 @@
     ListResourceInventoryResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTokensResponseTypeDef,
     ListUsageForLicenseConfigurationResponseTypeDef,
     MetadataTypeDef,
     OptionsTypeDef,
     OrganizationConfigurationTypeDef,
-    ProductInformationOutputTypeDef,
-    ProductInformationTypeDef,
+    ProductInformationUnionTypeDef,
     RejectGrantResponseTypeDef,
-    ReportContextOutputTypeDef,
-    ReportContextTypeDef,
+    ReportContextUnionTypeDef,
     ReportFrequencyTypeDef,
     TagTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -270,17 +268,15 @@
         LicenseCountingType: LicenseCountingTypeType,
         Description: str = ...,
         LicenseCount: int = ...,
         LicenseCountHardLimit: bool = ...,
         LicenseRules: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         DisassociateWhenNotFound: bool = ...,
-        ProductInformationList: Sequence[
-            Union[ProductInformationTypeDef, ProductInformationOutputTypeDef]
-        ] = ...
+        ProductInformationList: Sequence[ProductInformationUnionTypeDef] = ...
     ) -> CreateLicenseConfigurationResponseTypeDef:
         """
         Creates a license configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.create_license_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager/client/#create_license_configuration)
         """
@@ -298,15 +294,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager/client/#create_license_conversion_task_for_resource)
         """
     def create_license_manager_report_generator(
         self,
         *,
         ReportGeneratorName: str,
         Type: Sequence[ReportTypeType],
-        ReportContext: Union[ReportContextTypeDef, ReportContextOutputTypeDef],
+        ReportContext: ReportContextUnionTypeDef,
         ReportFrequency: ReportFrequencyTypeDef,
         ClientToken: str,
         Description: str = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateLicenseManagerReportGeneratorResponseTypeDef:
         """
         Creates a report generator.
@@ -701,32 +697,30 @@
         LicenseConfigurationArn: str,
         LicenseConfigurationStatus: LicenseConfigurationStatusType = ...,
         LicenseRules: Sequence[str] = ...,
         LicenseCount: int = ...,
         LicenseCountHardLimit: bool = ...,
         Name: str = ...,
         Description: str = ...,
-        ProductInformationList: Sequence[
-            Union[ProductInformationTypeDef, ProductInformationOutputTypeDef]
-        ] = ...,
+        ProductInformationList: Sequence[ProductInformationUnionTypeDef] = ...,
         DisassociateWhenNotFound: bool = ...
     ) -> Dict[str, Any]:
         """
         Modifies the attributes of an existing license configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.update_license_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager/client/#update_license_configuration)
         """
     def update_license_manager_report_generator(
         self,
         *,
         LicenseManagerReportGeneratorArn: str,
         ReportGeneratorName: str,
         Type: Sequence[ReportTypeType],
-        ReportContext: Union[ReportContextTypeDef, ReportContextOutputTypeDef],
+        ReportContext: ReportContextUnionTypeDef,
         ReportFrequency: ReportFrequencyTypeDef,
         ClientToken: str,
         Description: str = ...
     ) -> Dict[str, Any]:
         """
         Updates a report generator.
```

### Comparing `mypy-boto3-license-manager-1.28.15.post1/mypy_boto3_license_manager/literals.py` & `mypy-boto3-license-manager-1.28.16/mypy_boto3_license_manager/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-1.28.15.post1/mypy_boto3_license_manager/literals.pyi` & `mypy-boto3-license-manager-1.28.16/mypy_boto3_license_manager/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-1.28.15.post1/mypy_boto3_license_manager/paginator.py` & `mypy-boto3-license-manager-1.28.16/mypy_boto3_license_manager/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-1.28.15.post1/mypy_boto3_license_manager/paginator.pyi` & `mypy-boto3-license-manager-1.28.16/mypy_boto3_license_manager/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-1.28.15.post1/mypy_boto3_license_manager/type_defs.py` & `mypy-boto3-license-manager-1.28.16/mypy_boto3_license_manager/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_license_manager.type_defs import AcceptGrantRequestRequestTypeDef
 
-    data: AcceptGrantRequestRequestTypeDef = {...}
+    data: AcceptGrantRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -155,38 +155,40 @@
     "ListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef",
     "ListResourceInventoryRequestListResourceInventoryPaginateTypeDef",
     "ListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef",
     "ListResourceInventoryResponseTypeDef",
     "ListTokensResponseTypeDef",
     "ProductInformationOutputTypeDef",
     "ProductInformationTypeDef",
+    "ReportContextUnionTypeDef",
     "ReportGeneratorTypeDef",
     "ListFailuresForLicenseConfigurationOperationsResponseTypeDef",
     "CreateLicenseRequestRequestTypeDef",
     "CreateLicenseVersionRequestRequestTypeDef",
     "GrantedLicenseTypeDef",
     "LicenseTypeDef",
     "GetGrantResponseTypeDef",
     "ListDistributedGrantsResponseTypeDef",
     "ListReceivedGrantsForOrganizationResponseTypeDef",
     "ListReceivedGrantsResponseTypeDef",
     "ListLicenseConversionTasksResponseTypeDef",
     "GetLicenseUsageResponseTypeDef",
     "GetLicenseConfigurationResponseTypeDef",
     "LicenseConfigurationTypeDef",
-    "CreateLicenseConfigurationRequestRequestTypeDef",
-    "UpdateLicenseConfigurationRequestRequestTypeDef",
+    "ProductInformationUnionTypeDef",
     "GetLicenseManagerReportGeneratorResponseTypeDef",
     "ListLicenseManagerReportGeneratorsResponseTypeDef",
     "ListReceivedLicensesForOrganizationResponseTypeDef",
     "ListReceivedLicensesResponseTypeDef",
     "GetLicenseResponseTypeDef",
     "ListLicenseVersionsResponseTypeDef",
     "ListLicensesResponseTypeDef",
     "ListLicenseConfigurationsResponseTypeDef",
+    "CreateLicenseConfigurationRequestRequestTypeDef",
+    "UpdateLicenseConfigurationRequestRequestTypeDef",
 )
 
 AcceptGrantRequestRequestTypeDef = TypedDict(
     "AcceptGrantRequestRequestTypeDef",
     {
         "GrantArn": str,
     },
@@ -1685,14 +1687,15 @@
     "ProductInformationTypeDef",
     {
         "ResourceType": str,
         "ProductInformationFilterList": Sequence[ProductInformationFilterTypeDef],
     },
 )
 
+ReportContextUnionTypeDef = Union[ReportContextTypeDef, ReportContextOutputTypeDef]
 ReportGeneratorTypeDef = TypedDict(
     "ReportGeneratorTypeDef",
     {
         "ReportGeneratorName": str,
         "ReportType": List[ReportTypeType],
         "ReportContext": ReportContextOutputTypeDef,
         "ReportFrequency": ReportFrequencyTypeDef,
@@ -1918,76 +1921,15 @@
         "ManagedResourceSummaryList": List[ManagedResourceSummaryTypeDef],
         "ProductInformationList": List[ProductInformationOutputTypeDef],
         "AutomatedDiscoveryInformation": AutomatedDiscoveryInformationTypeDef,
     },
     total=False,
 )
 
-_RequiredCreateLicenseConfigurationRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateLicenseConfigurationRequestRequestTypeDef",
-    {
-        "Name": str,
-        "LicenseCountingType": LicenseCountingTypeType,
-    },
-)
-_OptionalCreateLicenseConfigurationRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateLicenseConfigurationRequestRequestTypeDef",
-    {
-        "Description": str,
-        "LicenseCount": int,
-        "LicenseCountHardLimit": bool,
-        "LicenseRules": Sequence[str],
-        "Tags": Sequence[TagTypeDef],
-        "DisassociateWhenNotFound": bool,
-        "ProductInformationList": Sequence[
-            Union[ProductInformationTypeDef, ProductInformationOutputTypeDef]
-        ],
-    },
-    total=False,
-)
-
-
-class CreateLicenseConfigurationRequestRequestTypeDef(
-    _RequiredCreateLicenseConfigurationRequestRequestTypeDef,
-    _OptionalCreateLicenseConfigurationRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredUpdateLicenseConfigurationRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateLicenseConfigurationRequestRequestTypeDef",
-    {
-        "LicenseConfigurationArn": str,
-    },
-)
-_OptionalUpdateLicenseConfigurationRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateLicenseConfigurationRequestRequestTypeDef",
-    {
-        "LicenseConfigurationStatus": LicenseConfigurationStatusType,
-        "LicenseRules": Sequence[str],
-        "LicenseCount": int,
-        "LicenseCountHardLimit": bool,
-        "Name": str,
-        "Description": str,
-        "ProductInformationList": Sequence[
-            Union[ProductInformationTypeDef, ProductInformationOutputTypeDef]
-        ],
-        "DisassociateWhenNotFound": bool,
-    },
-    total=False,
-)
-
-
-class UpdateLicenseConfigurationRequestRequestTypeDef(
-    _RequiredUpdateLicenseConfigurationRequestRequestTypeDef,
-    _OptionalUpdateLicenseConfigurationRequestRequestTypeDef,
-):
-    pass
-
-
+ProductInformationUnionTypeDef = Union[ProductInformationTypeDef, ProductInformationOutputTypeDef]
 GetLicenseManagerReportGeneratorResponseTypeDef = TypedDict(
     "GetLicenseManagerReportGeneratorResponseTypeDef",
     {
         "ReportGenerator": ReportGeneratorTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2049,7 +1991,64 @@
     "ListLicenseConfigurationsResponseTypeDef",
     {
         "LicenseConfigurations": List[LicenseConfigurationTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+
+_RequiredCreateLicenseConfigurationRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateLicenseConfigurationRequestRequestTypeDef",
+    {
+        "Name": str,
+        "LicenseCountingType": LicenseCountingTypeType,
+    },
+)
+_OptionalCreateLicenseConfigurationRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateLicenseConfigurationRequestRequestTypeDef",
+    {
+        "Description": str,
+        "LicenseCount": int,
+        "LicenseCountHardLimit": bool,
+        "LicenseRules": Sequence[str],
+        "Tags": Sequence[TagTypeDef],
+        "DisassociateWhenNotFound": bool,
+        "ProductInformationList": Sequence[ProductInformationUnionTypeDef],
+    },
+    total=False,
+)
+
+
+class CreateLicenseConfigurationRequestRequestTypeDef(
+    _RequiredCreateLicenseConfigurationRequestRequestTypeDef,
+    _OptionalCreateLicenseConfigurationRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredUpdateLicenseConfigurationRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateLicenseConfigurationRequestRequestTypeDef",
+    {
+        "LicenseConfigurationArn": str,
+    },
+)
+_OptionalUpdateLicenseConfigurationRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateLicenseConfigurationRequestRequestTypeDef",
+    {
+        "LicenseConfigurationStatus": LicenseConfigurationStatusType,
+        "LicenseRules": Sequence[str],
+        "LicenseCount": int,
+        "LicenseCountHardLimit": bool,
+        "Name": str,
+        "Description": str,
+        "ProductInformationList": Sequence[ProductInformationUnionTypeDef],
+        "DisassociateWhenNotFound": bool,
+    },
+    total=False,
+)
+
+
+class UpdateLicenseConfigurationRequestRequestTypeDef(
+    _RequiredUpdateLicenseConfigurationRequestRequestTypeDef,
+    _OptionalUpdateLicenseConfigurationRequestRequestTypeDef,
+):
+    pass
```

### Comparing `mypy-boto3-license-manager-1.28.15.post1/mypy_boto3_license_manager/type_defs.pyi` & `mypy-boto3-license-manager-1.28.16/mypy_boto3_license_manager/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_license_manager.type_defs import AcceptGrantRequestRequestTypeDef
 
-    data: AcceptGrantRequestRequestTypeDef = {...}
+    data: AcceptGrantRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -154,38 +154,40 @@
     "ListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef",
     "ListResourceInventoryRequestListResourceInventoryPaginateTypeDef",
     "ListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef",
     "ListResourceInventoryResponseTypeDef",
     "ListTokensResponseTypeDef",
     "ProductInformationOutputTypeDef",
     "ProductInformationTypeDef",
+    "ReportContextUnionTypeDef",
     "ReportGeneratorTypeDef",
     "ListFailuresForLicenseConfigurationOperationsResponseTypeDef",
     "CreateLicenseRequestRequestTypeDef",
     "CreateLicenseVersionRequestRequestTypeDef",
     "GrantedLicenseTypeDef",
     "LicenseTypeDef",
     "GetGrantResponseTypeDef",
     "ListDistributedGrantsResponseTypeDef",
     "ListReceivedGrantsForOrganizationResponseTypeDef",
     "ListReceivedGrantsResponseTypeDef",
     "ListLicenseConversionTasksResponseTypeDef",
     "GetLicenseUsageResponseTypeDef",
     "GetLicenseConfigurationResponseTypeDef",
     "LicenseConfigurationTypeDef",
-    "CreateLicenseConfigurationRequestRequestTypeDef",
-    "UpdateLicenseConfigurationRequestRequestTypeDef",
+    "ProductInformationUnionTypeDef",
     "GetLicenseManagerReportGeneratorResponseTypeDef",
     "ListLicenseManagerReportGeneratorsResponseTypeDef",
     "ListReceivedLicensesForOrganizationResponseTypeDef",
     "ListReceivedLicensesResponseTypeDef",
     "GetLicenseResponseTypeDef",
     "ListLicenseVersionsResponseTypeDef",
     "ListLicensesResponseTypeDef",
     "ListLicenseConfigurationsResponseTypeDef",
+    "CreateLicenseConfigurationRequestRequestTypeDef",
+    "UpdateLicenseConfigurationRequestRequestTypeDef",
 )
 
 AcceptGrantRequestRequestTypeDef = TypedDict(
     "AcceptGrantRequestRequestTypeDef",
     {
         "GrantArn": str,
     },
@@ -1620,14 +1622,15 @@
     "ProductInformationTypeDef",
     {
         "ResourceType": str,
         "ProductInformationFilterList": Sequence[ProductInformationFilterTypeDef],
     },
 )
 
+ReportContextUnionTypeDef = Union[ReportContextTypeDef, ReportContextOutputTypeDef]
 ReportGeneratorTypeDef = TypedDict(
     "ReportGeneratorTypeDef",
     {
         "ReportGeneratorName": str,
         "ReportType": List[ReportTypeType],
         "ReportContext": ReportContextOutputTypeDef,
         "ReportFrequency": ReportFrequencyTypeDef,
@@ -1849,72 +1852,15 @@
         "ManagedResourceSummaryList": List[ManagedResourceSummaryTypeDef],
         "ProductInformationList": List[ProductInformationOutputTypeDef],
         "AutomatedDiscoveryInformation": AutomatedDiscoveryInformationTypeDef,
     },
     total=False,
 )
 
-_RequiredCreateLicenseConfigurationRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateLicenseConfigurationRequestRequestTypeDef",
-    {
-        "Name": str,
-        "LicenseCountingType": LicenseCountingTypeType,
-    },
-)
-_OptionalCreateLicenseConfigurationRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateLicenseConfigurationRequestRequestTypeDef",
-    {
-        "Description": str,
-        "LicenseCount": int,
-        "LicenseCountHardLimit": bool,
-        "LicenseRules": Sequence[str],
-        "Tags": Sequence[TagTypeDef],
-        "DisassociateWhenNotFound": bool,
-        "ProductInformationList": Sequence[
-            Union[ProductInformationTypeDef, ProductInformationOutputTypeDef]
-        ],
-    },
-    total=False,
-)
-
-class CreateLicenseConfigurationRequestRequestTypeDef(
-    _RequiredCreateLicenseConfigurationRequestRequestTypeDef,
-    _OptionalCreateLicenseConfigurationRequestRequestTypeDef,
-):
-    pass
-
-_RequiredUpdateLicenseConfigurationRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateLicenseConfigurationRequestRequestTypeDef",
-    {
-        "LicenseConfigurationArn": str,
-    },
-)
-_OptionalUpdateLicenseConfigurationRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateLicenseConfigurationRequestRequestTypeDef",
-    {
-        "LicenseConfigurationStatus": LicenseConfigurationStatusType,
-        "LicenseRules": Sequence[str],
-        "LicenseCount": int,
-        "LicenseCountHardLimit": bool,
-        "Name": str,
-        "Description": str,
-        "ProductInformationList": Sequence[
-            Union[ProductInformationTypeDef, ProductInformationOutputTypeDef]
-        ],
-        "DisassociateWhenNotFound": bool,
-    },
-    total=False,
-)
-
-class UpdateLicenseConfigurationRequestRequestTypeDef(
-    _RequiredUpdateLicenseConfigurationRequestRequestTypeDef,
-    _OptionalUpdateLicenseConfigurationRequestRequestTypeDef,
-):
-    pass
-
+ProductInformationUnionTypeDef = Union[ProductInformationTypeDef, ProductInformationOutputTypeDef]
 GetLicenseManagerReportGeneratorResponseTypeDef = TypedDict(
     "GetLicenseManagerReportGeneratorResponseTypeDef",
     {
         "ReportGenerator": ReportGeneratorTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1976,7 +1922,61 @@
     "ListLicenseConfigurationsResponseTypeDef",
     {
         "LicenseConfigurations": List[LicenseConfigurationTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+
+_RequiredCreateLicenseConfigurationRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateLicenseConfigurationRequestRequestTypeDef",
+    {
+        "Name": str,
+        "LicenseCountingType": LicenseCountingTypeType,
+    },
+)
+_OptionalCreateLicenseConfigurationRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateLicenseConfigurationRequestRequestTypeDef",
+    {
+        "Description": str,
+        "LicenseCount": int,
+        "LicenseCountHardLimit": bool,
+        "LicenseRules": Sequence[str],
+        "Tags": Sequence[TagTypeDef],
+        "DisassociateWhenNotFound": bool,
+        "ProductInformationList": Sequence[ProductInformationUnionTypeDef],
+    },
+    total=False,
+)
+
+class CreateLicenseConfigurationRequestRequestTypeDef(
+    _RequiredCreateLicenseConfigurationRequestRequestTypeDef,
+    _OptionalCreateLicenseConfigurationRequestRequestTypeDef,
+):
+    pass
+
+_RequiredUpdateLicenseConfigurationRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateLicenseConfigurationRequestRequestTypeDef",
+    {
+        "LicenseConfigurationArn": str,
+    },
+)
+_OptionalUpdateLicenseConfigurationRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateLicenseConfigurationRequestRequestTypeDef",
+    {
+        "LicenseConfigurationStatus": LicenseConfigurationStatusType,
+        "LicenseRules": Sequence[str],
+        "LicenseCount": int,
+        "LicenseCountHardLimit": bool,
+        "Name": str,
+        "Description": str,
+        "ProductInformationList": Sequence[ProductInformationUnionTypeDef],
+        "DisassociateWhenNotFound": bool,
+    },
+    total=False,
+)
+
+class UpdateLicenseConfigurationRequestRequestTypeDef(
+    _RequiredUpdateLicenseConfigurationRequestRequestTypeDef,
+    _OptionalUpdateLicenseConfigurationRequestRequestTypeDef,
+):
+    pass
```

### Comparing `mypy-boto3-license-manager-1.28.15.post1/mypy_boto3_license_manager.egg-info/PKG-INFO` & `mypy-boto3-license-manager-1.28.16/mypy_boto3_license_manager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-license-manager
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.LicenseManager 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.LicenseManager 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 license-manager type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 license-manager type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-license-manager.svg?color=blue)](https://pypi.org/project/mypy-boto3-license-manager)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-license-manager)](https://pepy.tech/project/mypy-boto3-license-manager)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LicenseManager 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager)
+[boto3.LicenseManager 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager)
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
 [mypy-boto3-license-manager docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager/).
 
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
@@ -354,20 +354,20 @@
 )
 
 
 def check_value(value: ActivationOverrideBehaviorType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_license_manager.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_license_manager.type_defs import (
     AcceptGrantRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     AutomatedDiscoveryInformationTypeDef,
     BorrowConfigurationTypeDef,
@@ -476,42 +476,44 @@
     ListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef,
     ListResourceInventoryRequestListResourceInventoryPaginateTypeDef,
     ListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef,
     ListResourceInventoryResponseTypeDef,
     ListTokensResponseTypeDef,
     ProductInformationOutputTypeDef,
     ProductInformationTypeDef,
+    ReportContextUnionTypeDef,
     ReportGeneratorTypeDef,
     ListFailuresForLicenseConfigurationOperationsResponseTypeDef,
     CreateLicenseRequestRequestTypeDef,
     CreateLicenseVersionRequestRequestTypeDef,
     GrantedLicenseTypeDef,
     LicenseTypeDef,
     GetGrantResponseTypeDef,
     ListDistributedGrantsResponseTypeDef,
     ListReceivedGrantsForOrganizationResponseTypeDef,
     ListReceivedGrantsResponseTypeDef,
     ListLicenseConversionTasksResponseTypeDef,
     GetLicenseUsageResponseTypeDef,
     GetLicenseConfigurationResponseTypeDef,
     LicenseConfigurationTypeDef,
-    CreateLicenseConfigurationRequestRequestTypeDef,
-    UpdateLicenseConfigurationRequestRequestTypeDef,
+    ProductInformationUnionTypeDef,
     GetLicenseManagerReportGeneratorResponseTypeDef,
     ListLicenseManagerReportGeneratorsResponseTypeDef,
     ListReceivedLicensesForOrganizationResponseTypeDef,
     ListReceivedLicensesResponseTypeDef,
     GetLicenseResponseTypeDef,
     ListLicenseVersionsResponseTypeDef,
     ListLicensesResponseTypeDef,
     ListLicenseConfigurationsResponseTypeDef,
+    CreateLicenseConfigurationRequestRequestTypeDef,
+    UpdateLicenseConfigurationRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AcceptGrantRequestRequestTypeDef:
+def get_value() -> AcceptGrantRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-license-manager-1.28.15.post1/mypy_boto3_license_manager.egg-info/SOURCES.txt` & `mypy-boto3-license-manager-1.28.16/mypy_boto3_license_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-1.28.15.post1/setup.py` & `mypy-boto3-license-manager-1.28.16/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-license-manager",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_license_manager"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.LicenseManager 1.28.15 service generated with"
-        " mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.LicenseManager 1.28.16 service generated with"
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
-    keywords="boto3 license-manager type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 license-manager type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_license_manager": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

