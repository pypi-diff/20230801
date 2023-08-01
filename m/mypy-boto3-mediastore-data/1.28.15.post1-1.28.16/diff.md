# Comparing `tmp/mypy-boto3-mediastore-data-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-mediastore-data-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-mediastore-data-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:40 2023, max compression
+gzip compressed data, was "mypy-boto3-mediastore-data-1.28.16.tar", last modified: Tue Aug  1 11:37:20 2023, max compression
```

## Comparing `mypy-boto3-mediastore-data-1.28.15.post1.tar` & `mypy-boto3-mediastore-data-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:40.781284 mypy-boto3-mediastore-data-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:51:19.000000 mypy-boto3-mediastore-data-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13380 2023-07-29 10:03:40.781284 mypy-boto3-mediastore-data-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11856 2023-07-29 09:51:19.000000 mypy-boto3-mediastore-data-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:40.769284 mypy-boto3-mediastore-data-1.28.15.post1/mypy_boto3_mediastore_data/
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-07-29 09:51:19.000000 mypy-boto3-mediastore-data-1.28.15.post1/mypy_boto3_mediastore_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-29 09:51:19.000000 mypy-boto3-mediastore-data-1.28.15.post1/mypy_boto3_mediastore_data/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-29 09:51:19.000000 mypy-boto3-mediastore-data-1.28.15.post1/mypy_boto3_mediastore_data/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6708 2023-07-29 09:51:19.000000 mypy-boto3-mediastore-data-1.28.15.post1/mypy_boto3_mediastore_data/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-07-29 09:51:19.000000 mypy-boto3-mediastore-data-1.28.15.post1/mypy_boto3_mediastore_data/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8192 2023-07-29 09:51:19.000000 mypy-boto3-mediastore-data-1.28.15.post1/mypy_boto3_mediastore_data/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8190 2023-07-29 09:51:19.000000 mypy-boto3-mediastore-data-1.28.15.post1/mypy_boto3_mediastore_data/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-07-29 09:51:19.000000 mypy-boto3-mediastore-data-1.28.15.post1/mypy_boto3_mediastore_data/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-07-29 09:51:19.000000 mypy-boto3-mediastore-data-1.28.15.post1/mypy_boto3_mediastore_data/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:51:19.000000 mypy-boto3-mediastore-data-1.28.15.post1/mypy_boto3_mediastore_data/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     4689 2023-07-29 09:51:19.000000 mypy-boto3-mediastore-data-1.28.15.post1/mypy_boto3_mediastore_data/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-07-29 09:51:19.000000 mypy-boto3-mediastore-data-1.28.15.post1/mypy_boto3_mediastore_data/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:51:19.000000 mypy-boto3-mediastore-data-1.28.15.post1/mypy_boto3_mediastore_data/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:40.781284 mypy-boto3-mediastore-data-1.28.15.post1/mypy_boto3_mediastore_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13380 2023-07-29 10:03:40.000000 mypy-boto3-mediastore-data-1.28.15.post1/mypy_boto3_mediastore_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-29 10:03:40.000000 mypy-boto3-mediastore-data-1.28.15.post1/mypy_boto3_mediastore_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:40.000000 mypy-boto3-mediastore-data-1.28.15.post1/mypy_boto3_mediastore_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:40.000000 mypy-boto3-mediastore-data-1.28.15.post1/mypy_boto3_mediastore_data.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:40.000000 mypy-boto3-mediastore-data-1.28.15.post1/mypy_boto3_mediastore_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-29 10:03:40.000000 mypy-boto3-mediastore-data-1.28.15.post1/mypy_boto3_mediastore_data.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:40.781284 mypy-boto3-mediastore-data-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-07-29 09:51:18.000000 mypy-boto3-mediastore-data-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:20.668821 mypy-boto3-mediastore-data-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:24:17.000000 mypy-boto3-mediastore-data-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13365 2023-08-01 11:37:20.660821 mypy-boto3-mediastore-data-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11850 2023-08-01 11:24:17.000000 mypy-boto3-mediastore-data-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:20.656821 mypy-boto3-mediastore-data-1.28.16/mypy_boto3_mediastore_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-08-01 11:24:17.000000 mypy-boto3-mediastore-data-1.28.16/mypy_boto3_mediastore_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-08-01 11:24:17.000000 mypy-boto3-mediastore-data-1.28.16/mypy_boto3_mediastore_data/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-08-01 11:24:17.000000 mypy-boto3-mediastore-data-1.28.16/mypy_boto3_mediastore_data/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6640 2023-08-01 11:24:17.000000 mypy-boto3-mediastore-data-1.28.16/mypy_boto3_mediastore_data/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6627 2023-08-01 11:24:17.000000 mypy-boto3-mediastore-data-1.28.16/mypy_boto3_mediastore_data/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8192 2023-08-01 11:24:17.000000 mypy-boto3-mediastore-data-1.28.16/mypy_boto3_mediastore_data/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8190 2023-08-01 11:24:17.000000 mypy-boto3-mediastore-data-1.28.16/mypy_boto3_mediastore_data/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-08-01 11:24:17.000000 mypy-boto3-mediastore-data-1.28.16/mypy_boto3_mediastore_data/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-08-01 11:24:17.000000 mypy-boto3-mediastore-data-1.28.16/mypy_boto3_mediastore_data/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:24:17.000000 mypy-boto3-mediastore-data-1.28.16/mypy_boto3_mediastore_data/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     4688 2023-08-01 11:24:17.000000 mypy-boto3-mediastore-data-1.28.16/mypy_boto3_mediastore_data/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-08-01 11:24:17.000000 mypy-boto3-mediastore-data-1.28.16/mypy_boto3_mediastore_data/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:24:17.000000 mypy-boto3-mediastore-data-1.28.16/mypy_boto3_mediastore_data/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:20.660821 mypy-boto3-mediastore-data-1.28.16/mypy_boto3_mediastore_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13365 2023-08-01 11:37:20.000000 mypy-boto3-mediastore-data-1.28.16/mypy_boto3_mediastore_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-08-01 11:37:20.000000 mypy-boto3-mediastore-data-1.28.16/mypy_boto3_mediastore_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:20.000000 mypy-boto3-mediastore-data-1.28.16/mypy_boto3_mediastore_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:20.000000 mypy-boto3-mediastore-data-1.28.16/mypy_boto3_mediastore_data.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:20.000000 mypy-boto3-mediastore-data-1.28.16/mypy_boto3_mediastore_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-01 11:37:20.000000 mypy-boto3-mediastore-data-1.28.16/mypy_boto3_mediastore_data.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:20.668821 mypy-boto3-mediastore-data-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-08-01 11:24:17.000000 mypy-boto3-mediastore-data-1.28.16/setup.py
```

### Comparing `mypy-boto3-mediastore-data-1.28.15.post1/LICENSE` & `mypy-boto3-mediastore-data-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediastore-data-1.28.15.post1/PKG-INFO` & `mypy-boto3-mediastore-data-1.28.16/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mediastore-data
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.MediaStoreData 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.MediaStoreData 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore_data/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 mediastore-data type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 mediastore-data type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediastore-data.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediastore-data)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore_data/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mediastore-data)](https://pepy.tech/project/mypy-boto3-mediastore-data)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaStoreData 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore-data.html#MediaStoreData)
+[boto3.MediaStoreData 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore-data.html#MediaStoreData)
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
 [mypy-boto3-mediastore-data docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore_data/).
 
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
@@ -314,23 +314,24 @@
 )
 
 
 def check_value(value: ItemTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_mediastore_data.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_mediastore_data.type_defs import (
+    BlobTypeDef,
     DeleteObjectRequestRequestTypeDef,
     DescribeObjectRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     GetObjectRequestRequestTypeDef,
     ItemTypeDef,
     PaginatorConfigTypeDef,
     ListItemsRequestRequestTypeDef,
@@ -339,15 +340,15 @@
     GetObjectResponseTypeDef,
     PutObjectResponseTypeDef,
     ListItemsResponseTypeDef,
     ListItemsRequestListItemsPaginateTypeDef,
 )
 
 
-def get_structure() -> DeleteObjectRequestRequestTypeDef:
+def get_value() -> BlobTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-mediastore-data-1.28.15.post1/README.md` & `mypy-boto3-mediastore-data-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediastore-data.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediastore-data)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore_data/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mediastore-data)](https://pepy.tech/project/mypy-boto3-mediastore-data)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaStoreData 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore-data.html#MediaStoreData)
+[boto3.MediaStoreData 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore-data.html#MediaStoreData)
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
 [mypy-boto3-mediastore-data docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore_data/).
 
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
@@ -282,23 +282,24 @@
 )
 
 
 def check_value(value: ItemTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_mediastore_data.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_mediastore_data.type_defs import (
+    BlobTypeDef,
     DeleteObjectRequestRequestTypeDef,
     DescribeObjectRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     GetObjectRequestRequestTypeDef,
     ItemTypeDef,
     PaginatorConfigTypeDef,
     ListItemsRequestRequestTypeDef,
@@ -307,15 +308,15 @@
     GetObjectResponseTypeDef,
     PutObjectResponseTypeDef,
     ListItemsResponseTypeDef,
     ListItemsRequestListItemsPaginateTypeDef,
 )
 
 
-def get_structure() -> DeleteObjectRequestRequestTypeDef:
+def get_value() -> BlobTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-mediastore-data-1.28.15.post1/mypy_boto3_mediastore_data/__init__.py` & `mypy-boto3-mediastore-data-1.28.16/mypy_boto3_mediastore_data/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediastore-data-1.28.15.post1/mypy_boto3_mediastore_data/__init__.pyi` & `mypy-boto3-mediastore-data-1.28.16/mypy_boto3_mediastore_data/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediastore-data-1.28.15.post1/mypy_boto3_mediastore_data/client.py` & `mypy-boto3-mediastore-data-1.28.16/mypy_boto3_mediastore_data/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,22 +10,22 @@
     from mypy_boto3_mediastore_data.client import MediaStoreDataClient
 
     session = Session()
     client: MediaStoreDataClient = session.client("mediastore-data")
     ```
 """
 import sys
-from typing import IO, Any, Dict, Mapping, Type, Union
+from typing import Any, Dict, Mapping, Type
 
 from botocore.client import BaseClient, ClientMeta
-from botocore.response import StreamingBody
 
 from .literals import UploadAvailabilityType
 from .paginator import ListItemsPaginator
 from .type_defs import (
+    BlobTypeDef,
     DescribeObjectResponseTypeDef,
     GetObjectResponseTypeDef,
     ListItemsResponseTypeDef,
     PutObjectResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
@@ -134,15 +134,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore-data.html#MediaStoreData.Client.list_items)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore_data/client/#list_items)
         """
 
     def put_object(
         self,
         *,
-        Body: Union[str, bytes, IO[Any], StreamingBody],
+        Body: BlobTypeDef,
         Path: str,
         ContentType: str = ...,
         CacheControl: str = ...,
         StorageClass: Literal["TEMPORAL"] = ...,
         UploadAvailability: UploadAvailabilityType = ...
     ) -> PutObjectResponseTypeDef:
         """
```

### Comparing `mypy-boto3-mediastore-data-1.28.15.post1/mypy_boto3_mediastore_data/client.pyi` & `mypy-boto3-mediastore-data-1.28.16/mypy_boto3_mediastore_data/client.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -10,22 +10,22 @@
     from mypy_boto3_mediastore_data.client import MediaStoreDataClient
 
     session = Session()
     client: MediaStoreDataClient = session.client("mediastore-data")
     ```
 """
 import sys
-from typing import IO, Any, Dict, Mapping, Type, Union
+from typing import Any, Dict, Mapping, Type
 
 from botocore.client import BaseClient, ClientMeta
-from botocore.response import StreamingBody
 
 from .literals import UploadAvailabilityType
 from .paginator import ListItemsPaginator
 from .type_defs import (
+    BlobTypeDef,
     DescribeObjectResponseTypeDef,
     GetObjectResponseTypeDef,
     ListItemsResponseTypeDef,
     PutObjectResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
@@ -122,15 +122,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore-data.html#MediaStoreData.Client.list_items)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore_data/client/#list_items)
         """
     def put_object(
         self,
         *,
-        Body: Union[str, bytes, IO[Any], StreamingBody],
+        Body: BlobTypeDef,
         Path: str,
         ContentType: str = ...,
         CacheControl: str = ...,
         StorageClass: Literal["TEMPORAL"] = ...,
         UploadAvailability: UploadAvailabilityType = ...
     ) -> PutObjectResponseTypeDef:
         """
```

### Comparing `mypy-boto3-mediastore-data-1.28.15.post1/mypy_boto3_mediastore_data/literals.py` & `mypy-boto3-mediastore-data-1.28.16/mypy_boto3_mediastore_data/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediastore-data-1.28.15.post1/mypy_boto3_mediastore_data/literals.pyi` & `mypy-boto3-mediastore-data-1.28.16/mypy_boto3_mediastore_data/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediastore-data-1.28.15.post1/mypy_boto3_mediastore_data/paginator.py` & `mypy-boto3-mediastore-data-1.28.16/mypy_boto3_mediastore_data/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediastore-data-1.28.15.post1/mypy_boto3_mediastore_data/paginator.pyi` & `mypy-boto3-mediastore-data-1.28.16/mypy_boto3_mediastore_data/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediastore-data-1.28.15.post1/mypy_boto3_mediastore_data/type_defs.py` & `mypy-boto3-mediastore-data-1.28.16/mypy_boto3_mediastore_data/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for mediastore-data service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore_data/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_mediastore_data.type_defs import DeleteObjectRequestRequestTypeDef
+    from mypy_boto3_mediastore_data.type_defs import BlobTypeDef
 
-    data: DeleteObjectRequestRequestTypeDef = {...}
+    data: BlobTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Union
 
 from botocore.response import StreamingBody
@@ -26,14 +26,15 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
+    "BlobTypeDef",
     "DeleteObjectRequestRequestTypeDef",
     "DescribeObjectRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "GetObjectRequestRequestTypeDef",
     "ItemTypeDef",
     "PaginatorConfigTypeDef",
     "ListItemsRequestRequestTypeDef",
@@ -41,14 +42,15 @@
     "DescribeObjectResponseTypeDef",
     "GetObjectResponseTypeDef",
     "PutObjectResponseTypeDef",
     "ListItemsResponseTypeDef",
     "ListItemsRequestListItemsPaginateTypeDef",
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 DeleteObjectRequestRequestTypeDef = TypedDict(
     "DeleteObjectRequestRequestTypeDef",
     {
         "Path": str,
     },
 )
 
@@ -123,15 +125,15 @@
     },
     total=False,
 )
 
 _RequiredPutObjectRequestRequestTypeDef = TypedDict(
     "_RequiredPutObjectRequestRequestTypeDef",
     {
-        "Body": Union[str, bytes, IO[Any], StreamingBody],
+        "Body": BlobTypeDef,
         "Path": str,
     },
 )
 _OptionalPutObjectRequestRequestTypeDef = TypedDict(
     "_OptionalPutObjectRequestRequestTypeDef",
     {
         "ContentType": str,
```

### Comparing `mypy-boto3-mediastore-data-1.28.15.post1/mypy_boto3_mediastore_data/type_defs.pyi` & `mypy-boto3-mediastore-data-1.28.16/mypy_boto3_mediastore_data/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for mediastore-data service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore_data/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_mediastore_data.type_defs import DeleteObjectRequestRequestTypeDef
+    from mypy_boto3_mediastore_data.type_defs import BlobTypeDef
 
-    data: DeleteObjectRequestRequestTypeDef = {...}
+    data: BlobTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Union
 
 from botocore.response import StreamingBody
@@ -25,14 +25,15 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
+    "BlobTypeDef",
     "DeleteObjectRequestRequestTypeDef",
     "DescribeObjectRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "GetObjectRequestRequestTypeDef",
     "ItemTypeDef",
     "PaginatorConfigTypeDef",
     "ListItemsRequestRequestTypeDef",
@@ -40,14 +41,15 @@
     "DescribeObjectResponseTypeDef",
     "GetObjectResponseTypeDef",
     "PutObjectResponseTypeDef",
     "ListItemsResponseTypeDef",
     "ListItemsRequestListItemsPaginateTypeDef",
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 DeleteObjectRequestRequestTypeDef = TypedDict(
     "DeleteObjectRequestRequestTypeDef",
     {
         "Path": str,
     },
 )
 
@@ -120,15 +122,15 @@
     },
     total=False,
 )
 
 _RequiredPutObjectRequestRequestTypeDef = TypedDict(
     "_RequiredPutObjectRequestRequestTypeDef",
     {
-        "Body": Union[str, bytes, IO[Any], StreamingBody],
+        "Body": BlobTypeDef,
         "Path": str,
     },
 )
 _OptionalPutObjectRequestRequestTypeDef = TypedDict(
     "_OptionalPutObjectRequestRequestTypeDef",
     {
         "ContentType": str,
```

### Comparing `mypy-boto3-mediastore-data-1.28.15.post1/mypy_boto3_mediastore_data.egg-info/PKG-INFO` & `mypy-boto3-mediastore-data-1.28.16/mypy_boto3_mediastore_data.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mediastore-data
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.MediaStoreData 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.MediaStoreData 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore_data/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 mediastore-data type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 mediastore-data type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediastore-data.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediastore-data)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore_data/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mediastore-data)](https://pepy.tech/project/mypy-boto3-mediastore-data)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaStoreData 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore-data.html#MediaStoreData)
+[boto3.MediaStoreData 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore-data.html#MediaStoreData)
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
 [mypy-boto3-mediastore-data docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore_data/).
 
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
@@ -314,23 +314,24 @@
 )
 
 
 def check_value(value: ItemTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_mediastore_data.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_mediastore_data.type_defs import (
+    BlobTypeDef,
     DeleteObjectRequestRequestTypeDef,
     DescribeObjectRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     GetObjectRequestRequestTypeDef,
     ItemTypeDef,
     PaginatorConfigTypeDef,
     ListItemsRequestRequestTypeDef,
@@ -339,15 +340,15 @@
     GetObjectResponseTypeDef,
     PutObjectResponseTypeDef,
     ListItemsResponseTypeDef,
     ListItemsRequestListItemsPaginateTypeDef,
 )
 
 
-def get_structure() -> DeleteObjectRequestRequestTypeDef:
+def get_value() -> BlobTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-mediastore-data-1.28.15.post1/mypy_boto3_mediastore_data.egg-info/SOURCES.txt` & `mypy-boto3-mediastore-data-1.28.16/mypy_boto3_mediastore_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediastore-data-1.28.15.post1/setup.py` & `mypy-boto3-mediastore-data-1.28.16/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-mediastore-data",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_mediastore_data"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.MediaStoreData 1.28.15 service generated with"
-        " mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.MediaStoreData 1.28.16 service generated with"
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
-    keywords="boto3 mediastore-data type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 mediastore-data type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_mediastore_data": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore_data/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

