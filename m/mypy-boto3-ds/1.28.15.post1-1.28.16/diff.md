# Comparing `tmp/mypy-boto3-ds-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-ds-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-ds-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:59 2023, max compression
+gzip compressed data, was "mypy-boto3-ds-1.28.16.tar", last modified: Tue Aug  1 11:36:39 2023, max compression
```

## Comparing `mypy-boto3-ds-1.28.15.post1.tar` & `mypy-boto3-ds-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:59.153114 mypy-boto3-ds-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:42:50.000000 mypy-boto3-ds-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    22131 2023-07-29 10:02:59.149114 mypy-boto3-ds-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20644 2023-07-29 09:42:50.000000 mypy-boto3-ds-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:59.141114 mypy-boto3-ds-1.28.15.post1/mypy_boto3_ds/
--rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-07-29 09:42:50.000000 mypy-boto3-ds-1.28.15.post1/mypy_boto3_ds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-07-29 09:42:50.000000 mypy-boto3-ds-1.28.15.post1/mypy_boto3_ds/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-29 09:42:50.000000 mypy-boto3-ds-1.28.15.post1/mypy_boto3_ds/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    51985 2023-07-29 09:42:50.000000 mypy-boto3-ds-1.28.15.post1/mypy_boto3_ds/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    51897 2023-07-29 09:42:50.000000 mypy-boto3-ds-1.28.15.post1/mypy_boto3_ds/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13686 2023-07-29 09:42:51.000000 mypy-boto3-ds-1.28.15.post1/mypy_boto3_ds/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13684 2023-07-29 09:42:51.000000 mypy-boto3-ds-1.28.15.post1/mypy_boto3_ds/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    16998 2023-07-29 09:42:51.000000 mypy-boto3-ds-1.28.15.post1/mypy_boto3_ds/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    16981 2023-07-29 09:42:50.000000 mypy-boto3-ds-1.28.15.post1/mypy_boto3_ds/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:42:50.000000 mypy-boto3-ds-1.28.15.post1/mypy_boto3_ds/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    58274 2023-07-29 09:42:54.000000 mypy-boto3-ds-1.28.15.post1/mypy_boto3_ds/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    58201 2023-07-29 09:42:52.000000 mypy-boto3-ds-1.28.15.post1/mypy_boto3_ds/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:42:50.000000 mypy-boto3-ds-1.28.15.post1/mypy_boto3_ds/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:59.149114 mypy-boto3-ds-1.28.15.post1/mypy_boto3_ds.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22131 2023-07-29 10:02:58.000000 mypy-boto3-ds-1.28.15.post1/mypy_boto3_ds.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-29 10:02:58.000000 mypy-boto3-ds-1.28.15.post1/mypy_boto3_ds.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:58.000000 mypy-boto3-ds-1.28.15.post1/mypy_boto3_ds.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:58.000000 mypy-boto3-ds-1.28.15.post1/mypy_boto3_ds.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:58.000000 mypy-boto3-ds-1.28.15.post1/mypy_boto3_ds.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-29 10:02:58.000000 mypy-boto3-ds-1.28.15.post1/mypy_boto3_ds.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:59.153114 mypy-boto3-ds-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-07-29 09:42:50.000000 mypy-boto3-ds-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:39.136907 mypy-boto3-ds-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:15:22.000000 mypy-boto3-ds-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22191 2023-08-01 11:36:39.136907 mypy-boto3-ds-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20713 2023-08-01 11:15:22.000000 mypy-boto3-ds-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:39.136907 mypy-boto3-ds-1.28.16/mypy_boto3_ds/
+-rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-08-01 11:15:22.000000 mypy-boto3-ds-1.28.16/mypy_boto3_ds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-08-01 11:15:22.000000 mypy-boto3-ds-1.28.16/mypy_boto3_ds/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-08-01 11:15:22.000000 mypy-boto3-ds-1.28.16/mypy_boto3_ds/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51663 2023-08-01 11:15:23.000000 mypy-boto3-ds-1.28.16/mypy_boto3_ds/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51575 2023-08-01 11:15:23.000000 mypy-boto3-ds-1.28.16/mypy_boto3_ds/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13686 2023-08-01 11:15:23.000000 mypy-boto3-ds-1.28.16/mypy_boto3_ds/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13684 2023-08-01 11:15:23.000000 mypy-boto3-ds-1.28.16/mypy_boto3_ds/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    16998 2023-08-01 11:15:23.000000 mypy-boto3-ds-1.28.16/mypy_boto3_ds/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16981 2023-08-01 11:15:23.000000 mypy-boto3-ds-1.28.16/mypy_boto3_ds/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:15:22.000000 mypy-boto3-ds-1.28.16/mypy_boto3_ds/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    58551 2023-08-01 11:15:26.000000 mypy-boto3-ds-1.28.16/mypy_boto3_ds/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58478 2023-08-01 11:15:26.000000 mypy-boto3-ds-1.28.16/mypy_boto3_ds/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:15:22.000000 mypy-boto3-ds-1.28.16/mypy_boto3_ds/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:39.136907 mypy-boto3-ds-1.28.16/mypy_boto3_ds.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22191 2023-08-01 11:36:38.000000 mypy-boto3-ds-1.28.16/mypy_boto3_ds.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-08-01 11:36:38.000000 mypy-boto3-ds-1.28.16/mypy_boto3_ds.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:38.000000 mypy-boto3-ds-1.28.16/mypy_boto3_ds.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:38.000000 mypy-boto3-ds-1.28.16/mypy_boto3_ds.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:38.000000 mypy-boto3-ds-1.28.16/mypy_boto3_ds.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-01 11:36:38.000000 mypy-boto3-ds-1.28.16/mypy_boto3_ds.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:39.136907 mypy-boto3-ds-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-08-01 11:15:22.000000 mypy-boto3-ds-1.28.16/setup.py
```

### Comparing `mypy-boto3-ds-1.28.15.post1/LICENSE` & `mypy-boto3-ds-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ds-1.28.15.post1/PKG-INFO` & `mypy-boto3-ds-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ds
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.DirectoryService 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.DirectoryService 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 ds type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 ds type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ds.svg?color=blue)](https://pypi.org/project/mypy-boto3-ds)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ds)](https://pepy.tech/project/mypy-boto3-ds)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DirectoryService 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService)
+[boto3.DirectoryService 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService)
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
 [mypy-boto3-ds docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/).
 
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
@@ -400,20 +400,20 @@
 )
 
 
 def check_value(value: CertificateStateType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_ds.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_ds.type_defs import (
     AcceptSharedDirectoryRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     SharedDirectoryTypeDef,
     IpRouteTypeDef,
@@ -549,16 +549,18 @@
     DescribeEventTopicsResultTypeDef,
     DescribeLDAPSSettingsResultTypeDef,
     DescribeSettingsResultTypeDef,
     DescribeSnapshotsResultTypeDef,
     DescribeTrustsResultTypeDef,
     OwnerDirectoryDescriptionTypeDef,
     GetDirectoryLimitsResultTypeDef,
+    DirectoryVpcSettingsUnionTypeDef,
     RegionDescriptionTypeDef,
     EnableRadiusRequestRequestTypeDef,
+    RadiusSettingsUnionTypeDef,
     UpdateRadiusRequestRequestTypeDef,
     GetSnapshotLimitsResultTypeDef,
     ListIpRoutesResultTypeDef,
     ListLogSubscriptionsResultTypeDef,
     ListSchemaExtensionsResultTypeDef,
     UpdateDirectorySetupRequestRequestTypeDef,
     UpdateValueTypeDef,
@@ -571,15 +573,15 @@
     DescribeRegionsResultTypeDef,
     UpdateInfoEntryTypeDef,
     DescribeDirectoriesResultTypeDef,
     DescribeUpdateDirectoryResultTypeDef,
 )
 
 
-def get_structure() -> AcceptSharedDirectoryRequestRequestTypeDef:
+def get_value() -> AcceptSharedDirectoryRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-ds-1.28.15.post1/README.md` & `mypy-boto3-ds-1.28.16/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ds.svg?color=blue)](https://pypi.org/project/mypy-boto3-ds)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ds)](https://pepy.tech/project/mypy-boto3-ds)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DirectoryService 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService)
+[boto3.DirectoryService 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService)
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
 [mypy-boto3-ds docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/).
 
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
@@ -368,20 +368,20 @@
 )
 
 
 def check_value(value: CertificateStateType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_ds.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_ds.type_defs import (
     AcceptSharedDirectoryRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     SharedDirectoryTypeDef,
     IpRouteTypeDef,
@@ -517,16 +517,18 @@
     DescribeEventTopicsResultTypeDef,
     DescribeLDAPSSettingsResultTypeDef,
     DescribeSettingsResultTypeDef,
     DescribeSnapshotsResultTypeDef,
     DescribeTrustsResultTypeDef,
     OwnerDirectoryDescriptionTypeDef,
     GetDirectoryLimitsResultTypeDef,
+    DirectoryVpcSettingsUnionTypeDef,
     RegionDescriptionTypeDef,
     EnableRadiusRequestRequestTypeDef,
+    RadiusSettingsUnionTypeDef,
     UpdateRadiusRequestRequestTypeDef,
     GetSnapshotLimitsResultTypeDef,
     ListIpRoutesResultTypeDef,
     ListLogSubscriptionsResultTypeDef,
     ListSchemaExtensionsResultTypeDef,
     UpdateDirectorySetupRequestRequestTypeDef,
     UpdateValueTypeDef,
@@ -539,15 +541,15 @@
     DescribeRegionsResultTypeDef,
     UpdateInfoEntryTypeDef,
     DescribeDirectoriesResultTypeDef,
     DescribeUpdateDirectoryResultTypeDef,
 )
 
 
-def get_structure() -> AcceptSharedDirectoryRequestRequestTypeDef:
+def get_value() -> AcceptSharedDirectoryRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-ds-1.28.15.post1/mypy_boto3_ds/__init__.py` & `mypy-boto3-ds-1.28.16/mypy_boto3_ds/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ds-1.28.15.post1/mypy_boto3_ds/__init__.pyi` & `mypy-boto3-ds-1.28.16/mypy_boto3_ds/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ds-1.28.15.post1/mypy_boto3_ds/__main__.py` & `mypy-boto3-ds-1.28.16/mypy_boto3_ds/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.DirectoryService 1.28.15\nVersion:        "
-        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.DirectoryService 1.28.16\nVersion:         1.28.16\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService\nOther"
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

### Comparing `mypy-boto3-ds-1.28.15.post1/mypy_boto3_ds/client.py` & `mypy-boto3-ds-1.28.16/mypy_boto3_ds/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_ds.client import DirectoryServiceClient
 
     session = Session()
     client: DirectoryServiceClient = session.client("ds")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     CertificateTypeType,
     ClientAuthenticationTypeType,
     DirectoryConfigurationStatusType,
@@ -69,27 +69,25 @@
     DescribeRegionsResultTypeDef,
     DescribeSettingsResultTypeDef,
     DescribeSharedDirectoriesResultTypeDef,
     DescribeSnapshotsResultTypeDef,
     DescribeTrustsResultTypeDef,
     DescribeUpdateDirectoryResultTypeDef,
     DirectoryConnectSettingsTypeDef,
-    DirectoryVpcSettingsOutputTypeDef,
-    DirectoryVpcSettingsTypeDef,
+    DirectoryVpcSettingsUnionTypeDef,
     GetDirectoryLimitsResultTypeDef,
     GetSnapshotLimitsResultTypeDef,
     IpRouteTypeDef,
     ListCertificatesResultTypeDef,
     ListIpRoutesResultTypeDef,
     ListLogSubscriptionsResultTypeDef,
     ListSchemaExtensionsResultTypeDef,
     ListTagsForResourceResultTypeDef,
     OSUpdateSettingsTypeDef,
-    RadiusSettingsOutputTypeDef,
-    RadiusSettingsTypeDef,
+    RadiusSettingsUnionTypeDef,
     RegisterCertificateResultTypeDef,
     RejectSharedDirectoryResultTypeDef,
     SettingTypeDef,
     ShareDirectoryResultTypeDef,
     ShareTargetTypeDef,
     StartSchemaExtensionResultTypeDef,
     TagTypeDef,
@@ -199,19 +197,15 @@
         from your Microsoft AD on Amazon Web Services.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Client.add_ip_routes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/client/#add_ip_routes)
         """
 
     def add_region(
-        self,
-        *,
-        DirectoryId: str,
-        RegionName: str,
-        VPCSettings: Union[DirectoryVpcSettingsTypeDef, DirectoryVpcSettingsOutputTypeDef]
+        self, *, DirectoryId: str, RegionName: str, VPCSettings: DirectoryVpcSettingsUnionTypeDef
     ) -> Dict[str, Any]:
         """
         Adds two domain controllers in the specified Region for the specified directory.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Client.add_region)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/client/#add_region)
         """
@@ -309,15 +303,15 @@
         self,
         *,
         Name: str,
         Password: str,
         Size: DirectorySizeType,
         ShortName: str = ...,
         Description: str = ...,
-        VpcSettings: Union[DirectoryVpcSettingsTypeDef, DirectoryVpcSettingsOutputTypeDef] = ...,
+        VpcSettings: DirectoryVpcSettingsUnionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateDirectoryResultTypeDef:
         """
         Creates a Simple AD directory.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Client.create_directory)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/client/#create_directory)
@@ -334,15 +328,15 @@
         """
 
     def create_microsoft_ad(
         self,
         *,
         Name: str,
         Password: str,
-        VpcSettings: Union[DirectoryVpcSettingsTypeDef, DirectoryVpcSettingsOutputTypeDef],
+        VpcSettings: DirectoryVpcSettingsUnionTypeDef,
         ShortName: str = ...,
         Description: str = ...,
         Edition: DirectoryEditionType = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateMicrosoftADResultTypeDef:
         """
         Creates a Microsoft AD directory in the Amazon Web Services Cloud.
@@ -669,18 +663,15 @@
         Activates the switch for the specific directory to always use LDAP secure calls.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Client.enable_ldaps)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/client/#enable_ldaps)
         """
 
     def enable_radius(
-        self,
-        *,
-        DirectoryId: str,
-        RadiusSettings: Union[RadiusSettingsTypeDef, RadiusSettingsOutputTypeDef]
+        self, *, DirectoryId: str, RadiusSettings: RadiusSettingsUnionTypeDef
     ) -> Dict[str, Any]:
         """
         Enables multi-factor authentication (MFA) with the Remote Authentication Dial In
         User Service (RADIUS) server for an AD Connector or Microsoft AD directory.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Client.enable_radius)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/client/#enable_radius)
@@ -932,18 +923,15 @@
         Adds or removes domain controllers to or from the directory.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Client.update_number_of_domain_controllers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/client/#update_number_of_domain_controllers)
         """
 
     def update_radius(
-        self,
-        *,
-        DirectoryId: str,
-        RadiusSettings: Union[RadiusSettingsTypeDef, RadiusSettingsOutputTypeDef]
+        self, *, DirectoryId: str, RadiusSettings: RadiusSettingsUnionTypeDef
     ) -> Dict[str, Any]:
         """
         Updates the Remote Authentication Dial In User Service (RADIUS) server
         information for an AD Connector or Microsoft AD directory.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Client.update_radius)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/client/#update_radius)
```

### Comparing `mypy-boto3-ds-1.28.15.post1/mypy_boto3_ds/client.pyi` & `mypy-boto3-ds-1.28.16/mypy_boto3_ds/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_ds.client import DirectoryServiceClient
 
     session = Session()
     client: DirectoryServiceClient = session.client("ds")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     CertificateTypeType,
     ClientAuthenticationTypeType,
     DirectoryConfigurationStatusType,
@@ -69,27 +69,25 @@
     DescribeRegionsResultTypeDef,
     DescribeSettingsResultTypeDef,
     DescribeSharedDirectoriesResultTypeDef,
     DescribeSnapshotsResultTypeDef,
     DescribeTrustsResultTypeDef,
     DescribeUpdateDirectoryResultTypeDef,
     DirectoryConnectSettingsTypeDef,
-    DirectoryVpcSettingsOutputTypeDef,
-    DirectoryVpcSettingsTypeDef,
+    DirectoryVpcSettingsUnionTypeDef,
     GetDirectoryLimitsResultTypeDef,
     GetSnapshotLimitsResultTypeDef,
     IpRouteTypeDef,
     ListCertificatesResultTypeDef,
     ListIpRoutesResultTypeDef,
     ListLogSubscriptionsResultTypeDef,
     ListSchemaExtensionsResultTypeDef,
     ListTagsForResourceResultTypeDef,
     OSUpdateSettingsTypeDef,
-    RadiusSettingsOutputTypeDef,
-    RadiusSettingsTypeDef,
+    RadiusSettingsUnionTypeDef,
     RegisterCertificateResultTypeDef,
     RejectSharedDirectoryResultTypeDef,
     SettingTypeDef,
     ShareDirectoryResultTypeDef,
     ShareTargetTypeDef,
     StartSchemaExtensionResultTypeDef,
     TagTypeDef,
@@ -192,19 +190,15 @@
         address, you must add a CIDR address block to correctly route traffic to and
         from your Microsoft AD on Amazon Web Services.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Client.add_ip_routes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/client/#add_ip_routes)
         """
     def add_region(
-        self,
-        *,
-        DirectoryId: str,
-        RegionName: str,
-        VPCSettings: Union[DirectoryVpcSettingsTypeDef, DirectoryVpcSettingsOutputTypeDef]
+        self, *, DirectoryId: str, RegionName: str, VPCSettings: DirectoryVpcSettingsUnionTypeDef
     ) -> Dict[str, Any]:
         """
         Adds two domain controllers in the specified Region for the specified directory.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Client.add_region)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/client/#add_region)
         """
@@ -293,15 +287,15 @@
         self,
         *,
         Name: str,
         Password: str,
         Size: DirectorySizeType,
         ShortName: str = ...,
         Description: str = ...,
-        VpcSettings: Union[DirectoryVpcSettingsTypeDef, DirectoryVpcSettingsOutputTypeDef] = ...,
+        VpcSettings: DirectoryVpcSettingsUnionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateDirectoryResultTypeDef:
         """
         Creates a Simple AD directory.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Client.create_directory)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/client/#create_directory)
@@ -316,15 +310,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/client/#create_log_subscription)
         """
     def create_microsoft_ad(
         self,
         *,
         Name: str,
         Password: str,
-        VpcSettings: Union[DirectoryVpcSettingsTypeDef, DirectoryVpcSettingsOutputTypeDef],
+        VpcSettings: DirectoryVpcSettingsUnionTypeDef,
         ShortName: str = ...,
         Description: str = ...,
         Edition: DirectoryEditionType = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateMicrosoftADResultTypeDef:
         """
         Creates a Microsoft AD directory in the Amazon Web Services Cloud.
@@ -622,18 +616,15 @@
         """
         Activates the switch for the specific directory to always use LDAP secure calls.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Client.enable_ldaps)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/client/#enable_ldaps)
         """
     def enable_radius(
-        self,
-        *,
-        DirectoryId: str,
-        RadiusSettings: Union[RadiusSettingsTypeDef, RadiusSettingsOutputTypeDef]
+        self, *, DirectoryId: str, RadiusSettings: RadiusSettingsUnionTypeDef
     ) -> Dict[str, Any]:
         """
         Enables multi-factor authentication (MFA) with the Remote Authentication Dial In
         User Service (RADIUS) server for an AD Connector or Microsoft AD directory.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Client.enable_radius)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/client/#enable_radius)
@@ -861,18 +852,15 @@
         """
         Adds or removes domain controllers to or from the directory.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Client.update_number_of_domain_controllers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/client/#update_number_of_domain_controllers)
         """
     def update_radius(
-        self,
-        *,
-        DirectoryId: str,
-        RadiusSettings: Union[RadiusSettingsTypeDef, RadiusSettingsOutputTypeDef]
+        self, *, DirectoryId: str, RadiusSettings: RadiusSettingsUnionTypeDef
     ) -> Dict[str, Any]:
         """
         Updates the Remote Authentication Dial In User Service (RADIUS) server
         information for an AD Connector or Microsoft AD directory.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Client.update_radius)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/client/#update_radius)
```

### Comparing `mypy-boto3-ds-1.28.15.post1/mypy_boto3_ds/literals.py` & `mypy-boto3-ds-1.28.16/mypy_boto3_ds/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ds-1.28.15.post1/mypy_boto3_ds/literals.pyi` & `mypy-boto3-ds-1.28.16/mypy_boto3_ds/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ds-1.28.15.post1/mypy_boto3_ds/paginator.py` & `mypy-boto3-ds-1.28.16/mypy_boto3_ds/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ds-1.28.15.post1/mypy_boto3_ds/paginator.pyi` & `mypy-boto3-ds-1.28.16/mypy_boto3_ds/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ds-1.28.15.post1/mypy_boto3_ds/type_defs.py` & `mypy-boto3-ds-1.28.16/mypy_boto3_ds/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_ds.type_defs import AcceptSharedDirectoryRequestRequestTypeDef
 
-    data: AcceptSharedDirectoryRequestRequestTypeDef = {...}
+    data: AcceptSharedDirectoryRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence
+from typing import Dict, List, Sequence, Union
 
 from .literals import (
     CertificateStateType,
     CertificateTypeType,
     ClientAuthenticationStatusType,
     ClientAuthenticationTypeType,
     DirectoryConfigurationStatusType,
@@ -192,16 +192,18 @@
     "DescribeEventTopicsResultTypeDef",
     "DescribeLDAPSSettingsResultTypeDef",
     "DescribeSettingsResultTypeDef",
     "DescribeSnapshotsResultTypeDef",
     "DescribeTrustsResultTypeDef",
     "OwnerDirectoryDescriptionTypeDef",
     "GetDirectoryLimitsResultTypeDef",
+    "DirectoryVpcSettingsUnionTypeDef",
     "RegionDescriptionTypeDef",
     "EnableRadiusRequestRequestTypeDef",
+    "RadiusSettingsUnionTypeDef",
     "UpdateRadiusRequestRequestTypeDef",
     "GetSnapshotLimitsResultTypeDef",
     "ListIpRoutesResultTypeDef",
     "ListLogSubscriptionsResultTypeDef",
     "ListSchemaExtensionsResultTypeDef",
     "UpdateDirectorySetupRequestRequestTypeDef",
     "UpdateValueTypeDef",
@@ -1995,14 +1997,17 @@
     "GetDirectoryLimitsResultTypeDef",
     {
         "DirectoryLimits": DirectoryLimitsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DirectoryVpcSettingsUnionTypeDef = Union[
+    DirectoryVpcSettingsTypeDef, DirectoryVpcSettingsOutputTypeDef
+]
 RegionDescriptionTypeDef = TypedDict(
     "RegionDescriptionTypeDef",
     {
         "DirectoryId": str,
         "RegionName": str,
         "RegionType": RegionTypeType,
         "Status": DirectoryStageType,
@@ -2019,14 +2024,15 @@
     "EnableRadiusRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "RadiusSettings": RadiusSettingsTypeDef,
     },
 )
 
+RadiusSettingsUnionTypeDef = Union[RadiusSettingsTypeDef, RadiusSettingsOutputTypeDef]
 UpdateRadiusRequestRequestTypeDef = TypedDict(
     "UpdateRadiusRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "RadiusSettings": RadiusSettingsTypeDef,
     },
 )
```

### Comparing `mypy-boto3-ds-1.28.15.post1/mypy_boto3_ds/type_defs.pyi` & `mypy-boto3-ds-1.28.16/mypy_boto3_ds/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_ds.type_defs import AcceptSharedDirectoryRequestRequestTypeDef
 
-    data: AcceptSharedDirectoryRequestRequestTypeDef = {...}
+    data: AcceptSharedDirectoryRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence
+from typing import Dict, List, Sequence, Union
 
 from .literals import (
     CertificateStateType,
     CertificateTypeType,
     ClientAuthenticationStatusType,
     ClientAuthenticationTypeType,
     DirectoryConfigurationStatusType,
@@ -191,16 +191,18 @@
     "DescribeEventTopicsResultTypeDef",
     "DescribeLDAPSSettingsResultTypeDef",
     "DescribeSettingsResultTypeDef",
     "DescribeSnapshotsResultTypeDef",
     "DescribeTrustsResultTypeDef",
     "OwnerDirectoryDescriptionTypeDef",
     "GetDirectoryLimitsResultTypeDef",
+    "DirectoryVpcSettingsUnionTypeDef",
     "RegionDescriptionTypeDef",
     "EnableRadiusRequestRequestTypeDef",
+    "RadiusSettingsUnionTypeDef",
     "UpdateRadiusRequestRequestTypeDef",
     "GetSnapshotLimitsResultTypeDef",
     "ListIpRoutesResultTypeDef",
     "ListLogSubscriptionsResultTypeDef",
     "ListSchemaExtensionsResultTypeDef",
     "UpdateDirectorySetupRequestRequestTypeDef",
     "UpdateValueTypeDef",
@@ -1926,14 +1928,17 @@
     "GetDirectoryLimitsResultTypeDef",
     {
         "DirectoryLimits": DirectoryLimitsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DirectoryVpcSettingsUnionTypeDef = Union[
+    DirectoryVpcSettingsTypeDef, DirectoryVpcSettingsOutputTypeDef
+]
 RegionDescriptionTypeDef = TypedDict(
     "RegionDescriptionTypeDef",
     {
         "DirectoryId": str,
         "RegionName": str,
         "RegionType": RegionTypeType,
         "Status": DirectoryStageType,
@@ -1950,14 +1955,15 @@
     "EnableRadiusRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "RadiusSettings": RadiusSettingsTypeDef,
     },
 )
 
+RadiusSettingsUnionTypeDef = Union[RadiusSettingsTypeDef, RadiusSettingsOutputTypeDef]
 UpdateRadiusRequestRequestTypeDef = TypedDict(
     "UpdateRadiusRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "RadiusSettings": RadiusSettingsTypeDef,
     },
 )
```

### Comparing `mypy-boto3-ds-1.28.15.post1/mypy_boto3_ds.egg-info/PKG-INFO` & `mypy-boto3-ds-1.28.16/mypy_boto3_ds.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ds
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.DirectoryService 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.DirectoryService 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 ds type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 ds type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ds.svg?color=blue)](https://pypi.org/project/mypy-boto3-ds)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ds)](https://pepy.tech/project/mypy-boto3-ds)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DirectoryService 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService)
+[boto3.DirectoryService 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService)
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
 [mypy-boto3-ds docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/).
 
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
@@ -400,20 +400,20 @@
 )
 
 
 def check_value(value: CertificateStateType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_ds.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_ds.type_defs import (
     AcceptSharedDirectoryRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     SharedDirectoryTypeDef,
     IpRouteTypeDef,
@@ -549,16 +549,18 @@
     DescribeEventTopicsResultTypeDef,
     DescribeLDAPSSettingsResultTypeDef,
     DescribeSettingsResultTypeDef,
     DescribeSnapshotsResultTypeDef,
     DescribeTrustsResultTypeDef,
     OwnerDirectoryDescriptionTypeDef,
     GetDirectoryLimitsResultTypeDef,
+    DirectoryVpcSettingsUnionTypeDef,
     RegionDescriptionTypeDef,
     EnableRadiusRequestRequestTypeDef,
+    RadiusSettingsUnionTypeDef,
     UpdateRadiusRequestRequestTypeDef,
     GetSnapshotLimitsResultTypeDef,
     ListIpRoutesResultTypeDef,
     ListLogSubscriptionsResultTypeDef,
     ListSchemaExtensionsResultTypeDef,
     UpdateDirectorySetupRequestRequestTypeDef,
     UpdateValueTypeDef,
@@ -571,15 +573,15 @@
     DescribeRegionsResultTypeDef,
     UpdateInfoEntryTypeDef,
     DescribeDirectoriesResultTypeDef,
     DescribeUpdateDirectoryResultTypeDef,
 )
 
 
-def get_structure() -> AcceptSharedDirectoryRequestRequestTypeDef:
+def get_value() -> AcceptSharedDirectoryRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-ds-1.28.15.post1/mypy_boto3_ds.egg-info/SOURCES.txt` & `mypy-boto3-ds-1.28.16/mypy_boto3_ds.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ds-1.28.15.post1/setup.py` & `mypy-boto3-ds-1.28.16/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-ds",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_ds"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.DirectoryService 1.28.15 service generated with"
-        " mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.DirectoryService 1.28.16 service generated with"
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
-    keywords="boto3 ds type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 ds type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_ds": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ds/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

