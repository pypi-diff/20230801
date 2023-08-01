# Comparing `tmp/mypy-boto3-dax-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-dax-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-dax-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:55 2023, max compression
+gzip compressed data, was "mypy-boto3-dax-1.28.16.tar", last modified: Tue Aug  1 11:36:35 2023, max compression
```

## Comparing `mypy-boto3-dax-1.28.15.post1.tar` & `mypy-boto3-dax-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:55.637100 mypy-boto3-dax-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:42:09.000000 mypy-boto3-dax-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16092 2023-07-29 10:02:55.625100 mypy-boto3-dax-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14615 2023-07-29 09:42:09.000000 mypy-boto3-dax-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:55.625100 mypy-boto3-dax-1.28.15.post1/mypy_boto3_dax/
--rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-07-29 09:42:09.000000 mypy-boto3-dax-1.28.15.post1/mypy_boto3_dax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-07-29 09:42:09.000000 mypy-boto3-dax-1.28.15.post1/mypy_boto3_dax/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-29 09:42:09.000000 mypy-boto3-dax-1.28.15.post1/mypy_boto3_dax/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20424 2023-07-29 09:42:10.000000 mypy-boto3-dax-1.28.15.post1/mypy_boto3_dax/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    20389 2023-07-29 09:42:10.000000 mypy-boto3-dax-1.28.15.post1/mypy_boto3_dax/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9344 2023-07-29 09:42:10.000000 mypy-boto3-dax-1.28.15.post1/mypy_boto3_dax/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9342 2023-07-29 09:42:10.000000 mypy-boto3-dax-1.28.15.post1/mypy_boto3_dax/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8586 2023-07-29 09:42:10.000000 mypy-boto3-dax-1.28.15.post1/mypy_boto3_dax/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8577 2023-07-29 09:42:10.000000 mypy-boto3-dax-1.28.15.post1/mypy_boto3_dax/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:42:09.000000 mypy-boto3-dax-1.28.15.post1/mypy_boto3_dax/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    22331 2023-07-29 09:42:11.000000 mypy-boto3-dax-1.28.15.post1/mypy_boto3_dax/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    22308 2023-07-29 09:42:10.000000 mypy-boto3-dax-1.28.15.post1/mypy_boto3_dax/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:42:09.000000 mypy-boto3-dax-1.28.15.post1/mypy_boto3_dax/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:55.625100 mypy-boto3-dax-1.28.15.post1/mypy_boto3_dax.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16092 2023-07-29 10:02:55.000000 mypy-boto3-dax-1.28.15.post1/mypy_boto3_dax.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-29 10:02:55.000000 mypy-boto3-dax-1.28.15.post1/mypy_boto3_dax.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:55.000000 mypy-boto3-dax-1.28.15.post1/mypy_boto3_dax.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:55.000000 mypy-boto3-dax-1.28.15.post1/mypy_boto3_dax.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:55.000000 mypy-boto3-dax-1.28.15.post1/mypy_boto3_dax.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-29 10:02:55.000000 mypy-boto3-dax-1.28.15.post1/mypy_boto3_dax.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:55.637100 mypy-boto3-dax-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-29 09:42:09.000000 mypy-boto3-dax-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:35.720912 mypy-boto3-dax-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:14:42.000000 mypy-boto3-dax-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16104 2023-08-01 11:36:35.708912 mypy-boto3-dax-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14636 2023-08-01 11:14:42.000000 mypy-boto3-dax-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:35.708912 mypy-boto3-dax-1.28.16/mypy_boto3_dax/
+-rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-08-01 11:14:42.000000 mypy-boto3-dax-1.28.16/mypy_boto3_dax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-08-01 11:14:42.000000 mypy-boto3-dax-1.28.16/mypy_boto3_dax/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-08-01 11:14:42.000000 mypy-boto3-dax-1.28.16/mypy_boto3_dax/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20401 2023-08-01 11:14:42.000000 mypy-boto3-dax-1.28.16/mypy_boto3_dax/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20366 2023-08-01 11:14:42.000000 mypy-boto3-dax-1.28.16/mypy_boto3_dax/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9344 2023-08-01 11:14:42.000000 mypy-boto3-dax-1.28.16/mypy_boto3_dax/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9342 2023-08-01 11:14:42.000000 mypy-boto3-dax-1.28.16/mypy_boto3_dax/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8563 2023-08-01 11:14:42.000000 mypy-boto3-dax-1.28.16/mypy_boto3_dax/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8554 2023-08-01 11:14:42.000000 mypy-boto3-dax-1.28.16/mypy_boto3_dax/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:14:42.000000 mypy-boto3-dax-1.28.16/mypy_boto3_dax/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    22377 2023-08-01 11:14:43.000000 mypy-boto3-dax-1.28.16/mypy_boto3_dax/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22354 2023-08-01 11:14:42.000000 mypy-boto3-dax-1.28.16/mypy_boto3_dax/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:14:42.000000 mypy-boto3-dax-1.28.16/mypy_boto3_dax/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:35.708912 mypy-boto3-dax-1.28.16/mypy_boto3_dax.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16104 2023-08-01 11:36:35.000000 mypy-boto3-dax-1.28.16/mypy_boto3_dax.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-08-01 11:36:35.000000 mypy-boto3-dax-1.28.16/mypy_boto3_dax.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:35.000000 mypy-boto3-dax-1.28.16/mypy_boto3_dax.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:35.000000 mypy-boto3-dax-1.28.16/mypy_boto3_dax.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:35.000000 mypy-boto3-dax-1.28.16/mypy_boto3_dax.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-01 11:36:35.000000 mypy-boto3-dax-1.28.16/mypy_boto3_dax.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:35.720912 mypy-boto3-dax-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-08-01 11:14:42.000000 mypy-boto3-dax-1.28.16/setup.py
```

### Comparing `mypy-boto3-dax-1.28.15.post1/LICENSE` & `mypy-boto3-dax-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dax-1.28.15.post1/PKG-INFO` & `mypy-boto3-dax-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-dax
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.DAX 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.DAX 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dax/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 dax type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 dax type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-dax.svg?color=blue)](https://pypi.org/project/mypy-boto3-dax)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dax/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-dax)](https://pepy.tech/project/mypy-boto3-dax)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DAX 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX)
+[boto3.DAX 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX)
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
 [mypy-boto3-dax docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dax/).
 
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
@@ -342,20 +342,20 @@
 )
 
 
 def check_value(value: ChangeTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_dax.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_dax.type_defs import (
     EndpointTypeDef,
     NotificationConfigurationTypeDef,
     ParameterGroupStatusTypeDef,
     SSEDescriptionTypeDef,
@@ -369,15 +369,15 @@
     DecreaseReplicationFactorRequestRequestTypeDef,
     DeleteClusterRequestRequestTypeDef,
     DeleteParameterGroupRequestRequestTypeDef,
     DeleteSubnetGroupRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     DescribeClustersRequestRequestTypeDef,
     DescribeDefaultParametersRequestRequestTypeDef,
-    DescribeEventsRequestRequestTypeDef,
+    TimestampTypeDef,
     EventTypeDef,
     DescribeParameterGroupsRequestRequestTypeDef,
     DescribeParametersRequestRequestTypeDef,
     DescribeSubnetGroupsRequestRequestTypeDef,
     IncreaseReplicationFactorRequestRequestTypeDef,
     ListTagsRequestRequestTypeDef,
     NodeTypeSpecificValueTypeDef,
@@ -396,19 +396,20 @@
     TagResourceResponseTypeDef,
     UntagResourceResponseTypeDef,
     CreateParameterGroupResponseTypeDef,
     DescribeParameterGroupsResponseTypeDef,
     UpdateParameterGroupResponseTypeDef,
     DescribeClustersRequestDescribeClustersPaginateTypeDef,
     DescribeDefaultParametersRequestDescribeDefaultParametersPaginateTypeDef,
-    DescribeEventsRequestDescribeEventsPaginateTypeDef,
     DescribeParameterGroupsRequestDescribeParameterGroupsPaginateTypeDef,
     DescribeParametersRequestDescribeParametersPaginateTypeDef,
     DescribeSubnetGroupsRequestDescribeSubnetGroupsPaginateTypeDef,
     ListTagsRequestListTagsPaginateTypeDef,
+    DescribeEventsRequestDescribeEventsPaginateTypeDef,
+    DescribeEventsRequestRequestTypeDef,
     DescribeEventsResponseTypeDef,
     ParameterTypeDef,
     UpdateParameterGroupRequestRequestTypeDef,
     SubnetGroupTypeDef,
     ClusterTypeDef,
     DescribeDefaultParametersResponseTypeDef,
     DescribeParametersResponseTypeDef,
@@ -421,15 +422,15 @@
     DescribeClustersResponseTypeDef,
     IncreaseReplicationFactorResponseTypeDef,
     RebootNodeResponseTypeDef,
     UpdateClusterResponseTypeDef,
 )
 
 
-def get_structure() -> EndpointTypeDef:
+def get_value() -> EndpointTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-dax-1.28.15.post1/README.md` & `mypy-boto3-dax-1.28.16/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-dax.svg?color=blue)](https://pypi.org/project/mypy-boto3-dax)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dax/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-dax)](https://pepy.tech/project/mypy-boto3-dax)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DAX 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX)
+[boto3.DAX 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX)
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
 [mypy-boto3-dax docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dax/).
 
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
@@ -310,20 +310,20 @@
 )
 
 
 def check_value(value: ChangeTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_dax.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_dax.type_defs import (
     EndpointTypeDef,
     NotificationConfigurationTypeDef,
     ParameterGroupStatusTypeDef,
     SSEDescriptionTypeDef,
@@ -337,15 +337,15 @@
     DecreaseReplicationFactorRequestRequestTypeDef,
     DeleteClusterRequestRequestTypeDef,
     DeleteParameterGroupRequestRequestTypeDef,
     DeleteSubnetGroupRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     DescribeClustersRequestRequestTypeDef,
     DescribeDefaultParametersRequestRequestTypeDef,
-    DescribeEventsRequestRequestTypeDef,
+    TimestampTypeDef,
     EventTypeDef,
     DescribeParameterGroupsRequestRequestTypeDef,
     DescribeParametersRequestRequestTypeDef,
     DescribeSubnetGroupsRequestRequestTypeDef,
     IncreaseReplicationFactorRequestRequestTypeDef,
     ListTagsRequestRequestTypeDef,
     NodeTypeSpecificValueTypeDef,
@@ -364,19 +364,20 @@
     TagResourceResponseTypeDef,
     UntagResourceResponseTypeDef,
     CreateParameterGroupResponseTypeDef,
     DescribeParameterGroupsResponseTypeDef,
     UpdateParameterGroupResponseTypeDef,
     DescribeClustersRequestDescribeClustersPaginateTypeDef,
     DescribeDefaultParametersRequestDescribeDefaultParametersPaginateTypeDef,
-    DescribeEventsRequestDescribeEventsPaginateTypeDef,
     DescribeParameterGroupsRequestDescribeParameterGroupsPaginateTypeDef,
     DescribeParametersRequestDescribeParametersPaginateTypeDef,
     DescribeSubnetGroupsRequestDescribeSubnetGroupsPaginateTypeDef,
     ListTagsRequestListTagsPaginateTypeDef,
+    DescribeEventsRequestDescribeEventsPaginateTypeDef,
+    DescribeEventsRequestRequestTypeDef,
     DescribeEventsResponseTypeDef,
     ParameterTypeDef,
     UpdateParameterGroupRequestRequestTypeDef,
     SubnetGroupTypeDef,
     ClusterTypeDef,
     DescribeDefaultParametersResponseTypeDef,
     DescribeParametersResponseTypeDef,
@@ -389,15 +390,15 @@
     DescribeClustersResponseTypeDef,
     IncreaseReplicationFactorResponseTypeDef,
     RebootNodeResponseTypeDef,
     UpdateClusterResponseTypeDef,
 )
 
 
-def get_structure() -> EndpointTypeDef:
+def get_value() -> EndpointTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-dax-1.28.15.post1/mypy_boto3_dax/__init__.py` & `mypy-boto3-dax-1.28.16/mypy_boto3_dax/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dax-1.28.15.post1/mypy_boto3_dax/__init__.pyi` & `mypy-boto3-dax-1.28.16/mypy_boto3_dax/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dax-1.28.15.post1/mypy_boto3_dax/__main__.py` & `mypy-boto3-dax-1.28.16/mypy_boto3_dax/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.DAX 1.28.15\nVersion:         1.28.15.post1\nBuilder version:"
-        " 7.16.2\nDocs:           "
+        "Type annotations for boto3.DAX 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dax//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX\nOther"
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

### Comparing `mypy-boto3-dax-1.28.15.post1/mypy_boto3_dax/client.py` & `mypy-boto3-dax-1.28.16/mypy_boto3_dax/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from mypy_boto3_dax.client import DAXClient
 
     session = Session()
     client: DAXClient = session.client("dax")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import ClusterEndpointEncryptionTypeType, SourceTypeType
 from .paginator import (
     DescribeClustersPaginator,
     DescribeDefaultParametersPaginator,
@@ -46,14 +45,15 @@
     IncreaseReplicationFactorResponseTypeDef,
     ListTagsResponseTypeDef,
     ParameterNameValueTypeDef,
     RebootNodeResponseTypeDef,
     SSESpecificationTypeDef,
     TagResourceResponseTypeDef,
     TagTypeDef,
+    TimestampTypeDef,
     UntagResourceResponseTypeDef,
     UpdateClusterResponseTypeDef,
     UpdateParameterGroupResponseTypeDef,
     UpdateSubnetGroupResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
@@ -246,16 +246,16 @@
         """
 
     def describe_events(
         self,
         *,
         SourceName: str = ...,
         SourceType: SourceTypeType = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         Duration: int = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> DescribeEventsResponseTypeDef:
         """
         Returns events related to DAX clusters and parameter groups.
```

### Comparing `mypy-boto3-dax-1.28.15.post1/mypy_boto3_dax/client.pyi` & `mypy-boto3-dax-1.28.16/mypy_boto3_dax/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from mypy_boto3_dax.client import DAXClient
 
     session = Session()
     client: DAXClient = session.client("dax")
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import ClusterEndpointEncryptionTypeType, SourceTypeType
 from .paginator import (
     DescribeClustersPaginator,
     DescribeDefaultParametersPaginator,
@@ -46,14 +45,15 @@
     IncreaseReplicationFactorResponseTypeDef,
     ListTagsResponseTypeDef,
     ParameterNameValueTypeDef,
     RebootNodeResponseTypeDef,
     SSESpecificationTypeDef,
     TagResourceResponseTypeDef,
     TagTypeDef,
+    TimestampTypeDef,
     UntagResourceResponseTypeDef,
     UpdateClusterResponseTypeDef,
     UpdateParameterGroupResponseTypeDef,
     UpdateSubnetGroupResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
@@ -230,16 +230,16 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dax/client/#describe_default_parameters)
         """
     def describe_events(
         self,
         *,
         SourceName: str = ...,
         SourceType: SourceTypeType = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         Duration: int = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> DescribeEventsResponseTypeDef:
         """
         Returns events related to DAX clusters and parameter groups.
```

### Comparing `mypy-boto3-dax-1.28.15.post1/mypy_boto3_dax/literals.py` & `mypy-boto3-dax-1.28.16/mypy_boto3_dax/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dax-1.28.15.post1/mypy_boto3_dax/literals.pyi` & `mypy-boto3-dax-1.28.16/mypy_boto3_dax/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dax-1.28.15.post1/mypy_boto3_dax/paginator.py` & `mypy-boto3-dax-1.28.16/mypy_boto3_dax/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,29 +27,29 @@
     describe_events_paginator: DescribeEventsPaginator = client.get_paginator("describe_events")
     describe_parameter_groups_paginator: DescribeParameterGroupsPaginator = client.get_paginator("describe_parameter_groups")
     describe_parameters_paginator: DescribeParametersPaginator = client.get_paginator("describe_parameters")
     describe_subnet_groups_paginator: DescribeSubnetGroupsPaginator = client.get_paginator("describe_subnet_groups")
     list_tags_paginator: ListTagsPaginator = client.get_paginator("list_tags")
     ```
 """
-from datetime import datetime
-from typing import Generic, Iterator, Sequence, TypeVar, Union
+from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import SourceTypeType
 from .type_defs import (
     DescribeClustersResponseTypeDef,
     DescribeDefaultParametersResponseTypeDef,
     DescribeEventsResponseTypeDef,
     DescribeParameterGroupsResponseTypeDef,
     DescribeParametersResponseTypeDef,
     DescribeSubnetGroupsResponseTypeDef,
     ListTagsResponseTypeDef,
     PaginatorConfigTypeDef,
+    TimestampTypeDef,
 )
 
 __all__ = (
     "DescribeClustersPaginator",
     "DescribeDefaultParametersPaginator",
     "DescribeEventsPaginator",
     "DescribeParameterGroupsPaginator",
@@ -106,16 +106,16 @@
     """
 
     def paginate(
         self,
         *,
         SourceName: str = ...,
         SourceType: SourceTypeType = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         Duration: int = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeEventsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX.Paginator.DescribeEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dax/paginators/#describeeventspaginator)
         """
```

### Comparing `mypy-boto3-dax-1.28.15.post1/mypy_boto3_dax/paginator.pyi` & `mypy-boto3-dax-1.28.16/mypy_boto3_dax/paginator.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -27,29 +27,29 @@
     describe_events_paginator: DescribeEventsPaginator = client.get_paginator("describe_events")
     describe_parameter_groups_paginator: DescribeParameterGroupsPaginator = client.get_paginator("describe_parameter_groups")
     describe_parameters_paginator: DescribeParametersPaginator = client.get_paginator("describe_parameters")
     describe_subnet_groups_paginator: DescribeSubnetGroupsPaginator = client.get_paginator("describe_subnet_groups")
     list_tags_paginator: ListTagsPaginator = client.get_paginator("list_tags")
     ```
 """
-from datetime import datetime
-from typing import Generic, Iterator, Sequence, TypeVar, Union
+from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import SourceTypeType
 from .type_defs import (
     DescribeClustersResponseTypeDef,
     DescribeDefaultParametersResponseTypeDef,
     DescribeEventsResponseTypeDef,
     DescribeParameterGroupsResponseTypeDef,
     DescribeParametersResponseTypeDef,
     DescribeSubnetGroupsResponseTypeDef,
     ListTagsResponseTypeDef,
     PaginatorConfigTypeDef,
+    TimestampTypeDef,
 )
 
 __all__ = (
     "DescribeClustersPaginator",
     "DescribeDefaultParametersPaginator",
     "DescribeEventsPaginator",
     "DescribeParameterGroupsPaginator",
@@ -101,16 +101,16 @@
     """
 
     def paginate(
         self,
         *,
         SourceName: str = ...,
         SourceType: SourceTypeType = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         Duration: int = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeEventsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX.Paginator.DescribeEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dax/paginators/#describeeventspaginator)
         """
```

### Comparing `mypy-boto3-dax-1.28.15.post1/mypy_boto3_dax/type_defs.py` & `mypy-boto3-dax-1.28.16/mypy_boto3_dax/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dax/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_dax.type_defs import EndpointTypeDef
 
-    data: EndpointTypeDef = {...}
+    data: EndpointTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -45,15 +45,15 @@
     "DecreaseReplicationFactorRequestRequestTypeDef",
     "DeleteClusterRequestRequestTypeDef",
     "DeleteParameterGroupRequestRequestTypeDef",
     "DeleteSubnetGroupRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "DescribeClustersRequestRequestTypeDef",
     "DescribeDefaultParametersRequestRequestTypeDef",
-    "DescribeEventsRequestRequestTypeDef",
+    "TimestampTypeDef",
     "EventTypeDef",
     "DescribeParameterGroupsRequestRequestTypeDef",
     "DescribeParametersRequestRequestTypeDef",
     "DescribeSubnetGroupsRequestRequestTypeDef",
     "IncreaseReplicationFactorRequestRequestTypeDef",
     "ListTagsRequestRequestTypeDef",
     "NodeTypeSpecificValueTypeDef",
@@ -72,19 +72,20 @@
     "TagResourceResponseTypeDef",
     "UntagResourceResponseTypeDef",
     "CreateParameterGroupResponseTypeDef",
     "DescribeParameterGroupsResponseTypeDef",
     "UpdateParameterGroupResponseTypeDef",
     "DescribeClustersRequestDescribeClustersPaginateTypeDef",
     "DescribeDefaultParametersRequestDescribeDefaultParametersPaginateTypeDef",
-    "DescribeEventsRequestDescribeEventsPaginateTypeDef",
     "DescribeParameterGroupsRequestDescribeParameterGroupsPaginateTypeDef",
     "DescribeParametersRequestDescribeParametersPaginateTypeDef",
     "DescribeSubnetGroupsRequestDescribeSubnetGroupsPaginateTypeDef",
     "ListTagsRequestListTagsPaginateTypeDef",
+    "DescribeEventsRequestDescribeEventsPaginateTypeDef",
+    "DescribeEventsRequestRequestTypeDef",
     "DescribeEventsResponseTypeDef",
     "ParameterTypeDef",
     "UpdateParameterGroupRequestRequestTypeDef",
     "SubnetGroupTypeDef",
     "ClusterTypeDef",
     "DescribeDefaultParametersResponseTypeDef",
     "DescribeParametersResponseTypeDef",
@@ -296,28 +297,15 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-DescribeEventsRequestRequestTypeDef = TypedDict(
-    "DescribeEventsRequestRequestTypeDef",
-    {
-        "SourceName": str,
-        "SourceType": SourceTypeType,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "Duration": int,
-        "MaxResults": int,
-        "NextToken": str,
-    },
-    total=False,
-)
-
+TimestampTypeDef = Union[datetime, str]
 EventTypeDef = TypedDict(
     "EventTypeDef",
     {
         "SourceName": str,
         "SourceType": SourceTypeType,
         "Message": str,
         "Date": datetime,
@@ -637,27 +625,14 @@
     "DescribeDefaultParametersRequestDescribeDefaultParametersPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-DescribeEventsRequestDescribeEventsPaginateTypeDef = TypedDict(
-    "DescribeEventsRequestDescribeEventsPaginateTypeDef",
-    {
-        "SourceName": str,
-        "SourceType": SourceTypeType,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "Duration": int,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 DescribeParameterGroupsRequestDescribeParameterGroupsPaginateTypeDef = TypedDict(
     "DescribeParameterGroupsRequestDescribeParameterGroupsPaginateTypeDef",
     {
         "ParameterGroupNames": Sequence[str],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -712,14 +687,41 @@
 
 class ListTagsRequestListTagsPaginateTypeDef(
     _RequiredListTagsRequestListTagsPaginateTypeDef, _OptionalListTagsRequestListTagsPaginateTypeDef
 ):
     pass
 
 
+DescribeEventsRequestDescribeEventsPaginateTypeDef = TypedDict(
+    "DescribeEventsRequestDescribeEventsPaginateTypeDef",
+    {
+        "SourceName": str,
+        "SourceType": SourceTypeType,
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "Duration": int,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeEventsRequestRequestTypeDef = TypedDict(
+    "DescribeEventsRequestRequestTypeDef",
+    {
+        "SourceName": str,
+        "SourceType": SourceTypeType,
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "Duration": int,
+        "MaxResults": int,
+        "NextToken": str,
+    },
+    total=False,
+)
+
 DescribeEventsResponseTypeDef = TypedDict(
     "DescribeEventsResponseTypeDef",
     {
         "NextToken": str,
         "Events": List[EventTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-dax-1.28.15.post1/mypy_boto3_dax/type_defs.pyi` & `mypy-boto3-dax-1.28.16/mypy_boto3_dax/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dax/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_dax.type_defs import EndpointTypeDef
 
-    data: EndpointTypeDef = {...}
+    data: EndpointTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -44,15 +44,15 @@
     "DecreaseReplicationFactorRequestRequestTypeDef",
     "DeleteClusterRequestRequestTypeDef",
     "DeleteParameterGroupRequestRequestTypeDef",
     "DeleteSubnetGroupRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "DescribeClustersRequestRequestTypeDef",
     "DescribeDefaultParametersRequestRequestTypeDef",
-    "DescribeEventsRequestRequestTypeDef",
+    "TimestampTypeDef",
     "EventTypeDef",
     "DescribeParameterGroupsRequestRequestTypeDef",
     "DescribeParametersRequestRequestTypeDef",
     "DescribeSubnetGroupsRequestRequestTypeDef",
     "IncreaseReplicationFactorRequestRequestTypeDef",
     "ListTagsRequestRequestTypeDef",
     "NodeTypeSpecificValueTypeDef",
@@ -71,19 +71,20 @@
     "TagResourceResponseTypeDef",
     "UntagResourceResponseTypeDef",
     "CreateParameterGroupResponseTypeDef",
     "DescribeParameterGroupsResponseTypeDef",
     "UpdateParameterGroupResponseTypeDef",
     "DescribeClustersRequestDescribeClustersPaginateTypeDef",
     "DescribeDefaultParametersRequestDescribeDefaultParametersPaginateTypeDef",
-    "DescribeEventsRequestDescribeEventsPaginateTypeDef",
     "DescribeParameterGroupsRequestDescribeParameterGroupsPaginateTypeDef",
     "DescribeParametersRequestDescribeParametersPaginateTypeDef",
     "DescribeSubnetGroupsRequestDescribeSubnetGroupsPaginateTypeDef",
     "ListTagsRequestListTagsPaginateTypeDef",
+    "DescribeEventsRequestDescribeEventsPaginateTypeDef",
+    "DescribeEventsRequestRequestTypeDef",
     "DescribeEventsResponseTypeDef",
     "ParameterTypeDef",
     "UpdateParameterGroupRequestRequestTypeDef",
     "SubnetGroupTypeDef",
     "ClusterTypeDef",
     "DescribeDefaultParametersResponseTypeDef",
     "DescribeParametersResponseTypeDef",
@@ -289,28 +290,15 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-DescribeEventsRequestRequestTypeDef = TypedDict(
-    "DescribeEventsRequestRequestTypeDef",
-    {
-        "SourceName": str,
-        "SourceType": SourceTypeType,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "Duration": int,
-        "MaxResults": int,
-        "NextToken": str,
-    },
-    total=False,
-)
-
+TimestampTypeDef = Union[datetime, str]
 EventTypeDef = TypedDict(
     "EventTypeDef",
     {
         "SourceName": str,
         "SourceType": SourceTypeType,
         "Message": str,
         "Date": datetime,
@@ -618,27 +606,14 @@
     "DescribeDefaultParametersRequestDescribeDefaultParametersPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-DescribeEventsRequestDescribeEventsPaginateTypeDef = TypedDict(
-    "DescribeEventsRequestDescribeEventsPaginateTypeDef",
-    {
-        "SourceName": str,
-        "SourceType": SourceTypeType,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "Duration": int,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 DescribeParameterGroupsRequestDescribeParameterGroupsPaginateTypeDef = TypedDict(
     "DescribeParameterGroupsRequestDescribeParameterGroupsPaginateTypeDef",
     {
         "ParameterGroupNames": Sequence[str],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -689,14 +664,41 @@
 )
 
 class ListTagsRequestListTagsPaginateTypeDef(
     _RequiredListTagsRequestListTagsPaginateTypeDef, _OptionalListTagsRequestListTagsPaginateTypeDef
 ):
     pass
 
+DescribeEventsRequestDescribeEventsPaginateTypeDef = TypedDict(
+    "DescribeEventsRequestDescribeEventsPaginateTypeDef",
+    {
+        "SourceName": str,
+        "SourceType": SourceTypeType,
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "Duration": int,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeEventsRequestRequestTypeDef = TypedDict(
+    "DescribeEventsRequestRequestTypeDef",
+    {
+        "SourceName": str,
+        "SourceType": SourceTypeType,
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "Duration": int,
+        "MaxResults": int,
+        "NextToken": str,
+    },
+    total=False,
+)
+
 DescribeEventsResponseTypeDef = TypedDict(
     "DescribeEventsResponseTypeDef",
     {
         "NextToken": str,
         "Events": List[EventTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-dax-1.28.15.post1/mypy_boto3_dax.egg-info/PKG-INFO` & `mypy-boto3-dax-1.28.16/mypy_boto3_dax.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-dax
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.DAX 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.DAX 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dax/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 dax type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 dax type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-dax.svg?color=blue)](https://pypi.org/project/mypy-boto3-dax)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dax/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-dax)](https://pepy.tech/project/mypy-boto3-dax)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DAX 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX)
+[boto3.DAX 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX)
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
 [mypy-boto3-dax docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dax/).
 
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
@@ -342,20 +342,20 @@
 )
 
 
 def check_value(value: ChangeTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_dax.type_defs` module contains structures and shapes assembled to
-typed dictionaries for additional type checking.
+typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_dax.type_defs import (
     EndpointTypeDef,
     NotificationConfigurationTypeDef,
     ParameterGroupStatusTypeDef,
     SSEDescriptionTypeDef,
@@ -369,15 +369,15 @@
     DecreaseReplicationFactorRequestRequestTypeDef,
     DeleteClusterRequestRequestTypeDef,
     DeleteParameterGroupRequestRequestTypeDef,
     DeleteSubnetGroupRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     DescribeClustersRequestRequestTypeDef,
     DescribeDefaultParametersRequestRequestTypeDef,
-    DescribeEventsRequestRequestTypeDef,
+    TimestampTypeDef,
     EventTypeDef,
     DescribeParameterGroupsRequestRequestTypeDef,
     DescribeParametersRequestRequestTypeDef,
     DescribeSubnetGroupsRequestRequestTypeDef,
     IncreaseReplicationFactorRequestRequestTypeDef,
     ListTagsRequestRequestTypeDef,
     NodeTypeSpecificValueTypeDef,
@@ -396,19 +396,20 @@
     TagResourceResponseTypeDef,
     UntagResourceResponseTypeDef,
     CreateParameterGroupResponseTypeDef,
     DescribeParameterGroupsResponseTypeDef,
     UpdateParameterGroupResponseTypeDef,
     DescribeClustersRequestDescribeClustersPaginateTypeDef,
     DescribeDefaultParametersRequestDescribeDefaultParametersPaginateTypeDef,
-    DescribeEventsRequestDescribeEventsPaginateTypeDef,
     DescribeParameterGroupsRequestDescribeParameterGroupsPaginateTypeDef,
     DescribeParametersRequestDescribeParametersPaginateTypeDef,
     DescribeSubnetGroupsRequestDescribeSubnetGroupsPaginateTypeDef,
     ListTagsRequestListTagsPaginateTypeDef,
+    DescribeEventsRequestDescribeEventsPaginateTypeDef,
+    DescribeEventsRequestRequestTypeDef,
     DescribeEventsResponseTypeDef,
     ParameterTypeDef,
     UpdateParameterGroupRequestRequestTypeDef,
     SubnetGroupTypeDef,
     ClusterTypeDef,
     DescribeDefaultParametersResponseTypeDef,
     DescribeParametersResponseTypeDef,
@@ -421,15 +422,15 @@
     DescribeClustersResponseTypeDef,
     IncreaseReplicationFactorResponseTypeDef,
     RebootNodeResponseTypeDef,
     UpdateClusterResponseTypeDef,
 )
 
 
-def get_structure() -> EndpointTypeDef:
+def get_value() -> EndpointTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-dax-1.28.15.post1/mypy_boto3_dax.egg-info/SOURCES.txt` & `mypy-boto3-dax-1.28.16/mypy_boto3_dax.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dax-1.28.15.post1/setup.py` & `mypy-boto3-dax-1.28.16/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-dax",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_dax"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.DAX 1.28.15 service generated with mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.DAX 1.28.16 service generated with mypy-boto3-builder 7.17.1"
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
-    keywords="boto3 dax type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 dax type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_dax": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dax/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

