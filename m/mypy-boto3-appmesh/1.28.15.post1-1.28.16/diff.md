# Comparing `tmp/mypy-boto3-appmesh-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-appmesh-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-appmesh-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:31 2023, max compression
+gzip compressed data, was "mypy-boto3-appmesh-1.28.16.tar", last modified: Tue Aug  1 11:36:11 2023, max compression
```

## Comparing `mypy-boto3-appmesh-1.28.15.post1.tar` & `mypy-boto3-appmesh-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:31.145007 mypy-boto3-appmesh-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:38:20.000000 mypy-boto3-appmesh-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    24338 2023-07-29 10:02:31.141008 mypy-boto3-appmesh-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22845 2023-07-29 09:38:20.000000 mypy-boto3-appmesh-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:31.133007 mypy-boto3-appmesh-1.28.15.post1/mypy_boto3_appmesh/
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-07-29 09:38:20.000000 mypy-boto3-appmesh-1.28.15.post1/mypy_boto3_appmesh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-07-29 09:38:20.000000 mypy-boto3-appmesh-1.28.15.post1/mypy_boto3_appmesh/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-29 09:38:20.000000 mypy-boto3-appmesh-1.28.15.post1/mypy_boto3_appmesh/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30776 2023-07-29 09:38:21.000000 mypy-boto3-appmesh-1.28.15.post1/mypy_boto3_appmesh/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    30723 2023-07-29 09:38:21.000000 mypy-boto3-appmesh-1.28.15.post1/mypy_boto3_appmesh/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11115 2023-07-29 09:38:21.000000 mypy-boto3-appmesh-1.28.15.post1/mypy_boto3_appmesh/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11113 2023-07-29 09:38:21.000000 mypy-boto3-appmesh-1.28.15.post1/mypy_boto3_appmesh/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9467 2023-07-29 09:38:21.000000 mypy-boto3-appmesh-1.28.15.post1/mypy_boto3_appmesh/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9457 2023-07-29 09:38:21.000000 mypy-boto3-appmesh-1.28.15.post1/mypy_boto3_appmesh/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:38:20.000000 mypy-boto3-appmesh-1.28.15.post1/mypy_boto3_appmesh/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   100348 2023-07-29 09:38:25.000000 mypy-boto3-appmesh-1.28.15.post1/mypy_boto3_appmesh/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   100157 2023-07-29 09:38:22.000000 mypy-boto3-appmesh-1.28.15.post1/mypy_boto3_appmesh/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:38:20.000000 mypy-boto3-appmesh-1.28.15.post1/mypy_boto3_appmesh/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:31.141008 mypy-boto3-appmesh-1.28.15.post1/mypy_boto3_appmesh.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    24338 2023-07-29 10:02:30.000000 mypy-boto3-appmesh-1.28.15.post1/mypy_boto3_appmesh.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-29 10:02:30.000000 mypy-boto3-appmesh-1.28.15.post1/mypy_boto3_appmesh.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:30.000000 mypy-boto3-appmesh-1.28.15.post1/mypy_boto3_appmesh.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:30.000000 mypy-boto3-appmesh-1.28.15.post1/mypy_boto3_appmesh.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:30.000000 mypy-boto3-appmesh-1.28.15.post1/mypy_boto3_appmesh.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-29 10:02:30.000000 mypy-boto3-appmesh-1.28.15.post1/mypy_boto3_appmesh.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:31.145007 mypy-boto3-appmesh-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-07-29 09:38:20.000000 mypy-boto3-appmesh-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:11.908950 mypy-boto3-appmesh-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:10:52.000000 mypy-boto3-appmesh-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    24493 2023-08-01 11:36:11.908950 mypy-boto3-appmesh-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    23009 2023-08-01 11:10:52.000000 mypy-boto3-appmesh-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:11.904950 mypy-boto3-appmesh-1.28.16/mypy_boto3_appmesh/
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-08-01 11:10:52.000000 mypy-boto3-appmesh-1.28.16/mypy_boto3_appmesh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-08-01 11:10:52.000000 mypy-boto3-appmesh-1.28.16/mypy_boto3_appmesh/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-08-01 11:10:52.000000 mypy-boto3-appmesh-1.28.16/mypy_boto3_appmesh/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30304 2023-08-01 11:10:52.000000 mypy-boto3-appmesh-1.28.16/mypy_boto3_appmesh/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30251 2023-08-01 11:10:52.000000 mypy-boto3-appmesh-1.28.16/mypy_boto3_appmesh/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11115 2023-08-01 11:10:53.000000 mypy-boto3-appmesh-1.28.16/mypy_boto3_appmesh/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11113 2023-08-01 11:10:53.000000 mypy-boto3-appmesh-1.28.16/mypy_boto3_appmesh/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9467 2023-08-01 11:10:52.000000 mypy-boto3-appmesh-1.28.16/mypy_boto3_appmesh/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9457 2023-08-01 11:10:52.000000 mypy-boto3-appmesh-1.28.16/mypy_boto3_appmesh/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:10:52.000000 mypy-boto3-appmesh-1.28.16/mypy_boto3_appmesh/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   100978 2023-08-01 11:10:56.000000 mypy-boto3-appmesh-1.28.16/mypy_boto3_appmesh/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   100787 2023-08-01 11:10:55.000000 mypy-boto3-appmesh-1.28.16/mypy_boto3_appmesh/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:10:52.000000 mypy-boto3-appmesh-1.28.16/mypy_boto3_appmesh/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:11.904950 mypy-boto3-appmesh-1.28.16/mypy_boto3_appmesh.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    24493 2023-08-01 11:36:11.000000 mypy-boto3-appmesh-1.28.16/mypy_boto3_appmesh.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-08-01 11:36:11.000000 mypy-boto3-appmesh-1.28.16/mypy_boto3_appmesh.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:11.000000 mypy-boto3-appmesh-1.28.16/mypy_boto3_appmesh.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:11.000000 mypy-boto3-appmesh-1.28.16/mypy_boto3_appmesh.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:11.000000 mypy-boto3-appmesh-1.28.16/mypy_boto3_appmesh.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-01 11:36:11.000000 mypy-boto3-appmesh-1.28.16/mypy_boto3_appmesh.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:11.908950 mypy-boto3-appmesh-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-08-01 11:10:52.000000 mypy-boto3-appmesh-1.28.16/setup.py
```

### Comparing `mypy-boto3-appmesh-1.28.15.post1/LICENSE` & `mypy-boto3-appmesh-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appmesh-1.28.15.post1/PKG-INFO` & `mypy-boto3-appmesh-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-appmesh
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.AppMesh 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.AppMesh 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 appmesh type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 appmesh type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-appmesh.svg?color=blue)](https://pypi.org/project/mypy-boto3-appmesh)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-appmesh)](https://pepy.tech/project/mypy-boto3-appmesh)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AppMesh 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh)
+[boto3.AppMesh 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh)
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
 [mypy-boto3-appmesh docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/).
 
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
@@ -362,20 +362,20 @@
 )
 
 
 def check_value(value: DefaultGatewayRouteRewriteType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_appmesh.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_appmesh.type_defs import (
     AwsCloudMapInstanceAttributeTypeDef,
     ListenerTlsFileCertificateTypeDef,
     ListenerTlsSdsCertificateTypeDef,
     TagRefTypeDef,
@@ -560,14 +560,15 @@
     AccessLogOutputTypeDef,
     VirtualGatewayAccessLogOutputTypeDef,
     AccessLogTypeDef,
     VirtualGatewayAccessLogTypeDef,
     VirtualRouterDataTypeDef,
     CreateVirtualRouterInputRequestTypeDef,
     UpdateVirtualRouterInputRequestTypeDef,
+    VirtualRouterSpecUnionTypeDef,
     CreateMeshOutputTypeDef,
     DeleteMeshOutputTypeDef,
     DescribeMeshOutputTypeDef,
     UpdateMeshOutputTypeDef,
     ListenerTlsOutputTypeDef,
     ListenerTlsTypeDef,
     ClientPolicyTlsOutputTypeDef,
@@ -615,17 +616,19 @@
     VirtualServiceBackendOutputTypeDef,
     BackendDefaultsTypeDef,
     VirtualServiceBackendTypeDef,
     VirtualGatewayBackendDefaultsOutputTypeDef,
     VirtualGatewayBackendDefaultsTypeDef,
     GatewayRouteDataTypeDef,
     CreateGatewayRouteInputRequestTypeDef,
+    GatewayRouteSpecUnionTypeDef,
     UpdateGatewayRouteInputRequestTypeDef,
     RouteDataTypeDef,
     CreateRouteInputRequestTypeDef,
+    RouteSpecUnionTypeDef,
     UpdateRouteInputRequestTypeDef,
     BackendOutputTypeDef,
     BackendTypeDef,
     VirtualGatewaySpecOutputTypeDef,
     VirtualGatewaySpecTypeDef,
     CreateGatewayRouteOutputTypeDef,
     DeleteGatewayRouteOutputTypeDef,
@@ -636,29 +639,31 @@
     DescribeRouteOutputTypeDef,
     UpdateRouteOutputTypeDef,
     VirtualNodeSpecOutputTypeDef,
     VirtualNodeSpecTypeDef,
     VirtualGatewayDataTypeDef,
     CreateVirtualGatewayInputRequestTypeDef,
     UpdateVirtualGatewayInputRequestTypeDef,
+    VirtualGatewaySpecUnionTypeDef,
     VirtualNodeDataTypeDef,
     CreateVirtualNodeInputRequestTypeDef,
     UpdateVirtualNodeInputRequestTypeDef,
+    VirtualNodeSpecUnionTypeDef,
     CreateVirtualGatewayOutputTypeDef,
     DeleteVirtualGatewayOutputTypeDef,
     DescribeVirtualGatewayOutputTypeDef,
     UpdateVirtualGatewayOutputTypeDef,
     CreateVirtualNodeOutputTypeDef,
     DeleteVirtualNodeOutputTypeDef,
     DescribeVirtualNodeOutputTypeDef,
     UpdateVirtualNodeOutputTypeDef,
 )
 
 
-def get_structure() -> AwsCloudMapInstanceAttributeTypeDef:
+def get_value() -> AwsCloudMapInstanceAttributeTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-appmesh-1.28.15.post1/README.md` & `mypy-boto3-appmesh-1.28.16/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-appmesh.svg?color=blue)](https://pypi.org/project/mypy-boto3-appmesh)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-appmesh)](https://pepy.tech/project/mypy-boto3-appmesh)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AppMesh 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh)
+[boto3.AppMesh 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh)
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
 [mypy-boto3-appmesh docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/).
 
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
@@ -330,20 +330,20 @@
 )
 
 
 def check_value(value: DefaultGatewayRouteRewriteType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_appmesh.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_appmesh.type_defs import (
     AwsCloudMapInstanceAttributeTypeDef,
     ListenerTlsFileCertificateTypeDef,
     ListenerTlsSdsCertificateTypeDef,
     TagRefTypeDef,
@@ -528,14 +528,15 @@
     AccessLogOutputTypeDef,
     VirtualGatewayAccessLogOutputTypeDef,
     AccessLogTypeDef,
     VirtualGatewayAccessLogTypeDef,
     VirtualRouterDataTypeDef,
     CreateVirtualRouterInputRequestTypeDef,
     UpdateVirtualRouterInputRequestTypeDef,
+    VirtualRouterSpecUnionTypeDef,
     CreateMeshOutputTypeDef,
     DeleteMeshOutputTypeDef,
     DescribeMeshOutputTypeDef,
     UpdateMeshOutputTypeDef,
     ListenerTlsOutputTypeDef,
     ListenerTlsTypeDef,
     ClientPolicyTlsOutputTypeDef,
@@ -583,17 +584,19 @@
     VirtualServiceBackendOutputTypeDef,
     BackendDefaultsTypeDef,
     VirtualServiceBackendTypeDef,
     VirtualGatewayBackendDefaultsOutputTypeDef,
     VirtualGatewayBackendDefaultsTypeDef,
     GatewayRouteDataTypeDef,
     CreateGatewayRouteInputRequestTypeDef,
+    GatewayRouteSpecUnionTypeDef,
     UpdateGatewayRouteInputRequestTypeDef,
     RouteDataTypeDef,
     CreateRouteInputRequestTypeDef,
+    RouteSpecUnionTypeDef,
     UpdateRouteInputRequestTypeDef,
     BackendOutputTypeDef,
     BackendTypeDef,
     VirtualGatewaySpecOutputTypeDef,
     VirtualGatewaySpecTypeDef,
     CreateGatewayRouteOutputTypeDef,
     DeleteGatewayRouteOutputTypeDef,
@@ -604,29 +607,31 @@
     DescribeRouteOutputTypeDef,
     UpdateRouteOutputTypeDef,
     VirtualNodeSpecOutputTypeDef,
     VirtualNodeSpecTypeDef,
     VirtualGatewayDataTypeDef,
     CreateVirtualGatewayInputRequestTypeDef,
     UpdateVirtualGatewayInputRequestTypeDef,
+    VirtualGatewaySpecUnionTypeDef,
     VirtualNodeDataTypeDef,
     CreateVirtualNodeInputRequestTypeDef,
     UpdateVirtualNodeInputRequestTypeDef,
+    VirtualNodeSpecUnionTypeDef,
     CreateVirtualGatewayOutputTypeDef,
     DeleteVirtualGatewayOutputTypeDef,
     DescribeVirtualGatewayOutputTypeDef,
     UpdateVirtualGatewayOutputTypeDef,
     CreateVirtualNodeOutputTypeDef,
     DeleteVirtualNodeOutputTypeDef,
     DescribeVirtualNodeOutputTypeDef,
     UpdateVirtualNodeOutputTypeDef,
 )
 
 
-def get_structure() -> AwsCloudMapInstanceAttributeTypeDef:
+def get_value() -> AwsCloudMapInstanceAttributeTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-appmesh-1.28.15.post1/mypy_boto3_appmesh/__init__.py` & `mypy-boto3-appmesh-1.28.16/mypy_boto3_appmesh/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appmesh-1.28.15.post1/mypy_boto3_appmesh/__init__.pyi` & `mypy-boto3-appmesh-1.28.16/mypy_boto3_appmesh/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appmesh-1.28.15.post1/mypy_boto3_appmesh/__main__.py` & `mypy-boto3-appmesh-1.28.16/mypy_boto3_appmesh/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.AppMesh 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.AppMesh 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh\nOther"
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

### Comparing `mypy-boto3-appmesh-1.28.15.post1/mypy_boto3_appmesh/client.py` & `mypy-boto3-appmesh-1.28.16/mypy_boto3_appmesh/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_appmesh.client import AppMeshClient
 
     session = Session()
     client: AppMeshClient = session.client("appmesh")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .paginator import (
     ListGatewayRoutesPaginator,
     ListMeshesPaginator,
     ListRoutesPaginator,
@@ -46,75 +46,66 @@
     DescribeGatewayRouteOutputTypeDef,
     DescribeMeshOutputTypeDef,
     DescribeRouteOutputTypeDef,
     DescribeVirtualGatewayOutputTypeDef,
     DescribeVirtualNodeOutputTypeDef,
     DescribeVirtualRouterOutputTypeDef,
     DescribeVirtualServiceOutputTypeDef,
-    GatewayRouteSpecOutputTypeDef,
-    GatewayRouteSpecTypeDef,
+    GatewayRouteSpecUnionTypeDef,
     ListGatewayRoutesOutputTypeDef,
     ListMeshesOutputTypeDef,
     ListRoutesOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     ListVirtualGatewaysOutputTypeDef,
     ListVirtualNodesOutputTypeDef,
     ListVirtualRoutersOutputTypeDef,
     ListVirtualServicesOutputTypeDef,
     MeshSpecTypeDef,
-    RouteSpecOutputTypeDef,
-    RouteSpecTypeDef,
+    RouteSpecUnionTypeDef,
     TagRefTypeDef,
     UpdateGatewayRouteOutputTypeDef,
     UpdateMeshOutputTypeDef,
     UpdateRouteOutputTypeDef,
     UpdateVirtualGatewayOutputTypeDef,
     UpdateVirtualNodeOutputTypeDef,
     UpdateVirtualRouterOutputTypeDef,
     UpdateVirtualServiceOutputTypeDef,
-    VirtualGatewaySpecOutputTypeDef,
-    VirtualGatewaySpecTypeDef,
-    VirtualNodeSpecOutputTypeDef,
-    VirtualNodeSpecTypeDef,
-    VirtualRouterSpecOutputTypeDef,
-    VirtualRouterSpecTypeDef,
+    VirtualGatewaySpecUnionTypeDef,
+    VirtualNodeSpecUnionTypeDef,
+    VirtualRouterSpecUnionTypeDef,
     VirtualServiceSpecTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("AppMeshClient",)
 
-
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     BadRequestException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     ForbiddenException: Type[BotocoreClientError]
     InternalServerErrorException: Type[BotocoreClientError]
     LimitExceededException: Type[BotocoreClientError]
     NotFoundException: Type[BotocoreClientError]
     ResourceInUseException: Type[BotocoreClientError]
     ServiceUnavailableException: Type[BotocoreClientError]
     TooManyRequestsException: Type[BotocoreClientError]
     TooManyTagsException: Type[BotocoreClientError]
 
-
 class AppMeshClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/)
     """
 
     meta: ClientMeta
@@ -123,133 +114,124 @@
     def exceptions(self) -> Exceptions:
         """
         AppMeshClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#exceptions)
         """
-
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#can_paginate)
         """
-
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#close)
         """
-
     def create_gateway_route(
         self,
         *,
         gatewayRouteName: str,
         meshName: str,
-        spec: Union[GatewayRouteSpecTypeDef, GatewayRouteSpecOutputTypeDef],
+        spec: GatewayRouteSpecUnionTypeDef,
         virtualGatewayName: str,
         clientToken: str = ...,
         meshOwner: str = ...,
         tags: Sequence[TagRefTypeDef] = ...
     ) -> CreateGatewayRouteOutputTypeDef:
         """
         Creates a gateway route.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.create_gateway_route)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#create_gateway_route)
         """
-
     def create_mesh(
         self,
         *,
         meshName: str,
         clientToken: str = ...,
         spec: MeshSpecTypeDef = ...,
         tags: Sequence[TagRefTypeDef] = ...
     ) -> CreateMeshOutputTypeDef:
         """
         Creates a service mesh.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.create_mesh)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#create_mesh)
         """
-
     def create_route(
         self,
         *,
         meshName: str,
         routeName: str,
-        spec: Union[RouteSpecTypeDef, RouteSpecOutputTypeDef],
+        spec: RouteSpecUnionTypeDef,
         virtualRouterName: str,
         clientToken: str = ...,
         meshOwner: str = ...,
         tags: Sequence[TagRefTypeDef] = ...
     ) -> CreateRouteOutputTypeDef:
         """
         Creates a route that is associated with a virtual router.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.create_route)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#create_route)
         """
-
     def create_virtual_gateway(
         self,
         *,
         meshName: str,
-        spec: Union[VirtualGatewaySpecTypeDef, VirtualGatewaySpecOutputTypeDef],
+        spec: VirtualGatewaySpecUnionTypeDef,
         virtualGatewayName: str,
         clientToken: str = ...,
         meshOwner: str = ...,
         tags: Sequence[TagRefTypeDef] = ...
     ) -> CreateVirtualGatewayOutputTypeDef:
         """
         Creates a virtual gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.create_virtual_gateway)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#create_virtual_gateway)
         """
-
     def create_virtual_node(
         self,
         *,
         meshName: str,
-        spec: Union[VirtualNodeSpecTypeDef, VirtualNodeSpecOutputTypeDef],
+        spec: VirtualNodeSpecUnionTypeDef,
         virtualNodeName: str,
         clientToken: str = ...,
         meshOwner: str = ...,
         tags: Sequence[TagRefTypeDef] = ...
     ) -> CreateVirtualNodeOutputTypeDef:
         """
         Creates a virtual node within a service mesh.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.create_virtual_node)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#create_virtual_node)
         """
-
     def create_virtual_router(
         self,
         *,
         meshName: str,
-        spec: Union[VirtualRouterSpecTypeDef, VirtualRouterSpecOutputTypeDef],
+        spec: VirtualRouterSpecUnionTypeDef,
         virtualRouterName: str,
         clientToken: str = ...,
         meshOwner: str = ...,
         tags: Sequence[TagRefTypeDef] = ...
     ) -> CreateVirtualRouterOutputTypeDef:
         """
         Creates a virtual router within a service mesh.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.create_virtual_router)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#create_virtual_router)
         """
-
     def create_virtual_service(
         self,
         *,
         meshName: str,
         spec: VirtualServiceSpecTypeDef,
         virtualServiceName: str,
         clientToken: str = ...,
@@ -258,165 +240,149 @@
     ) -> CreateVirtualServiceOutputTypeDef:
         """
         Creates a virtual service within a service mesh.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.create_virtual_service)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#create_virtual_service)
         """
-
     def delete_gateway_route(
         self, *, gatewayRouteName: str, meshName: str, virtualGatewayName: str, meshOwner: str = ...
     ) -> DeleteGatewayRouteOutputTypeDef:
         """
         Deletes an existing gateway route.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.delete_gateway_route)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#delete_gateway_route)
         """
-
     def delete_mesh(self, *, meshName: str) -> DeleteMeshOutputTypeDef:
         """
         Deletes an existing service mesh.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.delete_mesh)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#delete_mesh)
         """
-
     def delete_route(
         self, *, meshName: str, routeName: str, virtualRouterName: str, meshOwner: str = ...
     ) -> DeleteRouteOutputTypeDef:
         """
         Deletes an existing route.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.delete_route)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#delete_route)
         """
-
     def delete_virtual_gateway(
         self, *, meshName: str, virtualGatewayName: str, meshOwner: str = ...
     ) -> DeleteVirtualGatewayOutputTypeDef:
         """
         Deletes an existing virtual gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.delete_virtual_gateway)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#delete_virtual_gateway)
         """
-
     def delete_virtual_node(
         self, *, meshName: str, virtualNodeName: str, meshOwner: str = ...
     ) -> DeleteVirtualNodeOutputTypeDef:
         """
         Deletes an existing virtual node.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.delete_virtual_node)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#delete_virtual_node)
         """
-
     def delete_virtual_router(
         self, *, meshName: str, virtualRouterName: str, meshOwner: str = ...
     ) -> DeleteVirtualRouterOutputTypeDef:
         """
         Deletes an existing virtual router.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.delete_virtual_router)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#delete_virtual_router)
         """
-
     def delete_virtual_service(
         self, *, meshName: str, virtualServiceName: str, meshOwner: str = ...
     ) -> DeleteVirtualServiceOutputTypeDef:
         """
         Deletes an existing virtual service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.delete_virtual_service)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#delete_virtual_service)
         """
-
     def describe_gateway_route(
         self, *, gatewayRouteName: str, meshName: str, virtualGatewayName: str, meshOwner: str = ...
     ) -> DescribeGatewayRouteOutputTypeDef:
         """
         Describes an existing gateway route.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.describe_gateway_route)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#describe_gateway_route)
         """
-
     def describe_mesh(self, *, meshName: str, meshOwner: str = ...) -> DescribeMeshOutputTypeDef:
         """
         Describes an existing service mesh.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.describe_mesh)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#describe_mesh)
         """
-
     def describe_route(
         self, *, meshName: str, routeName: str, virtualRouterName: str, meshOwner: str = ...
     ) -> DescribeRouteOutputTypeDef:
         """
         Describes an existing route.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.describe_route)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#describe_route)
         """
-
     def describe_virtual_gateway(
         self, *, meshName: str, virtualGatewayName: str, meshOwner: str = ...
     ) -> DescribeVirtualGatewayOutputTypeDef:
         """
         Describes an existing virtual gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.describe_virtual_gateway)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#describe_virtual_gateway)
         """
-
     def describe_virtual_node(
         self, *, meshName: str, virtualNodeName: str, meshOwner: str = ...
     ) -> DescribeVirtualNodeOutputTypeDef:
         """
         Describes an existing virtual node.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.describe_virtual_node)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#describe_virtual_node)
         """
-
     def describe_virtual_router(
         self, *, meshName: str, virtualRouterName: str, meshOwner: str = ...
     ) -> DescribeVirtualRouterOutputTypeDef:
         """
         Describes an existing virtual router.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.describe_virtual_router)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#describe_virtual_router)
         """
-
     def describe_virtual_service(
         self, *, meshName: str, virtualServiceName: str, meshOwner: str = ...
     ) -> DescribeVirtualServiceOutputTypeDef:
         """
         Describes an existing virtual service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.describe_virtual_service)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#describe_virtual_service)
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
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#generate_presigned_url)
         """
-
     def list_gateway_routes(
         self,
         *,
         meshName: str,
         virtualGatewayName: str,
         limit: int = ...,
         meshOwner: str = ...,
@@ -425,23 +391,21 @@
         """
         Returns a list of existing gateway routes that are associated to a virtual
         gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.list_gateway_routes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#list_gateway_routes)
         """
-
     def list_meshes(self, *, limit: int = ..., nextToken: str = ...) -> ListMeshesOutputTypeDef:
         """
         Returns a list of existing service meshes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.list_meshes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#list_meshes)
         """
-
     def list_routes(
         self,
         *,
         meshName: str,
         virtualRouterName: str,
         limit: int = ...,
         meshOwner: str = ...,
@@ -449,174 +413,160 @@
     ) -> ListRoutesOutputTypeDef:
         """
         Returns a list of existing routes in a service mesh.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.list_routes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#list_routes)
         """
-
     def list_tags_for_resource(
         self, *, resourceArn: str, limit: int = ..., nextToken: str = ...
     ) -> ListTagsForResourceOutputTypeDef:
         """
         List the tags for an App Mesh resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#list_tags_for_resource)
         """
-
     def list_virtual_gateways(
         self, *, meshName: str, limit: int = ..., meshOwner: str = ..., nextToken: str = ...
     ) -> ListVirtualGatewaysOutputTypeDef:
         """
         Returns a list of existing virtual gateways in a service mesh.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.list_virtual_gateways)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#list_virtual_gateways)
         """
-
     def list_virtual_nodes(
         self, *, meshName: str, limit: int = ..., meshOwner: str = ..., nextToken: str = ...
     ) -> ListVirtualNodesOutputTypeDef:
         """
         Returns a list of existing virtual nodes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.list_virtual_nodes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#list_virtual_nodes)
         """
-
     def list_virtual_routers(
         self, *, meshName: str, limit: int = ..., meshOwner: str = ..., nextToken: str = ...
     ) -> ListVirtualRoutersOutputTypeDef:
         """
         Returns a list of existing virtual routers in a service mesh.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.list_virtual_routers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#list_virtual_routers)
         """
-
     def list_virtual_services(
         self, *, meshName: str, limit: int = ..., meshOwner: str = ..., nextToken: str = ...
     ) -> ListVirtualServicesOutputTypeDef:
         """
         Returns a list of existing virtual services in a service mesh.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.list_virtual_services)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#list_virtual_services)
         """
-
     def tag_resource(self, *, resourceArn: str, tags: Sequence[TagRefTypeDef]) -> Dict[str, Any]:
         """
         Associates the specified tags to a resource with the specified `resourceArn`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#tag_resource)
         """
-
     def untag_resource(self, *, resourceArn: str, tagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Deletes specified tags from a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#untag_resource)
         """
-
     def update_gateway_route(
         self,
         *,
         gatewayRouteName: str,
         meshName: str,
-        spec: Union[GatewayRouteSpecTypeDef, GatewayRouteSpecOutputTypeDef],
+        spec: GatewayRouteSpecUnionTypeDef,
         virtualGatewayName: str,
         clientToken: str = ...,
         meshOwner: str = ...
     ) -> UpdateGatewayRouteOutputTypeDef:
         """
         Updates an existing gateway route that is associated to a specified virtual
         gateway in a service mesh.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.update_gateway_route)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#update_gateway_route)
         """
-
     def update_mesh(
         self, *, meshName: str, clientToken: str = ..., spec: MeshSpecTypeDef = ...
     ) -> UpdateMeshOutputTypeDef:
         """
         Updates an existing service mesh.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.update_mesh)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#update_mesh)
         """
-
     def update_route(
         self,
         *,
         meshName: str,
         routeName: str,
-        spec: Union[RouteSpecTypeDef, RouteSpecOutputTypeDef],
+        spec: RouteSpecUnionTypeDef,
         virtualRouterName: str,
         clientToken: str = ...,
         meshOwner: str = ...
     ) -> UpdateRouteOutputTypeDef:
         """
         Updates an existing route for a specified service mesh and virtual router.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.update_route)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#update_route)
         """
-
     def update_virtual_gateway(
         self,
         *,
         meshName: str,
-        spec: Union[VirtualGatewaySpecTypeDef, VirtualGatewaySpecOutputTypeDef],
+        spec: VirtualGatewaySpecUnionTypeDef,
         virtualGatewayName: str,
         clientToken: str = ...,
         meshOwner: str = ...
     ) -> UpdateVirtualGatewayOutputTypeDef:
         """
         Updates an existing virtual gateway in a specified service mesh.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.update_virtual_gateway)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#update_virtual_gateway)
         """
-
     def update_virtual_node(
         self,
         *,
         meshName: str,
-        spec: Union[VirtualNodeSpecTypeDef, VirtualNodeSpecOutputTypeDef],
+        spec: VirtualNodeSpecUnionTypeDef,
         virtualNodeName: str,
         clientToken: str = ...,
         meshOwner: str = ...
     ) -> UpdateVirtualNodeOutputTypeDef:
         """
         Updates an existing virtual node in a specified service mesh.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.update_virtual_node)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#update_virtual_node)
         """
-
     def update_virtual_router(
         self,
         *,
         meshName: str,
-        spec: Union[VirtualRouterSpecTypeDef, VirtualRouterSpecOutputTypeDef],
+        spec: VirtualRouterSpecUnionTypeDef,
         virtualRouterName: str,
         clientToken: str = ...,
         meshOwner: str = ...
     ) -> UpdateVirtualRouterOutputTypeDef:
         """
         Updates an existing virtual router in a specified service mesh.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.update_virtual_router)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#update_virtual_router)
         """
-
     def update_virtual_service(
         self,
         *,
         meshName: str,
         spec: VirtualServiceSpecTypeDef,
         virtualServiceName: str,
         clientToken: str = ...,
@@ -624,74 +574,66 @@
     ) -> UpdateVirtualServiceOutputTypeDef:
         """
         Updates an existing virtual service in a specified service mesh.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.update_virtual_service)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#update_virtual_service)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_gateway_routes"]
     ) -> ListGatewayRoutesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["list_meshes"]) -> ListMeshesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["list_routes"]) -> ListRoutesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_tags_for_resource"]
     ) -> ListTagsForResourcePaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_virtual_gateways"]
     ) -> ListVirtualGatewaysPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_virtual_nodes"]
     ) -> ListVirtualNodesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_virtual_routers"]
     ) -> ListVirtualRoutersPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_virtual_services"]
     ) -> ListVirtualServicesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#get_paginator)
```

### Comparing `mypy-boto3-appmesh-1.28.15.post1/mypy_boto3_appmesh/client.pyi` & `mypy-boto3-appmesh-1.28.16/mypy_boto3_appmesh/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_appmesh.client import AppMeshClient
 
     session = Session()
     client: AppMeshClient = session.client("appmesh")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .paginator import (
     ListGatewayRoutesPaginator,
     ListMeshesPaginator,
     ListRoutesPaginator,
@@ -46,71 +46,70 @@
     DescribeGatewayRouteOutputTypeDef,
     DescribeMeshOutputTypeDef,
     DescribeRouteOutputTypeDef,
     DescribeVirtualGatewayOutputTypeDef,
     DescribeVirtualNodeOutputTypeDef,
     DescribeVirtualRouterOutputTypeDef,
     DescribeVirtualServiceOutputTypeDef,
-    GatewayRouteSpecOutputTypeDef,
-    GatewayRouteSpecTypeDef,
+    GatewayRouteSpecUnionTypeDef,
     ListGatewayRoutesOutputTypeDef,
     ListMeshesOutputTypeDef,
     ListRoutesOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     ListVirtualGatewaysOutputTypeDef,
     ListVirtualNodesOutputTypeDef,
     ListVirtualRoutersOutputTypeDef,
     ListVirtualServicesOutputTypeDef,
     MeshSpecTypeDef,
-    RouteSpecOutputTypeDef,
-    RouteSpecTypeDef,
+    RouteSpecUnionTypeDef,
     TagRefTypeDef,
     UpdateGatewayRouteOutputTypeDef,
     UpdateMeshOutputTypeDef,
     UpdateRouteOutputTypeDef,
     UpdateVirtualGatewayOutputTypeDef,
     UpdateVirtualNodeOutputTypeDef,
     UpdateVirtualRouterOutputTypeDef,
     UpdateVirtualServiceOutputTypeDef,
-    VirtualGatewaySpecOutputTypeDef,
-    VirtualGatewaySpecTypeDef,
-    VirtualNodeSpecOutputTypeDef,
-    VirtualNodeSpecTypeDef,
-    VirtualRouterSpecOutputTypeDef,
-    VirtualRouterSpecTypeDef,
+    VirtualGatewaySpecUnionTypeDef,
+    VirtualNodeSpecUnionTypeDef,
+    VirtualRouterSpecUnionTypeDef,
     VirtualServiceSpecTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = ("AppMeshClient",)
 
+
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     BadRequestException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     ForbiddenException: Type[BotocoreClientError]
     InternalServerErrorException: Type[BotocoreClientError]
     LimitExceededException: Type[BotocoreClientError]
     NotFoundException: Type[BotocoreClientError]
     ResourceInUseException: Type[BotocoreClientError]
     ServiceUnavailableException: Type[BotocoreClientError]
     TooManyRequestsException: Type[BotocoreClientError]
     TooManyTagsException: Type[BotocoreClientError]
 
+
 class AppMeshClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/)
     """
 
     meta: ClientMeta
@@ -119,124 +118,133 @@
     def exceptions(self) -> Exceptions:
         """
         AppMeshClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#exceptions)
         """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#can_paginate)
         """
+
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#close)
         """
+
     def create_gateway_route(
         self,
         *,
         gatewayRouteName: str,
         meshName: str,
-        spec: Union[GatewayRouteSpecTypeDef, GatewayRouteSpecOutputTypeDef],
+        spec: GatewayRouteSpecUnionTypeDef,
         virtualGatewayName: str,
         clientToken: str = ...,
         meshOwner: str = ...,
         tags: Sequence[TagRefTypeDef] = ...
     ) -> CreateGatewayRouteOutputTypeDef:
         """
         Creates a gateway route.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.create_gateway_route)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#create_gateway_route)
         """
+
     def create_mesh(
         self,
         *,
         meshName: str,
         clientToken: str = ...,
         spec: MeshSpecTypeDef = ...,
         tags: Sequence[TagRefTypeDef] = ...
     ) -> CreateMeshOutputTypeDef:
         """
         Creates a service mesh.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.create_mesh)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#create_mesh)
         """
+
     def create_route(
         self,
         *,
         meshName: str,
         routeName: str,
-        spec: Union[RouteSpecTypeDef, RouteSpecOutputTypeDef],
+        spec: RouteSpecUnionTypeDef,
         virtualRouterName: str,
         clientToken: str = ...,
         meshOwner: str = ...,
         tags: Sequence[TagRefTypeDef] = ...
     ) -> CreateRouteOutputTypeDef:
         """
         Creates a route that is associated with a virtual router.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.create_route)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#create_route)
         """
+
     def create_virtual_gateway(
         self,
         *,
         meshName: str,
-        spec: Union[VirtualGatewaySpecTypeDef, VirtualGatewaySpecOutputTypeDef],
+        spec: VirtualGatewaySpecUnionTypeDef,
         virtualGatewayName: str,
         clientToken: str = ...,
         meshOwner: str = ...,
         tags: Sequence[TagRefTypeDef] = ...
     ) -> CreateVirtualGatewayOutputTypeDef:
         """
         Creates a virtual gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.create_virtual_gateway)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#create_virtual_gateway)
         """
+
     def create_virtual_node(
         self,
         *,
         meshName: str,
-        spec: Union[VirtualNodeSpecTypeDef, VirtualNodeSpecOutputTypeDef],
+        spec: VirtualNodeSpecUnionTypeDef,
         virtualNodeName: str,
         clientToken: str = ...,
         meshOwner: str = ...,
         tags: Sequence[TagRefTypeDef] = ...
     ) -> CreateVirtualNodeOutputTypeDef:
         """
         Creates a virtual node within a service mesh.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.create_virtual_node)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#create_virtual_node)
         """
+
     def create_virtual_router(
         self,
         *,
         meshName: str,
-        spec: Union[VirtualRouterSpecTypeDef, VirtualRouterSpecOutputTypeDef],
+        spec: VirtualRouterSpecUnionTypeDef,
         virtualRouterName: str,
         clientToken: str = ...,
         meshOwner: str = ...,
         tags: Sequence[TagRefTypeDef] = ...
     ) -> CreateVirtualRouterOutputTypeDef:
         """
         Creates a virtual router within a service mesh.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.create_virtual_router)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#create_virtual_router)
         """
+
     def create_virtual_service(
         self,
         *,
         meshName: str,
         spec: VirtualServiceSpecTypeDef,
         virtualServiceName: str,
         clientToken: str = ...,
@@ -245,149 +253,165 @@
     ) -> CreateVirtualServiceOutputTypeDef:
         """
         Creates a virtual service within a service mesh.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.create_virtual_service)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#create_virtual_service)
         """
+
     def delete_gateway_route(
         self, *, gatewayRouteName: str, meshName: str, virtualGatewayName: str, meshOwner: str = ...
     ) -> DeleteGatewayRouteOutputTypeDef:
         """
         Deletes an existing gateway route.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.delete_gateway_route)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#delete_gateway_route)
         """
+
     def delete_mesh(self, *, meshName: str) -> DeleteMeshOutputTypeDef:
         """
         Deletes an existing service mesh.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.delete_mesh)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#delete_mesh)
         """
+
     def delete_route(
         self, *, meshName: str, routeName: str, virtualRouterName: str, meshOwner: str = ...
     ) -> DeleteRouteOutputTypeDef:
         """
         Deletes an existing route.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.delete_route)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#delete_route)
         """
+
     def delete_virtual_gateway(
         self, *, meshName: str, virtualGatewayName: str, meshOwner: str = ...
     ) -> DeleteVirtualGatewayOutputTypeDef:
         """
         Deletes an existing virtual gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.delete_virtual_gateway)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#delete_virtual_gateway)
         """
+
     def delete_virtual_node(
         self, *, meshName: str, virtualNodeName: str, meshOwner: str = ...
     ) -> DeleteVirtualNodeOutputTypeDef:
         """
         Deletes an existing virtual node.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.delete_virtual_node)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#delete_virtual_node)
         """
+
     def delete_virtual_router(
         self, *, meshName: str, virtualRouterName: str, meshOwner: str = ...
     ) -> DeleteVirtualRouterOutputTypeDef:
         """
         Deletes an existing virtual router.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.delete_virtual_router)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#delete_virtual_router)
         """
+
     def delete_virtual_service(
         self, *, meshName: str, virtualServiceName: str, meshOwner: str = ...
     ) -> DeleteVirtualServiceOutputTypeDef:
         """
         Deletes an existing virtual service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.delete_virtual_service)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#delete_virtual_service)
         """
+
     def describe_gateway_route(
         self, *, gatewayRouteName: str, meshName: str, virtualGatewayName: str, meshOwner: str = ...
     ) -> DescribeGatewayRouteOutputTypeDef:
         """
         Describes an existing gateway route.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.describe_gateway_route)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#describe_gateway_route)
         """
+
     def describe_mesh(self, *, meshName: str, meshOwner: str = ...) -> DescribeMeshOutputTypeDef:
         """
         Describes an existing service mesh.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.describe_mesh)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#describe_mesh)
         """
+
     def describe_route(
         self, *, meshName: str, routeName: str, virtualRouterName: str, meshOwner: str = ...
     ) -> DescribeRouteOutputTypeDef:
         """
         Describes an existing route.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.describe_route)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#describe_route)
         """
+
     def describe_virtual_gateway(
         self, *, meshName: str, virtualGatewayName: str, meshOwner: str = ...
     ) -> DescribeVirtualGatewayOutputTypeDef:
         """
         Describes an existing virtual gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.describe_virtual_gateway)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#describe_virtual_gateway)
         """
+
     def describe_virtual_node(
         self, *, meshName: str, virtualNodeName: str, meshOwner: str = ...
     ) -> DescribeVirtualNodeOutputTypeDef:
         """
         Describes an existing virtual node.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.describe_virtual_node)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#describe_virtual_node)
         """
+
     def describe_virtual_router(
         self, *, meshName: str, virtualRouterName: str, meshOwner: str = ...
     ) -> DescribeVirtualRouterOutputTypeDef:
         """
         Describes an existing virtual router.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.describe_virtual_router)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#describe_virtual_router)
         """
+
     def describe_virtual_service(
         self, *, meshName: str, virtualServiceName: str, meshOwner: str = ...
     ) -> DescribeVirtualServiceOutputTypeDef:
         """
         Describes an existing virtual service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.describe_virtual_service)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#describe_virtual_service)
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
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#generate_presigned_url)
         """
+
     def list_gateway_routes(
         self,
         *,
         meshName: str,
         virtualGatewayName: str,
         limit: int = ...,
         meshOwner: str = ...,
@@ -396,21 +420,23 @@
         """
         Returns a list of existing gateway routes that are associated to a virtual
         gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.list_gateway_routes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#list_gateway_routes)
         """
+
     def list_meshes(self, *, limit: int = ..., nextToken: str = ...) -> ListMeshesOutputTypeDef:
         """
         Returns a list of existing service meshes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.list_meshes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#list_meshes)
         """
+
     def list_routes(
         self,
         *,
         meshName: str,
         virtualRouterName: str,
         limit: int = ...,
         meshOwner: str = ...,
@@ -418,160 +444,174 @@
     ) -> ListRoutesOutputTypeDef:
         """
         Returns a list of existing routes in a service mesh.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.list_routes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#list_routes)
         """
+
     def list_tags_for_resource(
         self, *, resourceArn: str, limit: int = ..., nextToken: str = ...
     ) -> ListTagsForResourceOutputTypeDef:
         """
         List the tags for an App Mesh resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#list_tags_for_resource)
         """
+
     def list_virtual_gateways(
         self, *, meshName: str, limit: int = ..., meshOwner: str = ..., nextToken: str = ...
     ) -> ListVirtualGatewaysOutputTypeDef:
         """
         Returns a list of existing virtual gateways in a service mesh.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.list_virtual_gateways)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#list_virtual_gateways)
         """
+
     def list_virtual_nodes(
         self, *, meshName: str, limit: int = ..., meshOwner: str = ..., nextToken: str = ...
     ) -> ListVirtualNodesOutputTypeDef:
         """
         Returns a list of existing virtual nodes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.list_virtual_nodes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#list_virtual_nodes)
         """
+
     def list_virtual_routers(
         self, *, meshName: str, limit: int = ..., meshOwner: str = ..., nextToken: str = ...
     ) -> ListVirtualRoutersOutputTypeDef:
         """
         Returns a list of existing virtual routers in a service mesh.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.list_virtual_routers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#list_virtual_routers)
         """
+
     def list_virtual_services(
         self, *, meshName: str, limit: int = ..., meshOwner: str = ..., nextToken: str = ...
     ) -> ListVirtualServicesOutputTypeDef:
         """
         Returns a list of existing virtual services in a service mesh.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.list_virtual_services)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#list_virtual_services)
         """
+
     def tag_resource(self, *, resourceArn: str, tags: Sequence[TagRefTypeDef]) -> Dict[str, Any]:
         """
         Associates the specified tags to a resource with the specified `resourceArn`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#tag_resource)
         """
+
     def untag_resource(self, *, resourceArn: str, tagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Deletes specified tags from a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#untag_resource)
         """
+
     def update_gateway_route(
         self,
         *,
         gatewayRouteName: str,
         meshName: str,
-        spec: Union[GatewayRouteSpecTypeDef, GatewayRouteSpecOutputTypeDef],
+        spec: GatewayRouteSpecUnionTypeDef,
         virtualGatewayName: str,
         clientToken: str = ...,
         meshOwner: str = ...
     ) -> UpdateGatewayRouteOutputTypeDef:
         """
         Updates an existing gateway route that is associated to a specified virtual
         gateway in a service mesh.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.update_gateway_route)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#update_gateway_route)
         """
+
     def update_mesh(
         self, *, meshName: str, clientToken: str = ..., spec: MeshSpecTypeDef = ...
     ) -> UpdateMeshOutputTypeDef:
         """
         Updates an existing service mesh.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.update_mesh)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#update_mesh)
         """
+
     def update_route(
         self,
         *,
         meshName: str,
         routeName: str,
-        spec: Union[RouteSpecTypeDef, RouteSpecOutputTypeDef],
+        spec: RouteSpecUnionTypeDef,
         virtualRouterName: str,
         clientToken: str = ...,
         meshOwner: str = ...
     ) -> UpdateRouteOutputTypeDef:
         """
         Updates an existing route for a specified service mesh and virtual router.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.update_route)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#update_route)
         """
+
     def update_virtual_gateway(
         self,
         *,
         meshName: str,
-        spec: Union[VirtualGatewaySpecTypeDef, VirtualGatewaySpecOutputTypeDef],
+        spec: VirtualGatewaySpecUnionTypeDef,
         virtualGatewayName: str,
         clientToken: str = ...,
         meshOwner: str = ...
     ) -> UpdateVirtualGatewayOutputTypeDef:
         """
         Updates an existing virtual gateway in a specified service mesh.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.update_virtual_gateway)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#update_virtual_gateway)
         """
+
     def update_virtual_node(
         self,
         *,
         meshName: str,
-        spec: Union[VirtualNodeSpecTypeDef, VirtualNodeSpecOutputTypeDef],
+        spec: VirtualNodeSpecUnionTypeDef,
         virtualNodeName: str,
         clientToken: str = ...,
         meshOwner: str = ...
     ) -> UpdateVirtualNodeOutputTypeDef:
         """
         Updates an existing virtual node in a specified service mesh.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.update_virtual_node)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#update_virtual_node)
         """
+
     def update_virtual_router(
         self,
         *,
         meshName: str,
-        spec: Union[VirtualRouterSpecTypeDef, VirtualRouterSpecOutputTypeDef],
+        spec: VirtualRouterSpecUnionTypeDef,
         virtualRouterName: str,
         clientToken: str = ...,
         meshOwner: str = ...
     ) -> UpdateVirtualRouterOutputTypeDef:
         """
         Updates an existing virtual router in a specified service mesh.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.update_virtual_router)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#update_virtual_router)
         """
+
     def update_virtual_service(
         self,
         *,
         meshName: str,
         spec: VirtualServiceSpecTypeDef,
         virtualServiceName: str,
         clientToken: str = ...,
@@ -579,66 +619,74 @@
     ) -> UpdateVirtualServiceOutputTypeDef:
         """
         Updates an existing virtual service in a specified service mesh.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.update_virtual_service)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#update_virtual_service)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_gateway_routes"]
     ) -> ListGatewayRoutesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["list_meshes"]) -> ListMeshesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["list_routes"]) -> ListRoutesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_tags_for_resource"]
     ) -> ListTagsForResourcePaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_virtual_gateways"]
     ) -> ListVirtualGatewaysPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_virtual_nodes"]
     ) -> ListVirtualNodesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_virtual_routers"]
     ) -> ListVirtualRoutersPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_virtual_services"]
     ) -> ListVirtualServicesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/client/#get_paginator)
```

### Comparing `mypy-boto3-appmesh-1.28.15.post1/mypy_boto3_appmesh/literals.py` & `mypy-boto3-appmesh-1.28.16/mypy_boto3_appmesh/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appmesh-1.28.15.post1/mypy_boto3_appmesh/literals.pyi` & `mypy-boto3-appmesh-1.28.16/mypy_boto3_appmesh/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appmesh-1.28.15.post1/mypy_boto3_appmesh/paginator.py` & `mypy-boto3-appmesh-1.28.16/mypy_boto3_appmesh/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appmesh-1.28.15.post1/mypy_boto3_appmesh/paginator.pyi` & `mypy-boto3-appmesh-1.28.16/mypy_boto3_appmesh/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appmesh-1.28.15.post1/mypy_boto3_appmesh/type_defs.py` & `mypy-boto3-appmesh-1.28.16/mypy_boto3_appmesh/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_appmesh.type_defs import AwsCloudMapInstanceAttributeTypeDef
 
-    data: AwsCloudMapInstanceAttributeTypeDef = {...}
+    data: AwsCloudMapInstanceAttributeTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence
+from typing import Dict, List, Sequence, Union
 
 from .literals import (
     DefaultGatewayRouteRewriteType,
     DnsResponseTypeType,
     DurationUnitType,
     EgressFilterTypeType,
     GatewayRouteStatusCodeType,
@@ -233,14 +233,15 @@
     "AccessLogOutputTypeDef",
     "VirtualGatewayAccessLogOutputTypeDef",
     "AccessLogTypeDef",
     "VirtualGatewayAccessLogTypeDef",
     "VirtualRouterDataTypeDef",
     "CreateVirtualRouterInputRequestTypeDef",
     "UpdateVirtualRouterInputRequestTypeDef",
+    "VirtualRouterSpecUnionTypeDef",
     "CreateMeshOutputTypeDef",
     "DeleteMeshOutputTypeDef",
     "DescribeMeshOutputTypeDef",
     "UpdateMeshOutputTypeDef",
     "ListenerTlsOutputTypeDef",
     "ListenerTlsTypeDef",
     "ClientPolicyTlsOutputTypeDef",
@@ -288,17 +289,19 @@
     "VirtualServiceBackendOutputTypeDef",
     "BackendDefaultsTypeDef",
     "VirtualServiceBackendTypeDef",
     "VirtualGatewayBackendDefaultsOutputTypeDef",
     "VirtualGatewayBackendDefaultsTypeDef",
     "GatewayRouteDataTypeDef",
     "CreateGatewayRouteInputRequestTypeDef",
+    "GatewayRouteSpecUnionTypeDef",
     "UpdateGatewayRouteInputRequestTypeDef",
     "RouteDataTypeDef",
     "CreateRouteInputRequestTypeDef",
+    "RouteSpecUnionTypeDef",
     "UpdateRouteInputRequestTypeDef",
     "BackendOutputTypeDef",
     "BackendTypeDef",
     "VirtualGatewaySpecOutputTypeDef",
     "VirtualGatewaySpecTypeDef",
     "CreateGatewayRouteOutputTypeDef",
     "DeleteGatewayRouteOutputTypeDef",
@@ -309,17 +312,19 @@
     "DescribeRouteOutputTypeDef",
     "UpdateRouteOutputTypeDef",
     "VirtualNodeSpecOutputTypeDef",
     "VirtualNodeSpecTypeDef",
     "VirtualGatewayDataTypeDef",
     "CreateVirtualGatewayInputRequestTypeDef",
     "UpdateVirtualGatewayInputRequestTypeDef",
+    "VirtualGatewaySpecUnionTypeDef",
     "VirtualNodeDataTypeDef",
     "CreateVirtualNodeInputRequestTypeDef",
     "UpdateVirtualNodeInputRequestTypeDef",
+    "VirtualNodeSpecUnionTypeDef",
     "CreateVirtualGatewayOutputTypeDef",
     "DeleteVirtualGatewayOutputTypeDef",
     "DescribeVirtualGatewayOutputTypeDef",
     "UpdateVirtualGatewayOutputTypeDef",
     "CreateVirtualNodeOutputTypeDef",
     "DeleteVirtualNodeOutputTypeDef",
     "DescribeVirtualNodeOutputTypeDef",
@@ -2883,14 +2888,15 @@
 
 class UpdateVirtualRouterInputRequestTypeDef(
     _RequiredUpdateVirtualRouterInputRequestTypeDef, _OptionalUpdateVirtualRouterInputRequestTypeDef
 ):
     pass
 
 
+VirtualRouterSpecUnionTypeDef = Union[VirtualRouterSpecTypeDef, VirtualRouterSpecOutputTypeDef]
 CreateMeshOutputTypeDef = TypedDict(
     "CreateMeshOutputTypeDef",
     {
         "mesh": MeshDataTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -3648,14 +3654,15 @@
 
 class CreateGatewayRouteInputRequestTypeDef(
     _RequiredCreateGatewayRouteInputRequestTypeDef, _OptionalCreateGatewayRouteInputRequestTypeDef
 ):
     pass
 
 
+GatewayRouteSpecUnionTypeDef = Union[GatewayRouteSpecTypeDef, GatewayRouteSpecOutputTypeDef]
 _RequiredUpdateGatewayRouteInputRequestTypeDef = TypedDict(
     "_RequiredUpdateGatewayRouteInputRequestTypeDef",
     {
         "gatewayRouteName": str,
         "meshName": str,
         "spec": GatewayRouteSpecTypeDef,
         "virtualGatewayName": str,
@@ -3711,14 +3718,15 @@
 
 class CreateRouteInputRequestTypeDef(
     _RequiredCreateRouteInputRequestTypeDef, _OptionalCreateRouteInputRequestTypeDef
 ):
     pass
 
 
+RouteSpecUnionTypeDef = Union[RouteSpecTypeDef, RouteSpecOutputTypeDef]
 _RequiredUpdateRouteInputRequestTypeDef = TypedDict(
     "_RequiredUpdateRouteInputRequestTypeDef",
     {
         "meshName": str,
         "routeName": str,
         "spec": RouteSpecTypeDef,
         "virtualRouterName": str,
@@ -3946,14 +3954,15 @@
 class UpdateVirtualGatewayInputRequestTypeDef(
     _RequiredUpdateVirtualGatewayInputRequestTypeDef,
     _OptionalUpdateVirtualGatewayInputRequestTypeDef,
 ):
     pass
 
 
+VirtualGatewaySpecUnionTypeDef = Union[VirtualGatewaySpecTypeDef, VirtualGatewaySpecOutputTypeDef]
 VirtualNodeDataTypeDef = TypedDict(
     "VirtualNodeDataTypeDef",
     {
         "meshName": str,
         "metadata": ResourceMetadataTypeDef,
         "spec": VirtualNodeSpecOutputTypeDef,
         "status": VirtualNodeStatusTypeDef,
@@ -4006,14 +4015,15 @@
 
 class UpdateVirtualNodeInputRequestTypeDef(
     _RequiredUpdateVirtualNodeInputRequestTypeDef, _OptionalUpdateVirtualNodeInputRequestTypeDef
 ):
     pass
 
 
+VirtualNodeSpecUnionTypeDef = Union[VirtualNodeSpecTypeDef, VirtualNodeSpecOutputTypeDef]
 CreateVirtualGatewayOutputTypeDef = TypedDict(
     "CreateVirtualGatewayOutputTypeDef",
     {
         "virtualGateway": VirtualGatewayDataTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-appmesh-1.28.15.post1/mypy_boto3_appmesh/type_defs.pyi` & `mypy-boto3-appmesh-1.28.16/mypy_boto3_appmesh/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_appmesh.type_defs import AwsCloudMapInstanceAttributeTypeDef
 
-    data: AwsCloudMapInstanceAttributeTypeDef = {...}
+    data: AwsCloudMapInstanceAttributeTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence
+from typing import Dict, List, Sequence, Union
 
 from .literals import (
     DefaultGatewayRouteRewriteType,
     DnsResponseTypeType,
     DurationUnitType,
     EgressFilterTypeType,
     GatewayRouteStatusCodeType,
@@ -232,14 +232,15 @@
     "AccessLogOutputTypeDef",
     "VirtualGatewayAccessLogOutputTypeDef",
     "AccessLogTypeDef",
     "VirtualGatewayAccessLogTypeDef",
     "VirtualRouterDataTypeDef",
     "CreateVirtualRouterInputRequestTypeDef",
     "UpdateVirtualRouterInputRequestTypeDef",
+    "VirtualRouterSpecUnionTypeDef",
     "CreateMeshOutputTypeDef",
     "DeleteMeshOutputTypeDef",
     "DescribeMeshOutputTypeDef",
     "UpdateMeshOutputTypeDef",
     "ListenerTlsOutputTypeDef",
     "ListenerTlsTypeDef",
     "ClientPolicyTlsOutputTypeDef",
@@ -287,17 +288,19 @@
     "VirtualServiceBackendOutputTypeDef",
     "BackendDefaultsTypeDef",
     "VirtualServiceBackendTypeDef",
     "VirtualGatewayBackendDefaultsOutputTypeDef",
     "VirtualGatewayBackendDefaultsTypeDef",
     "GatewayRouteDataTypeDef",
     "CreateGatewayRouteInputRequestTypeDef",
+    "GatewayRouteSpecUnionTypeDef",
     "UpdateGatewayRouteInputRequestTypeDef",
     "RouteDataTypeDef",
     "CreateRouteInputRequestTypeDef",
+    "RouteSpecUnionTypeDef",
     "UpdateRouteInputRequestTypeDef",
     "BackendOutputTypeDef",
     "BackendTypeDef",
     "VirtualGatewaySpecOutputTypeDef",
     "VirtualGatewaySpecTypeDef",
     "CreateGatewayRouteOutputTypeDef",
     "DeleteGatewayRouteOutputTypeDef",
@@ -308,17 +311,19 @@
     "DescribeRouteOutputTypeDef",
     "UpdateRouteOutputTypeDef",
     "VirtualNodeSpecOutputTypeDef",
     "VirtualNodeSpecTypeDef",
     "VirtualGatewayDataTypeDef",
     "CreateVirtualGatewayInputRequestTypeDef",
     "UpdateVirtualGatewayInputRequestTypeDef",
+    "VirtualGatewaySpecUnionTypeDef",
     "VirtualNodeDataTypeDef",
     "CreateVirtualNodeInputRequestTypeDef",
     "UpdateVirtualNodeInputRequestTypeDef",
+    "VirtualNodeSpecUnionTypeDef",
     "CreateVirtualGatewayOutputTypeDef",
     "DeleteVirtualGatewayOutputTypeDef",
     "DescribeVirtualGatewayOutputTypeDef",
     "UpdateVirtualGatewayOutputTypeDef",
     "CreateVirtualNodeOutputTypeDef",
     "DeleteVirtualNodeOutputTypeDef",
     "DescribeVirtualNodeOutputTypeDef",
@@ -2752,14 +2757,15 @@
 )
 
 class UpdateVirtualRouterInputRequestTypeDef(
     _RequiredUpdateVirtualRouterInputRequestTypeDef, _OptionalUpdateVirtualRouterInputRequestTypeDef
 ):
     pass
 
+VirtualRouterSpecUnionTypeDef = Union[VirtualRouterSpecTypeDef, VirtualRouterSpecOutputTypeDef]
 CreateMeshOutputTypeDef = TypedDict(
     "CreateMeshOutputTypeDef",
     {
         "mesh": MeshDataTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -3475,14 +3481,15 @@
 )
 
 class CreateGatewayRouteInputRequestTypeDef(
     _RequiredCreateGatewayRouteInputRequestTypeDef, _OptionalCreateGatewayRouteInputRequestTypeDef
 ):
     pass
 
+GatewayRouteSpecUnionTypeDef = Union[GatewayRouteSpecTypeDef, GatewayRouteSpecOutputTypeDef]
 _RequiredUpdateGatewayRouteInputRequestTypeDef = TypedDict(
     "_RequiredUpdateGatewayRouteInputRequestTypeDef",
     {
         "gatewayRouteName": str,
         "meshName": str,
         "spec": GatewayRouteSpecTypeDef,
         "virtualGatewayName": str,
@@ -3534,14 +3541,15 @@
 )
 
 class CreateRouteInputRequestTypeDef(
     _RequiredCreateRouteInputRequestTypeDef, _OptionalCreateRouteInputRequestTypeDef
 ):
     pass
 
+RouteSpecUnionTypeDef = Union[RouteSpecTypeDef, RouteSpecOutputTypeDef]
 _RequiredUpdateRouteInputRequestTypeDef = TypedDict(
     "_RequiredUpdateRouteInputRequestTypeDef",
     {
         "meshName": str,
         "routeName": str,
         "spec": RouteSpecTypeDef,
         "virtualRouterName": str,
@@ -3759,14 +3767,15 @@
 
 class UpdateVirtualGatewayInputRequestTypeDef(
     _RequiredUpdateVirtualGatewayInputRequestTypeDef,
     _OptionalUpdateVirtualGatewayInputRequestTypeDef,
 ):
     pass
 
+VirtualGatewaySpecUnionTypeDef = Union[VirtualGatewaySpecTypeDef, VirtualGatewaySpecOutputTypeDef]
 VirtualNodeDataTypeDef = TypedDict(
     "VirtualNodeDataTypeDef",
     {
         "meshName": str,
         "metadata": ResourceMetadataTypeDef,
         "spec": VirtualNodeSpecOutputTypeDef,
         "status": VirtualNodeStatusTypeDef,
@@ -3815,14 +3824,15 @@
 )
 
 class UpdateVirtualNodeInputRequestTypeDef(
     _RequiredUpdateVirtualNodeInputRequestTypeDef, _OptionalUpdateVirtualNodeInputRequestTypeDef
 ):
     pass
 
+VirtualNodeSpecUnionTypeDef = Union[VirtualNodeSpecTypeDef, VirtualNodeSpecOutputTypeDef]
 CreateVirtualGatewayOutputTypeDef = TypedDict(
     "CreateVirtualGatewayOutputTypeDef",
     {
         "virtualGateway": VirtualGatewayDataTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-appmesh-1.28.15.post1/mypy_boto3_appmesh.egg-info/PKG-INFO` & `mypy-boto3-appmesh-1.28.16/mypy_boto3_appmesh.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-appmesh
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.AppMesh 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.AppMesh 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 appmesh type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 appmesh type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-appmesh.svg?color=blue)](https://pypi.org/project/mypy-boto3-appmesh)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-appmesh)](https://pepy.tech/project/mypy-boto3-appmesh)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AppMesh 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh)
+[boto3.AppMesh 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh)
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
 [mypy-boto3-appmesh docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/).
 
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
@@ -362,20 +362,20 @@
 )
 
 
 def check_value(value: DefaultGatewayRouteRewriteType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_appmesh.type_defs` module contains structures and shapes assembled
-to typed dictionaries for additional type checking.
+to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_appmesh.type_defs import (
     AwsCloudMapInstanceAttributeTypeDef,
     ListenerTlsFileCertificateTypeDef,
     ListenerTlsSdsCertificateTypeDef,
     TagRefTypeDef,
@@ -560,14 +560,15 @@
     AccessLogOutputTypeDef,
     VirtualGatewayAccessLogOutputTypeDef,
     AccessLogTypeDef,
     VirtualGatewayAccessLogTypeDef,
     VirtualRouterDataTypeDef,
     CreateVirtualRouterInputRequestTypeDef,
     UpdateVirtualRouterInputRequestTypeDef,
+    VirtualRouterSpecUnionTypeDef,
     CreateMeshOutputTypeDef,
     DeleteMeshOutputTypeDef,
     DescribeMeshOutputTypeDef,
     UpdateMeshOutputTypeDef,
     ListenerTlsOutputTypeDef,
     ListenerTlsTypeDef,
     ClientPolicyTlsOutputTypeDef,
@@ -615,17 +616,19 @@
     VirtualServiceBackendOutputTypeDef,
     BackendDefaultsTypeDef,
     VirtualServiceBackendTypeDef,
     VirtualGatewayBackendDefaultsOutputTypeDef,
     VirtualGatewayBackendDefaultsTypeDef,
     GatewayRouteDataTypeDef,
     CreateGatewayRouteInputRequestTypeDef,
+    GatewayRouteSpecUnionTypeDef,
     UpdateGatewayRouteInputRequestTypeDef,
     RouteDataTypeDef,
     CreateRouteInputRequestTypeDef,
+    RouteSpecUnionTypeDef,
     UpdateRouteInputRequestTypeDef,
     BackendOutputTypeDef,
     BackendTypeDef,
     VirtualGatewaySpecOutputTypeDef,
     VirtualGatewaySpecTypeDef,
     CreateGatewayRouteOutputTypeDef,
     DeleteGatewayRouteOutputTypeDef,
@@ -636,29 +639,31 @@
     DescribeRouteOutputTypeDef,
     UpdateRouteOutputTypeDef,
     VirtualNodeSpecOutputTypeDef,
     VirtualNodeSpecTypeDef,
     VirtualGatewayDataTypeDef,
     CreateVirtualGatewayInputRequestTypeDef,
     UpdateVirtualGatewayInputRequestTypeDef,
+    VirtualGatewaySpecUnionTypeDef,
     VirtualNodeDataTypeDef,
     CreateVirtualNodeInputRequestTypeDef,
     UpdateVirtualNodeInputRequestTypeDef,
+    VirtualNodeSpecUnionTypeDef,
     CreateVirtualGatewayOutputTypeDef,
     DeleteVirtualGatewayOutputTypeDef,
     DescribeVirtualGatewayOutputTypeDef,
     UpdateVirtualGatewayOutputTypeDef,
     CreateVirtualNodeOutputTypeDef,
     DeleteVirtualNodeOutputTypeDef,
     DescribeVirtualNodeOutputTypeDef,
     UpdateVirtualNodeOutputTypeDef,
 )
 
 
-def get_structure() -> AwsCloudMapInstanceAttributeTypeDef:
+def get_value() -> AwsCloudMapInstanceAttributeTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-appmesh-1.28.15.post1/mypy_boto3_appmesh.egg-info/SOURCES.txt` & `mypy-boto3-appmesh-1.28.16/mypy_boto3_appmesh.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appmesh-1.28.15.post1/setup.py` & `mypy-boto3-appmesh-1.28.16/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-appmesh",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_appmesh"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.AppMesh 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.2"
+        "Type annotations for boto3.AppMesh 1.28.16 service generated with mypy-boto3-builder"
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
-    keywords="boto3 appmesh type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 appmesh type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_appmesh": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

