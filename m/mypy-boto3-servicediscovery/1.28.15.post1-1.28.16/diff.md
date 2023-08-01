# Comparing `tmp/mypy-boto3-servicediscovery-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-servicediscovery-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-servicediscovery-1.28.15.post1.tar", last modified: Sat Jul 29 10:04:11 2023, max compression
+gzip compressed data, was "mypy-boto3-servicediscovery-1.28.16.tar", last modified: Tue Aug  1 11:37:51 2023, max compression
```

## Comparing `mypy-boto3-servicediscovery-1.28.15.post1.tar` & `mypy-boto3-servicediscovery-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:11.985403 mypy-boto3-servicediscovery-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:59:28.000000 mypy-boto3-servicediscovery-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17200 2023-07-29 10:04:11.977403 mypy-boto3-servicediscovery-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15671 2023-07-29 09:59:28.000000 mypy-boto3-servicediscovery-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:11.977403 mypy-boto3-servicediscovery-1.28.15.post1/mypy_boto3_servicediscovery/
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-07-29 09:59:28.000000 mypy-boto3-servicediscovery-1.28.15.post1/mypy_boto3_servicediscovery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-07-29 09:59:28.000000 mypy-boto3-servicediscovery-1.28.15.post1/mypy_boto3_servicediscovery/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-29 09:59:28.000000 mypy-boto3-servicediscovery-1.28.15.post1/mypy_boto3_servicediscovery/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22879 2023-07-29 09:59:28.000000 mypy-boto3-servicediscovery-1.28.15.post1/mypy_boto3_servicediscovery/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    22842 2023-07-29 09:59:28.000000 mypy-boto3-servicediscovery-1.28.15.post1/mypy_boto3_servicediscovery/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10247 2023-07-29 09:59:29.000000 mypy-boto3-servicediscovery-1.28.15.post1/mypy_boto3_servicediscovery/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10245 2023-07-29 09:59:28.000000 mypy-boto3-servicediscovery-1.28.15.post1/mypy_boto3_servicediscovery/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-07-29 09:59:28.000000 mypy-boto3-servicediscovery-1.28.15.post1/mypy_boto3_servicediscovery/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5434 2023-07-29 09:59:28.000000 mypy-boto3-servicediscovery-1.28.15.post1/mypy_boto3_servicediscovery/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:59:28.000000 mypy-boto3-servicediscovery-1.28.15.post1/mypy_boto3_servicediscovery/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    28902 2023-07-29 09:59:29.000000 mypy-boto3-servicediscovery-1.28.15.post1/mypy_boto3_servicediscovery/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    28864 2023-07-29 09:59:29.000000 mypy-boto3-servicediscovery-1.28.15.post1/mypy_boto3_servicediscovery/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:59:28.000000 mypy-boto3-servicediscovery-1.28.15.post1/mypy_boto3_servicediscovery/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:11.977403 mypy-boto3-servicediscovery-1.28.15.post1/mypy_boto3_servicediscovery.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17200 2023-07-29 10:04:11.000000 mypy-boto3-servicediscovery-1.28.15.post1/mypy_boto3_servicediscovery.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-29 10:04:11.000000 mypy-boto3-servicediscovery-1.28.15.post1/mypy_boto3_servicediscovery.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:11.000000 mypy-boto3-servicediscovery-1.28.15.post1/mypy_boto3_servicediscovery.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:11.000000 mypy-boto3-servicediscovery-1.28.15.post1/mypy_boto3_servicediscovery.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:04:11.000000 mypy-boto3-servicediscovery-1.28.15.post1/mypy_boto3_servicediscovery.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-29 10:04:11.000000 mypy-boto3-servicediscovery-1.28.15.post1/mypy_boto3_servicediscovery.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:04:11.985403 mypy-boto3-servicediscovery-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-07-29 09:59:28.000000 mypy-boto3-servicediscovery-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:51.660729 mypy-boto3-servicediscovery-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:33:00.000000 mypy-boto3-servicediscovery-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17217 2023-08-01 11:37:51.660729 mypy-boto3-servicediscovery-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15697 2023-08-01 11:33:00.000000 mypy-boto3-servicediscovery-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:51.648729 mypy-boto3-servicediscovery-1.28.16/mypy_boto3_servicediscovery/
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-08-01 11:33:00.000000 mypy-boto3-servicediscovery-1.28.16/mypy_boto3_servicediscovery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-08-01 11:33:00.000000 mypy-boto3-servicediscovery-1.28.16/mypy_boto3_servicediscovery/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-08-01 11:33:00.000000 mypy-boto3-servicediscovery-1.28.16/mypy_boto3_servicediscovery/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22823 2023-08-01 11:33:00.000000 mypy-boto3-servicediscovery-1.28.16/mypy_boto3_servicediscovery/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22786 2023-08-01 11:33:00.000000 mypy-boto3-servicediscovery-1.28.16/mypy_boto3_servicediscovery/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10247 2023-08-01 11:33:01.000000 mypy-boto3-servicediscovery-1.28.16/mypy_boto3_servicediscovery/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10245 2023-08-01 11:33:00.000000 mypy-boto3-servicediscovery-1.28.16/mypy_boto3_servicediscovery/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-08-01 11:33:00.000000 mypy-boto3-servicediscovery-1.28.16/mypy_boto3_servicediscovery/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5434 2023-08-01 11:33:00.000000 mypy-boto3-servicediscovery-1.28.16/mypy_boto3_servicediscovery/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:33:00.000000 mypy-boto3-servicediscovery-1.28.16/mypy_boto3_servicediscovery/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    29008 2023-08-01 11:33:01.000000 mypy-boto3-servicediscovery-1.28.16/mypy_boto3_servicediscovery/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28970 2023-08-01 11:33:01.000000 mypy-boto3-servicediscovery-1.28.16/mypy_boto3_servicediscovery/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:33:00.000000 mypy-boto3-servicediscovery-1.28.16/mypy_boto3_servicediscovery/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:37:51.652729 mypy-boto3-servicediscovery-1.28.16/mypy_boto3_servicediscovery.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17217 2023-08-01 11:37:51.000000 mypy-boto3-servicediscovery-1.28.16/mypy_boto3_servicediscovery.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-08-01 11:37:51.000000 mypy-boto3-servicediscovery-1.28.16/mypy_boto3_servicediscovery.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:51.000000 mypy-boto3-servicediscovery-1.28.16/mypy_boto3_servicediscovery.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:37:51.000000 mypy-boto3-servicediscovery-1.28.16/mypy_boto3_servicediscovery.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:37:51.000000 mypy-boto3-servicediscovery-1.28.16/mypy_boto3_servicediscovery.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-01 11:37:51.000000 mypy-boto3-servicediscovery-1.28.16/mypy_boto3_servicediscovery.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:37:51.660729 mypy-boto3-servicediscovery-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-08-01 11:33:00.000000 mypy-boto3-servicediscovery-1.28.16/setup.py
```

### Comparing `mypy-boto3-servicediscovery-1.28.15.post1/LICENSE` & `mypy-boto3-servicediscovery-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-servicediscovery-1.28.15.post1/PKG-INFO` & `mypy-boto3-servicediscovery-1.28.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-servicediscovery
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.ServiceDiscovery 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.ServiceDiscovery 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicediscovery/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 servicediscovery type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 servicediscovery type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-servicediscovery.svg?color=blue)](https://pypi.org/project/mypy-boto3-servicediscovery)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicediscovery/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-servicediscovery)](https://pepy.tech/project/mypy-boto3-servicediscovery)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ServiceDiscovery 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery)
+[boto3.ServiceDiscovery 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery)
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
 [mypy-boto3-servicediscovery docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicediscovery/).
 
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
@@ -338,20 +338,20 @@
 )
 
 
 def check_value(value: CustomHealthStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_servicediscovery.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_servicediscovery.type_defs import (
     TagTypeDef,
     ResponseMetadataTypeDef,
     HealthCheckConfigTypeDef,
     HealthCheckCustomConfigTypeDef,
@@ -419,14 +419,15 @@
     ListServicesRequestRequestTypeDef,
     PrivateDnsPropertiesMutableChangeTypeDef,
     PublicDnsPropertiesMutableChangeTypeDef,
     ServiceChangeTypeDef,
     ServiceSummaryTypeDef,
     ServiceTypeDef,
     CreateServiceRequestRequestTypeDef,
+    DnsConfigUnionTypeDef,
     NamespacePropertiesTypeDef,
     PrivateDnsNamespacePropertiesTypeDef,
     PublicDnsNamespacePropertiesTypeDef,
     PrivateDnsNamespacePropertiesChangeTypeDef,
     PublicDnsNamespacePropertiesChangeTypeDef,
     UpdateServiceRequestRequestTypeDef,
     ListServicesResponseTypeDef,
@@ -441,15 +442,15 @@
     ListNamespacesResponseTypeDef,
     GetNamespaceResponseTypeDef,
     UpdatePrivateDnsNamespaceRequestRequestTypeDef,
     UpdatePublicDnsNamespaceRequestRequestTypeDef,
 )
 
 
-def get_structure() -> TagTypeDef:
+def get_value() -> TagTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-servicediscovery-1.28.15.post1/README.md` & `mypy-boto3-servicediscovery-1.28.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-servicediscovery.svg?color=blue)](https://pypi.org/project/mypy-boto3-servicediscovery)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicediscovery/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-servicediscovery)](https://pepy.tech/project/mypy-boto3-servicediscovery)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ServiceDiscovery 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery)
+[boto3.ServiceDiscovery 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery)
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
 [mypy-boto3-servicediscovery docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicediscovery/).
 
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
@@ -306,20 +306,20 @@
 )
 
 
 def check_value(value: CustomHealthStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_servicediscovery.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_servicediscovery.type_defs import (
     TagTypeDef,
     ResponseMetadataTypeDef,
     HealthCheckConfigTypeDef,
     HealthCheckCustomConfigTypeDef,
@@ -387,14 +387,15 @@
     ListServicesRequestRequestTypeDef,
     PrivateDnsPropertiesMutableChangeTypeDef,
     PublicDnsPropertiesMutableChangeTypeDef,
     ServiceChangeTypeDef,
     ServiceSummaryTypeDef,
     ServiceTypeDef,
     CreateServiceRequestRequestTypeDef,
+    DnsConfigUnionTypeDef,
     NamespacePropertiesTypeDef,
     PrivateDnsNamespacePropertiesTypeDef,
     PublicDnsNamespacePropertiesTypeDef,
     PrivateDnsNamespacePropertiesChangeTypeDef,
     PublicDnsNamespacePropertiesChangeTypeDef,
     UpdateServiceRequestRequestTypeDef,
     ListServicesResponseTypeDef,
@@ -409,15 +410,15 @@
     ListNamespacesResponseTypeDef,
     GetNamespaceResponseTypeDef,
     UpdatePrivateDnsNamespaceRequestRequestTypeDef,
     UpdatePublicDnsNamespaceRequestRequestTypeDef,
 )
 
 
-def get_structure() -> TagTypeDef:
+def get_value() -> TagTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-servicediscovery-1.28.15.post1/mypy_boto3_servicediscovery/__init__.py` & `mypy-boto3-servicediscovery-1.28.16/mypy_boto3_servicediscovery/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-servicediscovery-1.28.15.post1/mypy_boto3_servicediscovery/__init__.pyi` & `mypy-boto3-servicediscovery-1.28.16/mypy_boto3_servicediscovery/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-servicediscovery-1.28.15.post1/mypy_boto3_servicediscovery/__main__.py` & `mypy-boto3-servicediscovery-1.28.16/mypy_boto3_servicediscovery/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ServiceDiscovery 1.28.15\nVersion:        "
-        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.ServiceDiscovery 1.28.16\nVersion:         1.28.16\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicediscovery//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery\nOther"
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

### Comparing `mypy-boto3-servicediscovery-1.28.15.post1/mypy_boto3_servicediscovery/client.py` & `mypy-boto3-servicediscovery-1.28.16/mypy_boto3_servicediscovery/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_servicediscovery.client import ServiceDiscoveryClient
 
     session = Session()
     client: ServiceDiscoveryClient = session.client("servicediscovery")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import CustomHealthStatusType, HealthStatusFilterType
 from .paginator import (
     ListInstancesPaginator,
     ListNamespacesPaginator,
@@ -29,16 +29,15 @@
     CreateHttpNamespaceResponseTypeDef,
     CreatePrivateDnsNamespaceResponseTypeDef,
     CreatePublicDnsNamespaceResponseTypeDef,
     CreateServiceResponseTypeDef,
     DeleteNamespaceResponseTypeDef,
     DeregisterInstanceResponseTypeDef,
     DiscoverInstancesResponseTypeDef,
-    DnsConfigOutputTypeDef,
-    DnsConfigTypeDef,
+    DnsConfigUnionTypeDef,
     EmptyResponseMetadataTypeDef,
     GetInstanceResponseTypeDef,
     GetInstancesHealthStatusResponseTypeDef,
     GetNamespaceResponseTypeDef,
     GetOperationResponseTypeDef,
     GetServiceResponseTypeDef,
     HealthCheckConfigTypeDef,
@@ -185,15 +184,15 @@
     def create_service(
         self,
         *,
         Name: str,
         NamespaceId: str = ...,
         CreatorRequestId: str = ...,
         Description: str = ...,
-        DnsConfig: Union[DnsConfigTypeDef, DnsConfigOutputTypeDef] = ...,
+        DnsConfig: DnsConfigUnionTypeDef = ...,
         HealthCheckConfig: HealthCheckConfigTypeDef = ...,
         HealthCheckCustomConfig: HealthCheckCustomConfigTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         Type: Literal["HTTP"] = ...
     ) -> CreateServiceResponseTypeDef:
         """
         Creates a service.
```

### Comparing `mypy-boto3-servicediscovery-1.28.15.post1/mypy_boto3_servicediscovery/client.pyi` & `mypy-boto3-servicediscovery-1.28.16/mypy_boto3_servicediscovery/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_servicediscovery.client import ServiceDiscoveryClient
 
     session = Session()
     client: ServiceDiscoveryClient = session.client("servicediscovery")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import CustomHealthStatusType, HealthStatusFilterType
 from .paginator import (
     ListInstancesPaginator,
     ListNamespacesPaginator,
@@ -29,16 +29,15 @@
     CreateHttpNamespaceResponseTypeDef,
     CreatePrivateDnsNamespaceResponseTypeDef,
     CreatePublicDnsNamespaceResponseTypeDef,
     CreateServiceResponseTypeDef,
     DeleteNamespaceResponseTypeDef,
     DeregisterInstanceResponseTypeDef,
     DiscoverInstancesResponseTypeDef,
-    DnsConfigOutputTypeDef,
-    DnsConfigTypeDef,
+    DnsConfigUnionTypeDef,
     EmptyResponseMetadataTypeDef,
     GetInstanceResponseTypeDef,
     GetInstancesHealthStatusResponseTypeDef,
     GetNamespaceResponseTypeDef,
     GetOperationResponseTypeDef,
     GetServiceResponseTypeDef,
     HealthCheckConfigTypeDef,
@@ -175,15 +174,15 @@
     def create_service(
         self,
         *,
         Name: str,
         NamespaceId: str = ...,
         CreatorRequestId: str = ...,
         Description: str = ...,
-        DnsConfig: Union[DnsConfigTypeDef, DnsConfigOutputTypeDef] = ...,
+        DnsConfig: DnsConfigUnionTypeDef = ...,
         HealthCheckConfig: HealthCheckConfigTypeDef = ...,
         HealthCheckCustomConfig: HealthCheckCustomConfigTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         Type: Literal["HTTP"] = ...
     ) -> CreateServiceResponseTypeDef:
         """
         Creates a service.
```

### Comparing `mypy-boto3-servicediscovery-1.28.15.post1/mypy_boto3_servicediscovery/literals.py` & `mypy-boto3-servicediscovery-1.28.16/mypy_boto3_servicediscovery/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-servicediscovery-1.28.15.post1/mypy_boto3_servicediscovery/literals.pyi` & `mypy-boto3-servicediscovery-1.28.16/mypy_boto3_servicediscovery/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-servicediscovery-1.28.15.post1/mypy_boto3_servicediscovery/paginator.py` & `mypy-boto3-servicediscovery-1.28.16/mypy_boto3_servicediscovery/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-servicediscovery-1.28.15.post1/mypy_boto3_servicediscovery/paginator.pyi` & `mypy-boto3-servicediscovery-1.28.16/mypy_boto3_servicediscovery/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-servicediscovery-1.28.15.post1/mypy_boto3_servicediscovery/type_defs.py` & `mypy-boto3-servicediscovery-1.28.16/mypy_boto3_servicediscovery/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicediscovery/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_servicediscovery.type_defs import TagTypeDef
 
-    data: TagTypeDef = {...}
+    data: TagTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     CustomHealthStatusType,
     FilterConditionType,
     HealthCheckTypeType,
     HealthStatusFilterType,
     HealthStatusType,
@@ -111,14 +111,15 @@
     "ListServicesRequestRequestTypeDef",
     "PrivateDnsPropertiesMutableChangeTypeDef",
     "PublicDnsPropertiesMutableChangeTypeDef",
     "ServiceChangeTypeDef",
     "ServiceSummaryTypeDef",
     "ServiceTypeDef",
     "CreateServiceRequestRequestTypeDef",
+    "DnsConfigUnionTypeDef",
     "NamespacePropertiesTypeDef",
     "PrivateDnsNamespacePropertiesTypeDef",
     "PublicDnsNamespacePropertiesTypeDef",
     "PrivateDnsNamespacePropertiesChangeTypeDef",
     "PublicDnsNamespacePropertiesChangeTypeDef",
     "UpdateServiceRequestRequestTypeDef",
     "ListServicesResponseTypeDef",
@@ -960,14 +961,15 @@
 
 class CreateServiceRequestRequestTypeDef(
     _RequiredCreateServiceRequestRequestTypeDef, _OptionalCreateServiceRequestRequestTypeDef
 ):
     pass
 
 
+DnsConfigUnionTypeDef = Union[DnsConfigTypeDef, DnsConfigOutputTypeDef]
 NamespacePropertiesTypeDef = TypedDict(
     "NamespacePropertiesTypeDef",
     {
         "DnsProperties": DnsPropertiesTypeDef,
         "HttpProperties": HttpPropertiesTypeDef,
     },
     total=False,
```

### Comparing `mypy-boto3-servicediscovery-1.28.15.post1/mypy_boto3_servicediscovery/type_defs.pyi` & `mypy-boto3-servicediscovery-1.28.16/mypy_boto3_servicediscovery/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicediscovery/type_defs/)
 
 Usage::
 
     ```python
     from mypy_boto3_servicediscovery.type_defs import TagTypeDef
 
-    data: TagTypeDef = {...}
+    data: TagTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     CustomHealthStatusType,
     FilterConditionType,
     HealthCheckTypeType,
     HealthStatusFilterType,
     HealthStatusType,
@@ -110,14 +110,15 @@
     "ListServicesRequestRequestTypeDef",
     "PrivateDnsPropertiesMutableChangeTypeDef",
     "PublicDnsPropertiesMutableChangeTypeDef",
     "ServiceChangeTypeDef",
     "ServiceSummaryTypeDef",
     "ServiceTypeDef",
     "CreateServiceRequestRequestTypeDef",
+    "DnsConfigUnionTypeDef",
     "NamespacePropertiesTypeDef",
     "PrivateDnsNamespacePropertiesTypeDef",
     "PublicDnsNamespacePropertiesTypeDef",
     "PrivateDnsNamespacePropertiesChangeTypeDef",
     "PublicDnsNamespacePropertiesChangeTypeDef",
     "UpdateServiceRequestRequestTypeDef",
     "ListServicesResponseTypeDef",
@@ -929,14 +930,15 @@
 )
 
 class CreateServiceRequestRequestTypeDef(
     _RequiredCreateServiceRequestRequestTypeDef, _OptionalCreateServiceRequestRequestTypeDef
 ):
     pass
 
+DnsConfigUnionTypeDef = Union[DnsConfigTypeDef, DnsConfigOutputTypeDef]
 NamespacePropertiesTypeDef = TypedDict(
     "NamespacePropertiesTypeDef",
     {
         "DnsProperties": DnsPropertiesTypeDef,
         "HttpProperties": HttpPropertiesTypeDef,
     },
     total=False,
```

### Comparing `mypy-boto3-servicediscovery-1.28.15.post1/mypy_boto3_servicediscovery.egg-info/PKG-INFO` & `mypy-boto3-servicediscovery-1.28.16/mypy_boto3_servicediscovery.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-servicediscovery
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.ServiceDiscovery 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.ServiceDiscovery 1.28.16 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicediscovery/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 servicediscovery type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: boto3 servicediscovery type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-servicediscovery.svg?color=blue)](https://pypi.org/project/mypy-boto3-servicediscovery)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicediscovery/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-servicediscovery)](https://pepy.tech/project/mypy-boto3-servicediscovery)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ServiceDiscovery 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery)
+[boto3.ServiceDiscovery 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery)
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
 [mypy-boto3-servicediscovery docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicediscovery/).
 
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
@@ -338,20 +338,20 @@
 )
 
 
 def check_value(value: CustomHealthStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `mypy_boto3_servicediscovery.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from mypy_boto3_servicediscovery.type_defs import (
     TagTypeDef,
     ResponseMetadataTypeDef,
     HealthCheckConfigTypeDef,
     HealthCheckCustomConfigTypeDef,
@@ -419,14 +419,15 @@
     ListServicesRequestRequestTypeDef,
     PrivateDnsPropertiesMutableChangeTypeDef,
     PublicDnsPropertiesMutableChangeTypeDef,
     ServiceChangeTypeDef,
     ServiceSummaryTypeDef,
     ServiceTypeDef,
     CreateServiceRequestRequestTypeDef,
+    DnsConfigUnionTypeDef,
     NamespacePropertiesTypeDef,
     PrivateDnsNamespacePropertiesTypeDef,
     PublicDnsNamespacePropertiesTypeDef,
     PrivateDnsNamespacePropertiesChangeTypeDef,
     PublicDnsNamespacePropertiesChangeTypeDef,
     UpdateServiceRequestRequestTypeDef,
     ListServicesResponseTypeDef,
@@ -441,15 +442,15 @@
     ListNamespacesResponseTypeDef,
     GetNamespaceResponseTypeDef,
     UpdatePrivateDnsNamespaceRequestRequestTypeDef,
     UpdatePublicDnsNamespaceRequestRequestTypeDef,
 )
 
 
-def get_structure() -> TagTypeDef:
+def get_value() -> TagTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-servicediscovery-1.28.15.post1/mypy_boto3_servicediscovery.egg-info/SOURCES.txt` & `mypy-boto3-servicediscovery-1.28.16/mypy_boto3_servicediscovery.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-servicediscovery-1.28.15.post1/setup.py` & `mypy-boto3-servicediscovery-1.28.16/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-servicediscovery",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_servicediscovery"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ServiceDiscovery 1.28.15 service generated with"
-        " mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.ServiceDiscovery 1.28.16 service generated with"
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
-    keywords="boto3 servicediscovery type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="boto3 servicediscovery type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_servicediscovery": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicediscovery/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

