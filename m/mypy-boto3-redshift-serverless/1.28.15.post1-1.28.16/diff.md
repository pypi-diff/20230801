# Comparing `tmp/mypy-boto3-redshift-serverless-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-redshift-serverless-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-redshift-serverless-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:59 2023, max compression
+gzip compressed data, was "mypy-boto3-redshift-serverless-1.28.16.tar", last modified: Tue Aug  1 11:37:38 2023, max compression
```

## Comparing `mypy-boto3-redshift-serverless-1.28.15.post1.tar` & `mypy-boto3-redshift-serverless-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:59.005357 mypy-boto3-redshift-serverless-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:56:49.000000 mypy-boto3-redshift-serverless-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18345 2023-07-29 10:03:59.005357 mypy-boto3-redshift-serverless-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16805 2023-07-29 09:56:49.000000 mypy-boto3-redshift-serverless-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:59.005357 mypy-boto3-redshift-serverless-1.28.15.post1/mypy_boto3_redshift_serverless/
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-07-29 09:56:49.000000 mypy-boto3-redshift-serverless-1.28.15.post1/mypy_boto3_redshift_serverless/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-07-29 09:56:49.000000 mypy-boto3-redshift-serverless-1.28.15.post1/mypy_boto3_redshift_serverless/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-07-29 09:56:49.000000 mypy-boto3-redshift-serverless-1.28.15.post1/mypy_boto3_redshift_serverless/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32992 2023-07-29 09:56:49.000000 mypy-boto3-redshift-serverless-1.28.15.post1/mypy_boto3_redshift_serverless/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    32938 2023-07-29 09:56:49.000000 mypy-boto3-redshift-serverless-1.28.15.post1/mypy_boto3_redshift_serverless/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9686 2023-07-29 09:56:49.000000 mypy-boto3-redshift-serverless-1.28.15.post1/mypy_boto3_redshift_serverless/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9684 2023-07-29 09:56:49.000000 mypy-boto3-redshift-serverless-1.28.15.post1/mypy_boto3_redshift_serverless/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9409 2023-07-29 09:56:49.000000 mypy-boto3-redshift-serverless-1.28.15.post1/mypy_boto3_redshift_serverless/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9400 2023-07-29 09:56:49.000000 mypy-boto3-redshift-serverless-1.28.15.post1/mypy_boto3_redshift_serverless/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:56:49.000000 mypy-boto3-redshift-serverless-1.28.15.post1/mypy_boto3_redshift_serverless/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    33722 2023-07-29 09:56:50.000000 mypy-boto3-redshift-serverless-1.28.15.post1/mypy_boto3_redshift_serverless/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    33691 2023-07-29 09:56:50.000000 mypy-boto3-redshift-serverless-1.28.15.post1/mypy_boto3_redshift_serverless/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:56:49.000000 mypy-boto3-redshift-serverless-1.28.15.post1/mypy_boto3_redshift_serverless/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:59.005357 mypy-boto3-redshift-serverless-1.28.15.post1/mypy_boto3_redshift_serverless.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18345 2023-07-29 10:03:58.000000 mypy-boto3-redshift-serverless-1.28.15.post1/mypy_boto3_redshift_serverless.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-29 10:03:58.000000 mypy-boto3-redshift-serverless-1.28.15.post1/mypy_boto3_redshift_serverless.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:58.000000 mypy-boto3-redshift-serverless-1.28.15.post1/mypy_boto3_redshift_serverless.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:58.000000 mypy-boto3-redshift-serverless-1.28.15.post1/mypy_boto3_redshift_serverless.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:58.000000 mypy-boto3-redshift-serverless-1.28.15.post1/mypy_boto3_redshift_serverless.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-29 10:03:58.000000 mypy-boto3-redshift-serverless-1.28.15.post1/mypy_boto3_redshift_serverless.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:59.005357 mypy-boto3-redshift-serverless-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-07-29 09:56:49.000000 mypy-boto3-redshift-serverless-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:38.816774 mypy-boto3-redshift-serverless-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:30:10.000000 mypy-boto3-redshift-serverless-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18357 2023-08-01 11:37:38.816774 mypy-boto3-redshift-serverless-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16826 2023-08-01 11:30:10.000000 mypy-boto3-redshift-serverless-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:38.804774 mypy-boto3-redshift-serverless-1.28.16/mypy_boto3_redshift_serverless/
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-08-01 11:30:10.000000 mypy-boto3-redshift-serverless-1.28.16/mypy_boto3_redshift_serverless/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-08-01 11:30:10.000000 mypy-boto3-redshift-serverless-1.28.16/mypy_boto3_redshift_serverless/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-08-01 11:30:10.000000 mypy-boto3-redshift-serverless-1.28.16/mypy_boto3_redshift_serverless/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32961 2023-08-01 11:30:10.000000 mypy-boto3-redshift-serverless-1.28.16/mypy_boto3_redshift_serverless/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32907 2023-08-01 11:30:10.000000 mypy-boto3-redshift-serverless-1.28.16/mypy_boto3_redshift_serverless/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9686 2023-08-01 11:30:11.000000 mypy-boto3-redshift-serverless-1.28.16/mypy_boto3_redshift_serverless/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9684 2023-08-01 11:30:10.000000 mypy-boto3-redshift-serverless-1.28.16/mypy_boto3_redshift_serverless/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9378 2023-08-01 11:30:10.000000 mypy-boto3-redshift-serverless-1.28.16/mypy_boto3_redshift_serverless/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9369 2023-08-01 11:30:10.000000 mypy-boto3-redshift-serverless-1.28.16/mypy_boto3_redshift_serverless/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:30:10.000000 mypy-boto3-redshift-serverless-1.28.16/mypy_boto3_redshift_serverless/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    33752 2023-08-01 11:30:12.000000 mypy-boto3-redshift-serverless-1.28.16/mypy_boto3_redshift_serverless/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33721 2023-08-01 11:30:11.000000 mypy-boto3-redshift-serverless-1.28.16/mypy_boto3_redshift_serverless/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:30:10.000000 mypy-boto3-redshift-serverless-1.28.16/mypy_boto3_redshift_serverless/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:38.812774 mypy-boto3-redshift-serverless-1.28.16/mypy_boto3_redshift_serverless.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18357 2023-08-01 11:37:38.000000 mypy-boto3-redshift-serverless-1.28.16/mypy_boto3_redshift_serverless.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-08-01 11:37:38.000000 mypy-boto3-redshift-serverless-1.28.16/mypy_boto3_redshift_serverless.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:38.000000 mypy-boto3-redshift-serverless-1.28.16/mypy_boto3_redshift_serverless.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:38.000000 mypy-boto3-redshift-serverless-1.28.16/mypy_boto3_redshift_serverless.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:38.000000 mypy-boto3-redshift-serverless-1.28.16/mypy_boto3_redshift_serverless.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-01 11:37:38.000000 mypy-boto3-redshift-serverless-1.28.16/mypy_boto3_redshift_serverless.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:38.816774 mypy-boto3-redshift-serverless-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-08-01 11:30:10.000000 mypy-boto3-redshift-serverless-1.28.16/setup.py
```

### Comparing `mypy-boto3-redshift-serverless-1.28.15.post1/LICENSE` & `mypy-boto3-redshift-serverless-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-serverless-1.28.15.post1/PKG-INFO` & `mypy-boto3-redshift-serverless-1.28.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-redshift-serverless
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.RedshiftServerless 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.RedshiftServerless 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 redshift-serverless type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 redshift-serverless type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-redshift-serverless.svg?color=blue)](https://pypi.org/project/mypy-boto3-redshift-serverless)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-redshift-serverless)](https://pepy.tech/project/mypy-boto3-redshift-serverless)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.RedshiftServerless 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless)
+[boto3.RedshiftServerless 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless)
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
 [mypy-boto3-redshift-serverless docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/).
 
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
@@ -344,20 +344,20 @@
 )
 
 
 def check_value(value: ListEndpointAccessPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_redshift_serverless.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_redshift_serverless.type_defs import (
     ConfigParameterTypeDef,
     TagTypeDef,
     ResponseMetadataTypeDef,
     SnapshotTypeDef,
@@ -383,16 +383,15 @@
     GetTableRestoreStatusRequestRequestTypeDef,
     TableRestoreStatusTypeDef,
     GetUsageLimitRequestRequestTypeDef,
     GetWorkgroupRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     ListEndpointAccessRequestRequestTypeDef,
     ListNamespacesRequestRequestTypeDef,
-    ListRecoveryPointsRequestRequestTypeDef,
-    ListSnapshotsRequestRequestTypeDef,
+    TimestampTypeDef,
     ListTableRestoreStatusRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListUsageLimitsRequestRequestTypeDef,
     ListWorkgroupsRequestRequestTypeDef,
     NetworkInterfaceTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
     RestoreFromRecoveryPointRequestRequestTypeDef,
@@ -434,19 +433,21 @@
     GetResourcePolicyResponseTypeDef,
     PutResourcePolicyResponseTypeDef,
     GetTableRestoreStatusResponseTypeDef,
     ListTableRestoreStatusResponseTypeDef,
     RestoreTableFromSnapshotResponseTypeDef,
     ListEndpointAccessRequestListEndpointAccessPaginateTypeDef,
     ListNamespacesRequestListNamespacesPaginateTypeDef,
-    ListRecoveryPointsRequestListRecoveryPointsPaginateTypeDef,
-    ListSnapshotsRequestListSnapshotsPaginateTypeDef,
     ListTableRestoreStatusRequestListTableRestoreStatusPaginateTypeDef,
     ListUsageLimitsRequestListUsageLimitsPaginateTypeDef,
     ListWorkgroupsRequestListWorkgroupsPaginateTypeDef,
+    ListRecoveryPointsRequestListRecoveryPointsPaginateTypeDef,
+    ListRecoveryPointsRequestRequestTypeDef,
+    ListSnapshotsRequestListSnapshotsPaginateTypeDef,
+    ListSnapshotsRequestRequestTypeDef,
     VpcEndpointTypeDef,
     EndpointAccessTypeDef,
     EndpointTypeDef,
     CreateEndpointAccessResponseTypeDef,
     DeleteEndpointAccessResponseTypeDef,
     GetEndpointAccessResponseTypeDef,
     ListEndpointAccessResponseTypeDef,
@@ -456,15 +457,15 @@
     DeleteWorkgroupResponseTypeDef,
     GetWorkgroupResponseTypeDef,
     ListWorkgroupsResponseTypeDef,
     UpdateWorkgroupResponseTypeDef,
 )
 
 
-def get_structure() -> ConfigParameterTypeDef:
+def get_value() -> ConfigParameterTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-redshift-serverless-1.28.15.post1/README.md` & `mypy-boto3-redshift-serverless-1.28.16/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-redshift-serverless.svg?color=blue)](https://pypi.org/project/mypy-boto3-redshift-serverless)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-redshift-serverless)](https://pepy.tech/project/mypy-boto3-redshift-serverless)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.RedshiftServerless 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless)
+[boto3.RedshiftServerless 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless)
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
 [mypy-boto3-redshift-serverless docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/).
 
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
@@ -312,20 +312,20 @@
 )
 
 
 def check_value(value: ListEndpointAccessPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_redshift_serverless.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_redshift_serverless.type_defs import (
     ConfigParameterTypeDef,
     TagTypeDef,
     ResponseMetadataTypeDef,
     SnapshotTypeDef,
@@ -351,16 +351,15 @@
     GetTableRestoreStatusRequestRequestTypeDef,
     TableRestoreStatusTypeDef,
     GetUsageLimitRequestRequestTypeDef,
     GetWorkgroupRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     ListEndpointAccessRequestRequestTypeDef,
     ListNamespacesRequestRequestTypeDef,
-    ListRecoveryPointsRequestRequestTypeDef,
-    ListSnapshotsRequestRequestTypeDef,
+    TimestampTypeDef,
     ListTableRestoreStatusRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListUsageLimitsRequestRequestTypeDef,
     ListWorkgroupsRequestRequestTypeDef,
     NetworkInterfaceTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
     RestoreFromRecoveryPointRequestRequestTypeDef,
@@ -402,19 +401,21 @@
     GetResourcePolicyResponseTypeDef,
     PutResourcePolicyResponseTypeDef,
     GetTableRestoreStatusResponseTypeDef,
     ListTableRestoreStatusResponseTypeDef,
     RestoreTableFromSnapshotResponseTypeDef,
     ListEndpointAccessRequestListEndpointAccessPaginateTypeDef,
     ListNamespacesRequestListNamespacesPaginateTypeDef,
-    ListRecoveryPointsRequestListRecoveryPointsPaginateTypeDef,
-    ListSnapshotsRequestListSnapshotsPaginateTypeDef,
     ListTableRestoreStatusRequestListTableRestoreStatusPaginateTypeDef,
     ListUsageLimitsRequestListUsageLimitsPaginateTypeDef,
     ListWorkgroupsRequestListWorkgroupsPaginateTypeDef,
+    ListRecoveryPointsRequestListRecoveryPointsPaginateTypeDef,
+    ListRecoveryPointsRequestRequestTypeDef,
+    ListSnapshotsRequestListSnapshotsPaginateTypeDef,
+    ListSnapshotsRequestRequestTypeDef,
     VpcEndpointTypeDef,
     EndpointAccessTypeDef,
     EndpointTypeDef,
     CreateEndpointAccessResponseTypeDef,
     DeleteEndpointAccessResponseTypeDef,
     GetEndpointAccessResponseTypeDef,
     ListEndpointAccessResponseTypeDef,
@@ -424,15 +425,15 @@
     DeleteWorkgroupResponseTypeDef,
     GetWorkgroupResponseTypeDef,
     ListWorkgroupsResponseTypeDef,
     UpdateWorkgroupResponseTypeDef,
 )
 
 
-def get_structure() -> ConfigParameterTypeDef:
+def get_value() -> ConfigParameterTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-redshift-serverless-1.28.15.post1/mypy_boto3_redshift_serverless/__init__.py` & `mypy-boto3-redshift-serverless-1.28.16/mypy_boto3_redshift_serverless/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-serverless-1.28.15.post1/mypy_boto3_redshift_serverless/__init__.pyi` & `mypy-boto3-redshift-serverless-1.28.16/mypy_boto3_redshift_serverless/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-serverless-1.28.15.post1/mypy_boto3_redshift_serverless/__main__.py` & `mypy-boto3-redshift-serverless-1.28.16/mypy_boto3_redshift_serverless/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.RedshiftServerless 1.28.15\nVersion:        "
-        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.RedshiftServerless 1.28.16\nVersion:         1.28.16\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless//\nBoto3 docs: "
         "     https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless\nOther"
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

### Comparing `mypy-boto3-redshift-serverless-1.28.15.post1/mypy_boto3_redshift_serverless/client.py` & `mypy-boto3-redshift-serverless-1.28.16/mypy_boto3_redshift_serverless/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from mypy_boto3_redshift_serverless.client import RedshiftServerlessClient
 
     session = Session()
     client: RedshiftServerlessClient = session.client("redshift-serverless")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     LogExportType,
     UsageLimitBreachActionType,
     UsageLimitPeriodType,
@@ -65,14 +64,15 @@
     ListUsageLimitsResponseTypeDef,
     ListWorkgroupsResponseTypeDef,
     PutResourcePolicyResponseTypeDef,
     RestoreFromRecoveryPointResponseTypeDef,
     RestoreFromSnapshotResponseTypeDef,
     RestoreTableFromSnapshotResponseTypeDef,
     TagTypeDef,
+    TimestampTypeDef,
     UpdateEndpointAccessResponseTypeDef,
     UpdateNamespaceResponseTypeDef,
     UpdateSnapshotResponseTypeDef,
     UpdateUsageLimitResponseTypeDef,
     UpdateWorkgroupResponseTypeDef,
 )
 
@@ -413,38 +413,38 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Client.list_namespaces)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/client/#list_namespaces)
         """
 
     def list_recovery_points(
         self,
         *,
-        endTime: Union[datetime, str] = ...,
+        endTime: TimestampTypeDef = ...,
         maxResults: int = ...,
         namespaceArn: str = ...,
         namespaceName: str = ...,
         nextToken: str = ...,
-        startTime: Union[datetime, str] = ...
+        startTime: TimestampTypeDef = ...
     ) -> ListRecoveryPointsResponseTypeDef:
         """
         Returns an array of recovery points.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Client.list_recovery_points)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/client/#list_recovery_points)
         """
 
     def list_snapshots(
         self,
         *,
-        endTime: Union[datetime, str] = ...,
+        endTime: TimestampTypeDef = ...,
         maxResults: int = ...,
         namespaceArn: str = ...,
         namespaceName: str = ...,
         nextToken: str = ...,
         ownerAccount: str = ...,
-        startTime: Union[datetime, str] = ...
+        startTime: TimestampTypeDef = ...
     ) -> ListSnapshotsResponseTypeDef:
         """
         Returns a list of snapshots.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Client.list_snapshots)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/client/#list_snapshots)
         """
```

### Comparing `mypy-boto3-redshift-serverless-1.28.15.post1/mypy_boto3_redshift_serverless/client.pyi` & `mypy-boto3-redshift-serverless-1.28.16/mypy_boto3_redshift_serverless/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from mypy_boto3_redshift_serverless.client import RedshiftServerlessClient
 
     session = Session()
     client: RedshiftServerlessClient = session.client("redshift-serverless")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     LogExportType,
     UsageLimitBreachActionType,
     UsageLimitPeriodType,
@@ -65,14 +64,15 @@
     ListUsageLimitsResponseTypeDef,
     ListWorkgroupsResponseTypeDef,
     PutResourcePolicyResponseTypeDef,
     RestoreFromRecoveryPointResponseTypeDef,
     RestoreFromSnapshotResponseTypeDef,
     RestoreTableFromSnapshotResponseTypeDef,
     TagTypeDef,
+    TimestampTypeDef,
     UpdateEndpointAccessResponseTypeDef,
     UpdateNamespaceResponseTypeDef,
     UpdateSnapshotResponseTypeDef,
     UpdateUsageLimitResponseTypeDef,
     UpdateWorkgroupResponseTypeDef,
 )
 
@@ -382,37 +382,37 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Client.list_namespaces)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/client/#list_namespaces)
         """
     def list_recovery_points(
         self,
         *,
-        endTime: Union[datetime, str] = ...,
+        endTime: TimestampTypeDef = ...,
         maxResults: int = ...,
         namespaceArn: str = ...,
         namespaceName: str = ...,
         nextToken: str = ...,
-        startTime: Union[datetime, str] = ...
+        startTime: TimestampTypeDef = ...
     ) -> ListRecoveryPointsResponseTypeDef:
         """
         Returns an array of recovery points.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Client.list_recovery_points)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/client/#list_recovery_points)
         """
     def list_snapshots(
         self,
         *,
-        endTime: Union[datetime, str] = ...,
+        endTime: TimestampTypeDef = ...,
         maxResults: int = ...,
         namespaceArn: str = ...,
         namespaceName: str = ...,
         nextToken: str = ...,
         ownerAccount: str = ...,
-        startTime: Union[datetime, str] = ...
+        startTime: TimestampTypeDef = ...
     ) -> ListSnapshotsResponseTypeDef:
         """
         Returns a list of snapshots.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Client.list_snapshots)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/client/#list_snapshots)
         """
```

### Comparing `mypy-boto3-redshift-serverless-1.28.15.post1/mypy_boto3_redshift_serverless/literals.py` & `mypy-boto3-redshift-serverless-1.28.16/mypy_boto3_redshift_serverless/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-serverless-1.28.15.post1/mypy_boto3_redshift_serverless/literals.pyi` & `mypy-boto3-redshift-serverless-1.28.16/mypy_boto3_redshift_serverless/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-serverless-1.28.15.post1/mypy_boto3_redshift_serverless/paginator.py` & `mypy-boto3-redshift-serverless-1.28.16/mypy_boto3_redshift_serverless/paginator.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,29 +27,29 @@
     list_recovery_points_paginator: ListRecoveryPointsPaginator = client.get_paginator("list_recovery_points")
     list_snapshots_paginator: ListSnapshotsPaginator = client.get_paginator("list_snapshots")
     list_table_restore_status_paginator: ListTableRestoreStatusPaginator = client.get_paginator("list_table_restore_status")
     list_usage_limits_paginator: ListUsageLimitsPaginator = client.get_paginator("list_usage_limits")
     list_workgroups_paginator: ListWorkgroupsPaginator = client.get_paginator("list_workgroups")
     ```
 """
-from datetime import datetime
-from typing import Generic, Iterator, TypeVar, Union
+from typing import Generic, Iterator, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import UsageLimitUsageTypeType
 from .type_defs import (
     ListEndpointAccessResponseTypeDef,
     ListNamespacesResponseTypeDef,
     ListRecoveryPointsResponseTypeDef,
     ListSnapshotsResponseTypeDef,
     ListTableRestoreStatusResponseTypeDef,
     ListUsageLimitsResponseTypeDef,
     ListWorkgroupsResponseTypeDef,
     PaginatorConfigTypeDef,
+    TimestampTypeDef,
 )
 
 __all__ = (
     "ListEndpointAccessPaginator",
     "ListNamespacesPaginator",
     "ListRecoveryPointsPaginator",
     "ListSnapshotsPaginator",
@@ -108,18 +108,18 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Paginator.ListRecoveryPoints)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/paginators/#listrecoverypointspaginator)
     """
 
     def paginate(
         self,
         *,
-        endTime: Union[datetime, str] = ...,
+        endTime: TimestampTypeDef = ...,
         namespaceArn: str = ...,
         namespaceName: str = ...,
-        startTime: Union[datetime, str] = ...,
+        startTime: TimestampTypeDef = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRecoveryPointsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Paginator.ListRecoveryPoints.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/paginators/#listrecoverypointspaginator)
         """
 
@@ -129,19 +129,19 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Paginator.ListSnapshots)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/paginators/#listsnapshotspaginator)
     """
 
     def paginate(
         self,
         *,
-        endTime: Union[datetime, str] = ...,
+        endTime: TimestampTypeDef = ...,
         namespaceArn: str = ...,
         namespaceName: str = ...,
         ownerAccount: str = ...,
-        startTime: Union[datetime, str] = ...,
+        startTime: TimestampTypeDef = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSnapshotsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Paginator.ListSnapshots.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/paginators/#listsnapshotspaginator)
         """
```

### Comparing `mypy-boto3-redshift-serverless-1.28.15.post1/mypy_boto3_redshift_serverless/paginator.pyi` & `mypy-boto3-redshift-serverless-1.28.16/mypy_boto3_redshift_serverless/paginator.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -27,29 +27,29 @@
     list_recovery_points_paginator: ListRecoveryPointsPaginator = client.get_paginator("list_recovery_points")
     list_snapshots_paginator: ListSnapshotsPaginator = client.get_paginator("list_snapshots")
     list_table_restore_status_paginator: ListTableRestoreStatusPaginator = client.get_paginator("list_table_restore_status")
     list_usage_limits_paginator: ListUsageLimitsPaginator = client.get_paginator("list_usage_limits")
     list_workgroups_paginator: ListWorkgroupsPaginator = client.get_paginator("list_workgroups")
     ```
 """
-from datetime import datetime
-from typing import Generic, Iterator, TypeVar, Union
+from typing import Generic, Iterator, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import UsageLimitUsageTypeType
 from .type_defs import (
     ListEndpointAccessResponseTypeDef,
     ListNamespacesResponseTypeDef,
     ListRecoveryPointsResponseTypeDef,
     ListSnapshotsResponseTypeDef,
     ListTableRestoreStatusResponseTypeDef,
     ListUsageLimitsResponseTypeDef,
     ListWorkgroupsResponseTypeDef,
     PaginatorConfigTypeDef,
+    TimestampTypeDef,
 )
 
 __all__ = (
     "ListEndpointAccessPaginator",
     "ListNamespacesPaginator",
     "ListRecoveryPointsPaginator",
     "ListSnapshotsPaginator",
@@ -103,18 +103,18 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Paginator.ListRecoveryPoints)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/paginators/#listrecoverypointspaginator)
     """
 
     def paginate(
         self,
         *,
-        endTime: Union[datetime, str] = ...,
+        endTime: TimestampTypeDef = ...,
         namespaceArn: str = ...,
         namespaceName: str = ...,
-        startTime: Union[datetime, str] = ...,
+        startTime: TimestampTypeDef = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRecoveryPointsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Paginator.ListRecoveryPoints.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/paginators/#listrecoverypointspaginator)
         """
 
@@ -123,19 +123,19 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Paginator.ListSnapshots)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/paginators/#listsnapshotspaginator)
     """
 
     def paginate(
         self,
         *,
-        endTime: Union[datetime, str] = ...,
+        endTime: TimestampTypeDef = ...,
         namespaceArn: str = ...,
         namespaceName: str = ...,
         ownerAccount: str = ...,
-        startTime: Union[datetime, str] = ...,
+        startTime: TimestampTypeDef = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSnapshotsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Paginator.ListSnapshots.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/paginators/#listsnapshotspaginator)
         """
```

### Comparing `mypy-boto3-redshift-serverless-1.28.15.post1/mypy_boto3_redshift_serverless/type_defs.py` & `mypy-boto3-redshift-serverless-1.28.16/mypy_boto3_redshift_serverless/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_redshift_serverless.type_defs import ConfigParameterTypeDef
 
-    data: ConfigParameterTypeDef = {...}
+    data: ConfigParameterTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -58,16 +58,15 @@
     "GetTableRestoreStatusRequestRequestTypeDef",
     "TableRestoreStatusTypeDef",
     "GetUsageLimitRequestRequestTypeDef",
     "GetWorkgroupRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "ListEndpointAccessRequestRequestTypeDef",
     "ListNamespacesRequestRequestTypeDef",
-    "ListRecoveryPointsRequestRequestTypeDef",
-    "ListSnapshotsRequestRequestTypeDef",
+    "TimestampTypeDef",
     "ListTableRestoreStatusRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListUsageLimitsRequestRequestTypeDef",
     "ListWorkgroupsRequestRequestTypeDef",
     "NetworkInterfaceTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
     "RestoreFromRecoveryPointRequestRequestTypeDef",
@@ -109,19 +108,21 @@
     "GetResourcePolicyResponseTypeDef",
     "PutResourcePolicyResponseTypeDef",
     "GetTableRestoreStatusResponseTypeDef",
     "ListTableRestoreStatusResponseTypeDef",
     "RestoreTableFromSnapshotResponseTypeDef",
     "ListEndpointAccessRequestListEndpointAccessPaginateTypeDef",
     "ListNamespacesRequestListNamespacesPaginateTypeDef",
-    "ListRecoveryPointsRequestListRecoveryPointsPaginateTypeDef",
-    "ListSnapshotsRequestListSnapshotsPaginateTypeDef",
     "ListTableRestoreStatusRequestListTableRestoreStatusPaginateTypeDef",
     "ListUsageLimitsRequestListUsageLimitsPaginateTypeDef",
     "ListWorkgroupsRequestListWorkgroupsPaginateTypeDef",
+    "ListRecoveryPointsRequestListRecoveryPointsPaginateTypeDef",
+    "ListRecoveryPointsRequestRequestTypeDef",
+    "ListSnapshotsRequestListSnapshotsPaginateTypeDef",
+    "ListSnapshotsRequestRequestTypeDef",
     "VpcEndpointTypeDef",
     "EndpointAccessTypeDef",
     "EndpointTypeDef",
     "CreateEndpointAccessResponseTypeDef",
     "DeleteEndpointAccessResponseTypeDef",
     "GetEndpointAccessResponseTypeDef",
     "ListEndpointAccessResponseTypeDef",
@@ -486,41 +487,15 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-ListRecoveryPointsRequestRequestTypeDef = TypedDict(
-    "ListRecoveryPointsRequestRequestTypeDef",
-    {
-        "endTime": Union[datetime, str],
-        "maxResults": int,
-        "namespaceArn": str,
-        "namespaceName": str,
-        "nextToken": str,
-        "startTime": Union[datetime, str],
-    },
-    total=False,
-)
-
-ListSnapshotsRequestRequestTypeDef = TypedDict(
-    "ListSnapshotsRequestRequestTypeDef",
-    {
-        "endTime": Union[datetime, str],
-        "maxResults": int,
-        "namespaceArn": str,
-        "namespaceName": str,
-        "nextToken": str,
-        "ownerAccount": str,
-        "startTime": Union[datetime, str],
-    },
-    total=False,
-)
-
+TimestampTypeDef = Union[datetime, str]
 ListTableRestoreStatusRequestRequestTypeDef = TypedDict(
     "ListTableRestoreStatusRequestRequestTypeDef",
     {
         "maxResults": int,
         "namespaceName": str,
         "nextToken": str,
         "workgroupName": str,
@@ -1117,63 +1092,90 @@
     "ListNamespacesRequestListNamespacesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListRecoveryPointsRequestListRecoveryPointsPaginateTypeDef = TypedDict(
-    "ListRecoveryPointsRequestListRecoveryPointsPaginateTypeDef",
+ListTableRestoreStatusRequestListTableRestoreStatusPaginateTypeDef = TypedDict(
+    "ListTableRestoreStatusRequestListTableRestoreStatusPaginateTypeDef",
     {
-        "endTime": Union[datetime, str],
-        "namespaceArn": str,
         "namespaceName": str,
-        "startTime": Union[datetime, str],
+        "workgroupName": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListSnapshotsRequestListSnapshotsPaginateTypeDef = TypedDict(
-    "ListSnapshotsRequestListSnapshotsPaginateTypeDef",
+ListUsageLimitsRequestListUsageLimitsPaginateTypeDef = TypedDict(
+    "ListUsageLimitsRequestListUsageLimitsPaginateTypeDef",
+    {
+        "resourceArn": str,
+        "usageType": UsageLimitUsageTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListWorkgroupsRequestListWorkgroupsPaginateTypeDef = TypedDict(
+    "ListWorkgroupsRequestListWorkgroupsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListRecoveryPointsRequestListRecoveryPointsPaginateTypeDef = TypedDict(
+    "ListRecoveryPointsRequestListRecoveryPointsPaginateTypeDef",
     {
-        "endTime": Union[datetime, str],
+        "endTime": TimestampTypeDef,
         "namespaceArn": str,
         "namespaceName": str,
-        "ownerAccount": str,
-        "startTime": Union[datetime, str],
+        "startTime": TimestampTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListTableRestoreStatusRequestListTableRestoreStatusPaginateTypeDef = TypedDict(
-    "ListTableRestoreStatusRequestListTableRestoreStatusPaginateTypeDef",
+ListRecoveryPointsRequestRequestTypeDef = TypedDict(
+    "ListRecoveryPointsRequestRequestTypeDef",
     {
+        "endTime": TimestampTypeDef,
+        "maxResults": int,
+        "namespaceArn": str,
         "namespaceName": str,
-        "workgroupName": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "nextToken": str,
+        "startTime": TimestampTypeDef,
     },
     total=False,
 )
 
-ListUsageLimitsRequestListUsageLimitsPaginateTypeDef = TypedDict(
-    "ListUsageLimitsRequestListUsageLimitsPaginateTypeDef",
+ListSnapshotsRequestListSnapshotsPaginateTypeDef = TypedDict(
+    "ListSnapshotsRequestListSnapshotsPaginateTypeDef",
     {
-        "resourceArn": str,
-        "usageType": UsageLimitUsageTypeType,
+        "endTime": TimestampTypeDef,
+        "namespaceArn": str,
+        "namespaceName": str,
+        "ownerAccount": str,
+        "startTime": TimestampTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListWorkgroupsRequestListWorkgroupsPaginateTypeDef = TypedDict(
-    "ListWorkgroupsRequestListWorkgroupsPaginateTypeDef",
+ListSnapshotsRequestRequestTypeDef = TypedDict(
+    "ListSnapshotsRequestRequestTypeDef",
     {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "endTime": TimestampTypeDef,
+        "maxResults": int,
+        "namespaceArn": str,
+        "namespaceName": str,
+        "nextToken": str,
+        "ownerAccount": str,
+        "startTime": TimestampTypeDef,
     },
     total=False,
 )
 
 VpcEndpointTypeDef = TypedDict(
     "VpcEndpointTypeDef",
     {
```

### Comparing `mypy-boto3-redshift-serverless-1.28.15.post1/mypy_boto3_redshift_serverless/type_defs.pyi` & `mypy-boto3-redshift-serverless-1.28.16/mypy_boto3_redshift_serverless/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_redshift_serverless.type_defs import ConfigParameterTypeDef
 
-    data: ConfigParameterTypeDef = {...}
+    data: ConfigParameterTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -57,16 +57,15 @@
     "GetTableRestoreStatusRequestRequestTypeDef",
     "TableRestoreStatusTypeDef",
     "GetUsageLimitRequestRequestTypeDef",
     "GetWorkgroupRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "ListEndpointAccessRequestRequestTypeDef",
     "ListNamespacesRequestRequestTypeDef",
-    "ListRecoveryPointsRequestRequestTypeDef",
-    "ListSnapshotsRequestRequestTypeDef",
+    "TimestampTypeDef",
     "ListTableRestoreStatusRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListUsageLimitsRequestRequestTypeDef",
     "ListWorkgroupsRequestRequestTypeDef",
     "NetworkInterfaceTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
     "RestoreFromRecoveryPointRequestRequestTypeDef",
@@ -108,19 +107,21 @@
     "GetResourcePolicyResponseTypeDef",
     "PutResourcePolicyResponseTypeDef",
     "GetTableRestoreStatusResponseTypeDef",
     "ListTableRestoreStatusResponseTypeDef",
     "RestoreTableFromSnapshotResponseTypeDef",
     "ListEndpointAccessRequestListEndpointAccessPaginateTypeDef",
     "ListNamespacesRequestListNamespacesPaginateTypeDef",
-    "ListRecoveryPointsRequestListRecoveryPointsPaginateTypeDef",
-    "ListSnapshotsRequestListSnapshotsPaginateTypeDef",
     "ListTableRestoreStatusRequestListTableRestoreStatusPaginateTypeDef",
     "ListUsageLimitsRequestListUsageLimitsPaginateTypeDef",
     "ListWorkgroupsRequestListWorkgroupsPaginateTypeDef",
+    "ListRecoveryPointsRequestListRecoveryPointsPaginateTypeDef",
+    "ListRecoveryPointsRequestRequestTypeDef",
+    "ListSnapshotsRequestListSnapshotsPaginateTypeDef",
+    "ListSnapshotsRequestRequestTypeDef",
     "VpcEndpointTypeDef",
     "EndpointAccessTypeDef",
     "EndpointTypeDef",
     "CreateEndpointAccessResponseTypeDef",
     "DeleteEndpointAccessResponseTypeDef",
     "GetEndpointAccessResponseTypeDef",
     "ListEndpointAccessResponseTypeDef",
@@ -477,41 +478,15 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-ListRecoveryPointsRequestRequestTypeDef = TypedDict(
-    "ListRecoveryPointsRequestRequestTypeDef",
-    {
-        "endTime": Union[datetime, str],
-        "maxResults": int,
-        "namespaceArn": str,
-        "namespaceName": str,
-        "nextToken": str,
-        "startTime": Union[datetime, str],
-    },
-    total=False,
-)
-
-ListSnapshotsRequestRequestTypeDef = TypedDict(
-    "ListSnapshotsRequestRequestTypeDef",
-    {
-        "endTime": Union[datetime, str],
-        "maxResults": int,
-        "namespaceArn": str,
-        "namespaceName": str,
-        "nextToken": str,
-        "ownerAccount": str,
-        "startTime": Union[datetime, str],
-    },
-    total=False,
-)
-
+TimestampTypeDef = Union[datetime, str]
 ListTableRestoreStatusRequestRequestTypeDef = TypedDict(
     "ListTableRestoreStatusRequestRequestTypeDef",
     {
         "maxResults": int,
         "namespaceName": str,
         "nextToken": str,
         "workgroupName": str,
@@ -1086,63 +1061,90 @@
     "ListNamespacesRequestListNamespacesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListRecoveryPointsRequestListRecoveryPointsPaginateTypeDef = TypedDict(
-    "ListRecoveryPointsRequestListRecoveryPointsPaginateTypeDef",
+ListTableRestoreStatusRequestListTableRestoreStatusPaginateTypeDef = TypedDict(
+    "ListTableRestoreStatusRequestListTableRestoreStatusPaginateTypeDef",
     {
-        "endTime": Union[datetime, str],
-        "namespaceArn": str,
         "namespaceName": str,
-        "startTime": Union[datetime, str],
+        "workgroupName": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListSnapshotsRequestListSnapshotsPaginateTypeDef = TypedDict(
-    "ListSnapshotsRequestListSnapshotsPaginateTypeDef",
+ListUsageLimitsRequestListUsageLimitsPaginateTypeDef = TypedDict(
+    "ListUsageLimitsRequestListUsageLimitsPaginateTypeDef",
+    {
+        "resourceArn": str,
+        "usageType": UsageLimitUsageTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListWorkgroupsRequestListWorkgroupsPaginateTypeDef = TypedDict(
+    "ListWorkgroupsRequestListWorkgroupsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListRecoveryPointsRequestListRecoveryPointsPaginateTypeDef = TypedDict(
+    "ListRecoveryPointsRequestListRecoveryPointsPaginateTypeDef",
     {
-        "endTime": Union[datetime, str],
+        "endTime": TimestampTypeDef,
         "namespaceArn": str,
         "namespaceName": str,
-        "ownerAccount": str,
-        "startTime": Union[datetime, str],
+        "startTime": TimestampTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListTableRestoreStatusRequestListTableRestoreStatusPaginateTypeDef = TypedDict(
-    "ListTableRestoreStatusRequestListTableRestoreStatusPaginateTypeDef",
+ListRecoveryPointsRequestRequestTypeDef = TypedDict(
+    "ListRecoveryPointsRequestRequestTypeDef",
     {
+        "endTime": TimestampTypeDef,
+        "maxResults": int,
+        "namespaceArn": str,
         "namespaceName": str,
-        "workgroupName": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "nextToken": str,
+        "startTime": TimestampTypeDef,
     },
     total=False,
 )
 
-ListUsageLimitsRequestListUsageLimitsPaginateTypeDef = TypedDict(
-    "ListUsageLimitsRequestListUsageLimitsPaginateTypeDef",
+ListSnapshotsRequestListSnapshotsPaginateTypeDef = TypedDict(
+    "ListSnapshotsRequestListSnapshotsPaginateTypeDef",
     {
-        "resourceArn": str,
-        "usageType": UsageLimitUsageTypeType,
+        "endTime": TimestampTypeDef,
+        "namespaceArn": str,
+        "namespaceName": str,
+        "ownerAccount": str,
+        "startTime": TimestampTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListWorkgroupsRequestListWorkgroupsPaginateTypeDef = TypedDict(
-    "ListWorkgroupsRequestListWorkgroupsPaginateTypeDef",
+ListSnapshotsRequestRequestTypeDef = TypedDict(
+    "ListSnapshotsRequestRequestTypeDef",
     {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "endTime": TimestampTypeDef,
+        "maxResults": int,
+        "namespaceArn": str,
+        "namespaceName": str,
+        "nextToken": str,
+        "ownerAccount": str,
+        "startTime": TimestampTypeDef,
     },
     total=False,
 )
 
 VpcEndpointTypeDef = TypedDict(
     "VpcEndpointTypeDef",
     {
```

### Comparing `mypy-boto3-redshift-serverless-1.28.15.post1/mypy_boto3_redshift_serverless.egg-info/PKG-INFO` & `mypy-boto3-redshift-serverless-1.28.16/mypy_boto3_redshift_serverless.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-redshift-serverless
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.RedshiftServerless 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.RedshiftServerless 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 redshift-serverless type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 redshift-serverless type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-redshift-serverless.svg?color=blue)](https://pypi.org/project/mypy-boto3-redshift-serverless)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-redshift-serverless)](https://pepy.tech/project/mypy-boto3-redshift-serverless)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.RedshiftServerless 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless)
+[boto3.RedshiftServerless 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless)
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
 [mypy-boto3-redshift-serverless docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/).
 
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
@@ -344,20 +344,20 @@
 )
 
 
 def check_value(value: ListEndpointAccessPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_redshift_serverless.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_redshift_serverless.type_defs import (
     ConfigParameterTypeDef,
     TagTypeDef,
     ResponseMetadataTypeDef,
     SnapshotTypeDef,
@@ -383,16 +383,15 @@
     GetTableRestoreStatusRequestRequestTypeDef,
     TableRestoreStatusTypeDef,
     GetUsageLimitRequestRequestTypeDef,
     GetWorkgroupRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     ListEndpointAccessRequestRequestTypeDef,
     ListNamespacesRequestRequestTypeDef,
-    ListRecoveryPointsRequestRequestTypeDef,
-    ListSnapshotsRequestRequestTypeDef,
+    TimestampTypeDef,
     ListTableRestoreStatusRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListUsageLimitsRequestRequestTypeDef,
     ListWorkgroupsRequestRequestTypeDef,
     NetworkInterfaceTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
     RestoreFromRecoveryPointRequestRequestTypeDef,
@@ -434,19 +433,21 @@
     GetResourcePolicyResponseTypeDef,
     PutResourcePolicyResponseTypeDef,
     GetTableRestoreStatusResponseTypeDef,
     ListTableRestoreStatusResponseTypeDef,
     RestoreTableFromSnapshotResponseTypeDef,
     ListEndpointAccessRequestListEndpointAccessPaginateTypeDef,
     ListNamespacesRequestListNamespacesPaginateTypeDef,
-    ListRecoveryPointsRequestListRecoveryPointsPaginateTypeDef,
-    ListSnapshotsRequestListSnapshotsPaginateTypeDef,
     ListTableRestoreStatusRequestListTableRestoreStatusPaginateTypeDef,
     ListUsageLimitsRequestListUsageLimitsPaginateTypeDef,
     ListWorkgroupsRequestListWorkgroupsPaginateTypeDef,
+    ListRecoveryPointsRequestListRecoveryPointsPaginateTypeDef,
+    ListRecoveryPointsRequestRequestTypeDef,
+    ListSnapshotsRequestListSnapshotsPaginateTypeDef,
+    ListSnapshotsRequestRequestTypeDef,
     VpcEndpointTypeDef,
     EndpointAccessTypeDef,
     EndpointTypeDef,
     CreateEndpointAccessResponseTypeDef,
     DeleteEndpointAccessResponseTypeDef,
     GetEndpointAccessResponseTypeDef,
     ListEndpointAccessResponseTypeDef,
@@ -456,15 +457,15 @@
     DeleteWorkgroupResponseTypeDef,
     GetWorkgroupResponseTypeDef,
     ListWorkgroupsResponseTypeDef,
     UpdateWorkgroupResponseTypeDef,
 )
 
 
-def get_structure() -> ConfigParameterTypeDef:
+def get_value() -> ConfigParameterTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-redshift-serverless-1.28.15.post1/mypy_boto3_redshift_serverless.egg-info/SOURCES.txt` & `mypy-boto3-redshift-serverless-1.28.16/mypy_boto3_redshift_serverless.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-serverless-1.28.15.post1/setup.py` & `mypy-boto3-redshift-serverless-1.28.16/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-redshift-serverless",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_redshift_serverless"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.RedshiftServerless 1.28.15 service generated with"
-        " mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.RedshiftServerless 1.28.16 service generated with"
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
-    keywords="boto3 redshift-serverless type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 redshift-serverless type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_redshift_serverless": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/"
```

