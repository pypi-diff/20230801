# Comparing `tmp/mypy-boto3-cur-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-cur-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-cur-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:54 2023, max compression
+gzip compressed data, was "mypy-boto3-cur-1.28.16.tar", last modified: Tue Aug  1 11:36:35 2023, max compression
```

## Comparing `mypy-boto3-cur-1.28.15.post1.tar` & `mypy-boto3-cur-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:54.085095 mypy-boto3-cur-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:41:49.000000 mypy-boto3-cur-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13192 2023-07-29 10:02:54.085095 mypy-boto3-cur-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11693 2023-07-29 09:41:49.000000 mypy-boto3-cur-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:54.081095 mypy-boto3-cur-1.28.15.post1/mypy_boto3_cur/
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-07-29 09:41:49.000000 mypy-boto3-cur-1.28.15.post1/mypy_boto3_cur/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-07-29 09:41:49.000000 mypy-boto3-cur-1.28.15.post1/mypy_boto3_cur/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-29 09:41:49.000000 mypy-boto3-cur-1.28.15.post1/mypy_boto3_cur/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6217 2023-07-29 09:41:49.000000 mypy-boto3-cur-1.28.15.post1/mypy_boto3_cur/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6205 2023-07-29 09:41:49.000000 mypy-boto3-cur-1.28.15.post1/mypy_boto3_cur/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8971 2023-07-29 09:41:49.000000 mypy-boto3-cur-1.28.15.post1/mypy_boto3_cur/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-07-29 09:41:49.000000 mypy-boto3-cur-1.28.15.post1/mypy_boto3_cur/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-29 09:41:49.000000 mypy-boto3-cur-1.28.15.post1/mypy_boto3_cur/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-07-29 09:41:49.000000 mypy-boto3-cur-1.28.15.post1/mypy_boto3_cur/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:41:49.000000 mypy-boto3-cur-1.28.15.post1/mypy_boto3_cur/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-07-29 09:41:49.000000 mypy-boto3-cur-1.28.15.post1/mypy_boto3_cur/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4726 2023-07-29 09:41:49.000000 mypy-boto3-cur-1.28.15.post1/mypy_boto3_cur/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:41:49.000000 mypy-boto3-cur-1.28.15.post1/mypy_boto3_cur/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:54.085095 mypy-boto3-cur-1.28.15.post1/mypy_boto3_cur.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13192 2023-07-29 10:02:53.000000 mypy-boto3-cur-1.28.15.post1/mypy_boto3_cur.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-29 10:02:53.000000 mypy-boto3-cur-1.28.15.post1/mypy_boto3_cur.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:53.000000 mypy-boto3-cur-1.28.15.post1/mypy_boto3_cur.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:53.000000 mypy-boto3-cur-1.28.15.post1/mypy_boto3_cur.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:53.000000 mypy-boto3-cur-1.28.15.post1/mypy_boto3_cur.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-29 10:02:53.000000 mypy-boto3-cur-1.28.15.post1/mypy_boto3_cur.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:54.085095 mypy-boto3-cur-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-29 09:41:49.000000 mypy-boto3-cur-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:35.120913 mypy-boto3-cur-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:14:21.000000 mypy-boto3-cur-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13216 2023-08-01 11:36:35.120913 mypy-boto3-cur-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11726 2023-08-01 11:14:21.000000 mypy-boto3-cur-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:35.112913 mypy-boto3-cur-1.28.16/mypy_boto3_cur/
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-08-01 11:14:21.000000 mypy-boto3-cur-1.28.16/mypy_boto3_cur/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-08-01 11:14:21.000000 mypy-boto3-cur-1.28.16/mypy_boto3_cur/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-08-01 11:14:21.000000 mypy-boto3-cur-1.28.16/mypy_boto3_cur/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6090 2023-08-01 11:14:21.000000 mypy-boto3-cur-1.28.16/mypy_boto3_cur/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6078 2023-08-01 11:14:21.000000 mypy-boto3-cur-1.28.16/mypy_boto3_cur/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8971 2023-08-01 11:14:22.000000 mypy-boto3-cur-1.28.16/mypy_boto3_cur/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-08-01 11:14:22.000000 mypy-boto3-cur-1.28.16/mypy_boto3_cur/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-08-01 11:14:21.000000 mypy-boto3-cur-1.28.16/mypy_boto3_cur/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-08-01 11:14:21.000000 mypy-boto3-cur-1.28.16/mypy_boto3_cur/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:14:21.000000 mypy-boto3-cur-1.28.16/mypy_boto3_cur/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-08-01 11:14:22.000000 mypy-boto3-cur-1.28.16/mypy_boto3_cur/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-08-01 11:14:22.000000 mypy-boto3-cur-1.28.16/mypy_boto3_cur/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:14:21.000000 mypy-boto3-cur-1.28.16/mypy_boto3_cur/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:35.120913 mypy-boto3-cur-1.28.16/mypy_boto3_cur.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13216 2023-08-01 11:36:34.000000 mypy-boto3-cur-1.28.16/mypy_boto3_cur.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-08-01 11:36:34.000000 mypy-boto3-cur-1.28.16/mypy_boto3_cur.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:34.000000 mypy-boto3-cur-1.28.16/mypy_boto3_cur.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:34.000000 mypy-boto3-cur-1.28.16/mypy_boto3_cur.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:34.000000 mypy-boto3-cur-1.28.16/mypy_boto3_cur.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-01 11:36:34.000000 mypy-boto3-cur-1.28.16/mypy_boto3_cur.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:35.120913 mypy-boto3-cur-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-08-01 11:14:21.000000 mypy-boto3-cur-1.28.16/setup.py
```

### Comparing `mypy-boto3-cur-1.28.15.post1/LICENSE` & `mypy-boto3-cur-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cur-1.28.15.post1/PKG-INFO` & `mypy-boto3-cur-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cur
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.CostandUsageReportService 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.CostandUsageReportService 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cur/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 cur type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 cur type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cur.svg?color=blue)](https://pypi.org/project/mypy-boto3-cur)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cur/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cur)](https://pepy.tech/project/mypy-boto3-cur)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CostandUsageReportService 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService)
+[boto3.CostandUsageReportService 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService)
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
 [mypy-boto3-cur docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cur/).
 
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
@@ -318,38 +318,39 @@
 )
 
 
 def check_value(value: AWSRegionType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_cur.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_cur.type_defs import (
     DeleteReportDefinitionRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     PaginatorConfigTypeDef,
     DescribeReportDefinitionsRequestRequestTypeDef,
     ReportDefinitionOutputTypeDef,
     ReportDefinitionTypeDef,
     DeleteReportDefinitionResponseTypeDef,
     DescribeReportDefinitionsRequestDescribeReportDefinitionsPaginateTypeDef,
     DescribeReportDefinitionsResponseTypeDef,
     ModifyReportDefinitionRequestRequestTypeDef,
     PutReportDefinitionRequestRequestTypeDef,
+    ReportDefinitionUnionTypeDef,
 )
 
 
-def get_structure() -> DeleteReportDefinitionRequestRequestTypeDef:
+def get_value() -> DeleteReportDefinitionRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-cur-1.28.15.post1/README.md` & `mypy-boto3-cur-1.28.16/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cur.svg?color=blue)](https://pypi.org/project/mypy-boto3-cur)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cur/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cur)](https://pepy.tech/project/mypy-boto3-cur)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CostandUsageReportService 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService)
+[boto3.CostandUsageReportService 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService)
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
 [mypy-boto3-cur docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cur/).
 
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
@@ -286,38 +286,39 @@
 )
 
 
 def check_value(value: AWSRegionType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_cur.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_cur.type_defs import (
     DeleteReportDefinitionRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     PaginatorConfigTypeDef,
     DescribeReportDefinitionsRequestRequestTypeDef,
     ReportDefinitionOutputTypeDef,
     ReportDefinitionTypeDef,
     DeleteReportDefinitionResponseTypeDef,
     DescribeReportDefinitionsRequestDescribeReportDefinitionsPaginateTypeDef,
     DescribeReportDefinitionsResponseTypeDef,
     ModifyReportDefinitionRequestRequestTypeDef,
     PutReportDefinitionRequestRequestTypeDef,
+    ReportDefinitionUnionTypeDef,
 )
 
 
-def get_structure() -> DeleteReportDefinitionRequestRequestTypeDef:
+def get_value() -> DeleteReportDefinitionRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-cur-1.28.15.post1/mypy_boto3_cur/__init__.py` & `mypy-boto3-cur-1.28.16/mypy_boto3_cur/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cur-1.28.15.post1/mypy_boto3_cur/__init__.pyi` & `mypy-boto3-cur-1.28.16/mypy_boto3_cur/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cur-1.28.15.post1/mypy_boto3_cur/__main__.py` & `mypy-boto3-cur-1.28.16/mypy_boto3_cur/__main__.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CostandUsageReportService 1.28.15\nVersion:        "
-        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.CostandUsageReportService 1.28.16\nVersion:        "
+        " 1.28.16\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cur//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService\nOther"
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

### Comparing `mypy-boto3-cur-1.28.15.post1/mypy_boto3_cur/client.py` & `mypy-boto3-cur-1.28.16/mypy_boto3_cur/client.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -10,51 +10,46 @@
     from mypy_boto3_cur.client import CostandUsageReportServiceClient
 
     session = Session()
     client: CostandUsageReportServiceClient = session.client("cur")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Type, Union
+from typing import Any, Dict, Mapping, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .paginator import DescribeReportDefinitionsPaginator
 from .type_defs import (
     DeleteReportDefinitionResponseTypeDef,
     DescribeReportDefinitionsResponseTypeDef,
-    ReportDefinitionOutputTypeDef,
-    ReportDefinitionTypeDef,
+    ReportDefinitionUnionTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("CostandUsageReportServiceClient",)
 
-
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     ClientError: Type[BotocoreClientError]
     DuplicateReportNameException: Type[BotocoreClientError]
     InternalErrorException: Type[BotocoreClientError]
     ReportLimitReachedException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
-
 class CostandUsageReportServiceClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cur/client/)
     """
 
     meta: ClientMeta
@@ -63,88 +58,77 @@
     def exceptions(self) -> Exceptions:
         """
         CostandUsageReportServiceClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cur/client/#exceptions)
         """
-
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cur/client/#can_paginate)
         """
-
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cur/client/#close)
         """
-
     def delete_report_definition(
         self, *, ReportName: str = ...
     ) -> DeleteReportDefinitionResponseTypeDef:
         """
         Deletes the specified report.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService.Client.delete_report_definition)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cur/client/#delete_report_definition)
         """
-
     def describe_report_definitions(
         self, *, MaxResults: int = ..., NextToken: str = ...
     ) -> DescribeReportDefinitionsResponseTypeDef:
         """
         Lists the AWS Cost and Usage reports available to this account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService.Client.describe_report_definitions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cur/client/#describe_report_definitions)
         """
-
     def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cur/client/#generate_presigned_url)
         """
-
     def modify_report_definition(
-        self,
-        *,
-        ReportName: str,
-        ReportDefinition: Union[ReportDefinitionTypeDef, ReportDefinitionOutputTypeDef]
+        self, *, ReportName: str, ReportDefinition: ReportDefinitionUnionTypeDef
     ) -> Dict[str, Any]:
         """
         Allows you to programatically update your report preferences.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService.Client.modify_report_definition)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cur/client/#modify_report_definition)
         """
-
     def put_report_definition(
-        self, *, ReportDefinition: Union[ReportDefinitionTypeDef, ReportDefinitionOutputTypeDef]
+        self, *, ReportDefinition: ReportDefinitionUnionTypeDef
     ) -> Dict[str, Any]:
         """
         Creates a new report using the description that you provide.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService.Client.put_report_definition)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cur/client/#put_report_definition)
         """
-
     def get_paginator(
         self, operation_name: Literal["describe_report_definitions"]
     ) -> DescribeReportDefinitionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cur/client/#get_paginator)
         """
```

### Comparing `mypy-boto3-cur-1.28.15.post1/mypy_boto3_cur/client.pyi` & `mypy-boto3-cur-1.28.16/mypy_boto3_cur/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,47 +10,50 @@
     from mypy_boto3_cur.client import CostandUsageReportServiceClient
 
     session = Session()
     client: CostandUsageReportServiceClient = session.client("cur")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Type, Union
+from typing import Any, Dict, Mapping, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .paginator import DescribeReportDefinitionsPaginator
 from .type_defs import (
     DeleteReportDefinitionResponseTypeDef,
     DescribeReportDefinitionsResponseTypeDef,
-    ReportDefinitionOutputTypeDef,
-    ReportDefinitionTypeDef,
+    ReportDefinitionUnionTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = ("CostandUsageReportServiceClient",)
 
+
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     ClientError: Type[BotocoreClientError]
     DuplicateReportNameException: Type[BotocoreClientError]
     InternalErrorException: Type[BotocoreClientError]
     ReportLimitReachedException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
+
 class CostandUsageReportServiceClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cur/client/)
     """
 
     meta: ClientMeta
@@ -59,80 +62,85 @@
     def exceptions(self) -> Exceptions:
         """
         CostandUsageReportServiceClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cur/client/#exceptions)
         """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cur/client/#can_paginate)
         """
+
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cur/client/#close)
         """
+
     def delete_report_definition(
         self, *, ReportName: str = ...
     ) -> DeleteReportDefinitionResponseTypeDef:
         """
         Deletes the specified report.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService.Client.delete_report_definition)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cur/client/#delete_report_definition)
         """
+
     def describe_report_definitions(
         self, *, MaxResults: int = ..., NextToken: str = ...
     ) -> DescribeReportDefinitionsResponseTypeDef:
         """
         Lists the AWS Cost and Usage reports available to this account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService.Client.describe_report_definitions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cur/client/#describe_report_definitions)
         """
+
     def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cur/client/#generate_presigned_url)
         """
+
     def modify_report_definition(
-        self,
-        *,
-        ReportName: str,
-        ReportDefinition: Union[ReportDefinitionTypeDef, ReportDefinitionOutputTypeDef]
+        self, *, ReportName: str, ReportDefinition: ReportDefinitionUnionTypeDef
     ) -> Dict[str, Any]:
         """
         Allows you to programatically update your report preferences.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService.Client.modify_report_definition)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cur/client/#modify_report_definition)
         """
+
     def put_report_definition(
-        self, *, ReportDefinition: Union[ReportDefinitionTypeDef, ReportDefinitionOutputTypeDef]
+        self, *, ReportDefinition: ReportDefinitionUnionTypeDef
     ) -> Dict[str, Any]:
         """
         Creates a new report using the description that you provide.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService.Client.put_report_definition)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cur/client/#put_report_definition)
         """
+
     def get_paginator(
         self, operation_name: Literal["describe_report_definitions"]
     ) -> DescribeReportDefinitionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cur/client/#get_paginator)
         """
```

### Comparing `mypy-boto3-cur-1.28.15.post1/mypy_boto3_cur/literals.py` & `mypy-boto3-cur-1.28.16/mypy_boto3_cur/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cur-1.28.15.post1/mypy_boto3_cur/literals.pyi` & `mypy-boto3-cur-1.28.16/mypy_boto3_cur/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cur-1.28.15.post1/mypy_boto3_cur/paginator.py` & `mypy-boto3-cur-1.28.16/mypy_boto3_cur/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cur-1.28.15.post1/mypy_boto3_cur/paginator.pyi` & `mypy-boto3-cur-1.28.16/mypy_boto3_cur/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cur-1.28.15.post1/mypy_boto3_cur/type_defs.py` & `mypy-boto3-cur-1.28.16/mypy_boto3_cur/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cur/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_cur.type_defs import DeleteReportDefinitionRequestRequestTypeDef
 
-    data: DeleteReportDefinitionRequestRequestTypeDef = {...}
+    data: DeleteReportDefinitionRequestRequestTypeDef = ...
     ```
 """
 import sys
-from typing import Dict, List, Sequence
+from typing import Dict, List, Sequence, Union
 
 from .literals import (
     AdditionalArtifactType,
     AWSRegionType,
     CompressionFormatType,
     ReportFormatType,
     ReportVersioningType,
@@ -38,14 +38,15 @@
     "ReportDefinitionOutputTypeDef",
     "ReportDefinitionTypeDef",
     "DeleteReportDefinitionResponseTypeDef",
     "DescribeReportDefinitionsRequestDescribeReportDefinitionsPaginateTypeDef",
     "DescribeReportDefinitionsResponseTypeDef",
     "ModifyReportDefinitionRequestRequestTypeDef",
     "PutReportDefinitionRequestRequestTypeDef",
+    "ReportDefinitionUnionTypeDef",
 )
 
 DeleteReportDefinitionRequestRequestTypeDef = TypedDict(
     "DeleteReportDefinitionRequestRequestTypeDef",
     {
         "ReportName": str,
     },
@@ -177,7 +178,9 @@
 
 PutReportDefinitionRequestRequestTypeDef = TypedDict(
     "PutReportDefinitionRequestRequestTypeDef",
     {
         "ReportDefinition": ReportDefinitionTypeDef,
     },
 )
+
+ReportDefinitionUnionTypeDef = Union[ReportDefinitionTypeDef, ReportDefinitionOutputTypeDef]
```

### Comparing `mypy-boto3-cur-1.28.15.post1/mypy_boto3_cur/type_defs.pyi` & `mypy-boto3-cur-1.28.16/mypy_boto3_cur/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cur/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_cur.type_defs import DeleteReportDefinitionRequestRequestTypeDef
 
-    data: DeleteReportDefinitionRequestRequestTypeDef = {...}
+    data: DeleteReportDefinitionRequestRequestTypeDef = ...
     ```
 """
 import sys
-from typing import Dict, List, Sequence
+from typing import Dict, List, Sequence, Union
 
 from .literals import (
     AdditionalArtifactType,
     AWSRegionType,
     CompressionFormatType,
     ReportFormatType,
     ReportVersioningType,
@@ -37,14 +37,15 @@
     "ReportDefinitionOutputTypeDef",
     "ReportDefinitionTypeDef",
     "DeleteReportDefinitionResponseTypeDef",
     "DescribeReportDefinitionsRequestDescribeReportDefinitionsPaginateTypeDef",
     "DescribeReportDefinitionsResponseTypeDef",
     "ModifyReportDefinitionRequestRequestTypeDef",
     "PutReportDefinitionRequestRequestTypeDef",
+    "ReportDefinitionUnionTypeDef",
 )
 
 DeleteReportDefinitionRequestRequestTypeDef = TypedDict(
     "DeleteReportDefinitionRequestRequestTypeDef",
     {
         "ReportName": str,
     },
@@ -172,7 +173,9 @@
 
 PutReportDefinitionRequestRequestTypeDef = TypedDict(
     "PutReportDefinitionRequestRequestTypeDef",
     {
         "ReportDefinition": ReportDefinitionTypeDef,
     },
 )
+
+ReportDefinitionUnionTypeDef = Union[ReportDefinitionTypeDef, ReportDefinitionOutputTypeDef]
```

### Comparing `mypy-boto3-cur-1.28.15.post1/mypy_boto3_cur.egg-info/PKG-INFO` & `mypy-boto3-cur-1.28.16/mypy_boto3_cur.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cur
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.CostandUsageReportService 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.CostandUsageReportService 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cur/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 cur type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 cur type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cur.svg?color=blue)](https://pypi.org/project/mypy-boto3-cur)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cur/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cur)](https://pepy.tech/project/mypy-boto3-cur)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CostandUsageReportService 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService)
+[boto3.CostandUsageReportService 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService)
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
 [mypy-boto3-cur docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cur/).
 
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
@@ -318,38 +318,39 @@
 )
 
 
 def check_value(value: AWSRegionType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_cur.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_cur.type_defs import (
     DeleteReportDefinitionRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     PaginatorConfigTypeDef,
     DescribeReportDefinitionsRequestRequestTypeDef,
     ReportDefinitionOutputTypeDef,
     ReportDefinitionTypeDef,
     DeleteReportDefinitionResponseTypeDef,
     DescribeReportDefinitionsRequestDescribeReportDefinitionsPaginateTypeDef,
     DescribeReportDefinitionsResponseTypeDef,
     ModifyReportDefinitionRequestRequestTypeDef,
     PutReportDefinitionRequestRequestTypeDef,
+    ReportDefinitionUnionTypeDef,
 )
 
 
-def get_structure() -> DeleteReportDefinitionRequestRequestTypeDef:
+def get_value() -> DeleteReportDefinitionRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-cur-1.28.15.post1/mypy_boto3_cur.egg-info/SOURCES.txt` & `mypy-boto3-cur-1.28.16/mypy_boto3_cur.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cur-1.28.15.post1/setup.py` & `mypy-boto3-cur-1.28.16/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-cur",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_cur"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CostandUsageReportService 1.28.15 service generated with"
-        " mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.CostandUsageReportService 1.28.16 service generated with"
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
-    keywords="boto3 cur type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 cur type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_cur": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cur/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

