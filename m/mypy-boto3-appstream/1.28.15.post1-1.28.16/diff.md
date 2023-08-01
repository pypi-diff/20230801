# Comparing `tmp/mypy-boto3-appstream-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-appstream-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-appstream-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:31 2023, max compression
+gzip compressed data, was "mypy-boto3-appstream-1.28.16.tar", last modified: Tue Aug  1 11:36:11 2023, max compression
```

## Comparing `mypy-boto3-appstream-1.28.15.post1.tar` & `mypy-boto3-appstream-1.28.16.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:31.245008 mypy-boto3-appstream-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:38:29.000000 mypy-boto3-appstream-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    23483 2023-07-29 10:02:31.245008 mypy-boto3-appstream-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21982 2023-07-29 09:38:29.000000 mypy-boto3-appstream-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:31.241008 mypy-boto3-appstream-1.28.15.post1/mypy_boto3_appstream/
--rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-07-29 09:38:29.000000 mypy-boto3-appstream-1.28.15.post1/mypy_boto3_appstream/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-07-29 09:38:29.000000 mypy-boto3-appstream-1.28.15.post1/mypy_boto3_appstream/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-29 09:38:29.000000 mypy-boto3-appstream-1.28.15.post1/mypy_boto3_appstream/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    58261 2023-07-29 09:38:29.000000 mypy-boto3-appstream-1.28.15.post1/mypy_boto3_appstream/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    58167 2023-07-29 09:38:29.000000 mypy-boto3-appstream-1.28.15.post1/mypy_boto3_appstream/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14966 2023-07-29 09:38:30.000000 mypy-boto3-appstream-1.28.15.post1/mypy_boto3_appstream/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14964 2023-07-29 09:38:29.000000 mypy-boto3-appstream-1.28.15.post1/mypy_boto3_appstream/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12301 2023-07-29 09:38:29.000000 mypy-boto3-appstream-1.28.15.post1/mypy_boto3_appstream/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12289 2023-07-29 09:38:29.000000 mypy-boto3-appstream-1.28.15.post1/mypy_boto3_appstream/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:38:29.000000 mypy-boto3-appstream-1.28.15.post1/mypy_boto3_appstream/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    70476 2023-07-29 09:38:32.000000 mypy-boto3-appstream-1.28.15.post1/mypy_boto3_appstream/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    70377 2023-07-29 09:38:31.000000 mypy-boto3-appstream-1.28.15.post1/mypy_boto3_appstream/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:38:29.000000 mypy-boto3-appstream-1.28.15.post1/mypy_boto3_appstream/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-07-29 09:38:29.000000 mypy-boto3-appstream-1.28.15.post1/mypy_boto3_appstream/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-07-29 09:38:29.000000 mypy-boto3-appstream-1.28.15.post1/mypy_boto3_appstream/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:31.245008 mypy-boto3-appstream-1.28.15.post1/mypy_boto3_appstream.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    23483 2023-07-29 10:02:30.000000 mypy-boto3-appstream-1.28.15.post1/mypy_boto3_appstream.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-29 10:02:31.000000 mypy-boto3-appstream-1.28.15.post1/mypy_boto3_appstream.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:30.000000 mypy-boto3-appstream-1.28.15.post1/mypy_boto3_appstream.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:30.000000 mypy-boto3-appstream-1.28.15.post1/mypy_boto3_appstream.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:30.000000 mypy-boto3-appstream-1.28.15.post1/mypy_boto3_appstream.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-29 10:02:30.000000 mypy-boto3-appstream-1.28.15.post1/mypy_boto3_appstream.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:31.245008 mypy-boto3-appstream-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-07-29 09:38:28.000000 mypy-boto3-appstream-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:11.948950 mypy-boto3-appstream-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:11:00.000000 mypy-boto3-appstream-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    23534 2023-08-01 11:36:11.944950 mypy-boto3-appstream-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22042 2023-08-01 11:11:00.000000 mypy-boto3-appstream-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:11.944950 mypy-boto3-appstream-1.28.16/mypy_boto3_appstream/
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-08-01 11:11:00.000000 mypy-boto3-appstream-1.28.16/mypy_boto3_appstream/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-08-01 11:11:00.000000 mypy-boto3-appstream-1.28.16/mypy_boto3_appstream/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-08-01 11:11:00.000000 mypy-boto3-appstream-1.28.16/mypy_boto3_appstream/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57961 2023-08-01 11:11:01.000000 mypy-boto3-appstream-1.28.16/mypy_boto3_appstream/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57867 2023-08-01 11:11:01.000000 mypy-boto3-appstream-1.28.16/mypy_boto3_appstream/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14966 2023-08-01 11:11:01.000000 mypy-boto3-appstream-1.28.16/mypy_boto3_appstream/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14964 2023-08-01 11:11:01.000000 mypy-boto3-appstream-1.28.16/mypy_boto3_appstream/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12301 2023-08-01 11:11:01.000000 mypy-boto3-appstream-1.28.16/mypy_boto3_appstream/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12289 2023-08-01 11:11:01.000000 mypy-boto3-appstream-1.28.16/mypy_boto3_appstream/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:11:00.000000 mypy-boto3-appstream-1.28.16/mypy_boto3_appstream/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    70594 2023-08-01 11:11:04.000000 mypy-boto3-appstream-1.28.16/mypy_boto3_appstream/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70495 2023-08-01 11:11:03.000000 mypy-boto3-appstream-1.28.16/mypy_boto3_appstream/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:11:00.000000 mypy-boto3-appstream-1.28.16/mypy_boto3_appstream/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-08-01 11:11:01.000000 mypy-boto3-appstream-1.28.16/mypy_boto3_appstream/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-08-01 11:11:01.000000 mypy-boto3-appstream-1.28.16/mypy_boto3_appstream/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:11.944950 mypy-boto3-appstream-1.28.16/mypy_boto3_appstream.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23534 2023-08-01 11:36:11.000000 mypy-boto3-appstream-1.28.16/mypy_boto3_appstream.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-08-01 11:36:11.000000 mypy-boto3-appstream-1.28.16/mypy_boto3_appstream.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:11.000000 mypy-boto3-appstream-1.28.16/mypy_boto3_appstream.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:11.000000 mypy-boto3-appstream-1.28.16/mypy_boto3_appstream.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:11.000000 mypy-boto3-appstream-1.28.16/mypy_boto3_appstream.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-01 11:36:11.000000 mypy-boto3-appstream-1.28.16/mypy_boto3_appstream.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:11.948950 mypy-boto3-appstream-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-08-01 11:11:00.000000 mypy-boto3-appstream-1.28.16/setup.py
```

### Comparing `mypy-boto3-appstream-1.28.15.post1/LICENSE` & `mypy-boto3-appstream-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appstream-1.28.15.post1/PKG-INFO` & `mypy-boto3-appstream-1.28.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-appstream
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.AppStream 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.AppStream 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 appstream type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 appstream type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-appstream.svg?color=blue)](https://pypi.org/project/mypy-boto3-appstream)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-appstream)](https://pepy.tech/project/mypy-boto3-appstream)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AppStream 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream)
+[boto3.AppStream 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream)
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
 [mypy-boto3-appstream docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/).
 
 See how it helps to find and fix potential bugs:
 
@@ -75,15 +75,15 @@
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Waiters annotations](#waiters-annotations)
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
@@ -406,20 +406,20 @@
 )
 
 
 def check_value(value: AccessEndpointTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_appstream.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_appstream.type_defs import (
     AccessEndpointTypeDef,
     AppBlockBuilderAppBlockAssociationTypeDef,
     AppBlockBuilderStateChangeReasonTypeDef,
     ResourceErrorTypeDef,
@@ -441,16 +441,14 @@
     CopyImageRequestRequestTypeDef,
     VpcConfigTypeDef,
     CreateAppBlockBuilderStreamingURLRequestRequestTypeDef,
     ServiceAccountCredentialsTypeDef,
     EntitlementAttributeTypeDef,
     DomainJoinInfoTypeDef,
     CreateImageBuilderStreamingURLRequestRequestTypeDef,
-    StorageConnectorOutputTypeDef,
-    StorageConnectorTypeDef,
     StreamingExperienceSettingsTypeDef,
     UserSettingTypeDef,
     CreateStreamingURLRequestRequestTypeDef,
     CreateUpdatedImageRequestRequestTypeDef,
     CreateUserRequestRequestTypeDef,
     DeleteAppBlockBuilderRequestRequestTypeDef,
     DeleteAppBlockRequestRequestTypeDef,
@@ -497,20 +495,22 @@
     ImageStateChangeReasonTypeDef,
     LastReportGenerationExecutionErrorTypeDef,
     ListAssociatedFleetsRequestRequestTypeDef,
     ListAssociatedStacksRequestRequestTypeDef,
     ListEntitledApplicationsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     StackErrorTypeDef,
+    StorageConnectorOutputTypeDef,
     StartAppBlockBuilderRequestRequestTypeDef,
     StartFleetRequestRequestTypeDef,
     StartImageBuilderRequestRequestTypeDef,
     StopAppBlockBuilderRequestRequestTypeDef,
     StopFleetRequestRequestTypeDef,
     StopImageBuilderRequestRequestTypeDef,
+    StorageConnectorTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     AppBlockBuilderTypeDef,
     ApplicationTypeDef,
     CreateApplicationRequestRequestTypeDef,
     ScriptDetailsTypeDef,
     UpdateApplicationRequestRequestTypeDef,
@@ -528,25 +528,24 @@
     ListTagsForResourceResponseTypeDef,
     BatchAssociateUserStackRequestRequestTypeDef,
     BatchDisassociateUserStackRequestRequestTypeDef,
     DescribeUserStackAssociationsResultTypeDef,
     UserStackAssociationErrorTypeDef,
     CreateAppBlockBuilderRequestRequestTypeDef,
     UpdateAppBlockBuilderRequestRequestTypeDef,
+    VpcConfigUnionTypeDef,
     CreateDirectoryConfigRequestRequestTypeDef,
     DirectoryConfigTypeDef,
     UpdateDirectoryConfigRequestRequestTypeDef,
     CreateEntitlementRequestRequestTypeDef,
     EntitlementTypeDef,
     UpdateEntitlementRequestRequestTypeDef,
     CreateFleetRequestRequestTypeDef,
     CreateImageBuilderRequestRequestTypeDef,
     UpdateFleetRequestRequestTypeDef,
-    CreateStackRequestRequestTypeDef,
-    UpdateStackRequestRequestTypeDef,
     DescribeDirectoryConfigsRequestDescribeDirectoryConfigsPaginateTypeDef,
     DescribeFleetsRequestDescribeFleetsPaginateTypeDef,
     DescribeImageBuildersRequestDescribeImageBuildersPaginateTypeDef,
     DescribeImagesRequestDescribeImagesPaginateTypeDef,
     DescribeSessionsRequestDescribeSessionsPaginateTypeDef,
     DescribeStacksRequestDescribeStacksPaginateTypeDef,
     DescribeUserStackAssociationsRequestDescribeUserStackAssociationsPaginateTypeDef,
@@ -560,14 +559,15 @@
     FleetTypeDef,
     ImageBuilderTypeDef,
     SessionTypeDef,
     SharedImagePermissionsTypeDef,
     UpdateImagePermissionsRequestRequestTypeDef,
     UsageReportSubscriptionTypeDef,
     StackTypeDef,
+    StorageConnectorUnionTypeDef,
     CreateAppBlockBuilderResultTypeDef,
     DescribeAppBlockBuildersResultTypeDef,
     StartAppBlockBuilderResultTypeDef,
     StopAppBlockBuilderResultTypeDef,
     UpdateAppBlockBuilderResultTypeDef,
     CreateApplicationResultTypeDef,
     DescribeApplicationsResultTypeDef,
@@ -593,23 +593,25 @@
     StopImageBuilderResultTypeDef,
     DescribeSessionsResultTypeDef,
     DescribeImagePermissionsResultTypeDef,
     DescribeUsageReportSubscriptionsResultTypeDef,
     CreateStackResultTypeDef,
     DescribeStacksResultTypeDef,
     UpdateStackResultTypeDef,
+    CreateStackRequestRequestTypeDef,
+    UpdateStackRequestRequestTypeDef,
     CreateUpdatedImageResultTypeDef,
     DeleteImageResultTypeDef,
     DescribeImagesResultTypeDef,
     CreateAppBlockResultTypeDef,
     DescribeAppBlocksResultTypeDef,
 )
 
 
-def get_structure() -> AccessEndpointTypeDef:
+def get_value() -> AccessEndpointTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-appstream-1.28.15.post1/README.md` & `mypy-boto3-appstream-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-appstream.svg?color=blue)](https://pypi.org/project/mypy-boto3-appstream)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-appstream)](https://pepy.tech/project/mypy-boto3-appstream)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AppStream 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream)
+[boto3.AppStream 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream)
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
 [mypy-boto3-appstream docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/).
 
 See how it helps to find and fix potential bugs:
 
@@ -43,15 +43,15 @@
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Waiters annotations](#waiters-annotations)
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
@@ -374,20 +374,20 @@
 )
 
 
 def check_value(value: AccessEndpointTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_appstream.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_appstream.type_defs import (
     AccessEndpointTypeDef,
     AppBlockBuilderAppBlockAssociationTypeDef,
     AppBlockBuilderStateChangeReasonTypeDef,
     ResourceErrorTypeDef,
@@ -409,16 +409,14 @@
     CopyImageRequestRequestTypeDef,
     VpcConfigTypeDef,
     CreateAppBlockBuilderStreamingURLRequestRequestTypeDef,
     ServiceAccountCredentialsTypeDef,
     EntitlementAttributeTypeDef,
     DomainJoinInfoTypeDef,
     CreateImageBuilderStreamingURLRequestRequestTypeDef,
-    StorageConnectorOutputTypeDef,
-    StorageConnectorTypeDef,
     StreamingExperienceSettingsTypeDef,
     UserSettingTypeDef,
     CreateStreamingURLRequestRequestTypeDef,
     CreateUpdatedImageRequestRequestTypeDef,
     CreateUserRequestRequestTypeDef,
     DeleteAppBlockBuilderRequestRequestTypeDef,
     DeleteAppBlockRequestRequestTypeDef,
@@ -465,20 +463,22 @@
     ImageStateChangeReasonTypeDef,
     LastReportGenerationExecutionErrorTypeDef,
     ListAssociatedFleetsRequestRequestTypeDef,
     ListAssociatedStacksRequestRequestTypeDef,
     ListEntitledApplicationsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     StackErrorTypeDef,
+    StorageConnectorOutputTypeDef,
     StartAppBlockBuilderRequestRequestTypeDef,
     StartFleetRequestRequestTypeDef,
     StartImageBuilderRequestRequestTypeDef,
     StopAppBlockBuilderRequestRequestTypeDef,
     StopFleetRequestRequestTypeDef,
     StopImageBuilderRequestRequestTypeDef,
+    StorageConnectorTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     AppBlockBuilderTypeDef,
     ApplicationTypeDef,
     CreateApplicationRequestRequestTypeDef,
     ScriptDetailsTypeDef,
     UpdateApplicationRequestRequestTypeDef,
@@ -496,25 +496,24 @@
     ListTagsForResourceResponseTypeDef,
     BatchAssociateUserStackRequestRequestTypeDef,
     BatchDisassociateUserStackRequestRequestTypeDef,
     DescribeUserStackAssociationsResultTypeDef,
     UserStackAssociationErrorTypeDef,
     CreateAppBlockBuilderRequestRequestTypeDef,
     UpdateAppBlockBuilderRequestRequestTypeDef,
+    VpcConfigUnionTypeDef,
     CreateDirectoryConfigRequestRequestTypeDef,
     DirectoryConfigTypeDef,
     UpdateDirectoryConfigRequestRequestTypeDef,
     CreateEntitlementRequestRequestTypeDef,
     EntitlementTypeDef,
     UpdateEntitlementRequestRequestTypeDef,
     CreateFleetRequestRequestTypeDef,
     CreateImageBuilderRequestRequestTypeDef,
     UpdateFleetRequestRequestTypeDef,
-    CreateStackRequestRequestTypeDef,
-    UpdateStackRequestRequestTypeDef,
     DescribeDirectoryConfigsRequestDescribeDirectoryConfigsPaginateTypeDef,
     DescribeFleetsRequestDescribeFleetsPaginateTypeDef,
     DescribeImageBuildersRequestDescribeImageBuildersPaginateTypeDef,
     DescribeImagesRequestDescribeImagesPaginateTypeDef,
     DescribeSessionsRequestDescribeSessionsPaginateTypeDef,
     DescribeStacksRequestDescribeStacksPaginateTypeDef,
     DescribeUserStackAssociationsRequestDescribeUserStackAssociationsPaginateTypeDef,
@@ -528,14 +527,15 @@
     FleetTypeDef,
     ImageBuilderTypeDef,
     SessionTypeDef,
     SharedImagePermissionsTypeDef,
     UpdateImagePermissionsRequestRequestTypeDef,
     UsageReportSubscriptionTypeDef,
     StackTypeDef,
+    StorageConnectorUnionTypeDef,
     CreateAppBlockBuilderResultTypeDef,
     DescribeAppBlockBuildersResultTypeDef,
     StartAppBlockBuilderResultTypeDef,
     StopAppBlockBuilderResultTypeDef,
     UpdateAppBlockBuilderResultTypeDef,
     CreateApplicationResultTypeDef,
     DescribeApplicationsResultTypeDef,
@@ -561,23 +561,25 @@
     StopImageBuilderResultTypeDef,
     DescribeSessionsResultTypeDef,
     DescribeImagePermissionsResultTypeDef,
     DescribeUsageReportSubscriptionsResultTypeDef,
     CreateStackResultTypeDef,
     DescribeStacksResultTypeDef,
     UpdateStackResultTypeDef,
+    CreateStackRequestRequestTypeDef,
+    UpdateStackRequestRequestTypeDef,
     CreateUpdatedImageResultTypeDef,
     DeleteImageResultTypeDef,
     DescribeImagesResultTypeDef,
     CreateAppBlockResultTypeDef,
     DescribeAppBlocksResultTypeDef,
 )
 
 
-def get_structure() -> AccessEndpointTypeDef:
+def get_value() -> AccessEndpointTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-appstream-1.28.15.post1/mypy_boto3_appstream/__init__.py` & `mypy-boto3-appstream-1.28.16/mypy_boto3_appstream/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appstream-1.28.15.post1/mypy_boto3_appstream/__init__.pyi` & `mypy-boto3-appstream-1.28.16/mypy_boto3_appstream/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appstream-1.28.15.post1/mypy_boto3_appstream/__main__.py` & `mypy-boto3-appstream-1.28.16/mypy_boto3_appstream/__main__.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.AppStream 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.AppStream 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream\nOther"
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

### Comparing `mypy-boto3-appstream-1.28.15.post1/mypy_boto3_appstream/client.py` & `mypy-boto3-appstream-1.28.16/mypy_boto3_appstream/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_appstream.client import AppStreamClient
 
     session = Session()
     client: AppStreamClient = session.client("appstream")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AppBlockBuilderAttributeType,
     ApplicationAttributeType,
     AppVisibilityType,
@@ -95,27 +95,25 @@
     S3LocationTypeDef,
     ScriptDetailsTypeDef,
     ServiceAccountCredentialsTypeDef,
     StartAppBlockBuilderResultTypeDef,
     StartImageBuilderResultTypeDef,
     StopAppBlockBuilderResultTypeDef,
     StopImageBuilderResultTypeDef,
-    StorageConnectorOutputTypeDef,
-    StorageConnectorTypeDef,
+    StorageConnectorUnionTypeDef,
     StreamingExperienceSettingsTypeDef,
     UpdateAppBlockBuilderResultTypeDef,
     UpdateApplicationResultTypeDef,
     UpdateDirectoryConfigResultTypeDef,
     UpdateEntitlementResultTypeDef,
     UpdateFleetResultTypeDef,
     UpdateStackResultTypeDef,
     UserSettingTypeDef,
     UserStackAssociationTypeDef,
-    VpcConfigOutputTypeDef,
-    VpcConfigTypeDef,
+    VpcConfigUnionTypeDef,
 )
 from .waiter import FleetStartedWaiter, FleetStoppedWaiter
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -278,15 +276,15 @@
 
     def create_app_block_builder(
         self,
         *,
         Name: str,
         Platform: Literal["WINDOWS_SERVER_2019"],
         InstanceType: str,
-        VpcConfig: Union[VpcConfigTypeDef, VpcConfigOutputTypeDef],
+        VpcConfig: VpcConfigUnionTypeDef,
         Description: str = ...,
         DisplayName: str = ...,
         Tags: Mapping[str, str] = ...,
         EnableDefaultInternetAccess: bool = ...,
         IamRoleArn: str = ...,
         AccessEndpoints: Sequence[AccessEndpointTypeDef] = ...
     ) -> CreateAppBlockBuilderResultTypeDef:
@@ -365,15 +363,15 @@
         *,
         Name: str,
         InstanceType: str,
         ImageName: str = ...,
         ImageArn: str = ...,
         FleetType: FleetTypeType = ...,
         ComputeCapacity: ComputeCapacityTypeDef = ...,
-        VpcConfig: Union[VpcConfigTypeDef, VpcConfigOutputTypeDef] = ...,
+        VpcConfig: VpcConfigUnionTypeDef = ...,
         MaxUserDurationInSeconds: int = ...,
         DisconnectTimeoutInSeconds: int = ...,
         Description: str = ...,
         DisplayName: str = ...,
         EnableDefaultInternetAccess: bool = ...,
         DomainJoinInfo: DomainJoinInfoTypeDef = ...,
         Tags: Mapping[str, str] = ...,
@@ -397,15 +395,15 @@
         *,
         Name: str,
         InstanceType: str,
         ImageName: str = ...,
         ImageArn: str = ...,
         Description: str = ...,
         DisplayName: str = ...,
-        VpcConfig: Union[VpcConfigTypeDef, VpcConfigOutputTypeDef] = ...,
+        VpcConfig: VpcConfigUnionTypeDef = ...,
         IamRoleArn: str = ...,
         EnableDefaultInternetAccess: bool = ...,
         DomainJoinInfo: DomainJoinInfoTypeDef = ...,
         AppstreamAgentVersion: str = ...,
         Tags: Mapping[str, str] = ...,
         AccessEndpoints: Sequence[AccessEndpointTypeDef] = ...
     ) -> CreateImageBuilderResultTypeDef:
@@ -428,17 +426,15 @@
 
     def create_stack(
         self,
         *,
         Name: str,
         Description: str = ...,
         DisplayName: str = ...,
-        StorageConnectors: Sequence[
-            Union[StorageConnectorTypeDef, StorageConnectorOutputTypeDef]
-        ] = ...,
+        StorageConnectors: Sequence[StorageConnectorUnionTypeDef] = ...,
         RedirectURL: str = ...,
         FeedbackURL: str = ...,
         UserSettings: Sequence[UserSettingTypeDef] = ...,
         ApplicationSettings: ApplicationSettingsTypeDef = ...,
         Tags: Mapping[str, str] = ...,
         AccessEndpoints: Sequence[AccessEndpointTypeDef] = ...,
         EmbedHostDomains: Sequence[str] = ...,
@@ -1003,15 +999,15 @@
         self,
         *,
         Name: str,
         Description: str = ...,
         DisplayName: str = ...,
         Platform: PlatformTypeType = ...,
         InstanceType: str = ...,
-        VpcConfig: Union[VpcConfigTypeDef, VpcConfigOutputTypeDef] = ...,
+        VpcConfig: VpcConfigUnionTypeDef = ...,
         EnableDefaultInternetAccess: bool = ...,
         IamRoleArn: str = ...,
         AccessEndpoints: Sequence[AccessEndpointTypeDef] = ...,
         AttributesToDelete: Sequence[AppBlockBuilderAttributeType] = ...
     ) -> UpdateAppBlockBuilderResultTypeDef:
         """
         Updates an app block builder.
@@ -1075,15 +1071,15 @@
         self,
         *,
         ImageName: str = ...,
         ImageArn: str = ...,
         Name: str = ...,
         InstanceType: str = ...,
         ComputeCapacity: ComputeCapacityTypeDef = ...,
-        VpcConfig: Union[VpcConfigTypeDef, VpcConfigOutputTypeDef] = ...,
+        VpcConfig: VpcConfigUnionTypeDef = ...,
         MaxUserDurationInSeconds: int = ...,
         DisconnectTimeoutInSeconds: int = ...,
         DeleteVpcConfig: bool = ...,
         Description: str = ...,
         DisplayName: str = ...,
         EnableDefaultInternetAccess: bool = ...,
         DomainJoinInfo: DomainJoinInfoTypeDef = ...,
@@ -1115,17 +1111,15 @@
 
     def update_stack(
         self,
         *,
         Name: str,
         DisplayName: str = ...,
         Description: str = ...,
-        StorageConnectors: Sequence[
-            Union[StorageConnectorTypeDef, StorageConnectorOutputTypeDef]
-        ] = ...,
+        StorageConnectors: Sequence[StorageConnectorUnionTypeDef] = ...,
         DeleteStorageConnectors: bool = ...,
         RedirectURL: str = ...,
         FeedbackURL: str = ...,
         AttributesToDelete: Sequence[StackAttributeType] = ...,
         UserSettings: Sequence[UserSettingTypeDef] = ...,
         ApplicationSettings: ApplicationSettingsTypeDef = ...,
         AccessEndpoints: Sequence[AccessEndpointTypeDef] = ...,
```

### Comparing `mypy-boto3-appstream-1.28.15.post1/mypy_boto3_appstream/client.pyi` & `mypy-boto3-appstream-1.28.16/mypy_boto3_appstream/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_appstream.client import AppStreamClient
 
     session = Session()
     client: AppStreamClient = session.client("appstream")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AppBlockBuilderAttributeType,
     ApplicationAttributeType,
     AppVisibilityType,
@@ -95,27 +95,25 @@
     S3LocationTypeDef,
     ScriptDetailsTypeDef,
     ServiceAccountCredentialsTypeDef,
     StartAppBlockBuilderResultTypeDef,
     StartImageBuilderResultTypeDef,
     StopAppBlockBuilderResultTypeDef,
     StopImageBuilderResultTypeDef,
-    StorageConnectorOutputTypeDef,
-    StorageConnectorTypeDef,
+    StorageConnectorUnionTypeDef,
     StreamingExperienceSettingsTypeDef,
     UpdateAppBlockBuilderResultTypeDef,
     UpdateApplicationResultTypeDef,
     UpdateDirectoryConfigResultTypeDef,
     UpdateEntitlementResultTypeDef,
     UpdateFleetResultTypeDef,
     UpdateStackResultTypeDef,
     UserSettingTypeDef,
     UserStackAssociationTypeDef,
-    VpcConfigOutputTypeDef,
-    VpcConfigTypeDef,
+    VpcConfigUnionTypeDef,
 )
 from .waiter import FleetStartedWaiter, FleetStoppedWaiter
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -263,15 +261,15 @@
         """
     def create_app_block_builder(
         self,
         *,
         Name: str,
         Platform: Literal["WINDOWS_SERVER_2019"],
         InstanceType: str,
-        VpcConfig: Union[VpcConfigTypeDef, VpcConfigOutputTypeDef],
+        VpcConfig: VpcConfigUnionTypeDef,
         Description: str = ...,
         DisplayName: str = ...,
         Tags: Mapping[str, str] = ...,
         EnableDefaultInternetAccess: bool = ...,
         IamRoleArn: str = ...,
         AccessEndpoints: Sequence[AccessEndpointTypeDef] = ...
     ) -> CreateAppBlockBuilderResultTypeDef:
@@ -345,15 +343,15 @@
         *,
         Name: str,
         InstanceType: str,
         ImageName: str = ...,
         ImageArn: str = ...,
         FleetType: FleetTypeType = ...,
         ComputeCapacity: ComputeCapacityTypeDef = ...,
-        VpcConfig: Union[VpcConfigTypeDef, VpcConfigOutputTypeDef] = ...,
+        VpcConfig: VpcConfigUnionTypeDef = ...,
         MaxUserDurationInSeconds: int = ...,
         DisconnectTimeoutInSeconds: int = ...,
         Description: str = ...,
         DisplayName: str = ...,
         EnableDefaultInternetAccess: bool = ...,
         DomainJoinInfo: DomainJoinInfoTypeDef = ...,
         Tags: Mapping[str, str] = ...,
@@ -376,15 +374,15 @@
         *,
         Name: str,
         InstanceType: str,
         ImageName: str = ...,
         ImageArn: str = ...,
         Description: str = ...,
         DisplayName: str = ...,
-        VpcConfig: Union[VpcConfigTypeDef, VpcConfigOutputTypeDef] = ...,
+        VpcConfig: VpcConfigUnionTypeDef = ...,
         IamRoleArn: str = ...,
         EnableDefaultInternetAccess: bool = ...,
         DomainJoinInfo: DomainJoinInfoTypeDef = ...,
         AppstreamAgentVersion: str = ...,
         Tags: Mapping[str, str] = ...,
         AccessEndpoints: Sequence[AccessEndpointTypeDef] = ...
     ) -> CreateImageBuilderResultTypeDef:
@@ -405,17 +403,15 @@
         """
     def create_stack(
         self,
         *,
         Name: str,
         Description: str = ...,
         DisplayName: str = ...,
-        StorageConnectors: Sequence[
-            Union[StorageConnectorTypeDef, StorageConnectorOutputTypeDef]
-        ] = ...,
+        StorageConnectors: Sequence[StorageConnectorUnionTypeDef] = ...,
         RedirectURL: str = ...,
         FeedbackURL: str = ...,
         UserSettings: Sequence[UserSettingTypeDef] = ...,
         ApplicationSettings: ApplicationSettingsTypeDef = ...,
         Tags: Mapping[str, str] = ...,
         AccessEndpoints: Sequence[AccessEndpointTypeDef] = ...,
         EmbedHostDomains: Sequence[str] = ...,
@@ -927,15 +923,15 @@
         self,
         *,
         Name: str,
         Description: str = ...,
         DisplayName: str = ...,
         Platform: PlatformTypeType = ...,
         InstanceType: str = ...,
-        VpcConfig: Union[VpcConfigTypeDef, VpcConfigOutputTypeDef] = ...,
+        VpcConfig: VpcConfigUnionTypeDef = ...,
         EnableDefaultInternetAccess: bool = ...,
         IamRoleArn: str = ...,
         AccessEndpoints: Sequence[AccessEndpointTypeDef] = ...,
         AttributesToDelete: Sequence[AppBlockBuilderAttributeType] = ...
     ) -> UpdateAppBlockBuilderResultTypeDef:
         """
         Updates an app block builder.
@@ -995,15 +991,15 @@
         self,
         *,
         ImageName: str = ...,
         ImageArn: str = ...,
         Name: str = ...,
         InstanceType: str = ...,
         ComputeCapacity: ComputeCapacityTypeDef = ...,
-        VpcConfig: Union[VpcConfigTypeDef, VpcConfigOutputTypeDef] = ...,
+        VpcConfig: VpcConfigUnionTypeDef = ...,
         MaxUserDurationInSeconds: int = ...,
         DisconnectTimeoutInSeconds: int = ...,
         DeleteVpcConfig: bool = ...,
         Description: str = ...,
         DisplayName: str = ...,
         EnableDefaultInternetAccess: bool = ...,
         DomainJoinInfo: DomainJoinInfoTypeDef = ...,
@@ -1033,17 +1029,15 @@
         """
     def update_stack(
         self,
         *,
         Name: str,
         DisplayName: str = ...,
         Description: str = ...,
-        StorageConnectors: Sequence[
-            Union[StorageConnectorTypeDef, StorageConnectorOutputTypeDef]
-        ] = ...,
+        StorageConnectors: Sequence[StorageConnectorUnionTypeDef] = ...,
         DeleteStorageConnectors: bool = ...,
         RedirectURL: str = ...,
         FeedbackURL: str = ...,
         AttributesToDelete: Sequence[StackAttributeType] = ...,
         UserSettings: Sequence[UserSettingTypeDef] = ...,
         ApplicationSettings: ApplicationSettingsTypeDef = ...,
         AccessEndpoints: Sequence[AccessEndpointTypeDef] = ...,
```

### Comparing `mypy-boto3-appstream-1.28.15.post1/mypy_boto3_appstream/literals.py` & `mypy-boto3-appstream-1.28.16/mypy_boto3_appstream/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appstream-1.28.15.post1/mypy_boto3_appstream/literals.pyi` & `mypy-boto3-appstream-1.28.16/mypy_boto3_appstream/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appstream-1.28.15.post1/mypy_boto3_appstream/paginator.py` & `mypy-boto3-appstream-1.28.16/mypy_boto3_appstream/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appstream-1.28.15.post1/mypy_boto3_appstream/paginator.pyi` & `mypy-boto3-appstream-1.28.16/mypy_boto3_appstream/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appstream-1.28.15.post1/mypy_boto3_appstream/type_defs.py` & `mypy-boto3-appstream-1.28.16/mypy_boto3_appstream/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_appstream.type_defs import AccessEndpointTypeDef
 
-    data: AccessEndpointTypeDef = {...}
+    data: AccessEndpointTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -81,16 +81,14 @@
     "CopyImageRequestRequestTypeDef",
     "VpcConfigTypeDef",
     "CreateAppBlockBuilderStreamingURLRequestRequestTypeDef",
     "ServiceAccountCredentialsTypeDef",
     "EntitlementAttributeTypeDef",
     "DomainJoinInfoTypeDef",
     "CreateImageBuilderStreamingURLRequestRequestTypeDef",
-    "StorageConnectorOutputTypeDef",
-    "StorageConnectorTypeDef",
     "StreamingExperienceSettingsTypeDef",
     "UserSettingTypeDef",
     "CreateStreamingURLRequestRequestTypeDef",
     "CreateUpdatedImageRequestRequestTypeDef",
     "CreateUserRequestRequestTypeDef",
     "DeleteAppBlockBuilderRequestRequestTypeDef",
     "DeleteAppBlockRequestRequestTypeDef",
@@ -137,20 +135,22 @@
     "ImageStateChangeReasonTypeDef",
     "LastReportGenerationExecutionErrorTypeDef",
     "ListAssociatedFleetsRequestRequestTypeDef",
     "ListAssociatedStacksRequestRequestTypeDef",
     "ListEntitledApplicationsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "StackErrorTypeDef",
+    "StorageConnectorOutputTypeDef",
     "StartAppBlockBuilderRequestRequestTypeDef",
     "StartFleetRequestRequestTypeDef",
     "StartImageBuilderRequestRequestTypeDef",
     "StopAppBlockBuilderRequestRequestTypeDef",
     "StopFleetRequestRequestTypeDef",
     "StopImageBuilderRequestRequestTypeDef",
+    "StorageConnectorTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "AppBlockBuilderTypeDef",
     "ApplicationTypeDef",
     "CreateApplicationRequestRequestTypeDef",
     "ScriptDetailsTypeDef",
     "UpdateApplicationRequestRequestTypeDef",
@@ -168,25 +168,24 @@
     "ListTagsForResourceResponseTypeDef",
     "BatchAssociateUserStackRequestRequestTypeDef",
     "BatchDisassociateUserStackRequestRequestTypeDef",
     "DescribeUserStackAssociationsResultTypeDef",
     "UserStackAssociationErrorTypeDef",
     "CreateAppBlockBuilderRequestRequestTypeDef",
     "UpdateAppBlockBuilderRequestRequestTypeDef",
+    "VpcConfigUnionTypeDef",
     "CreateDirectoryConfigRequestRequestTypeDef",
     "DirectoryConfigTypeDef",
     "UpdateDirectoryConfigRequestRequestTypeDef",
     "CreateEntitlementRequestRequestTypeDef",
     "EntitlementTypeDef",
     "UpdateEntitlementRequestRequestTypeDef",
     "CreateFleetRequestRequestTypeDef",
     "CreateImageBuilderRequestRequestTypeDef",
     "UpdateFleetRequestRequestTypeDef",
-    "CreateStackRequestRequestTypeDef",
-    "UpdateStackRequestRequestTypeDef",
     "DescribeDirectoryConfigsRequestDescribeDirectoryConfigsPaginateTypeDef",
     "DescribeFleetsRequestDescribeFleetsPaginateTypeDef",
     "DescribeImageBuildersRequestDescribeImageBuildersPaginateTypeDef",
     "DescribeImagesRequestDescribeImagesPaginateTypeDef",
     "DescribeSessionsRequestDescribeSessionsPaginateTypeDef",
     "DescribeStacksRequestDescribeStacksPaginateTypeDef",
     "DescribeUserStackAssociationsRequestDescribeUserStackAssociationsPaginateTypeDef",
@@ -200,14 +199,15 @@
     "FleetTypeDef",
     "ImageBuilderTypeDef",
     "SessionTypeDef",
     "SharedImagePermissionsTypeDef",
     "UpdateImagePermissionsRequestRequestTypeDef",
     "UsageReportSubscriptionTypeDef",
     "StackTypeDef",
+    "StorageConnectorUnionTypeDef",
     "CreateAppBlockBuilderResultTypeDef",
     "DescribeAppBlockBuildersResultTypeDef",
     "StartAppBlockBuilderResultTypeDef",
     "StopAppBlockBuilderResultTypeDef",
     "UpdateAppBlockBuilderResultTypeDef",
     "CreateApplicationResultTypeDef",
     "DescribeApplicationsResultTypeDef",
@@ -233,14 +233,16 @@
     "StopImageBuilderResultTypeDef",
     "DescribeSessionsResultTypeDef",
     "DescribeImagePermissionsResultTypeDef",
     "DescribeUsageReportSubscriptionsResultTypeDef",
     "CreateStackResultTypeDef",
     "DescribeStacksResultTypeDef",
     "UpdateStackResultTypeDef",
+    "CreateStackRequestRequestTypeDef",
+    "UpdateStackRequestRequestTypeDef",
     "CreateUpdatedImageResultTypeDef",
     "DeleteImageResultTypeDef",
     "DescribeImagesResultTypeDef",
     "CreateAppBlockResultTypeDef",
     "DescribeAppBlocksResultTypeDef",
 )
 
@@ -569,56 +571,14 @@
 class CreateImageBuilderStreamingURLRequestRequestTypeDef(
     _RequiredCreateImageBuilderStreamingURLRequestRequestTypeDef,
     _OptionalCreateImageBuilderStreamingURLRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredStorageConnectorOutputTypeDef = TypedDict(
-    "_RequiredStorageConnectorOutputTypeDef",
-    {
-        "ConnectorType": StorageConnectorTypeType,
-    },
-)
-_OptionalStorageConnectorOutputTypeDef = TypedDict(
-    "_OptionalStorageConnectorOutputTypeDef",
-    {
-        "ResourceIdentifier": str,
-        "Domains": List[str],
-    },
-    total=False,
-)
-
-
-class StorageConnectorOutputTypeDef(
-    _RequiredStorageConnectorOutputTypeDef, _OptionalStorageConnectorOutputTypeDef
-):
-    pass
-
-
-_RequiredStorageConnectorTypeDef = TypedDict(
-    "_RequiredStorageConnectorTypeDef",
-    {
-        "ConnectorType": StorageConnectorTypeType,
-    },
-)
-_OptionalStorageConnectorTypeDef = TypedDict(
-    "_OptionalStorageConnectorTypeDef",
-    {
-        "ResourceIdentifier": str,
-        "Domains": Sequence[str],
-    },
-    total=False,
-)
-
-
-class StorageConnectorTypeDef(_RequiredStorageConnectorTypeDef, _OptionalStorageConnectorTypeDef):
-    pass
-
-
 StreamingExperienceSettingsTypeDef = TypedDict(
     "StreamingExperienceSettingsTypeDef",
     {
         "PreferredProtocol": PreferredProtocolType,
     },
     total=False,
 )
@@ -1246,14 +1206,36 @@
     {
         "ErrorCode": StackErrorCodeType,
         "ErrorMessage": str,
     },
     total=False,
 )
 
+_RequiredStorageConnectorOutputTypeDef = TypedDict(
+    "_RequiredStorageConnectorOutputTypeDef",
+    {
+        "ConnectorType": StorageConnectorTypeType,
+    },
+)
+_OptionalStorageConnectorOutputTypeDef = TypedDict(
+    "_OptionalStorageConnectorOutputTypeDef",
+    {
+        "ResourceIdentifier": str,
+        "Domains": List[str],
+    },
+    total=False,
+)
+
+
+class StorageConnectorOutputTypeDef(
+    _RequiredStorageConnectorOutputTypeDef, _OptionalStorageConnectorOutputTypeDef
+):
+    pass
+
+
 StartAppBlockBuilderRequestRequestTypeDef = TypedDict(
     "StartAppBlockBuilderRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -1302,14 +1284,34 @@
 StopImageBuilderRequestRequestTypeDef = TypedDict(
     "StopImageBuilderRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
+_RequiredStorageConnectorTypeDef = TypedDict(
+    "_RequiredStorageConnectorTypeDef",
+    {
+        "ConnectorType": StorageConnectorTypeType,
+    },
+)
+_OptionalStorageConnectorTypeDef = TypedDict(
+    "_OptionalStorageConnectorTypeDef",
+    {
+        "ResourceIdentifier": str,
+        "Domains": Sequence[str],
+    },
+    total=False,
+)
+
+
+class StorageConnectorTypeDef(_RequiredStorageConnectorTypeDef, _OptionalStorageConnectorTypeDef):
+    pass
+
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -1647,14 +1649,15 @@
 class UpdateAppBlockBuilderRequestRequestTypeDef(
     _RequiredUpdateAppBlockBuilderRequestRequestTypeDef,
     _OptionalUpdateAppBlockBuilderRequestRequestTypeDef,
 ):
     pass
 
 
+VpcConfigUnionTypeDef = Union[VpcConfigTypeDef, VpcConfigOutputTypeDef]
 _RequiredCreateDirectoryConfigRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDirectoryConfigRequestRequestTypeDef",
     {
         "DirectoryName": str,
         "OrganizationalUnitDistinguishedNames": Sequence[str],
     },
 )
@@ -1890,81 +1893,14 @@
         "MaxConcurrentSessions": int,
         "UsbDeviceFilterStrings": Sequence[str],
         "SessionScriptS3Location": S3LocationTypeDef,
     },
     total=False,
 )
 
-_RequiredCreateStackRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateStackRequestRequestTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalCreateStackRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateStackRequestRequestTypeDef",
-    {
-        "Description": str,
-        "DisplayName": str,
-        "StorageConnectors": Sequence[
-            Union[StorageConnectorTypeDef, StorageConnectorOutputTypeDef]
-        ],
-        "RedirectURL": str,
-        "FeedbackURL": str,
-        "UserSettings": Sequence[UserSettingTypeDef],
-        "ApplicationSettings": ApplicationSettingsTypeDef,
-        "Tags": Mapping[str, str],
-        "AccessEndpoints": Sequence[AccessEndpointTypeDef],
-        "EmbedHostDomains": Sequence[str],
-        "StreamingExperienceSettings": StreamingExperienceSettingsTypeDef,
-    },
-    total=False,
-)
-
-
-class CreateStackRequestRequestTypeDef(
-    _RequiredCreateStackRequestRequestTypeDef, _OptionalCreateStackRequestRequestTypeDef
-):
-    pass
-
-
-_RequiredUpdateStackRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateStackRequestRequestTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalUpdateStackRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateStackRequestRequestTypeDef",
-    {
-        "DisplayName": str,
-        "Description": str,
-        "StorageConnectors": Sequence[
-            Union[StorageConnectorTypeDef, StorageConnectorOutputTypeDef]
-        ],
-        "DeleteStorageConnectors": bool,
-        "RedirectURL": str,
-        "FeedbackURL": str,
-        "AttributesToDelete": Sequence[StackAttributeType],
-        "UserSettings": Sequence[UserSettingTypeDef],
-        "ApplicationSettings": ApplicationSettingsTypeDef,
-        "AccessEndpoints": Sequence[AccessEndpointTypeDef],
-        "EmbedHostDomains": Sequence[str],
-        "StreamingExperienceSettings": StreamingExperienceSettingsTypeDef,
-    },
-    total=False,
-)
-
-
-class UpdateStackRequestRequestTypeDef(
-    _RequiredUpdateStackRequestRequestTypeDef, _OptionalUpdateStackRequestRequestTypeDef
-):
-    pass
-
-
 DescribeDirectoryConfigsRequestDescribeDirectoryConfigsPaginateTypeDef = TypedDict(
     "DescribeDirectoryConfigsRequestDescribeDirectoryConfigsPaginateTypeDef",
     {
         "DirectoryNames": Sequence[str],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -2306,14 +2242,15 @@
 )
 
 
 class StackTypeDef(_RequiredStackTypeDef, _OptionalStackTypeDef):
     pass
 
 
+StorageConnectorUnionTypeDef = Union[StorageConnectorTypeDef, StorageConnectorOutputTypeDef]
 CreateAppBlockBuilderResultTypeDef = TypedDict(
     "CreateAppBlockBuilderResultTypeDef",
     {
         "AppBlockBuilder": AppBlockBuilderTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2646,14 +2583,77 @@
     "UpdateStackResultTypeDef",
     {
         "Stack": StackTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredCreateStackRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateStackRequestRequestTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalCreateStackRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateStackRequestRequestTypeDef",
+    {
+        "Description": str,
+        "DisplayName": str,
+        "StorageConnectors": Sequence[StorageConnectorUnionTypeDef],
+        "RedirectURL": str,
+        "FeedbackURL": str,
+        "UserSettings": Sequence[UserSettingTypeDef],
+        "ApplicationSettings": ApplicationSettingsTypeDef,
+        "Tags": Mapping[str, str],
+        "AccessEndpoints": Sequence[AccessEndpointTypeDef],
+        "EmbedHostDomains": Sequence[str],
+        "StreamingExperienceSettings": StreamingExperienceSettingsTypeDef,
+    },
+    total=False,
+)
+
+
+class CreateStackRequestRequestTypeDef(
+    _RequiredCreateStackRequestRequestTypeDef, _OptionalCreateStackRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredUpdateStackRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateStackRequestRequestTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalUpdateStackRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateStackRequestRequestTypeDef",
+    {
+        "DisplayName": str,
+        "Description": str,
+        "StorageConnectors": Sequence[StorageConnectorUnionTypeDef],
+        "DeleteStorageConnectors": bool,
+        "RedirectURL": str,
+        "FeedbackURL": str,
+        "AttributesToDelete": Sequence[StackAttributeType],
+        "UserSettings": Sequence[UserSettingTypeDef],
+        "ApplicationSettings": ApplicationSettingsTypeDef,
+        "AccessEndpoints": Sequence[AccessEndpointTypeDef],
+        "EmbedHostDomains": Sequence[str],
+        "StreamingExperienceSettings": StreamingExperienceSettingsTypeDef,
+    },
+    total=False,
+)
+
+
+class UpdateStackRequestRequestTypeDef(
+    _RequiredUpdateStackRequestRequestTypeDef, _OptionalUpdateStackRequestRequestTypeDef
+):
+    pass
+
+
 CreateUpdatedImageResultTypeDef = TypedDict(
     "CreateUpdatedImageResultTypeDef",
     {
         "image": ImageTypeDef,
         "canUpdateImage": bool,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-appstream-1.28.15.post1/mypy_boto3_appstream/type_defs.pyi` & `mypy-boto3-appstream-1.28.16/mypy_boto3_appstream/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_appstream.type_defs import AccessEndpointTypeDef
 
-    data: AccessEndpointTypeDef = {...}
+    data: AccessEndpointTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -80,16 +80,14 @@
     "CopyImageRequestRequestTypeDef",
     "VpcConfigTypeDef",
     "CreateAppBlockBuilderStreamingURLRequestRequestTypeDef",
     "ServiceAccountCredentialsTypeDef",
     "EntitlementAttributeTypeDef",
     "DomainJoinInfoTypeDef",
     "CreateImageBuilderStreamingURLRequestRequestTypeDef",
-    "StorageConnectorOutputTypeDef",
-    "StorageConnectorTypeDef",
     "StreamingExperienceSettingsTypeDef",
     "UserSettingTypeDef",
     "CreateStreamingURLRequestRequestTypeDef",
     "CreateUpdatedImageRequestRequestTypeDef",
     "CreateUserRequestRequestTypeDef",
     "DeleteAppBlockBuilderRequestRequestTypeDef",
     "DeleteAppBlockRequestRequestTypeDef",
@@ -136,20 +134,22 @@
     "ImageStateChangeReasonTypeDef",
     "LastReportGenerationExecutionErrorTypeDef",
     "ListAssociatedFleetsRequestRequestTypeDef",
     "ListAssociatedStacksRequestRequestTypeDef",
     "ListEntitledApplicationsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "StackErrorTypeDef",
+    "StorageConnectorOutputTypeDef",
     "StartAppBlockBuilderRequestRequestTypeDef",
     "StartFleetRequestRequestTypeDef",
     "StartImageBuilderRequestRequestTypeDef",
     "StopAppBlockBuilderRequestRequestTypeDef",
     "StopFleetRequestRequestTypeDef",
     "StopImageBuilderRequestRequestTypeDef",
+    "StorageConnectorTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "AppBlockBuilderTypeDef",
     "ApplicationTypeDef",
     "CreateApplicationRequestRequestTypeDef",
     "ScriptDetailsTypeDef",
     "UpdateApplicationRequestRequestTypeDef",
@@ -167,25 +167,24 @@
     "ListTagsForResourceResponseTypeDef",
     "BatchAssociateUserStackRequestRequestTypeDef",
     "BatchDisassociateUserStackRequestRequestTypeDef",
     "DescribeUserStackAssociationsResultTypeDef",
     "UserStackAssociationErrorTypeDef",
     "CreateAppBlockBuilderRequestRequestTypeDef",
     "UpdateAppBlockBuilderRequestRequestTypeDef",
+    "VpcConfigUnionTypeDef",
     "CreateDirectoryConfigRequestRequestTypeDef",
     "DirectoryConfigTypeDef",
     "UpdateDirectoryConfigRequestRequestTypeDef",
     "CreateEntitlementRequestRequestTypeDef",
     "EntitlementTypeDef",
     "UpdateEntitlementRequestRequestTypeDef",
     "CreateFleetRequestRequestTypeDef",
     "CreateImageBuilderRequestRequestTypeDef",
     "UpdateFleetRequestRequestTypeDef",
-    "CreateStackRequestRequestTypeDef",
-    "UpdateStackRequestRequestTypeDef",
     "DescribeDirectoryConfigsRequestDescribeDirectoryConfigsPaginateTypeDef",
     "DescribeFleetsRequestDescribeFleetsPaginateTypeDef",
     "DescribeImageBuildersRequestDescribeImageBuildersPaginateTypeDef",
     "DescribeImagesRequestDescribeImagesPaginateTypeDef",
     "DescribeSessionsRequestDescribeSessionsPaginateTypeDef",
     "DescribeStacksRequestDescribeStacksPaginateTypeDef",
     "DescribeUserStackAssociationsRequestDescribeUserStackAssociationsPaginateTypeDef",
@@ -199,14 +198,15 @@
     "FleetTypeDef",
     "ImageBuilderTypeDef",
     "SessionTypeDef",
     "SharedImagePermissionsTypeDef",
     "UpdateImagePermissionsRequestRequestTypeDef",
     "UsageReportSubscriptionTypeDef",
     "StackTypeDef",
+    "StorageConnectorUnionTypeDef",
     "CreateAppBlockBuilderResultTypeDef",
     "DescribeAppBlockBuildersResultTypeDef",
     "StartAppBlockBuilderResultTypeDef",
     "StopAppBlockBuilderResultTypeDef",
     "UpdateAppBlockBuilderResultTypeDef",
     "CreateApplicationResultTypeDef",
     "DescribeApplicationsResultTypeDef",
@@ -232,14 +232,16 @@
     "StopImageBuilderResultTypeDef",
     "DescribeSessionsResultTypeDef",
     "DescribeImagePermissionsResultTypeDef",
     "DescribeUsageReportSubscriptionsResultTypeDef",
     "CreateStackResultTypeDef",
     "DescribeStacksResultTypeDef",
     "UpdateStackResultTypeDef",
+    "CreateStackRequestRequestTypeDef",
+    "UpdateStackRequestRequestTypeDef",
     "CreateUpdatedImageResultTypeDef",
     "DeleteImageResultTypeDef",
     "DescribeImagesResultTypeDef",
     "CreateAppBlockResultTypeDef",
     "DescribeAppBlocksResultTypeDef",
 )
 
@@ -552,52 +554,14 @@
 
 class CreateImageBuilderStreamingURLRequestRequestTypeDef(
     _RequiredCreateImageBuilderStreamingURLRequestRequestTypeDef,
     _OptionalCreateImageBuilderStreamingURLRequestRequestTypeDef,
 ):
     pass
 
-_RequiredStorageConnectorOutputTypeDef = TypedDict(
-    "_RequiredStorageConnectorOutputTypeDef",
-    {
-        "ConnectorType": StorageConnectorTypeType,
-    },
-)
-_OptionalStorageConnectorOutputTypeDef = TypedDict(
-    "_OptionalStorageConnectorOutputTypeDef",
-    {
-        "ResourceIdentifier": str,
-        "Domains": List[str],
-    },
-    total=False,
-)
-
-class StorageConnectorOutputTypeDef(
-    _RequiredStorageConnectorOutputTypeDef, _OptionalStorageConnectorOutputTypeDef
-):
-    pass
-
-_RequiredStorageConnectorTypeDef = TypedDict(
-    "_RequiredStorageConnectorTypeDef",
-    {
-        "ConnectorType": StorageConnectorTypeType,
-    },
-)
-_OptionalStorageConnectorTypeDef = TypedDict(
-    "_OptionalStorageConnectorTypeDef",
-    {
-        "ResourceIdentifier": str,
-        "Domains": Sequence[str],
-    },
-    total=False,
-)
-
-class StorageConnectorTypeDef(_RequiredStorageConnectorTypeDef, _OptionalStorageConnectorTypeDef):
-    pass
-
 StreamingExperienceSettingsTypeDef = TypedDict(
     "StreamingExperienceSettingsTypeDef",
     {
         "PreferredProtocol": PreferredProtocolType,
     },
     total=False,
 )
@@ -1203,14 +1167,34 @@
     {
         "ErrorCode": StackErrorCodeType,
         "ErrorMessage": str,
     },
     total=False,
 )
 
+_RequiredStorageConnectorOutputTypeDef = TypedDict(
+    "_RequiredStorageConnectorOutputTypeDef",
+    {
+        "ConnectorType": StorageConnectorTypeType,
+    },
+)
+_OptionalStorageConnectorOutputTypeDef = TypedDict(
+    "_OptionalStorageConnectorOutputTypeDef",
+    {
+        "ResourceIdentifier": str,
+        "Domains": List[str],
+    },
+    total=False,
+)
+
+class StorageConnectorOutputTypeDef(
+    _RequiredStorageConnectorOutputTypeDef, _OptionalStorageConnectorOutputTypeDef
+):
+    pass
+
 StartAppBlockBuilderRequestRequestTypeDef = TypedDict(
     "StartAppBlockBuilderRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -1257,14 +1241,32 @@
 StopImageBuilderRequestRequestTypeDef = TypedDict(
     "StopImageBuilderRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
+_RequiredStorageConnectorTypeDef = TypedDict(
+    "_RequiredStorageConnectorTypeDef",
+    {
+        "ConnectorType": StorageConnectorTypeType,
+    },
+)
+_OptionalStorageConnectorTypeDef = TypedDict(
+    "_OptionalStorageConnectorTypeDef",
+    {
+        "ResourceIdentifier": str,
+        "Domains": Sequence[str],
+    },
+    total=False,
+)
+
+class StorageConnectorTypeDef(_RequiredStorageConnectorTypeDef, _OptionalStorageConnectorTypeDef):
+    pass
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -1590,14 +1592,15 @@
 
 class UpdateAppBlockBuilderRequestRequestTypeDef(
     _RequiredUpdateAppBlockBuilderRequestRequestTypeDef,
     _OptionalUpdateAppBlockBuilderRequestRequestTypeDef,
 ):
     pass
 
+VpcConfigUnionTypeDef = Union[VpcConfigTypeDef, VpcConfigOutputTypeDef]
 _RequiredCreateDirectoryConfigRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDirectoryConfigRequestRequestTypeDef",
     {
         "DirectoryName": str,
         "OrganizationalUnitDistinguishedNames": Sequence[str],
     },
 )
@@ -1817,77 +1820,14 @@
         "MaxConcurrentSessions": int,
         "UsbDeviceFilterStrings": Sequence[str],
         "SessionScriptS3Location": S3LocationTypeDef,
     },
     total=False,
 )
 
-_RequiredCreateStackRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateStackRequestRequestTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalCreateStackRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateStackRequestRequestTypeDef",
-    {
-        "Description": str,
-        "DisplayName": str,
-        "StorageConnectors": Sequence[
-            Union[StorageConnectorTypeDef, StorageConnectorOutputTypeDef]
-        ],
-        "RedirectURL": str,
-        "FeedbackURL": str,
-        "UserSettings": Sequence[UserSettingTypeDef],
-        "ApplicationSettings": ApplicationSettingsTypeDef,
-        "Tags": Mapping[str, str],
-        "AccessEndpoints": Sequence[AccessEndpointTypeDef],
-        "EmbedHostDomains": Sequence[str],
-        "StreamingExperienceSettings": StreamingExperienceSettingsTypeDef,
-    },
-    total=False,
-)
-
-class CreateStackRequestRequestTypeDef(
-    _RequiredCreateStackRequestRequestTypeDef, _OptionalCreateStackRequestRequestTypeDef
-):
-    pass
-
-_RequiredUpdateStackRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateStackRequestRequestTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalUpdateStackRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateStackRequestRequestTypeDef",
-    {
-        "DisplayName": str,
-        "Description": str,
-        "StorageConnectors": Sequence[
-            Union[StorageConnectorTypeDef, StorageConnectorOutputTypeDef]
-        ],
-        "DeleteStorageConnectors": bool,
-        "RedirectURL": str,
-        "FeedbackURL": str,
-        "AttributesToDelete": Sequence[StackAttributeType],
-        "UserSettings": Sequence[UserSettingTypeDef],
-        "ApplicationSettings": ApplicationSettingsTypeDef,
-        "AccessEndpoints": Sequence[AccessEndpointTypeDef],
-        "EmbedHostDomains": Sequence[str],
-        "StreamingExperienceSettings": StreamingExperienceSettingsTypeDef,
-    },
-    total=False,
-)
-
-class UpdateStackRequestRequestTypeDef(
-    _RequiredUpdateStackRequestRequestTypeDef, _OptionalUpdateStackRequestRequestTypeDef
-):
-    pass
-
 DescribeDirectoryConfigsRequestDescribeDirectoryConfigsPaginateTypeDef = TypedDict(
     "DescribeDirectoryConfigsRequestDescribeDirectoryConfigsPaginateTypeDef",
     {
         "DirectoryNames": Sequence[str],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -2213,14 +2153,15 @@
     },
     total=False,
 )
 
 class StackTypeDef(_RequiredStackTypeDef, _OptionalStackTypeDef):
     pass
 
+StorageConnectorUnionTypeDef = Union[StorageConnectorTypeDef, StorageConnectorOutputTypeDef]
 CreateAppBlockBuilderResultTypeDef = TypedDict(
     "CreateAppBlockBuilderResultTypeDef",
     {
         "AppBlockBuilder": AppBlockBuilderTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2547,14 +2488,73 @@
     "UpdateStackResultTypeDef",
     {
         "Stack": StackTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredCreateStackRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateStackRequestRequestTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalCreateStackRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateStackRequestRequestTypeDef",
+    {
+        "Description": str,
+        "DisplayName": str,
+        "StorageConnectors": Sequence[StorageConnectorUnionTypeDef],
+        "RedirectURL": str,
+        "FeedbackURL": str,
+        "UserSettings": Sequence[UserSettingTypeDef],
+        "ApplicationSettings": ApplicationSettingsTypeDef,
+        "Tags": Mapping[str, str],
+        "AccessEndpoints": Sequence[AccessEndpointTypeDef],
+        "EmbedHostDomains": Sequence[str],
+        "StreamingExperienceSettings": StreamingExperienceSettingsTypeDef,
+    },
+    total=False,
+)
+
+class CreateStackRequestRequestTypeDef(
+    _RequiredCreateStackRequestRequestTypeDef, _OptionalCreateStackRequestRequestTypeDef
+):
+    pass
+
+_RequiredUpdateStackRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateStackRequestRequestTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalUpdateStackRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateStackRequestRequestTypeDef",
+    {
+        "DisplayName": str,
+        "Description": str,
+        "StorageConnectors": Sequence[StorageConnectorUnionTypeDef],
+        "DeleteStorageConnectors": bool,
+        "RedirectURL": str,
+        "FeedbackURL": str,
+        "AttributesToDelete": Sequence[StackAttributeType],
+        "UserSettings": Sequence[UserSettingTypeDef],
+        "ApplicationSettings": ApplicationSettingsTypeDef,
+        "AccessEndpoints": Sequence[AccessEndpointTypeDef],
+        "EmbedHostDomains": Sequence[str],
+        "StreamingExperienceSettings": StreamingExperienceSettingsTypeDef,
+    },
+    total=False,
+)
+
+class UpdateStackRequestRequestTypeDef(
+    _RequiredUpdateStackRequestRequestTypeDef, _OptionalUpdateStackRequestRequestTypeDef
+):
+    pass
+
 CreateUpdatedImageResultTypeDef = TypedDict(
     "CreateUpdatedImageResultTypeDef",
     {
         "image": ImageTypeDef,
         "canUpdateImage": bool,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-appstream-1.28.15.post1/mypy_boto3_appstream/waiter.py` & `mypy-boto3-appstream-1.28.16/mypy_boto3_appstream/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appstream-1.28.15.post1/mypy_boto3_appstream/waiter.pyi` & `mypy-boto3-appstream-1.28.16/mypy_boto3_appstream/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appstream-1.28.15.post1/mypy_boto3_appstream.egg-info/PKG-INFO` & `mypy-boto3-appstream-1.28.16/mypy_boto3_appstream.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-appstream
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.AppStream 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.AppStream 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 appstream type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 appstream type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-appstream.svg?color=blue)](https://pypi.org/project/mypy-boto3-appstream)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-appstream)](https://pepy.tech/project/mypy-boto3-appstream)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AppStream 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream)
+[boto3.AppStream 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#AppStream)
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
 [mypy-boto3-appstream docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/).
 
 See how it helps to find and fix potential bugs:
 
@@ -75,15 +75,15 @@
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Waiters annotations](#waiters-annotations)
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
@@ -406,20 +406,20 @@
 )
 
 
 def check_value(value: AccessEndpointTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_appstream.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_appstream.type_defs import (
     AccessEndpointTypeDef,
     AppBlockBuilderAppBlockAssociationTypeDef,
     AppBlockBuilderStateChangeReasonTypeDef,
     ResourceErrorTypeDef,
@@ -441,16 +441,14 @@
     CopyImageRequestRequestTypeDef,
     VpcConfigTypeDef,
     CreateAppBlockBuilderStreamingURLRequestRequestTypeDef,
     ServiceAccountCredentialsTypeDef,
     EntitlementAttributeTypeDef,
     DomainJoinInfoTypeDef,
     CreateImageBuilderStreamingURLRequestRequestTypeDef,
-    StorageConnectorOutputTypeDef,
-    StorageConnectorTypeDef,
     StreamingExperienceSettingsTypeDef,
     UserSettingTypeDef,
     CreateStreamingURLRequestRequestTypeDef,
     CreateUpdatedImageRequestRequestTypeDef,
     CreateUserRequestRequestTypeDef,
     DeleteAppBlockBuilderRequestRequestTypeDef,
     DeleteAppBlockRequestRequestTypeDef,
@@ -497,20 +495,22 @@
     ImageStateChangeReasonTypeDef,
     LastReportGenerationExecutionErrorTypeDef,
     ListAssociatedFleetsRequestRequestTypeDef,
     ListAssociatedStacksRequestRequestTypeDef,
     ListEntitledApplicationsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     StackErrorTypeDef,
+    StorageConnectorOutputTypeDef,
     StartAppBlockBuilderRequestRequestTypeDef,
     StartFleetRequestRequestTypeDef,
     StartImageBuilderRequestRequestTypeDef,
     StopAppBlockBuilderRequestRequestTypeDef,
     StopFleetRequestRequestTypeDef,
     StopImageBuilderRequestRequestTypeDef,
+    StorageConnectorTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     AppBlockBuilderTypeDef,
     ApplicationTypeDef,
     CreateApplicationRequestRequestTypeDef,
     ScriptDetailsTypeDef,
     UpdateApplicationRequestRequestTypeDef,
@@ -528,25 +528,24 @@
     ListTagsForResourceResponseTypeDef,
     BatchAssociateUserStackRequestRequestTypeDef,
     BatchDisassociateUserStackRequestRequestTypeDef,
     DescribeUserStackAssociationsResultTypeDef,
     UserStackAssociationErrorTypeDef,
     CreateAppBlockBuilderRequestRequestTypeDef,
     UpdateAppBlockBuilderRequestRequestTypeDef,
+    VpcConfigUnionTypeDef,
     CreateDirectoryConfigRequestRequestTypeDef,
     DirectoryConfigTypeDef,
     UpdateDirectoryConfigRequestRequestTypeDef,
     CreateEntitlementRequestRequestTypeDef,
     EntitlementTypeDef,
     UpdateEntitlementRequestRequestTypeDef,
     CreateFleetRequestRequestTypeDef,
     CreateImageBuilderRequestRequestTypeDef,
     UpdateFleetRequestRequestTypeDef,
-    CreateStackRequestRequestTypeDef,
-    UpdateStackRequestRequestTypeDef,
     DescribeDirectoryConfigsRequestDescribeDirectoryConfigsPaginateTypeDef,
     DescribeFleetsRequestDescribeFleetsPaginateTypeDef,
     DescribeImageBuildersRequestDescribeImageBuildersPaginateTypeDef,
     DescribeImagesRequestDescribeImagesPaginateTypeDef,
     DescribeSessionsRequestDescribeSessionsPaginateTypeDef,
     DescribeStacksRequestDescribeStacksPaginateTypeDef,
     DescribeUserStackAssociationsRequestDescribeUserStackAssociationsPaginateTypeDef,
@@ -560,14 +559,15 @@
     FleetTypeDef,
     ImageBuilderTypeDef,
     SessionTypeDef,
     SharedImagePermissionsTypeDef,
     UpdateImagePermissionsRequestRequestTypeDef,
     UsageReportSubscriptionTypeDef,
     StackTypeDef,
+    StorageConnectorUnionTypeDef,
     CreateAppBlockBuilderResultTypeDef,
     DescribeAppBlockBuildersResultTypeDef,
     StartAppBlockBuilderResultTypeDef,
     StopAppBlockBuilderResultTypeDef,
     UpdateAppBlockBuilderResultTypeDef,
     CreateApplicationResultTypeDef,
     DescribeApplicationsResultTypeDef,
@@ -593,23 +593,25 @@
     StopImageBuilderResultTypeDef,
     DescribeSessionsResultTypeDef,
     DescribeImagePermissionsResultTypeDef,
     DescribeUsageReportSubscriptionsResultTypeDef,
     CreateStackResultTypeDef,
     DescribeStacksResultTypeDef,
     UpdateStackResultTypeDef,
+    CreateStackRequestRequestTypeDef,
+    UpdateStackRequestRequestTypeDef,
     CreateUpdatedImageResultTypeDef,
     DeleteImageResultTypeDef,
     DescribeImagesResultTypeDef,
     CreateAppBlockResultTypeDef,
     DescribeAppBlocksResultTypeDef,
 )
 
 
-def get_structure() -> AccessEndpointTypeDef:
+def get_value() -> AccessEndpointTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-appstream-1.28.15.post1/mypy_boto3_appstream.egg-info/SOURCES.txt` & `mypy-boto3-appstream-1.28.16/mypy_boto3_appstream.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appstream-1.28.15.post1/setup.py` & `mypy-boto3-appstream-1.28.16/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-appstream",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_appstream"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.AppStream 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.2"
+        "Type annotations for boto3.AppStream 1.28.16 service generated with mypy-boto3-builder"
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
-    keywords="boto3 appstream type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 appstream type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_appstream": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appstream/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

