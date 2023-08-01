# Comparing `tmp/mypy-boto3-efs-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-efs-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-efs-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:02 2023, max compression
+gzip compressed data, was "mypy-boto3-efs-1.28.16.tar", last modified: Tue Aug  1 11:36:42 2023, max compression
```

## Comparing `mypy-boto3-efs-1.28.15.post1.tar` & `mypy-boto3-efs-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:02.509128 mypy-boto3-efs-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:44:27.000000 mypy-boto3-efs-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15683 2023-07-29 10:03:02.509128 mypy-boto3-efs-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14206 2023-07-29 09:44:27.000000 mypy-boto3-efs-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:02.497128 mypy-boto3-efs-1.28.15.post1/mypy_boto3_efs/
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-07-29 09:44:27.000000 mypy-boto3-efs-1.28.15.post1/mypy_boto3_efs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-29 09:44:27.000000 mypy-boto3-efs-1.28.15.post1/mypy_boto3_efs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-29 09:44:27.000000 mypy-boto3-efs-1.28.15.post1/mypy_boto3_efs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23569 2023-07-29 09:44:27.000000 mypy-boto3-efs-1.28.15.post1/mypy_boto3_efs/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    23529 2023-07-29 09:44:27.000000 mypy-boto3-efs-1.28.15.post1/mypy_boto3_efs/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9560 2023-07-29 09:44:27.000000 mypy-boto3-efs-1.28.15.post1/mypy_boto3_efs/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9558 2023-07-29 09:44:27.000000 mypy-boto3-efs-1.28.15.post1/mypy_boto3_efs/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-07-29 09:44:27.000000 mypy-boto3-efs-1.28.15.post1/mypy_boto3_efs/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-07-29 09:44:27.000000 mypy-boto3-efs-1.28.15.post1/mypy_boto3_efs/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:44:27.000000 mypy-boto3-efs-1.28.15.post1/mypy_boto3_efs/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    24584 2023-07-29 09:44:28.000000 mypy-boto3-efs-1.28.15.post1/mypy_boto3_efs/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    24553 2023-07-29 09:44:27.000000 mypy-boto3-efs-1.28.15.post1/mypy_boto3_efs/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:44:27.000000 mypy-boto3-efs-1.28.15.post1/mypy_boto3_efs/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:02.509128 mypy-boto3-efs-1.28.15.post1/mypy_boto3_efs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15683 2023-07-29 10:03:02.000000 mypy-boto3-efs-1.28.15.post1/mypy_boto3_efs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-29 10:03:02.000000 mypy-boto3-efs-1.28.15.post1/mypy_boto3_efs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:02.000000 mypy-boto3-efs-1.28.15.post1/mypy_boto3_efs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:02.000000 mypy-boto3-efs-1.28.15.post1/mypy_boto3_efs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:02.000000 mypy-boto3-efs-1.28.15.post1/mypy_boto3_efs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-29 10:03:02.000000 mypy-boto3-efs-1.28.15.post1/mypy_boto3_efs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:02.509128 mypy-boto3-efs-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-29 09:44:27.000000 mypy-boto3-efs-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:42.508901 mypy-boto3-efs-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:17:01.000000 mypy-boto3-efs-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15700 2023-08-01 11:36:42.508901 mypy-boto3-efs-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14232 2023-08-01 11:17:01.000000 mypy-boto3-efs-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:42.500901 mypy-boto3-efs-1.28.16/mypy_boto3_efs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-08-01 11:17:01.000000 mypy-boto3-efs-1.28.16/mypy_boto3_efs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-08-01 11:17:01.000000 mypy-boto3-efs-1.28.16/mypy_boto3_efs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-08-01 11:17:01.000000 mypy-boto3-efs-1.28.16/mypy_boto3_efs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23513 2023-08-01 11:17:01.000000 mypy-boto3-efs-1.28.16/mypy_boto3_efs/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23473 2023-08-01 11:17:01.000000 mypy-boto3-efs-1.28.16/mypy_boto3_efs/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9560 2023-08-01 11:17:02.000000 mypy-boto3-efs-1.28.16/mypy_boto3_efs/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9558 2023-08-01 11:17:01.000000 mypy-boto3-efs-1.28.16/mypy_boto3_efs/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-08-01 11:17:01.000000 mypy-boto3-efs-1.28.16/mypy_boto3_efs/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-08-01 11:17:01.000000 mypy-boto3-efs-1.28.16/mypy_boto3_efs/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:17:01.000000 mypy-boto3-efs-1.28.16/mypy_boto3_efs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    24690 2023-08-01 11:17:02.000000 mypy-boto3-efs-1.28.16/mypy_boto3_efs/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24659 2023-08-01 11:17:02.000000 mypy-boto3-efs-1.28.16/mypy_boto3_efs/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:17:01.000000 mypy-boto3-efs-1.28.16/mypy_boto3_efs/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:42.508901 mypy-boto3-efs-1.28.16/mypy_boto3_efs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15700 2023-08-01 11:36:42.000000 mypy-boto3-efs-1.28.16/mypy_boto3_efs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-08-01 11:36:42.000000 mypy-boto3-efs-1.28.16/mypy_boto3_efs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:42.000000 mypy-boto3-efs-1.28.16/mypy_boto3_efs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:42.000000 mypy-boto3-efs-1.28.16/mypy_boto3_efs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:42.000000 mypy-boto3-efs-1.28.16/mypy_boto3_efs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-01 11:36:42.000000 mypy-boto3-efs-1.28.16/mypy_boto3_efs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:42.508901 mypy-boto3-efs-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-08-01 11:17:01.000000 mypy-boto3-efs-1.28.16/setup.py
```

### Comparing `mypy-boto3-efs-1.28.15.post1/LICENSE` & `mypy-boto3-efs-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-efs-1.28.15.post1/PKG-INFO` & `mypy-boto3-efs-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-efs
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.EFS 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.EFS 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_efs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 efs type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 efs type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-efs.svg?color=blue)](https://pypi.org/project/mypy-boto3-efs)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_efs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-efs)](https://pepy.tech/project/mypy-boto3-efs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EFS 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS)
+[boto3.EFS 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS)
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
 [mypy-boto3-efs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_efs/).
 
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
@@ -329,20 +329,20 @@
 )
 
 
 def check_value(value: DescribeFileSystemsPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_efs.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_efs.type_defs import (
     PosixUserOutputTypeDef,
     ResponseMetadataTypeDef,
     TagTypeDef,
     BackupPolicyTypeDef,
@@ -385,14 +385,15 @@
     CreateFileSystemRequestRequestTypeDef,
     CreateTagsRequestRequestTypeDef,
     DescribeTagsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     BackupPolicyDescriptionTypeDef,
     PutBackupPolicyRequestRequestTypeDef,
+    PosixUserUnionTypeDef,
     CreateReplicationConfigurationRequestRequestTypeDef,
     RootDirectoryTypeDef,
     DescribeAccountPreferencesResponseTypeDef,
     PutAccountPreferencesResponseTypeDef,
     DescribeFileSystemsRequestDescribeFileSystemsPaginateTypeDef,
     DescribeMountTargetsRequestDescribeMountTargetsPaginateTypeDef,
     DescribeTagsRequestDescribeTagsPaginateTypeDef,
@@ -408,15 +409,15 @@
     CreateAccessPointRequestRequestTypeDef,
     DescribeReplicationConfigurationsResponseTypeDef,
     DescribeFileSystemsResponseTypeDef,
     DescribeAccessPointsResponseTypeDef,
 )
 
 
-def get_structure() -> PosixUserOutputTypeDef:
+def get_value() -> PosixUserOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-efs-1.28.15.post1/README.md` & `mypy-boto3-efs-1.28.16/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-efs.svg?color=blue)](https://pypi.org/project/mypy-boto3-efs)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_efs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-efs)](https://pepy.tech/project/mypy-boto3-efs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EFS 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS)
+[boto3.EFS 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS)
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
 [mypy-boto3-efs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_efs/).
 
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
@@ -297,20 +297,20 @@
 )
 
 
 def check_value(value: DescribeFileSystemsPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_efs.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_efs.type_defs import (
     PosixUserOutputTypeDef,
     ResponseMetadataTypeDef,
     TagTypeDef,
     BackupPolicyTypeDef,
@@ -353,14 +353,15 @@
     CreateFileSystemRequestRequestTypeDef,
     CreateTagsRequestRequestTypeDef,
     DescribeTagsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     BackupPolicyDescriptionTypeDef,
     PutBackupPolicyRequestRequestTypeDef,
+    PosixUserUnionTypeDef,
     CreateReplicationConfigurationRequestRequestTypeDef,
     RootDirectoryTypeDef,
     DescribeAccountPreferencesResponseTypeDef,
     PutAccountPreferencesResponseTypeDef,
     DescribeFileSystemsRequestDescribeFileSystemsPaginateTypeDef,
     DescribeMountTargetsRequestDescribeMountTargetsPaginateTypeDef,
     DescribeTagsRequestDescribeTagsPaginateTypeDef,
@@ -376,15 +377,15 @@
     CreateAccessPointRequestRequestTypeDef,
     DescribeReplicationConfigurationsResponseTypeDef,
     DescribeFileSystemsResponseTypeDef,
     DescribeAccessPointsResponseTypeDef,
 )
 
 
-def get_structure() -> PosixUserOutputTypeDef:
+def get_value() -> PosixUserOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-efs-1.28.15.post1/mypy_boto3_efs/__init__.py` & `mypy-boto3-efs-1.28.16/mypy_boto3_efs/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-efs-1.28.15.post1/mypy_boto3_efs/__init__.pyi` & `mypy-boto3-efs-1.28.16/mypy_boto3_efs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-efs-1.28.15.post1/mypy_boto3_efs/__main__.py` & `mypy-boto3-efs-1.28.16/mypy_boto3_efs/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.EFS 1.28.15\nVersion:         1.28.15.post1\nBuilder version:"
-        " 7.16.2\nDocs:           "
+        "Type annotations for boto3.EFS 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_efs//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS\nOther"
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

### Comparing `mypy-boto3-efs-1.28.15.post1/mypy_boto3_efs/client.py` & `mypy-boto3-efs-1.28.16/mypy_boto3_efs/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_efs.client import EFSClient
 
     session = Session()
     client: EFSClient = session.client("efs")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import PerformanceModeType, ResourceIdTypeType, ThroughputModeType
 from .paginator import (
     DescribeFileSystemsPaginator,
     DescribeMountTargetsPaginator,
@@ -39,16 +39,15 @@
     EmptyResponseMetadataTypeDef,
     FileSystemDescriptionResponseTypeDef,
     FileSystemPolicyDescriptionTypeDef,
     LifecycleConfigurationDescriptionTypeDef,
     LifecyclePolicyTypeDef,
     ListTagsForResourceResponseTypeDef,
     MountTargetDescriptionResponseTypeDef,
-    PosixUserOutputTypeDef,
-    PosixUserTypeDef,
+    PosixUserUnionTypeDef,
     PutAccountPreferencesResponseTypeDef,
     ReplicationConfigurationDescriptionResponseTypeDef,
     RootDirectoryTypeDef,
     TagTypeDef,
 )
 
 if sys.version_info >= (3, 9):
@@ -137,15 +136,15 @@
 
     def create_access_point(
         self,
         *,
         ClientToken: str,
         FileSystemId: str,
         Tags: Sequence[TagTypeDef] = ...,
-        PosixUser: Union[PosixUserTypeDef, PosixUserOutputTypeDef] = ...,
+        PosixUser: PosixUserUnionTypeDef = ...,
         RootDirectory: RootDirectoryTypeDef = ...
     ) -> AccessPointDescriptionResponseTypeDef:
         """
         Creates an EFS access point.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Client.create_access_point)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_efs/client/#create_access_point)
```

### Comparing `mypy-boto3-efs-1.28.15.post1/mypy_boto3_efs/client.pyi` & `mypy-boto3-efs-1.28.16/mypy_boto3_efs/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_efs.client import EFSClient
 
     session = Session()
     client: EFSClient = session.client("efs")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import PerformanceModeType, ResourceIdTypeType, ThroughputModeType
 from .paginator import (
     DescribeFileSystemsPaginator,
     DescribeMountTargetsPaginator,
@@ -39,16 +39,15 @@
     EmptyResponseMetadataTypeDef,
     FileSystemDescriptionResponseTypeDef,
     FileSystemPolicyDescriptionTypeDef,
     LifecycleConfigurationDescriptionTypeDef,
     LifecyclePolicyTypeDef,
     ListTagsForResourceResponseTypeDef,
     MountTargetDescriptionResponseTypeDef,
-    PosixUserOutputTypeDef,
-    PosixUserTypeDef,
+    PosixUserUnionTypeDef,
     PutAccountPreferencesResponseTypeDef,
     ReplicationConfigurationDescriptionResponseTypeDef,
     RootDirectoryTypeDef,
     TagTypeDef,
 )
 
 if sys.version_info >= (3, 9):
@@ -130,15 +129,15 @@
         """
     def create_access_point(
         self,
         *,
         ClientToken: str,
         FileSystemId: str,
         Tags: Sequence[TagTypeDef] = ...,
-        PosixUser: Union[PosixUserTypeDef, PosixUserOutputTypeDef] = ...,
+        PosixUser: PosixUserUnionTypeDef = ...,
         RootDirectory: RootDirectoryTypeDef = ...
     ) -> AccessPointDescriptionResponseTypeDef:
         """
         Creates an EFS access point.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Client.create_access_point)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_efs/client/#create_access_point)
```

### Comparing `mypy-boto3-efs-1.28.15.post1/mypy_boto3_efs/literals.py` & `mypy-boto3-efs-1.28.16/mypy_boto3_efs/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-efs-1.28.15.post1/mypy_boto3_efs/literals.pyi` & `mypy-boto3-efs-1.28.16/mypy_boto3_efs/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-efs-1.28.15.post1/mypy_boto3_efs/paginator.py` & `mypy-boto3-efs-1.28.16/mypy_boto3_efs/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-efs-1.28.15.post1/mypy_boto3_efs/paginator.pyi` & `mypy-boto3-efs-1.28.16/mypy_boto3_efs/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-efs-1.28.15.post1/mypy_boto3_efs/type_defs.py` & `mypy-boto3-efs-1.28.16/mypy_boto3_efs/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_efs/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_efs.type_defs import PosixUserOutputTypeDef
 
-    data: PosixUserOutputTypeDef = {...}
+    data: PosixUserOutputTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence
+from typing import Dict, List, Sequence, Union
 
 from .literals import (
     LifeCycleStateType,
     PerformanceModeType,
     ReplicationStatusType,
     ResourceIdTypeType,
     ResourceType,
@@ -80,14 +80,15 @@
     "CreateFileSystemRequestRequestTypeDef",
     "CreateTagsRequestRequestTypeDef",
     "DescribeTagsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "BackupPolicyDescriptionTypeDef",
     "PutBackupPolicyRequestRequestTypeDef",
+    "PosixUserUnionTypeDef",
     "CreateReplicationConfigurationRequestRequestTypeDef",
     "RootDirectoryTypeDef",
     "DescribeAccountPreferencesResponseTypeDef",
     "PutAccountPreferencesResponseTypeDef",
     "DescribeFileSystemsRequestDescribeFileSystemsPaginateTypeDef",
     "DescribeMountTargetsRequestDescribeMountTargetsPaginateTypeDef",
     "DescribeTagsRequestDescribeTagsPaginateTypeDef",
@@ -680,14 +681,15 @@
     "PutBackupPolicyRequestRequestTypeDef",
     {
         "FileSystemId": str,
         "BackupPolicy": BackupPolicyTypeDef,
     },
 )
 
+PosixUserUnionTypeDef = Union[PosixUserTypeDef, PosixUserOutputTypeDef]
 CreateReplicationConfigurationRequestRequestTypeDef = TypedDict(
     "CreateReplicationConfigurationRequestRequestTypeDef",
     {
         "SourceFileSystemId": str,
         "Destinations": Sequence[DestinationToCreateTypeDef],
     },
 )
```

### Comparing `mypy-boto3-efs-1.28.15.post1/mypy_boto3_efs/type_defs.pyi` & `mypy-boto3-efs-1.28.16/mypy_boto3_efs/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_efs/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_efs.type_defs import PosixUserOutputTypeDef
 
-    data: PosixUserOutputTypeDef = {...}
+    data: PosixUserOutputTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence
+from typing import Dict, List, Sequence, Union
 
 from .literals import (
     LifeCycleStateType,
     PerformanceModeType,
     ReplicationStatusType,
     ResourceIdTypeType,
     ResourceType,
@@ -79,14 +79,15 @@
     "CreateFileSystemRequestRequestTypeDef",
     "CreateTagsRequestRequestTypeDef",
     "DescribeTagsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "BackupPolicyDescriptionTypeDef",
     "PutBackupPolicyRequestRequestTypeDef",
+    "PosixUserUnionTypeDef",
     "CreateReplicationConfigurationRequestRequestTypeDef",
     "RootDirectoryTypeDef",
     "DescribeAccountPreferencesResponseTypeDef",
     "PutAccountPreferencesResponseTypeDef",
     "DescribeFileSystemsRequestDescribeFileSystemsPaginateTypeDef",
     "DescribeMountTargetsRequestDescribeMountTargetsPaginateTypeDef",
     "DescribeTagsRequestDescribeTagsPaginateTypeDef",
@@ -655,14 +656,15 @@
     "PutBackupPolicyRequestRequestTypeDef",
     {
         "FileSystemId": str,
         "BackupPolicy": BackupPolicyTypeDef,
     },
 )
 
+PosixUserUnionTypeDef = Union[PosixUserTypeDef, PosixUserOutputTypeDef]
 CreateReplicationConfigurationRequestRequestTypeDef = TypedDict(
     "CreateReplicationConfigurationRequestRequestTypeDef",
     {
         "SourceFileSystemId": str,
         "Destinations": Sequence[DestinationToCreateTypeDef],
     },
 )
```

### Comparing `mypy-boto3-efs-1.28.15.post1/mypy_boto3_efs.egg-info/PKG-INFO` & `mypy-boto3-efs-1.28.16/mypy_boto3_efs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-efs
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.EFS 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.EFS 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_efs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 efs type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 efs type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-efs.svg?color=blue)](https://pypi.org/project/mypy-boto3-efs)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_efs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-efs)](https://pepy.tech/project/mypy-boto3-efs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EFS 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS)
+[boto3.EFS 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS)
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
 [mypy-boto3-efs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_efs/).
 
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
@@ -329,20 +329,20 @@
 )
 
 
 def check_value(value: DescribeFileSystemsPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_efs.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_efs.type_defs import (
     PosixUserOutputTypeDef,
     ResponseMetadataTypeDef,
     TagTypeDef,
     BackupPolicyTypeDef,
@@ -385,14 +385,15 @@
     CreateFileSystemRequestRequestTypeDef,
     CreateTagsRequestRequestTypeDef,
     DescribeTagsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     BackupPolicyDescriptionTypeDef,
     PutBackupPolicyRequestRequestTypeDef,
+    PosixUserUnionTypeDef,
     CreateReplicationConfigurationRequestRequestTypeDef,
     RootDirectoryTypeDef,
     DescribeAccountPreferencesResponseTypeDef,
     PutAccountPreferencesResponseTypeDef,
     DescribeFileSystemsRequestDescribeFileSystemsPaginateTypeDef,
     DescribeMountTargetsRequestDescribeMountTargetsPaginateTypeDef,
     DescribeTagsRequestDescribeTagsPaginateTypeDef,
@@ -408,15 +409,15 @@
     CreateAccessPointRequestRequestTypeDef,
     DescribeReplicationConfigurationsResponseTypeDef,
     DescribeFileSystemsResponseTypeDef,
     DescribeAccessPointsResponseTypeDef,
 )
 
 
-def get_structure() -> PosixUserOutputTypeDef:
+def get_value() -> PosixUserOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-efs-1.28.15.post1/mypy_boto3_efs.egg-info/SOURCES.txt` & `mypy-boto3-efs-1.28.16/mypy_boto3_efs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-efs-1.28.15.post1/setup.py` & `mypy-boto3-efs-1.28.16/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-efs",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_efs"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.EFS 1.28.15 service generated with mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.EFS 1.28.16 service generated with mypy-boto3-builder 7.17.1"
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
-    keywords="boto3 efs type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 efs type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_efs": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_efs/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

